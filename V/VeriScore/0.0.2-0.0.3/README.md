# Comparing `tmp/veriscore-0.0.2.tar.gz` & `tmp/veriscore-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veriscore-0.0.2.tar", last modified: Fri May 31 18:43:36 2024, max compression
+gzip compressed data, was "veriscore-0.0.3.tar", last modified: Mon Jun  3 06:40:13 2024, max compression
```

## Comparing `veriscore-0.0.2.tar` & `veriscore-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-31 18:43:36.448060 veriscore-0.0.2/
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     1068 2024-05-21 17:48:27.000000 veriscore-0.0.2/LICENSE
--rw-r--r--   0 yekyungkim (32790) yekyungkim (32790)      522 2024-05-31 18:43:36.448060 veriscore-0.0.2/PKG-INFO
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       11 2024-05-21 17:48:27.000000 veriscore-0.0.2/README.md
-drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-31 18:43:36.448060 veriscore-0.0.2/VeriScore.egg-info/
--rw-r--r--   0 yekyungkim (32790) yekyungkim (32790)      522 2024-05-31 18:43:36.000000 veriscore-0.0.2/VeriScore.egg-info/PKG-INFO
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      391 2024-05-31 18:43:36.000000 veriscore-0.0.2/VeriScore.egg-info/SOURCES.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)        1 2024-05-31 18:43:36.000000 veriscore-0.0.2/VeriScore.egg-info/dependency_links.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       31 2024-05-31 18:43:36.000000 veriscore-0.0.2/VeriScore.egg-info/requires.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       10 2024-05-31 18:43:36.000000 veriscore-0.0.2/VeriScore.egg-info/top_level.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       38 2024-05-31 18:43:36.448060 veriscore-0.0.2/setup.cfg
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      685 2024-05-31 18:42:29.000000 veriscore-0.0.2/setup.py
-drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-31 18:43:36.448060 veriscore-0.0.2/veriscore/
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     6857 2024-05-22 19:10:56.000000 veriscore-0.0.2/veriscore/ClaimExtractor.py
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     4003 2024-05-22 19:10:56.000000 veriscore-0.0.2/veriscore/GetResponse.py
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     3315 2024-05-22 19:10:56.000000 veriscore-0.0.2/veriscore/SearchAPI.py
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       22 2024-05-31 18:42:25.000000 veriscore-0.0.2/veriscore/__init__.py
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)    26609 2024-05-22 19:10:56.000000 veriscore-0.0.2/veriscore/claim_extraction_prompt_utils.py
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     2006 2024-05-22 19:10:56.000000 veriscore-0.0.2/veriscore/evidence_retrieval.py
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     7023 2024-05-22 19:10:56.000000 veriscore-0.0.2/veriscore/extract_claims.py
+drwxrwsr-x   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)        0 2024-06-03 06:40:13.056623 veriscore-0.0.3/
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)     1068 2024-05-21 17:48:27.000000 veriscore-0.0.3/LICENSE
+-rw-r--r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)      543 2024-06-03 06:40:13.051867 veriscore-0.0.3/PKG-INFO
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)       11 2024-05-21 17:48:27.000000 veriscore-0.0.3/README.md
+drwxrwsr-x   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)        0 2024-06-03 06:40:13.046189 veriscore-0.0.3/VeriScore.egg-info/
+-rw-r--r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)      543 2024-06-03 06:40:12.000000 veriscore-0.0.3/VeriScore.egg-info/PKG-INFO
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)      429 2024-06-03 06:40:12.000000 veriscore-0.0.3/VeriScore.egg-info/SOURCES.txt
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)        1 2024-06-03 06:40:12.000000 veriscore-0.0.3/VeriScore.egg-info/dependency_links.txt
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)       37 2024-06-03 06:40:12.000000 veriscore-0.0.3/VeriScore.egg-info/requires.txt
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)       10 2024-06-03 06:40:12.000000 veriscore-0.0.3/VeriScore.egg-info/top_level.txt
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)       38 2024-06-03 06:40:13.057968 veriscore-0.0.3/setup.cfg
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)      700 2024-06-03 06:35:16.000000 veriscore-0.0.3/setup.py
+drwxrwsr-x   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)        0 2024-06-03 06:40:13.041023 veriscore-0.0.3/veriscore/
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)       22 2024-06-03 06:35:16.000000 veriscore-0.0.3/veriscore/__init__.py
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)     7042 2024-06-03 06:11:04.000000 veriscore-0.0.3/veriscore/claim_extractor.py
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)     5002 2024-06-03 06:11:04.000000 veriscore-0.0.3/veriscore/claim_verifier.py
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)     3757 2024-06-03 06:11:04.000000 veriscore-0.0.3/veriscore/extract_claims.py
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)     3839 2024-06-03 06:36:16.000000 veriscore-0.0.3/veriscore/get_response.py
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)     2036 2024-06-03 06:11:04.000000 veriscore-0.0.3/veriscore/retrieval_evidence.py
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)     3123 2024-06-03 06:11:04.000000 veriscore-0.0.3/veriscore/search_API.py
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)     2136 2024-06-03 06:11:04.000000 veriscore-0.0.3/veriscore/verify_claims.py
+-rw-rw-r--   0 yekyungkim_umass_edu  (2662) pi_miyyer_umass_edu (10067)     8287 2024-06-03 06:33:47.000000 veriscore-0.0.3/veriscore/veriscore.py
```

### Comparing `veriscore-0.0.2/LICENSE` & `veriscore-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `veriscore-0.0.2/PKG-INFO` & `veriscore-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: VeriScore
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pip package for Verifact
 Home-page: https://github.com/mungg/VeriScore
 Author: Yixio Song
 Author-email: yixiaosong@umass.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: spacy
 Requires-Dist: openai
 Requires-Dist: anthropic
 Requires-Dist: tiktoken
 Requires-Dist: tqdm
 
 # VeriScore
```

