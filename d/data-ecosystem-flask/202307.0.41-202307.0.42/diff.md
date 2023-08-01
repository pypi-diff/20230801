# Comparing `tmp/data_ecosystem_flask-202307.0.41.tar.gz` & `tmp/data_ecosystem_flask-202307.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_flask-202307.0.41.tar", max compression
+gzip compressed data, was "data_ecosystem_flask-202307.0.42.tar", max compression
```

## Comparing `data_ecosystem_flask-202307.0.41.tar` & `data_ecosystem_flask-202307.0.42.tar`

### file list

```diff
@@ -1,38 +1,30 @@
--rw-r--r--   0        0        0      573 2023-07-31 03:16:38.733862 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/.env
--rw-r--r--   0        0        0      863 2023-07-28 12:14:08.336487 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/Makefile.ps1
--rw-r--r--   0        0        0     1155 2023-07-28 12:14:08.339487 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/__init__.py
--rw-r--r--   0        0        0    44698 2023-07-31 01:23:52.403322 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/app.py
--rw-r--r--   0        0        0    14371 2023-07-31 10:28:32.451044 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/app_startup.py
--rw-r--r--   0        0        0     5341 2023-07-31 03:16:38.718857 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/config/config.dev.json
--rw-r--r--   0        0        0     5071 2023-07-31 03:16:38.721863 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/config/config.prod.json
--rw-r--r--   0        0        0      344 2023-07-31 03:16:38.724862 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/config/manifest.json
--rw-r--r--   0        0        0    59440 2023-07-31 03:16:38.707859 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/excel-manifest-schema.xlsx
--rw-r--r--   0        0        0    24571 2023-07-31 03:16:38.696864 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/excel_manifest_schema_for_schemas_sql.xlsx
--rw-r--r--   0        0        0    12829 2023-07-31 03:16:38.693865 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/excel_manifest_schema_for_schemas_sql_merged.xlsx
--rw-r--r--   0        0        0    27811 2023-07-31 03:16:38.699864 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/excel_manifest_schema_for_tables_sql.xlsx
--rw-r--r--   0        0        0    38559 2023-07-31 03:16:38.703859 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/excel_manifest_schema_valuesets.xlsx
--rw-r--r--   0        0        0    28571 2023-07-28 12:14:08.351488 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/install.py
--rw-r--r--   0        0        0    14945 2023-07-31 03:16:38.679873 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/json-manifest-schema.json
--rw-r--r--   0        0        0      344 2023-07-28 20:05:27.819214 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/manifest.json
--rw-r--r--   0        0        0    14015 2023-07-31 03:16:38.683854 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/manifest.schema.json
--rw-r--r--   0        0        0    11000 2023-07-31 03:16:41.695832 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/requirements.txt
--rw-r--r--   0        0        0     7042 2023-07-31 22:15:55.425162 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/templates/download.html
--rw-r--r--   0        0        0      432 2023-07-28 12:14:08.365485 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/templates/error.html
--rw-r--r--   0        0        0     2723 2023-07-28 12:14:08.367490 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/templates/log_file.html
--rw-r--r--   0        0        0     1905 2023-07-28 12:14:08.370482 data_ecosystem_flask-202307.0.41/data_ecosystem_flask/templates/upload.html
--rw-r--r--   0        0        0    59440 2023-07-27 10:12:39.655773 data_ecosystem_flask-202307.0.41/dev_schema/excel-manifest-schema.xlsx
--rw-r--r--   0        0        0    24571 2023-07-27 10:12:39.658771 data_ecosystem_flask-202307.0.41/dev_schema/excel_manifest_schema_for_schemas_sql.xlsx
--rw-r--r--   0        0        0    12829 2023-07-27 10:12:39.660775 data_ecosystem_flask-202307.0.41/dev_schema/excel_manifest_schema_for_schemas_sql_merged.xlsx
--rw-r--r--   0        0        0    27811 2023-07-27 10:12:39.663772 data_ecosystem_flask-202307.0.41/dev_schema/excel_manifest_schema_for_tables_sql.xlsx
--rw-r--r--   0        0        0    38559 2023-07-27 10:12:39.666775 data_ecosystem_flask-202307.0.41/dev_schema/excel_manifest_schema_valuesets.xlsx
--rw-r--r--   0        0        0    14945 2023-07-27 10:12:39.669778 data_ecosystem_flask-202307.0.41/dev_schema/json-manifest-schema.json
--rw-r--r--   0        0        0    14015 2023-07-27 10:12:39.671783 data_ecosystem_flask-202307.0.41/dev_schema/manifest.schema.json
--rw-r--r--   0        0        0    11368 2023-07-30 21:12:34.051256 data_ecosystem_flask-202307.0.41/license.md
--rw-r--r--   0        0        0     5341 2023-07-31 00:45:49.413323 data_ecosystem_flask-202307.0.41/ocio/ocio_pade_dev/config/config.dev.json
--rw-r--r--   0        0        0     5071 2023-07-30 01:26:52.658842 data_ecosystem_flask-202307.0.41/ocio/ocio_pade_dev/config/config.prod.json
--rw-r--r--   0        0        0      344 2023-07-30 01:26:52.662843 data_ecosystem_flask-202307.0.41/ocio/ocio_pade_dev/config/manifest.json
--rw-r--r--   0        0        0     2895 2023-07-31 22:33:45.587725 data_ecosystem_flask-202307.0.41/pyproject.toml
--rw-r--r--   0        0        0    15048 2023-07-31 02:47:55.916878 data_ecosystem_flask-202307.0.41/readme.md
--rw-r--r--   0        0        0      126 2023-06-30 18:22:06.511392 data_ecosystem_flask-202307.0.41/setup.cfg
--rw-r--r--   0        0        0      127 2023-06-30 18:22:06.514388 data_ecosystem_flask-202307.0.41/setup.py
--rw-r--r--   0        0        0     1889 1970-01-01 00:00:00.000000 data_ecosystem_flask-202307.0.41/PKG-INFO
+-rw-r--r--   0        0        0      573 2023-08-01 01:30:38.203096 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/.env
+-rw-r--r--   0        0        0      863 2023-07-28 12:14:08.336487 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/Makefile.ps1
+-rw-r--r--   0        0        0     1155 2023-07-28 12:14:08.339487 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/__init__.py
+-rw-r--r--   0        0        0    44698 2023-07-31 01:23:52.403322 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/app.py
+-rw-r--r--   0        0        0    14371 2023-07-31 10:28:32.451044 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/app_startup.py
+-rw-r--r--   0        0        0     5341 2023-08-01 01:30:38.189095 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/config/config.dev.json
+-rw-r--r--   0        0        0     5071 2023-08-01 01:30:38.192101 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/config/config.prod.json
+-rw-r--r--   0        0        0      344 2023-08-01 01:30:38.195099 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/config/manifest.json
+-rw-r--r--   0        0        0    28571 2023-07-28 12:14:08.351488 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/install.py
+-rw-r--r--   0        0        0    17797 2023-08-01 01:36:49.707967 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/requirements.txt
+-rw-r--r--   0        0        0     7052 2023-08-01 01:29:41.755916 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/templates/download.html
+-rw-r--r--   0        0        0      432 2023-07-28 12:14:08.365485 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/templates/error.html
+-rw-r--r--   0        0        0     2723 2023-07-28 12:14:08.367490 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/templates/log_file.html
+-rw-r--r--   0        0        0     1905 2023-07-28 12:14:08.370482 data_ecosystem_flask-202307.0.42/data_ecosystem_flask/templates/upload.html
+-rw-r--r--   0        0        0    59440 2023-07-27 10:12:39.655773 data_ecosystem_flask-202307.0.42/dev_schema/excel-manifest-schema.xlsx
+-rw-r--r--   0        0        0    24571 2023-07-27 10:12:39.658771 data_ecosystem_flask-202307.0.42/dev_schema/excel_manifest_schema_for_schemas_sql.xlsx
+-rw-r--r--   0        0        0    12829 2023-07-27 10:12:39.660775 data_ecosystem_flask-202307.0.42/dev_schema/excel_manifest_schema_for_schemas_sql_merged.xlsx
+-rw-r--r--   0        0        0    27811 2023-07-27 10:12:39.663772 data_ecosystem_flask-202307.0.42/dev_schema/excel_manifest_schema_for_tables_sql.xlsx
+-rw-r--r--   0        0        0    38559 2023-07-27 10:12:39.666775 data_ecosystem_flask-202307.0.42/dev_schema/excel_manifest_schema_valuesets.xlsx
+-rw-r--r--   0        0        0    14945 2023-07-27 10:12:39.669778 data_ecosystem_flask-202307.0.42/dev_schema/json-manifest-schema.json
+-rw-r--r--   0        0        0    14015 2023-07-27 10:12:39.671783 data_ecosystem_flask-202307.0.42/dev_schema/manifest.schema.json
+-rw-r--r--   0        0        0    11368 2023-07-30 21:12:34.051256 data_ecosystem_flask-202307.0.42/license.md
+-rw-r--r--   0        0        0     5341 2023-07-31 00:45:49.413323 data_ecosystem_flask-202307.0.42/ocio/ocio_pade_dev/config/config.dev.json
+-rw-r--r--   0        0        0     5071 2023-07-30 01:26:52.658842 data_ecosystem_flask-202307.0.42/ocio/ocio_pade_dev/config/config.prod.json
+-rw-r--r--   0        0        0      344 2023-07-30 01:26:52.662843 data_ecosystem_flask-202307.0.42/ocio/ocio_pade_dev/config/manifest.json
+-rw-r--r--   0        0        0     2895 2023-08-01 01:34:39.127225 data_ecosystem_flask-202307.0.42/pyproject.toml
+-rw-r--r--   0        0        0    15048 2023-07-31 02:47:55.916878 data_ecosystem_flask-202307.0.42/readme.md
+-rw-r--r--   0        0        0      126 2023-06-30 18:22:06.511392 data_ecosystem_flask-202307.0.42/setup.cfg
+-rw-r--r--   0        0        0      127 2023-06-30 18:22:06.514388 data_ecosystem_flask-202307.0.42/setup.py
+-rw-r--r--   0        0        0     1889 1970-01-01 00:00:00.000000 data_ecosystem_flask-202307.0.42/PKG-INFO
```

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/.env` & `data_ecosystem_flask-202307.0.42/data_ecosystem_flask/.env`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/Makefile.ps1` & `data_ecosystem_flask-202307.0.42/data_ecosystem_flask/Makefile.ps1`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/__init__.py` & `data_ecosystem_flask-202307.0.42/data_ecosystem_flask/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/app.py` & `data_ecosystem_flask-202307.0.42/data_ecosystem_flask/app.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/app_startup.py` & `data_ecosystem_flask-202307.0.42/data_ecosystem_flask/app_startup.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/config/config.dev.json` & `data_ecosystem_flask-202307.0.42/data_ecosystem_flask/config/config.dev.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/config/config.prod.json` & `data_ecosystem_flask-202307.0.42/data_ecosystem_flask/config/config.prod.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/excel-manifest-schema.xlsx` & `data_ecosystem_flask-202307.0.42/dev_schema/excel-manifest-schema.xlsx`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/excel_manifest_schema_for_schemas_sql.xlsx` & `data_ecosystem_flask-202307.0.42/dev_schema/excel_manifest_schema_for_schemas_sql.xlsx`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/excel_manifest_schema_for_schemas_sql_merged.xlsx` & `data_ecosystem_flask-202307.0.42/dev_schema/excel_manifest_schema_for_schemas_sql_merged.xlsx`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/excel_manifest_schema_for_tables_sql.xlsx` & `data_ecosystem_flask-202307.0.42/dev_schema/excel_manifest_schema_for_tables_sql.xlsx`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/excel_manifest_schema_valuesets.xlsx` & `data_ecosystem_flask-202307.0.42/dev_schema/excel_manifest_schema_valuesets.xlsx`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/install.py` & `data_ecosystem_flask-202307.0.42/data_ecosystem_flask/install.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/json-manifest-schema.json` & `data_ecosystem_flask-202307.0.42/dev_schema/json-manifest-schema.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/manifest.schema.json` & `data_ecosystem_flask-202307.0.42/dev_schema/manifest.schema.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/requirements.txt` & `data_ecosystem_flask-202307.0.42/data_ecosystem_flask/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,146 +1,237 @@
+adal==1.2.7 ; python_version >= "3.9" and python_version < "4.0"
+alabaster==0.7.13 ; python_version >= "3.9" and python_version < "4.0"
 alation==0.1.14 ; python_version >= "3.9" and python_version < "4.0"
 aniso8601==9.0.1 ; python_version >= "3.9" and python_version < "4.0"
