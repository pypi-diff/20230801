# Comparing `tmp/dkist-service-configuration-1.0.0rc4.tar.gz` & `tmp/dkist-service-configuration-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-service-configuration-1.0.0rc4.tar", last modified: Thu Jul 27 19:47:27 2023, max compression
+gzip compressed data, was "dkist-service-configuration-1.0.1.tar", last modified: Mon Jul 31 22:47:00 2023, max compression
```

## Comparing `dkist-service-configuration-1.0.0rc4.tar` & `dkist-service-configuration-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-27 19:47:27.546760 dkist-service-configuration-1.0.0rc4/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-27 19:47:27.546760 dkist-service-configuration-1.0.0rc4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1394 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-27 19:47:27.546760 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-27 19:47:27.546760 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/tests/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/tests/test_settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-27 19:47:27.546760 dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-27 19:47:27.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-07-27 19:47:27.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-27 19:47:27.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-27 19:47:27.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-27 19:47:27.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-27 19:47:27.546760 dkist-service-configuration-1.0.0rc4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 22:47:00.058409 dkist-service-configuration-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-07-31 22:47:00.058409 dkist-service-configuration-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 22:47:00.058409 dkist-service-configuration-1.0.1/dkist_service_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/dkist_service_configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/dkist_service_configuration/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/dkist_service_configuration/settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 22:47:00.058409 dkist-service-configuration-1.0.1/dkist_service_configuration/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/dkist_service_configuration/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/dkist_service_configuration/tests/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/dkist_service_configuration/tests/test_settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 22:47:00.058409 dkist-service-configuration-1.0.1/dkist_service_configuration.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-07-31 22:47:00.000000 dkist-service-configuration-1.0.1/dkist_service_configuration.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-07-31 22:47:00.000000 dkist-service-configuration-1.0.1/dkist_service_configuration.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-31 22:47:00.000000 dkist-service-configuration-1.0.1/dkist_service_configuration.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-31 22:47:00.000000 dkist-service-configuration-1.0.1/dkist_service_configuration.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-31 22:47:00.000000 dkist-service-configuration-1.0.1/dkist_service_configuration.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-31 22:47:00.058409 dkist-service-configuration-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-31 22:46:45.000000 dkist-service-configuration-1.0.1/setup.py
```

### Comparing `dkist-service-configuration-1.0.0rc4/.gitignore` & `dkist-service-configuration-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc4/.pre-commit-config.yaml` & `dkist-service-configuration-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc4/LICENSE` & `dkist-service-configuration-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc4/bitbucket-pipelines.yml` & `dkist-service-configuration-1.0.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc4/dkist_service_configuration/logging.py` & `dkist-service-configuration-1.0.1/dkist_service_configuration/logging.py`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc4/dkist_service_configuration/settings.py` & `dkist-service-configuration-1.0.1/dkist_service_configuration/settings.py`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc4/dkist_service_configuration/tests/test_settings.py` & `dkist-service-configuration-1.0.1/dkist_service_configuration/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/SOURCES.txt` & `dkist-service-configuration-1.0.1/dkist_service_configuration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc4/setup.cfg` & `dkist-service-configuration-1.0.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
 	loguru
-	pydantic < 2.0
+	pydantic[dotenv] < 2.0
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 
 [tool:pytest]
```

