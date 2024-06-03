# Comparing `tmp/fastapix_py-0.9.2-py3-none-any.whl.zip` & `tmp/fastapix_py-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2416908 bytes, number of entries: 44
+Zip file size: 2416918 bytes, number of entries: 44
 -rw-r--r--  2.0 fat      663 b- defN 20-Feb-02 00:00 fastapix/__init__.py
 -rw-r--r--  2.0 fat      205 b- defN 20-Feb-02 00:00 fastapix/__main__.py
 -rw-r--r--  2.0 fat      440 b- defN 20-Feb-02 00:00 fastapix/exceptions.py
 -rw-r--r--  2.0 fat     2391 b- defN 20-Feb-02 00:00 fastapix/handlers.py
 -rw-r--r--  2.0 fat      231 b- defN 20-Feb-02 00:00 fastapix/innerclient.py
 -rw-r--r--  2.0 fat    15953 b- defN 20-Feb-02 00:00 fastapix/main.py
 -rw-r--r--  2.0 fat     2269 b- defN 20-Feb-02 00:00 fastapix/responses.py
@@ -31,16 +31,16 @@
 -rw-r--r--  2.0 fat  3724181 b- defN 20-Feb-02 00:00 fastapix/offline/static/openapi/redoc.standalone.js.map
 -rw-r--r--  2.0 fat  1398528 b- defN 20-Feb-02 00:00 fastapix/offline/static/openapi/swagger-ui-bundle.js
 -rw-r--r--  2.0 fat  1901775 b- defN 20-Feb-02 00:00 fastapix/offline/static/openapi/swagger-ui-bundle.js.map
 -rw-r--r--  2.0 fat   152084 b- defN 20-Feb-02 00:00 fastapix/offline/static/openapi/swagger-ui.css
 -rw-r--r--  2.0 fat   262641 b- defN 20-Feb-02 00:00 fastapix/offline/static/openapi/swagger-ui.css.map
 -rw-r--r--  2.0 fat      139 b- defN 20-Feb-02 00:00 fastapix/sso/__init__.py
 -rw-r--r--  2.0 fat    15276 b- defN 20-Feb-02 00:00 fastapix/sso/_casx.py
--rw-r--r--  2.0 fat     4083 b- defN 20-Feb-02 00:00 fastapix/sso/_client.py
+-rw-r--r--  2.0 fat     4160 b- defN 20-Feb-02 00:00 fastapix/sso/_client.py
 -rw-r--r--  2.0 fat     1300 b- defN 20-Feb-02 00:00 fastapix/sso/cas.py
 -rw-r--r--  2.0 fat      169 b- defN 20-Feb-02 00:00 fastapix/sso/extend/__init__.py
 -rw-r--r--  2.0 fat     1498 b- defN 20-Feb-02 00:00 fastapix/sso/extend/casdoor.py
-?rw-r--r--  2.0 fat     4021 b- defN 20-Feb-02 00:00 fastapix_py-0.9.2.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 fastapix_py-0.9.2.dist-info/WHEEL
-?rw-r--r--  2.0 fat    11558 b- defN 20-Feb-02 00:00 fastapix_py-0.9.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat     3787 b- defN 20-Feb-02 00:00 fastapix_py-0.9.2.dist-info/RECORD
-44 files, 8667149 bytes uncompressed, 2410892 bytes compressed:  72.2%
+?rw-r--r--  2.0 fat     4021 b- defN 20-Feb-02 00:00 fastapix_py-0.9.3.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 fastapix_py-0.9.3.dist-info/WHEEL
+?rw-r--r--  2.0 fat    11558 b- defN 20-Feb-02 00:00 fastapix_py-0.9.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat     3787 b- defN 20-Feb-02 00:00 fastapix_py-0.9.3.dist-info/RECORD
+44 files, 8667226 bytes uncompressed, 2410902 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -114,20 +114,20 @@
 
 Filename: fastapix/sso/extend/__init__.py
 Comment: 
 
 Filename: fastapix/sso/extend/casdoor.py
 Comment: 
 
