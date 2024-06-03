# Comparing `tmp/liteium-1.0.4.tar.gz` & `tmp/liteium-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteium-1.0.4.tar", last modified: Mon May 20 20:34:53 2024, max compression
+gzip compressed data, was "liteium-1.0.5.tar", last modified: Mon Jun  3 01:55:45 2024, max compression
```

## Comparing `liteium-1.0.4.tar` & `liteium-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 20:34:53.560053 liteium-1.0.4/
--rw-rw-rw-   0        0        0      853 2024-05-20 20:34:53.557055 liteium-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      457 2024-05-11 04:46:56.000000 liteium-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 20:34:53.511369 liteium-1.0.4/liteium/
--rw-rw-rw-   0        0        0       19 2024-05-20 20:20:46.000000 liteium-1.0.4/liteium/__init__.py
--rw-rw-rw-   0        0        0    10078 2024-05-20 20:31:18.000000 liteium-1.0.4/liteium/main.py
-drwxrwxrwx   0        0        0        0 2024-05-20 20:34:53.552057 liteium-1.0.4/liteium.egg-info/
--rw-rw-rw-   0        0        0      853 2024-05-20 20:34:53.000000 liteium-1.0.4/liteium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-20 20:34:53.000000 liteium-1.0.4/liteium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 20:34:53.000000 liteium-1.0.4/liteium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-20 20:34:53.000000 liteium-1.0.4/liteium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-20 20:34:53.000000 liteium-1.0.4/liteium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 20:34:53.560053 liteium-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      630 2024-05-20 20:31:26.000000 liteium-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 01:55:45.079840 liteium-1.0.5/
+-rw-rw-rw-   0        0        0     1997 2024-06-03 01:55:45.077843 liteium-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1574 2024-06-03 00:29:53.000000 liteium-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 01:55:45.028679 liteium-1.0.5/liteium/
+-rw-rw-rw-   0        0        0       19 2024-06-03 00:29:56.000000 liteium-1.0.5/liteium/__init__.py
+-rw-rw-rw-   0        0        0    12295 2024-06-03 00:06:15.000000 liteium-1.0.5/liteium/main.py
+drwxrwxrwx   0        0        0        0 2024-06-03 01:55:45.073837 liteium-1.0.5/liteium.egg-info/
+-rw-rw-rw-   0        0        0     1997 2024-06-03 01:55:44.000000 liteium-1.0.5/liteium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-06-03 01:55:44.000000 liteium-1.0.5/liteium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 01:55:44.000000 liteium-1.0.5/liteium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 01:55:44.000000 liteium-1.0.5/liteium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-03 01:55:44.000000 liteium-1.0.5/liteium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 01:55:45.080838 liteium-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      705 2024-06-03 01:55:40.000000 liteium-1.0.5/setup.py
```

### Comparing `liteium-1.0.4/liteium/main.py` & `liteium-1.0.5/liteium/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,199 +4,277 @@
 import os, pickle
 from io import open as io_open
 from urllib.parse import urlparse
 from selenium.common.exceptions import NoAlertPresentException
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.common.exceptions import TimeoutException, NoSuchElementException
+# from selenium.common.exceptions as selenium_exceptions
 
 global driver1
 driver1 = ''
 
 class ElementWrapper:
     def __init__(self, element):
         self.element = element
 
 class ElementsWrapper:
     def __init__(self, elements):
         self.elements = elements
 
 def driver(driver_path):
+    """
+    Initialize the WebDriver with the given path.
+    """
     try:
         global driver1
         driver1 = webdriver.Chrome(service=Service(driver_path))
         return driver1
     except Exception as e:
         print("An error occurred while initializing driver:", e)
 
 def close():
+    """
+    Close the WebDriver session.
+    """
     try:
         global driver1
         driver1.quit()
     except Exception as e:
         print("An error occurred while closing driver:", e)
 
 def open(url):
+    """
+    Open the specified URL in the browser.
+    """
     try:
         global driver1
         driver1.get(url)
     except Exception as e:
         print("An error occurred while opening URL:", e)
 
 def find_element(by, value, time=0):
+    """
+    Find a single element by the given locator.
+    """
     try:
         locator = (by, value)
         wait = WebDriverWait(driver1, time)
         return ElementWrapper(wait.until(EC.presence_of_element_located(locator)))
     except TimeoutException:
         print("Timeout occurred while waiting for element.")
     except NoSuchElementException:
         print("Element not found.")
 
 def find_elements(by, value, time=0):
+    """
+    Find multiple elements by the given locator.
+    """
     try:
         locator = (by, value)
         wait = WebDriverWait(driver1, time)
         return ElementsWrapper(wait.until(EC.presence_of_all_elements_located(locator)))
-        # return ElementsWrapper(driver1.find_elements(*locator))
     except Exception as e:
         print("An error occurred while finding elements:", e)
 
-def id(value,  time=0):
+def id(value, time=0):
+    """
+    Find a single element by ID.
+    """
     try:
         return find_element(By.ID, value, time).element
     except Exception as e:
         print("An error occurred while finding element by ID:", e)
 