+anyascii==0.3.2 ; python_version >= "3.9" and python_version < "4.0"
 anyio==3.7.1 ; python_version >= "3.9" and python_version < "4.0"
 appdirs==1.4.4 ; python_version >= "3.9" and python_version < "4.0"
 appnope==0.1.3 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "darwin" or python_version >= "3.9" and python_version < "4.0" and platform_system == "Darwin"
 argon2-cffi-bindings==21.2.0 ; python_version >= "3.9" and python_version < "4.0"
 argon2-cffi==21.3.0 ; python_version >= "3.9" and python_version < "4.0"
 arrow==1.2.3 ; python_version >= "3.9" and python_version < "4.0"
+astroid==2.15.6 ; python_version >= "3.9" and python_version < "4.0"
 asttokens==2.2.1 ; python_version >= "3.9" and python_version < "4.0"
 attrs==23.1.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-common==1.1.28 ; python_version >= "3.9" and python_version < "4.0"
 azure-core==1.28.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-identity==1.13.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-keyvault-certificates==4.7.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-keyvault-keys==4.8.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-keyvault-secrets==4.7.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-keyvault==4.2.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-mgmt-core==1.4.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-mgmt-monitor==5.0.1 ; python_version >= "3.9" and python_version < "4.0"
+azure-mgmt-resource==23.0.1 ; python_version >= "3.9" and python_version < "4.0"
 azure-monitor-opentelemetry-exporter==1.0.0b14 ; python_version >= "3.9" and python_version < "4.0"