-Filename: fastapix_py-0.9.2.dist-info/METADATA
+Filename: fastapix_py-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: fastapix_py-0.9.2.dist-info/WHEEL
+Filename: fastapix_py-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: fastapix_py-0.9.2.dist-info/licenses/LICENSE
+Filename: fastapix_py-0.9.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: fastapix_py-0.9.2.dist-info/RECORD
+Filename: fastapix_py-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastapix/__init__.py

```diff
@@ -1,13 +1,13 @@
 # !/usr/bin/env Python3
 # -*- coding: utf-8 -*-
 # @Author   : zhangzhanqi
 # @FILE     : __init__.py
 # @Time     : 2023/11/16 16:37
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 
 from fastapi import FastAPI
 
 from .main import run, main
```

## fastapix/sso/_client.py

```diff
@@ -60,15 +60,15 @@
 
         @router.get(signin_path, include_in_schema=False)
         @router.post(signin_path, include_in_schema=False)
         async def signin(request: Request, redirect_url: str = Query("/docs")):
             query = urllib_parse.urlencode({'redirect_url': redirect_url})
             signin_url = str(request.url.replace(query=query))
             if self.proxy:
-                signin_url = self.proxy + '/' + signin_url.split("/", 3)[3]
+                signin_url = urllib_parse.urljoin(self.proxy, signin_url.split("/", 3)[3])
             user = await self.verify_user(request, signin_url)
             request.session[SESSION_KEY] = user
             return RedirectResponse(redirect_url)
 
         @router.get(signout_path, include_in_schema=False)
         @router.post(signout_path, include_in_schema=False)
         async def signout(request: Request, redirect_url: str = Query("/docs")):
@@ -76,26 +76,27 @@
                 request.session.pop(SESSION_KEY)
             return RedirectResponse(redirect_url)
 
         @router.get('/toLogin', description=f'[重定向到此地址以完成登录](#/{prefix}/toLogin)')
         async def to_login(request: Request, redirect_url: str = Query("/docs")):
             parent_url = str(request.url).split('/toLogin')[0]
             if self.proxy:
-                parent_url = self.proxy + '/' + parent_url.split("/", 3)[3]
+                parent_url = urllib_parse.urljoin(self.proxy, parent_url.split("/", 3)[3])
             query = urllib_parse.urlencode({'redirect_url': redirect_url})
             signin_url = parent_url + signin_path + '?' + query
             return RedirectResponse(await self.sso_login_url(signin_url))
 
         @router.get('/toLogout', description=f'[重定向到此地址以完成退出](#/{prefix}/toLogout)')
         async def to_logout(request: Request, redirect_url: str = Query("/docs")):
             parent_url = str(request.url).split('/toLogout')[0]
             if self.proxy:
-                parent_url = self.proxy + '/' + parent_url.split("/", 3)[3]
+                parent_url = urllib_parse.urljoin(self.proxy, parent_url.split("/", 3)[3])
             query = urllib_parse.urlencode({'redirect_url': redirect_url})
             signout_url = parent_url + signout_path + '?' + query
+            print(signout_url)
             return RedirectResponse(await self.sso_logout_url(signout_url))
 
         return router
 
     async def sso_login_url(self, signin_url: str) -> str:
         raise NotImplementedError
```

## Comparing `fastapix_py-0.9.2.dist-info/METADATA` & `fastapix_py-0.9.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapix-py
-Version: 0.9.2
+Version: 0.9.3
 Summary: A FastAPI plugin that quickly builds CRUD-API based on SQLAlchemy
 Project-URL: Homepage, https://gitee.com/kaiqione/fastapix
 Project-URL: Repository, https://gitee.com/kaiqione/fastapix
 Project-URL: Source, https://gitee.com/kaiqione/fastapix
 Author-email: zhangzhanqi <zzq120203@163.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

