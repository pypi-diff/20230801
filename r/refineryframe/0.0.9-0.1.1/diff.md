# Comparing `tmp/refineryframe-0.0.9.tar.gz` & `tmp/refineryframe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.0.9.tar", last modified: Sun Jul 30 17:35:49 2023, max compression
+gzip compressed data, was "refineryframe-0.1.1.tar", last modified: Tue Aug  1 02:17:43 2023, max compression
```

## Comparing `refineryframe-0.0.9.tar` & `refineryframe-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:35:49.533758 refineryframe-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-30 17:35:36.000000 refineryframe-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-07-30 17:35:49.533758 refineryframe-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18622 2023-07-30 17:35:48.000000 refineryframe-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:35:49.533758 refineryframe-0.0.9/refineryframe/
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-07-30 17:35:36.000000 refineryframe-0.0.9/refineryframe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34997 2023-07-30 17:35:36.000000 refineryframe-0.0.9/refineryframe/detect_unexpected.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-07-30 17:35:36.000000 refineryframe-0.0.9/refineryframe/other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16129 2023-07-30 17:35:36.000000 refineryframe-0.0.9/refineryframe/refiner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-07-30 17:35:36.000000 refineryframe-0.0.9/refineryframe/replace_unexpected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:35:49.533758 refineryframe-0.0.9/refineryframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-07-30 17:35:49.000000 refineryframe-0.0.9/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-30 17:35:49.000000 refineryframe-0.0.9/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 17:35:49.000000 refineryframe-0.0.9/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-30 17:35:49.000000 refineryframe-0.0.9/refineryframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-30 17:35:49.000000 refineryframe-0.0.9/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 17:35:49.533758 refineryframe-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-30 17:35:48.000000 refineryframe-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:35:49.533758 refineryframe-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 17:35:36.000000 refineryframe-0.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-30 17:35:36.000000 refineryframe-0.0.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-07-30 17:35:36.000000 refineryframe-0.0.9/tests/test_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:17:43.741247 refineryframe-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-01 02:17:28.000000 refineryframe-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-08-01 02:17:43.741247 refineryframe-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29623 2023-08-01 02:17:42.000000 refineryframe-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:17:43.737247 refineryframe-0.1.1/refineryframe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-01 02:17:28.000000 refineryframe-0.1.1/refineryframe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34997 2023-08-01 02:17:28.000000 refineryframe-0.1.1/refineryframe/detect_unexpected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-01 02:17:28.000000 refineryframe-0.1.1/refineryframe/other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17760 2023-08-01 02:17:28.000000 refineryframe-0.1.1/refineryframe/refiner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-01 02:17:28.000000 refineryframe-0.1.1/refineryframe/replace_unexpected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:17:43.741247 refineryframe-0.1.1/refineryframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-08-01 02:17:43.000000 refineryframe-0.1.1/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 02:17:43.000000 refineryframe-0.1.1/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:17:43.000000 refineryframe-0.1.1/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 02:17:43.000000 refineryframe-0.1.1/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 02:17:43.000000 refineryframe-0.1.1/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 02:17:43.741247 refineryframe-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-01 02:17:42.000000 refineryframe-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:17:43.741247 refineryframe-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:17:28.000000 refineryframe-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-08-01 02:17:28.000000 refineryframe-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-08-01 02:17:28.000000 refineryframe-0.1.1/tests/test_refiner.py
```

### Comparing `refineryframe-0.0.9/LICENSE` & `refineryframe-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.9/refineryframe/detect_unexpected.py` & `refineryframe-0.1.1/refineryframe/detect_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.9/refineryframe/other.py` & `refineryframe-0.1.1/refineryframe/other.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.9/refineryframe/refiner.py` & `refineryframe-0.1.1/refineryframe/refiner.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,22 +95,25 @@
         logging.basicConfig(level=self.loggerLvl)
         logger = logging.getLogger(self.logger_name)
         logger.setLevel(self.loggerLvl)
 
         self.logger = logger
 
 
-    def shout(self):
+    def shout(self, mess = None) -> None:
 
         """
         Prints a line of text with a specified length and format.
         """
 
