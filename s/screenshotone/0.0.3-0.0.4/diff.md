# Comparing `tmp/screenshotone-0.0.3.tar.gz` & `tmp/screenshotone-0.0.4.tar.gz`

## Comparing `screenshotone-0.0.3.tar` & `screenshotone-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 screenshotone-0.0.3/.github/workflows/pypi-release.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 screenshotone-0.0.3/src/screenshotone/__init__.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 screenshotone-0.0.3/src/screenshotone/sdk.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 screenshotone-0.0.3/LICENSE
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 screenshotone-0.0.3/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 screenshotone-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 screenshotone-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 screenshotone-0.0.4/.github/workflows/pypi-release.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 screenshotone-0.0.4/src/screenshotone/__init__.py
+-rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 screenshotone-0.0.4/src/screenshotone/sdk.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 screenshotone-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 screenshotone-0.0.4/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 screenshotone-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 screenshotone-0.0.4/PKG-INFO
```

### Comparing `screenshotone-0.0.3/.github/workflows/pypi-release.yml` & `screenshotone-0.0.4/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `screenshotone-0.0.3/src/screenshotone/sdk.py` & `screenshotone-0.0.4/src/screenshotone/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,19 @@
         return self
 
     def block_cookie_banners(self, value): 	
         self.options['block_cookie_banners'] = value
 
         return self
 
+    def block_banners_by_heuristics(self, value): 	
+        self.options['block_banners_by_heuristics'] = value
+
+        return self
+
     def block_chats(self, value): 	
         self.options['block_chats'] = value
 
         return self
 
     def block_ads(self, value): 	
         self.options['block_ads'] = value
```

### Comparing `screenshotone-0.0.3/LICENSE` & `screenshotone-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `screenshotone-0.0.3/README.md` & `screenshotone-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -38,10 +38,14 @@
 image = client.take(options)
 
 # store the screenshot the example.png file
 with open('example.png', 'wb') as result_file:
     shutil.copyfileobj(image, result_file)
 ```
 
+## Release 
+
+[Github Actions](https://github.com/screenshotone/pythonsdk/blob/main/.github/workflows/pypi-release.yml) is used to automate the release process and publishing to PyPI. Update the library version in `pyproject.toml` and [create a new release](https://github.com/screenshotone/pythonsdk/releases/new) to launch the `publish` workflow. 
+
 ## License 
 
 `screenshotone/pythonsdk` is released under [the MIT license](LICENSE).
```

### Comparing `screenshotone-0.0.3/pyproject.toml` & `screenshotone-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "screenshotone"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Dmytro Krasun", email="support@screenshotone.com" },
 ]
 dependencies = [
     "requests >= 2.28.1"
 ]
 description = "A Python SDK for ScreenshotOne.com API to take screenshots of URLs, render HTML as images and PDF"
```

### Comparing `screenshotone-0.0.3/PKG-INFO` & `screenshotone-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenshotone
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python SDK for ScreenshotOne.com API to take screenshots of URLs, render HTML as images and PDF
 Project-URL: Homepage, https://screenshotone.com/
 Project-URL: Docs, https://screenshotone.com/docs/getting-started/
 Author-email: Dmytro Krasun <support@screenshotone.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,10 +53,14 @@
 image = client.take(options)
 
 # store the screenshot the example.png file
 with open('example.png', 'wb') as result_file:
     shutil.copyfileobj(image, result_file)
 ```
 
+## Release 
+
+[Github Actions](https://github.com/screenshotone/pythonsdk/blob/main/.github/workflows/pypi-release.yml) is used to automate the release process and publishing to PyPI. Update the library version in `pyproject.toml` and [create a new release](https://github.com/screenshotone/pythonsdk/releases/new) to launch the `publish` workflow. 
+
 ## License 
 
 `screenshotone/pythonsdk` is released under [the MIT license](LICENSE).
```

