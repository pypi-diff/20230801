# Comparing `tmp/dbt-datadict-0.0.1.tar.gz` & `tmp/dbt-datadict-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-datadict-0.0.1.tar", last modified: Mon Jul 31 21:12:25 2023, max compression
+gzip compressed data, was "dbt-datadict-0.0.2.tar", last modified: Mon Jul 31 22:10:42 2023, max compression
```

## Comparing `dbt-datadict-0.0.1.tar` & `dbt-datadict-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tomshelley   (501) staff       (20)        0 2023-07-31 21:12:25.161122 dbt-datadict-0.0.1/
--rw-r--r--   0 tomshelley   (501) staff       (20)    35128 2023-07-19 13:05:29.000000 dbt-datadict-0.0.1/LICENSE
--rw-r--r--   0 tomshelley   (501) staff       (20)       15 2023-07-19 13:02:27.000000 dbt-datadict-0.0.1/MANIFEST.in
--rw-r--r--   0 tomshelley   (501) staff       (20)     7397 2023-07-31 21:12:25.160988 dbt-datadict-0.0.1/PKG-INFO
-drwxr-xr-x   0 tomshelley   (501) staff       (20)        0 2023-07-31 21:12:25.159171 dbt-datadict-0.0.1/datadict/
--rw-r--r--   0 tomshelley   (501) staff       (20)       96 2023-07-28 11:41:23.000000 dbt-datadict-0.0.1/datadict/__init__.py
--rw-r--r--   0 tomshelley   (501) staff       (20)    23398 2023-07-28 11:41:23.000000 dbt-datadict-0.0.1/datadict/datadict_class.py
--rw-r--r--   0 tomshelley   (501) staff       (20)     4780 2023-07-31 21:10:41.000000 dbt-datadict-0.0.1/datadict/datadict_dbt.py
--rw-r--r--   0 tomshelley   (501) staff       (20)     5507 2023-07-31 19:24:53.000000 dbt-datadict-0.0.1/datadict/datadict_helpers.py
--rw-r--r--   0 tomshelley   (501) staff       (20)     1596 2023-07-31 21:10:41.000000 dbt-datadict-0.0.1/datadict/datadict_main.py
--rw-r--r--   0 tomshelley   (501) staff       (20)     8155 2023-07-31 21:10:41.000000 dbt-datadict-0.0.1/datadict/datadict_yaml.py
-drwxr-xr-x   0 tomshelley   (501) staff       (20)        0 2023-07-31 21:12:25.160498 dbt-datadict-0.0.1/dbt_datadict.egg-info/
--rw-r--r--   0 tomshelley   (501) staff       (20)     7397 2023-07-31 21:12:25.000000 dbt-datadict-0.0.1/dbt_datadict.egg-info/PKG-INFO
--rw-r--r--   0 tomshelley   (501) staff       (20)      413 2023-07-31 21:12:25.000000 dbt-datadict-0.0.1/dbt_datadict.egg-info/SOURCES.txt
--rw-r--r--   0 tomshelley   (501) staff       (20)        1 2023-07-31 21:12:25.000000 dbt-datadict-0.0.1/dbt_datadict.egg-info/dependency_links.txt
--rw-r--r--   0 tomshelley   (501) staff       (20)       61 2023-07-31 21:12:25.000000 dbt-datadict-0.0.1/dbt_datadict.egg-info/entry_points.txt
--rw-r--r--   0 tomshelley   (501) staff       (20)       57 2023-07-31 21:12:25.000000 dbt-datadict-0.0.1/dbt_datadict.egg-info/requires.txt
--rw-r--r--   0 tomshelley   (501) staff       (20)       26 2023-07-31 21:12:25.000000 dbt-datadict-0.0.1/dbt_datadict.egg-info/top_level.txt
--rw-r--r--   0 tomshelley   (501) staff       (20)       38 2023-07-31 21:12:25.161162 dbt-datadict-0.0.1/setup.cfg
--rw-r--r--   0 tomshelley   (501) staff       (20)     1084 2023-07-31 21:10:46.000000 dbt-datadict-0.0.1/setup.py
-drwxr-xr-x   0 tomshelley   (501) staff       (20)        0 2023-07-31 21:12:25.160666 dbt-datadict-0.0.1/test/
--rw-r--r--   0 tomshelley   (501) staff       (20)    19755 2023-07-31 21:10:41.000000 dbt-datadict-0.0.1/test/test.py
+drwxr-xr-x   0 tomshelley   (501) staff       (20)        0 2023-07-31 22:10:42.745632 dbt-datadict-0.0.2/
+-rw-r--r--   0 tomshelley   (501) staff       (20)    35128 2023-07-19 13:05:29.000000 dbt-datadict-0.0.2/LICENSE
+-rw-r--r--   0 tomshelley   (501) staff       (20)       15 2023-07-19 13:02:27.000000 dbt-datadict-0.0.2/MANIFEST.in
+-rw-r--r--   0 tomshelley   (501) staff       (20)     7595 2023-07-31 22:10:42.745481 dbt-datadict-0.0.2/PKG-INFO
+drwxr-xr-x   0 tomshelley   (501) staff       (20)        0 2023-07-31 22:10:42.743593 dbt-datadict-0.0.2/datadict/
+-rw-r--r--   0 tomshelley   (501) staff       (20)       96 2023-07-28 11:41:23.000000 dbt-datadict-0.0.2/datadict/__init__.py
+-rw-r--r--   0 tomshelley   (501) staff       (20)    23398 2023-07-28 11:41:23.000000 dbt-datadict-0.0.2/datadict/datadict_class.py
+-rw-r--r--   0 tomshelley   (501) staff       (20)     4780 2023-07-31 21:10:41.000000 dbt-datadict-0.0.2/datadict/datadict_dbt.py
+-rw-r--r--   0 tomshelley   (501) staff       (20)     5507 2023-07-31 19:24:53.000000 dbt-datadict-0.0.2/datadict/datadict_helpers.py
+-rw-r--r--   0 tomshelley   (501) staff       (20)     1596 2023-07-31 21:10:41.000000 dbt-datadict-0.0.2/datadict/datadict_main.py
+-rw-r--r--   0 tomshelley   (501) staff       (20)     8837 2023-07-31 22:09:23.000000 dbt-datadict-0.0.2/datadict/datadict_yaml.py
+drwxr-xr-x   0 tomshelley   (501) staff       (20)        0 2023-07-31 22:10:42.744787 dbt-datadict-0.0.2/dbt_datadict.egg-info/
+-rw-r--r--   0 tomshelley   (501) staff       (20)     7595 2023-07-31 22:10:42.000000 dbt-datadict-0.0.2/dbt_datadict.egg-info/PKG-INFO
+-rw-r--r--   0 tomshelley   (501) staff       (20)      413 2023-07-31 22:10:42.000000 dbt-datadict-0.0.2/dbt_datadict.egg-info/SOURCES.txt
+-rw-r--r--   0 tomshelley   (501) staff       (20)        1 2023-07-31 22:10:42.000000 dbt-datadict-0.0.2/dbt_datadict.egg-info/dependency_links.txt
+-rw-r--r--   0 tomshelley   (501) staff       (20)       61 2023-07-31 22:10:42.000000 dbt-datadict-0.0.2/dbt_datadict.egg-info/entry_points.txt
+-rw-r--r--   0 tomshelley   (501) staff       (20)       57 2023-07-31 22:10:42.000000 dbt-datadict-0.0.2/dbt_datadict.egg-info/requires.txt
+-rw-r--r--   0 tomshelley   (501) staff       (20)       26 2023-07-31 22:10:42.000000 dbt-datadict-0.0.2/dbt_datadict.egg-info/top_level.txt
+-rw-r--r--   0 tomshelley   (501) staff       (20)       38 2023-07-31 22:10:42.745676 dbt-datadict-0.0.2/setup.cfg
+-rw-r--r--   0 tomshelley   (501) staff       (20)     1084 2023-07-31 22:05:55.000000 dbt-datadict-0.0.2/setup.py
+drwxr-xr-x   0 tomshelley   (501) staff       (20)        0 2023-07-31 22:10:42.744962 dbt-datadict-0.0.2/test/
+-rw-r--r--   0 tomshelley   (501) staff       (20)    19755 2023-07-31 21:10:41.000000 dbt-datadict-0.0.2/test/test.py
```

### Comparing `dbt-datadict-0.0.1/LICENSE` & `dbt-datadict-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-datadict-0.0.1/PKG-INFO` & `dbt-datadict-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-datadict
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python application for automating the application of consistent field definitions to large multi-layered dbt projects
 Home-page: https://github.com/TasmanAnalytics/dbt-datadictionary
 Author: Tom Shelley
 Author-email: tom@tasman.ai
 License: GNU GENERAL PUBLIC LICENSE
 Description: # dbt Data Dictionary
         