### Comparing `veriscore-0.0.2/VeriScore.egg-info/PKG-INFO` & `veriscore-0.0.3/VeriScore.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: VeriScore
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pip package for Verifact
 Home-page: https://github.com/mungg/VeriScore
 Author: Yixio Song
 Author-email: yixiaosong@umass.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: spacy
 Requires-Dist: openai
 Requires-Dist: anthropic
 Requires-Dist: tiktoken
 Requires-Dist: tqdm
 
 # VeriScore
```

### Comparing `veriscore-0.0.2/setup.py` & `veriscore-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
    name="VeriScore",
-   version="0.0.2",
+   version="0.0.3",
    packages=find_packages(),
    install_requires=[
        #'requests', 'numpy'
+      'spacy',
       'openai',
       'anthropic',
       'tiktoken',
       'tqdm'
    ],
    author="Yixio Song",
    author_email="yixiaosong@umass.edu",
```

### Comparing `veriscore-0.0.2/veriscore/ClaimExtractor.py` & `veriscore-0.0.3/veriscore/claim_extractor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import regex
 import pdb
 import json
 import spacy
 from tqdm import tqdm
-from .GetResponse import GetResponse
-from .claim_extraction_prompt_utils import non_qa_prompt_temp, qa_prompt_temp
+from .get_response import GetResponse
+
 
 class ClaimExtractor():
-    def __init__(self, model_name, input_file_name, cache_dir):
+    def __init__(self, model_name, cache_dir="./data/cache/"):
         cache_dir = os.path.join(cache_dir, model_name)
         os.makedirs(cache_dir, exist_ok=True)
-        self.cache_file = os.path.join(cache_dir, f"response_decompose_cache_{input_file_name}.json")
+        self.cache_file = os.path.join(cache_dir, f"claim_extraction_cache.json")
         self.spacy_nlp = spacy.load('en_core_web_sm')
         self.get_model_response = GetResponse(cache_file=self.cache_file,
                                               model_name=model_name,
                                               max_tokens=1000,
                                               temperature=0)
         self.system_message = "You are a helpful assistant who can extract verifiable atomic claims from a piece of text. Each atomic fact should be verifiable against reliable external world knowledge (e.g., via Wikipedia)"
 
@@ -34,28 +34,29 @@
         all_facts_lst = []
         # keep track of token counts
         prompt_tok_cnt, response_tok_cnt = 0, 0
         for para in paragraph_lst:
             # split the text into sentences using spaCy
             sentences = self.get_sentence(para)
             for i in range(len(sentences)):
-                lead_sent = sentences[0] # 1st sentence of the para
+                lead_sent = sentences[0]  # 1st sentence of the para
                 context1 = " ".join(sentences[max(0, i - 3):i])
                 sentence = f"<SOS>{sentences[i].strip()}<EOS>"
-                context2 = " ".join(sentences[i+1:i+2])
+                context2 = " ".join(sentences[i + 1:i + 2])
 
                 # if the para is not long
                 if len(sentences) <= 5:
                     snippet = f"{context1.strip()} {sentence.strip()} {context2.strip()}".strip()
                 # if the para is long, add lead sentence to context1
                 else:
                     snippet = f"{lead_sent.strip()} {context1.strip()} {sentence.strip()} {context2.strip()}".strip()
 
                 # call fact_extractor on each snippet
-                facts, prompt_tok_num, response_tok_num = self.fact_extractor(snippet, sentences[i].strip(), qa_input = False)
+                facts, prompt_tok_num, response_tok_num = self.fact_extractor(snippet, sentences[i].strip(),
+                                                                              qa_input=False)
 
                 # update token counts
                 prompt_tok_cnt += prompt_tok_num
                 response_tok_cnt += response_tok_num
 
                 if facts == None:
                     continue