-def name(value,  time=0):
+def name(value, time=0):
+    """
+    Find a single element by name attribute.
+    """
     try:
         return find_element(By.NAME, value, time).element
     except Exception as e:
         print("An error occurred while finding element by name:", e)
 
-def xpath(value,  time=0):
+def xpath(value, time=0):
+    """
+    Find a single element by XPath.
+    """
     try:
         return find_element(By.XPATH, value, time).element
     except Exception as e:
-        print("An error occurred while finding element by xpath:", e)
+        print("An error occurred while finding element by XPath:", e)
 
-def link_text(value,  time=0):
+def link_text(value, time=0):
+    """
+    Find a single element by link text.
+    """
     try:
         return find_element(By.LINK_TEXT, value, time).element
     except Exception as e:
         print("An error occurred while finding element by link text:", e)
 
-def partial_link_text(value,  time=0):
+def partial_link_text(value, time=0):
+    """
+    Find a single element by partial link text.
+    """
     try:
         return find_element(By.PARTIAL_LINK_TEXT, value, time).element
     except Exception as e:
         print("An error occurred while finding element by partial link text:", e)
 
-def tag_name(value,  time=0):
+def tag_name(value, time=0):
+    """
+    Find a single element by tag name.
+    """
     try:
         return find_element(By.TAG_NAME, value, time).element
     except Exception as e:
         print("An error occurred while finding element by tag name:", e)
 
 def class_name(value, time=0):
+    """
+    Find a single element by class name.
+    """
     try:
         return find_element(By.CLASS_NAME, value, time).element
     except Exception as e:
         print("An error occurred while finding element by class name:", e)
 
-def css_selector(value,  time=0):
+def css_selector(value, time=0):
+    """
+    Find a single element by CSS selector.
+    """
     try:
         return find_element(By.CSS_SELECTOR, value, time).element
     except Exception as e:
         print("An error occurred while finding element by CSS selector:", e)
 
 def ids(value, time=0):
+    """
+    Find multiple elements by ID.
+    """
     try:
         return find_elements(By.ID, value, time).elements
     except Exception as e:
         print("An error occurred while finding elements by ID:", e)
 
 def names(value, time=0):
+    """
+    Find multiple elements by name attribute.
+    """
     try:
         return find_elements(By.NAME, value, time).elements
     except Exception as e:
         print("An error occurred while finding elements by name:", e)
 
 def xpaths(value, time=0):
+    """
+    Find multiple elements by XPath.
+    """
     try:
         return find_elements(By.XPATH, value, time).elements
     except Exception as e:
-        print("An error occurred while finding elements by xpath:", e)
+        print("An error occurred while finding elements by XPath:", e)
 
 def link_texts(value, time=0):
+    """
+    Find multiple elements by link text.
+    """
     try:
         return find_elements(By.LINK_TEXT, value, time).elements
     except Exception as e:
         print("An error occurred while finding elements by link text:", e)
 
 def partial_link_texts(value, time=0):
+    """
+    Find multiple elements by partial link text.
+    """
     try:
         return find_elements(By.PARTIAL_LINK_TEXT, value, time).elements
     except Exception as e:
         print("An error occurred while finding elements by partial link text:", e)
 
 def tag_names(value, time=0):
+    """
+    Find multiple elements by tag name.
+    """
     try:
         return find_elements(By.TAG_NAME, value, time).elements
     except Exception as e:
         print("An error occurred while finding elements by tag name:", e)
 
 def class_names(value, time=0):
+    """
+    Find multiple elements by class name.
+    """
     try:
         return find_elements(By.CLASS_NAME, value, time).elements
     except Exception as e:
         print("An error occurred while finding elements by class name:", e)
 
 def css_selectors(value, time=0):
+    """
+    Find multiple elements by CSS selector.
+    """
     try:
         return find_elements(By.CSS_SELECTOR, value, time).elements
     except Exception as e:
         print("An error occurred while finding elements by CSS selector:", e)
 
 def browser_version():
+    """
+    Get the version of the browser being used.
+    """
     global driver1
     try:
         return driver1.capabilities['browserVersion']
     except Exception as e:
         print("Exception:", e)
         return ""
 
 def window_position(x, y):
+    """
+    Set the position of the browser window.
+    """
     global driver1
     try:
         driver1.set_window_position(x, y)
     except Exception as e:
         print("Exception:", e)
 
 def window_size(width, height):
+    """
+    Set the size of the browser window.
+    """
     global driver1
     try:
         driver1.set_window_size(width, height)
     except Exception as e:
         print("Exception:", e)
 
 def screenshot(filename=None):
+    """
+    Take a screenshot and save it to the specified filename.
+    """
     global driver1
     try:
         if filename is None:
             filename = "screenshot.png"
         elif not os.path.isabs(filename):
             filename = os.path.join(os.getcwd(), filename)
         
         driver1.save_screenshot(filename)
         print("Screenshot saved at:", filename)
     except Exception as e:
         print("Exception:", e)
 
 def save_cookies(filename=None):