@@ -16,15 +16,15 @@
         ## **How to Use the Application**
         
         ### **Installation**
         
         1. Install dbt data dictionary using
             
             ```bash
-            pip install dbt-datadictionary
+            pip install dbt-datadict
             ```
             
         
         ### **Command-Line Interface (CLI) Usage**
         
         The Data Dictionary Application provides a command-line interface (CLI) that allows you to interact with the library easily.
         ### Command: `generate`
@@ -32,15 +32,15 @@
         This command generates yaml files using the dbt-codegen package. Where it finds existing model yaml files, it will merge the full column lists. For missing models, it will create a separate model yaml file using the name provided.
         
         **IMPORTANT**: This command will only run in a valid dbt project with dbt-labs/codegen installed.
         
         ### **Usage:**
         
         ```bash
-        $ dbt_datadict generate [-d <DICTIONARY>] [-D <DIRECTORY>]
+        $ datadict generate [-d <DICTIONARY>] [-D <DIRECTORY>]
         ```
         
         ### **Options:**
         
         - `-D, --directory <DIRECTORY>`: Directory to apply the dictionary. Default: 'models/'.
         - `-f, --file <NAME>`: The file to store any new models in.
         - `--sort`: Triggers the generated YAML files to be sorted alphabetically.
@@ -56,15 +56,15 @@
         ### Command: **`apply`**
         
         This command applies data dictionary updates to all model YAML files in the specified directory and its subdirectories.
         
         ### **Usage:**
         
         ```bash
-        $ dbt_datadict apply [-d <DICTIONARY>] [-D <DIRECTORY>]
+        $ datadict apply [-d <DICTIONARY>] [-D <DIRECTORY>]
         ```
         
         ### **Options:**
         
         - **`-d, --dictionary <DICTIONARY>`**: Location of the dictionary file. Default: 'datadictionary.yml'.
         - **`-D, --directory <DIRECTORY>`**: Directory to apply the dictionary. Default: 'models/'.
         