@@ -65,21 +66,21 @@
                     if fact.strip() == "":
                         continue
                     # cases where GPT returns its justification
                     elif fact.startswith("Note:"):
                         continue
                     elif fact not in all_facts_lst:
                         all_facts_lst.append(fact)
-        
+
         print(f"Returning facts and token counts for the whole response ...")
         if all_facts_lst == None:
             return None, prompt_tok_cnt, response_tok_cnt
         else:
             return all_facts_lst, prompt_tok_cnt, response_tok_cnt
-        
+
     def qa_scanner_extractor(self, question, response):
         """
         Given a model output to a question
         - split the response into sentences using spaCy
         - snippet = question (context1 = 0-3 sentence) <SOS>Sent<EOS> (context2 = 0-1 sentence)
         - call fact_extractor on each snippet
         """
@@ -97,16 +98,16 @@
             context2 = " ".join(sentences[i + 1:i + 2])
 
             snippet = f"Question: {question.strip()}\nResponse: {context1.strip()} {sentence.strip()} {context2.strip()}".strip()
             # new return value
             snippet_lst.append(snippet)
 
             # call fact_extractor on each tesnippetxt
-            facts, prompt_tok_num, response_tok_num = self.fact_extractor(snippet, sentences[i].strip(), qa_input = True)
-            
+            facts, prompt_tok_num, response_tok_num = self.fact_extractor(snippet, sentences[i].strip(), qa_input=True)
+
             # update token counts
             prompt_tok_cnt += prompt_tok_num
             response_tok_cnt += response_tok_num
 
             if facts == None:
                 fact_lst_lst.append([None])
                 continue
@@ -120,34 +121,39 @@
                 elif fact.startswith("Note:"):
                     continue
                 elif fact not in all_facts_lst:
                     all_facts_lst.append(fact.strip())
                 fact_lst.append(fact.strip())
             fact_lst_lst.append(fact_lst)
         print(f"Returning facts and token counts for the whole response ...")
-        # if all_facts_lst == None:
-        #     return None, prompt_tok_cnt, response_tok_cnt
-        # else:
-        #     return all_facts_lst, prompt_tok_cnt, response_tok_cnt
+
         return snippet_lst, fact_lst_lst, all_facts_lst, prompt_tok_cnt, response_tok_cnt
 
     def get_sentence(self, text):
         # use spaCy to split the text into sentences
         return [x.text.strip() for x in self.spacy_nlp(text).sents]
-    
-    def fact_extractor(self, snippet, sentence, qa_input = False):
+
+    def get_prompt_template(self, qa_input):
+        if qa_input:
+            prompt_template = open("./prompt/extraction_qa_template.txt", "r").read()
+        else:
+            prompt_template = open("./prompt/extraction_non_qa_template.txt", "r").read()
+        return prompt_template
+
+    def fact_extractor(self, snippet, sentence, qa_input=False):
         """
         snippet = (context1) <SOS>sentence<EOS> (context2)
         sentence = the sentence to be focused on
         """
-        prompt_template = qa_prompt_temp if qa_input else non_qa_prompt_temp
+        prompt_template = self.get_prompt_template(qa_input)  # qa_prompt_temp if qa_input else non_qa_prompt_temp
         prompt_text = prompt_template.format(snippet=snippet, sentence=sentence)
-        response, prompt_tok_cnt, response_tok_cnt = self.get_model_response.get_response(self.system_message, prompt_text)
+        response, prompt_tok_cnt, response_tok_cnt = self.get_model_response.get_response(self.system_message,
+                                                                                          prompt_text)
 
         if "No verifiable claim." in response:
             return None, prompt_tok_cnt, response_tok_cnt
         else:
             # remove itemized list
             facts = [x.strip().replace("- ", "") for x in response.split("\n")]
             # remove numbers in the beginning
             facts = [regex.sub(r"^\d+\.?\s", "", x) for x in facts]
-            return facts, prompt_tok_cnt, response_tok_cnt
+            return facts, prompt_tok_cnt, response_tok_cnt
```

### Comparing `veriscore-0.0.2/veriscore/GetResponse.py` & `veriscore-0.0.3/veriscore/get_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import pdb
 import json
 import tiktoken
 from openai import OpenAI
 from anthropic import Anthropic
 
+
 class GetResponse():
     # OpenAI model list: https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo
     # Claude3 model list: https://www.anthropic.com/claude
     # "claude-3-opus-20240229", gpt-4-0125-preview
     def __init__(self, cache_file, model_name="gpt-4-0125-preview", max_tokens=1000, temperature=0):
         self.model_name = model_name
         self.max_tokens = max_tokens
@@ -31,56 +32,55 @@
         self.save_interval = 20
 
     # Returns the response from the model given a system message and a prompt text.
     def get_response(self, system_message, prompt_text):
         # check if prompt is in cache; if so, return from cache
         cache_key = prompt_text.strip()
         if cache_key in self.cache_dict:
-            print("Getting response from cache ...")
             return self.cache_dict[cache_key], 0, 0
