# Comparing `tmp/dark_web_scraper-0.3.tar.gz` & `tmp/dark_web_scraper-1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dark_web_scraper-0.3.tar", last modified: Mon Jul 31 14:36:28 2023, max compression
+gzip compressed data, was "dark_web_scraper-1.tar", last modified: Mon Jul 31 19:38:18 2023, max compression
```

## Comparing `dark_web_scraper-0.3.tar` & `dark_web_scraper-1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 14:36:28.859561 dark_web_scraper-0.3/
--rw-rw-rw-   0        0        0     1087 2023-07-30 16:23:56.000000 dark_web_scraper-0.3/LICENSE
--rw-rw-rw-   0        0        0     2112 2023-07-31 14:36:28.858410 dark_web_scraper-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1599 2023-07-31 14:31:05.000000 dark_web_scraper-0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 14:36:28.860565 dark_web_scraper-0.3/setup.cfg
--rw-rw-rw-   0        0        0      900 2023-07-31 14:36:13.000000 dark_web_scraper-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:36:28.775247 dark_web_scraper-0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 14:36:28.847463 dark_web_scraper-0.3/src/dark_web_scraper.egg-info/
--rw-rw-rw-   0        0        0     2112 2023-07-31 14:36:28.000000 dark_web_scraper-0.3/src/dark_web_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-07-31 14:36:28.000000 dark_web_scraper-0.3/src/dark_web_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 14:36:28.000000 dark_web_scraper-0.3/src/dark_web_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-31 14:36:28.000000 dark_web_scraper-0.3/src/dark_web_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-31 14:36:28.000000 dark_web_scraper-0.3/src/dark_web_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2222 2023-07-30 18:04:28.000000 dark_web_scraper-0.3/src/dark_web_scraper.py
+drwxrwxrwx   0        0        0        0 2023-07-31 19:38:18.836801 dark_web_scraper-1/
+-rw-rw-rw-   0        0        0     1087 2023-07-30 16:23:56.000000 dark_web_scraper-1/LICENSE
+-rw-rw-rw-   0        0        0     3524 2023-07-31 19:38:18.833552 dark_web_scraper-1/PKG-INFO
+-rw-rw-rw-   0        0        0     3013 2023-07-31 19:36:28.000000 dark_web_scraper-1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 19:38:18.836801 dark_web_scraper-1/setup.cfg
+-rw-rw-rw-   0        0        0      898 2023-07-31 19:36:49.000000 dark_web_scraper-1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 19:38:18.787635 dark_web_scraper-1/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 19:38:18.831510 dark_web_scraper-1/src/dark_web_scraper.egg-info/
+-rw-rw-rw-   0        0        0     3524 2023-07-31 19:38:18.000000 dark_web_scraper-1/src/dark_web_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-07-31 19:38:18.000000 dark_web_scraper-1/src/dark_web_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 19:38:18.000000 dark_web_scraper-1/src/dark_web_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-31 19:38:18.000000 dark_web_scraper-1/src/dark_web_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 19:38:18.000000 dark_web_scraper-1/src/dark_web_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2210 2023-07-31 19:33:40.000000 dark_web_scraper-1/src/dark_web_scraper.py
```

### Comparing `dark_web_scraper-0.3/LICENSE` & `dark_web_scraper-1/LICENSE`

 * *Files identical despite different names*

### Comparing `dark_web_scraper-0.3/setup.py` & `dark_web_scraper-1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='dark_web_scraper',
-    version='0.3',
+    version='1',
     description='A dark web link and image scraper',
     author= 'Pritam Sarbajna',
     url = 'https://github.com/PritamSarbajna/dark-web-scraper',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     keywords=['darkweb', 'web scraper', 'scraper'],
```

### Comparing `dark_web_scraper-0.3/src/dark_web_scraper.py` & `dark_web_scraper-1/src/dark_web_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 proxies = {
     'http': 'socks5h://localhost:9050',
     'https': 'socks5h://localhost:9050'
 }
 
 headers = { 'User-Agent': UserAgent().random }
 
-url = ''
-
 
 
 def find_onion_links(url):
     response = requests.get(url, headers=headers, proxies=proxies)
 
     soup = BeautifulSoup(response.text, 'html.parser')
```