+azure-storage-blob==12.17.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-storage-file-datalake==12.12.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-storage-queue==12.6.0 ; python_version >= "3.9" and python_version < "4.0"
+babel==2.12.1 ; python_version >= "3.9" and python_version < "4.0"
 backcall==0.2.0 ; python_version >= "3.9" and python_version < "4.0"
 beautifulsoup4==4.12.2 ; python_version >= "3.9" and python_version < "4.0"
 bleach==6.0.0 ; python_version >= "3.9" and python_version < "4.0"
 blinker==1.6.2 ; python_version >= "3.9" and python_version < "4.0"
+boto3==1.21.18 ; python_version >= "3.9" and python_version < "4.0"
+botocore==1.24.18 ; python_version >= "3.9" and python_version < "4.0"
+cachetools==5.3.1 ; python_version >= "3.9" and python_version < "4.0"
 certifi==2023.5.7 ; python_version >= "3.9" and python_version < "4.0"
 cffi==1.15.1 ; python_version >= "3.9" and python_version < "4.0"
+chardet==5.1.0 ; python_version >= "3.9" and python_version < "4.0"
 charset-normalizer==3.2.0 ; python_version >= "3.9" and python_version < "4.0"
 click==8.1.6 ; python_version >= "3.9" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and platform_system == "Windows" or python_version >= "3.9" and python_version < "4.0" and sys_platform == "win32"
 comm==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
