# Comparing `tmp/webuiapi-0.9.8-py3-none-any.whl.zip` & `tmp/webuiapi-0.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 19404 bytes, number of entries: 7
--rw-r--r--  2.0 unx     1233 b- defN 24-Jan-14 14:03 webuiapi/__init__.py
--rw-r--r--  2.0 unx    68057 b- defN 24-Jan-14 14:02 webuiapi/webuiapi.py
--rw-r--r--  2.0 unx     1079 b- defN 24-Jan-14 14:03 webuiapi-0.9.8.dist-info/LICENSE
--rw-r--r--  2.0 unx    17285 b- defN 24-Jan-14 14:03 webuiapi-0.9.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-14 14:03 webuiapi-0.9.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Jan-14 14:03 webuiapi-0.9.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      546 b- defN 24-Jan-14 14:03 webuiapi-0.9.8.dist-info/RECORD
-7 files, 88301 bytes uncompressed, 18442 bytes compressed:  79.1%
+Zip file size: 20522 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     1253 b- defN 24-Mar-12 02:02 webuiapi/__init__.py
+-rw-r--r--  2.0 unx    70075 b- defN 24-Mar-12 02:00 webuiapi/webuiapi.py
+-rw-r--r--  2.0 unx     1079 b- defN 24-Mar-12 02:02 webuiapi-0.9.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx    19623 b- defN 24-Mar-12 02:02 webuiapi-0.9.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-12 02:02 webuiapi-0.9.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Mar-12 02:02 webuiapi-0.9.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      546 b- defN 24-Mar-12 02:02 webuiapi-0.9.9.dist-info/RECORD
+7 files, 92677 bytes uncompressed, 19560 bytes compressed:  78.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: webuiapi/__init__.py
 Comment: 
 
 Filename: webuiapi/webuiapi.py
 Comment: 
 
-Filename: webuiapi-0.9.8.dist-info/LICENSE
+Filename: webuiapi-0.9.9.dist-info/LICENSE
 Comment: 
 
-Filename: webuiapi-0.9.8.dist-info/METADATA
+Filename: webuiapi-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: webuiapi-0.9.8.dist-info/WHEEL
+Filename: webuiapi-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: webuiapi-0.9.8.dist-info/top_level.txt
+Filename: webuiapi-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: webuiapi-0.9.8.dist-info/RECORD
+Filename: webuiapi-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webuiapi/__init__.py

```diff
@@ -12,24 +12,25 @@
     ControlNetUnit,
     RemBGInterface,
     ADetailer,
     Roop,
     ReActor,
     ADetailer,    
     Roop,
+    Sag,
     SegmentAnythingInterface,
     SegmentAnythingSamResult,
     SegmentAnythingDilationResult,
     SegmentAnythingGinoResult,
     SegmentAnythingControlNetSegRandomResult,
     SegmentAnythingControlNetSegNotRandomResult,
     SegmentAnythingSemanticSegWithCatIdResult
 )
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 __all__ = [
     "__version__",
     "WebUIApi",
     "WebUIApiResult",
     "Upscaler",
     "HiResUpscaler",
@@ -39,14 +40,15 @@
     "InstructPix2PixInterface",
     "ControlNetInterface",
     "ControlNetUnit",
     "RemBGInterface",
     "ADetailer",
     "Roop",
     "ReActor",
+    "Sag",
     "SegmentAnythingInterface",
     "SegmentAnythingSamResult",
     "SegmentAnythingDilationResult",
     "SegmentAnythingGinoResult",
     "SegmentAnythingControlNetSegRandomResult",
     "SegmentAnythingControlNetSegNotRandomResult",
     "SegmentAnythingSemanticSegWithCatIdResult"
```

## webuiapi/webuiapi.py

