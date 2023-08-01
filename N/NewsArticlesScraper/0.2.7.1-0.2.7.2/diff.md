# Comparing `tmp/NewsArticlesScraper-0.2.7.1.tar.gz` & `tmp/NewsArticlesScraper-0.2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\NewsArticlesScraper-0.2.7.1.tar", last modified: Thu Jul 27 04:29:09 2023, max compression
+gzip compressed data, was "dist\NewsArticlesScraper-0.2.7.2.tar", last modified: Tue Aug  1 11:06:39 2023, max compression
```

## Comparing `NewsArticlesScraper-0.2.7.1.tar` & `NewsArticlesScraper-0.2.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 04:29:09.363278 NewsArticlesScraper-0.2.7.1/
-drwxrwxrwx   0        0        0        0 2023-07-27 04:29:09.335364 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper/
--rw-rw-rw-   0        0        0    11240 2023-07-27 04:28:28.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper/ArticleUrlSrapers.py
--rw-rw-rw-   0        0        0    14676 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper/Scrapers.py
--rw-rw-rw-   0        0        0       64 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 04:29:09.360280 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/
--rw-rw-rw-   0        0        0      650 2023-07-27 04:29:09.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-07-27 04:29:09.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 04:29:09.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-27 04:29:09.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-27 04:29:09.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      650 2023-07-27 04:29:09.362273 NewsArticlesScraper-0.2.7.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-27 04:29:09.363278 NewsArticlesScraper-0.2.7.1/setup.cfg
--rw-rw-rw-   0        0        0      998 2023-07-27 04:28:28.000000 NewsArticlesScraper-0.2.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:06:39.086018 NewsArticlesScraper-0.2.7.2/
+drwxrwxrwx   0        0        0        0 2023-08-01 11:06:39.069774 NewsArticlesScraper-0.2.7.2/NewsArticlesScraper/
+-rw-rw-rw-   0        0        0    11241 2023-08-01 10:56:58.000000 NewsArticlesScraper-0.2.7.2/NewsArticlesScraper/ArticleUrlSrapers.py
+-rw-rw-rw-   0        0        0    14676 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.2/NewsArticlesScraper/Scrapers.py
+-rw-rw-rw-   0        0        0       64 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.2/NewsArticlesScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:06:39.083086 NewsArticlesScraper-0.2.7.2/NewsArticlesScraper.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-08-01 11:06:38.000000 NewsArticlesScraper-0.2.7.2/NewsArticlesScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-08-01 11:06:38.000000 NewsArticlesScraper-0.2.7.2/NewsArticlesScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 11:06:38.000000 NewsArticlesScraper-0.2.7.2/NewsArticlesScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-01 11:06:38.000000 NewsArticlesScraper-0.2.7.2/NewsArticlesScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-01 11:06:38.000000 NewsArticlesScraper-0.2.7.2/NewsArticlesScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      650 2023-08-01 11:06:39.084024 NewsArticlesScraper-0.2.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 11:06:39.086018 NewsArticlesScraper-0.2.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      998 2023-08-01 11:06:10.000000 NewsArticlesScraper-0.2.7.2/setup.py
```

### Comparing `NewsArticlesScraper-0.2.7.1/NewsArticlesScraper/ArticleUrlSrapers.py` & `NewsArticlesScraper-0.2.7.2/NewsArticlesScraper/ArticleUrlSrapers.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         'LOG_LEVEL': 'WARN',
         'USER_AGENT': 'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.1 (KHTML, like Gecko) Chrome/22.0.1207.1 '
                       'Safari/537.1',
         'ROBOTSTXT_OBEY': False,
         'DOWNLOAD_DELAY': 12,
         # 'JOBDIR': './News/NYTJobs',
         'REQUEST_FINGERPRINTER_IMPLEMENTATION': '2.7',
-        'DOWNLOAD_TIMEOUT': 300,
+        'DOWNLOAD_TIMEOUT': 1200,
         'DOWNLOADER_MIDDLEWARES': {
             'scrapy.downloadermiddlewares.useragent.UserAgentMiddleware': None,
             'scrapy_user_agents.middlewares.RandomUserAgentMiddleware': 400,
         },
         'RANDOM_UA_TYPE': "random",
         'RETRY_ENABLED': True,
         'RETRY_TIMES': 5,
```

### Comparing `NewsArticlesScraper-0.2.7.1/NewsArticlesScraper/Scrapers.py` & `NewsArticlesScraper-0.2.7.2/NewsArticlesScraper/Scrapers.py`

 * *Files identical despite different names*

### Comparing `NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/PKG-INFO` & `NewsArticlesScraper-0.2.7.2/NewsArticlesScraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.7.1
+Version: 0.2.7.2
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.7.1/PKG-INFO` & `NewsArticlesScraper-0.2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.7.1
+Version: 0.2.7.2
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.7.1/setup.py` & `NewsArticlesScraper-0.2.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.7.1'
+VERSION = '0.2.7.2'
 DESCRIPTION = 'Scraping news articles'
 LONG_DESCRIPTION = 'A package that allows you to scrape news articles from various news sites via scrapy.'
 
 # Setting up
 setup(
     name="NewsArticlesScraper",
     version=VERSION,
```