+cryptography==41.0.2 ; python_version >= "3.9" and python_version < "4.0"
+data-ecosystem-services==202307.0.41 ; python_version >= "3.9" and python_version < "4.0"
+ddlparse==1.10.0 ; python_version >= "3.9" and python_version < "4.0"
 debugpy==1.6.7 ; python_version >= "3.9" and python_version < "4.0"
 decorator==5.1.1 ; python_version >= "3.9" and python_version < "4.0"
 defusedxml==0.7.1 ; python_version >= "3.9" and python_version < "4.0"
+delta-spark==2.4.0 ; python_version >= "3.9" and python_version < "4.0"
 deprecated==1.2.14 ; python_version >= "3.9" and python_version < "4.0"
+docutils==0.17.1 ; python_version >= "3.9" and python_version < "4.0"
 entrypoints==0.4 ; python_version >= "3.9" and python_version < "4.0"
 et-xmlfile==1.1.0 ; python_version >= "3.9" and python_version < "4.0"
 exceptiongroup==1.1.2 ; python_version >= "3.9" and python_version < "3.11"
 executing==1.2.0 ; python_version >= "3.9" and python_version < "4.0"
 fastjsonschema==2.18.0 ; python_version >= "3.9" and python_version < "4.0"
+findspark==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 fixedint==0.1.6 ; python_version >= "3.9" and python_version < "4.0"
 flake8==4.0.1 ; python_version >= "3.9" and python_version < "4.0"
 flask-restful==0.3.10 ; python_version >= "3.9" and python_version < "4.0"
 flask-restx==1.1.0 ; python_version >= "3.9" and python_version < "4.0"
 flask==2.3.2 ; python_version >= "3.9" and python_version < "4.0"
 fqdn==1.5.1 ; python_version >= "3.9" and python_version < "4"
 fsspec==2023.6.0 ; python_version >= "3.9" and python_version < "4.0"
