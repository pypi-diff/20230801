# Comparing `tmp/rtsf-web-1.3.5.tar.gz` & `tmp/rtsf-web-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rtsf-web-1.3.5.tar", last modified: Tue Nov  9 04:32:20 2021, max compression
+gzip compressed data, was "dist\rtsf-web-1.3.6.tar", last modified: Tue Aug  1 01:39:24 2023, max compression
```

## Comparing `rtsf-web-1.3.5.tar` & `rtsf-web-1.3.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2021-11-09 04:32:20.000000 rtsf-web-1.3.5/
--rw-rw-rw-   0        0        0    25257 2021-11-09 04:32:20.000000 rtsf-web-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    21165 2021-11-09 04:23:53.000000 rtsf-web-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2021-11-09 04:32:20.000000 rtsf-web-1.3.5/rtsf_web.egg-info/
--rw-rw-rw-   0        0        0        1 2021-11-09 04:32:19.000000 rtsf-web-1.3.5/rtsf_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      180 2021-11-09 04:32:19.000000 rtsf-web-1.3.5/rtsf_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    25257 2021-11-09 04:32:19.000000 rtsf-web-1.3.5/rtsf_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       23 2021-11-09 04:32:19.000000 rtsf-web-1.3.5/rtsf_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0      926 2021-11-09 04:32:19.000000 rtsf-web-1.3.5/rtsf_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2021-11-09 04:32:19.000000 rtsf-web-1.3.5/rtsf_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-11-09 04:32:20.000000 rtsf-web-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     2793 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:32:20.000000 rtsf-web-1.3.5/webuidriver/
--rw-rw-rw-   0        0        0    23527 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/actions.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:32:20.000000 rtsf-web-1.3.5/webuidriver/chrome/
--rw-rw-rw-   0        0        0     1727 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/chrome/options.py
--rw-rw-rw-   0        0        0      355 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/chrome/webdriver.py
--rw-rw-rw-   0        0        0       37 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/chrome/__init__.py
--rw-rw-rw-   0        0        0     6026 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/cli.py
--rw-rw-rw-   0        0        0     8071 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/driver.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:32:20.000000 rtsf-web-1.3.5/webuidriver/edge/
--rw-rw-rw-   0        0        0      347 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/edge/webdriver.py
--rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/edge/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:32:20.000000 rtsf-web-1.3.5/webuidriver/firefox/
--rw-rw-rw-   0        0        0     1304 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/firefox/firefox_profile.py
--rw-rw-rw-   0        0        0      359 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/firefox/webdriver.py
--rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/firefox/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:32:20.000000 rtsf-web-1.3.5/webuidriver/ie/
--rw-rw-rw-   0        0        0      339 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/ie/webdriver.py
--rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/ie/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:32:20.000000 rtsf-web-1.3.5/webuidriver/opera/
--rw-rw-rw-   0        0        0      353 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/opera/webdriver.py
--rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/opera/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:32:20.000000 rtsf-web-1.3.5/webuidriver/remote/
--rw-rw-rw-   0        0        0     3703 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/remote/SeleniumHatch.py
--rw-rw-rw-   0        0        0     2856 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/remote/SeleniumJar.py
--rw-rw-rw-   0        0        0     5917 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/remote/wait_until.py
--rw-rw-rw-   0        0        0      355 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/remote/webdriver.py
--rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/remote/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:32:20.000000 rtsf-web-1.3.5/webuidriver/safari/
--rw-rw-rw-   0        0        0      357 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/safari/webdriver.py
--rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/safari/__init__.py
--rw-rw-rw-   0        0        0      341 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/__about__.py
--rw-rw-rw-   0        0        0      526 2021-11-09 04:19:43.000000 rtsf-web-1.3.5/webuidriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/
+-rw-rw-rw-   0        0        0    25257 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0    21165 2021-11-09 04:23:53.000000 rtsf-web-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      180 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    25257 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      926 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     2877 2023-08-01 01:33:06.000000 rtsf-web-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/
+-rw-rw-rw-   0        0        0    23527 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/actions.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/chrome/
+-rw-rw-rw-   0        0        0     1727 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/chrome/options.py
+-rw-rw-rw-   0        0        0      355 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/chrome/webdriver.py
+-rw-rw-rw-   0        0        0       37 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/chrome/__init__.py
+-rw-rw-rw-   0        0        0     6026 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/cli.py
+-rw-rw-rw-   0        0        0     8071 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/driver.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/edge/
+-rw-rw-rw-   0        0        0      347 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/edge/webdriver.py
+-rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/edge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/firefox/
+-rw-rw-rw-   0        0        0     1304 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/firefox/firefox_profile.py
+-rw-rw-rw-   0        0        0      359 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/firefox/webdriver.py
+-rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/firefox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/ie/
+-rw-rw-rw-   0        0        0      339 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/ie/webdriver.py
+-rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/ie/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/opera/
+-rw-rw-rw-   0        0        0      353 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/opera/webdriver.py
+-rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/opera/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/remote/
+-rw-rw-rw-   0        0        0     3703 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/remote/SeleniumHatch.py
+-rw-rw-rw-   0        0        0     2856 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/remote/SeleniumJar.py
+-rw-rw-rw-   0        0        0     5917 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/remote/wait_until.py
+-rw-rw-rw-   0        0        0      355 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/remote/webdriver.py
+-rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/remote/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/safari/
+-rw-rw-rw-   0        0        0      357 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/safari/webdriver.py
+-rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/safari/__init__.py
+-rw-rw-rw-   0        0        0      341 2023-08-01 01:33:56.000000 rtsf-web-1.3.6/webuidriver/__about__.py
+-rw-rw-rw-   0        0        0      578 2023-08-01 01:31:48.000000 rtsf-web-1.3.6/webuidriver/__init__.py
```

### Comparing `rtsf-web-1.3.5/PKG-INFO` & `rtsf-web-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtsf-web
-Version: 1.3.5
+Version: 1.3.6
 Summary: only for web ui test, base on rtsf
 Home-page: https://github.com/RockFeng0/rtsf-web
 Author: 罗科峰
 Author-email: lkf20031988@163.com
 License: MIT
 Description: # rtsf-web
          基于rtsf测试框架和selenium程序框架，关键字驱动Web UI层面，进行自动化的功能测试
