# Comparing `tmp/NewsArticlesScraper-0.2.7.3.tar.gz` & `tmp/NewsArticlesScraper-0.2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\NewsArticlesScraper-0.2.7.3.tar", last modified: Tue Aug  1 11:11:45 2023, max compression
+gzip compressed data, was "dist\NewsArticlesScraper-0.2.7.4.tar", last modified: Tue Aug  1 14:15:54 2023, max compression
```

## Comparing `NewsArticlesScraper-0.2.7.3.tar` & `NewsArticlesScraper-0.2.7.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 11:11:45.860225 NewsArticlesScraper-0.2.7.3/
-drwxrwxrwx   0        0        0        0 2023-08-01 11:11:45.839295 NewsArticlesScraper-0.2.7.3/NewsArticlesScraper/
--rw-rw-rw-   0        0        0    11273 2023-08-01 11:10:39.000000 NewsArticlesScraper-0.2.7.3/NewsArticlesScraper/ArticleUrlSrapers.py
--rw-rw-rw-   0        0        0    14676 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.3/NewsArticlesScraper/Scrapers.py
--rw-rw-rw-   0        0        0       64 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.3/NewsArticlesScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 11:11:45.858254 NewsArticlesScraper-0.2.7.3/NewsArticlesScraper.egg-info/
--rw-rw-rw-   0        0        0      650 2023-08-01 11:11:45.000000 NewsArticlesScraper-0.2.7.3/NewsArticlesScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-08-01 11:11:45.000000 NewsArticlesScraper-0.2.7.3/NewsArticlesScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 11:11:45.000000 NewsArticlesScraper-0.2.7.3/NewsArticlesScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-08-01 11:11:45.000000 NewsArticlesScraper-0.2.7.3/NewsArticlesScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-08-01 11:11:45.000000 NewsArticlesScraper-0.2.7.3/NewsArticlesScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      650 2023-08-01 11:11:45.859228 NewsArticlesScraper-0.2.7.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.3/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 11:11:45.861221 NewsArticlesScraper-0.2.7.3/setup.cfg
--rw-rw-rw-   0        0        0      998 2023-08-01 11:11:14.000000 NewsArticlesScraper-0.2.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:15:54.706276 NewsArticlesScraper-0.2.7.4/
+drwxrwxrwx   0        0        0        0 2023-08-01 14:15:54.686497 NewsArticlesScraper-0.2.7.4/NewsArticlesScraper/
+-rw-rw-rw-   0        0        0    11274 2023-08-01 14:14:34.000000 NewsArticlesScraper-0.2.7.4/NewsArticlesScraper/ArticleUrlSrapers.py
+-rw-rw-rw-   0        0        0    14676 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.4/NewsArticlesScraper/Scrapers.py
+-rw-rw-rw-   0        0        0       64 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.4/NewsArticlesScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:15:54.704343 NewsArticlesScraper-0.2.7.4/NewsArticlesScraper.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-08-01 14:15:54.000000 NewsArticlesScraper-0.2.7.4/NewsArticlesScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-08-01 14:15:54.000000 NewsArticlesScraper-0.2.7.4/NewsArticlesScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 14:15:54.000000 NewsArticlesScraper-0.2.7.4/NewsArticlesScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-01 14:15:54.000000 NewsArticlesScraper-0.2.7.4/NewsArticlesScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-01 14:15:54.000000 NewsArticlesScraper-0.2.7.4/NewsArticlesScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      650 2023-08-01 14:15:54.705281 NewsArticlesScraper-0.2.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 14:15:54.706276 NewsArticlesScraper-0.2.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      998 2023-08-01 14:15:35.000000 NewsArticlesScraper-0.2.7.4/setup.py
```

### Comparing `NewsArticlesScraper-0.2.7.3/NewsArticlesScraper/ArticleUrlSrapers.py` & `NewsArticlesScraper-0.2.7.4/NewsArticlesScraper/ArticleUrlSrapers.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         'DOWNLOAD_TIMEOUT': 1200,
         'DOWNLOADER_MIDDLEWARES': {
             'scrapy.downloadermiddlewares.useragent.UserAgentMiddleware': None,
             'scrapy_user_agents.middlewares.RandomUserAgentMiddleware': 400,
         },
         'RANDOM_UA_TYPE': "random",
         'RETRY_ENABLED': True,
-        'RETRY_TIMES': 5,
+        'RETRY_TIMES': 10,
     }
 
     def __init__(self, from_time: datetime.datetime, until_time: datetime.datetime, api_key, user_agent=None,
                  subsections_to_include: list = None, **kwargs):
         self.api_key = api_key
         self.from_time = from_time
         self.until_time = until_time
```

### Comparing `NewsArticlesScraper-0.2.7.3/NewsArticlesScraper/Scrapers.py` & `NewsArticlesScraper-0.2.7.4/NewsArticlesScraper/Scrapers.py`

 * *Files identical despite different names*

### Comparing `NewsArticlesScraper-0.2.7.3/NewsArticlesScraper.egg-info/PKG-INFO` & `NewsArticlesScraper-0.2.7.4/NewsArticlesScraper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.7.3
+Version: 0.2.7.4
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.7.3/PKG-INFO` & `NewsArticlesScraper-0.2.7.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.7.3
+Version: 0.2.7.4
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.7.3/setup.py` & `NewsArticlesScraper-0.2.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.7.3'
+VERSION = '0.2.7.4'
 DESCRIPTION = 'Scraping news articles'
 LONG_DESCRIPTION = 'A package that allows you to scrape news articles from various news sites via scrapy.'
 
 # Setting up
 setup(
     name="NewsArticlesScraper",
     version=VERSION,
```