-        
+
         # Example message: "You are a helpful assistant who can extract verifiable atomic claims from a piece of text."
         if "gpt" in self.model_name:
             message = [{"role": "system", "content": system_message},
                        {"role": "user", "content": prompt_text}]
             response = self.client.chat.completions.create(
-                        model=self.model_name,
-                        messages=message,
-                        max_tokens=self.max_tokens,
-                        temperature=self.temperature,
-                        seed=self.seed,
-                        )
+                model=self.model_name,
+                messages=message,
+                max_tokens=self.max_tokens,
+                temperature=self.temperature,
+                seed=self.seed,
+            )
             response_content = response.choices[0].message.content.strip()
         elif "claude" in self.model_name:
             response = self.client.messages.create(
-                        model=self.model_name,
-                        messages=[{"role": "user", "content": prompt_text}],
-                        temperature=self.temperature,
-                        max_tokens=self.max_tokens
-                        )
+                model=self.model_name,
+                messages=[{"role": "user", "content": prompt_text}],
+                temperature=self.temperature,
+                max_tokens=self.max_tokens
+            )
             response_content = response.content[0].text.strip()
 
         # update cache
         self.cache_dict[cache_key] = response_content.strip()
         self.add_n += 1
 
         # save cache every save_interval times
         if self.add_n % self.save_interval == 0:
             self.save_cache()
 
         # count tokens in prompt and response
         prompt_tokens = len(self.tokenizer.encode(prompt_text))
         response_tokens = len(self.tokenizer.encode(response_content))
         return response_content, prompt_tokens, response_tokens
-    
+
     # Returns the number of tokens in a text string.
     def tok_count(self, text: str) -> int:
         num_tokens = len(self.tokenizer.encode(text))
         return num_tokens
-    
+
     def save_cache(self):
         # load the latest cache first, since if there were other processes running in parallel, cache might have been updated
         for k, v in self.load_cache().items():
             self.cache_dict[k] = v
         print(f"Saving cache to {self.cache_file}...")
         with open(self.cache_file, "w") as f:
             json.dump(self.cache_dict, f, indent=4)
```

### Comparing `veriscore-0.0.2/veriscore/SearchAPI.py` & `veriscore-0.0.3/veriscore/search_API.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,89 +1,87 @@
 import os
 from ast import literal_eval
 import pdb
 import json
 import requests
 from tqdm import tqdm
 
+
 class SearchAPI():
     def __init__(self):
         # invariant variables
         self.serper_key = os.getenv("SERPER_KEY_PRIVATE")
-        self.serper_key = os.getenv("SERPER_KEY")
         self.url = "https://google.serper.dev/search"
         self.headers = {'X-API-KEY': self.serper_key,
                         'Content-Type': 'application/json'}
-        # # cache related
-        # self.cache_file = "fine_tune_code_data/data/run_ft-ed_models_on_110_datapoints/cache"
-        # self.cache_dict = self.load_cache()
-        # self.add_n = 0
-        # self.save_interval = 10
+        # cache related
+        self.cache_file = "data/cache/search_cache.json"
+        self.cache_dict = self.load_cache()
+        self.add_n = 0
+        self.save_interval = 10
 
     def get_snippets(self, claim_lst):
         text_claim_snippets_dict = {}
         for query in claim_lst:
             search_result = self.get_search_res(query)
+            if "statusCode" in search_result:  # and search_result['statusCode'] == 403:
+                print(search_result['message'])
+                exit()
             if "organic" in search_result:
                 organic_res = search_result["organic"]
             else:
                 organic_res = []
 
             search_res_lst = []
             for item in organic_res:
                 title = item["title"] if "title" in item else ""
                 snippet = item["snippet"] if "snippet" in item else ""
                 link = item["link"] if "link" in item else ""
 
