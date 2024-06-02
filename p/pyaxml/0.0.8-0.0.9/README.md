# Comparing `tmp/pyaxml-0.0.8.tar.gz` & `tmp/pyaxml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaxml-0.0.8.tar", last modified: Wed May 15 10:32:37 2024, max compression
+gzip compressed data, was "pyaxml-0.0.9.tar", last modified: Sun Jun  2 22:00:51 2024, max compression
```

## Comparing `pyaxml-0.0.8.tar` & `pyaxml-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:32:37.617050 pyaxml-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2024-05-15 10:31:58.000000 pyaxml-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    22709 2024-05-15 10:32:37.616049 pyaxml-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1267 2024-05-15 10:31:58.000000 pyaxml-0.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1180 2024-05-15 10:31:58.000000 pyaxml-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 10:32:37.617050 pyaxml-0.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:32:37.611050 pyaxml-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:32:37.614050 pyaxml-0.0.8/src/pyaxml/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    65663 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/axml.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:32:37.616049 pyaxml-0.0.8/src/pyaxml/proto/
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/proto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5694 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/proto/axml.proto
--rw-rw-rw-   0 root         (0) root         (0)   106820 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/public.json
--rw-rw-rw-   0 root         (0) root         (0)     2011 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/public.py
--rw-rw-rw-   0 root         (0) root         (0)   191207 2024-05-15 10:31:58.000000 pyaxml-0.0.8/src/pyaxml/public.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:32:37.616049 pyaxml-0.0.8/src/pyaxml.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22709 2024-05-15 10:32:37.000000 pyaxml-0.0.8/src/pyaxml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      399 2024-05-15 10:32:37.000000 pyaxml-0.0.8/src/pyaxml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 10:32:37.000000 pyaxml-0.0.8/src/pyaxml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-15 10:32:37.000000 pyaxml-0.0.8/src/pyaxml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-15 10:32:37.000000 pyaxml-0.0.8/src/pyaxml.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:32:37.616049 pyaxml-0.0.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)      541 2024-05-15 10:31:58.000000 pyaxml-0.0.8/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:00:51.718267 pyaxml-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2024-06-02 22:00:13.000000 pyaxml-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22709 2024-06-02 22:00:51.717267 pyaxml-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2024-06-02 22:00:13.000000 pyaxml-0.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2024-06-02 22:00:13.000000 pyaxml-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-02 22:00:51.718267 pyaxml-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:00:51.712267 pyaxml-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:00:51.715267 pyaxml-0.0.9/src/pyaxml/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-06-02 22:00:13.000000 pyaxml-0.0.9/src/pyaxml/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    69088 2024-06-02 22:00:13.000000 pyaxml-0.0.9/src/pyaxml/axml.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-06-02 22:00:13.000000 pyaxml-0.0.9/src/pyaxml/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:00:51.717267 pyaxml-0.0.9/src/pyaxml/proto/
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-06-02 22:00:13.000000 pyaxml-0.0.9/src/pyaxml/proto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5694 2024-06-02 22:00:13.000000 pyaxml-0.0.9/src/pyaxml/proto/axml.proto
+-rw-rw-rw-   0 root         (0) root         (0)   106820 2024-06-02 22:00:13.000000 pyaxml-0.0.9/src/pyaxml/public.json
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2024-06-02 22:00:13.000000 pyaxml-0.0.9/src/pyaxml/public.py
+-rw-rw-rw-   0 root         (0) root         (0)   242391 2024-06-02 22:00:13.000000 pyaxml-0.0.9/src/pyaxml/public.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:00:51.717267 pyaxml-0.0.9/src/pyaxml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22709 2024-06-02 22:00:51.000000 pyaxml-0.0.9/src/pyaxml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      399 2024-06-02 22:00:51.000000 pyaxml-0.0.9/src/pyaxml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-02 22:00:51.000000 pyaxml-0.0.9/src/pyaxml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-06-02 22:00:51.000000 pyaxml-0.0.9/src/pyaxml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-06-02 22:00:51.000000 pyaxml-0.0.9/src/pyaxml.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 22:00:51.717267 pyaxml-0.0.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-06-02 22:00:13.000000 pyaxml-0.0.9/tests/test.py
```

### Comparing `pyaxml-0.0.8/LICENSE` & `pyaxml-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaxml-0.0.8/PKG-INFO` & `pyaxml-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaxml
-Version: 0.0.8
+Version: 0.0.9
 Summary: Manipulate AXML file and create one from scratch
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
```

### Comparing `pyaxml-0.0.8/README.md` & `pyaxml-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyaxml-0.0.8/pyproject.toml` & `pyaxml-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyaxml-0.0.8/src/pyaxml/axml.py` & `pyaxml-0.0.9/src/pyaxml/axml.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,15 +251,18 @@
         """Compute all fields to have all StringBlocks elements
         """
 
         idx = 0
         del self.proto.stringoffsets[:]
         for s in self.proto.stringblocks:
             self.proto.stringoffsets.append(idx)
-            idx += len(StringBlock(proto=s, utf8=self.proto.hnd.flag & axml_pb2.UTF8_FLAG == axml_pb2.UTF8_FLAG).pack())
+            s_obj = StringBlock(proto=s, utf8=self.proto.hnd.flag & axml_pb2.UTF8_FLAG == axml_pb2.UTF8_FLAG)
+            s_obj.compute()
+            idx += len(s_obj.pack())
+            s.CopyFrom(s_obj.proto)
 
         self.proto.hnd.stringoffset = AXML_STRING_POOL_HEADER_SIZE + \
             len(b"".join(pack('<I', x) for x in self.proto.stringoffsets)) + \
             len(b"".join(pack('<I', x) for x in self.proto.styleoffsets))
         
         self.proto.hnd.styleoffset = 0
         self.proto.hnd.hnd.CopyFrom(AXMLHeader(axml_pb2.RES_STRING_POOL_TYPE, len(self.pack())).proto)
