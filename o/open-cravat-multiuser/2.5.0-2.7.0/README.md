# Comparing `tmp/open-cravat-multiuser-2.5.0.tar.gz` & `tmp/open-cravat-multiuser-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-cravat-multiuser-2.5.0.tar", last modified: Mon Feb 26 16:08:25 2024, max compression
+gzip compressed data, was "open-cravat-multiuser-2.7.0.tar", last modified: Mon Jun  3 14:54:33 2024, max compression
```

## Comparing `open-cravat-multiuser-2.5.0.tar` & `open-cravat-multiuser-2.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:25.207788 open-cravat-multiuser-2.5.0/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1114 2024-02-26 16:08:25.207788 open-cravat-multiuser-2.5.0/PKG-INFO
--rw-r--r--   0 kyle      (1000) kyle      (1000)      858 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/README.rst
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:25.205788 open-cravat-multiuser-2.5.0/cravat_multiuser/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    29327 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/cravat_multiuser/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      591 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/cravat_multiuser/favicon.ico
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/cravat_multiuser/favicon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1797 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/cravat_multiuser/logout.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:25.206788 open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3605 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/cravat_multiuser.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    33193 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/cravat_multiuser.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    33359 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/cravat_multiuser_module.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4577 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/login.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)    41816 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/login.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    66634 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/logo.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)   372952 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/oc.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1616 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/cravat_multiuser/pwchng.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:25.207788 open-cravat-multiuser-2.5.0/open_cravat_multiuser.egg-info/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1114 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/open_cravat_multiuser.egg-info/PKG-INFO
--rw-r--r--   0 kyle      (1000) kyle      (1000)      666 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/open_cravat_multiuser.egg-info/SOURCES.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)        1 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/open_cravat_multiuser.egg-info/dependency_links.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)       48 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/open_cravat_multiuser.egg-info/requires.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)       17 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/open_cravat_multiuser.egg-info/top_level.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)       38 2024-02-26 16:08:25.207788 open-cravat-multiuser-2.5.0/setup.cfg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      959 2024-02-26 16:08:25.000000 open-cravat-multiuser-2.5.0/setup.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-06-03 14:54:33.311267 open-cravat-multiuser-2.7.0/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1207 2024-06-03 14:54:33.311267 open-cravat-multiuser-2.7.0/PKG-INFO
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      858 2023-02-13 16:43:21.000000 open-cravat-multiuser-2.7.0/README.rst
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-06-03 14:54:33.309267 open-cravat-multiuser-2.7.0/cravat_multiuser/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    29327 2023-04-20 16:55:32.000000 open-cravat-multiuser-2.7.0/cravat_multiuser/__init__.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      591 2023-02-13 16:43:21.000000 open-cravat-multiuser-2.7.0/cravat_multiuser/favicon.ico
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-02-13 16:43:21.000000 open-cravat-multiuser-2.7.0/cravat_multiuser/favicon.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1797 2023-02-13 16:43:21.000000 open-cravat-multiuser-2.7.0/cravat_multiuser/logout.png
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-06-03 14:54:33.310267 open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3566 2024-06-03 13:35:16.000000 open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/cravat_multiuser.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    33193 2024-02-26 09:44:39.000000 open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/cravat_multiuser.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    33775 2024-06-03 13:35:16.000000 open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/cravat_multiuser_module.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4577 2024-06-03 13:35:15.000000 open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/login.html
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    41816 2023-02-13 16:43:21.000000 open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/login.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    66634 2023-02-13 16:43:21.000000 open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/logo.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   372952 2023-02-13 16:43:21.000000 open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/oc.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1616 2023-02-13 16:43:21.000000 open-cravat-multiuser-2.7.0/cravat_multiuser/pwchng.png
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-06-03 14:54:33.311267 open-cravat-multiuser-2.7.0/open_cravat_multiuser.egg-info/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1207 2024-06-03 14:54:33.000000 open-cravat-multiuser-2.7.0/open_cravat_multiuser.egg-info/PKG-INFO
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      666 2024-06-03 14:54:33.000000 open-cravat-multiuser-2.7.0/open_cravat_multiuser.egg-info/SOURCES.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        1 2024-06-03 14:54:33.000000 open-cravat-multiuser-2.7.0/open_cravat_multiuser.egg-info/dependency_links.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       48 2024-06-03 14:54:33.000000 open-cravat-multiuser-2.7.0/open_cravat_multiuser.egg-info/requires.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       17 2024-06-03 14:54:33.000000 open-cravat-multiuser-2.7.0/open_cravat_multiuser.egg-info/top_level.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       38 2024-06-03 14:54:33.311267 open-cravat-multiuser-2.7.0/setup.cfg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      959 2024-06-03 14:54:03.000000 open-cravat-multiuser-2.7.0/setup.py
```

### Comparing `open-cravat-multiuser-2.5.0/PKG-INFO` & `open-cravat-multiuser-2.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: open-cravat-multiuser
-Version: 2.5.0
+Version: 2.7.0
 Summary: OpenCRAVAT Multiuser Addon
 Home-page: http://www.opencravat.org
 Author: Rick Kim, Kyle Moad, Mike Ryan, and Rachel Karchin
 Author-email: rkim@insilico.us.com
 Requires-Python: >=3.6