@@ -181,21 +181,25 @@
         
         `python setup.py develop`
         
         Building for distribution
         
         `python setup.py sdist bdist_wheel`
         
-        Pushing the distribution to the test server (changes require upversioning)
+        Pushing the distribution to Test PyPi (changes require upversioning and access)
+        
+        `twine upload --repository testpypi --skip-existing dist/*`
+        
+        Pushing the distribution to Production PyPi (changes require upversioning and access)
         
         `twine upload --repository pypi --skip-existing dist/*`
         
-        Pulling the distribution for use in another project
+        Pulling a test distribution
         
-        `pip install dbt-datadictionary==0.0.12`
+        `pip install --extra-index-url https://test.pypi.org/simple/ dbt-datadictionary==<version>`
         
         ## **Important Note**
         
         It is highly recommend to only use this library in a version controlled environment, such as git. Additionally, please ensure that you have backed up your model YAML files and data dictionary before applying any updates. The application modifies files in place and does not create backups automatically.
         
         Use this application responsibly and verify the updates before proceeding.
 Platform: UNKNOWN
```

### Comparing `dbt-datadict-0.0.1/datadict/datadict_class.py` & `dbt-datadict-0.0.2/datadict/datadict_class.py`

 * *Files identical despite different names*

### Comparing `dbt-datadict-0.0.1/datadict/datadict_dbt.py` & `dbt-datadict-0.0.2/datadict/datadict_dbt.py`

 * *Files identical despite different names*

### Comparing `dbt-datadict-0.0.1/datadict/datadict_helpers.py` & `dbt-datadict-0.0.2/datadict/datadict_helpers.py`

 * *Files identical despite different names*

### Comparing `dbt-datadict-0.0.1/datadict/datadict_main.py` & `dbt-datadict-0.0.2/datadict/datadict_main.py`

 * *Files identical despite different names*

### Comparing `dbt-datadict-0.0.1/datadict/datadict_yaml.py` & `dbt-datadict-0.0.2/datadict/datadict_yaml.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,23 @@
 def check_files_for_models(yaml_obj, files) -> dict:
     try:
         file_yamls = []
         model_list = []
         for file_path in files:
             file_contents = datadict_helpers.open_model_yml_file(yaml_obj, file_path)
             if file_contents['status'] == 'valid':