@@ -313,14 +316,28 @@
             int: return the index of the stringblock
         """
         name_encoded = StringBlock(data=name, utf8=self.proto.hnd.flag & axml_pb2.UTF8_FLAG == axml_pb2.UTF8_FLAG)
         for i in range(0, len(self.proto.stringblocks)):
             if self.proto.stringblocks[i].data == name_encoded.proto.data:
                 return i
         raise ValueError
+    
+    def update(self, index : int, name : str):
+        name_encoded = StringBlock(data=name, utf8=self.proto.hnd.flag & axml_pb2.UTF8_FLAG == axml_pb2.UTF8_FLAG)
+        self.proto.stringblocks[index].data = name_encoded.proto.data
+
+    def replace(self, old_name : str, new_name : str):
+        index = self.index(old_name)
+        self.update(index, new_name)
+
+    def switch(self, name1 : str, name2 : str):
+        index1 = self.index(name1)
+        index2 = self.index(name2)
+        self.update(index1, name2)
+        self.update(index2, name1)
 
     def decode_str(self, index : int) -> str:
         data = self.proto.stringblocks[index].data
         try:
             return data.decode('utf-8') if self.proto.hnd.flag & axml_pb2.UTF8_FLAG == axml_pb2.UTF8_FLAG else data.decode('utf-16')
         except UnicodeDecodeError:
             return data
@@ -1772,9 +1789,74 @@
         axml.proto.header_xml.CopyFrom(hnd.proto)
         axml.proto.stringblocks.CopyFrom(sb.proto)
         axml.stringblocks = sb
         axml.proto.resourcemap.CopyFrom(res.proto)
         axml.proto.resourcexml.CopyFrom(resxml.proto)
 
         return axml, buff
+
+    def get_elt_string(self, index):
+        if index == 4294967295:
+            return ""
+        if index < len(self.proto.resourcemap.res):
+            return public.SYSTEM_RESOURCES['attributes']['inverse'][self.proto.resourcemap.res[index]]
+        else:
+            
+            data = self.proto.stringblocks.stringblocks[index].data
+            if self.proto.stringblocks.hnd.flag & axml_pb2.UTF8_FLAG == axml_pb2.UTF8_FLAG:
+                return data.decode('utf-8')
+            else:
+                return data.decode('utf-16')
+
+    def to_xml(self):
+        root = None
+        cur = root
+        NSMAP = {"android" : 'http://schemas.android.com/apk/res/android'}
+
+        for xmlelt in self.proto.resourcexml.elts:
+            if xmlelt.HasField('start_elt'):
+                ns = self.get_elt_string(xmlelt.start_elt.namespaceURI)
+                name = self.get_elt_string(xmlelt.start_elt.name)
+                if ns is "":
+                    node = etree.Element(f"{name}")
+                else:
+                    node = etree.Element("{" + ns + "}" + name)
+                for att in xmlelt.start_elt.attributes:
+                    ns_att = self.get_elt_string(att.namespaceURI)
+                    name_att = self.get_elt_string(att.name)
+                    v = att.value
+                    if att.type == 0x3000008:
+                        v = self.get_elt_string(att.value)
+                    elif att.type == 0x10000008:
+                        v = str(ctypes.c_int32(att.data).value)
+                    elif att.type == 0x40000008:
+                        v = str(ctypes.c_float(att.data).value)
+                    elif att.type & 0x12000000 == 0x12000000:
+                        v = "false" if att.data == 0 else "true"
+                    elif att.type & 0x11000000 == 0x11000000:
+                        v = hex(att.data)
+                    elif att.type & 0x1000000 == 0x1000000:
+                        v = f"@{hex(att.data)[2:]}"
+                    else:
+                        v = str(v)
+                    if ns_att is "":
+                        node.attrib[f"{name_att}"] = v
+                    else:
+                        node.attrib["{" + ns_att +"}" + name_att] = v
+                if root == None:
+                    node = etree.Element(node.tag, attrib=node.attrib, nsmap=NSMAP)
+                    root = node
+                    cur = node
+                else:
+                    cur.append(node)
+                    cur = node
+            elif xmlelt.HasField('end_elt'):
+                cur = cur.getparent()
+                #xmlelt.end_elt
+            elif xmlelt.HasField('start_ns'):
+                xmlelt.start_ns
+            elif xmlelt.HasField('end_ns'):
+                xmlelt.end_ns
+        return root
+
```

### Comparing `pyaxml-0.0.8/src/pyaxml/proto/axml.proto` & `pyaxml-0.0.9/src/pyaxml/proto/axml.proto`

 * *Files identical despite different names*

### Comparing `pyaxml-0.0.8/src/pyaxml/public.json` & `pyaxml-0.0.9/src/pyaxml/public.json`

 * *Files identical despite different names*

### Comparing `pyaxml-0.0.8/src/pyaxml/public.py` & `pyaxml-0.0.9/src/pyaxml/public.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,18 @@
     xmlfile = os.path.join(root, "public.xml")
     if os.path.isfile(xmlfile):
         with open(xmlfile, "r") as fp:
             _xml = minidom.parseString(fp.read())
             for element in _xml.getElementsByTagName("public"):
                 _type = element.getAttribute('type')
                 _name = element.getAttribute('name')
-                _id = int(element.getAttribute('id'), 16)
+                if element.getAttribute('id') == "":
+                    _id = None
+                else:
+                    _id = int(element.getAttribute('id'), 16)
                 if _type not in _public_res:
                     _public_res[_type] = {}
                 _public_res[_type][_name] = _id
     else:
         raise Exception("need to copy the sdk/platforms/android-?/data/res/values/public.xml here")
 
 SYSTEM_RESOURCES = {
@@ -29,28 +32,28 @@
         "forward": {k: v for k, v in _public_res['style'].items()},
         "inverse": {v: k for k, v in _public_res['style'].items()}
     }
 }
 
 
 
-if __name__ == '__main__':
-    import json
-    _resources = None
-    if _resources is None:
-        root = os.path.dirname(os.path.realpath(__file__))
-        resfile = os.path.join(root, "public.json")
-
-        if os.path.isfile(resfile):
-            with open(resfile, "r") as fp:
-                _resources = json.load(fp)
-        else:
-            # TODO raise error instead?
-            _resources = {}
-    for _type in set([] + list(_public_res.keys()) + list(_resources.keys())):
-        for k in set([] + list(_public_res.get(_type, {}).keys())
-                     + list(_resources.get(_type, {}).keys())):
-            a,b = _public_res.get(_type, {}).get(k), \
-                  _resources.get(_type, {}).get(k),
-            if a != b:
-                print(k, a,b)
-    print(None)
+#if __name__ == '__main__':
+#    import json
+#    _resources = None
+#    if _resources is None:
+#        root = os.path.dirname(os.path.realpath(__file__))
+#        resfile = os.path.join(root, "public.json")
+#
+#        if os.path.isfile(resfile):
+#            with open(resfile, "r") as fp:
+#                _resources = json.load(fp)
+#        else:
+#            # TODO raise error instead?
+#            _resources = {}
+#    for _type in set([] + list(_public_res.keys()) + list(_resources.keys())):
+#        for k in set([] + list(_public_res.get(_type, {}).keys())
+#                     + list(_resources.get(_type, {}).keys())):
+#            a,b = _public_res.get(_type, {}).get(k), \
+#                  _resources.get(_type, {}).get(k),
+#            if a != b:
+#                print(k, a,b)
+#    print(None)
```

### Comparing `pyaxml-0.0.8/src/pyaxml/public.xml` & `pyaxml-0.0.9/src/pyaxml/public.xml`

 * *Files 21% similar despite different names*

#### Comparing `pyaxml-0.0.8/src/pyaxml/public.xml` & `pyaxml-0.0.9/src/pyaxml/public.xml`

```diff
@@ -696,31 +696,46 @@
   <public type="string" name="VideoView_error_button" id="0x01040010"/>
   <public type="string" name="VideoView_error_text_unknown" id="0x01040011"/>
   <public type="string" name="VideoView_error_title" id="0x01040012"/>
   <public type="string" name="yes" id="0x01040013"/>
   <public type="dimen" name="app_icon_size" id="0x01050000"/>
   <public type="dimen" name="thumbnail_height" id="0x01050001"/>
   <public type="dimen" name="thumbnail_width" id="0x01050002"/>
+  <!-- Equivalent to 0xffaaaaaa -->
   <public type="color" name="darker_gray" id="0x01060000"/>
+  <!-- {@deprecated Use a text color from your theme instead.} -->
   <public type="color" name="primary_text_dark" id="0x01060001"/>
+  <!-- {@deprecated Use a text color from your theme instead.} -->
   <public type="color" name="primary_text_dark_nodisable" id="0x01060002"/>
+  <!-- {@deprecated Use a text color from your theme instead.} -->
   <public type="color" name="primary_text_light" id="0x01060003"/>
+  <!-- {@deprecated Use a text color from your theme instead.} -->
   <public type="color" name="primary_text_light_nodisable" id="0x01060004"/>
+  <!-- {@deprecated Use a text color from your theme instead.} -->
   <public type="color" name="secondary_text_dark" id="0x01060005"/>
+  <!-- {@deprecated Use a text color from your theme instead.} -->
   <public type="color" name="secondary_text_dark_nodisable" id="0x01060006"/>
+  <!-- {@deprecated Use a text color from your theme instead.} -->
   <public type="color" name="secondary_text_light" id="0x01060007"/>
+  <!-- {@deprecated Use a text color from your theme instead.} -->
   <public type="color" name="secondary_text_light_nodisable" id="0x01060008"/>
+  <!-- Equivalent to 0xff808080 -->
   <public type="color" name="tab_indicator_text" id="0x01060009"/>
+  <!-- Equivalent to 0xff000000 -->
   <public type="color" name="widget_edittext_dark" id="0x0106000a"/>
   <public type="color" name="white" id="0x0106000b"/>
   <public type="color" name="black" id="0x0106000c"/>
   <public type="color" name="transparent" id="0x0106000d"/>
+  <!-- Equivalent to 0xff000000 -->
   <public type="color" name="background_dark" id="0x0106000e"/>
+  <!-- Equivalent to 0xffffffff -->
   <public type="color" name="background_light" id="0x0106000f"/>
+  <!-- {@deprecated Use a text color from your theme instead.} -->
   <public type="color" name="tertiary_text_dark" id="0x01060010"/>
+  <!-- {@deprecated Use a text color from your theme instead.} -->
   <public type="color" name="tertiary_text_light" id="0x01060011"/>
   <public type="array" name="emailAddressTypes" id="0x01070000"/>
   <public type="array" name="imProtocols" id="0x01070001"/>
   <public type="array" name="organizationTypes" id="0x01070002"/>
   <public type="array" name="phoneTypes" id="0x01070003"/>
   <public type="array" name="postalAddressTypes" id="0x01070004"/>
   <public type="drawable" name="alert_dark_frame" id="0x01080000"/>
@@ -1027,27 +1042,29 @@
   <!-- Context menu ID for the "Input Method" menu item to being up the
        input method picker dialog, allowing the user to switch to another
        input method. -->
   <public type="id" name="switchInputMethod" id="0x01020024"/>
   <!-- View ID of the text editor inside of an extracted text layout. -->
   <public type="id" name="inputExtractEditText" id="0x01020025"/>
   <!-- View ID of the {@link android.inputmethodservice.KeyboardView} within
-        an input method's input area. -->
+       an input method's input area.
+       {@deprecated Use Copy this definition into your own application project.} -->
   <public type="id" name="keyboardView" id="0x01020026"/>
   <!-- View ID of a {@link android.view.View} to close a popup keyboard -->
   <public type="id" name="closeButton" id="0x01020027"/>
   <!-- Menu ID to perform a "start selecting text" operation. -->
   <public type="id" name="startSelectingText" id="0x01020028"/>
   <!-- Menu ID to perform a "stop selecting text" operation. -->
   <public type="id" name="stopSelectingText" id="0x01020029"/>
   <!-- Menu ID to perform a "add to dictionary" operation. -->
   <public type="id" name="addToDictionary" id="0x0102002a"/>
   <public type="style" name="Theme.InputMethod" id="0x01030054"/>
   <public type="style" name="Theme.NoDisplay" id="0x01030055"/>
   <public type="style" name="Animation.InputMethod" id="0x01030056"/>
+  <!-- {@deprecated Use Copy this definition into your own application project.} -->
   <public type="style" name="Widget.KeyboardView" id="0x01030057"/>
   <public type="style" name="ButtonBar" id="0x01030058"/>
   <public type="style" name="Theme.Panel" id="0x01030059"/>
   <public type="style" name="Theme.Light.Panel" id="0x0103005a"/>
   <public type="string" name="dialog_alert_title" id="0x01040014"/>
   <public type="string" name="VideoView_error_text_invalid_progressive_playback" id="0x01040015"/>
   <public type="drawable" name="ic_btn_speak_now" id="0x010800a4"/>
@@ -1440,21 +1457,21 @@
   <public type="style" name="Theme.WithActionBar" id="0x01030069"/>
   <public type="style" name="Theme.NoTitleBar.OverlayActionModes" id="0x0103006a"/>
   <public type="style" name="Theme.Holo" id="0x0103006b"/>
   <public type="style" name="Theme.Holo.NoActionBar" id="0x0103006c"/>
   <public type="style" name="Theme.Holo.NoActionBar.Fullscreen" id="0x0103006d"/>
   <public type="style" name="Theme.Holo.Light" id="0x0103006e"/>
   <public type="style" name="Theme.Holo.Dialog" id="0x0103006f"/>
-  <public type="style" name="Theme.Holo.Dialogger.MinWidth" id="0x01030070"/>
-  <public type="style" name="Theme.Holo.Dialogger.NoActionBar" id="0x01030071"/>
-  <public type="style" name="Theme.Holo.Dialogger.NoActionBar.MinWidth" id="0x01030072"/>
+  <public type="style" name="Theme.Holo.Dialog.MinWidth" id="0x01030070"/>
+  <public type="style" name="Theme.Holo.Dialog.NoActionBar" id="0x01030071"/>
+  <public type="style" name="Theme.Holo.Dialog.NoActionBar.MinWidth" id="0x01030072"/>
   <public type="style" name="Theme.Holo.Light.Dialog" id="0x01030073"/>
-  <public type="style" name="Theme.Holo.Light.Dialogger.MinWidth" id="0x01030074"/>
-  <public type="style" name="Theme.Holo.Light.Dialogger.NoActionBar" id="0x01030075"/>
-  <public type="style" name="Theme.Holo.Light.Dialogger.NoActionBar.MinWidth" id="0x01030076"/>
+  <public type="style" name="Theme.Holo.Light.Dialog.MinWidth" id="0x01030074"/>
+  <public type="style" name="Theme.Holo.Light.Dialog.NoActionBar" id="0x01030075"/>
+  <public type="style" name="Theme.Holo.Light.Dialog.NoActionBar.MinWidth" id="0x01030076"/>
   <public type="style" name="Theme.Holo.DialogWhenLarge" id="0x01030077"/>
   <public type="style" name="Theme.Holo.DialogWhenLarge.NoActionBar" id="0x01030078"/>
   <public type="style" name="Theme.Holo.Light.DialogWhenLarge" id="0x01030079"/>
   <public type="style" name="Theme.Holo.Light.DialogWhenLarge.NoActionBar" id="0x0103007a"/>
   <public type="style" name="Theme.Holo.Panel" id="0x0103007b"/>
   <public type="style" name="Theme.Holo.Light.Panel" id="0x0103007c"/>
   <public type="style" name="Theme.Holo.Wallpaper" id="0x0103007d"/>
@@ -1717,21 +1734,21 @@
   <public type="style" name="Theme.DeviceDefault" id="0x01030128"/>
   <public type="style" name="Theme.DeviceDefault.NoActionBar" id="0x01030129"/>
   <public type="style" name="Theme.DeviceDefault.NoActionBar.Fullscreen" id="0x0103012a"/>
   <public type="style" name="Theme.DeviceDefault.Light" id="0x0103012b"/>
   <public type="style" name="Theme.DeviceDefault.Light.NoActionBar" id="0x0103012c"/>
   <public type="style" name="Theme.DeviceDefault.Light.NoActionBar.Fullscreen" id="0x0103012d"/>
   <public type="style" name="Theme.DeviceDefault.Dialog" id="0x0103012e"/>
-  <public type="style" name="Theme.DeviceDefault.Dialogger.MinWidth" id="0x0103012f"/>
-  <public type="style" name="Theme.DeviceDefault.Dialogger.NoActionBar" id="0x01030130"/>
-  <public type="style" name="Theme.DeviceDefault.Dialogger.NoActionBar.MinWidth" id="0x01030131"/>
+  <public type="style" name="Theme.DeviceDefault.Dialog.MinWidth" id="0x0103012f"/>
+  <public type="style" name="Theme.DeviceDefault.Dialog.NoActionBar" id="0x01030130"/>
+  <public type="style" name="Theme.DeviceDefault.Dialog.NoActionBar.MinWidth" id="0x01030131"/>
   <public type="style" name="Theme.DeviceDefault.Light.Dialog" id="0x01030132"/>
-  <public type="style" name="Theme.DeviceDefault.Light.Dialogger.MinWidth" id="0x01030133"/>
-  <public type="style" name="Theme.DeviceDefault.Light.Dialogger.NoActionBar" id="0x01030134"/>
-  <public type="style" name="Theme.DeviceDefault.Light.Dialogger.NoActionBar.MinWidth" id="0x01030135"/>
+  <public type="style" name="Theme.DeviceDefault.Light.Dialog.MinWidth" id="0x01030133"/>
+  <public type="style" name="Theme.DeviceDefault.Light.Dialog.NoActionBar" id="0x01030134"/>
+  <public type="style" name="Theme.DeviceDefault.Light.Dialog.NoActionBar.MinWidth" id="0x01030135"/>
   <public type="style" name="Theme.DeviceDefault.DialogWhenLarge" id="0x01030136"/>
   <public type="style" name="Theme.DeviceDefault.DialogWhenLarge.NoActionBar" id="0x01030137"/>
   <public type="style" name="Theme.DeviceDefault.Light.DialogWhenLarge" id="0x01030138"/>
   <public type="style" name="Theme.DeviceDefault.Light.DialogWhenLarge.NoActionBar" id="0x01030139"/>
   <public type="style" name="Theme.DeviceDefault.Panel" id="0x0103013a"/>
   <public type="style" name="Theme.DeviceDefault.Light.Panel" id="0x0103013b"/>
   <public type="style" name="Theme.DeviceDefault.Wallpaper" id="0x0103013c"/>
@@ -2270,19 +2287,19 @@
   <public type="style" name="TextAppearance.Material.Widget.TextView.PopupMenu" id="0x0103021f"/>
   <public type="style" name="TextAppearance.Material.Widget.TextView.SpinnerItem" id="0x01030220"/>
   <public type="style" name="TextAppearance.Material.Widget.Toolbar.Subtitle" id="0x01030221"/>
   <public type="style" name="TextAppearance.Material.Widget.Toolbar.Title" id="0x01030222"/>
   <public type="style" name="Theme.DeviceDefault.Settings" id="0x01030223"/>
   <public type="style" name="Theme.Material" id="0x01030224"/>
   <public type="style" name="Theme.Material.Dialog" id="0x01030225"/>
-  <public type="style" name="Theme.Material.Dialogger.Alert" id="0x01030226"/>
-  <public type="style" name="Theme.Material.Dialogger.MinWidth" id="0x01030227"/>
-  <public type="style" name="Theme.Material.Dialogger.NoActionBar" id="0x01030228"/>
-  <public type="style" name="Theme.Material.Dialogger.NoActionBar.MinWidth" id="0x01030229"/>
-  <public type="style" name="Theme.Material.Dialogger.Presentation" id="0x0103022a"/>
+  <public type="style" name="Theme.Material.Dialog.Alert" id="0x01030226"/>
+  <public type="style" name="Theme.Material.Dialog.MinWidth" id="0x01030227"/>
+  <public type="style" name="Theme.Material.Dialog.NoActionBar" id="0x01030228"/>
+  <public type="style" name="Theme.Material.Dialog.NoActionBar.MinWidth" id="0x01030229"/>
+  <public type="style" name="Theme.Material.Dialog.Presentation" id="0x0103022a"/>
   <public type="style" name="Theme.Material.DialogWhenLarge" id="0x0103022b"/>
   <public type="style" name="Theme.Material.DialogWhenLarge.NoActionBar" id="0x0103022c"/>
   <public type="style" name="Theme.Material.InputMethod" id="0x0103022d"/>
   <public type="style" name="Theme.Material.NoActionBar" id="0x0103022e"/>
   <public type="style" name="Theme.Material.NoActionBar.Fullscreen" id="0x0103022f"/>
   <public type="style" name="Theme.Material.NoActionBar.Overscan" id="0x01030230"/>
   <public type="style" name="Theme.Material.NoActionBar.TranslucentDecor" id="0x01030231"/>
@@ -2290,19 +2307,19 @@
   <public type="style" name="Theme.Material.Settings" id="0x01030233"/>
   <public type="style" name="Theme.Material.Voice" id="0x01030234"/>
   <public type="style" name="Theme.Material.Wallpaper" id="0x01030235"/>
   <public type="style" name="Theme.Material.Wallpaper.NoTitleBar" id="0x01030236"/>
   <public type="style" name="Theme.Material.Light" id="0x01030237"/>
   <public type="style" name="Theme.Material.Light.DarkActionBar" id="0x01030238"/>
   <public type="style" name="Theme.Material.Light.Dialog" id="0x01030239"/>
-  <public type="style" name="Theme.Material.Light.Dialogger.Alert" id="0x0103023a"/>
-  <public type="style" name="Theme.Material.Light.Dialogger.MinWidth" id="0x0103023b"/>
-  <public type="style" name="Theme.Material.Light.Dialogger.NoActionBar" id="0x0103023c"/>
-  <public type="style" name="Theme.Material.Light.Dialogger.NoActionBar.MinWidth" id="0x0103023d"/>
-  <public type="style" name="Theme.Material.Light.Dialogger.Presentation" id="0x0103023e"/>
+  <public type="style" name="Theme.Material.Light.Dialog.Alert" id="0x0103023a"/>
+  <public type="style" name="Theme.Material.Light.Dialog.MinWidth" id="0x0103023b"/>
+  <public type="style" name="Theme.Material.Light.Dialog.NoActionBar" id="0x0103023c"/>
+  <public type="style" name="Theme.Material.Light.Dialog.NoActionBar.MinWidth" id="0x0103023d"/>
+  <public type="style" name="Theme.Material.Light.Dialog.Presentation" id="0x0103023e"/>
   <public type="style" name="Theme.Material.Light.DialogWhenLarge" id="0x0103023f"/>
   <public type="style" name="Theme.Material.Light.DialogWhenLarge.NoActionBar" id="0x01030240"/>
   <public type="style" name="Theme.Material.Light.NoActionBar" id="0x01030241"/>
   <public type="style" name="Theme.Material.Light.NoActionBar.Fullscreen" id="0x01030242"/>
   <public type="style" name="Theme.Material.Light.NoActionBar.Overscan" id="0x01030243"/>
   <public type="style" name="Theme.Material.Light.NoActionBar.TranslucentDecor" id="0x01030244"/>
   <public type="style" name="Theme.Material.Light.Panel" id="0x01030245"/>
@@ -2490,16 +2507,16 @@
   <public type="attr" name="accessibilityTraversalAfter" id="0x010104d2"/>
   <public type="attr" name="dialogPreferredPadding" id="0x010104d3"/>
   <public type="attr" name="searchHintIcon" id="0x010104d4"/>
   <public type="attr" name="revisionCode" id="0x010104d5"/>
   <public type="attr" name="drawableTint" id="0x010104d6"/>
   <public type="attr" name="drawableTintMode" id="0x010104d7"/>
   <public type="attr" name="fraction" id="0x010104d8"/>
-  <public type="style" name="Theme.DeviceDefault.Dialogger.Alert" id="0x010302d1"/>
-  <public type="style" name="Theme.DeviceDefault.Light.Dialogger.Alert" id="0x010302d2"/>
+  <public type="style" name="Theme.DeviceDefault.Dialog.Alert" id="0x010302d1"/>
+  <public type="style" name="Theme.DeviceDefault.Light.Dialog.Alert" id="0x010302d2"/>
   <!-- ===============================================================
        Resources added in version M of the platform
        =============================================================== -->
   <eat-comment/>
   <public type="attr" name="trackTint" id="0x010104d9"/>
   <public type="attr" name="trackTintMode" id="0x010104da"/>
   <public type="attr" name="start" id="0x010104db"/>
@@ -2525,15 +2542,15 @@
   <public type="attr" name="showForAllUsers" id="0x010104ef"/>
   <public type="attr" name="supportsAssist" id="0x010104f0"/>
   <public type="attr" name="supportsLaunchVoiceAssistFromKeyguard" id="0x010104f1"/>
   <public type="style" name="Widget.Material.Button.Colored" id="0x010302d3"/>
   <public type="style" name="TextAppearance.Material.Widget.Button.Inverse" id="0x010302d4"/>
   <public type="style" name="Theme.Material.Light.LightStatusBar" id="0x010302d5"/>
   <public type="style" name="ThemeOverlay.Material.Dialog" id="0x010302d6"/>
-  <public type="style" name="ThemeOverlay.Material.Dialogger.Alert" id="0x010302d7"/>
+  <public type="style" name="ThemeOverlay.Material.Dialog.Alert" id="0x010302d7"/>
   <public type="id" name="pasteAsPlainText" id="0x01020031"/>
   <public type="id" name="undo" id="0x01020032"/>
   <public type="id" name="redo" id="0x01020033"/>
   <public type="id" name="replaceText" id="0x01020034"/>
   <public type="id" name="shareText" id="0x01020035"/>
   <public type="id" name="accessibilityActionShowOnScreen" id="0x01020036"/>
   <public type="id" name="accessibilityActionScrollToPosition" id="0x01020037"/>
@@ -2624,26 +2641,14 @@
   <public type="attr" name="roundIcon" id="0x0101052c"/>
   <public type="attr" name="contextUri" id="0x0101052d"/>
   <public type="attr" name="contextDescription" id="0x0101052e"/>
   <public type="attr" name="showMetadataInPreview" id="0x0101052f"/>
   <public type="attr" name="colorSecondary" id="0x01010530"/>
   <!-- ===============================================================
        Resources added in version O of the platform
-
-       NOTE: add <public> elements within a <public-group> like so:
-
-       <public-group type="attr" first-id="0x01010531">
-           <public name="exampleAttr1" />
-           <public name="exampleAttr2" />
-       </public-group>
-
-       To add a new public-group block, choose an id value that is 1 greater
-       than the last of that item above. For example, the last "attr" id
-       value above is 0x01010530, so the public-group of attrs below has
-       the id value of 0x01010531.
        =============================================================== -->
   <eat-comment/>
   <public type="attr" name="visibleToInstantApps" id="0x01010531"/>
   <public type="attr" name="font" id="0x01010532"/>
   <public type="attr" name="fontWeight" id="0x01010533"/>
   <public type="attr" name="tooltipText" id="0x01010534"/>
   <public type="attr" name="autoSizeTextType" id="0x01010535"/>
@@ -2689,49 +2694,870 @@
   <public type="attr" name="fontProviderCerts" id="0x0101055d"/>
   <public type="attr" name="iconTint" id="0x0101055e"/>
   <public type="attr" name="iconTintMode" id="0x0101055f"/>
   <public type="attr" name="maxAspectRatio" id="0x01010560"/>
   <public type="attr" name="iconSpaceReserved" id="0x01010561"/>
   <public type="attr" name="defaultFocusHighlightEnabled" id="0x01010562"/>
   <public type="attr" name="persistentWhenFeatureAvailable" id="0x01010563"/>
+  <!-- {@deprecated Use windowSplashscreenAnimatedIcon instead } -->
   <public type="attr" name="windowSplashscreenContent" id="0x01010564"/>
   <!-- @hide @SystemApi -->
   <public type="attr" name="requiredSystemPropertyName" id="0x01010565"/>
   <!-- @hide @SystemApi -->
   <public type="attr" name="requiredSystemPropertyValue" id="0x01010566"/>
   <public type="attr" name="justificationMode" id="0x01010567"/>
   <public type="attr" name="autofilledHighlight" id="0x01010568"/>
   <public type="id" name="textAssist" id="0x01020041"/>
   <public type="id" name="accessibilityActionMoveWindow" id="0x01020042"/>
   <public type="id" name="autofill" id="0x01020043"/>
   <public type="string" name="paste_as_plain_text" id="0x01040019"/>
   <!-- ===============================================================
        Resources added in version O MR1 of the platform
-
-       NOTE: add <public> elements within a <public-group> like so:
-
-       <public-group type="attr" first-id="0x01010531">
-           <public name="exampleAttr1" />
-           <public name="exampleAttr2" />
-       </public-group>
-
-       To add a new public-group block, choose an id value that is 1 greater
-       than the last of that item above. For example, the last "attr" id
-       value above is 0x01010530, so the public-group of attrs below has
-       the id value of 0x01010531.
        =============================================================== -->
   <eat-comment/>
   <public type="attr" name="showWhenLocked" id="0x01010569"/>
   <public type="attr" name="turnScreenOn" id="0x0101056a"/>
   <public type="attr" name="classLoader" id="0x0101056b"/>
   <public type="attr" name="windowLightNavigationBar" id="0x0101056c"/>
   <public type="attr" name="navigationBarDividerColor" id="0x0101056d"/>
   <public type="string" name="autofill" id="0x0104001a"/>
   <!-- ===============================================================
-       DO NOT ADD UN-GROUPED ITEMS HERE
-
-       Any new items (attrs, styles, ids, etc.) *must* be added in a
-       public-group block, as the preceding comment explains.
-       Items added outside of a group may have their value recalculated
-       every time something new is added to this file.
+       Resources added in version P of the platform
+       =============================================================== -->
+  <eat-comment/>
+  <public type="attr" name="cantSaveState" id="0x0101056e"/>
+  <public type="attr" name="ttcIndex" id="0x0101056f"/>
+  <public type="attr" name="fontVariationSettings" id="0x01010570"/>
+  <public type="attr" name="dialogCornerRadius" id="0x01010571"/>
+  <!-- @hide For use by platform and tools only. Developers should not specify this value. -->
+  <public type="attr" name="compileSdkVersion" id="0x01010572"/>
+  <!-- @hide For use by platform and tools only. Developers should not specify this value. -->
+  <public type="attr" name="compileSdkVersionCodename" id="0x01010573"/>
+  <public type="attr" name="screenReaderFocusable" id="0x01010574"/>
+  <public type="attr" name="buttonCornerRadius" id="0x01010575"/>
+  <public type="attr" name="versionCodeMajor" id="0x01010576"/>
+  <public type="attr" name="versionMajor" id="0x01010577"/>
+  <!-- @hide @SystemApi -->
+  <public type="attr" name="isVrOnly" id="0x01010578"/>
+  <public type="attr" name="widgetFeatures" id="0x01010579"/>
+  <public type="attr" name="appComponentFactory" id="0x0101057a"/>
+  <public type="attr" name="fallbackLineSpacing" id="0x0101057b"/>
+  <public type="attr" name="accessibilityPaneTitle" id="0x0101057c"/>
+  <public type="attr" name="firstBaselineToTopHeight" id="0x0101057d"/>
+  <public type="attr" name="lastBaselineToBottomHeight" id="0x0101057e"/>
+  <public type="attr" name="lineHeight" id="0x0101057f"/>
+  <public type="attr" name="accessibilityHeading" id="0x01010580"/>
+  <public type="attr" name="outlineSpotShadowColor" id="0x01010581"/>
+  <public type="attr" name="outlineAmbientShadowColor" id="0x01010582"/>
+  <public type="attr" name="maxLongVersionCode" id="0x01010583"/>
+  <!-- @hide @SystemApi -->
+  <public type="attr" name="userRestriction" id="0x01010584"/>
+  <public type="attr" name="textFontWeight" id="0x01010585"/>
+  <public type="attr" name="windowLayoutInDisplayCutoutMode" id="0x01010586"/>
+  <public type="style" name="Widget.DeviceDefault.Button.Colored" id="0x010302e0"/>
+  <public type="style" name="Widget.DeviceDefault.Button.Borderless.Colored" id="0x010302e1"/>
+  <public type="id" name="accessibilityActionShowTooltip" id="0x01020044"/>
+  <public type="id" name="accessibilityActionHideTooltip" id="0x01020045"/>
+  <!-- An interpolator which accelerates fast but decelerates extra slowly. -->
+  <public type="interpolator" name="fast_out_extra_slow_in" id="0x10c001a"/>
+  <!-- ===============================================================
+       Resources added in version Q of the platform
        =============================================================== -->
+  <eat-comment/>
+  <public type="attr" name="packageType" id="0x01010587"/>
+  <public type="attr" name="opticalInsetLeft" id="0x01010588"/>
+  <public type="attr" name="opticalInsetTop" id="0x01010589"/>
+  <public type="attr" name="opticalInsetRight" id="0x0101058a"/>
+  <public type="attr" name="opticalInsetBottom" id="0x0101058b"/>
+  <public type="attr" name="forceDarkAllowed" id="0x0101058c"/>
+  <!-- @hide @SystemApi -->
+  <public type="attr" name="supportsAmbientMode" id="0x0101058d"/>
+  <!-- @hide For use by platform and tools only. Developers should not specify this value. -->
+  <public type="attr" name="usesNonSdkApi" id="0x0101058e"/>
+  <public type="attr" name="nonInteractiveUiTimeout" id="0x0101058f"/>
+  <public type="attr" name="isLightTheme" id="0x01010590"/>
+  <!-- {@deprecated Use requiredSplitTypes instead.} -->
+  <public type="attr" name="isSplitRequired" id="0x01010591"/>
+  <public type="attr" name="textLocale" id="0x01010592"/>
+  <public type="attr" name="settingsSliceUri" id="0x01010593"/>
+  <public type="attr" name="shell" id="0x01010594"/>
+  <public type="attr" name="interactiveUiTimeout" id="0x01010595"/>
+  <public type="attr" name="supportsMultipleDisplays" id="0x01010596"/>
+  <public type="attr" name="useAppZygote" id="0x01010597"/>
+  <public type="attr" name="selectionDividerHeight" id="0x01010598"/>
+  <public type="attr" name="foregroundServiceType" id="0x01010599"/>
+  <public type="attr" name="hasFragileUserData" id="0x0101059a"/>
+  <public type="attr" name="minAspectRatio" id="0x0101059b"/>
+  <public type="attr" name="inheritShowWhenLocked" id="0x0101059c"/>
+  <public type="attr" name="zygotePreloadName" id="0x0101059d"/>
+  <public type="attr" name="useEmbeddedDex" id="0x0101059e"/>
+  <public type="attr" name="forceUriPermissions" id="0x0101059f"/>
+  <!-- @hide @SystemApi -->
+  <public type="attr" name="allowClearUserDataOnFailedRestore" id="0x01010600"/>
+  <public type="attr" name="allowAudioPlaybackCapture" id="0x01010601"/>
+  <public type="attr" name="secureElementName" id="0x01010602"/>
+  <public type="attr" name="requestLegacyExternalStorage" id="0x01010603"/>
+  <public type="attr" name="enforceStatusBarContrast" id="0x01010604"/>
+  <public type="attr" name="enforceNavigationBarContrast" id="0x01010605"/>
+  <public type="attr" name="identifier" id="0x01010606"/>
+  <!-- @hide @SystemApi -->
+  <public type="drawable" name="ic_info" id="0x010800b4"/>
+  <!-- @hide @SystemApi -->
+  <public type="style" name="Theme.DeviceDefault.DocumentsUI" id="0x010302e2"/>
+  <public type="style" name="Theme.DeviceDefault.DayNight" id="0x010302e3"/>
+  <public type="style" name="ThemeOverlay.DeviceDefault.Accent.DayNight" id="0x010302e4"/>
+  <public type="id" name="accessibilityActionPageUp" id="0x01020046"/>
+  <public type="id" name="accessibilityActionPageDown" id="0x01020047"/>
+  <public type="id" name="accessibilityActionPageLeft" id="0x01020048"/>
+  <public type="id" name="accessibilityActionPageRight" id="0x01020049"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_helpPackageNameKey" id="0x0104001b"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_helpPackageNameValue" id="0x0104001c"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_helpIntentExtraKey" id="0x0104001d"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_helpIntentNameKey" id="0x0104001e"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_feedbackIntentExtraKey" id="0x0104001f"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_feedbackIntentNameKey" id="0x01040020"/>
+  <!-- @hide @SystemApi @TestApi -->
+  <public type="string" name="config_defaultAssistant" id="0x01040021"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_defaultBrowser" id="0x01040022"/>
+  <!-- @hide @SystemApi @TestApi -->
+  <public type="string" name="config_defaultDialer" id="0x01040023"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_defaultSms" id="0x01040024"/>
+  <!-- @hide @SystemApi -->
+  <public type="bool" name="config_sendPackageName" id="0x01110000"/>
+  <!-- @hide @SystemApi -->
+  <public type="bool" name="config_showDefaultAssistant" id="0x01110001"/>
+  <!-- @hide @SystemApi -->
+  <public type="bool" name="config_showDefaultEmergency" id="0x01110002"/>
+  <!-- @hide @SystemApi -->
+  <public type="bool" name="config_showDefaultHome" id="0x01110003"/>
+  <!-- @hide @TestApi -->
+  <public type="bool" name="config_perDisplayFocusEnabled" id="0x01110004"/>
+  <!-- @hide @SystemApi -->
+  <public type="dimen" name="config_restrictedIconSize" id="0x01050007"/>
+  <!-- @hide @SystemApi -->
+  <public type="color" name="system_notification_accent_color" id="0x0106001c"/>
+  <!-- ===============================================================
+     Resources added in version R of the platform
+     =============================================================== -->
+  <eat-comment/>
+  <public type="attr" name="importantForContentCapture" id="0x01010607"/>
+  <public type="attr" name="forceQueryable" id="0x01010608"/>
+  <public type="attr" name="resourcesMap" id="0x01010609"/>
+  <public type="attr" name="animatedImageDrawable" id="0x0101060a"/>
+  <public type="attr" name="htmlDescription" id="0x0101060b"/>
+  <public type="attr" name="preferMinimalPostProcessing" id="0x0101060c"/>
+  <public type="attr" name="supportsInlineSuggestions" id="0x0101060d"/>
+  <public type="attr" name="crossProfile" id="0x0101060e"/>
+  <public type="attr" name="canTakeScreenshot" id="0x0101060f"/>
+  <!-- @hide @SystemApi -->
+  <public type="attr" name="sdkVersion" id="0x01010610"/>
+  <!-- @hide @SystemApi -->
+  <public type="attr" name="minExtensionVersion" id="0x01010611"/>
+  <public type="attr" name="allowNativeHeapPointerTagging" id="0x01010612"/>
+  <public type="attr" name="autoRevokePermissions" id="0x01010613"/>
+  <public type="attr" name="preserveLegacyExternalStorage" id="0x01010614"/>
+  <public type="attr" name="mimeGroup" id="0x01010615"/>
+  <public type="attr" name="gwpAsanMode" id="0x01010616"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_defaultCallRedirection" id="0x01040025"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_defaultCallScreening" id="0x01040026"/>
+  <!-- @hide @SystemApi @TestApi -->
+  <public type="string" name="config_systemGallery" id="0x01040027"/>
+  <public type="id" name="accessibilityActionPressAndHold" id="0x0102004a"/>
+  <public type="id" name="accessibilitySystemActionBack" id="0x0102004b"/>
+  <public type="id" name="accessibilitySystemActionHome" id="0x0102004c"/>
+  <public type="id" name="accessibilitySystemActionRecents" id="0x0102004d"/>
+  <public type="id" name="accessibilitySystemActionNotifications" id="0x0102004e"/>
+  <public type="id" name="accessibilitySystemActionQuickSettings" id="0x0102004f"/>
+  <public type="id" name="accessibilitySystemActionPowerDialog" id="0x01020050"/>
+  <public type="id" name="accessibilitySystemActionToggleSplitScreen" id="0x01020051"/>
+  <public type="id" name="accessibilitySystemActionLockScreen" id="0x01020052"/>
+  <public type="id" name="accessibilitySystemActionTakeScreenshot" id="0x01020053"/>
+  <public type="id" name="accessibilityActionImeEnter" id="0x01020054"/>
+  <!-- @hide @TestApi -->
+  <public type="bool" name="config_assistantOnTopOfDream" id="0x01110005"/>
+  <!-- @hide @TestApi -->
+  <public type="bool" name="config_remoteInsetsControllerControlsSystemBars" id="0x01110006"/>
+  <!-- ===============================================================
+     Resources added in version S of the platform
+     =============================================================== -->
+  <eat-comment/>
+  <public type="attr" name="rollbackDataPolicy" id="0x01010617"/>
+  <public type="attr" name="allowClickWhenDisabled" id="0x01010618"/>
+  <public type="attr" name="windowLayoutAffinity" id="0x01010619"/>
+  <public type="attr" name="canPauseRecording" id="0x0101061a"/>
+  <public type="attr" name="windowBlurBehindRadius" id="0x0101061b"/>
+  <public type="attr" name="windowBlurBehindEnabled" id="0x0101061c"/>
+  <public type="attr" name="requireDeviceScreenOn" id="0x0101061d"/>
+  <public type="attr" name="pathSuffix" id="0x0101061e"/>
+  <public type="attr" name="sspSuffix" id="0x0101061f"/>
+  <public type="attr" name="pathAdvancedPattern" id="0x01010620"/>
+  <public type="attr" name="sspAdvancedPattern" id="0x01010621"/>
+  <public type="attr" name="fontProviderSystemFontFamily" id="0x01010622"/>
+  <public type="attr" name="hand_second" id="0x01010623"/>
+  <public type="attr" name="memtagMode" id="0x01010624"/>
+  <public type="attr" name="nativeHeapZeroInitialized" id="0x01010625"/>
+  <!-- @hide @SystemApi -->
+  <public type="attr" name="hotwordDetectionService" id="0x01010626"/>
+  <public type="attr" name="previewLayout" id="0x01010627"/>
+  <public type="attr" name="clipToOutline" id="0x01010628"/>
+  <!-- <public type="attr" name="__removed3" id="0x01010629" /> -->
+  <public type="attr" name="knownCerts" id="0x0101062a"/>
+  <public type="attr" name="windowBackgroundBlurRadius" id="0x0101062b"/>
+  <public type="attr" name="windowSplashScreenBackground" id="0x0101062c"/>
+  <public type="attr" name="windowSplashScreenAnimatedIcon" id="0x0101062d"/>
+  <public type="attr" name="windowSplashScreenAnimationDuration" id="0x0101062e"/>
+  <public type="attr" name="windowSplashScreenBrandingImage" id="0x0101062f"/>
+  <public type="attr" name="windowSplashScreenIconBackgroundColor" id="0x01010630"/>
+  <public type="attr" name="splashScreenTheme" id="0x01010631"/>
+  <public type="attr" name="maxResizeWidth" id="0x01010632"/>
+  <public type="attr" name="maxResizeHeight" id="0x01010633"/>
+  <public type="attr" name="targetCellWidth" id="0x01010634"/>
+  <public type="attr" name="targetCellHeight" id="0x01010635"/>
+  <public type="attr" name="dialTint" id="0x01010636"/>
+  <public type="attr" name="dialTintMode" id="0x01010637"/>
+  <public type="attr" name="hand_hourTint" id="0x01010638"/>
+  <public type="attr" name="hand_hourTintMode" id="0x01010639"/>
+  <public type="attr" name="hand_minuteTint" id="0x0101063a"/>
+  <public type="attr" name="hand_minuteTintMode" id="0x0101063b"/>
+  <public type="attr" name="hand_secondTint" id="0x0101063c"/>
+  <public type="attr" name="hand_secondTintMode" id="0x0101063d"/>
+  <public type="attr" name="dataExtractionRules" id="0x0101063e"/>
+  <public type="attr" name="passwordsActivity" id="0x0101063f"/>
+  <public type="attr" name="selectableAsDefault" id="0x01010640"/>
+  <public type="attr" name="isAccessibilityTool" id="0x01010641"/>
+  <public type="attr" name="attributionTags" id="0x01010642"/>
+  <public type="attr" name="suppressesSpellChecker" id="0x01010643"/>
+  <public type="attr" name="usesPermissionFlags" id="0x01010644"/>
+  <public type="attr" name="requestRawExternalStorageAccess" id="0x01010645"/>
+  <!-- @hide @SystemApi -->
+  <public type="attr" name="playHomeTransitionSound" id="0x01010646"/>
+  <public type="attr" name="lStar" id="0x01010647"/>
+  <public type="attr" name="showInInputMethodPicker" id="0x01010648"/>
+  <public type="attr" name="effectColor" id="0x01010649"/>
+  <!-- @hide @TestApi -->
+  <public type="attr" name="requestForegroundServiceExemption" id="0x0101064a"/>
+  <public type="attr" name="attributionsAreUserVisible" id="0x0101064b"/>
+  <public type="color" name="system_neutral1_0" id="0x0106001d"/>
+  <public type="color" name="system_neutral1_10" id="0x0106001e"/>
+  <public type="color" name="system_neutral1_50" id="0x0106001f"/>
+  <public type="color" name="system_neutral1_100" id="0x01060020"/>
+  <public type="color" name="system_neutral1_200" id="0x01060021"/>
+  <public type="color" name="system_neutral1_300" id="0x01060022"/>
+  <public type="color" name="system_neutral1_400" id="0x01060023"/>
+  <public type="color" name="system_neutral1_500" id="0x01060024"/>
+  <public type="color" name="system_neutral1_600" id="0x01060025"/>
+  <public type="color" name="system_neutral1_700" id="0x01060026"/>
+  <public type="color" name="system_neutral1_800" id="0x01060027"/>
+  <public type="color" name="system_neutral1_900" id="0x01060028"/>
+  <public type="color" name="system_neutral1_1000" id="0x01060029"/>
+  <public type="color" name="system_neutral2_0" id="0x0106002a"/>
+  <public type="color" name="system_neutral2_10" id="0x0106002b"/>
+  <public type="color" name="system_neutral2_50" id="0x0106002c"/>
+  <public type="color" name="system_neutral2_100" id="0x0106002d"/>
+  <public type="color" name="system_neutral2_200" id="0x0106002e"/>
+  <public type="color" name="system_neutral2_300" id="0x0106002f"/>
+  <public type="color" name="system_neutral2_400" id="0x01060030"/>
+  <public type="color" name="system_neutral2_500" id="0x01060031"/>
+  <public type="color" name="system_neutral2_600" id="0x01060032"/>
+  <public type="color" name="system_neutral2_700" id="0x01060033"/>
+  <public type="color" name="system_neutral2_800" id="0x01060034"/>
+  <public type="color" name="system_neutral2_900" id="0x01060035"/>
+  <public type="color" name="system_neutral2_1000" id="0x01060036"/>
+  <public type="color" name="system_accent1_0" id="0x01060037"/>
+  <public type="color" name="system_accent1_10" id="0x01060038"/>
+  <public type="color" name="system_accent1_50" id="0x01060039"/>
+  <public type="color" name="system_accent1_100" id="0x0106003a"/>
+  <public type="color" name="system_accent1_200" id="0x0106003b"/>
+  <public type="color" name="system_accent1_300" id="0x0106003c"/>
+  <public type="color" name="system_accent1_400" id="0x0106003d"/>
+  <public type="color" name="system_accent1_500" id="0x0106003e"/>
+  <public type="color" name="system_accent1_600" id="0x0106003f"/>
+  <public type="color" name="system_accent1_700" id="0x01060040"/>
+  <public type="color" name="system_accent1_800" id="0x01060041"/>
+  <public type="color" name="system_accent1_900" id="0x01060042"/>
+  <public type="color" name="system_accent1_1000" id="0x01060043"/>
+  <public type="color" name="system_accent2_0" id="0x01060044"/>
+  <public type="color" name="system_accent2_10" id="0x01060045"/>
+  <public type="color" name="system_accent2_50" id="0x01060046"/>
+  <public type="color" name="system_accent2_100" id="0x01060047"/>
+  <public type="color" name="system_accent2_200" id="0x01060048"/>
+  <public type="color" name="system_accent2_300" id="0x01060049"/>
+  <public type="color" name="system_accent2_400" id="0x0106004a"/>
+  <public type="color" name="system_accent2_500" id="0x0106004b"/>
+  <public type="color" name="system_accent2_600" id="0x0106004c"/>
+  <public type="color" name="system_accent2_700" id="0x0106004d"/>
+  <public type="color" name="system_accent2_800" id="0x0106004e"/>
+  <public type="color" name="system_accent2_900" id="0x0106004f"/>
+  <public type="color" name="system_accent2_1000" id="0x01060050"/>
+  <public type="color" name="system_accent3_0" id="0x01060051"/>
+  <public type="color" name="system_accent3_10" id="0x01060052"/>
+  <public type="color" name="system_accent3_50" id="0x01060053"/>
+  <public type="color" name="system_accent3_100" id="0x01060054"/>
+  <public type="color" name="system_accent3_200" id="0x01060055"/>
+  <public type="color" name="system_accent3_300" id="0x01060056"/>
+  <public type="color" name="system_accent3_400" id="0x01060057"/>
+  <public type="color" name="system_accent3_500" id="0x01060058"/>
+  <public type="color" name="system_accent3_600" id="0x01060059"/>
+  <public type="color" name="system_accent3_700" id="0x0106005a"/>
+  <public type="color" name="system_accent3_800" id="0x0106005b"/>
+  <public type="color" name="system_accent3_900" id="0x0106005c"/>
+  <public type="color" name="system_accent3_1000" id="0x0106005d"/>
+  <public type="dimen" name="system_app_widget_background_radius" id="0x01050008"/>
+  <public type="dimen" name="system_app_widget_inner_radius" id="0x01050009"/>
+  <!-- @hide @SystemApi @TestApi -->
+  <public type="string" name="config_systemAutomotiveCluster" id="0x01040028"/>
+  <!-- @hide @SystemApi @TestApi -->
+  <public type="string" name="config_systemAutomotiveProjection" id="0x01040029"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemShell" id="0x0104002a"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemContacts" id="0x0104002b"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_customMediaKeyDispatcher" id="0x0104002c"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_customMediaSessionPolicyProvider" id="0x0104002d"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemSpeechRecognizer" id="0x0104002e"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemWifiCoexManager" id="0x0104002f"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemWellbeing" id="0x01040030"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemTelevisionNotificationHandler" id="0x01040031"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemUiIntelligence" id="0x01040032"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemAmbientAudioIntelligence" id="0x01040033"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemAudioIntelligence" id="0x01040034"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemNotificationIntelligence" id="0x01040035"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemTextIntelligence" id="0x01040036"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemVisualIntelligence" id="0x01040037"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemActivityRecognizer" id="0x01040038"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemCompanionDeviceProvider" id="0x01040039"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemUi" id="0x0104003a"/>
+  <!-- @hide For use by platform and tools only. Developers should not specify this value. -->
+  <public type="string" name="config_defaultRingtoneVibrationSound" id="0x0104003b"/>
+  <!-- ===============================================================
+    Resources added in version S-V2 of the platform
+    =============================================================== -->
+  <eat-comment/>
+  <staging-public-group-final type="attr" first-id="0x01ff0000">
+    <public name="shouldUseDefaultUnfoldTransition"/>
+  </staging-public-group-final>
+  <public type="attr" name="shouldUseDefaultUnfoldTransition" id="0x0101064c"/>
+  <staging-public-group-final type="id" first-id="0x01fe0000">
+    <public name="accessibilityActionDragStart"/>
+    <public name="accessibilityActionDragDrop"/>
+    <public name="accessibilityActionDragCancel"/>
+  </staging-public-group-final>
+  <public type="id" name="accessibilityActionDragStart" id="0x01020055"/>
+  <public type="id" name="accessibilityActionDragDrop" id="0x01020056"/>
+  <public type="id" name="accessibilityActionDragCancel" id="0x01020057"/>
+  <!-- ===============================================================
+    Resources added in version T of the platform
+
+    NOTE: After this version of the platform is forked, changes cannot be made to the root
+    branch's groups for that release. Only merge changes to the forked platform branch.
+    =============================================================== -->
+  <eat-comment/>
+  <staging-public-group-final type="attr" first-id="0x01df0000">
+    <public name="sharedUserMaxSdkVersion"/>
+    <public name="requiredSplitTypes"/>
+    <public name="splitTypes"/>
+    <public name="canDisplayOnRemoteDevices"/>
+    <public name="supportedTypes"/>
+    <public name="resetEnabledSettingsOnAppDataCleared"/>
+    <public name="supportsStylusHandwriting"/>
+    <public name="showClockAndComplications"/>
+    <!-- @hide @SystemApi -->
+    <public name="gameSessionService"/>
+    <public name="supportsBatteryGameMode"/>
+    <public name="supportsPerformanceGameMode"/>
+    <public name="allowGameAngleDriver"/>
+    <public name="allowGameDownscaling"/>
+    <public name="allowGameFpsOverride"/>
+    <public name="localeConfig"/>
+    <public name="showBackdrop"/>
+    <public name="removed_useTargetActivityForQuickAccess"/>
+    <public name="removed_inheritKeyStoreKeys"/>
+    <public name="preferKeepClear"/>
+    <public name="autoHandwritingEnabled"/>
+    <public name="fromExtendLeft"/>
+    <public name="fromExtendTop"/>
+    <public name="fromExtendRight"/>
+    <public name="fromExtendBottom"/>
+    <public name="toExtendLeft"/>
+    <public name="toExtendTop"/>
+    <public name="toExtendRight"/>
+    <public name="toExtendBottom"/>
+    <public name="tileService"/>
+    <public name="windowSplashScreenBehavior"/>
+    <public name="allowUntrustedActivityEmbedding"/>
+    <public name="knownActivityEmbeddingCerts"/>
+    <public name="intro"/>
+    <public name="enableOnBackInvokedCallback"/>
+    <public name="supportsInlineSuggestionsWithTouchExploration"/>
+    <public name="lineBreakStyle"/>
+    <public name="lineBreakWordStyle"/>
+    <!-- @hide -->
+    <public name="maxDrawableWidth"/>
+    <!-- @hide -->
+    <public name="maxDrawableHeight"/>
+    <public name="backdropColor"/>
+  </staging-public-group-final>
+  <public type="attr" name="sharedUserMaxSdkVersion" id="0x0101064d"/>
+  <public type="attr" name="requiredSplitTypes" id="0x0101064e"/>
+  <public type="attr" name="splitTypes" id="0x0101064f"/>
+  <public type="attr" name="canDisplayOnRemoteDevices" id="0x01010650"/>
+  <public type="attr" name="supportedTypes" id="0x01010651"/>
+  <public type="attr" name="resetEnabledSettingsOnAppDataCleared" id="0x01010652"/>
+  <public type="attr" name="supportsStylusHandwriting" id="0x01010653"/>
+  <public type="attr" name="showClockAndComplications" id="0x01010654"/>
+  <!-- @hide @SystemApi -->
+  <public type="attr" name="gameSessionService" id="0x01010655"/>
+  <public type="attr" name="supportsBatteryGameMode" id="0x01010656"/>
+  <public type="attr" name="supportsPerformanceGameMode" id="0x01010657"/>
+  <public type="attr" name="allowGameAngleDriver" id="0x01010658"/>
+  <public type="attr" name="allowGameDownscaling" id="0x01010659"/>
+  <public type="attr" name="allowGameFpsOverride" id="0x0101065a"/>
+  <public type="attr" name="localeConfig" id="0x0101065b"/>
+  <public type="attr" name="showBackdrop" id="0x0101065c"/>
+  <public type="attr" name="preferKeepClear" id="0x0101065d"/>
+  <public type="attr" name="autoHandwritingEnabled" id="0x0101065e"/>
+  <public type="attr" name="fromExtendLeft" id="0x0101065f"/>
+  <public type="attr" name="fromExtendTop" id="0x01010660"/>
+  <public type="attr" name="fromExtendRight" id="0x01010661"/>
+  <public type="attr" name="fromExtendBottom" id="0x01010662"/>
+  <public type="attr" name="toExtendLeft" id="0x01010663"/>
+  <public type="attr" name="toExtendTop" id="0x01010664"/>
+  <public type="attr" name="toExtendRight" id="0x01010665"/>
+  <public type="attr" name="toExtendBottom" id="0x01010666"/>
+  <public type="attr" name="tileService" id="0x01010667"/>
+  <public type="attr" name="windowSplashScreenBehavior" id="0x01010668"/>
+  <public type="attr" name="allowUntrustedActivityEmbedding" id="0x01010669"/>
+  <public type="attr" name="knownActivityEmbeddingCerts" id="0x0101066a"/>
+  <public type="attr" name="intro" id="0x0101066b"/>
+  <public type="attr" name="enableOnBackInvokedCallback" id="0x0101066c"/>
+  <public type="attr" name="supportsInlineSuggestionsWithTouchExploration" id="0x0101066d"/>
+  <public type="attr" name="lineBreakStyle" id="0x0101066e"/>
+  <public type="attr" name="lineBreakWordStyle" id="0x0101066f"/>
+  <!-- @hide -->
+  <public type="attr" name="maxDrawableWidth" id="0x01010670"/>
+  <!-- @hide -->
+  <public type="attr" name="maxDrawableHeight" id="0x01010671"/>
+  <public type="attr" name="backdropColor" id="0x01010672"/>
+  <staging-public-group-final type="id" first-id="0x01de0000">
+    <public name="removed_accessibilityActionSwipeLeft"/>
+    <public name="removed_accessibilityActionSwipeRight"/>
+    <public name="removed_accessibilityActionSwipeUp"/>
+    <public name="removed_accessibilityActionSwipeDown"/>
+    <public name="accessibilityActionShowTextSuggestions"/>
+    <public name="inputExtractAction"/>
+    <public name="inputExtractAccessories"/>
+  </staging-public-group-final>
+  <public type="id" name="accessibilityActionShowTextSuggestions" id="0x01020058"/>
+  <public type="id" name="inputExtractAction" id="0x01020059"/>
+  <public type="id" name="inputExtractAccessories" id="0x0102005a"/>
+  <staging-public-group-final type="style" first-id="0x01dd0000">
+    <public name="TextAppearance.DeviceDefault.Headline"/>
+  </staging-public-group-final>
+  <public type="style" name="TextAppearance.DeviceDefault.Headline" id="0x010302e5"/>
+  <staging-public-group-final type="string" first-id="0x01dc0000">
+    <!-- @hide @SystemApi -->
+    <public name="config_systemSupervision"/>
+    <!-- @hide @SystemApi -->
+    <public name="config_devicePolicyManagement"/>
+    <!-- @hide @SystemApi -->
+    <public name="config_systemAppProtectionService"/>
+    <!-- @hide @SystemApi @TestApi -->
+    <public name="config_systemAutomotiveCalendarSyncManager"/>
+    <!-- @hide @SystemApi -->
+    <public name="config_defaultAutomotiveNavigation"/>
+    <!-- @hide @SystemApi -->
+    <public name="safety_protection_display_text"/>
+    <!-- @hide @SystemApi -->
+    <public name="config_systemSettingsIntelligence"/>
+    <!-- @hide -->
+    <public name="config_systemBluetoothStack"/>
+  </staging-public-group-final>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemSupervision" id="0x0104003c"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_devicePolicyManagement" id="0x0104003d"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemAppProtectionService" id="0x0104003e"/>
+  <!-- @hide @SystemApi @TestApi -->
+  <public type="string" name="config_systemAutomotiveCalendarSyncManager" id="0x0104003f"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_defaultAutomotiveNavigation" id="0x01040040"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="safety_protection_display_text" id="0x01040041"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemSettingsIntelligence" id="0x01040042"/>
+  <!-- @hide -->
+  <public type="string" name="config_systemBluetoothStack" id="0x01040043"/>
+  <staging-public-group-final type="array" first-id="0x01d90000">
+    <!-- @hide @SystemApi -->
+    <public name="config_optionalIpSecAlgorithms"/>
+  </staging-public-group-final>
+  <!-- @hide @SystemApi -->
+  <public type="array" name="config_optionalIpSecAlgorithms" id="0x01070006"/>
+  <staging-public-group-final type="drawable" first-id="0x01d80000">
+    <!-- @hide @SystemApi -->
+    <public name="ic_safety_protection"/>
+  </staging-public-group-final>
+  <!-- @hide @SystemApi -->
+  <public type="drawable" name="ic_safety_protection" id="0x010800b5"/>
+  <staging-public-group-final type="bool" first-id="0x01cf0000">
+    <!-- @hide @TestApi -->
+    <public name="config_preventImeStartupUnlessTextEditor"/>
+    <!-- @hide @SystemApi -->
+    <public name="config_enableQrCodeScannerOnLockScreen"/>
+  </staging-public-group-final>
+  <!-- @hide @TestApi -->
+  <public type="bool" name="config_preventImeStartupUnlessTextEditor" id="0x01110007"/>
+  <!-- @hide @SystemApi -->
+  <public type="bool" name="config_enableQrCodeScannerOnLockScreen" id="0x01110008"/>
+  <!-- ===============================================================
+    Resources added in version U of the platform
+
+    NOTE: After this version of the platform is forked, changes cannot be made to the root
+    branch's groups for that release. Only merge changes to the forked platform branch.
+    =============================================================== -->
+  <eat-comment/>
+  <staging-public-group-final type="attr" first-id="0x01ce0000">
+    <public name="handwritingBoundsOffsetLeft"/>
+    <public name="handwritingBoundsOffsetTop"/>
+    <public name="handwritingBoundsOffsetRight"/>
+    <public name="handwritingBoundsOffsetBottom"/>
+    <public name="accessibilityDataSensitive"/>
+    <public name="enableTextStylingShortcuts"/>
+    <public name="requiredDisplayCategory"/>
+    <public name="removed_maxConcurrentSessionsCount"/>
+    <public name="visualQueryDetectionService"/>
+    <public name="physicalKeyboardHintLanguageTag"/>
+    <public name="physicalKeyboardHintLayoutType"/>
+    <public name="allowSharedIsolatedProcess"/>
+    <public name="keyboardLocale"/>
+    <public name="keyboardLayoutType"/>
+    <public name="allowUpdateOwnership"/>
+    <public name="isCredential"/>
+    <public name="searchResultHighlightColor"/>
+    <public name="focusedSearchResultHighlightColor"/>
+    <public name="stylusHandwritingSettingsActivity"/>
+    <public name="windowNoMoveAnimation"/>
+    <public name="settingsSubtitle"/>
+    <public name="capability"/>
+  </staging-public-group-final>
+  <public type="attr" name="handwritingBoundsOffsetLeft" id="0x01010673"/>
+  <public type="attr" name="handwritingBoundsOffsetTop" id="0x01010674"/>
+  <public type="attr" name="handwritingBoundsOffsetRight" id="0x01010675"/>
+  <public type="attr" name="handwritingBoundsOffsetBottom" id="0x01010676"/>
+  <public type="attr" name="accessibilityDataSensitive" id="0x01010677"/>
+  <public type="attr" name="enableTextStylingShortcuts" id="0x01010678"/>
+  <public type="attr" name="requiredDisplayCategory" id="0x01010679"/>
+  <public type="attr" name="visualQueryDetectionService" id="0x0101067a"/>
+  <public type="attr" name="physicalKeyboardHintLanguageTag" id="0x0101067b"/>
+  <public type="attr" name="physicalKeyboardHintLayoutType" id="0x0101067c"/>
+  <public type="attr" name="allowSharedIsolatedProcess" id="0x0101067d"/>
+  <public type="attr" name="keyboardLocale" id="0x0101067e"/>
+  <public type="attr" name="keyboardLayoutType" id="0x0101067f"/>
+  <public type="attr" name="allowUpdateOwnership" id="0x01010680"/>
+  <public type="attr" name="isCredential" id="0x01010681"/>
+  <public type="attr" name="searchResultHighlightColor" id="0x01010682"/>
+  <public type="attr" name="focusedSearchResultHighlightColor" id="0x01010683"/>
+  <public type="attr" name="stylusHandwritingSettingsActivity" id="0x01010684"/>
+  <public type="attr" name="windowNoMoveAnimation" id="0x01010685"/>
+  <public type="attr" name="settingsSubtitle" id="0x01010686"/>
+  <public type="attr" name="capability" id="0x01010687"/>
+  <staging-public-group-final type="id" first-id="0x01cd0000">
+    <public name="bold"/>
+    <public name="italic"/>
+    <public name="underline"/>
+    <public name="accessibilityActionScrollInDirection"/>
+  </staging-public-group-final>
+  <public type="id" name="bold" id="0x0102005b"/>
+  <public type="id" name="italic" id="0x0102005c"/>
+  <public type="id" name="underline" id="0x0102005d"/>
+  <public type="id" name="accessibilityActionScrollInDirection" id="0x0102005e"/>
+  <staging-public-group-final type="string" first-id="0x01cb0000">
+    <!-- @hide @SystemApi -->
+    <public name="config_systemWearHealthService"/>
+    <!-- @hide @SystemApi -->
+    <public name="config_defaultNotes"/>
+    <!-- @hide @SystemApi -->
+    <public name="config_systemFinancedDeviceController"/>
+    <!-- @hide @SystemApi -->
+    <public name="config_systemCallStreaming"/>
+  </staging-public-group-final>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemWearHealthService" id="0x01040044"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_defaultNotes" id="0x01040045"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemFinancedDeviceController" id="0x01040046"/>
+  <!-- @hide @SystemApi -->
+  <public type="string" name="config_systemCallStreaming" id="0x01040047"/>
+  <staging-public-group-final type="dimen" first-id="0x01ca0000">
+    <!-- @hide @SystemApi -->
+    <public name="config_viewConfigurationHandwritingGestureLineMargin"/>
+  </staging-public-group-final>
+  <!-- @hide @SystemApi -->
+  <public type="dimen" name="config_viewConfigurationHandwritingGestureLineMargin" id="0x0105000a"/>
+  <staging-public-group-final type="color" first-id="0x01c90000">
+    <public name="system_primary_container_light"/>
+    <public name="system_on_primary_container_light"/>
+    <public name="system_primary_light"/>
+    <public name="system_on_primary_light"/>
+    <public name="system_secondary_container_light"/>
+    <public name="system_on_secondary_container_light"/>
+    <public name="system_secondary_light"/>
+    <public name="system_on_secondary_light"/>
+    <public name="system_tertiary_container_light"/>
+    <public name="system_on_tertiary_container_light"/>
+    <public name="system_tertiary_light"/>
+    <public name="system_on_tertiary_light"/>
+    <public name="system_background_light"/>
+    <public name="system_on_background_light"/>
+    <public name="system_surface_light"/>
+    <public name="system_on_surface_light"/>
+    <public name="system_surface_container_low_light"/>
+    <public name="system_surface_container_lowest_light"/>
+    <public name="system_surface_container_light"/>
+    <public name="system_surface_container_high_light"/>
+    <public name="system_surface_container_highest_light"/>
+    <public name="system_surface_bright_light"/>
+    <public name="system_surface_dim_light"/>
+    <public name="system_surface_variant_light"/>
+    <public name="system_on_surface_variant_light"/>
+    <public name="system_outline_light"/>
+    <public name="system_error_light"/>
+    <public name="system_on_error_light"/>
+    <public name="system_error_container_light"/>
+    <public name="system_on_error_container_light"/>
+    <public name="removed_system_primary_fixed_light"/>
+    <public name="removed_system_primary_fixed_dim_light"/>
+    <public name="removed_system_on_primary_fixed_light"/>
+    <public name="removed_system_on_primary_fixed_variant_light"/>
+    <public name="removed_system_secondary_fixed_light"/>
+    <public name="removed_system_secondary_fixed_dim_light"/>
+    <public name="removed_system_on_secondary_fixed_light"/>
+    <public name="removed_system_on_secondary_fixed_variant_light"/>
+    <public name="removed_system_tertiary_fixed_light"/>
+    <public name="removed_system_tertiary_fixed_dim_light"/>
+    <public name="removed_system_on_tertiary_fixed_light"/>
+    <public name="removed_system_on_tertiary_fixed_variant_light"/>
+    <public name="system_control_activated_light"/>
+    <public name="system_control_normal_light"/>
+    <public name="system_control_highlight_light"/>
+    <public name="system_text_primary_inverse_light"/>
+    <public name="system_text_secondary_and_tertiary_inverse_light"/>
+    <public name="system_text_primary_inverse_disable_only_light"/>
+    <public name="system_text_secondary_and_tertiary_inverse_disabled_light"/>
+    <public name="system_text_hint_inverse_light"/>
+    <public name="system_palette_key_color_primary_light"/>
+    <public name="system_palette_key_color_secondary_light"/>
+    <public name="system_palette_key_color_tertiary_light"/>
+    <public name="system_palette_key_color_neutral_light"/>
+    <public name="system_palette_key_color_neutral_variant_light"/>
+    <public name="system_primary_container_dark"/>
+    <public name="system_on_primary_container_dark"/>
+    <public name="system_primary_dark"/>
+    <public name="system_on_primary_dark"/>
+    <public name="system_secondary_container_dark"/>
+    <public name="system_on_secondary_container_dark"/>
+    <public name="system_secondary_dark"/>
+    <public name="system_on_secondary_dark"/>
+    <public name="system_tertiary_container_dark"/>
+    <public name="system_on_tertiary_container_dark"/>
+    <public name="system_tertiary_dark"/>
+    <public name="system_on_tertiary_dark"/>
+    <public name="system_background_dark"/>
+    <public name="system_on_background_dark"/>
+    <public name="system_surface_dark"/>
+    <public name="system_on_surface_dark"/>
+    <public name="system_surface_container_low_dark"/>
+    <public name="system_surface_container_lowest_dark"/>
+    <public name="system_surface_container_dark"/>
+    <public name="system_surface_container_high_dark"/>
+    <public name="system_surface_container_highest_dark"/>
+    <public name="system_surface_bright_dark"/>
+    <public name="system_surface_dim_dark"/>
+    <public name="system_surface_variant_dark"/>
+    <public name="system_on_surface_variant_dark"/>
+    <public name="system_outline_dark"/>
+    <public name="system_error_dark"/>
+    <public name="system_on_error_dark"/>
+    <public name="system_error_container_dark"/>
+    <public name="system_on_error_container_dark"/>
+    <public name="removed_system_primary_fixed_dark"/>
+    <public name="removed_system_primary_fixed_dim_dark"/>
+    <public name="removed_system_on_primary_fixed_dark"/>
+    <public name="removed_system_on_primary_fixed_variant_dark"/>
+    <public name="removed_system_secondary_fixed_dark"/>
+    <public name="removed_system_secondary_fixed_dim_dark"/>
+    <public name="removed_system_on_secondary_fixed_dark"/>
+    <public name="removed_system_on_secondary_fixed_variant_dark"/>
+    <public name="removed_system_tertiary_fixed_dark"/>
+    <public name="removed_system_tertiary_fixed_dim_dark"/>
+    <public name="removed_system_on_tertiary_fixed_dark"/>
+    <public name="removed_system_on_tertiary_fixed_variant_dark"/>
+    <public name="system_control_activated_dark"/>
+    <public name="system_control_normal_dark"/>
+    <public name="system_control_highlight_dark"/>
+    <public name="system_text_primary_inverse_dark"/>
+    <public name="system_text_secondary_and_tertiary_inverse_dark"/>
+    <public name="system_text_primary_inverse_disable_only_dark"/>
+    <public name="system_text_secondary_and_tertiary_inverse_disabled_dark"/>
+    <public name="system_text_hint_inverse_dark"/>
+    <public name="system_palette_key_color_primary_dark"/>
+    <public name="system_palette_key_color_secondary_dark"/>
+    <public name="system_palette_key_color_tertiary_dark"/>
+    <public name="system_palette_key_color_neutral_dark"/>
+    <public name="system_palette_key_color_neutral_variant_dark"/>
+    <public name="system_primary_fixed"/>
+    <public name="system_primary_fixed_dim"/>
+    <public name="system_on_primary_fixed"/>
+    <public name="system_on_primary_fixed_variant"/>
+    <public name="system_secondary_fixed"/>
+    <public name="system_secondary_fixed_dim"/>
+    <public name="system_on_secondary_fixed"/>
+    <public name="system_on_secondary_fixed_variant"/>
+    <public name="system_tertiary_fixed"/>
+    <public name="system_tertiary_fixed_dim"/>
+    <public name="system_on_tertiary_fixed"/>
+    <public name="system_on_tertiary_fixed_variant"/>
+    <public name="system_outline_variant_light"/>
+    <public name="system_outline_variant_dark"/>
+  </staging-public-group-final>
+  <public type="color" name="system_primary_container_light" id="0x0106005e"/>
+  <public type="color" name="system_on_primary_container_light" id="0x0106005f"/>
+  <public type="color" name="system_primary_light" id="0x01060060"/>
+  <public type="color" name="system_on_primary_light" id="0x01060061"/>
+  <public type="color" name="system_secondary_container_light" id="0x01060062"/>
+  <public type="color" name="system_on_secondary_container_light" id="0x01060063"/>
+  <public type="color" name="system_secondary_light" id="0x01060064"/>
+  <public type="color" name="system_on_secondary_light" id="0x01060065"/>
+  <public type="color" name="system_tertiary_container_light" id="0x01060066"/>
+  <public type="color" name="system_on_tertiary_container_light" id="0x01060067"/>
+  <public type="color" name="system_tertiary_light" id="0x01060068"/>
+  <public type="color" name="system_on_tertiary_light" id="0x01060069"/>
+  <public type="color" name="system_background_light" id="0x0106006a"/>
+  <public type="color" name="system_on_background_light" id="0x0106006b"/>
+  <public type="color" name="system_surface_light" id="0x0106006c"/>
+  <public type="color" name="system_on_surface_light" id="0x0106006d"/>
+  <public type="color" name="system_surface_container_low_light" id="0x0106006e"/>
+  <public type="color" name="system_surface_container_lowest_light" id="0x0106006f"/>
+  <public type="color" name="system_surface_container_light" id="0x01060070"/>
+  <public type="color" name="system_surface_container_high_light" id="0x01060071"/>
+  <public type="color" name="system_surface_container_highest_light" id="0x01060072"/>
+  <public type="color" name="system_surface_bright_light" id="0x01060073"/>
+  <public type="color" name="system_surface_dim_light" id="0x01060074"/>
+  <public type="color" name="system_surface_variant_light" id="0x01060075"/>
+  <public type="color" name="system_on_surface_variant_light" id="0x01060076"/>
+  <public type="color" name="system_outline_light" id="0x01060077"/>
+  <public type="color" name="system_error_light" id="0x01060078"/>
+  <public type="color" name="system_on_error_light" id="0x01060079"/>
+  <public type="color" name="system_error_container_light" id="0x0106007a"/>
+  <public type="color" name="system_on_error_container_light" id="0x0106007b"/>
+  <public type="color" name="system_control_activated_light" id="0x0106007c"/>
+  <public type="color" name="system_control_normal_light" id="0x0106007d"/>
+  <public type="color" name="system_control_highlight_light" id="0x0106007e"/>
+  <public type="color" name="system_text_primary_inverse_light" id="0x0106007f"/>
+  <public type="color" name="system_text_secondary_and_tertiary_inverse_light" id="0x01060080"/>
+  <public type="color" name="system_text_primary_inverse_disable_only_light" id="0x01060081"/>
+  <public type="color" name="system_text_secondary_and_tertiary_inverse_disabled_light" id="0x01060082"/>
+  <public type="color" name="system_text_hint_inverse_light" id="0x01060083"/>
+  <public type="color" name="system_palette_key_color_primary_light" id="0x01060084"/>
+  <public type="color" name="system_palette_key_color_secondary_light" id="0x01060085"/>
+  <public type="color" name="system_palette_key_color_tertiary_light" id="0x01060086"/>
+  <public type="color" name="system_palette_key_color_neutral_light" id="0x01060087"/>
+  <public type="color" name="system_palette_key_color_neutral_variant_light" id="0x01060088"/>
+  <public type="color" name="system_primary_container_dark" id="0x01060089"/>
+  <public type="color" name="system_on_primary_container_dark" id="0x0106008a"/>
+  <public type="color" name="system_primary_dark" id="0x0106008b"/>
+  <public type="color" name="system_on_primary_dark" id="0x0106008c"/>
+  <public type="color" name="system_secondary_container_dark" id="0x0106008d"/>
+  <public type="color" name="system_on_secondary_container_dark" id="0x0106008e"/>
+  <public type="color" name="system_secondary_dark" id="0x0106008f"/>
+  <public type="color" name="system_on_secondary_dark" id="0x01060090"/>
+  <public type="color" name="system_tertiary_container_dark" id="0x01060091"/>
+  <public type="color" name="system_on_tertiary_container_dark" id="0x01060092"/>
+  <public type="color" name="system_tertiary_dark" id="0x01060093"/>
+  <public type="color" name="system_on_tertiary_dark" id="0x01060094"/>
+  <public type="color" name="system_background_dark" id="0x01060095"/>
+  <public type="color" name="system_on_background_dark" id="0x01060096"/>
+  <public type="color" name="system_surface_dark" id="0x01060097"/>
+  <public type="color" name="system_on_surface_dark" id="0x01060098"/>
+  <public type="color" name="system_surface_container_low_dark" id="0x01060099"/>
+  <public type="color" name="system_surface_container_lowest_dark" id="0x0106009a"/>
+  <public type="color" name="system_surface_container_dark" id="0x0106009b"/>
+  <public type="color" name="system_surface_container_high_dark" id="0x0106009c"/>
+  <public type="color" name="system_surface_container_highest_dark" id="0x0106009d"/>
+  <public type="color" name="system_surface_bright_dark" id="0x0106009e"/>
+  <public type="color" name="system_surface_dim_dark" id="0x0106009f"/>
+  <public type="color" name="system_surface_variant_dark" id="0x010600a0"/>
+  <public type="color" name="system_on_surface_variant_dark" id="0x010600a1"/>
+  <public type="color" name="system_outline_dark" id="0x010600a2"/>
+  <public type="color" name="system_error_dark" id="0x010600a3"/>
+  <public type="color" name="system_on_error_dark" id="0x010600a4"/>
+  <public type="color" name="system_error_container_dark" id="0x010600a5"/>
+  <public type="color" name="system_on_error_container_dark" id="0x010600a6"/>
+  <public type="color" name="system_control_activated_dark" id="0x010600a7"/>
+  <public type="color" name="system_control_normal_dark" id="0x010600a8"/>
+  <public type="color" name="system_control_highlight_dark" id="0x010600a9"/>
+  <public type="color" name="system_text_primary_inverse_dark" id="0x010600aa"/>
+  <public type="color" name="system_text_secondary_and_tertiary_inverse_dark" id="0x010600ab"/>
+  <public type="color" name="system_text_primary_inverse_disable_only_dark" id="0x010600ac"/>
+  <public type="color" name="system_text_secondary_and_tertiary_inverse_disabled_dark" id="0x010600ad"/>
+  <public type="color" name="system_text_hint_inverse_dark" id="0x010600ae"/>
+  <public type="color" name="system_palette_key_color_primary_dark" id="0x010600af"/>
+  <public type="color" name="system_palette_key_color_secondary_dark" id="0x010600b0"/>
+  <public type="color" name="system_palette_key_color_tertiary_dark" id="0x010600b1"/>
+  <public type="color" name="system_palette_key_color_neutral_dark" id="0x010600b2"/>
+  <public type="color" name="system_palette_key_color_neutral_variant_dark" id="0x010600b3"/>
+  <public type="color" name="system_primary_fixed" id="0x010600b4"/>
+  <public type="color" name="system_primary_fixed_dim" id="0x010600b5"/>
+  <public type="color" name="system_on_primary_fixed" id="0x010600b6"/>
+  <public type="color" name="system_on_primary_fixed_variant" id="0x010600b7"/>
+  <public type="color" name="system_secondary_fixed" id="0x010600b8"/>
+  <public type="color" name="system_secondary_fixed_dim" id="0x010600b9"/>
+  <public type="color" name="system_on_secondary_fixed" id="0x010600ba"/>
+  <public type="color" name="system_on_secondary_fixed_variant" id="0x010600bb"/>
+  <public type="color" name="system_tertiary_fixed" id="0x010600bc"/>
+  <public type="color" name="system_tertiary_fixed_dim" id="0x010600bd"/>
+  <public type="color" name="system_on_tertiary_fixed" id="0x010600be"/>
+  <public type="color" name="system_on_tertiary_fixed_variant" id="0x010600bf"/>
+  <public type="color" name="system_outline_variant_light" id="0x010600c0"/>
+  <public type="color" name="system_outline_variant_dark" id="0x010600c1"/>
+  <staging-public-group-final type="bool" first-id="0x01be0000">
+    <!-- @hide @SystemApi -->
+    <public name="config_safetyProtectionEnabled"/>
+    <!-- @hide @SystemApi -->
+    <public name="config_enableDefaultNotes"/>
+    <!-- @hide @SystemApi -->
+    <public name="config_enableDefaultNotesForWorkProfile"/>
+  </staging-public-group-final>
+  <!-- @hide @SystemApi -->
+  <public type="bool" name="config_safetyProtectionEnabled" id="0x01110009"/>
+  <!-- @hide @SystemApi -->
+  <public type="bool" name="config_enableDefaultNotes" id="0x0111000a"/>
+  <!-- @hide @SystemApi -->
+  <public type="bool" name="config_enableDefaultNotesForWorkProfile" id="0x0111000b"/>
 </resources>
```

### Comparing `pyaxml-0.0.8/src/pyaxml.egg-info/PKG-INFO` & `pyaxml-0.0.9/src/pyaxml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaxml
-Version: 0.0.8
+Version: 0.0.9
 Summary: Manipulate AXML file and create one from scratch
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
```

### Comparing `pyaxml-0.0.8/tests/test.py` & `pyaxml-0.0.9/tests/test.py`

 * *Files identical despite different names*