+        if mess is None:
+            mess = self.mess
+
         shoutOUT(output_type=self.shout_type,
-                 mess=self.mess,
+                 mess=mess,
                  dotline_length=self.dotline_length,
                  logger=self.logger)
 
     def get_type_dict_from_dataframe(self,
                       explicit=True,
                       stringout=False):
 
@@ -167,89 +170,134 @@
 
         self.dataframe = set_types(dataframe=self.dataframe,
                                   types_dict_str=type_dict,
                                   replace_dict=replace_dict,
                                   expected_date_format=expected_date_format,
                                       logger = self.logger)
 
-    def check_missing_types(self):
+        self.type_dict = type_dict
+
+    def get_refiner_settings(self) -> dict:
+
+        """
+        Extracts values of parameters from refiner and saves them in dictionary for later use.
+        """
+
+        exclude_attributes = ['dataframe',
+                      'MISSING_TYPES_TEST',
+                      'MISSING_COUNT_TEST',
+                      'NUM_INF_TEST',
+                      'DATE_FORMAT_TEST',
+                      'DATE_RANGE_TEST',
+                      'DUPLICATES_TEST',
+                      'COL_NAMES_TYPES_TEST',
+                      'NUMERIC_RANGE_TEST',
+                      'logger',
+                      'duv_score',
+                      'ruv_score0',
+                      'ruv_score1',
+                      'ruv_score2']
+
+        # Getting the dictionary representation of the instance
+        my_instance_dict = attr.asdict(self)
+
+        # Excluding 'exclude_attributes' from the dictionary representation
+        filtered_instance_dict = {key: value for key, value in my_instance_dict.items() if key not in exclude_attributes}
+
+        return filtered_instance_dict
+
+    def set_refiner_settings(self, settings : dict) -> None:
+
+        """
+        Updates input parameters with values from provided settings dict.
+        """
+
+        # Overwrite parameters of the existing instance
+        for key, value in settings.items():
+            setattr(self, key, value)
+
+        # Reinitialize logger
+        self.initialize_logger()
+
+
+    def check_missing_types(self) -> None:
 
         """
         Takes a DataFrame and a dictionary of missing types as input,
         and searches for any instances of these missing types in each column of the DataFrame.
 
         If any instances are found, a warning message is logged containing the column name,
         the missing value, and the count of missing values found.
         """
 
         self.MISSING_TYPES_TEST = check_missing_types(dataframe = self.dataframe,
                                                         MISSING_TYPES = self.MISSING_TYPES,
                                                         independent = True,
                                       logger = self.logger)
 
-    def check_missing_values(self):
+    def check_missing_values(self) -> None:
 
         """
         Counts the number of NaN, None, and NaT values in each column of a pandas DataFrame.
         """
 
         self.MISSING_COUNT_TEST = check_missing_values(dataframe = self.dataframe,
                                       logger = self.logger)
 
-    def check_inf_values(self):
+    def check_inf_values(self) -> None:
 
         """
         Counts the inf values in each column of a pandas DataFrame.
         """
 
         self.NUM_INF_TEST = check_inf_values(dataframe = self.dataframe,
                                              independent = True,
                                              logger = self.logger)
 
-    def check_date_format(self):
+    def check_date_format(self) -> None:
 
         """
         Checks if the values in the datetime columns of the input dataframe
         have the expected 'YYYY-MM-DD' format.
         """
 
         self.DATE_FORMAT_TEST = check_date_format(dataframe = self.dataframe,
                                                   expected_date_format = self.expected_date_format,
                                                   independent = True,
                                                   logger = self.logger)
 
     def check_duplicates(self,
-                         subset = None):
+                         subset = None) -> None:
 
         """
         Checks for duplicates in a pandas DataFrame.
         """
 
         self.DUPLICATES_TEST = check_duplicates(dataframe = self.dataframe,
                                                  subset = subset,
                                                  independent = True,
                                                  logger = self.logger)
 