```diff
@@ -41,14 +41,15 @@
 
 
 @dataclass
 class WebUIApiResult:
     images: list
     parameters: dict
     info: dict
+    json: dict
 
     @property
     def image(self):
         return self.images[0]
 
 
 class ControlNetUnit:
@@ -351,14 +352,31 @@
             self.target_hash_check,
             self.device,
             self.mask_face,
             self.select_source,
             self.face_model,
         ]
 
+class Sag:
+    def __init__(self,
+                enable: bool = True,  #1 Enable Sag
+                scale: float = 0.75,
+                mask_threshold: float = 1.00
+    ):
+        self.enable = enable
+        self.scale = scale
+        self.mask_threshold = mask_threshold
+
+    def to_dict(self):
+        
+        return [
+            self.enable,
+            self.scale,
+            self.mask_threshold,
+        ]
 
 
 
 def b64_img(image: Image) -> str:
     return "data:image/png;base64," + raw_b64_img(image)
 
 
@@ -455,15 +473,15 @@
         elif "caption" in r.keys():
             info = r["caption"]
 
         parameters = ""
         if "parameters" in r.keys():
             parameters = r["parameters"]
 
-        return WebUIApiResult(images, parameters, info)
+        return WebUIApiResult(images, parameters, info, r)
 
     async def _to_api_result_async(self, response):
         if response.status != 200:
             raise RuntimeError(response.status, await response.text())
 
         r = await response.json()
         images = []
@@ -483,15 +501,15 @@
         elif "caption" in r.keys():
             info = r["caption"]
 
         parameters = ""
         if "parameters" in r.keys():
             parameters = r["parameters"]
 
-        return WebUIApiResult(images, parameters, info)
+        return WebUIApiResult(images, parameters, info, r)
 
     def txt2img(
         self,
         enable_hr=False,
         denoising_strength=0.7,
         firstphase_width=0,
         firstphase_height=0,
@@ -531,14 +549,15 @@
         send_images=True,
         save_images=False,
         alwayson_scripts={},
         controlnet_units: List[ControlNetUnit] = [],
         adetailer: List[ADetailer] = [],
         roop: Roop = None,
         reactor: ReActor = None,
+        sag: Sag = None,
         sampler_index=None,  # deprecated: use sampler_name
         use_deprecated_controlnet=False,
         use_async=False,
     ):
         if sampler_index is None:
             sampler_index = self.default_sampler
         if sampler_name is None:
@@ -615,14 +634,20 @@
             }
 
         if reactor :
             payload["alwayson_scripts"]["reactor"] = {
                 "args": reactor.to_dict()
             }
 
+        if sag :
+            payload["alwayson_scripts"]["Self Attention Guidance"] = {
+                "args": sag.to_dict()
+            }
+
+
         if controlnet_units and len(controlnet_units) > 0:
             payload["alwayson_scripts"]["ControlNet"] = {
                 "args": [x.to_dict() for x in controlnet_units]
             }
         elif self.has_controlnet:
             # workaround : if not passed, webui will use previous args!
             payload["alwayson_scripts"]["ControlNet"] = {"args": []}
@@ -695,14 +720,15 @@
         send_images=True,
         save_images=False,
         alwayson_scripts={},
         controlnet_units: List[ControlNetUnit] = [],
         adetailer: List[ADetailer] = [],
         roop: Roop = None,
         reactor: ReActor = None,
+        sag: Sag = None,
         use_deprecated_controlnet=False,
         use_async=False,
     ):
         if sampler_name is None:
             sampler_name = self.default_sampler
         if sampler_index is None:
             sampler_index = self.default_sampler
@@ -782,14 +808,19 @@
                 "args": roop.to_dict()
             }
 
         if reactor:
             payload["alwayson_scripts"]["reactor"] = {
                 "args": reactor.to_dict()
             }
+        
+        if sag:
+            payload["alwayson_scripts"]["Self Attention Guidance"] = {
+                "args": sag.to_dict()
+            }
             
         if controlnet_units and len(controlnet_units) > 0:
             payload["alwayson_scripts"]["ControlNet"] = {
                 "args": [x.to_dict() for x in controlnet_units]
             }
         elif self.has_controlnet:
             payload["alwayson_scripts"]["ControlNet"] = {"args": []}
@@ -905,15 +936,53 @@
         payload = {
             "image": b64_img(image) if isinstance(image, Image.Image) else image,
             "model": model,
         }
 
         response = self.session.post(url=f"{self.baseurl}/interrogate", json=payload)
         return self._to_api_result(response)
+        
+    def list_prompt_gen_models(self):
+        r = self.custom_get("promptgen/list_models")
+        return r['available_models']
+
+    def prompt_gen(self, 
+        model_name: str = "AUTOMATIC/promptgen-lexart",
+        batch_count: int = 1,
+        batch_size: int = 10,
+        text: str = "",
+        min_length: int = 20,
+        max_length: int = 150,
+        num_beams: int = 1,
+        temperature: float = 1,
+        repetition_penalty: float = 1,
+        length_preference: float = 1,
+        sampling_mode: str = "Top K",
+        top_k: float = 12,
+        top_p: float = 0.15,
+    ):
+        payload = {
+            "model_name": model_name,
+            "batch_count": batch_count,
+            "batch_size": batch_size,
+            "text": text,
+            "min_length": min_length,
+            "max_length": max_length,
+            "num_beams": num_beams,
+            "temperature": temperature,
+            "repetition_penalty": repetition_penalty,
+            "length_preference": length_preference,
+            "sampling_mode": sampling_mode,
+            "top_k": top_k,
+            "top_p": top_p
+        }
 
+        r = self.custom_post("promptgen/generate", payload=payload) 
+        return r.json['prompts']
+    
     def interrupt(self):
         response = self.session.post(url=f"{self.baseurl}/interrupt")
         return response.json()
 
     def skip(self):
         response = self.session.post(url=f"{self.baseurl}/skip")
         return response.json()
```

## Comparing `webuiapi-0.9.8.dist-info/LICENSE` & `webuiapi-0.9.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `webuiapi-0.9.8.dist-info/METADATA` & `webuiapi-0.9.9.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webuiapi
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python API client for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/mix1009/sdwebuiapi
 Author: ChunKoo Park
 Author-email: mix1009@gmail.com
 License: MIT
 Keywords: stable-diffuion-webui,AUTOMATIC1111,stable-diffusion,api
 Requires-Python: >=3.7, <4
