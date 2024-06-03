# Comparing `tmp/django-image-crop-0.0.2.tar.gz` & `tmp/django-image-crop-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-image-crop-0.0.2.tar", last modified: Thu May 30 13:48:18 2024, max compression
+gzip compressed data, was "django-image-crop-0.0.3.tar", last modified: Mon Jun  3 01:44:58 2024, max compression
```

## Comparing `django-image-crop-0.0.2.tar` & `django-image-crop-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 13:48:18.031675 django-image-crop-0.0.2/
--rw-rw-rw-   0        0        0     1084 2024-05-28 11:27:49.000000 django-image-crop-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       95 2024-05-30 13:48:12.000000 django-image-crop-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2323 2024-05-30 13:48:18.031675 django-image-crop-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1642 2024-05-30 09:15:55.000000 django-image-crop-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 13:48:18.022918 django-image-crop-0.0.2/django_image_crop.egg-info/
--rw-rw-rw-   0        0        0     2323 2024-05-30 13:48:17.000000 django-image-crop-0.0.2/django_image_crop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      575 2024-05-30 13:48:17.000000 django-image-crop-0.0.2/django_image_crop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 13:48:17.000000 django-image-crop-0.0.2/django_image_crop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-30 13:48:17.000000 django-image-crop-0.0.2/django_image_crop.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 13:48:18.025903 django-image-crop-0.0.2/image_crop/
--rw-rw-rw-   0        0        0       36 2024-05-29 00:39:11.000000 django-image-crop-0.0.2/image_crop/__init__.py
--rw-rw-rw-   0        0        0      163 2024-05-30 03:21:41.000000 django-image-crop-0.0.2/image_crop/apps.py
--rw-rw-rw-   0        0        0      611 2024-05-30 00:56:34.000000 django-image-crop-0.0.2/image_crop/fields.py
--rw-rw-rw-   0        0        0      438 2024-05-30 06:49:48.000000 django-image-crop-0.0.2/image_crop/models.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:48:18.009739 django-image-crop-0.0.2/image_crop/static/
-drwxrwxrwx   0        0        0        0 2024-05-30 13:48:18.027402 django-image-crop-0.0.2/image_crop/static/css/
--rw-rw-rw-   0        0        0   153111 2020-12-07 15:50:12.000000 django-image-crop-0.0.2/image_crop/static/css/bootstrap.min.css
--rw-rw-rw-   0        0        0     3805 2024-05-28 00:57:04.000000 django-image-crop-0.0.2/image_crop/static/css/cropper.min.css
--rw-rw-rw-   0        0        0     1961 2024-05-30 08:55:01.000000 django-image-crop-0.0.2/image_crop/static/css/image_crop.css
-drwxrwxrwx   0        0        0        0 2024-05-30 13:48:18.029682 django-image-crop-0.0.2/image_crop/static/js/
--rw-rw-rw-   0        0        0    62411 2020-12-07 15:50:12.000000 django-image-crop-0.0.2/image_crop/static/js/bootstrap.min.js
--rw-rw-rw-   0        0        0    37380 2024-05-28 00:57:39.000000 django-image-crop-0.0.2/image_crop/static/js/cropper.min.js
--rw-rw-rw-   0        0        0    87533 2024-05-27 09:41:48.000000 django-image-crop-0.0.2/image_crop/static/js/jquery-3.7.1.min.js
-drwxrwxrwx   0        0        0        0 2024-05-30 13:48:18.030678 django-image-crop-0.0.2/image_crop/templates/
--rw-rw-rw-   0        0        0    10052 2024-05-30 08:51:12.000000 django-image-crop-0.0.2/image_crop/templates/image_crop.html
--rw-rw-rw-   0        0        0     1059 2024-05-30 00:54:51.000000 django-image-crop-0.0.2/image_crop/widgets.py
--rw-rw-rw-   0        0        0       42 2024-05-30 13:48:18.031675 django-image-crop-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1013 2024-05-30 13:47:15.000000 django-image-crop-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 01:44:58.118122 django-image-crop-0.0.3/
+-rw-rw-rw-   0        0        0     1084 2024-05-28 11:27:49.000000 django-image-crop-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       95 2024-06-03 01:06:55.000000 django-image-crop-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6234 2024-06-03 01:44:58.117125 django-image-crop-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4181 2024-06-03 01:03:52.000000 django-image-crop-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 01:44:58.105181 django-image-crop-0.0.3/django_image_crop.egg-info/
+-rw-rw-rw-   0        0        0     6234 2024-06-03 01:44:58.000000 django-image-crop-0.0.3/django_image_crop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2024-06-03 01:44:58.000000 django-image-crop-0.0.3/django_image_crop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 01:44:58.000000 django-image-crop-0.0.3/django_image_crop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-06-03 01:44:58.000000 django-image-crop-0.0.3/django_image_crop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 01:44:58.109147 django-image-crop-0.0.3/image_crop/
+-rw-rw-rw-   0        0        0       36 2024-05-29 00:39:11.000000 django-image-crop-0.0.3/image_crop/__init__.py
+-rw-rw-rw-   0        0        0      163 2024-05-30 03:21:41.000000 django-image-crop-0.0.3/image_crop/apps.py
+-rw-rw-rw-   0        0        0      611 2024-05-30 00:56:34.000000 django-image-crop-0.0.3/image_crop/fields.py
+drwxrwxrwx   0        0        0        0 2024-06-03 01:44:58.097177 django-image-crop-0.0.3/image_crop/static/
+drwxrwxrwx   0        0        0        0 2024-06-03 01:44:58.112139 django-image-crop-0.0.3/image_crop/static/css/
+-rw-rw-rw-   0        0        0   153111 2020-12-07 15:50:12.000000 django-image-crop-0.0.3/image_crop/static/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0     3805 2024-05-28 00:57:04.000000 django-image-crop-0.0.3/image_crop/static/css/cropper.min.css
+-rw-rw-rw-   0        0        0     1961 2024-05-30 08:55:01.000000 django-image-crop-0.0.3/image_crop/static/css/image_crop.css
+drwxrwxrwx   0        0        0        0 2024-06-03 01:44:58.115130 django-image-crop-0.0.3/image_crop/static/js/
+-rw-rw-rw-   0        0        0    62411 2020-12-07 15:50:12.000000 django-image-crop-0.0.3/image_crop/static/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0    37380 2024-05-28 00:57:39.000000 django-image-crop-0.0.3/image_crop/static/js/cropper.min.js
+-rw-rw-rw-   0        0        0    87533 2024-05-27 09:41:48.000000 django-image-crop-0.0.3/image_crop/static/js/jquery-3.7.1.min.js
+drwxrwxrwx   0        0        0        0 2024-06-03 01:44:58.116127 django-image-crop-0.0.3/image_crop/templates/
+-rw-rw-rw-   0        0        0    10172 2024-05-31 06:43:21.000000 django-image-crop-0.0.3/image_crop/templates/image_crop.html
+-rw-rw-rw-   0        0        0     1059 2024-05-30 00:54:51.000000 django-image-crop-0.0.3/image_crop/widgets.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 01:44:58.118122 django-image-crop-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2024-06-03 01:16:32.000000 django-image-crop-0.0.3/setup.py
```

### Comparing `django-image-crop-0.0.2/LICENSE` & `django-image-crop-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-image-crop-0.0.2/image_crop/fields.py` & `django-image-crop-0.0.3/image_crop/fields.py`

 * *Files identical despite different names*

### Comparing `django-image-crop-0.0.2/image_crop/static/css/bootstrap.min.css` & `django-image-crop-0.0.3/image_crop/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-image-crop-0.0.2/image_crop/static/css/cropper.min.css` & `django-image-crop-0.0.3/image_crop/static/css/cropper.min.css`

 * *Files identical despite different names*

### Comparing `django-image-crop-0.0.2/image_crop/static/css/image_crop.css` & `django-image-crop-0.0.3/image_crop/static/css/image_crop.css`

 * *Files identical despite different names*

### Comparing `django-image-crop-0.0.2/image_crop/static/js/bootstrap.min.js` & `django-image-crop-0.0.3/image_crop/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-image-crop-0.0.2/image_crop/static/js/cropper.min.js` & `django-image-crop-0.0.3/image_crop/static/js/cropper.min.js`

 * *Files identical despite different names*

### Comparing `django-image-crop-0.0.2/image_crop/static/js/jquery-3.7.1.min.js` & `django-image-crop-0.0.3/image_crop/static/js/jquery-3.7.1.min.js`

 * *Files identical despite different names*

### Comparing `django-image-crop-0.0.2/image_crop/templates/image_crop.html` & `django-image-crop-0.0.3/image_crop/templates/image_crop.html`

 * *Files 4% similar despite different names*

```diff
@@ -173,14 +173,19 @@
   /**
    * 添加图片按钮实例
    */
   const addImage = $("#add-image")
   addImage.hide()
 
   /**
+   * 大小限制
+   */
+  const cropSize = $("#crop-size")
+
+  /**
    * 打开文件管理器
    */
   const openFileMange = () => {
     // 重置files
     imageInput[0].files = new DataTransfer().files
     imageInput && imageInput.click()
   }