+google-api-core==2.11.1 ; python_version >= "3.9" and python_version < "4.0"
+google-auth==2.22.0 ; python_version >= "3.9" and python_version < "4.0"
+googleapis-common-protos==1.60.0 ; python_version >= "3.9" and python_version < "4.0"
+html2text==2020.1.16 ; python_version >= "3.9" and python_version < "4.0"
 humanize==4.7.0 ; python_version >= "3.9" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.9" and python_version < "4.0"
+imagesize==1.4.1 ; python_version >= "3.9" and python_version < "4.0"
 importlib-metadata==6.0.1 ; python_version >= "3.9" and python_version < "4.0"
 importlib-resources==6.0.0 ; python_version >= "3.9" and python_version < "4.0"
+iniconfig==2.0.0 ; python_version >= "3.9" and python_version < "4.0"
 ipykernel==6.25.0 ; python_version >= "3.9" and python_version < "4.0"
 ipython-genutils==0.2.0 ; python_version >= "3.9" and python_version < "4.0"
 ipython==8.14.0 ; python_version >= "3.9" and python_version < "4.0"
 isodate==0.6.1 ; python_version >= "3.9" and python_version < "4.0"
 isoduration==20.11.0 ; python_version >= "3.9" and python_version < "4.0"
 itsdangerous==2.1.2 ; python_version >= "3.9" and python_version < "4.0"
 jedi==0.19.0 ; python_version >= "3.9" and python_version < "4.0"
 jinja2==3.1.2 ; python_version >= "3.9" and python_version < "4.0"
+jmespath==0.10.0 ; python_version >= "3.9" and python_version < "4.0"
 joblib==1.3.1 ; python_version >= "3.9" and python_version < "4.0"
+jsondiff==2.0.0 ; python_version >= "3.9" and python_version < "4.0"
 jsonpointer==2.4 ; python_version >= "3.9" and python_version < "4.0"
 jsonschema-specifications==2023.7.1 ; python_version >= "3.9" and python_version < "4.0"
 jsonschema==4.18.4 ; python_version >= "3.9" and python_version < "4.0"
 jsonschema[format-nongpl]==4.18.4 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-client==7.4.9 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-core==5.3.1 ; python_version >= "3.9" and python_version < "4.0"
-jupyter-events==0.6.3 ; python_version >= "3.9" and python_version < "4.0"
+jupyter-events==0.7.0 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-server-terminals==0.4.4 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-server==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
 jupyterlab-pygments==0.2.2 ; python_version >= "3.9" and python_version < "4.0"
+lazy-object-proxy==1.9.0 ; python_version >= "3.9" and python_version < "4.0"
 lxml==4.9.3 ; python_version >= "3.9" and python_version < "4.0"
+markdown-it-py==2.2.0 ; python_version >= "3.9" and python_version < "4.0"
+markdown==3.4.4 ; python_version >= "3.9" and python_version < "4.0"
 markupsafe==2.1.3 ; python_version >= "3.9" and python_version < "4.0"
 matplotlib-inline==0.1.6 ; python_version >= "3.9" and python_version < "4.0"
 mccabe==0.6.1 ; python_version >= "3.9" and python_version < "4.0"
+mdit-py-plugins==0.3.5 ; python_version >= "3.9" and python_version < "4.0"
+mdurl==0.1.2 ; python_version >= "3.9" and python_version < "4.0"
 mistune==0.8.4 ; python_version >= "3.9" and python_version < "4.0"