-                search_res_lst.append({"title": title, 
-                                       "snippet": snippet, 
+                search_res_lst.append({"title": title,
+                                       "snippet": snippet,
                                        "link": link})
             text_claim_snippets_dict[query] = search_res_lst
         return text_claim_snippets_dict
 
     def get_search_res(self, query):
-        # # check if prompt is in cache; if so, return from cache
-        # cache_key = query.strip()
-        # if cache_key in self.cache_dict:
-        #     print("Getting search results from cache ...")
-        #     return self.cache_dict[cache_key]
+        # check if prompt is in cache; if so, return from cache
+        cache_key = query.strip()
+        if cache_key in self.cache_dict:
+            # print("Getting search results from cache ...")
+            return self.cache_dict[cache_key]
 
-        payload = json.dumps({"q": query, "autocorrect": False})
+        payload = json.dumps({"q": query})
         response = requests.request("POST",
                                     self.url,
                                     headers=self.headers,
                                     data=payload)
-        # pdb.set_trace()
-        # response_json = literal_eval(response.text)
-        try:
-            response_json = json.loads(response.text)
-        except json.JSONDecodeError as e:
-            print(f"Error: {e}")
-
-        # # update cache
-        # self.cache_dict[query.strip()] = response_json
-        # self.add_n += 1
-
-        # # save cache every save_interval times
-        # if self.add_n % self.save_interval == 0:
-        #     self.save_cache()
-        
+        response_json = literal_eval(response.text)
+
+        # update cache
+        self.cache_dict[query.strip()] = response_json
+        self.add_n += 1
+
+        # save cache every save_interval times
+        if self.add_n % self.save_interval == 0:
+            self.save_cache()
+
         return response_json
 
-    # def save_cache(self):
-    #     # load the latest cache first, since if there were other processes running in parallel, cache might have been updated
-    #     cache = self.load_cache().items()
-    #     for k, v in cache:
-    #         self.cache_dict[k] = v
-    #     print(f"Saving search cache ...")
-    #     with open(self.cache_file, "w") as f:
-    #         json.dump(self.cache_dict, f, indent=4)
-
-    # def load_cache(self):
-    #     if os.path.exists(self.cache_file):
-    #         with open(self.cache_file, "r") as f:
-    #             # load a json file
-    #             cache = json.load(f)
-    #             print(f"Loading cache ...")
-    #     else:
-    #         cache = {}
-    #     return cache
+    def save_cache(self):
+        # load the latest cache first, since if there were other processes running in parallel, cache might have been updated
+        cache = self.load_cache().items()
+        for k, v in cache:
+            self.cache_dict[k] = v
+        print(f"Saving search cache ...")
+        with open(self.cache_file, "w") as f:
+            json.dump(self.cache_dict, f, indent=4)
+
+    def load_cache(self):
+        if os.path.exists(self.cache_file):
+            with open(self.cache_file, "r") as f:
+                # load a json file
+                cache = json.load(f)
+                print(f"Loading cache ...")
+        else:
+            cache = {}
+        return cache
```

### Comparing `veriscore-0.0.2/veriscore/evidence_retrieval.py` & `veriscore-0.0.3/veriscore/retrieval_evidence.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 import os
 import pdb
 import json
 import random
 import argparse
 from tqdm import tqdm
-from SearchAPI import SearchAPI
+from .search_API import SearchAPI
 
-# add argparse argument
-parser = argparse.ArgumentParser()
-parser.add_argument("--multiple", type=str, default="5")
-args = parser.parse_args()
-
-"""
-Read in extracted claim file
-"""
-begin = 400 * (int(args.multiple) - 1)
-end = 400 * int(args.multiple)
-
-file_dir = f"fine_tune_code_data/data/run_ft-ed_models_on_110_datapoints/4800_response_claim_extracted/merged_sampled_data_4800_extracted_{begin}_{end}.jsonl"
-
-"""
-Get search results for each claim
-Store as a dictionary {claim: {"search_results": [search_results]}}
-"""
-# initialize search api
-fetch_search = SearchAPI()
-
-# read in extracted claim data
-with open(file_dir, "r") as f:
-    data = [json.loads(x) for x in f.readlines()]
-
-# set up output directory
-out_dir = f"fine_tune_code_data/data/run_ft-ed_models_on_110_datapoints/4800_response_claim_extracted_w_evidence/merged_sampled_data_4800_extracted_{begin}_{end}_searched.jsonl"
-os.makedirs(os.path.dirname(out_dir), exist_ok=True)
-
-# get the pick up point
-try:
-    with open(out_dir, "r") as f:
-        pick_up_point = len(f.readlines())
-        print(f"Pick up point: {pick_up_point}")
-except:
-    pick_up_point = 0
-    print("No pick up point")
-    pass
-
-# iterate through each data point and get search results
-print(f"Begin{begin} End{end} Multiple {args.multiple}")
-with open(out_dir, "a+") as f:
-    for dict_item in tqdm(data[pick_up_point:]):
-        if dict_item['abstained'] == True:
-            f.write(json.dumps(dict_item) + "\n")
-            continue
-        
-        claim_lst = dict_item["all_claim_lst"]
-        if claim_lst == ["No verifiable claim."]:
-            dict_item["claim_srch_res_lst"] = []
-            f.write(json.dumps(dict_item) + "\n")
-            continue
-        claim_snippets = fetch_search.get_snippets(claim_lst)
-        dict_item["claim_srch_res_lst"] = claim_snippets
+if __name__ == '__main__':
 
-        f.write(json.dumps(dict_item) + "\n")
-        f.flush()
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--data_dir", type=str, default='./data')
+    parser.add_argument("--input_file", type=str, required=True)
+    parser.add_argument("--output_dir", type=str, default='./data')
+    args = parser.parse_args()
+
+    """
+    Get search results for each claim
+    Store as a dictionary {claim: {"search_results": [search_results]}}
+    """
+    # initialize search api
+    fetch_search = SearchAPI()
+
+    input_file_name = "".join(args.input_file.split('.')[:-1])
+    input_path = os.path.join(args.data_dir, args.input_file)
+
+    # read in extracted claim data
+    with open(input_path, "r") as f:
+        data = [json.loads(x) for x in f.readlines()]
+
+    output_dir = args.output_dir
+    output_file = f"evidence_{input_file_name}.jsonl"
+    output_path = os.path.join(output_dir, output_file)
+    os.makedirs(os.path.dirname(output_dir), exist_ok=True)
+
+    # get the pick up point
+    # try:
+    #     with open(output_path, "r") as f:
+    #         pick_up_point = len(f.readlines())
+    #         print(f"Pick up point: {pick_up_point}")
+    # except:
+    #     pick_up_point = 0
+    #     print("No pick up point")
+    #     pass
+
+    # iterate through each data point and get search results
+    with open(output_path, "w") as f:
+        for dict_item in tqdm(data):
+            if dict_item['abstained']:
+                f.write(json.dumps(dict_item) + "\n")
+                continue
+
+            claim_lst = dict_item["all_claim_lst"]
+            if claim_lst == ["No verifiable claim."]:
+                dict_item["claim_snippets_dict"] = []
+                f.write(json.dumps(dict_item) + "\n")
+                continue
+            claim_snippets = fetch_search.get_snippets(claim_lst)
+            dict_item["claim_snippets_dict"] = claim_snippets
+
+            f.write(json.dumps(dict_item) + "\n")
+            f.flush()
```

### Comparing `veriscore-0.0.2/veriscore/extract_claims.py` & `veriscore-0.0.3/veriscore/veriscore.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,88 +1,21 @@
 """
 This script is written to extract claims from the model responses.
 model generations: /data/yixiao/atomic_claims/data/model_generation_decomposition/model_generations
 """
 
 import os
-import pdb
 import json
 import argparse
+import spacy
 from tqdm import tqdm
-from .ClaimExtractor import ClaimExtractor
-#
-# args = argparse.ArgumentParser()
-# args.add_argument("--input_file", type=str, required=True)
-# args = args.parse_args()
-#
-# input_file_names = ['Mistral-7B-Instruct-v0.1',
-#                     'Mistral-7B-Instruct-v0.2',
-#                     'Mixtral-8x7B-Instruct-v0.1',
-#                     'Mixtral-8x22B-Instruct-v0.1',
-#                     'gpt-4-0125-preview',
-#                     'gpt-3.5-turbo-1106',
-#                     'gpt-3.5-turbo-0613',
-#                     'claude-3-opus-20240229',
-#                     'claude-3-sonnet-20240229',
-#                     'claude-3-haiku-20240307',
-#                     'dbrx-instruct',
-#                     'OLMo-7B-Instruct', ]
-#
-# abstain_responses = ["I'm sorry, I cannot fulfill that request.",
-#                      "I'm sorry, I can't fulfill that request.",
-#                      "I'm sorry, but I cannot fulfill that request.",
-#                      "I'm sorry, but I can't fulfill that request.",
-#                      "Sorry, but I can't fulfill that request.",
-#                      "Sorry, I can't do that."]
-#
-# # read data
-# input_file_name = args.input_file
-# assert input_file_name in input_file_names
-# input_file_dir = f"data/model_generation_decomposition/model_generations/data_{input_file_name}.jsonl"
-# with open(input_file_dir, "r") as f:
-#     data = [json.loads(x) for x in f.readlines() if x.strip()]
-#
-# # initialize objects
-# model_name = "gpt-4-0125-preview"
-# claim_extractor = ClaimExtractor(model_name, input_file_name)
-#
-# output_dir = f"data/model_generation_decomposition/decomposed_responses/claims_{input_file_name}.jsonl"
-# with open(output_dir, "a+") as f:
-#     for dict_item in tqdm(data[1558:]):
-#         # get necessary info
-#         question = dict_item["question"]
-#         response = dict_item["response"]
-#         prompt_source = dict_item["prompt_source"]
-#         model = dict_item["model"]
-#
-#         # skip abstained responses
-#         if response.strip() in abstain_responses:
-#             output_dict = {"question": question.strip(),
-#                            "response": response.strip(),
-#                            "abstained": True,
-#                            "prompt_source": prompt_source,
-#                            "model": model,}
-#             f.write(json.dumps(output_dict) + "\n")
-#             continue
-#
-#         # extract claims
-#         snippet_lst, fact_lst_lst, all_facts_lst, prompt_tok_cnt, response_tok_cnt = claim_extractor.qa_scanner_extractor(question, response)
-#
-#         # write output
-#         output_dict = {"question": question.strip(),
-#                        "response": response.strip(),
-#                        "abstained": False, # "abstained": False, "abstained": True
-#                        "snippet_lst": snippet_lst,
-#                        "fact_lst_lst": fact_lst_lst,
-#                        "all_facts_lst": all_facts_lst,
-#                        "prompt_tok_cnt": prompt_tok_cnt,
-#                        "response_tok_cnt": response_tok_cnt,
-#                        "prompt_source": prompt_source,
-#                        "model": model,}
-#         f.write(json.dumps(output_dict) + "\n")
+from .claim_extractor import ClaimExtractor
+from .search_API import SearchAPI
+from .claim_verifier import ClaimVerifier
+
 
 input_file_names = ['Mistral-7B-Instruct-v0.1',
                     'Mistral-7B-Instruct-v0.2',
                     'Mixtral-8x7B-Instruct-v0.1',
                     'Mixtral-8x22B-Instruct-v0.1',
                     'gpt-4-0125-preview',
                     'gpt-3.5-turbo-1106',
@@ -96,67 +29,153 @@
 abstain_responses = ["I'm sorry, I cannot fulfill that request.",
                      "I'm sorry, I can't fulfill that request.",
                      "I'm sorry, but I cannot fulfill that request.",
                      "I'm sorry, but I can't fulfill that request.",
                      "Sorry, but I can't fulfill that request.",
                      "Sorry, I can't do that."]
 
+class VeriScorer(object):
+    def __init__(self,
+                 model_name_extraction='gpt-4-0125-preview',
+                 model_name_verification='gpt-4o',
+                 data_dir='./data',
+                 cache_dir='./data/cache',
+                 output_dir='./data_cache',
+                 label_n=3,
+                 search_res_num=5):
+        self.data_dir = data_dir
+        self.output_dir = output_dir
+        self.cache_dir = cache_dir
+
+        os.makedirs(output_dir, exist_ok=True)
+        os.makedirs(self.cache_dir, exist_ok=True)
+
+        self.spacy_nlp = spacy.load('en_core_web_sm')
+
+        self.system_message_extraction = "You are a helpful assistant who can extract verifiable atomic claims from a piece of text. Each atomic fact should be verifiable against reliable external world knowledge (e.g., via Wikipedia)"
+
+        self.claim_extractor = ClaimExtractor(model_name_extraction, cache_dir=self.cache_dir)
+
+        self.fetch_search = SearchAPI()
+
+        demon_dir = os.path.join(self.data_dir, 'demos')
+        self.model_name_verification = model_name_verification
+        self.claim_verifier = ClaimVerifier(model_name=model_name_verification, label_n=label_n,
+                                         cache_dir=self.cache_dir, demon_dir=demon_dir)
+        self.label_n = label_n
+        self.search_res_num = search_res_num
+
+    def get_veriscore(self, data, input_file_name):
+
+        ### extract claims ###
+        output_file = f"claims_{input_file_name}.jsonl"
+        output_path = os.path.join(self.output_dir, output_file)
+
+        extracted_claims = []
+        with open(output_path, "w") as f:
+            for dict_item in tqdm(data):
+                question = dict_item["question"]
+                response = dict_item["response"]
+                prompt_source = dict_item["prompt_source"]
+                model = dict_item["model"]
+
+                # skip abstained responses
+                if response.strip() in abstain_responses:
+                    output_dict = {"question": question.strip(),
+                                   "response": response.strip(),
+                                   "abstained": True,
+                                   "prompt_source": prompt_source,
+                                   "model": model, }
+                    f.write(json.dumps(output_dict) + "\n")
+                    extracted_claims.append(output_dict)
+                    continue
+
+                # extract claims
+                snippet_lst, claim_lst_lst, all_claim_lst, prompt_tok_cnt, response_tok_cnt = self.claim_extractor.qa_scanner_extractor(
+                    question, response)
+
+                # write output
+                output_dict = {"question": question.strip(),
+                               "prompt_source": prompt_source,
+                               "response": response.strip(),
+                               "prompt_tok_cnt": prompt_tok_cnt,
+                               "response_tok_cnt": response_tok_cnt,
+                               "model": model,
+                               "abstained": False,  # "abstained": False, "abstained": True
+                               "claim_lst_lst": claim_lst_lst,
+                               "all_claim_lst": all_claim_lst
+                               }
+                f.write(json.dumps(output_dict) + "\n")
+                extracted_claims.append(output_dict)
+
+        print(f"claim extraction is done! saved to {output_path}")
+
+        output_file = f"evidence_{input_file_name}.jsonl"
+        output_path = os.path.join(self.output_dir, output_file)
+        searched_evidence_dict = []
+        with open(output_path, "w") as f:
+            for dict_item in tqdm(extracted_claims):
+                if dict_item['abstained']:
+                    f.write(json.dumps(dict_item) + "\n")
+                    searched_evidence_dict.append(dict_item)
+                    continue
+
+                claim_lst = dict_item["all_claim_lst"]
+                if claim_lst == ["No verifiable claim."]:
+                    dict_item["claim_snippets_dict"] = []
+                    f.write(json.dumps(dict_item) + "\n")
+                    searched_evidence_dict.append(dict_item)
+                    continue
+                claim_snippets = self.fetch_search.get_snippets(claim_lst)
+                dict_item["claim_snippets_dict"] = claim_snippets
+                searched_evidence_dict.append(dict_item)
+                f.write(json.dumps(dict_item) + "\n")
+                f.flush()
+        print(f"evidence searching is done! saved to {output_path}")
+
+        output_dir = os.path.join(args.output_dir, 'model_output')
+        os.makedirs(output_dir, exist_ok=True)
+        output_file = f'verification_{input_file_name}_{self.model_name_verification}_{self.label_n}.jsonl'
+        output_path = os.path.join(output_dir, output_file)
+
+        total_prompt_tok_cnt = 0
+        total_resp_tok_cnt = 0
+        with open(output_path, "w") as f:
+            for dict_item in tqdm(searched_evidence_dict):
+                claim_snippets_dict = dict_item["claim_snippets_dict"]
+                claim_verify_res_dict, prompt_tok_cnt, response_tok_cnt = self.claim_verifier.verifying_claim(
+                    claim_snippets_dict, search_res_num=args.search_res_num)
+                json.dump(claim_verify_res_dict, f)
+                f.write("\n")
+                total_prompt_tok_cnt += prompt_tok_cnt
+                total_resp_tok_cnt += response_tok_cnt
+
+        print(f"claim verification is done! saved to {output_path}")
+        print(f"Total cost: {total_prompt_tok_cnt * 10 / 1e6 + total_resp_tok_cnt * 30 / 1e6}")
+
 if __name__ == '__main__':
-    args = argparse.ArgumentParser()
-    args.add_argument("--data_dir", type=str, default='data')
-    args.add_argument("--input_file", type=str, required=True)
-    args.add_argument("--output_dir", type=str, default='data')
-    args.add_argument("--cache_dir", type=str, default='data/cache')
-    args.add_argument("--model_name", type=str, default="gpt-4-0125-preview")
-    args = args.parse_args()
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--data_dir", type=str, default='./data')
+    parser.add_argument("--input_file", type=str, required=True)
+    parser.add_argument("--output_dir", type=str, default='./data')
+    parser.add_argument("--cache_dir", type=str, default='./data/cache')
+    parser.add_argument("--model_name_extraction", type=str, default="gpt-4-0125-preview")
+    parser.add_argument("--model_name_verification", type=str, default="gpt-4o")
+    parser.add_argument("--label_n", type=int, default=3, choices=[2, 3])
+    parser.add_argument("--search_res_num", type=int, default=5)
+    args = parser.parse_args()
+
+
+    vs = VeriScorer(model_name_extraction=args.model_name_extraction,
+                    model_name_verification=args.model_name_verification,
+                    data_dir=args.data_dir,
+                    output_dir=args.output_dir,
+                    cache_dir=args.cache_dir,
+                    label_n=args.label_n,
+                    search_res_num=args.search_res_num)
 
     input_file_name = "".join(args.input_file.split('.')[:-1])
-    # assert input_file_name in input_file_names
-
     input_path = os.path.join(args.data_dir, args.input_file)
     with open(input_path, "r") as f:
         data = [json.loads(x) for x in f.readlines() if x.strip()]
 
-    # initialize objects
-    model_name = args.model_name
-    claim_extractor = ClaimExtractor(model_name, input_file_name, args.cache_dir)
-
-    output_dir = args.output_dir
-    output_file = f"claims_{input_file_name}.jsonl"
-    output_path = os.path.join(output_dir, output_file)
-
-    print(os.path.abspath(output_path))
-
-    with open(output_path, "a+") as f:
-
-        for dict_item in tqdm(data):
-            # get necessary info
-            question = dict_item["question"]
-            response = dict_item["response"]
-            prompt_source = dict_item["prompt_source"]
-            model = dict_item["model"]
-
-            # skip abstained responses
-            if response.strip() in abstain_responses:
-                output_dict = {"question": question.strip(),
-                               "response": response.strip(),
-                               "abstained": True,
-                               "prompt_source": prompt_source,
-                               "model": model,}
-                f.write(json.dumps(output_dict) + "\n")
-                continue
-
-            # extract claims
-            snippet_lst, claim_lst_lst, all_claim_lst, prompt_tok_cnt, response_tok_cnt = claim_extractor.qa_scanner_extractor(question, response)
-
-            # write output
-            output_dict = {"question": question.strip(),
-                           "prompt_source": prompt_source,
-                           "response": response.strip(),
-                           "prompt_tok_cnt": prompt_tok_cnt,
-                           "response_tok_cnt": response_tok_cnt,
-                           "model": model,
-                           "abstained": False, # "abstained": False, "abstained": True
-                           "claim_lst_lst": claim_lst_lst,
-                           "all_claim_lst": all_claim_lst
-                           }
-            f.write(json.dumps(output_dict) + "\n")
+    vs.get_veriscore(data, input_file_name)
```

