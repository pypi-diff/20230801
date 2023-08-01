# Comparing `tmp/creepypasta-0.0.3.tar.gz` & `tmp/creepypasta-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creepypasta-0.0.3.tar", last modified: Mon Jul 31 04:41:58 2023, max compression
+gzip compressed data, was "creepypasta-0.0.4.tar", last modified: Tue Aug  1 11:41:05 2023, max compression
```

## Comparing `creepypasta-0.0.3.tar` & `creepypasta-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:41:58.554147 creepypasta-0.0.3/
--rw-r--r--   0 sandrews   (501) staff       (20)      661 2023-07-31 04:41:58.554192 creepypasta-0.0.3/PKG-INFO
--rw-r--r--   0 sandrews   (501) staff       (20)       66 2023-07-31 03:53:30.000000 creepypasta-0.0.3/README.md
--rw-r--r--   0 sandrews   (501) staff       (20)      898 2023-07-31 04:41:43.000000 creepypasta-0.0.3/pyproject.toml
--rw-r--r--   0 sandrews   (501) staff       (20)      918 2023-07-31 04:41:58.554454 creepypasta-0.0.3/setup.cfg
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:41:58.552567 creepypasta-0.0.3/src/
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:41:58.553324 creepypasta-0.0.3/src/creepypasta/
--rw-r--r--   0 sandrews   (501) staff       (20)       59 2023-07-31 04:40:38.000000 creepypasta-0.0.3/src/creepypasta/__init__.py
--rw-r--r--   0 sandrews   (501) staff       (20)     8825 2023-07-28 13:46:50.000000 creepypasta-0.0.3/src/creepypasta/pasta_listings.py
--rw-r--r--   0 sandrews   (501) staff       (20)    16890 2023-07-28 13:46:50.000000 creepypasta-0.0.3/src/creepypasta/pasta_stories.py
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:41:58.553937 creepypasta-0.0.3/src/creepypasta.egg-info/
--rw-r--r--   0 sandrews   (501) staff       (20)      661 2023-07-31 04:41:58.000000 creepypasta-0.0.3/src/creepypasta.egg-info/PKG-INFO
--rw-r--r--   0 sandrews   (501) staff       (20)      342 2023-07-31 04:41:58.000000 creepypasta-0.0.3/src/creepypasta.egg-info/SOURCES.txt
--rw-r--r--   0 sandrews   (501) staff       (20)        1 2023-07-31 04:41:58.000000 creepypasta-0.0.3/src/creepypasta.egg-info/dependency_links.txt
--rw-r--r--   0 sandrews   (501) staff       (20)      181 2023-07-31 04:41:58.000000 creepypasta-0.0.3/src/creepypasta.egg-info/requires.txt
--rw-r--r--   0 sandrews   (501) staff       (20)       12 2023-07-31 04:41:58.000000 creepypasta-0.0.3/src/creepypasta.egg-info/top_level.txt
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-07-31 04:41:58.554053 creepypasta-0.0.3/test/
--rw-r--r--   0 sandrews   (501) staff       (20)     2453 2023-07-28 13:51:00.000000 creepypasta-0.0.3/test/test-units.py
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 11:41:05.328323 creepypasta-0.0.4/
+-rw-r--r--   0 sandrews   (501) staff       (20)      661 2023-08-01 11:41:05.328385 creepypasta-0.0.4/PKG-INFO
+-rw-r--r--   0 sandrews   (501) staff       (20)       66 2023-07-31 03:53:30.000000 creepypasta-0.0.4/README.md
+-rw-r--r--   0 sandrews   (501) staff       (20)      898 2023-08-01 10:26:33.000000 creepypasta-0.0.4/pyproject.toml
+-rw-r--r--   0 sandrews   (501) staff       (20)      918 2023-08-01 11:41:05.328646 creepypasta-0.0.4/setup.cfg
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 11:41:05.325790 creepypasta-0.0.4/src/
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 11:41:05.327154 creepypasta-0.0.4/src/creepypasta/
+-rw-r--r--   0 sandrews   (501) staff       (20)       59 2023-07-31 04:40:38.000000 creepypasta-0.0.4/src/creepypasta/__init__.py
+-rw-r--r--   0 sandrews   (501) staff       (20)     8825 2023-07-28 13:46:50.000000 creepypasta-0.0.4/src/creepypasta/pasta_listings.py
+-rw-r--r--   0 sandrews   (501) staff       (20)    17564 2023-08-01 11:34:15.000000 creepypasta-0.0.4/src/creepypasta/pasta_stories.py
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 11:41:05.327989 creepypasta-0.0.4/src/creepypasta.egg-info/
+-rw-r--r--   0 sandrews   (501) staff       (20)      661 2023-08-01 11:41:05.000000 creepypasta-0.0.4/src/creepypasta.egg-info/PKG-INFO
+-rw-r--r--   0 sandrews   (501) staff       (20)      342 2023-08-01 11:41:05.000000 creepypasta-0.0.4/src/creepypasta.egg-info/SOURCES.txt
+-rw-r--r--   0 sandrews   (501) staff       (20)        1 2023-08-01 11:41:05.000000 creepypasta-0.0.4/src/creepypasta.egg-info/dependency_links.txt
+-rw-r--r--   0 sandrews   (501) staff       (20)      181 2023-08-01 11:41:05.000000 creepypasta-0.0.4/src/creepypasta.egg-info/requires.txt
+-rw-r--r--   0 sandrews   (501) staff       (20)       12 2023-08-01 11:41:05.000000 creepypasta-0.0.4/src/creepypasta.egg-info/top_level.txt
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 11:41:05.328106 creepypasta-0.0.4/test/
+-rw-r--r--   0 sandrews   (501) staff       (20)     2453 2023-07-28 13:51:00.000000 creepypasta-0.0.4/test/test-units.py
```

### Comparing `creepypasta-0.0.3/PKG-INFO` & `creepypasta-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creepypasta
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small package to crawl CreepyPasta and parse into structured data.
 Home-page: https://jellomoat.github.io/pasta/
 Author: Stephanie Andrews
 Author-email: Stephanie Andrews <jellomoat@gmail.com>
 Project-URL: Homepage, https://github.com/jellomoat/pasta
 Project-URL: Bug Tracker, https://github.com/jellomoat/pasta/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `creepypasta-0.0.3/pyproject.toml` & `creepypasta-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = [
     "setuptools>=61.0",
     "beautifulsoup4>=4.12.2",