-                file_yamls.append({'file_path': file_path, 'file_yaml': file_contents['yaml']})
-                for model in file_contents['yaml']['models']:
-                    model_list.append({'name': model['name'], 'file': file_path})
+                try:
+                    for model in file_contents['yaml']['models']:
+                        model_list.append({'name': model['name'], 'file': file_path})
+                    file_yamls.append({'file_path': file_path, 'file_yaml': file_contents['yaml']})
+                except:
+                    logging.error(f"There was an issue processing file '{file_path}'. Ensure it is formatted correctly and retry.")
         return {'model_list': model_list, 'file_yamls': file_yamls}
     except Exception as e:
-        logging.error('Issues encountered when iterating through files to collect models: ' + e)
+        logging.error('Issues encountered when iterating through files to collect models. Error: ' + str(e))
 
 def combine_column_lists(current_yml, expected_yml) -> dict:
     updated = False
     combined_yaml = current_yml.copy()
     existing_columns = combined_yaml.setdefault('columns', [])
     # Iterate through the columns of expected_yml and add the missing ones to current_yml
     for column in expected_yml.get('columns', []):
@@ -160,13 +163,23 @@
         for model_num, model in enumerate(model_column_list['models']):
             if any(existing_model['name'] == model['name'] for existing_model in existing_model_list):
                 models_to_be_updated.append(model_column_list['models'][model_num])
             else:
                 models_to_be_added.append(model_column_list['models'][model_num])
         
         #5. For models in existing files, combine the column lists and write back to the existing file
-        updated_existing_files(yaml_obj, existing_file_yamls, models_to_be_updated, sort)
+        if len(models_to_be_updated) > 0:
+            logging.info(f"There are {len(models_to_be_updated)} models to be checked")
+            updated_existing_files(yaml_obj, existing_file_yamls, models_to_be_updated, sort)
+        else:
+            logging.info('There are no models requiring updating.')
 
         #6. For models missing from existing files, create a new file with the given name and output the metadata
-        add_missing_models(yaml_obj, os.path.join(directory, name), models_to_be_added, sort)
+        if len(models_to_be_added) > 0:
+            file_name = os.path.join(directory, name)
+            logging.info(f"There are {len(models_to_be_added)} models to be added to file '{file_name}'")
+            add_missing_models(yaml_obj, file_name, models_to_be_added, sort)
+        else:
+            logging.info('There are no models to be added.')
+
     except Exception as e:
-        logging.error('There was an error generating the YAML files. Error: ' + e)
+        logging.error('There was an error generating the YAML files. Error: ' + str(e))
```

### Comparing `dbt-datadict-0.0.1/dbt_datadict.egg-info/PKG-INFO` & `dbt-datadict-0.0.2/dbt_datadict.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-datadict
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python application for automating the application of consistent field definitions to large multi-layered dbt projects
 Home-page: https://github.com/TasmanAnalytics/dbt-datadictionary
 Author: Tom Shelley
 Author-email: tom@tasman.ai
 License: GNU GENERAL PUBLIC LICENSE
 Description: # dbt Data Dictionary
         