+    """
+    Save the browser's cookies to a file.
+    """
     try:
         if filename is None:
             current_url = driver1.current_url
             parsed_url = urlparse(current_url)
             hostname = parsed_url.hostname
             if hostname:
                 if hostname.startswith("www."):
@@ -213,31 +291,39 @@
         cookies = driver1.get_cookies()
         with io_open(filename, 'wb') as file:
             pickle.dump(cookies, file)
     except Exception as e:
         print("Exception:", e)
 
 def delete_cookies():
+    """
+    Delete all cookies in the browser.
+    """
     try:
         driver1.delete_all_cookies()
     except Exception as e:
         print("Exception:", e)
 
 def set_cookies(filename):
+    """
+    Load cookies from a file and set them in the browser.
+    """
     try:
-
         with io_open(filename, 'rb') as file:
             cookies = pickle.load(file)
 
         for cookie in cookies:
             driver1.add_cookie(cookie)
     except Exception as e:
         print("Exception:", e)
 
 def switch_to_alert(action='accept'):
+    """
+    Switch to an alert and perform an action (accept, cancel, or get text).
+    """
     try:
         alert = driver1.switch_to.alert
         if action == 'accept':
             alert.accept()
         elif action == 'cancel':
             alert.dismiss()
         elif action == 'text':
@@ -246,70 +332,95 @@
             print("Invalid action specified.")
     except NoAlertPresentException:
         print("No alert present")
     except Exception as e:
         print("Exception:", e)
 
 def switch_to_default():
+    """
+    Switch to the default content (main document).
+    """
     try:
         driver1.switch_to.default_content()
     except Exception as e:
         print("Exception:", e)
 
 def switch_to_frame(frame):
+    """
+    Switch to a specified frame.
+    """
     try:
         driver1.switch_to.frame(frame)
     except Exception as e:
         print("Exception:", e)
 
 def switch_to_window(index_or_name):
+    """
+    Switch to a window by index or name.
+    """
     try:
         if isinstance(index_or_name, int):
             driver1.switch_to.window(driver1.window_handles[index_or_name])
         else:
             driver1.switch_to.window(index_or_name)
     except Exception as e:
         print("Exception:", e)
 
 def new_window(url="about:blank"):
+    """
+    Open a new browser window with the specified URL.
+    """
     try:
         driver1.execute_script("window.open(arguments[0], '_blank');", url)
     except Exception as e:
         print("Exception:", e)
 
 def js(script):
+    """
+    Execute a JavaScript script in the browser.
+    """
     try:
         driver1.execute_script(script)
     except Exception as e:
         print("Exception:", e)
 
 def refresh():
+    """
+    Refresh the current page.
+    """
     try:
         driver1.refresh()
     except Exception as e:
         print("Exception:", e)
 
 def forward():
+    """
+    Navigate forward in the browser history.
+    """
     try:
         driver1.forward()
     except Exception as e:
         print("Exception:", e)
 
 def back():
+    """
+    Navigate backward in the browser history.
+    """
     try:
         driver1.back()
     except Exception as e:
         print("Exception:", e)
 
-# def perform_actions(*actions):
-#     global driver1
-#     try:
-#         action_chains = webdriver.ActionChains(driver1)
-#         for action in actions:
-#             action_chains = action_chains.perform(action)
-#     except Exception as e:
-#         print("Exception:", e)
+
+def hhh():
+    """
+    Navigate backward in the browser history.
+    """
+    try:
+        driver1.back()
+    except Exception as e:
+        print("Exception:", e)
 
 __all__ = ['driver', 'open', 'close', 'id', 'name', 'xpath', 'link_text', 'partial_link_text', 'tag_name', 'class_name', 'css_selector', 
            'ids', 'names', 'xpaths', 'link_texts', 'partial_link_texts', 'tag_names', 'class_names', 'css_selectors', 'browser_version',
            'window_position', 'window_size', 'screenshot', 'save_cookies', 'delete_cookies', 'set_cookies', 'switch_to_alert', 'switch_to_default',
-           'switch_to_frame', 'switch_to_window', 'new_window', 'js', 'refresh', 'back', 'forward']
+           'switch_to_frame', 'switch_to_window', 'new_window', 'js', 'refresh', 'back', 'forward', 'hhh']
```

### Comparing `liteium-1.0.4/setup.py` & `liteium-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from setuptools import setup, find_packages
 
+with open('README.md', encoding='utf-8') as f:
+    long_description = f.read()
+
 setup(
     name='liteium',
-    version='1.0.4',
+    version='1.0.5',
     description='Description of your package',
-    long_description=open('README.md').read(),
+    long_description=long_description,
     long_description_content_type='text/markdown',
     author='El Bettioui Reda',
     author_email='redaelbettioui@gmail.com',
     url='https://github.com/XredaX/liteium',
     packages=find_packages(),
     install_requires=[
         'selenium',
```

