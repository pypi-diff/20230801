# Comparing `tmp/Processador-XML-NFE-1.0.0.tar.gz` & `tmp/Processador-XML-NFE-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Processador-XML-NFE-1.0.0.tar", last modified: Tue Aug  1 00:30:09 2023, max compression
+gzip compressed data, was "Processador-XML-NFE-1.0.1.tar", last modified: Tue Aug  1 00:35:29 2023, max compression
```

## Comparing `Processador-XML-NFE-1.0.0.tar` & `Processador-XML-NFE-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 henrique  (1000) henrique  (1000)        0 2023-08-01 00:30:09.516645 Processador-XML-NFE-1.0.0/
--rw-rw-r--   0 henrique  (1000) henrique  (1000)     1078 2023-07-31 23:16:14.000000 Processador-XML-NFE-1.0.0/LICENSE
--rw-rw-r--   0 henrique  (1000) henrique  (1000)      617 2023-08-01 00:30:09.516645 Processador-XML-NFE-1.0.0/PKG-INFO
-drwxrwxr-x   0 henrique  (1000) henrique  (1000)        0 2023-08-01 00:30:09.516645 Processador-XML-NFE-1.0.0/Processador_XML_NFE.egg-info/
--rw-rw-r--   0 henrique  (1000) henrique  (1000)      617 2023-08-01 00:30:09.000000 Processador-XML-NFE-1.0.0/Processador_XML_NFE.egg-info/PKG-INFO
--rw-rw-r--   0 henrique  (1000) henrique  (1000)      299 2023-08-01 00:30:09.000000 Processador-XML-NFE-1.0.0/Processador_XML_NFE.egg-info/SOURCES.txt
--rw-rw-r--   0 henrique  (1000) henrique  (1000)        1 2023-08-01 00:30:09.000000 Processador-XML-NFE-1.0.0/Processador_XML_NFE.egg-info/dependency_links.txt
--rw-rw-r--   0 henrique  (1000) henrique  (1000)       16 2023-08-01 00:30:09.000000 Processador-XML-NFE-1.0.0/Processador_XML_NFE.egg-info/requires.txt
--rw-rw-r--   0 henrique  (1000) henrique  (1000)       16 2023-08-01 00:30:09.000000 Processador-XML-NFE-1.0.0/Processador_XML_NFE.egg-info/top_level.txt
--rw-rw-r--   0 henrique  (1000) henrique  (1000)      277 2023-08-01 00:20:23.000000 Processador-XML-NFE-1.0.0/README.md
-drwxrwxr-x   0 henrique  (1000) henrique  (1000)        0 2023-08-01 00:30:09.516645 Processador-XML-NFE-1.0.0/processador_nfe/
--rw-rw-r--   0 henrique  (1000) henrique  (1000)       26 2023-08-01 00:16:53.000000 Processador-XML-NFE-1.0.0/processador_nfe/__init__.py
--rw-rw-r--   0 henrique  (1000) henrique  (1000)     3203 2023-07-31 23:23:16.000000 Processador-XML-NFE-1.0.0/processador_nfe/processador.py
--rw-rw-r--   0 henrique  (1000) henrique  (1000)       38 2023-08-01 00:30:09.516645 Processador-XML-NFE-1.0.0/setup.cfg
--rw-rw-r--   0 henrique  (1000) henrique  (1000)      584 2023-08-01 00:28:55.000000 Processador-XML-NFE-1.0.0/setup.py
+drwxrwxr-x   0 henrique  (1000) henrique  (1000)        0 2023-08-01 00:35:29.763608 Processador-XML-NFE-1.0.1/
+-rw-rw-r--   0 henrique  (1000) henrique  (1000)     1078 2023-07-31 23:16:14.000000 Processador-XML-NFE-1.0.1/LICENSE
+-rw-rw-r--   0 henrique  (1000) henrique  (1000)      601 2023-08-01 00:35:29.763608 Processador-XML-NFE-1.0.1/PKG-INFO
+drwxrwxr-x   0 henrique  (1000) henrique  (1000)        0 2023-08-01 00:35:29.763608 Processador-XML-NFE-1.0.1/Processador_XML_NFE.egg-info/
+-rw-rw-r--   0 henrique  (1000) henrique  (1000)      601 2023-08-01 00:35:29.000000 Processador-XML-NFE-1.0.1/Processador_XML_NFE.egg-info/PKG-INFO
+-rw-rw-r--   0 henrique  (1000) henrique  (1000)      299 2023-08-01 00:35:29.000000 Processador-XML-NFE-1.0.1/Processador_XML_NFE.egg-info/SOURCES.txt
+-rw-rw-r--   0 henrique  (1000) henrique  (1000)        1 2023-08-01 00:35:29.000000 Processador-XML-NFE-1.0.1/Processador_XML_NFE.egg-info/dependency_links.txt
+-rw-rw-r--   0 henrique  (1000) henrique  (1000)       16 2023-08-01 00:35:29.000000 Processador-XML-NFE-1.0.1/Processador_XML_NFE.egg-info/requires.txt
+-rw-rw-r--   0 henrique  (1000) henrique  (1000)       16 2023-08-01 00:35:29.000000 Processador-XML-NFE-1.0.1/Processador_XML_NFE.egg-info/top_level.txt
+-rw-rw-r--   0 henrique  (1000) henrique  (1000)      277 2023-08-01 00:20:23.000000 Processador-XML-NFE-1.0.1/README.md
+drwxrwxr-x   0 henrique  (1000) henrique  (1000)        0 2023-08-01 00:35:29.763608 Processador-XML-NFE-1.0.1/processador_nfe/
+-rw-rw-r--   0 henrique  (1000) henrique  (1000)       26 2023-08-01 00:16:53.000000 Processador-XML-NFE-1.0.1/processador_nfe/__init__.py
+-rw-rw-r--   0 henrique  (1000) henrique  (1000)     3203 2023-07-31 23:23:16.000000 Processador-XML-NFE-1.0.1/processador_nfe/processador.py
+-rw-rw-r--   0 henrique  (1000) henrique  (1000)       38 2023-08-01 00:35:29.763608 Processador-XML-NFE-1.0.1/setup.cfg
+-rw-rw-r--   0 henrique  (1000) henrique  (1000)      560 2023-08-01 00:35:25.000000 Processador-XML-NFE-1.0.1/setup.py
```

### Comparing `Processador-XML-NFE-1.0.0/LICENSE` & `Processador-XML-NFE-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Processador-XML-NFE-1.0.0/PKG-INFO` & `Processador-XML-NFE-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: Processador-XML-NFE
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extraia relatórios a partir do XML de diversas Notas Fiscais Eletrônicas(NFE) de uma só vez!
 Author: Henrique Venancio
 Author-email: hvs.git@gmail.com
 License: MIT License
