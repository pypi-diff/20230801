# Comparing `tmp/bkapi-plugins-py-0.731.tar.gz` & `tmp/bkapi-plugins-py-0.801.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkapi-plugins-py-0.731.tar", last modified: Mon Jul 31 01:59:04 2023, max compression
+gzip compressed data, was "bkapi-plugins-py-0.801.tar", last modified: Tue Aug  1 09:34:16 2023, max compression
```

## Comparing `bkapi-plugins-py-0.731.tar` & `bkapi-plugins-py-0.801.tar`

### file list

```diff
@@ -1,19 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 01:59:04.128327 bkapi-plugins-py-0.731/
--rw-rw-rw-   0        0        0       39 2023-07-27 00:30:58.000000 bkapi-plugins-py-0.731/MANIFEST.in
--rw-rw-rw-   0        0        0      187 2023-07-31 01:59:04.128327 bkapi-plugins-py-0.731/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-31 01:59:04.116687 bkapi-plugins-py-0.731/bkapi_plugins/
--rw-rw-rw-   0        0        0      172 2023-07-27 00:30:58.000000 bkapi-plugins-py-0.731/bkapi_plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 01:59:04.123328 bkapi-plugins-py-0.731/bkapi_plugins/files/
--rw-rw-rw-   0        0        0     3900 2023-07-31 01:46:13.000000 bkapi-plugins-py-0.731/bkapi_plugins/files/ali-Ubuntu.txt
--rw-rw-rw-   0        0        0     2932 2023-07-31 01:50:08.000000 bkapi-plugins-py-0.731/bkapi_plugins/files/ali-centos.txt
--rw-rw-rw-   0        0        0     1226 2023-07-31 01:54:59.000000 bkapi-plugins-py-0.731/bkapi_plugins/files/ali-epel
--rw-rw-rw-   0        0        0     1272 2023-07-31 01:53:55.000000 bkapi-plugins-py-0.731/bkapi_plugins/files/ali-k8s
--rw-rw-rw-   0        0        0      744 2023-07-31 01:51:43.000000 bkapi-plugins-py-0.731/bkapi_plugins/files/ali-pypi
--rw-rw-rw-   0        0        0     1792 2023-07-28 09:45:31.000000 bkapi-plugins-py-0.731/bkapi_plugins/files/centos8_base.repo
-drwxrwxrwx   0        0        0        0 2023-07-31 01:59:04.127327 bkapi-plugins-py-0.731/bkapi_plugins_py.egg-info/
--rw-rw-rw-   0        0        0      187 2023-07-31 01:59:04.000000 bkapi-plugins-py-0.731/bkapi_plugins_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-07-31 01:59:04.000000 bkapi-plugins-py-0.731/bkapi_plugins_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 01:59:04.000000 bkapi-plugins-py-0.731/bkapi_plugins_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-31 01:59:04.000000 bkapi-plugins-py-0.731/bkapi_plugins_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 01:59:04.129327 bkapi-plugins-py-0.731/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-07-31 01:47:22.000000 bkapi-plugins-py-0.731/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:34:16.606083 bkapi-plugins-py-0.801/
+-rw-rw-rw-   0        0        0       39 2023-07-27 00:30:58.000000 bkapi-plugins-py-0.801/MANIFEST.in
+-rw-rw-rw-   0        0        0      187 2023-08-01 09:34:16.607084 bkapi-plugins-py-0.801/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 09:34:16.585864 bkapi-plugins-py-0.801/bkapi_plugins/
+-rw-rw-rw-   0        0        0      172 2023-07-27 00:30:58.000000 bkapi-plugins-py-0.801/bkapi_plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:34:16.589858 bkapi-plugins-py-0.801/bkapi_plugins/files/
+-rw-rw-rw-   0        0        0      312 2023-08-01 09:34:13.000000 bkapi-plugins-py-0.801/bkapi_plugins/files/test
+drwxrwxrwx   0        0        0        0 2023-08-01 09:34:16.603080 bkapi-plugins-py-0.801/bkapi_plugins_py.egg-info/
+-rw-rw-rw-   0        0        0      187 2023-08-01 09:34:16.000000 bkapi-plugins-py-0.801/bkapi_plugins_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-08-01 09:34:16.000000 bkapi-plugins-py-0.801/bkapi_plugins_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:34:16.000000 bkapi-plugins-py-0.801/bkapi_plugins_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-08-01 09:34:16.000000 bkapi-plugins-py-0.801/bkapi_plugins_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 09:34:16.609083 bkapi-plugins-py-0.801/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-08-01 09:34:13.000000 bkapi-plugins-py-0.801/setup.py
```

### Comparing `bkapi-plugins-py-0.731/setup.py` & `bkapi-plugins-py-0.801/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = ''
 
 setup(
     description='',
     long_description=readme,
     name='bkapi-plugins-py', # 包的名字
-    version='0.731', # 版本号每次打包完要改一下
+    version='0.801', # 版本号每次打包完要改一下
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
     author='fadewalk',
     license='Apach License 2.0',
     # packages=find_packages(),
     # namespace_packages=['bkapi_plugins'],
     package_dir={'': '.'},
     include_package_data=True,
```

