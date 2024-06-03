# Comparing `tmp/rwkv_tokenizer-0.2.0.tar.gz` & `tmp/rwkv_tokenizer-0.3.0.tar.gz`

## Comparing `rwkv_tokenizer-0.2.0.tar` & `rwkv_tokenizer-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 rwkv_tokenizer-0.2.0/Cargo.toml
--rw-r--r--   0      501       20     3526 2024-05-29 11:45:26.000000 rwkv_tokenizer-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0      501       20      686 2024-05-29 11:45:26.000000 rwkv_tokenizer-0.2.0/.gitignore
--rw-r--r--   0      501       20       17 2024-05-29 13:34:05.000000 rwkv_tokenizer-0.2.0/README.md
--rw-r--r--   0      501       20     1851 2024-05-31 12:36:16.000000 rwkv_tokenizer-0.2.0/src/lib.rs
--rw-r--r--   0      501       20  1093733 2024-05-29 13:15:51.000000 rwkv_tokenizer-0.2.0/src/rwkv_vocab_v20230424.txt
--rw-r--r--   0      501       20     2459 2024-05-31 14:47:02.000000 rwkv_tokenizer-0.2.0/src/trie.rs
--rw-r--r--   0      501       20      713 2024-05-30 10:38:37.000000 rwkv_tokenizer-0.2.0/test/comparison.rs
--rw-r--r--   0      501       20     9458 2024-05-31 14:54:04.000000 rwkv_tokenizer-0.2.0/Cargo.lock
--rw-r--r--   0      501       20      394 2024-05-29 11:45:26.000000 rwkv_tokenizer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 rwkv_tokenizer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 rwkv_tokenizer-0.3.0/Cargo.toml
+-rw-r--r--   0      501       20     3526 2024-05-29 11:45:26.000000 rwkv_tokenizer-0.3.0/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      686 2024-05-29 11:45:26.000000 rwkv_tokenizer-0.3.0/.gitignore
+-rw-r--r--   0      501       20     1001 2024-06-02 17:37:38.000000 rwkv_tokenizer-0.3.0/README.md
+-rw-r--r--   0      501       20     2480 2024-06-03 12:29:18.000000 rwkv_tokenizer-0.3.0/src/lib.rs
+-rw-r--r--   0      501       20  1093733 2024-05-29 13:15:51.000000 rwkv_tokenizer-0.3.0/src/rwkv_vocab_v20230424.txt
+-rw-r--r--   0      501       20     2502 2024-06-03 12:28:24.000000 rwkv_tokenizer-0.3.0/src/trie.rs
+-rw-r--r--   0      501       20      713 2024-05-30 10:38:37.000000 rwkv_tokenizer-0.3.0/test/comparison.rs
+-rw-r--r--   0      501       20     9458 2024-06-03 12:39:59.000000 rwkv_tokenizer-0.3.0/Cargo.lock
+-rw-r--r--   0      501       20      394 2024-05-29 11:45:26.000000 rwkv_tokenizer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 rwkv_tokenizer-0.3.0/PKG-INFO
```

### Comparing `rwkv_tokenizer-0.2.0/.github/workflows/CI.yml` & `rwkv_tokenizer-0.3.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rwkv_tokenizer-0.2.0/.gitignore` & `rwkv_tokenizer-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rwkv_tokenizer-0.2.0/src/lib.rs` & `rwkv_tokenizer-0.3.0/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -21,25 +21,32 @@
         let mut tokenizer = Tokenizer {
             tokens: Vec::new(),
             trie: Trie::new()
         };
         let file = File::open(filename)?;
         let reader = io::BufReader::new(file);
 
-        let re = Regex::new(r"(\d+)\s+b?(.+)\s+(\d+)").unwrap();
+        let re = Regex::new(r"(\d+)\s+(b?)(.+)\s+(\d+)").unwrap();
         tokenizer.tokens.push("".to_string());
         for line in reader.lines() {
             let line = line?;
             if let Some(captures) = re.captures(&line) {
                 let id = captures[1].parse::<u16>().unwrap();
-                let mut string = captures[2].to_string();
-                let _length = captures[3].parse::<usize>().unwrap();
+                let is_byte = captures[2].to_string();
+                let _length = captures[4].parse::<usize>().unwrap();
+                let mut string: String = captures[3].to_string();
                 string = string[1..string.len()-1].parse().unwrap();
-                let string = unescape(string.as_str()).unwrap();
-                tokenizer.trie.insert(string.as_str(), id);
+                let sbytes: Vec<u8>;
+                if is_byte.len() == 0 {
+                    string = unescape(string.as_str()).unwrap();
+                    sbytes = string.clone().into_bytes();
+                } else {
+                    sbytes = hex_to_bytes(string.as_str()).unwrap();
+                }
+                tokenizer.trie.insert(&sbytes, id);
                 tokenizer.tokens.push(string.to_string());
             }
             else {
                 println!("Line with issue: {:?}", line)
             }
         }
         Ok(tokenizer)