## Comparing `fastapix_py-0.9.2.dist-info/licenses/LICENSE` & `fastapix_py-0.9.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `fastapix_py-0.9.2.dist-info/RECORD` & `fastapix_py-0.9.3.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-fastapix/__init__.py,sha256=1Ssj--5RDLHFuJhIL-WM9-eI2-IDLBD_M6llbwwgkEA,663
+fastapix/__init__.py,sha256=RLu2YPcPrE8JnwwyVV-7dQRrrpr068gyzoV5ZRA5k84,663
 fastapix/__main__.py,sha256=WogZFAxuhjiIytlYwhI99oCr8wkkckXYeszffuoATME,205
 fastapix/exceptions.py,sha256=nBIxrGe5df-AUWaQaPfuohO_U2TiAwmTb8hZNcVSrxU,440
 fastapix/handlers.py,sha256=cnwQvAEsp9rDU_9-w66X-lHovKRB8_hbBxpSPQFwpjA,2391
 fastapix/innerclient.py,sha256=v-N1oy3JOJmdf4p91fzureIdGukeIGjYGdagtNcaRKk,231
 fastapix/main.py,sha256=tiNz8HMQp_rWd9uH0qOVBsAfPnkEFGg6r9JRfqaLXng,15953
 fastapix/responses.py,sha256=P09DvuCQnUFskzKznyOZnM78hrn0QKlMtySS9cppWyw,2269
 fastapix/common/__init__.py,sha256=ja58PU71hlquXyhcw2oGajdEl02NxGSoZ-57h5Aq9iQ,139
@@ -30,15 +30,15 @@
 fastapix/offline/static/openapi/redoc.standalone.js.map,sha256=cjZFZyZMVGvpghjM22KA0Xhim14QdTNFRo67WctMwFw,3724181
 fastapix/offline/static/openapi/swagger-ui-bundle.js,sha256=ElVTwsimKgbsD2sT1KXGkK-orChKQcpYp2XM9-CLW9s,1398528
 fastapix/offline/static/openapi/swagger-ui-bundle.js.map,sha256=qGr3YoNMCxBxsO8ohgPJYCqmERM74jqyAjFHV_15mWA,1901775
 fastapix/offline/static/openapi/swagger-ui.css,sha256=58dWC2uof9SkVRL6dIdFyw6e-pWTlA-eiFBheXcvMh0,152084
 fastapix/offline/static/openapi/swagger-ui.css.map,sha256=N8OBv4HRVRMJQSqlZtAY0wfo11iKbZKC80oOhJOqomk,262641
 fastapix/sso/__init__.py,sha256=XIYcx2UBD63MdJNbA1g9Pol68a4_FSNYbRCyLTKf7YY,139
 fastapix/sso/_casx.py,sha256=nYV5RSGhDiXZDbq76-IaXigKGmvPzgh3HwtwgA1eRMs,15276
-fastapix/sso/_client.py,sha256=Aj8599k2gZSf257yFvCRLyQQ6gzhj4YfDiW-iI-u2UQ,4083
+fastapix/sso/_client.py,sha256=01C4qX1xwfRbirpgeTOYQGnBeOs92qFE-ZscEfYulyE,4160
 fastapix/sso/cas.py,sha256=uR-jEaIoRbMvjetebKEmOFn2vdC9k9kUSkdazjA1Gok,1300
 fastapix/sso/extend/__init__.py,sha256=MDvryZzqYcquZL9KADv1HW0ui0E97HcNQjU99c_q-OE,169
 fastapix/sso/extend/casdoor.py,sha256=gijKtU9W3oBwgoSL5e1u0vzwumeXBQkIKn_OBwrvurU,1498
-fastapix_py-0.9.2.dist-info/METADATA,sha256=PxYf5V_N-uxly21B2Pi5AAD5xbFfvpXnwW6qpnFKF1Y,4021
-fastapix_py-0.9.2.dist-info/WHEEL,sha256=mRYSEL3Ih6g5a_CVMIcwiF__0Ae4_gLYh01YFNwiq1k,87
-fastapix_py-0.9.2.dist-info/licenses/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-fastapix_py-0.9.2.dist-info/RECORD,,
+fastapix_py-0.9.3.dist-info/METADATA,sha256=ivjOXZVUiW5KCRPhG3ebUeJ7gdkNB0AimawqVB7X4n0,4021
+fastapix_py-0.9.3.dist-info/WHEEL,sha256=mRYSEL3Ih6g5a_CVMIcwiF__0Ae4_gLYh01YFNwiq1k,87
+fastapix_py-0.9.3.dist-info/licenses/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+fastapix_py-0.9.3.dist-info/RECORD,,
```