@@ -16,15 +16,15 @@
         ## **How to Use the Application**
         
         ### **Installation**
         
         1. Install dbt data dictionary using
             
             ```bash
-            pip install dbt-datadictionary
+            pip install dbt-datadict
             ```
             
         
         ### **Command-Line Interface (CLI) Usage**
         
         The Data Dictionary Application provides a command-line interface (CLI) that allows you to interact with the library easily.
         ### Command: `generate`
@@ -32,15 +32,15 @@
         This command generates yaml files using the dbt-codegen package. Where it finds existing model yaml files, it will merge the full column lists. For missing models, it will create a separate model yaml file using the name provided.
         
         **IMPORTANT**: This command will only run in a valid dbt project with dbt-labs/codegen installed.
         
         ### **Usage:**
         
         ```bash
-        $ dbt_datadict generate [-d <DICTIONARY>] [-D <DIRECTORY>]
+        $ datadict generate [-d <DICTIONARY>] [-D <DIRECTORY>]
         ```
         
         ### **Options:**
         
         - `-D, --directory <DIRECTORY>`: Directory to apply the dictionary. Default: 'models/'.
         - `-f, --file <NAME>`: The file to store any new models in.
         - `--sort`: Triggers the generated YAML files to be sorted alphabetically.
@@ -56,15 +56,15 @@
         ### Command: **`apply`**
         
         This command applies data dictionary updates to all model YAML files in the specified directory and its subdirectories.
         
         ### **Usage:**
         
         ```bash
-        $ dbt_datadict apply [-d <DICTIONARY>] [-D <DIRECTORY>]
+        $ datadict apply [-d <DICTIONARY>] [-D <DIRECTORY>]
         ```
         
         ### **Options:**
         
         - **`-d, --dictionary <DICTIONARY>`**: Location of the dictionary file. Default: 'datadictionary.yml'.
         - **`-D, --directory <DIRECTORY>`**: Directory to apply the dictionary. Default: 'models/'.
         
@@ -181,21 +181,25 @@
         
         `python setup.py develop`
         
         Building for distribution
         
         `python setup.py sdist bdist_wheel`
         
-        Pushing the distribution to the test server (changes require upversioning)
+        Pushing the distribution to Test PyPi (changes require upversioning and access)
+        
+        `twine upload --repository testpypi --skip-existing dist/*`
+        
+        Pushing the distribution to Production PyPi (changes require upversioning and access)
         
         `twine upload --repository pypi --skip-existing dist/*`
         
-        Pulling the distribution for use in another project
+        Pulling a test distribution
         
-        `pip install dbt-datadictionary==0.0.12`
+        `pip install --extra-index-url https://test.pypi.org/simple/ dbt-datadictionary==<version>`
         
         ## **Important Note**
         
         It is highly recommend to only use this library in a version controlled environment, such as git. Additionally, please ensure that you have backed up your model YAML files and data dictionary before applying any updates. The application modifies files in place and does not create backups automatically.
         
         Use this application responsibly and verify the updates before proceeding.
 Platform: UNKNOWN
```

### Comparing `dbt-datadict-0.0.1/setup.py` & `dbt-datadict-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name = 'dbt-datadict',
-    version = '0.0.1',
+    version = '0.0.2',
     author = 'Tom Shelley',
     author_email = 'tom@tasman.ai',
     license = 'GNU GENERAL PUBLIC LICENSE',
     description = 'A Python application for automating the application of consistent field definitions to large multi-layered dbt projects',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/TasmanAnalytics/dbt-datadictionary',
```

### Comparing `dbt-datadict-0.0.1/test/test.py` & `dbt-datadict-0.0.2/test/test.py`

 * *Files identical despite different names*