+msal-extensions==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
+msal==1.23.0 ; python_version >= "3.9" and python_version < "4.0"
 msrest==0.7.1 ; python_version >= "3.9" and python_version < "4.0"
+myst-parser==0.18.1 ; python_version >= "3.9" and python_version < "4.0"
 nbclassic==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
 nbclient==0.8.0 ; python_version >= "3.9" and python_version < "4.0"
 nbconvert==6.5.4 ; python_version >= "3.9" and python_version < "4.0"
-nbformat==5.9.1 ; python_version >= "3.9" and python_version < "4.0"
+nbformat==5.9.2 ; python_version >= "3.9" and python_version < "4.0"
 nest-asyncio==1.5.7 ; python_version >= "3.9" and python_version < "4.0"
 notebook-shim==0.2.3 ; python_version >= "3.9" and python_version < "4.0"
 notebook==6.5.5 ; python_version >= "3.9" and python_version < "4.0"
-numpy==1.25.1 ; python_version >= "3.9" and python_version < "4.0"
+numpy==1.25.2 ; python_version >= "3.9" and python_version < "4.0"
 oauthlib==3.2.2 ; python_version >= "3.9" and python_version < "4.0"
+opencensus-context==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
+opencensus-ext-azure==1.1.9 ; python_version >= "3.9" and python_version < "4.0"
+opencensus==0.11.2 ; python_version >= "3.9" and python_version < "4.0"
 openpyxl==3.1.2 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-api==1.18.0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-instrumentation-flask==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-instrumentation-wsgi==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-instrumentation==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-sdk==1.18.0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-semantic-conventions==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-util-http==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 overrides==7.3.1 ; python_version >= "3.9" and python_version < "4.0"
 packaging==23.1 ; python_version >= "3.9" and python_version < "4.0"
 pandas==2.0.3 ; python_version >= "3.9" and python_version < "4.0"
 pandocfilters==1.5.0 ; python_version >= "3.9" and python_version < "4.0"
 parso==0.8.3 ; python_version >= "3.9" and python_version < "4.0"
+pathlib==1.0.1 ; python_version >= "3.9" and python_version < "4.0"
+pbr==5.11.1 ; python_version >= "3.9" and python_version < "4.0"
 pexpect==4.8.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform != "win32"
 pickleshare==0.7.5 ; python_version >= "3.9" and python_version < "4.0"
 pins==0.8.1 ; python_version >= "3.9" and python_version < "4.0"
+pip-system-certs==4.0 ; python_version >= "3.9" and python_version < "4.0"
 pip==23.2.1 ; python_version >= "3.9" and python_version < "4.0"
 platformdirs==3.10.0 ; python_version >= "3.9" and python_version < "4.0"
+pluggy==1.2.0 ; python_version >= "3.9" and python_version < "4.0"
+portalocker==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
 prometheus-client==0.17.1 ; python_version >= "3.9" and python_version < "4.0"
 prompt-toolkit==3.0.39 ; python_version >= "3.9" and python_version < "4.0"
+protobuf==4.23.4 ; python_version >= "3.9" and python_version < "4.0"
 psutil==5.9.5 ; python_version >= "3.9" and python_version < "4.0"
 ptyprocess==0.7.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform != "win32" or python_version >= "3.9" and python_version < "4.0" and os_name != "nt"
 pure-eval==0.2.2 ; python_version >= "3.9" and python_version < "4.0"
+py4j==0.10.9.7 ; python_version >= "3.9" and python_version < "4.0"
 py==1.11.0 ; python_version >= "3.9" and python_version < "4.0" and implementation_name == "pypy"
+pyarrow==10.0.1 ; python_version >= "3.9" and python_version < "4.0"
+pyasn1-modules==0.3.0 ; python_version >= "3.9" and python_version < "4.0"
+pyasn1==0.5.0 ; python_version >= "3.9" and python_version < "4.0"
 pycodestyle==2.8.0 ; python_version >= "3.9" and python_version < "4.0"
 pycparser==2.21 ; python_version >= "3.9" and python_version < "4.0"
