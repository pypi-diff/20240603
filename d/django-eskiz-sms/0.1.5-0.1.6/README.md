# Comparing `tmp/django-eskiz-sms-0.1.5.tar.gz` & `tmp/django_eskiz_sms-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-eskiz-sms-0.1.5.tar", last modified: Sun Aug  6 16:47:25 2023, max compression
+gzip compressed data, was "django_eskiz_sms-0.1.6.tar", last modified: Mon Jun  3 12:39:32 2024, max compression
```

## Comparing `django-eskiz-sms-0.1.5.tar` & `django_eskiz_sms-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 16:47:25.658759 django-eskiz-sms-0.1.5/
--rw-rw-rw-   0        0        0       78 2023-07-15 02:08:52.000000 django-eskiz-sms-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2291 2023-08-06 16:47:25.658759 django-eskiz-sms-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      995 2023-07-15 09:33:10.000000 django-eskiz-sms-0.1.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-06 16:47:25.625758 django-eskiz-sms-0.1.5/django_eskiz_sms.egg-info/
--rw-rw-rw-   0        0        0     2291 2023-08-06 16:47:25.000000 django-eskiz-sms-0.1.5/django_eskiz_sms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2023-08-06 16:47:25.000000 django-eskiz-sms-0.1.5/django_eskiz_sms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 16:47:25.000000 django-eskiz-sms-0.1.5/django_eskiz_sms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-06 16:47:25.000000 django-eskiz-sms-0.1.5/django_eskiz_sms.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       21 2023-08-06 16:47:25.000000 django-eskiz-sms-0.1.5/django_eskiz_sms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-06 16:47:25.000000 django-eskiz-sms-0.1.5/django_eskiz_sms.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-06 16:47:25.644755 django-eskiz-sms-0.1.5/eskiz_sms/
--rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.5/eskiz_sms/__init__.py
--rw-rw-rw-   0        0        0      799 2023-08-06 15:02:08.000000 django-eskiz-sms-0.1.5/eskiz_sms/admin.py
--rw-rw-rw-   0        0        0      187 2023-08-06 14:48:21.000000 django-eskiz-sms-0.1.5/eskiz_sms/apps.py
-drwxrwxrwx   0        0        0        0 2023-08-06 16:47:25.652755 django-eskiz-sms-0.1.5/eskiz_sms/migrations/
--rw-rw-rw-   0        0        0     4017 2023-08-06 15:21:35.000000 django-eskiz-sms-0.1.5/eskiz_sms/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.5/eskiz_sms/migrations/__init__.py
--rw-rw-rw-   0        0        0     2415 2023-08-06 14:49:27.000000 django-eskiz-sms-0.1.5/eskiz_sms/models.py
-drwxrwxrwx   0        0        0        0 2023-08-06 16:47:25.655760 django-eskiz-sms-0.1.5/eskiz_sms/templates/
--rw-rw-rw-   0        0        0      931 2023-07-15 01:13:57.000000 django-eskiz-sms-0.1.5/eskiz_sms/templates/send_sms.html
--rw-rw-rw-   0        0        0      161 2023-07-15 01:08:28.000000 django-eskiz-sms-0.1.5/eskiz_sms/urls.py
--rw-rw-rw-   0        0        0     1651 2023-07-15 01:07:39.000000 django-eskiz-sms-0.1.5/eskiz_sms/views.py
--rw-rw-rw-   0        0        0       93 2023-07-15 08:41:20.000000 django-eskiz-sms-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0      252 2023-08-06 16:47:25.662755 django-eskiz-sms-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1751 2023-08-06 16:47:20.000000 django-eskiz-sms-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:39:32.809207 django_eskiz_sms-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-06-03 12:39:32.809207 django_eskiz_sms-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:39:32.809207 django_eskiz_sms-0.1.6/django_eskiz_sms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-06-03 12:39:32.000000 django_eskiz_sms-0.1.6/django_eskiz_sms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-06-03 12:39:32.000000 django_eskiz_sms-0.1.6/django_eskiz_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:39:32.000000 django_eskiz_sms-0.1.6/django_eskiz_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/django_eskiz_sms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-03 12:39:32.000000 django_eskiz_sms-0.1.6/django_eskiz_sms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 12:39:32.000000 django_eskiz_sms-0.1.6/django_eskiz_sms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:39:32.805207 django_eskiz_sms-0.1.6/eskiz_sms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/eskiz_sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/eskiz_sms/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/eskiz_sms/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:39:32.805207 django_eskiz_sms-0.1.6/eskiz_sms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/eskiz_sms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/eskiz_sms/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/eskiz_sms/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:39:32.805207 django_eskiz_sms-0.1.6/eskiz_sms/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/eskiz_sms/templates/send_sms.html
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/eskiz_sms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/eskiz_sms/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-06-03 12:39:32.809207 django_eskiz_sms-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-06-03 12:39:02.000000 django_eskiz_sms-0.1.6/setup.py
```

### Comparing `django-eskiz-sms-0.1.5/PKG-INFO` & `django_eskiz_sms-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,115 @@
-Metadata-Version: 2.1
-Name: django-eskiz-sms
-Version: 0.1.5
-Summary: Djangoda Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket
-Home-page: https://docs.tijorat.org/django/
-Author: Ro'zmat Otajonov
-Author-email: hello@tijorat.org
-Maintainer: Ro'zmat Otajonov
-Maintainer-email: hello@tijorat.org
-License: MIT
-Project-URL: Batafsil qo'llanma, https://docs.tijorat.org/django-eskiz-sms
-Project-URL: GitHub Soure Code, https://github.com/Otajonov/django-eskiz-sms
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-
-Djangodan EskizUz yordamida SMS yuborish uchun eng mukammal paket
-
-Paketni pip install django-eskiz-sms deb o'rnatib,
-asosiy appni settings.py ida INSTALLED_APPS ga eskiz_sms deb qo'shing.
-
-Makemigration va migratedan keyin django adminga o'ting.
-U yerda EskizSMS degan modelga EskizUZ emailingiz va kabinetdan olgan parolingizni kiriting.
-
-So'ngra asosiy urls.py ga eskiz_sms.urls ni include qiling, bu sms browserda forma orqali sms
-yuborib sinab ko'rish uchun. Xavfsizlik yuzasidan keyin uni uzib qo'ying.
-Bu faqat test uchun. Paketni asli quyidagi yo'l bilan ishlatasiz:
-
-Odatiy ishlatish uchun istalgan joyda from eskiz_sms.views import send_sms yoki boshqa
-yo'l bilan send_sms() degan metodni chaqirib ishlating. Qolgan ishlarni o'zi bajaradi.
-Shuningdek admin panelda SMSLog orqali jo'natilgan SMSlar statistikasini ko'rib tursangiz bo'ladi.
-
-
-Yordam kerak bo'lsa Telegram: https://t.me/a1ie9
-Ishlatish uchun batafsil qo'llanma: https://docs.tijorat.org/django-eskiz-sms
+Metadata-Version: 2.1
+Name: django-eskiz-sms
+Version: 0.1.6
+Summary: Djangoda Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket
+Home-page: https://github.com/Otajonov/django-eskiz-sms
+Author: Ro'zmat Otajonov
+Author-email: hello@tijorat.org
+Maintainer: Ro'zmat Otajonov
+Maintainer-email: hello@tijorat.org
+License: MIT
+Project-URL: Yordam, https://t.me/RozmatOtajonov
+Project-URL: GitHub Soure Code, https://github.com/Otajonov/django-eskiz-sms
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
+License-File: LICENSE
+Requires-Dist: Django>=3.2
+Requires-Dist: requests
+
+Django Eskiz SMS Integration
+============================
+
+Easily integrate EskizUz SMS functionality into your Django application.
+
+Installation
+------------
+
+First, install the package using pip:
+
+.. code-block:: sh
+
+    pip install django-eskiz-sms
+
+Then, add ``eskiz_sms`` to your ``INSTALLED_APPS`` in ``settings.py``:
+
+.. code-block:: python
+
+    INSTALLED_APPS = [
+        ...
+        'eskiz_sms',
+    ]
+
+Setup
+-----
+
+After adding the app, run migrations to set up the necessary database tables:
+
+.. code-block:: sh
+
+    python manage.py makemigrations eskiz_sms
+    python manage.py migrate eskiz_sms
+
+Next, go to the Django admin panel and add your EskizUz email and API token in the ``EskizSMS`` model.
+
+Usage
+-----
+
+### Sending SMS
+
+To send an SMS, you can use the ``send_sms`` method. Import it into any part of your application where you need to send an SMS:
+
+.. code-block:: python
+
+    from eskiz_sms.views import send_sms
+
+    send_sms(phone_number, message)
+
+### Testing
+
+To test the SMS functionality through the browser, include ``eskiz_sms.urls`` in your project's ``urls.py``:
+
+.. code-block:: python
+
+    from django.urls import path, include
+
+    urlpatterns = [
+        ...
+        path('sms/', include('eskiz_sms.urls')),
+    ]
+
+Visit the provided URL in your browser to send test SMS messages. **For security reasons, remove this URL after testing.**
+
+SMS Log
+-------
+
+You can view the statistics of sent SMS messages in the ``SMSLog`` model in the Django admin panel.
+
+Support
+-------
+
+For additional help, join our Telegram group: `Telegram Support <https://t.me/RozmatOtajonov>`_
+
+For a detailed guide, visit: `Django Eskiz SMS Documentation <https://otajonov.dev/django-eskiz-sms>`_
+
+License
+-------
+
+MIT License
```

### Comparing `django-eskiz-sms-0.1.5/django_eskiz_sms.egg-info/PKG-INFO` & `django_eskiz_sms-0.1.6/django_eskiz_sms.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,115 @@
-Metadata-Version: 2.1
-Name: django-eskiz-sms
-Version: 0.1.5
-Summary: Djangoda Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket
-Home-page: https://docs.tijorat.org/django/
-Author: Ro'zmat Otajonov
-Author-email: hello@tijorat.org
-Maintainer: Ro'zmat Otajonov
-Maintainer-email: hello@tijorat.org
-License: MIT
-Project-URL: Batafsil qo'llanma, https://docs.tijorat.org/django-eskiz-sms
-Project-URL: GitHub Soure Code, https://github.com/Otajonov/django-eskiz-sms
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-
-Djangodan EskizUz yordamida SMS yuborish uchun eng mukammal paket
-
-Paketni pip install django-eskiz-sms deb o'rnatib,
-asosiy appni settings.py ida INSTALLED_APPS ga eskiz_sms deb qo'shing.
-
-Makemigration va migratedan keyin django adminga o'ting.
-U yerda EskizSMS degan modelga EskizUZ emailingiz va kabinetdan olgan parolingizni kiriting.
-
-So'ngra asosiy urls.py ga eskiz_sms.urls ni include qiling, bu sms browserda forma orqali sms
-yuborib sinab ko'rish uchun. Xavfsizlik yuzasidan keyin uni uzib qo'ying.
-Bu faqat test uchun. Paketni asli quyidagi yo'l bilan ishlatasiz:
-
-Odatiy ishlatish uchun istalgan joyda from eskiz_sms.views import send_sms yoki boshqa
-yo'l bilan send_sms() degan metodni chaqirib ishlating. Qolgan ishlarni o'zi bajaradi.
-Shuningdek admin panelda SMSLog orqali jo'natilgan SMSlar statistikasini ko'rib tursangiz bo'ladi.
-
-
-Yordam kerak bo'lsa Telegram: https://t.me/a1ie9
-Ishlatish uchun batafsil qo'llanma: https://docs.tijorat.org/django-eskiz-sms
+Metadata-Version: 2.1
+Name: django-eskiz-sms
+Version: 0.1.6
+Summary: Djangoda Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket
+Home-page: https://github.com/Otajonov/django-eskiz-sms
+Author: Ro'zmat Otajonov
+Author-email: hello@tijorat.org
+Maintainer: Ro'zmat Otajonov
+Maintainer-email: hello@tijorat.org
+License: MIT
+Project-URL: Yordam, https://t.me/RozmatOtajonov
+Project-URL: GitHub Soure Code, https://github.com/Otajonov/django-eskiz-sms
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
+License-File: LICENSE
+Requires-Dist: Django>=3.2
+Requires-Dist: requests
+
+Django Eskiz SMS Integration
+============================
+
+Easily integrate EskizUz SMS functionality into your Django application.
+
+Installation
+------------
+
+First, install the package using pip:
+
+.. code-block:: sh
+
+    pip install django-eskiz-sms
+
+Then, add ``eskiz_sms`` to your ``INSTALLED_APPS`` in ``settings.py``:
+
+.. code-block:: python
+
+    INSTALLED_APPS = [
+        ...
+        'eskiz_sms',
+    ]
+
+Setup
+-----
+
+After adding the app, run migrations to set up the necessary database tables:
+
+.. code-block:: sh
+
+    python manage.py makemigrations eskiz_sms
+    python manage.py migrate eskiz_sms
+
+Next, go to the Django admin panel and add your EskizUz email and API token in the ``EskizSMS`` model.
+
+Usage
+-----
+
+### Sending SMS
+
+To send an SMS, you can use the ``send_sms`` method. Import it into any part of your application where you need to send an SMS:
+
+.. code-block:: python
+
+    from eskiz_sms.views import send_sms
+
+    send_sms(phone_number, message)
+
+### Testing
+
+To test the SMS functionality through the browser, include ``eskiz_sms.urls`` in your project's ``urls.py``:
+
+.. code-block:: python
+
+    from django.urls import path, include
+
+    urlpatterns = [
+        ...
+        path('sms/', include('eskiz_sms.urls')),
+    ]
+
+Visit the provided URL in your browser to send test SMS messages. **For security reasons, remove this URL after testing.**
+
+SMS Log
+-------
+
+You can view the statistics of sent SMS messages in the ``SMSLog`` model in the Django admin panel.
+
+Support
+-------
+
+For additional help, join our Telegram group: `Telegram Support <https://t.me/RozmatOtajonov>`_
+
+For a detailed guide, visit: `Django Eskiz SMS Documentation <https://otajonov.dev/django-eskiz-sms>`_
+
+License
+-------
+
+MIT License
```

### Comparing `django-eskiz-sms-0.1.5/eskiz_sms/admin.py` & `django_eskiz_sms-0.1.6/eskiz_sms/admin.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from django.contrib import admin
-from .models import EskizSMS, SMSLog
-
-
-@admin.register(EskizSMS)
-class EskizSMSAdmin(admin.ModelAdmin):
-    list_display = ('email', 'from_name', 'callback_url', 'last_updated', 'eskiz_token')
-    
-    def get_readonly_fields(self, request, obj=None):
-        return ['last_updated', 'eskiz_token']
-
-
-@admin.register(SMSLog)
-class SMSLogAdmin(admin.ModelAdmin):
-    list_display = ('phone_number', 'message', 'from_name', 'status', 'status_date',  'from_app', 'error_message')
-    list_filter = ['status', 'from_app', 'from_name', 'status_date' ]
-    search_fields = ['phone_number', 'message' ]
-    
-    def has_add_permission(self, request):
-        return False
-
-    def has_change_permission(self, request, obj=None):
-        return False
+from django.contrib import admin
+from .models import EskizSMS, SMSLog
+
+
+@admin.register(EskizSMS)
+class EskizSMSAdmin(admin.ModelAdmin):
+    list_display = ('email', 'from_name', 'callback_url', 'last_updated', 'eskiz_token')
+    
+    def get_readonly_fields(self, request, obj=None):
+        return ['last_updated', 'eskiz_token']
+
+
+@admin.register(SMSLog)
+class SMSLogAdmin(admin.ModelAdmin):
+    list_display = ('phone_number', 'message', 'from_name', 'status', 'status_date',  'from_app', 'error_message')
+    list_filter = ['status', 'from_app', 'from_name', 'status_date' ]
+    search_fields = ['phone_number', 'message' ]
+    
+    def has_add_permission(self, request):
+        return False
+
+    def has_change_permission(self, request, obj=None):
+        return False
```

### Comparing `django-eskiz-sms-0.1.5/eskiz_sms/models.py` & `django_eskiz_sms-0.1.6/eskiz_sms/models.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from django.db import models
-from django.utils import timezone
-import requests
-
-
-
-class EskizSMS(models.Model):
-    
-    email = models.EmailField('Eskiz Email')
-    password = models.CharField('Eskiz kabinetidan parol', max_length=255)
-    from_name = models.CharField('Nickname (Birlamchi 4546)', max_length=255, blank=True, null=True)
-    callback_url = models.URLField("Callback URL (Ixtiyoriy)", null=True, blank=True)
-
-    eskiz_token = models.TextField("Token (Avtomatik yangilanadi)", null=True, blank=True)
-    last_updated = models.DateTimeField("So'ngi yangilanish", default=timezone.now)
-
-    class Meta:
-        verbose_name = "Sozlama"
-        verbose_name_plural = "Sozlamalar"
-        
-    def __str__(self):
-        return self.email
-    
-
-    def update_token(self):
-        
-        payload = {
-            'email': self.email,
-            'password': self.password
-        }
-        
-        response = requests.post("https://notify.eskiz.uz/api/auth/login", headers={}, data=payload)
-        
-        if response.status_code == 200:
-            resp_data = response.json()
-            
-            self.last_updated = timezone.now()
-            self.eskiz_token = resp_data.get('data', {}).get('token', '')
-            self.save()
-            
-            return resp_data.get('data', {}).get('token', '')
-        return None
-
-
-
-
-
-class SMSLog(models.Model):
-    phone_number = models.CharField('Telefon raqam', max_length=20)
-    message = models.TextField('SMS matni')
-    from_name = models.CharField('Qaysi nikdan', max_length=255)
-    status = models.CharField('Holati', max_length=10)
-    status_date = models.DateTimeField("Oxirgi o'zgarish", default=timezone.now)
-    error_message = models.TextField('Xatolik', blank=True, null=True)
-    from_app = models.CharField("Qaysi 'app'dan", max_length=255, blank=True, null=True)
-
-    class Meta:
-        verbose_name = "SMS tarixi"
-        verbose_name_plural = "SMSlar tarixi"
-        
-    def __str__(self):
-        return f"{self.phone_number} - {self.message}"
-
-def save_sms_log(phone_number, message, from_name, status, error_message=None, from_app=None):
-    SMSLog.objects.create(
-        phone_number=phone_number,
-        message=message,
-        from_name=from_name,
-        status=status,
-        error_message=error_message,
-        from_app=from_app
-    )
+from django.db import models
+from django.utils import timezone
+import requests
+
+
+
+class EskizSMS(models.Model):
+    
+    email = models.EmailField('Eskiz Email')
+    password = models.CharField('Eskiz kabinetidan parol', max_length=255)
+    from_name = models.CharField('Nickname (Birlamchi 4546)', max_length=255, blank=True, null=True)
+    callback_url = models.URLField("Callback URL (Ixtiyoriy)", null=True, blank=True)
+
+    eskiz_token = models.TextField("Token (Avtomatik yangilanadi)", null=True, blank=True)
+    last_updated = models.DateTimeField("So'ngi yangilanish", default=timezone.now)
+
+    class Meta:
+        verbose_name = "Sozlama"
+        verbose_name_plural = "Sozlamalar"
+        
+    def __str__(self):
+        return self.email
+    
+
+    def update_token(self):
+        
+        payload = {
+            'email': self.email,
+            'password': self.password
+        }
+        
+        response = requests.post("https://notify.eskiz.uz/api/auth/login", headers={}, data=payload)
+        
+        if response.status_code == 200:
+            resp_data = response.json()
+            
+            self.last_updated = timezone.now()
+            self.eskiz_token = resp_data.get('data', {}).get('token', '')
+            self.save()
+            
+            return resp_data.get('data', {}).get('token', '')
+        return None
+
+
+
+
+
+class SMSLog(models.Model):
+    phone_number = models.CharField('Telefon raqam', max_length=20)
+    message = models.TextField('SMS matni')
+    from_name = models.CharField('Qaysi nikdan', max_length=255)
+    status = models.CharField('Holati', max_length=10)
+    status_date = models.DateTimeField("Oxirgi o'zgarish", default=timezone.now)
+    error_message = models.TextField('Xatolik', blank=True, null=True)
+    from_app = models.CharField("Qaysi 'app'dan", max_length=255, blank=True, null=True)
+
+    class Meta:
+        verbose_name = "SMS tarixi"
+        verbose_name_plural = "SMSlar tarixi"
+        
+    def __str__(self):
+        return f"{self.phone_number} - {self.message}"
+
+def save_sms_log(phone_number, message, from_name, status, error_message=None, from_app=None):
+    SMSLog.objects.create(
+        phone_number=phone_number,
+        message=message,
+        from_name=from_name,
+        status=status,
+        error_message=error_message,
+        from_app=from_app
+    )
```

### Comparing `django-eskiz-sms-0.1.5/eskiz_sms/templates/send_sms.html` & `django_eskiz_sms-0.1.6/eskiz_sms/templates/send_sms.html`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-<!DOCTYPE html>
-<html>
-<head>
-    <title>Send SMS</title>
-</head>
-<body>
-
-    <h1>Eskiz.Uz dan SMS yuborish</h1>
-
-    <p>Hozircha faqat o'zbek raqamlarga ishlaydi va ushbu sahifa urls.py ini faqat test uchun ishlating!</p>
-    
-    <form method="post" action="{% url 'eskiz_sms:send_sms' %}">
-        {% csrf_token %}
-        <label for="phone">Telefon:</label>
-        <input type="text" id="phone" name="phone" required><br>
-        <label for="sms">SMS matni (160 belgi max):</label>
-        <textarea id="sms" name="sms" required maxlength="160"></textarea><br>
-        <label for="from">Nik (Nik olmagan bo'lsangiz bo'sh qolsin):</label>
-        <input type="text" id="from" name="from"><br>
-        <label for="from_app">Qaysi Appdan (Ixtiyoriy):</label>
-        <input type="text" id="from_app" name="from_app"><br>
-        <button type="submit">SMS ni yuborish</button>
-    </form>
-</body>
-</html>
+<!DOCTYPE html>
+<html>
+<head>
+    <title>Send SMS</title>
+</head>
+<body>
+
+    <h1>Eskiz.Uz dan SMS yuborish</h1>
+
+    <p>Hozircha faqat o'zbek raqamlarga ishlaydi va ushbu sahifa urls.py ini faqat test uchun ishlating!</p>
+    
+    <form method="post" action="{% url 'eskiz_sms:send_sms' %}">
+        {% csrf_token %}
+        <label for="phone">Telefon:</label>
+        <input type="text" id="phone" name="phone" required><br>
+        <label for="sms">SMS matni (160 belgi max):</label>
+        <textarea id="sms" name="sms" required maxlength="160"></textarea><br>
+        <label for="from">Nik (Nik olmagan bo'lsangiz bo'sh qolsin):</label>
+        <input type="text" id="from" name="from"><br>
+        <label for="from_app">Qaysi Appdan (Ixtiyoriy):</label>
+        <input type="text" id="from_app" name="from_app"><br>
+        <button type="submit">SMS ni yuborish</button>
+    </form>
+</body>
+</html>
```