+Requires-Dist: aiohttp_session
+Requires-Dist: cryptography
+Requires-Dist: open-cravat>=2.2.2
 
 open-cravat-server enables OpenCRAVAT to support multiple users in its web server.
 
 OpenCRAVAT is a python package that performs genomic variant interpretation including variant impact, annotation, and scoring.  It has a modular architecture with a wide variety of analysis modules that are developed both by the CRAVAT team and the broader variant analysis community. OpenCRAVAT is a product of the `Karchin Lab`_ at Johns Hopkins University in collaboration with `In Silico Solutions`_ with funding provided by the National Cancer Institute's `ITCR`_ program.
 
 .. _Karchin Lab: http://karchinlab.org
 .. _In Silico Solutions: http://insilico.us.com
```

### Comparing `open-cravat-multiuser-2.5.0/README.rst` & `open-cravat-multiuser-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `open-cravat-multiuser-2.5.0/cravat_multiuser/__init__.py` & `open-cravat-multiuser-2.7.0/cravat_multiuser/__init__.py`

 * *Files identical despite different names*

### Comparing `open-cravat-multiuser-2.5.0/cravat_multiuser/favicon.ico` & `open-cravat-multiuser-2.7.0/cravat_multiuser/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-multiuser-2.5.0/cravat_multiuser/favicon.png` & `open-cravat-multiuser-2.7.0/cravat_multiuser/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-multiuser-2.5.0/cravat_multiuser/logout.png` & `open-cravat-multiuser-2.7.0/cravat_multiuser/logout.png`

 * *Files identical despite different names*

### Comparing `open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/cravat_multiuser.css` & `open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/cravat_multiuser.css`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     flex-direction: column;
     position: absolute;
     top: 2rem;
     right: 3rem;
     padding: 10px;
     background-color: white;
     border: 1px solid black;
+    z-index: 202;
 }
 
 #admindiv {
     position: relative;
     top: 100px;
     height: calc(100% - 100px);
 }
@@ -82,27 +83,24 @@
 }
 
 .adminsection-div table {
     margin: 20px;
 }
 
 #accountdiv {
-    position: absolute;
-    right: 132px;
-    top: 4px;
     display: flex;
     align-items: center;
 }
 
 #accountdiv span {
     font-size: 12px;
 }
 
 #logdiv {
-    display: inline-block;
+    display: inline-flex;
 }
 
 #logdiv img {
     height: 18px;
     cursor: pointer;
     vertical-align: middle;
 }
```

### Comparing `open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/cravat_multiuser.js` & `open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/cravat_multiuser.js`

 * *Files identical despite different names*

### Comparing `open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/cravat_multiuser_module.js` & `open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/cravat_multiuser_module.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -327,15 +327,15 @@
         setupAdminMode();
     }
     OC.mediator.publish('populateJobs');
 }
 
 function setupAdminMode() {
     document.getElementById('settingsdiv').style.display = 'none';
-    document.querySelector('.threedotsdiv').style.display = 'block';
+    document.querySelector('.threedotsdiv').style.display = '';
     $('#storediv_tabhead[value=storediv]')[0].style.display = 'inline-block';
     $('#admindiv_tabhead[value=admindiv]')[0].style.display = 'inline-block';
     document.getElementById('admindiv_tabhead').setAttribute('disabled', 'f');
     document.getElementById('submitcontentdiv').style.display = 'none';
     populateAdminTab();
 }
 
@@ -812,31 +812,39 @@
     var userDiv = getEl('span');
     userDiv.id = 'userdiv';
     userDiv.textContent = username + '\xa0';
     addEl(div, userDiv);
     var logoutDiv = getEl('div');
     logoutDiv.id = 'logdiv';
     addEl(div, logoutDiv);
+    let chngpwdContainer = getEl('div');
+    chngpwdContainer.classList.add('menu-icon-container');
     var btn = getEl('img');
     btn.src = '/server/pwchng.png';
     btn.addEventListener('click', function(evt) {
         changePassword();
     });
     btn.title = 'Change password';
-    addEl(logoutDiv, btn);
+    btn.classList.add('menu-icon');
+    addEl(chngpwdContainer, btn);
+    addEl(logoutDiv, chngpwdContainer);
     var span = getEl('span');
     span.textContent = '\xa0\xa0';
     addEl(logoutDiv, span);