+pydash==7.0.6 ; python_version >= "3.9" and python_version < "4.0"
 pyflakes==2.4.0 ; python_version >= "3.9" and python_version < "4.0"
 pygments==2.15.1 ; python_version >= "3.9" and python_version < "4.0"
 pyjwt==2.8.0 ; python_version >= "3.9" and python_version < "4.0"
+pyjwt[crypto]==2.8.0 ; python_version >= "3.9" and python_version < "4.0"
+pyparsing==3.1.1 ; python_version >= "3.9" and python_version < "4.0"
+pyreadstat==1.2.2 ; python_version >= "3.9" and python_version < "4.0"
+pyspark==3.4.1 ; python_version >= "3.9" and python_version < "4.0"
+pytest==7.4.0 ; python_version >= "3.9" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.9" and python_version < "4.0"
 python-dotenv==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
 python-json-logger==2.0.7 ; python_version >= "3.9" and python_version < "4.0"
 pytz==2023.3 ; python_version >= "3.9" and python_version < "4.0"
-pywin32==306 ; sys_platform == "win32" and platform_python_implementation != "PyPy" and python_version >= "3.9" and python_version < "4.0"
+pywin32==306 ; python_version >= "3.9" and sys_platform == "win32" and python_version < "4.0" and platform_python_implementation != "PyPy" or python_version >= "3.9" and platform_system == "Windows" and python_version < "4.0"
 pywinpty==2.0.11 ; python_version >= "3.9" and python_version < "4.0" and os_name == "nt"
 pyyaml==6.0.1 ; python_version >= "3.9" and python_version < "4.0"
 pyzmq==24.0.1 ; python_version >= "3.9" and python_version < "4.0"
 referencing==0.30.0 ; python_version >= "3.9" and python_version < "4.0"
 requests-oauthlib==1.3.1 ; python_version >= "3.9" and python_version < "4.0"
 requests==2.31.0 ; python_version >= "3.9" and python_version < "4.0"
+retrying==1.3.4 ; python_version >= "3.9" and python_version < "4.0"
 rfc3339-validator==0.1.4 ; python_version >= "3.9" and python_version < "4.0"
 rfc3986-validator==0.1.1 ; python_version >= "3.9" and python_version < "4.0"
+rich==13.5.1 ; python_version >= "3.9" and python_version < "4.0"
 rpds-py==0.9.2 ; python_version >= "3.9" and python_version < "4.0"
+rsa==4.9 ; python_version >= "3.9" and python_version < "4"
 rsconnect-jupyter==1.8.0 ; python_version >= "3.9" and python_version < "4.0"
 rsconnect-python==1.19.0 ; python_version >= "3.9" and python_version < "4.0"
 rsconnect==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
+s3transfer==0.5.2 ; python_version >= "3.9" and python_version < "4.0"
 semver==2.13.0 ; python_version >= "3.9" and python_version < "4.0"
 send2trash==1.8.2 ; python_version >= "3.9" and python_version < "4.0"
 setuptools==65.6.3 ; python_version >= "3.9" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.9" and python_version < "4.0"
 sniffio==1.3.0 ; python_version >= "3.9" and python_version < "4.0"
+snowballstemmer==2.2.0 ; python_version >= "3.9" and python_version < "4.0"
 soupsieve==2.4.1 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-autoapi==2.1.1 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-autodoc-typehints==1.23.0 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-markdown-builder==0.5.5 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-markdown-tables==0.0.17 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-rtd-theme==1.2.2 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-sitemap==2.5.0 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-sql==1.3.5 ; python_version >= "3.9" and python_version < "4.0"
+sphinx==5.3.0 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-applehelp==1.0.4 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-devhelp==1.0.2 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-htmlhelp==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-jquery==4.1 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-jsmath==1.0.1 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-mermaid==0.7.1 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-qthelp==1.0.3 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-serializinghtml==1.1.5 ; python_version >= "3.9" and python_version < "4.0"
 stack-data==0.6.2 ; python_version >= "3.9" and python_version < "4.0"
+style==1.1.6 ; python_version >= "3.9" and python_version < "4.0"
 terminado==0.17.1 ; python_version >= "3.9" and python_version < "4.0"
+testresources==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 tinycss2==1.2.1 ; python_version >= "3.9" and python_version < "4.0"
+toml==0.10.2 ; python_version >= "3.9" and python_version < "4.0"
+tomli==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 tornado==6.3.2 ; python_version >= "3.9" and python_version < "4.0"
 traitlets==5.9.0 ; python_version >= "3.9" and python_version < "4.0"
