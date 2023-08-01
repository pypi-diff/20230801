# Comparing `tmp/moderne_visualizations_misc-0.1.3.tar.gz` & `tmp/moderne_visualizations_misc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moderne_visualizations_misc-0.1.3.tar", last modified: Mon Jul 31 16:00:36 2023, max compression
+gzip compressed data, was "moderne_visualizations_misc-0.1.5.tar", last modified: Tue Aug  1 02:14:35 2023, max compression
```

## Comparing `moderne_visualizations_misc-0.1.3.tar` & `moderne_visualizations_misc-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:00:36.448368 moderne_visualizations_misc-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 16:00:36.444368 moderne_visualizations_misc-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:00:36.444368 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/dependency_vulnerabilities.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:00:36.444368 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    31410 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/language_composition.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/parse_failure_analysis.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    24871 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/sql_crud.300.png
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/language_composition.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/parse_failure_analysis.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:00:36.444368 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/language_composition.yml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/parse_failure_analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/sql_crud.yml
--rw-r--r--   0 runner    (1001) docker     (123)   152398 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/sql_crud.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:00:36.444368 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 16:00:36.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-31 16:00:36.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:00:36.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 16:00:36.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 16:00:36.000000 moderne_visualizations_misc-0.1.3/moderne_visualizations_misc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-31 16:00:04.000000 moderne_visualizations_misc-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:00:36.448368 moderne_visualizations_misc-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:35.958880 moderne_visualizations_misc-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-01 02:14:35.958880 moderne_visualizations_misc-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:35.958880 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/cobol_find_copy_book.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/dependency_vulnerabilities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/find_methods.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:35.958880 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/images/cobol_find_copy_book.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31410 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/images/language_composition.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/images/parse_failure_analysis.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24871 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/images/sql_crud.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/language_composition.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/parse_failure_analysis.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:35.958880 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/specs/cobol_find_copy_book.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/specs/find_methods.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/specs/language_composition.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/specs/parse_failure_analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/specs/sql_crud.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   152398 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/sql_crud.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:35.958880 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-01 02:14:35.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-01 02:14:35.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:14:35.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 02:14:35.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 02:14:35.000000 moderne_visualizations_misc-0.1.5/moderne_visualizations_misc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-01 02:14:19.000000 moderne_visualizations_misc-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 02:14:35.958880 moderne_visualizations_misc-0.1.5/setup.cfg
```

### Comparing `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/dependency_vulnerabilities.ipynb` & `moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/dependency_vulnerabilities.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png` & `moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/language_composition.300.png` & `moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/images/language_composition.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/parse_failure_analysis.300.png` & `moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/images/parse_failure_analysis.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/images/sql_crud.300.png` & `moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/images/sql_crud.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/language_composition.ipynb` & `moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/language_composition.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9633928571428572%*

 * *Differences: {"'cells'": "{3: {'source': []}, insert: [(2, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', 1), ('metadata', OrderedDict()), ('outputs', "*

 * *            '[OrderedDict([(\'ename\', \'ModuleNotFoundError\'), (\'evalue\', "No module named '*

 * *            '\'plotly\'"), (\'output_type\', \'error\'), (\'traceback\', '*

 * *            "['\\x1b[1;31m---------------------------------------------------------------------------\\x1b[0m', "*

 * *            "'\\x1b[1;31mModuleNotFoundError\\x1b[0m           […]*

```diff
@@ -12,17 +12,29 @@
             "metadata": {},
             "source": [
                 "This report shows the different languages that are used in the projects."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "ename": "ModuleNotFoundError",
+                    "evalue": "No module named 'plotly'",
+                    "output_type": "error",
+                    "traceback": [
+                        "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
+                        "\u001b[1;31mModuleNotFoundError\u001b[0m                       Traceback (most recent call last)",
+                        "Cell \u001b[1;32mIn[1], line 1\u001b[0m\n\u001b[1;32m----> 1\u001b[0m \u001b[38;5;28;01mimport\u001b[39;00m \u001b[38;5;21;01mplotly\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mexpress\u001b[39;00m \u001b[38;5;28;01mas\u001b[39;00m \u001b[38;5;21;01mpx\u001b[39;00m\n\u001b[0;32m      2\u001b[0m \u001b[38;5;28;01mimport\u001b[39;00m \u001b[38;5;21;01mpandas\u001b[39;00m \u001b[38;5;28;01mas\u001b[39;00m \u001b[38;5;21;01mpd\u001b[39;00m\n\u001b[0;32m      3\u001b[0m \u001b[38;5;28;01mimport\u001b[39;00m \u001b[38;5;21;01mwarnings\u001b[39;00m\n",
+                        "\u001b[1;31mModuleNotFoundError\u001b[0m: No module named 'plotly'"
+                    ]
+                }
+            ],
             "source": [
                 "import plotly.express as px\n",
                 "import pandas as pd\n",
                 "import warnings\n",
                 "import moderne_pkg.helpers as helpers\n",
                 "\n",
                 "warnings.simplefilter(\"ignore\")\n",
@@ -107,14 +119,21 @@
                 "    )\n",
                 "\n",
                 "    fig.data[0].textinfo = 'label+text+value'\n",
                 "\n",
                 "    # Output the visualization\n",
                 "    fig.show(render='plotly_mimetype')"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -125,13 +144,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.10.4"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/parse_failure_analysis.ipynb` & `moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/parse_failure_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml` & `moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/specs/parse_failure_analysis.yml` & `moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/specs/parse_failure_analysis.yml`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.3/moderne_visualizations_misc/sql_crud.ipynb` & `moderne_visualizations_misc-0.1.5/moderne_visualizations_misc/sql_crud.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.3/pyproject.toml` & `moderne_visualizations_misc-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # @see https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "moderne_visualizations_misc"
-version = "0.1.3"
+version = "0.1.5"
 description = "Miscellaneous visualizations for the Moderne platform"
 authors = [
     { name = "Jonathan Schneider", email = "jonathan@moderne.io" },
     { name = "Kyle Scully", email = "kyle@moderne.io" }
 ]
 license = { text = "Apache-2.0" }
 dependencies = [
     "pandas==2.0.3",
     "ipython==8.13.0",
-    "code_data_science==1.1.4"
+    "code_data_science==1.1.4",
+    "graphviz==0.20.1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/moderneinc/visualizations-misc"
 
 [tool.setuptools.packages.find]
 include = [
```

