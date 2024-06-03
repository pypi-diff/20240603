# Comparing `tmp/html_summary-0.3.0-py3-none-any.whl.zip` & `tmp/html_summary-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3706 bytes, number of entries: 8
+Zip file size: 3710 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 html_summary/__init__.py
 -rw-r--r--  2.0 unx      998 b- defN 80-Jan-01 00:00 html_summary/cli.py
--rw-r--r--  2.0 unx     1406 b- defN 80-Jan-01 00:00 html_summary/summary.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 html_summary-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      789 b- defN 80-Jan-01 00:00 html_summary-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 html_summary-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 html_summary-0.3.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      646 b- defN 16-Jan-01 00:00 html_summary-0.3.0.dist-info/RECORD
-8 files, 5047 bytes uncompressed, 2570 bytes compressed:  49.1%
+-rw-r--r--  2.0 unx     1401 b- defN 80-Jan-01 00:00 html_summary/summary.py
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 html_summary-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      840 b- defN 80-Jan-01 00:00 html_summary-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 html_summary-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 html_summary-0.3.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      646 b- defN 16-Jan-01 00:00 html_summary-0.3.1.dist-info/RECORD
+8 files, 5093 bytes uncompressed, 2574 bytes compressed:  49.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: html_summary/cli.py
 Comment: 
 
 Filename: html_summary/summary.py
 Comment: 
 
-Filename: html_summary-0.3.0.dist-info/LICENSE
+Filename: html_summary-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: html_summary-0.3.0.dist-info/METADATA
+Filename: html_summary-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: html_summary-0.3.0.dist-info/WHEEL
+Filename: html_summary-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: html_summary-0.3.0.dist-info/entry_points.txt
+Filename: html_summary-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: html_summary-0.3.0.dist-info/RECORD
+Filename: html_summary-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## html_summary/summary.py

```diff
@@ -19,15 +19,15 @@
 {text}
 
 Summary:"""
 
 
 @functools.cache
 def get_chain() -> RunnableSerializable:
-    llm = ChatOpenAI(temperature=0, model="gpt-4-turbo")
+    llm = ChatOpenAI(temperature=0, model="gpt-4o")
     prompt = PromptTemplate.from_template(PROMPT_TEMPLATE)
     chain = prompt | llm
     return chain
 
 
 def load_html(f: str) -> str:
     loader = BSHTMLLoader(f)
```

## Comparing `html_summary-0.3.0.dist-info/LICENSE` & `html_summary-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `html_summary-0.3.0.dist-info/METADATA` & `html_summary-0.3.1.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: html_summary
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: narumi
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
-Requires-Dist: langchain (>=0.1.17,<0.2.0)
-Requires-Dist: langchain-openai (>=0.1.6,<0.2.0)
-Requires-Dist: langchain-text-splitters (>=0.0.1,<0.0.2)
+Requires-Dist: langchain (>=0.2.1,<0.3.0)
+Requires-Dist: langchain-community (>=0.2.1,<0.3.0)
+Requires-Dist: langchain-openai (>=0.1.8,<0.2.0)
+Requires-Dist: langchain-text-splitters (>=0.2.0,<0.3.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: pypdf (>=4.2.0,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
```

## Comparing `html_summary-0.3.0.dist-info/RECORD` & `html_summary-0.3.1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 html_summary/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 html_summary/cli.py,sha256=YQ8HL5itdHUy3dZVKnjsgGhTqxbtaoMDC6ycVjSI070,998
-html_summary/summary.py,sha256=lsJ_xi5roXS1uK7m_m8Ofk_nAOY2L-jNvsUPpJTqz2E,1406
-html_summary-0.3.0.dist-info/LICENSE,sha256=H2T3_RTgmcngMeC7p_SXT3GwBLkd2DaNgAZuxulcfiA,1066
-html_summary-0.3.0.dist-info/METADATA,sha256=JHhtAUznq6DMJ_Z-VzYrVjuqgRDjTo73s9JjB1UL3aU,789
-html_summary-0.3.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-html_summary-0.3.0.dist-info/entry_points.txt,sha256=oUHajPykJSfIzQR2yTXw3M9HasZCYyG4unSL2lkkies,54
-html_summary-0.3.0.dist-info/RECORD,,
+html_summary/summary.py,sha256=GWlTSmZDxmH4_yBEB0sOaacmNqqN6y5Y6PowsTg7FPQ,1401
+html_summary-0.3.1.dist-info/LICENSE,sha256=H2T3_RTgmcngMeC7p_SXT3GwBLkd2DaNgAZuxulcfiA,1066
+html_summary-0.3.1.dist-info/METADATA,sha256=etvMX9Mstiqblp0MRCSflbdisRl2xlUPVEs0HBdpxLM,840
+html_summary-0.3.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+html_summary-0.3.1.dist-info/entry_points.txt,sha256=oUHajPykJSfIzQR2yTXw3M9HasZCYyG4unSL2lkkies,54
+html_summary-0.3.1.dist-info/RECORD,,
```