+    let logoutContainer = getEl('div');
+    logoutContainer.classList.add('menu-icon-container');
     var btn = getEl('img');
-    btn.src = '/server/logout.png';
+    btn.src = '/server/sign-out.svg';
     btn.addEventListener('click', function(evt) {
         logout();
     });
     btn.title = 'Logout';
-    addEl(logoutDiv, btn);
+    btn.classList.add('menu-icon');
+    addEl(logoutContainer, btn);
+    addEl(logoutDiv, logoutContainer);
     var sdiv = getEl('div');
     sdiv.id = 'changepassworddiv';
     var span = getEl('span');
     span.textContent = 'Current password: ';
     addEl(sdiv, span);
     var input = getEl('input');
     input.type = 'password';
@@ -871,16 +879,17 @@
     btn.classList.add('butn');
     btn.addEventListener('click', function(evt) {
         submitNewPassword();
     });
     btn.textContent = 'Submit';
     addEl(sdiv, btn);
     addEl(div, sdiv);
-    var headerDiv = document.querySelector('.headerdiv');
-    addEl(headerDiv, div);
+    var headerDiv = document.getElementById('top-menu');
+    headerDiv.insertBefore(div, headerDiv.firstChild);
+    // addEl(headerDiv, div);
     if (isGuestAccount(username)) {
         document.querySelector('#changepassworddiv input:nth-child(2)').style.display = 'none';
         document.querySelector('#changepassworddiv span:first-child').style.display = 'none';
         var sdiv = getEl('div');
         sdiv.id = 'guest_warn_div';
         var span = getEl('span');
         span.textContent = 'This guest account will be deleted after ' + noRemDays + (noRemDays > 1 ? ' days' : ' day') + '. To keep your jobs, click the change account information icon to the right of user name and enter your email address and a new password.';
```

### Comparing `open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/login.html` & `open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/login.html`

 * *Files identical despite different names*

### Comparing `open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/login.png` & `open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/login.png`

 * *Files identical despite different names*

### Comparing `open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/logo.png` & `open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/logo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-multiuser-2.5.0/cravat_multiuser/nocache/oc.png` & `open-cravat-multiuser-2.7.0/cravat_multiuser/nocache/oc.png`

 * *Files identical despite different names*

### Comparing `open-cravat-multiuser-2.5.0/cravat_multiuser/pwchng.png` & `open-cravat-multiuser-2.7.0/cravat_multiuser/pwchng.png`

 * *Files identical despite different names*

### Comparing `open-cravat-multiuser-2.5.0/open_cravat_multiuser.egg-info/PKG-INFO` & `open-cravat-multiuser-2.7.0/open_cravat_multiuser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: open-cravat-multiuser
-Version: 2.5.0
+Version: 2.7.0
 Summary: OpenCRAVAT Multiuser Addon
 Home-page: http://www.opencravat.org
 Author: Rick Kim, Kyle Moad, Mike Ryan, and Rachel Karchin
 Author-email: rkim@insilico.us.com
 Requires-Python: >=3.6
+Requires-Dist: aiohttp_session
+Requires-Dist: cryptography
+Requires-Dist: open-cravat>=2.2.2
 
 open-cravat-server enables OpenCRAVAT to support multiple users in its web server.
 
 OpenCRAVAT is a python package that performs genomic variant interpretation including variant impact, annotation, and scoring.  It has a modular architecture with a wide variety of analysis modules that are developed both by the CRAVAT team and the broader variant analysis community. OpenCRAVAT is a product of the `Karchin Lab`_ at Johns Hopkins University in collaboration with `In Silico Solutions`_ with funding provided by the National Cancer Institute's `ITCR`_ program.
 
 .. _Karchin Lab: http://karchinlab.org
 .. _In Silico Solutions: http://insilico.us.com
```

### Comparing `open-cravat-multiuser-2.5.0/open_cravat_multiuser.egg-info/SOURCES.txt` & `open-cravat-multiuser-2.7.0/open_cravat_multiuser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-multiuser-2.5.0/setup.py` & `open-cravat-multiuser-2.7.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 data_files = ['favicon.ico', 'favicon.png', 'logout.png', 'pwchng.png']
 for root, dirs, files in os.walk(os.path.join('cravat_multiuser', 'nocache')):
     root_files = [os.path.join('..', root, f) for f in files]
     data_files.extend(root_files)
 
 setup(
     name='open-cravat-multiuser',
-    version='2.5.0',
+    version='2.7.0',
     description='OpenCRAVAT Multiuser Addon',
     long_description=readme(),
     author='Rick Kim, Kyle Moad, Mike Ryan, and Rachel Karchin',
     author_email='rkim@insilico.us.com',
     url='http://www.opencravat.org',
     license='',
     package_data={
```

