# Comparing `tmp/asmek_authcogs-1.0.4.tar.gz` & `tmp/asmek_authcogs-1.1.1.tar.gz`

## Comparing `asmek_authcogs-1.0.4.tar` & `asmek_authcogs-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/CHANGELOG.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/__init__.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/app_settings.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/apps.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/auth_hooks.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/Images/__init__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/Images/eve-o-4.png
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/Images/smt_bomb_icon-1.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/cogs/__init__.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/cogs/about.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/cogs/auth.py
--rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/cogs/links.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/migrations/0001_initial.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/migrations/0002_alter_link_name.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/migrations/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/LICENSE
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/README.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/__init__.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/app_settings.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/apps.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/auth_hooks.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/Images/__init__.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/Images/eve-o-4.png
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/Images/smt_bomb_icon-1.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/cogs/__init__.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/cogs/about.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/cogs/auth.py
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/cogs/links.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/cogs/siege.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/migrations/0001_initial.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/migrations/0002_alter_link_name.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/migrations/0003_alter_general_options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/migrations/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/PKG-INFO
```

### Comparing `asmek_authcogs-1.0.4/CHANGELOG.md` & `asmek_authcogs-1.1.1/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 ## [In Development] - Unreleased
 
 ### Added
 
+## [1.1.1] - 2023-07-31
+
+### Added
+
+-siege command
+    updates in alert image in a specific channel
+
 ## [1.0.0] - 2023-07-04
 
 ### Added
 
 -about command: basic command about auth bot
 -auth command:
     -home
```

### Comparing `asmek_authcogs-1.0.4/.github/workflows/publish.yml` & `asmek_authcogs-1.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.4/asmek_authcogs/models.py` & `asmek_authcogs-1.1.1/asmek_authcogs/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """Meta model for app permissions"""
 
     class Meta:
         """Meta definitions"""
 
         managed = False
         default_permissions = ()
-        permissions = (("basic_access", "Basic access to this app"),)
+        permissions = (("basic_access", "Basic access to this app"),("siege_control", "Control siege colours"),)
 
 
 class Link(models.Model):
     description = models.TextField(max_length=500)
     name = models.CharField(max_length=255, null=False, unique=True)
     url = models.CharField(max_length=255, null=False)
     thumbnail = models.CharField(max_length=255)
```

### Comparing `asmek_authcogs-1.0.4/asmek_authcogs/Images/eve-o-4.png` & `asmek_authcogs-1.1.1/asmek_authcogs/Images/eve-o-4.png`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.4/asmek_authcogs/Images/smt_bomb_icon-1.png` & `asmek_authcogs-1.1.1/asmek_authcogs/Images/smt_bomb_icon-1.png`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.4/asmek_authcogs/cogs/about.py` & `asmek_authcogs-1.1.1/asmek_authcogs/cogs/about.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.4/asmek_authcogs/cogs/auth.py` & `asmek_authcogs-1.1.1/asmek_authcogs/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.4/asmek_authcogs/cogs/links.py` & `asmek_authcogs-1.1.1/asmek_authcogs/cogs/links.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.4/asmek_authcogs/migrations/0001_initial.py` & `asmek_authcogs-1.1.1/asmek_authcogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.4/.gitignore` & `asmek_authcogs-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.4/LICENSE` & `asmek_authcogs-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.4/README.md` & `asmek_authcogs-1.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -24,13 +24,15 @@
 ## Settings
 
 Setting | Default | Description
 --- | --- | ---
 `ASMEK_ALLIANCE_ID` |  | alliance id
 `ASMEK_ALLIANCE_NAME` |  | alliance name to display on embeds
 `ASMEK_ALLIANCE_URL` |  | URL for alliances auth system
+`ASMEK_SIEGE_CHANNEL` |  | channel id for siege alerts
 
 ## Permissions
 
 Perm | Description
 --- | ---
  link.manage_links | Can manage links in the links cog
+ general.siege_control | Can use siege commands
```

### Comparing `asmek_authcogs-1.0.4/pyproject.toml` & `asmek_authcogs-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.4/PKG-INFO` & `asmek_authcogs-1.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asmek-authcogs
-Version: 1.0.4
+Version: 1.1.1
 Summary: ASMEK customized cogs for aa-discordbot
 Project-URL: Documentation, https://github.com/AstrumMechanica/asmek-authcogs#readme
 Project-URL: Issues, https://github.com/AstrumMechanica/asmek-authcogs/issues
 Project-URL: Source, https://github.com/AstrumMechanica/asmek-authcogs
 Author-email: AstrumMechanica <astrummechanica@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE
@@ -48,13 +48,15 @@
 ## Settings
 
 Setting | Default | Description
 --- | --- | ---
 `ASMEK_ALLIANCE_ID` |  | alliance id
 `ASMEK_ALLIANCE_NAME` |  | alliance name to display on embeds
 `ASMEK_ALLIANCE_URL` |  | URL for alliances auth system
+`ASMEK_SIEGE_CHANNEL` |  | channel id for siege alerts
 
 ## Permissions
 
 Perm | Description
 --- | ---
  link.manage_links | Can manage links in the links cog
+ general.siege_control | Can use siege commands
```