+tryceratops==2.3.2 ; python_version >= "3.9" and python_version < "4.0"
 typing-extensions==4.7.1 ; python_version >= "3.9" and python_version < "4.0"
 tzdata==2023.3 ; python_version >= "3.9" and python_version < "4.0"
+unify==0.5 ; python_version >= "3.9" and python_version < "4.0"
+untokenize==0.1.1 ; python_version >= "3.9" and python_version < "4.0"
 uri-template==1.3.0 ; python_version >= "3.9" and python_version < "4.0"
 urllib3==1.26.16 ; python_version >= "3.9" and python_version < "4.0"
 wcwidth==0.2.6 ; python_version >= "3.9" and python_version < "4.0"
 webcolors==1.13 ; python_version >= "3.9" and python_version < "4.0"
 webencodings==0.5.1 ; python_version >= "3.9" and python_version < "4.0"
 websocket-client==1.6.1 ; python_version >= "3.9" and python_version < "4.0"
 werkzeug==2.3.6 ; python_version >= "3.9" and python_version < "4.0"
 wrapt==1.15.0 ; python_version >= "3.9" and python_version < "4.0"
 xlsxwriter==3.1.2 ; python_version >= "3.9" and python_version < "4.0"
 xxhash==3.3.0 ; python_version >= "3.9" and python_version < "4.0"
+yapf==0.33.0 ; python_version >= "3.9" and python_version < "4.0"
 zipp==3.16.2 ; python_version >= "3.9" and python_version < "4.0"
```

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/templates/download.html` & `data_ecosystem_flask-202307.0.42/data_ecosystem_flask/templates/download.html`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
         // Show the loader container while preparing the download
         loaderContainer.style.display = "flex";
         download_link.style.pointerEvents = "none"; // Disable the link to prevent multiple clicks
         errorMessage.innerText = ""; // Clear any previous error message
 
         // Set the download URL directly
-        download_url = `/alation/metadata_excel_file_download/${schema_id}`;
+        download_url = `/alation/metadata_excel_file_download?schema_id=${schema_id}`;
 
         // Make a request to the server to get the actual download URL
         fetch(download_url)
           .then((response) => {
             if (!response.ok) {
               // If the response is not successful, try to parse it as JSON
               return response
```

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/templates/log_file.html` & `data_ecosystem_flask-202307.0.42/data_ecosystem_flask/templates/log_file.html`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/data_ecosystem_flask/templates/upload.html` & `data_ecosystem_flask-202307.0.42/data_ecosystem_flask/templates/upload.html`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/license.md` & `data_ecosystem_flask-202307.0.42/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/ocio/ocio_pade_dev/config/config.dev.json` & `data_ecosystem_flask-202307.0.42/ocio/ocio_pade_dev/config/config.dev.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/ocio/ocio_pade_dev/config/config.prod.json` & `data_ecosystem_flask-202307.0.42/ocio/ocio_pade_dev/config/config.prod.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/pyproject.toml` & `data_ecosystem_flask-202307.0.42/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "data_ecosystem_flask"
 authors = [{name="John Bowyer", email="zfi4@cdc.gov" }]
 description = "Data Ecosystem Flask (PADE)  - Python "
 readme = "readme.md"
 requires-python = ">=3.9,<4.0"
-version = "202307.0.41"
+version = "202307.0.42"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9"
 ]
 
@@ -16,15 +16,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name = "data_ecosystem_flask"
-version="202307.0.41"
+version="202307.0.42"
 description = "Program Agnostic Data Ecosystem (PADE) - Flask Web Service"
 authors = ["John Bowyer <zfi4@cdc.gov>"]
 license = "Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
     "Development Status :: 4 - Beta",
```

### Comparing `data_ecosystem_flask-202307.0.41/readme.md` & `data_ecosystem_flask-202307.0.42/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.41/PKG-INFO` & `data_ecosystem_flask-202307.0.42/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-flask
-Version: 202307.0.41
+Version: 202307.0.42
 Summary: Program Agnostic Data Ecosystem (PADE) - Flask Web Service
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