```

### Comparing `rtsf-web-1.3.5/README.md` & `rtsf-web-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.5/rtsf_web.egg-info/PKG-INFO` & `rtsf-web-1.3.6/rtsf_web.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtsf-web
-Version: 1.3.5
+Version: 1.3.6
 Summary: only for web ui test, base on rtsf
 Home-page: https://github.com/RockFeng0/rtsf-web
 Author: 罗科峰
 Author-email: lkf20031988@163.com
 License: MIT
 Description: # rtsf-web
          基于rtsf测试框架和selenium程序框架，关键字驱动Web UI层面，进行自动化的功能测试
```

### Comparing `rtsf-web-1.3.5/rtsf_web.egg-info/SOURCES.txt` & `rtsf-web-1.3.6/rtsf_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.5/setup.py` & `rtsf-web-1.3.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,35 +54,35 @@
         os.system('git tag v{0}'.format(__about__.__version__))
         os.system('git push --tags')
 
         sys.exit()
 
 
 install_requires = [
-    "selenium",
+    "selenium>=3.141.0",  # 建议版本 python 3.6 + selenium 3.141.0;  如果使用selenium 4，需要python>=3.7
     "requests",
     "rtsf",
 ]
 
 # dependency_links=[
 # "git+https://github.com/RockFeng0/rtsf.git#egg=rtsf-0"
 # ]
 
 setup(
         name=__about__.__title__,
-        version=__about__.__version__,        
+        version=__about__.__version__,
         description=__about__.__short_desc__,
         long_description=long_description,
         long_description_content_type='text/markdown',
         author=__about__.__autor__,
         author_email=__about__.__author_email__,
         url=__about__.HOME_PAGE,
         license=__about__.__license__,
         python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4',
-        packages=find_packages(exclude=()),        
+        packages=find_packages(exclude=()),
         keywords='test web ui',
         install_requires=install_requires,
         # dependency_links=dependency_links,
         extras_require={},
         entry_points={
             'console_scripts': [
                 'wldriver=webuidriver.cli:local_main_run',  # local driver
```

### Comparing `rtsf-web-1.3.5/webuidriver/actions.py` & `rtsf-web-1.3.6/webuidriver/actions.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.5/webuidriver/chrome/options.py` & `rtsf-web-1.3.6/webuidriver/chrome/options.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.5/webuidriver/cli.py` & `rtsf-web-1.3.6/webuidriver/cli.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.5/webuidriver/driver.py` & `rtsf-web-1.3.6/webuidriver/driver.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.5/webuidriver/firefox/firefox_profile.py` & `rtsf-web-1.3.6/webuidriver/firefox/firefox_profile.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.5/webuidriver/remote/SeleniumHatch.py` & `rtsf-web-1.3.6/webuidriver/remote/SeleniumHatch.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.5/webuidriver/remote/SeleniumJar.py` & `rtsf-web-1.3.6/webuidriver/remote/SeleniumJar.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.5/webuidriver/remote/wait_until.py` & `rtsf-web-1.3.6/webuidriver/remote/wait_until.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.5/webuidriver/__init__.py` & `rtsf-web-1.3.6/webuidriver/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .firefox.webdriver import WebDriver as Firefox  # noqa
 from .firefox.firefox_profile import FirefoxProfile  # noqa
 from .chrome.webdriver import WebDriver as Chrome  # noqa
 from .chrome.options import Options as ChromeOptions  # noqa
 from .ie.webdriver import WebDriver as Ie  # noqa
 from .edge.webdriver import WebDriver as Edge  # noqa
-from .opera.webdriver import WebDriver as Opera  # noqa
+# from .opera.webdriver import WebDriver as Opera  # opera不支持w3c标准，因此selenium 4存在问题
 from .safari.webdriver import WebDriver as Safari  # noqa
 from .remote.webdriver import WebDriver as Remote  # noqa
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

