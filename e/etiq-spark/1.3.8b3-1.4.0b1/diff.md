# Comparing `tmp/etiq_spark-1.3.8b3-cp39-cp39-win_amd64.whl.zip` & `tmp/etiq_spark-1.4.0b1-cp39-cp39-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 347764 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat  1065472 b- defN 23-Apr-27 15:01 etiq/spark.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1238 b- defN 23-Apr-27 15:01 etiq/spark.pyi
--rw-rw-rw-  2.0 fat     2041 b- defN 23-Apr-27 15:01 etiq_spark-1.3.8b3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-27 15:01 etiq_spark-1.3.8b3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-27 15:01 etiq_spark-1.3.8b3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      477 b- defN 23-Apr-27 15:01 etiq_spark-1.3.8b3.dist-info/RECORD
-6 files, 1069327 bytes uncompressed, 346904 bytes compressed:  67.6%
+Zip file size: 473018 bytes, number of entries: 6
+-rw-r--r--  2.0 unx  1495288 b- defN 23-Aug-01 20:15 etiq/spark.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     1280 b- defN 23-Aug-01 20:15 etiq/spark.pyi
+-rw-r--r--  2.0 unx     2029 b- defN 23-Aug-01 20:15 etiq_spark-1.4.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       97 b- defN 23-Aug-01 20:15 etiq_spark-1.4.0b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Aug-01 20:14 etiq_spark-1.4.0b1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      489 b- defN 23-Aug-01 20:15 etiq_spark-1.4.0b1.dist-info/RECORD
+6 files, 1499188 bytes uncompressed, 472134 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: etiq/spark.cp39-win_amd64.pyd
+Filename: etiq/spark.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
 Filename: etiq/spark.pyi
 Comment: 
 
-Filename: etiq_spark-1.3.8b3.dist-info/METADATA
+Filename: etiq_spark-1.4.0b1.dist-info/METADATA
 Comment: 
 
-Filename: etiq_spark-1.3.8b3.dist-info/WHEEL
+Filename: etiq_spark-1.4.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: etiq_spark-1.3.8b3.dist-info/top_level.txt
+Filename: etiq_spark-1.4.0b1.dist-info/top_level.txt
 Comment: 
 
-Filename: etiq_spark-1.3.8b3.dist-info/RECORD
+Filename: etiq_spark-1.4.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## etiq/spark.pyi

```diff
@@ -1,43 +1,48 @@
-# This file was generated by Nuitka and describes the types of the
-# created shared library.
-
-# At this time it lists only the imports made and can be used by the
-# tools that bundle libraries, including Nuitka itself. For instance
-# standalone mode usage of the created library will need it.
-
-# In the future, this will also contain type information for values
-# in the module, so IDEs will use this. Therefore please include it
-# when you make software releases of the extension module that it
-# describes.
-
-import datasets
-import calculation_handlers
-import etiq
-import pyspark.sql.dataframe
-import collections
-import numpy
-import pyspark.sql.functions
-import pyspark.sql.window
-import scipy.stats
-import simple_spark_dataset
-import bias_spark_dataset
-import builders
-import uuid
-import pandas
-import pyspark.sql
-import pyspark.sql.types
-import etiq.licensing
-import etiq.dataprofile
-import etiq.datasets
-import etiq.utils
-import utils
-import base_spark_dataset
-import simple_dataset_builder
-import bias_dataset_builder
-import etiq.biasparams
-import etiq.config
-
-# This is not Python source even if it looks so. Make it clear for
-# now. This was decided by PEP 484 designers.
-__name__ = ...
-
+# This file was generated by Nuitka and describes the types of the
+# created shared library.
+
+# At this time it lists only the imports made and can be used by the
+# tools that bundle libraries, including Nuitka itself. For instance
+# standalone mode usage of the created library will need it.
+
+# In the future, this will also contain type information for values
+# in the module, so IDEs will use this. Therefore please include it
+# when you make software releases of the extension module that it
+# describes.
+
+import etiq
+import pyspark.sql.dataframe
+import calculation_handlers
+import datasets
+import metrics
+import model
+import utils
+import collections
+import numpy
+import scipy
+import etiq.calculation_handlers
+import pyspark.sql.functions
+import pyspark.sql.window
+import simple_spark_dataset
+import bias_spark_dataset
+import builders
+import uuid
+import etiq.licensing
+import pandas
+import etiq.dataprofile
+import etiq.datasets
+import etiq.utils
+import pyspark.sql
+import pyspark.sql.types
+import base_spark_dataset
+import simple_dataset_builder
+import bias_dataset_builder
+import etiq.biasparams
+import etiq.config
+import math
+import etiq.model
+
+# This is not Python source even if it looks so. Make it clear for
+# now. This was decided by PEP 484 designers.
+__name__ = ...
+
```

