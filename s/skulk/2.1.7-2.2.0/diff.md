# Comparing `tmp/skulk-2.1.7-py2.py3-none-any.whl.zip` & `tmp/skulk-2.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 11358 bytes, number of entries: 12
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-17 03:54 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-17 03:54 skulk/__init__.py
--rw-r--r--  2.0 unx    10725 b- defN 23-Jun-17 03:54 skulk/bumper.py
--rw-r--r--  2.0 unx     2294 b- defN 23-Jun-17 03:54 skulk/questions.py
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-17 03:54 skulk/questions_fallback.py
--rw-r--r--  2.0 unx    10237 b- defN 23-Jun-17 03:54 skulk/skulk.py
--rw-r--r--  2.0 unx     3490 b- defN 23-Jun-17 03:54 skulk/util.py
--rw-r--r--  2.0 unx      675 b- defN 23-Jun-17 03:54 skulk-2.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-17 03:54 skulk-2.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 23-Jun-17 03:54 skulk-2.1.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-17 03:54 skulk-2.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      894 b- defN 23-Jun-17 03:54 skulk-2.1.7.dist-info/RECORD
-12 files, 31080 bytes uncompressed, 9874 bytes compressed:  68.2%
+Zip file size: 12142 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        5 b- defN 23-Aug-01 04:05 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 04:05 skulk/__init__.py
+-rw-r--r--  2.0 unx    10675 b- defN 23-Aug-01 04:05 skulk/bumper.py
+-rw-r--r--  2.0 unx     2294 b- defN 23-Aug-01 04:05 skulk/questions.py
+-rw-r--r--  2.0 unx     2601 b- defN 23-Aug-01 04:05 skulk/questions_fallback.py
+-rw-r--r--  2.0 unx    10237 b- defN 23-Aug-01 04:05 skulk/skulk.py
+-rw-r--r--  2.0 unx     1689 b- defN 23-Aug-01 04:05 skulk/skulk_parse.py
+-rw-r--r--  2.0 unx     3490 b- defN 23-Aug-01 04:05 skulk/util.py
+-rw-r--r--  2.0 unx      696 b- defN 23-Aug-01 04:05 skulk-2.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Aug-01 04:05 skulk-2.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       80 b- defN 23-Aug-01 04:05 skulk-2.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Aug-01 04:05 skulk-2.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      971 b- defN 23-Aug-01 04:05 skulk-2.2.0.dist-info/RECORD
+13 files, 32854 bytes uncompressed, 10542 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -12,26 +12,29 @@
 
 Filename: skulk/questions_fallback.py
 Comment: 
 
 Filename: skulk/skulk.py
 Comment: 
 
+Filename: skulk/skulk_parse.py
+Comment: 
+
 Filename: skulk/util.py
 Comment: 
 
-Filename: skulk-2.1.7.dist-info/METADATA
+Filename: skulk-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: skulk-2.1.7.dist-info/WHEEL
+Filename: skulk-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-2.1.7.dist-info/entry_points.txt
+Filename: skulk-2.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-2.1.7.dist-info/top_level.txt
+Filename: skulk-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-2.1.7.dist-info/RECORD
+Filename: skulk-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-2.1.7
+2.2.0
```

## skulk/bumper.py

```diff
@@ -90,17 +90,17 @@
         if release_scope == RELEASE_SCOPE_BETA:
             sources = ["test", "pypi", "tags"]
         else:
             sources = ["pypi", "tags"]
         token = RELEASE_TOKENS[release_scope]
         reference_version = self.latest_version(*sources)
         result = get_version_options(reference_version, token=token)
-        for i, v in enumerate(["patch", "minor", "major"]):
+        for i in range(len(result)):
             result[i] = {
-                "label": f"{result[i]} : {VERSION_POLICY[v]}",
+                "label": result[i],
                 "value": result[i],
             }
 
         return result
 
     def versions_table(self, max_versions=10):
         """Return a table of versions where the columns are the sources, and the rows are the versions."""
```

## Comparing `skulk-2.1.7.dist-info/METADATA` & `skulk-2.2.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 2.1.7
+Version: 2.2.0
 Summary: Streamline release for Conductor client tools and others
 Home-page: https://github.com/ConductorTechnologies/skulk
 Author: Julian Mann
 Author-email: julian@conductortech.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Requires-Dist: GitPython (<4.0.0,>=3.1.31)
 Requires-Dist: semver (<4.0.0,>=3.0.0)
 Requires-Dist: twine (>=4.0.2)
 Requires-Dist: future (>=0.18.3)
 Requires-Dist: bullet (>=2.2.0)
 Requires-Dist: tabulate (>=0.9.0)
+Requires-Dist: Click
 
 Streamline release for Conductor client tools and others
```

## Comparing `skulk-2.1.7.dist-info/RECORD` & `skulk-2.2.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-skulk/VERSION,sha256=UWlFItN7l7WK9wepGFQZFCnWjnLxT6VWRF2wqSNBq3U,5
+skulk/VERSION,sha256=7cjjlaUYLjsjGBbhkbMDQH1RH3DB2cttUyknzFWcUHw,5
 skulk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-skulk/bumper.py,sha256=BCJZNjh73oXR2p6BkLRPiU802TG03iyzRhBgMI91hew,10725
+skulk/bumper.py,sha256=rC54qBhGXZB6f544-If2HZQNPOAmkOpg3APgZLlGD_c,10675
 skulk/questions.py,sha256=ihDx7B1JNw4wQnwjox6BRHpDUM_VzTajmf867IugP-U,2294
 skulk/questions_fallback.py,sha256=aQrtgxnHr6VUlJHO4OcVvPbzJj5V8U2OwXyJ4hBwHi8,2601
 skulk/skulk.py,sha256=OfT4HjKv_1PhjNW2RRs--P6D2GUULrcFXptpQdgjDoY,10237
+skulk/skulk_parse.py,sha256=WS67aXcKd5T4ZM-Yehzl-anT0vYIsqn7V71NChBn61I,1689
 skulk/util.py,sha256=qoiXmwPmAndSc-NJ7I8LUsyeM3XzdE4_R4IqHufLw_c,3490
-skulk-2.1.7.dist-info/METADATA,sha256=nWKqd_2rAjPpjNulefQjVQTLAz7juSVabR9OweBT9uo,675
-skulk-2.1.7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-skulk-2.1.7.dist-info/entry_points.txt,sha256=8DGRFZ3C46ZQBYFsfNj4eYw5ZGq8NWW8uKe-2xC-c34,43
-skulk-2.1.7.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
-skulk-2.1.7.dist-info/RECORD,,
+skulk-2.2.0.dist-info/METADATA,sha256=dqskOX5rOg-jgWT6czzA-Xx2OWq42-K3wihhFrcelmI,696
+skulk-2.2.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+skulk-2.2.0.dist-info/entry_points.txt,sha256=wnBg1z2ixnIcAD1KxsdoYgw-XlaCZmKZmjBU3kgp094,80
+skulk-2.2.0.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
+skulk-2.2.0.dist-info/RECORD,,
```