@@ -288,24 +293,23 @@
     const imageType = $("#image-type")[0].value
 
     const base64Image = cropper.getCroppedCanvas().toDataURL(imageType)
     const imageFile = base64ToFile(base64Image, protoImage.prop("alt"))
 
     const fileKb = imageFile.size / 1024
 
-    if (parseInt('{{ max_size }}') > fileKb) {
-
+    if ('{{ max_size }}' === 'None' || parseInt('{{ max_size }}') > fileKb) {
       let fileList = new DataTransfer()
       fileList.items.add(imageFile)
       imageUpload[0].files = fileList.files
 
       cropImageObj.val = base64Image
       cropperModal.modal("hide")
     } else {
-      $("#crop-size")[0].innerHTML = `（${parseInt(`${fileKb}`)}kb）`
+      if (cropSize[0]) cropSize[0].innerHTML = `（${parseInt(`${fileKb}`)}kb）`
     }
   }
 
   $("#deleteBtn").on("click", () => {
     cropImageObj.val = ''
     imageUpload[0].files = new DataTransfer().files
   })
@@ -320,12 +324,12 @@
       }
     })
   })
 
   $("#crop-reset").on("click", () => cropper.reset())
 
   cropperModal.on("hide.bs.modal", () => {
-    $("#crop-size")[0].innerHTML = ''
+    if (cropSize[0]) cropSize[0].innerHTML = ''
     // 存在则删除cropper实例
     cropper && cropper.destroy()
   })
 </script>
```

### Comparing `django-image-crop-0.0.2/image_crop/widgets.py` & `django-image-crop-0.0.3/image_crop/widgets.py`

 * *Files identical despite different names*

### Comparing `django-image-crop-0.0.2/setup.py` & `django-image-crop-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-image-crop",
-    version="0.0.2",
-    author="bj.tr",
+    version="0.0.3",
+    author="bj.t",
     author_email="bj.t@foxmail.com",
     description="Image cropping plugin, can be directly applied to django admin.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
     keyword=["django-image-crop", "django", "image", "crop", "cropper"],
```