-    def check_col_names_types(self):
+    def check_col_names_types(self) -> None:
 
         """
         Checks if a given dataframe has the same column names as keys in a given dictionary
         and those columns have the same types as items in the dictionary.
         """
 
         self.COL_NAMES_TYPES_TEST = check_col_names_types(dataframe = self.dataframe,
                           types_dict_str = self.type_dict,
                           independent = True,
                                       logger = self.logger)
 
     def check_numeric_range(self,
-                            numeric_cols = None,
+                            numeric_cols : list = None,
                             lower_bound = None,
                             upper_bound = None,
-                            ignore_values = None):
+                            ignore_values = None) -> None:
 
         """
         Checks if numeric values are in expected ranges.
         """
 
         if lower_bound is None:
             lower_bound = self.lower_bound
@@ -265,15 +313,15 @@
                                                       independent = True,
                                                       ignore_values = ignore_values,
                                                       logger = self.logger)
 
     def check_date_range(self,
                         earliest_date = None,
                         latest_date = None,
-                        ignore_dates = None):
+                        ignore_dates = None) -> None:
 
         """
         Checks if dates are in expected ranges.
         """
 
         if earliest_date is None:
             earliest_date = self.earliest_date
@@ -297,15 +345,15 @@
                                  TEST_DUV_FLAGS_PATH = None,
                                  types_dict_str = None,
                                  expected_date_format = None,
                                  earliest_date = None,
                                  latest_date = None,
                                  numeric_lower_bound = None,
                                  numeric_upper_bound = None,
-                                 print_score = True):
+                                 print_score = True) -> None:
 
         """
         Detects unexpected values in a pandas DataFrame.
         """
 
         if MISSING_TYPES is None:
             MISSING_TYPES = self.MISSING_TYPES
@@ -345,15 +393,15 @@
                              MISSING_TYPES = None,
                              unexpected_exceptions = None,
                              unexpected_conditions = None,
                              TEST_RUV_FLAGS_PATH = None,
                              earliest_date = None,
                              latest_date = None,
                              numeric_lower_bound = None,
-                             numeric_upper_bound = None):
+                             numeric_upper_bound = None) -> None:
 
         """
         Replaces unexpected values in a pandas DataFrame with missing types.
         """
 
         if MISSING_TYPES is None:
             MISSING_TYPES = self.MISSING_TYPES
```

### Comparing `refineryframe-0.0.9/refineryframe/replace_unexpected.py` & `refineryframe-0.1.1/refineryframe/replace_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.9/setup.py` & `refineryframe-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "attrs>=22.2.0",
     "datetime",
     "pandas",
     "numpy",
     "unidecode"
 ]
 
