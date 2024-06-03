# Comparing `tmp/lavague_drivers_selenium-0.2.0.tar.gz` & `tmp/lavague_drivers_selenium-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_drivers_selenium-0.2.0.tar", max compression
+gzip compressed data, was "lavague_drivers_selenium-0.2.1.tar", max compression
```

## Comparing `lavague_drivers_selenium-0.2.0.tar` & `lavague_drivers_selenium-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       34 2024-05-28 08:59:04.857656 lavague_drivers_selenium-0.2.0/README.md
--rw-r--r--   0        0        0       57 2024-05-28 08:59:04.858191 lavague_drivers_selenium-0.2.0/lavague/drivers/selenium/__init__.py
--rw-r--r--   0        0        0    28288 2024-05-28 21:01:47.308219 lavague_drivers_selenium-0.2.0/lavague/drivers/selenium/base.py
--rw-r--r--   0        0        0      976 2024-05-28 21:04:27.242800 lavague_drivers_selenium-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-05-28 08:59:04.857656 lavague_drivers_selenium-0.2.1/README.md
+-rw-r--r--   0        0        0       57 2024-05-28 08:59:04.858191 lavague_drivers_selenium-0.2.1/lavague/drivers/selenium/__init__.py
+-rw-r--r--   0        0        0    19441 2024-06-03 12:55:13.235262 lavague_drivers_selenium-0.2.1/lavague/drivers/selenium/base.py
+-rw-r--r--   0        0        0      976 2024-06-03 12:53:32.164094 lavague_drivers_selenium-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.2.1/PKG-INFO
```

### Comparing `lavague_drivers_selenium-0.2.0/lavague/drivers/selenium/base.py` & `lavague_drivers_selenium-0.2.1/lavague/drivers/selenium/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -267,40 +267,8 @@
 # /html/body/section/devsite-header/div/div[1]/div/div/div[2]/div[1]/devsite-tabs/nav/tab[2]/div/tab[1]/a
 
 # Thus, we use this XPATH to identify and click on the "Gemma" option:
 gemma_option = driver.find_element(By.XPATH, "/html/body/section/devsite-header/div/div[1]/div/div/div[2]/div[1]/devsite-tabs/nav/tab[2]/div/tab[1]/a")
 gemma_option.click()
 ```
 ---
-HTML:
-<div class="_8dhNBCZ2S74-" data-test="icCalendar-wrapper" style="border: 2px solid red;" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[1]/div"><span aria-hidden="true" class="irNswZTgdxU- ywR-N4gLSdc-" data-test="icCalendar" data-testid="icCalendar" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[1]/div/span"><svg viewbox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[1]/div/span/svg"><path d="M7 4a1 1 0 0 1 2 0v1h6V4a1 1 0 1 1 2 0v1h2a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V7a2 2 0 0 1 2-2h2V4ZM5 7v2h14V7H5Zm0 4v8h14v-8H5Z" fill="#2D333F" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[1]/div/span/svg/path"></path></svg></span><p class="Z5-QmB-1pug-" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[1]/div/p">Tue, May 21</p></div></li><li class="c2SNlvnt0Z4-" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[2]"><div class="_8dhNBCZ2S74-" data-test="icClock-wrapper" style="border: 2px solid red;" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[2]/div"><span aria-hidden="true" class="irNswZTgdxU- ywR-N4gLSdc-" data-test="icClock" data-testid="icClock" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[2]/div/span"><svg viewbox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[2]/div/span/svg"><path d="M11 7.5a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 .5.5V11h1.5a.5.5 0 0 1 .5.5v1a.5.5 0 0 1-.5.5h-3a.5.5 0 0 1-.5-.5v-5Z" fill="#2D333F" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[2]/div/span/svg/path[1]"></path><path d="M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Zm-2 0a7 7 0 1 0-14 0 7 7 0 0 0 14 0Z" fill="#2D333F" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[2]/div/span/svg/path[2]"></path></svg></span><p class="Z5-QmB-1pug-" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[2]/div/p">8:30 PM</p></div></li><li class="c2SNlvnt0Z4-" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[3]"><div class="_8dhNBCZ2S74-" data-test="icPerson-wrapper" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[3]/div"><span aria-hidden="true" class="irNswZTgdxU- ywR-N4gLSdc-" data-test="icPerson" data-testid="icPerson" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[3]/div/span"><svg viewbox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[3]/div/span/svg"><path d="M7.002 8a5 5 0 1 1 7.572 4.288c2.43.594 4.162 2.108 5.192 4.543A3 3 0 0 1 17.004 21H7a3 3 0 0 1-2.763-4.169c1.03-2.435 2.759-3.949 5.19-4.543A4.995 4.995 0 0 1 7.002 8Zm2 0A2.999 2.999 0 1 0 15 8a3 3 0 1 0-6 0Zm-2.31 10.949a.994.994 0 0 0 .316.051h9.987a1 1 0 0 0 .95-1.314C17.13 15.229 15.15 14 12.002 14c-3.15 0-5.13 1.229-5.943 3.686a.999.999 0 0 0 .634 1.263Z" fill="#2D333F" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[3]/div/span/svg/path"></path></svg></span><p class="Z5-QmB-1pug-" xpath="/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[3]/div/p">2 people</p></div></li></ul></div></div></div>
-<div id="onetrust-consent-sdk" xpath="/html/body/div[2]"><div class="onetrust-pc-dark-filter ot-hide ot-fade-in" xpath="/html/body/div[2]/div[1]"></div><div aria-label="Preference center" class="otPcCenter ot-hide ot-fade-in" id="onetrust-pc-sdk" lang="en" role="region" xpath="/html/body/div[2]/div[2]"><div aria-describedby="ot-pc-desc" aria-label="Privacy Preference Center" aria-modal="true" role="alertdialog" style="height: 100%;" xpath="/html/body/div[2]/div[2]/div"><!-- Close Button --><div class="ot-pc-header" xpath="/html/body/div[2]/div[2]/div/div[1]"><!-- Logo Tag --><div aria-label="Company Logo" class="ot-pc-logo" role="img" xpath="/html/body/div[2]/div[2]/div/div[1]/div"><img alt="Company Logo" src="https://cdn.cookielaw.org/logos/static/ot_company_logo.png" xpath="/html/body/div[2]/div[2]/div/div[1]/div/img"/></div><button aria-label="Close" class="ot-close-icon" id="close-pc-btn-handler" style='background-image: url("https://cdn.cookielaw.org/logos/static/ot_close.svg");' xpath="/html/body/div[2]/div[2]/div/div[1]/button"></button></div><!-- Close Button --><div class="ot-pc-scrollbar" id="ot-pc-content" xpath="/html/body/div[2]/div[2]/div/div[2]"><div class="ot-optout-signal ot-hide" xpath="/html/body/div[2]/div[2]/div/div[2]/div[1]"><div class="ot-optout-icon" xpath="/html/body/div[2]/div[2]/div/div[2]/div[1]/div"><svg xmlns="http://www.w3.org/2000/svg" xpath="/html/body/div[2]/div[2]/div/div[2]/div[1]/div/svg"><path class="ot-floating-button__svg-fill" d="M14.588 0l.445.328c1.807 1.303 3.961 2.533 6.461 3.688 2.015.93 4.576 1.746 7.682 2.446 0 14.178-4.73 24.133-14.19 29.864l-.398.236C4.863 30.87 0 20.837 0 6.462c3.107-.7 5.668-1.516 7.682-2.446 2.709-1.251 5.01-2.59 6.906-4.016zm5.87 13.88a.75.75 0 00-.974.159l-5.475 6.625-3.005-2.997-.077-.067a.75.75 0 00-.983 1.13l4.172 4.16 6.525-7.895.06-.083a.75.75 0 00-.16-.973z" fill="#FFF" fill-rule="evenodd" xpath="/html/body/div[2]/div[2]/div/div[2]/div[1]/div/svg/path"></path></svg></div><span xpath="/html/body/div[2]/div[2]/div/div[2]/div[1]/span"></span></div><h2 id="ot-pc-title" xpath="/html/body/div[2]/div[2]/div/div[2]/h2">Privacy Preference Center</h2><div id="ot-pc-desc" xpath="/html/body/div[2]/div[2]/div/div[2]/div[2]">When you visit any website, it may store or retrieve information on your browser, mostly in the form of cookies. This information might be about you, your preferences or your device and is mostly used to make the site work as you expect it to. The information does not usually directly identify you, but it can give you a more personalized web experience. Because we respect your right to privacy, you can choose not to allow some types of cookies. Click on the different category headings to find out more and change our default settings. However, blocking some types of cookies may impact your experience of the site and the services we are able to offer.
-For additional information, please visit our <a href="https://www.opentable.com/legal/cookie-policy" xpath="/html/body/div[2]/div[2]/div/div[2]/div[2]/a[1]">Cookies Policy</a> and our <a href="https://www.opentable.com/legal/privacy-policy" xpath="/html/body/div[2]/div[2]/div/div[2]/div[2]/a[2]">Privacy Policy</a>.</div><button id="accept-recommended-btn-handler" xpath="/html/body/div[2]/div[2]/div/div[2]/button">Allow All</button><section class="ot-sdk-row ot-cat-grp" xpath="/html/body/div[2]/div[2]/div/div[2]/section"><h3 id="ot-category-title" xpath="/html/body/div[2]/div[2]/div/div[2]/section/h3"> Manage Consent Preferences</h3><div class="ot-accordion-layout ot-cat-item ot-vs-config" data-optanongroupid="C0001" xpath="/html/body/div[2]/div[2]/div/div[2]/section/div[1]"><button aria-controls="ot-desc-id-C0001" aria-expanded="false" aria-labelledby="ot-header-id-C0001 ot-status-id-C0001" ot-accordion="true" xpath="/html/body/div[2]/div[2]/div/div[2]/section/div[1]/button"></button><!-- Accordion header -->
-Query: Click on the date selector and choose May 25th. Then, click on the time selector and choose 1:00 PM.
-Completion:
-```python
-# Let's think step by step
-
-# The query asks us to first click on the date selector and choose May 25th. 
-# Then, we need to click on the time selector and choose 1:00 PM.
-
-# In the provided HTML, we can see the date selector and time selector elements within a list structure.
-
-# We need to identify the correct elements for both the date and time selectors.
-
-# First, we locate the date selector. It is inside a div element with a specific class and data-test attributes.
-# The date selector is found at the following XPath:
-date_selector = driver.find_element(By.XPATH, "/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[1]/div")
-
-# Click on the date selector to open the date selection dropdown
-date_selector.click()
-
-# To choose May 25th, we would typically need to select it from the opened date picker. This part is omitted in the explanation for brevity.
-
-# Next, we locate the time selector. It is also inside a div element with specific class and data-test attributes.
-# The time selector is found at the following XPath:
-time_selector = driver.find_element(By.XPATH, "/html/body/div[1]/div/div/main/div/div/div/section/div[1]/div[2]/div/ul/li[2]/div")
-
-# Click on the time selector to open the time selection dropdown
-time_selector.click()
-```python
 """
```

### Comparing `lavague_drivers_selenium-0.2.0/pyproject.toml` & `lavague_drivers_selenium-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-drivers-selenium"
-version = "0.2.0"
+version = "0.2.1"
 description = "Selenium integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_drivers_selenium-0.2.0/PKG-INFO` & `lavague_drivers_selenium-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-drivers-selenium
-Version: 0.2.0
+Version: 0.2.1
 Summary: Selenium integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,selenium
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