@@ -54,12 +61,25 @@
         for index in vec.iter() {
             result.push_str(&*self.tokens[*index as usize]);
         }
         return result;
     }
 }
 
+fn hex_to_bytes(hex: &str) -> Option<Vec<u8>> {
+    let hex = hex.replace("\\x", "");
+    if hex.len() % 2 == 0 {
+        (0..hex.len())
+            .step_by(2)
+            .map(|i| hex.get(i..i + 2)
+                .and_then(|sub| u8::from_str_radix(sub, 16).ok()))
+            .collect()
+    } else {
+        None
+    }
+}
+
 #[pymodule]
 fn rwkv_tokenizer(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<Tokenizer>()?;
     Ok(())
 }
```

### Comparing `rwkv_tokenizer-0.2.0/src/rwkv_vocab_v20230424.txt` & `rwkv_tokenizer-0.3.0/src/rwkv_vocab_v20230424.txt`

 * *Files identical despite different names*

### Comparing `rwkv_tokenizer-0.2.0/src/trie.rs` & `rwkv_tokenizer-0.3.0/src/trie.rs`

 * *Files 8% similar despite different names*

```diff
@@ -27,35 +27,35 @@
 impl Trie {
     pub(crate) fn new() -> Self {
         Trie {
             root: TrieNode::new(),
         }
     }
 
-    pub(crate) fn insert(&mut self, word: &str, id: u16) {
+    pub(crate) fn insert(&mut self, word: &Vec<u8>, id: u16) {
         let mut node = &mut self.root;
-        for ch in word.bytes() {
-            if node.children[ch as usize].is_none() {
-                node.children[ch as usize] = Option::from(TrieNode::new());
+        for ch in word {
+            if node.children[u8::from_be(*ch) as usize].is_none() {
+                node.children[u8::from_be(*ch) as usize] = Option::from(TrieNode::new());
             }
-            match &mut node.children[ch as usize] {
+            match &mut node.children[u8::from_be(*ch) as usize] {
                 Some(next_node) => node = next_node,
                 None => unreachable!(),  // We've just checked that it's not None
             }
         }
         node.id = id
     }
 
-    fn search_the_longest(&self, word: &str) -> (u16, u16) {
+    fn search_the_longest(&self, word: &[u8]) -> (u16, u16) {
         let mut node = &self.root;
         let mut old_node: &TrieNode = &self.root;
         let mut index = 0;
         let mut old_index = 0;
-        for ch in word.bytes() {
-            if let Some(next_node) = &node.children[ch as usize] {
+        for ch in word {
+            if let Some(next_node) = &node.children[*ch as usize] {
                 if node.id != 0 {
                     old_node = node;
                     old_index = index;
                 }
                 node = &next_node;
                 index += 1;
             } else {
@@ -76,15 +76,15 @@
     }
 
     pub(crate) fn tokenize(&self, text: &str) -> Vec<u16> {
         let mut vec: Vec<u16> = Vec::new();
         let text_length = text.len();
         let mut index: usize = 0;
         loop {
-            let result = self.search_the_longest(&text[index..]);
+            let result = self.search_the_longest(&text.as_bytes()[index..]);
             if result.0 != 0 {
                 vec.push(result.1.into());
                 index += <u16 as Into<usize>>::into(result.0);
             } else {
                 return vec;
             }
             if index >= text_length {
```

### Comparing `rwkv_tokenizer-0.2.0/test/comparison.rs` & `rwkv_tokenizer-0.3.0/test/comparison.rs`

 * *Files identical despite different names*

### Comparing `rwkv_tokenizer-0.2.0/Cargo.lock` & `rwkv_tokenizer-0.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rwkv_tokenizer"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "pyo3",
  "regex",
  "unescape",
 ]
 
 [[package]]
```