## Comparing `etiq_spark-1.3.8b3.dist-info/METADATA` & `etiq_spark-1.4.0b1.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,51 @@
-Metadata-Version: 2.1
-Name: etiq-spark
-Version: 1.3.8b3
-Summary: ETIQ.ai ML Testing library
-Home-page: https://etiq.ai/
-Author: ETIQ AI
-Author-email: devops@etiq.ai
-License: UNKNOWN
-Keywords: ai,bias,etiq,fairness
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: MacOS X
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: Framework :: IPython
-Classifier: Framework :: Jupyter
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: Other/Proprietary License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6,<3.11
-Description-Content-Type: text/markdown
-Requires-Dist: etiq (==1.3.8b3)
-Requires-Dist: pyspark
-
-
-# ETIQ AI
-
-Etiq helps companies test and monitor ML models. For data science & ML teams,
-Etiq tests ML algorithms, identifying issues and preventing accuracy loss in
-both building & production stages. Etiq helps identify the following issue
-types in the dataset/model: Bias, Data Leakage, Accuracy Issues, Drift, across
-both pre-production and production stages. Additionally, Etiq helps identify
-which segments are impacted by each issue type and provides modular tests
-that you can plug at different points in your pipeline.
-
-## Getting Started
-
-To get started with this package, view our quickstart guide at
-https://docs.etiq.ai/
-
-
-## Licence
-
-This library is distributed under the Creative Commons "Attribution-NoDerivatives 4.0
-International (CC BY-ND 4.0)":
-
-https://creativecommons.org/licenses/by-nd/4.0/
-
-
+Metadata-Version: 2.1
+Name: etiq-spark
+Version: 1.4.0b1
+Summary: This is an optional, extension to the etiq library to provide spark datasets
+Author-email: ETIQ AI <devops@etiq.ai>
+Project-URL: homepage, https://etiq.ai
+Keywords: ai,bias,etiq,fairness
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: MacOS X
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Framework :: IPython
+Classifier: Framework :: Jupyter
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: <3.12,>=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: etiq (==1.4.0b1)
+Requires-Dist: pyspark[pandas_on_spark] (>=3.3.2)
+
+# ETIQ AI
+
+Etiq helps companies test and monitor ML models. For data science & ML teams,
+Etiq tests ML algorithms, identifying issues and preventing accuracy loss in
+both building & production stages. Etiq helps identify the following issue
+types in the dataset/model: Bias, Data Leakage, Accuracy Issues, Drift, across
+both pre-production and production stages. Additionally, Etiq helps identify
+which segments are impacted by each issue type and provides modular tests
+that you can plug at different points in your pipeline.
+
+## Getting Started
+
+To get started with this package, view our quickstart guide at
+https://docs.etiq.ai/
+
+
+## Licence
+
+This library is distributed under the Creative Commons "Attribution-NoDerivatives 4.0
+International (CC BY-ND 4.0)":
+
+https://creativecommons.org/licenses/by-nd/4.0/
```

