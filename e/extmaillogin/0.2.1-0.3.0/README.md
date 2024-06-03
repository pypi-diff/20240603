# Comparing `tmp/extmaillogin-0.2.1.tar.gz` & `tmp/extmaillogin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extmaillogin-0.2.1.tar", max compression
+gzip compressed data, was "extmaillogin-0.3.0.tar", max compression
```

## Comparing `extmaillogin-0.2.1.tar` & `extmaillogin-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      484 2022-10-18 11:17:48.978559 extmaillogin-0.2.1/LICENSE
--rw-r--r--   0        0        0        0 2022-10-18 11:15:13.636804 extmaillogin-0.2.1/extmaillogin/__init__.py
--rw-r--r--   0        0        0      665 2022-10-18 11:15:13.636804 extmaillogin-0.2.1/extmaillogin/auth_backends.py
--rw-r--r--   0        0        0     3146 2022-11-01 19:12:22.756735 extmaillogin-0.2.1/extmaillogin/middleware.py
--rw-r--r--   0        0        0      366 2022-11-01 19:12:59.029131 extmaillogin-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      595 2022-11-01 19:13:27.470907 extmaillogin-0.2.1/setup.py
--rw-r--r--   0        0        0      389 2022-11-01 19:13:27.471178 extmaillogin-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      484 2022-10-18 11:17:48.978559 extmaillogin-0.3.0/LICENSE
+-rw-r--r--   0        0        0        0 2022-10-18 11:15:13.636804 extmaillogin-0.3.0/extmaillogin/__init__.py
+-rw-r--r--   0        0        0      665 2022-10-18 11:15:13.636804 extmaillogin-0.3.0/extmaillogin/auth_backends.py
+-rw-r--r--   0        0        0     3324 2024-06-03 08:36:42.652944 extmaillogin-0.3.0/extmaillogin/middleware.py
+-rw-r--r--   0        0        0      366 2024-06-03 08:37:22.105452 extmaillogin-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 extmaillogin-0.3.0/PKG-INFO
```

### Comparing `extmaillogin-0.2.1/extmaillogin/auth_backends.py` & `extmaillogin-0.3.0/extmaillogin/auth_backends.py`

 * *Files identical despite different names*

### Comparing `extmaillogin-0.2.1/extmaillogin/middleware.py` & `extmaillogin-0.3.0/extmaillogin/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,30 @@
 
 logger = logging.getLogger(__name__)
 
 
 class ExternalEmailAuthenticationMiddleware(RemoteUserMiddleware):
 
     header = getattr(settings, 'EXT_AUTH_EMAIL_HEADER', 'HTTP_X_MAIL')
+    header_extractor = getattr(settings, 'EXT_AUTH_EMAIL_EXTRACTOR', None)
     allow_anonymous = getattr(settings, 'EXT_AUTH_ALLOW_ANONYMOUS', False)
 
     def process_request(self, request):
         # AuthenticationMiddleware is required so that request.user exists.
         if not hasattr(request, "user"):
             raise ImproperlyConfigured(
                 "This middleware requires the authentication middleware to be installed. "
                 "Edit your MIDDLEWARE setting to insert "
                 "'django.contrib.auth.middleware.AuthenticationMiddleware'"
                 " before the RemoteUserMiddleware class."
             )
-        email = request.META.get(self.header)
+        if self.header_extractor:
+            email = self.header_extractor(request)
+        else:
+            email = request.META.get(self.header)
         if not email:
             logger.debug("No or empty email header (%s) found in request", self.header)
             # If specified header doesn't exist then remove any existing
             # authenticated remote-user, or return (leaving request.user set to
             # AnonymousUser by the AuthenticationMiddleware).
             if request.user.is_authenticated:
                 self._remove_invalid_user(request)
```

