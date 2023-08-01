# Comparing `tmp/agentbrowser-0.2.0.tar.gz` & `tmp/agentbrowser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentbrowser-0.2.0.tar", last modified: Tue Aug  1 04:49:46 2023, max compression
+gzip compressed data, was "agentbrowser-0.2.1.tar", last modified: Tue Aug  1 11:53:41 2023, max compression
```

## Comparing `agentbrowser-0.2.0.tar` & `agentbrowser-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:49:46.141365 agentbrowser-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-01 04:49:46.141365 agentbrowser-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:49:46.137365 agentbrowser-0.2.0/agentbrowser/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/agentbrowser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/agentbrowser/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/agentbrowser/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/agentbrowser/test_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:49:46.141365 agentbrowser-0.2.0/agentbrowser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-01 04:49:46.000000 agentbrowser-0.2.0/agentbrowser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 04:49:46.000000 agentbrowser-0.2.0/agentbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:49:46.000000 agentbrowser-0.2.0/agentbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 04:49:46.000000 agentbrowser-0.2.0/agentbrowser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 04:49:46.000000 agentbrowser-0.2.0/agentbrowser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 04:49:46.141365 agentbrowser-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 04:49:33.000000 agentbrowser-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:53:41.282443 agentbrowser-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-01 11:53:27.000000 agentbrowser-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-08-01 11:53:41.282443 agentbrowser-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-08-01 11:53:27.000000 agentbrowser-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:53:41.282443 agentbrowser-0.2.1/agentbrowser/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:53:27.000000 agentbrowser-0.2.1/agentbrowser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10617 2023-08-01 11:53:27.000000 agentbrowser-0.2.1/agentbrowser/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-01 11:53:27.000000 agentbrowser-0.2.1/agentbrowser/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-01 11:53:27.000000 agentbrowser-0.2.1/agentbrowser/test_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:53:41.282443 agentbrowser-0.2.1/agentbrowser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-08-01 11:53:41.000000 agentbrowser-0.2.1/agentbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 11:53:41.000000 agentbrowser-0.2.1/agentbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:53:41.000000 agentbrowser-0.2.1/agentbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 11:53:41.000000 agentbrowser-0.2.1/agentbrowser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 11:53:41.000000 agentbrowser-0.2.1/agentbrowser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:53:41.282443 agentbrowser-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-01 11:53:27.000000 agentbrowser-0.2.1/setup.py
```

### Comparing `agentbrowser-0.2.0/LICENSE` & `agentbrowser-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentbrowser-0.2.0/PKG-INFO` & `agentbrowser-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: agentbrowser
-Version: 0.2.0
+Version: 0.2.1
 Summary: A browser for your agent, built on Playwright.
-Home-page: https://github.com/lalalune/agentbrowser
+Home-page: https://github.com/AutonomousResearchGroup/agentbrowser
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `agentbrowser-0.2.0/README.md` & `agentbrowser-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `agentbrowser-0.2.0/agentbrowser/browser.py` & `agentbrowser-0.2.1/agentbrowser/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     :param url: The URL to navigate to.
     :type url: str
     :param page: The page to navigate in.
     :type page: playwright.async_api.Page
     :return: The page after navigation.
     :rtype: playwright.async_api.Page
     """
+    ensure_event_loop()
     return asyncio.get_event_loop().run_until_complete(async_navigate_to(url, page, wait_until=wait_until))
 
 
 def get_document_html(page):
     """
     Get the HTML content of a page.
```

### Comparing `agentbrowser-0.2.0/agentbrowser/test.py` & `agentbrowser-0.2.1/agentbrowser/test.py`

 * *Files identical despite different names*

### Comparing `agentbrowser-0.2.0/agentbrowser/test_async.py` & `agentbrowser-0.2.1/agentbrowser/test_async.py`

 * *Files identical despite different names*

### Comparing `agentbrowser-0.2.0/agentbrowser.egg-info/PKG-INFO` & `agentbrowser-0.2.1/agentbrowser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: agentbrowser
-Version: 0.2.0
+Version: 0.2.1
 Summary: A browser for your agent, built on Playwright.
-Home-page: https://github.com/lalalune/agentbrowser
+Home-page: https://github.com/AutonomousResearchGroup/agentbrowser
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `agentbrowser-0.2.0/setup.py` & `agentbrowser-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="agentbrowser",
-    version="0.2.0",
+    version="0.2.1",
     description="A browser for your agent, built on Playwright.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
-    url="https://github.com/lalalune/agentbrowser",
+    url="https://github.com/AutonomousResearchGroup/agentbrowser",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
     packages=["agentbrowser"],
     install_requires=["playwright"],
     readme="README.md",
     classifiers=[
```