-    "lxml==4.9.3",
+    "lxml>=4.9.3",
     "requests==2.31.0",
     "pandas==2.0.3",
     "pathlib==1.0.1",
-    "chromedriver-binary-auto==0.2.6",
+    "chromedriver-binary-auto>=0.2.6",
     "selenium==4.10.0",
     "selenium-wire==5.1.0",
     "tqdm==4.65.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "creepypasta"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Stephanie Andrews", email="jellomoat@gmail.com" },
 ]
 description = "A small package to crawl CreepyPasta and parse into structured data."
 
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `creepypasta-0.0.3/setup.cfg` & `creepypasta-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `creepypasta-0.0.3/src/creepypasta/pasta_listings.py` & `creepypasta-0.0.4/src/creepypasta/pasta_listings.py`

 * *Files identical despite different names*

### Comparing `creepypasta-0.0.3/src/creepypasta/pasta_stories.py` & `creepypasta-0.0.4/src/creepypasta/pasta_stories.py`

 * *Files 3% similar despite different names*

```diff
@@ -420,14 +420,31 @@
 
 def format_stories_df(df):
     df["story_rating"] = df["story_rating"].apply(lambda x: float(x))
     df["reading_time_min"] = df["reading_time_min"].apply(lambda x: float(x))
     # TODO: swap to use entry-title for title instead?
     df["cleaned_title"] = df["title"].apply(lambda x: re.sub(r"\ *-\ *Creepypasta", "", x))
 
+# TODO: integrate into csv export
+def get_all_tags_list():
+    categories_page = PageFetcherUtils.fetch_page(
+        "https://www.creepypasta.com/archive/sorted-by-category/")
+    soup = BeautifulSoup(resp.text)
+    return [cat["value"] for cat in soup.findAll(
+        "select", {"name" : "tx_category"})[0].select("option")][1:]
+
+def get_df_with_expanded_story_cats_cols(df):
+    cat_tag_links = get_all_tags_list()
+    story_cats_df = df["story_cats"].apply(
+        lambda story_cats: pd.Series(
+            [cat in story_cats for cat in cat_tag_links], 
+            index=cat_tag_links)).add_prefix("cat__")
+    return pd.concat(
+        [df, story_cats_df], axis=1)
+
 
 if __name__ == "__main__":
     # Get/fetch and parse stories    
     stories_dict_list = get_stories_from_listings_dirpath("./list-pages/")
     # Load into dataframe for analysis
     stories_df = pd.DataFrame(stories_dict_list)
     # Write to disk
```

### Comparing `creepypasta-0.0.3/src/creepypasta.egg-info/PKG-INFO` & `creepypasta-0.0.4/src/creepypasta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creepypasta
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small package to crawl CreepyPasta and parse into structured data.
 Home-page: https://jellomoat.github.io/pasta/
 Author: Stephanie Andrews
 Author-email: Stephanie Andrews <jellomoat@gmail.com>
 Project-URL: Homepage, https://github.com/jellomoat/pasta
 Project-URL: Bug Tracker, https://github.com/jellomoat/pasta/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `creepypasta-0.0.3/test/test-units.py` & `creepypasta-0.0.4/test/test-units.py`

 * *Files identical despite different names*

