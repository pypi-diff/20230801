# Comparing `tmp/plex-tvdb-alt-orderer-0.2.3.tar.gz` & `tmp/plex-tvdb-alt-orderer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-tvdb-alt-orderer-0.2.3.tar", last modified: Sun Jun 11 22:32:39 2023, max compression
+gzip compressed data, was "plex-tvdb-alt-orderer-0.2.4.tar", last modified: Tue Aug  1 21:54:21 2023, max compression
```

## Comparing `plex-tvdb-alt-orderer-0.2.3.tar` & `plex-tvdb-alt-orderer-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 22:32:39.129782 plex-tvdb-alt-orderer-0.2.3/
--rw-rw-rw-   0        0        0     1073 2023-06-07 23:45:38.000000 plex-tvdb-alt-orderer-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     5870 2023-06-11 22:32:39.128791 plex-tvdb-alt-orderer-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     5250 2023-06-09 21:39:05.000000 plex-tvdb-alt-orderer-0.2.3/README.md
--rw-rw-rw-   0        0        0      877 2023-06-11 20:47:36.000000 plex-tvdb-alt-orderer-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-11 22:32:39.129782 plex-tvdb-alt-orderer-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-11 22:32:39.084179 plex-tvdb-alt-orderer-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 22:32:39.105180 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer/
--rw-rw-rw-   0        0        0     7869 2023-06-11 22:20:51.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer/main.py
-drwxrwxrwx   0        0        0        0 2023-06-11 22:32:39.126783 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/
--rw-rw-rw-   0        0        0     5870 2023-06-11 22:32:39.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-06-11 22:32:39.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 22:32:39.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-11 22:32:39.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2023-06-11 22:32:39.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-11 22:32:39.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 21:54:21.463419 plex-tvdb-alt-orderer-0.2.4/
+-rw-rw-rw-   0        0        0     1073 2023-06-07 23:45:38.000000 plex-tvdb-alt-orderer-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     5870 2023-08-01 21:54:21.462419 plex-tvdb-alt-orderer-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5250 2023-06-09 21:39:05.000000 plex-tvdb-alt-orderer-0.2.4/README.md
+-rw-rw-rw-   0        0        0      877 2023-08-01 21:35:50.000000 plex-tvdb-alt-orderer-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 21:54:21.464419 plex-tvdb-alt-orderer-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 21:54:21.434418 plex-tvdb-alt-orderer-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 21:54:21.443419 plex-tvdb-alt-orderer-0.2.4/src/plex_tvdb_alt_orderer/
+-rw-rw-rw-   0        0        0     8231 2023-08-01 21:39:21.000000 plex-tvdb-alt-orderer-0.2.4/src/plex_tvdb_alt_orderer/main.py
+drwxrwxrwx   0        0        0        0 2023-08-01 21:54:21.461418 plex-tvdb-alt-orderer-0.2.4/src/plex_tvdb_alt_orderer.egg-info/
+-rw-rw-rw-   0        0        0     5870 2023-08-01 21:54:21.000000 plex-tvdb-alt-orderer-0.2.4/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-08-01 21:54:21.000000 plex-tvdb-alt-orderer-0.2.4/src/plex_tvdb_alt_orderer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 21:54:21.000000 plex-tvdb-alt-orderer-0.2.4/src/plex_tvdb_alt_orderer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-08-01 21:54:21.000000 plex-tvdb-alt-orderer-0.2.4/src/plex_tvdb_alt_orderer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       70 2023-08-01 21:54:21.000000 plex-tvdb-alt-orderer-0.2.4/src/plex_tvdb_alt_orderer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-01 21:54:21.000000 plex-tvdb-alt-orderer-0.2.4/src/plex_tvdb_alt_orderer.egg-info/top_level.txt
```

### Comparing `plex-tvdb-alt-orderer-0.2.3/LICENSE` & `plex-tvdb-alt-orderer-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plex-tvdb-alt-orderer-0.2.3/PKG-INFO` & `plex-tvdb-alt-orderer-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-tvdb-alt-orderer
-Version: 0.2.3
+Version: 0.2.4
 Summary: A utility that applies alternate TVDB orders to Plex.
 Author: bpoxy
 Project-URL: Homepage, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Project-URL: Bug Tracker, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `plex-tvdb-alt-orderer-0.2.3/README.md` & `plex-tvdb-alt-orderer-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `plex-tvdb-alt-orderer-0.2.3/pyproject.toml` & `plex-tvdb-alt-orderer-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "plex-tvdb-alt-orderer"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="bpoxy" },
 ]
 description = "A utility that applies alternate TVDB orders to Plex."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["click", "inquirer", "plexapi", "progress", "termcolor", "tvdb_v4_official", "validators"]
```

### Comparing `plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer/main.py` & `plex-tvdb-alt-orderer-0.2.4/src/plex_tvdb_alt_orderer/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     plex_show = get_plex_show(plex_section, plex_show_name)
     plex_episodes = plex_show.episodes()
     
     tvdb_pin = text_prompt_if_unspecified(tvdb_pin, "your TVDB subscriber PIN")
     tvdb = TVDB(apikey="5f119e31-f9c5-4f0c-b1c3-064b3225e7d9", pin=tvdb_pin)
     tvdb_id = next(match.group("id") for match in [re.match(r"tvdb://(?P<id>\d+)", guid.id) for guid in plex_show.guids] if match)
     tvdb_season_type = get_tvdb_season_type(tvdb, tvdb_id, tvdb_order_name)
-    tvdb_episodes = tvdb.get_series_episodes(tvdb_id, season_type=tvdb_season_type, lang="eng")["episodes"]
+    tvdb_episodes = get_tvdb_episodes(tvdb, tvdb_id, tvdb_season_type)
     
     update_plex(season, plex_episodes, tvdb_episodes)
 
 def dict_prompt(dict: dict, description: str):
     return dict[inquirer.prompt([inquirer.List("answer", message=f"Select {description}", choices=dict.keys())])["answer"]]
 
 def error_exit(text: str):
@@ -85,14 +85,29 @@
     if len(shows) == 0:
          error_exit(f"Your TV show library doesn't contain a show with name '{show_name}'.")
     elif len(shows) == 1:
         return shows[0]
     else:
         return dict_prompt({s.title: s for s in shows}, "the show to update")
 
+def get_tvdb_episodes(tvdb: TVDB, tvdb_id: int, tvdb_season_type: str) -> list[dict]:
+    episodes = []
+    page = 0
+
+    while True:
+        data = tvdb.get_series_episodes(tvdb_id, season_type=tvdb_season_type, page=page, lang="eng")
+
+        if not len(data["episodes"]):
+            break
+
+        episodes.extend(data["episodes"])
+        page += 1
+        
+    return episodes
+
 def get_tvdb_season_type(tvdb: TVDB, tvdb_id: int, order_name: str) -> str:
     season_types = tvdb.get_season_types(tvdb_id)
     season_types_dict = {s["name"]: s["type"] for s in season_types}
 
     if order_name:
         return season_types_dict.get(order_name, None) or error_exit(f"TVDB doesn't define an order with name '{order_name}'.")
```

### Comparing `plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO` & `plex-tvdb-alt-orderer-0.2.4/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-tvdb-alt-orderer
-Version: 0.2.3
+Version: 0.2.4
 Summary: A utility that applies alternate TVDB orders to Plex.
 Author: bpoxy
 Project-URL: Homepage, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Project-URL: Bug Tracker, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

