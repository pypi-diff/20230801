# Comparing `tmp/goconfigure-0.1.3.tar.gz` & `tmp/goconfigure-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goconfigure-0.1.3.tar", last modified: Tue Aug  1 21:25:44 2023, max compression
+gzip compressed data, was "goconfigure-0.1.4.tar", last modified: Tue Aug  1 21:37:12 2023, max compression
```

## Comparing `goconfigure-0.1.3.tar` & `goconfigure-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 lewis     (1000) lewis     (1000)        0 2023-08-01 21:25:44.108257 goconfigure-0.1.3/
-drwxr-xr-x   0 lewis     (1000) lewis     (1000)        0 2023-08-01 21:25:44.108257 goconfigure-0.1.3/GoConf/
--rw-r--r--   0 lewis     (1000) lewis     (1000)       37 2023-08-01 21:10:12.000000 goconfigure-0.1.3/GoConf/__init__.py
--rw-r--r--   0 lewis     (1000) lewis     (1000)     3805 2023-08-01 21:10:54.000000 goconfigure-0.1.3/GoConf/goconfigure.py
--rw-r--r--   0 lewis     (1000) lewis     (1000)      248 2023-08-01 21:25:44.108257 goconfigure-0.1.3/PKG-INFO
-drwxr-xr-x   0 lewis     (1000) lewis     (1000)        0 2023-08-01 21:25:44.108257 goconfigure-0.1.3/goconfigure.egg-info/
--rw-r--r--   0 lewis     (1000) lewis     (1000)      248 2023-08-01 21:25:44.000000 goconfigure-0.1.3/goconfigure.egg-info/PKG-INFO
--rw-r--r--   0 lewis     (1000) lewis     (1000)      189 2023-08-01 21:25:44.000000 goconfigure-0.1.3/goconfigure.egg-info/SOURCES.txt
--rw-r--r--   0 lewis     (1000) lewis     (1000)        1 2023-08-01 21:25:44.000000 goconfigure-0.1.3/goconfigure.egg-info/dependency_links.txt
--rw-r--r--   0 lewis     (1000) lewis     (1000)        7 2023-08-01 21:25:44.000000 goconfigure-0.1.3/goconfigure.egg-info/top_level.txt
--rw-r--r--   0 lewis     (1000) lewis     (1000)       38 2023-08-01 21:25:44.108257 goconfigure-0.1.3/setup.cfg
--rw-r--r--   0 lewis     (1000) lewis     (1000)      332 2023-08-01 21:25:24.000000 goconfigure-0.1.3/setup.py
+drwxr-xr-x   0 lewis     (1000) lewis     (1000)        0 2023-08-01 21:37:12.623097 goconfigure-0.1.4/
+drwxr-xr-x   0 lewis     (1000) lewis     (1000)        0 2023-08-01 21:37:12.619763 goconfigure-0.1.4/GoConf/
+-rw-r--r--   0 lewis     (1000) lewis     (1000)       37 2023-08-01 21:10:12.000000 goconfigure-0.1.4/GoConf/__init__.py
+-rw-r--r--   0 lewis     (1000) lewis     (1000)     3804 2023-08-01 21:36:40.000000 goconfigure-0.1.4/GoConf/goconfigure.py
+-rw-r--r--   0 lewis     (1000) lewis     (1000)      248 2023-08-01 21:37:12.623097 goconfigure-0.1.4/PKG-INFO
+drwxr-xr-x   0 lewis     (1000) lewis     (1000)        0 2023-08-01 21:37:12.623097 goconfigure-0.1.4/goconfigure.egg-info/
+-rw-r--r--   0 lewis     (1000) lewis     (1000)      248 2023-08-01 21:37:12.000000 goconfigure-0.1.4/goconfigure.egg-info/PKG-INFO
+-rw-r--r--   0 lewis     (1000) lewis     (1000)      189 2023-08-01 21:37:12.000000 goconfigure-0.1.4/goconfigure.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis     (1000) lewis     (1000)        1 2023-08-01 21:37:12.000000 goconfigure-0.1.4/goconfigure.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis     (1000) lewis     (1000)        7 2023-08-01 21:37:12.000000 goconfigure-0.1.4/goconfigure.egg-info/top_level.txt
+-rw-r--r--   0 lewis     (1000) lewis     (1000)       38 2023-08-01 21:37:12.623097 goconfigure-0.1.4/setup.cfg
+-rw-r--r--   0 lewis     (1000) lewis     (1000)      332 2023-08-01 21:36:29.000000 goconfigure-0.1.4/setup.py
```

### Comparing `goconfigure-0.1.3/GoConf/goconfigure.py` & `goconfigure-0.1.4/GoConf/goconfigure.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
         with open(self._fl, "r") as f:
             for line in f:
                 ln = line.strip()
                 # section
                 section = re.search('[[].*[]]', ln)
                 comment = re.search("[#].*", ln)
-                val = None if ln.count("=") == 0 else val
+                val = None if ln.count("=") == 0 else ln
                 if section:
                     current_section = section.group(0).replace("[", "").replace("]", "")
                     comment_no = 0
                     self._conf_dict[current_section] = {}
                 elif comment:
                     self._conf_dict[current_section][f"comment_{comment_no}"] = comment.group(0).replace("#",
                                                                                                          "").strip()
```