-VERSION = '0.0.9'
+VERSION = '0.1.1'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them according to set of predefined rules'
 
 # Setting up
 setup(
     name="refineryframe",
     #use_scm_version=True,
@@ -29,15 +29,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=base_packages,
     keywords=['python', 'data cleaning', 'safeguards'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
```

### Comparing `refineryframe-0.0.9/tests/conftest.py` & `refineryframe-0.1.1/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -100,14 +100,71 @@
     "duplicates": "ALL",
     "date_range": "NONE",
     "numeric_range": "NONE"
 }
 
     yield unexpected_exceptions
 
+@pytest.fixture(scope='session')
+def unexpected_exceptions2():
+
+    unexpected_exceptions2 = {
+    "col_names_types": "NONE",
+    "missing_values": "ALL",
+    "missing_types": "ALL",
+    "inf_values": "NONE",
+    "date_format": "NONE",
+    "duplicates": "ALL",
+    "date_range": "NONE",
+    "numeric_range": "ALL"
+}
+
+    yield unexpected_exceptions2
+
+
+@pytest.fixture(scope='session')
+def refiner_settings():
+
+    refiner_settings = {'replace_dict': {-996: -999, '1000-01-09': '1850-01-09'},
+                        'MISSING_TYPES': {'date_not_delivered': '1850-01-09',
+                        'numeric_not_delivered': -999,
+                        'character_not_delivered': 'missing'},
+                        'expected_date_format': '%Y-%m-%d',
+                        'mess': 'INITIAL PREPROCESSING',
+                        'shout_type': 'HEAD2',
+                        'logger_name': 'Refiner',
+                        'loggerLvl': 10,
+                        'dotline_length': 50,
+                        'lower_bound': -np.inf,
+                        'upper_bound': np.inf,
+                        'earliest_date': '1900-08-25',
+                        'latest_date': '2100-01-01',
+                        'unexpected_exceptions_duv': {'col_names_types': 'NONE',
+                        'missing_values': 'ALL',
+                        'missing_types': 'ALL',
+                        'inf_values': 'NONE',
+                        'date_format': 'NONE',
+                        'duplicates': 'ALL',
+                        'date_range': 'NONE',
+                        'numeric_range': 'ALL'},
+                        'unexpected_exceptions_ruv': {'irregular_values': 'NONE',
+                        'date_range': 'NONE',
+                        'numeric_range': 'NONE',
+                        'capitalization': 'NONE',
+                        'unicode_character': 'NONE'},
+                        'unexpected_conditions': None,
+                        'ignore_values': [],
+                        'ignore_dates': [],
+                        'type_dict': {}}
+
+    yield refiner_settings
+
+
+
+
 
 @pytest.fixture(scope='session')
 def types_dict_str():
 
     types_dict_str = {'num_id' : 'int64',
                    'NumericColumn' : 'float64',
                    'NumericColumn_exepted' : 'float64',
@@ -136,14 +193,24 @@
               replace_dict = replace_dict,
               loggerLvl = logging.DEBUG,
               unexpected_exceptions_duv = unexpected_exceptions)
 
     yield tns
 
 @pytest.fixture(scope='session')
+def tns2(df,replace_dict,unexpected_exceptions2):
+
+    tns = Refiner(dataframe = df,
+              replace_dict = replace_dict,
+              loggerLvl = logging.DEBUG,
+              unexpected_exceptions_duv = unexpected_exceptions2)
+
+    yield tns
+
+@pytest.fixture(scope='session')
 def unexpected_conditions():
 
     unexpected_conditions = {
     '1': {
         'description': 'Replace numeric missing with with zero',
         'group': 'regex_columns',
         'features': r'^Numeric',
```

### Comparing `refineryframe-0.0.9/tests/test_refiner.py` & `refineryframe-0.1.1/tests/test_refiner.py`

 * *Files 13% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     assert "checking for presense of inf values in numeric colums" in caplog.text
     assert "checking expected numeric range" in caplog.text
 
     assert "Replace numeric missing with with zero" in caplog.text
     assert "Replace numeric missing with with zero :: 1" in caplog.text
     assert "Detect/Replace numeric values in certain column with zeros if > 2" in caplog.text
     assert "Detect/Replace numeric values in certain column with zeros if > 2 :: 2" in caplog.text
-    assert "Percentage of passed tests: 75.00%" in caplog.text
+    assert "Percentage of passed tests: 66.67%" in caplog.text
 
 
 def test_replace_unexpected_with_conds(tns,df2, unexpected_conditions, caplog):
 
     tns.replace_unexpected_values(unexpected_conditions = unexpected_conditions)
 
     assert "replacing missing values in category cols with missing types" in caplog.text
@@ -195,14 +195,33 @@
     assert "Usable values in the dataframe:  82.22%" in caplog.text
     assert "Uncorrected data quality score:  88.89%" in caplog.text
     assert "Corrected data quality score:  97.53%" in caplog.text
 
     assert tns.dataframe.equals(df2)
 
 
+def test_get_refiner_settings(tns2,refiner_settings):
+
+    refiner_settings2 = tns2.get_refiner_settings()
+
+    assert refiner_settings2 == refiner_settings
+
+def test_set_refiner_settings(tns2,df, refiner_settings):
+
+    tns = Refiner(dataframe = df)
+
+    tns.set_refiner_settings(refiner_settings)
+
+    tns.shout(mess = "TNS1")
+    tns.detect_unexpected_values()
+    tns2.shout(mess = "TNS2")
+    tns2.detect_unexpected_values()
+
+    assert tns.duv_score == tns2.duv_score
+
 
 #     @pytest.mark.parametrize("a,expected", [
 #     (2, 4),
 #     (6, 8)
 # ])
 # def test_my_function2(a,expected):
```