@@ -600,7 +600,104 @@
     height=512,
     reactor=reactor
 )
 
 file_path = "face_swapped_image.png"
 result1.image.save(file_path)
 ```
+
+
+### Support for Self Attention Guidance (contributed by yano)
+
+https://github.com/ashen-sensored/sd_webui_SAG
+
+```
+import webuiapi
+from PIL import Image
+
+img = Image.open("/path/to/your/image.jpg")
+
+api = webuiapi.WebUIApi()
+
+your_desired_face = Image.open("/path/to/your/desired/face.jpeg")
+
+sag = webuiapi.Sag(
+    enable=True,
+    scale=0.75,
+    mask_threshold=1.00
+)
+
+result1 = api.img2img(
+    images=[img], 
+    prompt="a cute squirrel", 
+    steps=25, 
+    seed=-1, 
+    cfg_scale=7, 
+    denoising_strength=0.5, 
+    resize_mode=2,
+    width=512,
+    height=512,
+    sag=sag
+)
+
+file_path = "face_swapped_image.png"
+result1.image.save(file_path)
+```
+
+### Prompt generator API by [David Martin Rius](https://github.com/davidmartinrius/):
+
+
+This is an unofficial implementation to use the api of promptgen. 
+Before installing the extension you have to check if you already have an extension called Promptgen. If so, you need to uninstall it.
+Once uninstalled you can install it in two ways:
+
+#### 1. From the user interface
+![image](https://github.com/davidmartinrius/sdwebuiapi/assets/16558194/d879719f-bb9f-44a7-aef7-b893d117bbea)
+
+#### 2. From the command line
+
+cd stable-diffusion-webui/extensions
+
+git clone -b api-implementation https://github.com/davidmartinrius/stable-diffusion-webui-promptgen.git
+
+Once installed:
+```
+api = webuiapi.WebUIApi()
+
+result = api.list_prompt_gen_models()
+print("list of models")
+print(result)
+# you will get something like this:
+#['AUTOMATIC/promptgen-lexart', 'AUTOMATIC/promptgen-majinai-safe', 'AUTOMATIC/promptgen-majinai-unsafe']
+
+text = "a box"
+
+To create a prompt from a text:
+# by default model_name is "AUTOMATIC/promptgen-lexart"
+result = api.prompt_gen(text=text)
+
+# Using a different model
+result = api.prompt_gen(text=text, model_name="AUTOMATIC/promptgen-majinai-unsafe")
+
+#Complete usage
+result =  api.prompt_gen(
+        text=text, 
+        model_name="AUTOMATIC/promptgen-majinai-unsafe",
+        batch_count= 1,
+        batch_size=10,
+        min_length=20,
+        max_length=150,
+        num_beams=1,
+        temperature=1,
+        repetition_penalty=1,
+        length_preference=1,
+        sampling_mode="Top K",
+        top_k=12,
+        top_p=0.15
+    )
+
+# result is a list of prompts. You can iterate the list or just get the first result like this: result[0]
+
+```
+
+
+
```

## Comparing `webuiapi-0.9.8.dist-info/RECORD` & `webuiapi-0.9.9.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-webuiapi/__init__.py,sha256=M1DYpowbPq6vWtKXgPNwENzcK3H2bR5O1noc6mYYRjk,1233
-webuiapi/webuiapi.py,sha256=Nu_EvkuCDZs9sYIc-xI53cudPLl-ITiK_m_0jLVzjkE,68057
-webuiapi-0.9.8.dist-info/LICENSE,sha256=Zl3ztitjIWviypQXfHYvUR099Y5IUOh15IVxAOw9XV8,1079
-webuiapi-0.9.8.dist-info/METADATA,sha256=UVP2jNBRP-vObNkt4iCrrMiHVw6ob-pMGJo2shp0dr8,17285
-webuiapi-0.9.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-webuiapi-0.9.8.dist-info/top_level.txt,sha256=84RprjAaGWFS3oujg2AE1dTHp6o4yGT9isvN6frk5p4,9
-webuiapi-0.9.8.dist-info/RECORD,,
+webuiapi/__init__.py,sha256=437d8xY3TEEoKJLPAG-bwTMyxAOENgTaQLULu_K9F44,1253
+webuiapi/webuiapi.py,sha256=SMfwmjVN0ofg-BQg6x7Pa2B7XRQq-_IFPqJdysmDC2M,70075
+webuiapi-0.9.9.dist-info/LICENSE,sha256=Zl3ztitjIWviypQXfHYvUR099Y5IUOh15IVxAOw9XV8,1079
+webuiapi-0.9.9.dist-info/METADATA,sha256=d_0q8YfAo6q-Izrgp0oyIhGAzqkEKG0yvWi0CfdmNJE,19623
+webuiapi-0.9.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+webuiapi-0.9.9.dist-info/top_level.txt,sha256=84RprjAaGWFS3oujg2AE1dTHp6o4yGT9isvN6frk5p4,9
+webuiapi-0.9.9.dist-info/RECORD,,
```