-Keywords: NFE,Nota Fiscal,XML
+Keywords: NFE
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Processador-XML
 
 Script que filtra arquivos .XML que definem uma NFE e extrai algumas informações gerando um
 arquivo do tipo .xlsx (Excel).
```

### Comparing `Processador-XML-NFE-1.0.0/Processador_XML_NFE.egg-info/PKG-INFO` & `Processador-XML-NFE-1.0.1/Processador_XML_NFE.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: Processador-XML-NFE
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extraia relatórios a partir do XML de diversas Notas Fiscais Eletrônicas(NFE) de uma só vez!
 Author: Henrique Venancio
 Author-email: hvs.git@gmail.com
 License: MIT License
-Keywords: NFE,Nota Fiscal,XML
+Keywords: NFE
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Processador-XML
 
 Script que filtra arquivos .XML que definem uma NFE e extrai algumas informações gerando um
 arquivo do tipo .xlsx (Excel).
```

### Comparing `Processador-XML-NFE-1.0.0/processador_nfe/processador.py` & `Processador-XML-NFE-1.0.1/processador_nfe/processador.py`

 * *Files identical despite different names*

### Comparing `Processador-XML-NFE-1.0.0/setup.py` & `Processador-XML-NFE-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='Processador-XML-NFE',
-      version='1.0.0',
+      version='1.0.1',
       license='MIT License',
       author='Henrique Venancio',
       long_description=readme,
       long_description_content_type="text/markdown",
       author_email='hvs.git@gmail.com',
-      keywords=['NFE', 'Nota Fiscal', 'XML'],
+      keywords='NFE',
       description=u'Extraia relatórios a partir do XML de diversas Notas Fiscais Eletrônicas(NFE) de uma só vez!',
       packages=['processador_nfe'],
       install_requires=['pandas', 'openpyxl'], )
```

