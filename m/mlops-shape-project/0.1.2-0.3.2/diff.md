# Comparing `tmp/mlops_shape_project-0.1.2.tar.gz` & `tmp/mlops_shape_project-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_shape_project-0.1.2.tar", max compression
+gzip compressed data, was "mlops_shape_project-0.3.2.tar", max compression
```

## Comparing `mlops_shape_project-0.1.2.tar` & `mlops_shape_project-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       23 2023-07-31 05:01:46.969290 mlops_shape_project-0.1.2/mlops_shape_project/__init__.py
--rw-r--r--   0        0        0     1375 2023-07-31 04:49:17.779008 mlops_shape_project-0.1.2/mlops_shape_project/app.py
--rw-r--r--   0        0        0     3218 2023-07-31 22:02:11.147467 mlops_shape_project-0.1.2/mlops_shape_project/data_loader.py
--rw-r--r--   0        0        0     3478 2023-07-31 03:32:55.063354 mlops_shape_project-0.1.2/mlops_shape_project/dataframe_checker.py
--rw-r--r--   0        0        0     2213 2023-07-31 05:56:11.704527 mlops_shape_project-0.1.2/mlops_shape_project/feature_engineering_predict.py
--rw-r--r--   0        0        0     4060 2023-07-31 03:56:56.781253 mlops_shape_project-0.1.2/mlops_shape_project/pipeline_utils.py
--rw-r--r--   0        0        0     1766 2023-08-01 03:36:08.277292 mlops_shape_project-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    10974 2023-08-01 03:33:48.518911 mlops_shape_project-0.1.2/README.md
--rw-r--r--   0        0        0    12010 1970-01-01 00:00:00.000000 mlops_shape_project-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-07-31 05:01:46.969290 mlops_shape_project-0.3.2/mlops_shape_project/__init__.py
+-rw-r--r--   0        0        0     3321 2023-08-01 20:10:40.315249 mlops_shape_project-0.3.2/mlops_shape_project/data_loader.py
+-rw-r--r--   0        0        0     5414 2023-08-01 18:19:03.147549 mlops_shape_project-0.3.2/mlops_shape_project/dataframe_checker.py
+-rw-r--r--   0        0        0     2228 2023-08-01 15:09:35.748418 mlops_shape_project-0.3.2/mlops_shape_project/feature_engineering_predict.py
+-rw-r--r--   0        0        0     8265 2023-08-01 20:51:04.966161 mlops_shape_project-0.3.2/mlops_shape_project/main.py
+-rw-r--r--   0        0        0     4125 2023-08-01 15:09:35.764416 mlops_shape_project-0.3.2/mlops_shape_project/pipeline_utils.py
+-rw-r--r--   0        0        0      411 2023-08-01 20:51:04.704564 mlops_shape_project-0.3.2/mlops_shape_project/shape.py
+-rw-r--r--   0        0        0     1996 2023-08-01 20:52:40.455764 mlops_shape_project-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    13089 2023-08-01 20:49:12.989467 mlops_shape_project-0.3.2/README.md
+-rw-r--r--   0        0        0    14222 1970-01-01 00:00:00.000000 mlops_shape_project-0.3.2/PKG-INFO
```

### Comparing `mlops_shape_project-0.1.2/mlops_shape_project/data_loader.py` & `mlops_shape_project-0.3.2/mlops_shape_project/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional, Type
+
 import pandas as pd
 
 
 class DataLoader:
     """
     Utility class for loading datasets into pandas DataFrames.
 
@@ -14,15 +16,15 @@
     to read the file into a DataFrame, detecting or using a specified format.
 
     Usage:
         data_df = DataLoader.read_data_dataframe('path_to_file.csv')
     """
 
     @staticmethod
-    def detect_sep(data_path):
+    def detect_sep(data_path: str) -> str:
         """
         Detect the delimiter used in a file, specifically targeting CSV-like files.
 
         The function checks for common delimiters such as semicolon (;) and comma (,).
         It reads the first line of the file and identifies the delimiter based on its presence.
 
         Args:
@@ -44,15 +46,17 @@
             return ','
         else:
             raise ValueError(
                 'Delimiter not detected. The file may be in an unsupported format.'
             )
 
     @staticmethod
-    def read_data_dataframe(data_path, format=None):
+    def read_data_dataframe(
+        data_path: str, format: Optional[str] = None
+    ) -> pd.DataFrame:
         """
         Read data from the given path into a pandas DataFrame based on the specified format.
 
         This function aims to detect and read various file formats into a pandas DataFrame.
         If the format is not explicitly provided, it infers the format from the file extension.
 
         Args:
```

### Comparing `mlops_shape_project-0.1.2/mlops_shape_project/dataframe_checker.py` & `mlops_shape_project-0.3.2/mlops_shape_project/dataframe_checker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,71 @@
+import datetime
+from typing import Type
+
 import numpy as np
 import pandas as pd
 
 
 class DataFrameChecker:
-    """Class responsible for checking, transforming, and validating DataFrames."""
+    """
+    Class for ensuring the validity and consistency of a pandas DataFrame, primarily tailored for
+    vibration data. It offers various methods to check and transform the DataFrame to meet specific criteria.
+
+    Attributes:
+        dataframe (pd.DataFrame): Input DataFrame to be checked and transformed.
+
+    Methods:
+        check_empty_dataframe: Asserts if the DataFrame is non-empty.
+        fill_na_and_drop: Fills null values with zeros and optionally drops the 'time' column.
+        check_expected_columns: Ensures the presence of specific columns in the DataFrame.
+        check_positive_values: Validates that all values in the DataFrame are non-negative.
+        check_datatype_float: Confirms that all columns are of float datatype.
+        get_dataframe: Returns the processed DataFrame.
+        pipeline_checker: A convenience method that applies a sequence of checks and transformations.
+        _log_failure: Logs exceptions to a specified file.
+    """
 
-    def __init__(self, dataframe):
+    def __init__(self, dataframe) -> None:
         """
         Initializes the DataFrameChecker with a pandas DataFrame.
 
         Args:
             dataframe (pd.DataFrame): The input pandas DataFrame to be checked and transformed.
         """
         self.dataframe = dataframe
 
-    def check_empty_dataframe(self):
+    def check_empty_dataframe(self) -> 'DataFrameChecker':
         """
         Check if the DataFrame is empty.
 
         Raises:
             ValueError: If the DataFrame is empty.
 
         Returns:
             DataFrameChecker: Returns self to allow method chaining.
         """
         if self.dataframe.empty:
             raise ValueError('The DataFrame is empty!')
+            _log_failure(e)
         return self
 
-    def fill_na_and_drop(self):
+    def fill_na_and_drop(self) -> 'DataFrameChecker':
         """
         Fill null values with zero.
 
         Returns:
             DataFrameChecker: Returns self to allow method chaining.
         """
         self.dataframe = self.dataframe.fillna(0)
 
         if 'time' in self.dataframe.columns:
             self.dataframe.drop(columns=['time'], inplace=True)
         return self
 
-    def check_expected_columns(self):
+    def check_expected_columns(self) -> 'DataFrameChecker':
         """
         Verify the DataFrame contains the expected columns.
 
         Raises:
             ValueError: If any expected column is missing.
 
         Returns:
@@ -54,62 +74,90 @@
         expected_columns = ['vibration_x', 'vibration_y', 'vibration_z']
         existing_columns = self.dataframe.columns
         for col in expected_columns:
             if col not in existing_columns:
                 raise ValueError(f"Expected column '{col}' not found!")
         return self
 
-    def check_positive_values(self):
+    def check_positive_values(self) -> 'DataFrameChecker':
         """
         Check if all columns have only positive values.
 
         Raises:
             ValueError: If any column contains negative values.
 
         Returns:
             DataFrameChecker: Returns self to allow method chaining.
         """
         if (self.dataframe < 0).any().any():
             raise ValueError('The DataFrame contains negative values!')
+            _log_failure(e)
         return self
 
-    def check_datatype_float(self):
+    def check_datatype_float(self) -> 'DataFrameChecker':
         """
         Validate the datatype of all columns to ensure they are float.
 
         Raises:
             ValueError: If any column doesn't have a float datatype.
 
         Returns:
             DataFrameChecker: Returns self to allow method chaining.
         """
         for column in self.dataframe.columns:
             if self.dataframe[column].dtype != np.float64:
                 raise ValueError(
                     f'Column {column} does not have float datatype!'
                 )
+                _log_failure(e)
         return self
 
-    def get_dataframe(self):
+    def get_dataframe(self) -> pd.DataFrame:
         """
         Get the processed pandas DataFrame.
 
         Returns:
             pd.DataFrame: The validated and transformed pandas DataFrame.
         """
         return self.dataframe
 
-    def pipeline_checker(self):
+    def pipeline_checker(self) -> pd.DataFrame:
         """
         Execute a series of checks and transformations on the DataFrame.
 
         Returns:
             pd.DataFrame: The validated and transformed pandas DataFrame.
         """
 
         self.check_empty_dataframe()
         self.fill_na_and_drop()
         self.check_expected_columns()
         self.check_positive_values()
         self.check_datatype_float()
 
         return self.get_dataframe()
+
+    def _log_failure(e):
+        """
+        Log the exception to a failure log file.
+
+        This function writes details of the provided exception 'e' to a
+        file named 'failure.log' located in the 'logs' directory. If the file
+        or directory does not exist, it will be created.
+
+        Parameters:
+        - e (Exception): The exception instance to be logged.
+
+        Returns:
+        None
+
+        Example:
+        >>> try:
+        ...     1/0
+        ... except Exception as ex:
+        ...     _log_failure(ex)
+        """
+
+        LOG_DUMP_PATH = 'logs/failure.log'
+
+        with open(LOG_DUMP_PATH, 'a') as fLog:
+            fLog.write(f'{datetime.datetime.now()} - Failure: {str(e)}\n')
```

### Comparing `mlops_shape_project-0.1.2/mlops_shape_project/feature_engineering_predict.py` & `mlops_shape_project-0.3.2/mlops_shape_project/feature_engineering_predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,47 @@
+from typing import Optional, Union
+
 from mlops_shape_project.pipeline_utils import PipelineCreator
 
 
 class FeatureEngPredict:
     """
     A class responsible for processing a dataframe using a provided transformation pipeline
-    and a partial pipeline creator to obtain predictions of model OneClassSVM 
+    and a partial pipeline creator to obtain predictions of model OneClassSVM
 
     Attributes:
         pipeline_transform (Pipeline): The transformation pipeline to process the data.
         partial_pipeline_creator (Any): The utility to create a partial pipeline based on the transformation pipeline.
 
     Methods:
         process_dataframe(dataframe_input: pd.DataFrame, pipeline_transform: Pipeline) -> Tuple[np.array, pd.DataFrame]:
             Processes the input dataframe and returns the model's predictions along with the updated dataframe.
     """
+
     def __init__(self, pipeline_transform, partial_pipeline_creator):
-        
+
         self.pipeline_transform = pipeline_transform
         self.partial_pipeline_creator = partial_pipeline_creator
 
     def process_dataframe(dataframe_input, pipeline_transform):
-        
+
         """
         Processes the input dataframe using the transformation pipeline and returns the model's predictions
         along with an updated dataframe containing these predictions.
 
         Args:
             dataframe_input (pd.DataFrame): The input dataframe to process.
             pipeline_transform (Pipeline): The transformation pipeline to process the data.
 
         Returns:
             tuple:
                 - model_predict (np.array): The predictions of the model.
                 - dataframe_output (pd.DataFrame): The updated dataframe containing the predictions.
         """
-        
+
         feature_engineering_pipe = PipelineCreator.create_partial_pipeline(
             pipeline_transform
         )
         dataframe_feature_engineering = feature_engineering_pipe.fit_transform(
             dataframe_input
         )
```

### Comparing `mlops_shape_project-0.1.2/mlops_shape_project/pipeline_utils.py` & `mlops_shape_project-0.3.2/mlops_shape_project/pipeline_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import pickle
+from typing import Union
 
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import (
     PolynomialFeatures,
     QuantileTransformer,
     StandardScaler,
 )
@@ -32,15 +33,15 @@
         Pipeline: A scikit-learn pipeline based on the provided configuration.
 
     Usage:
         pipeline = PipelineCreator.create_pipeline_from_file('path_to_config.jsonc')
     """
 
     @staticmethod
-    def create_pipeline_from_file(jsonc_file_path):
+    def create_pipeline_from_file(jsonc_file_path: str) -> Pipeline:
         """
         Create a scikit-learn pipeline from a configuration file.
 
         This function constructs a pipeline by reading a JSONC formatted configuration file.
         The configuration file specifies preprocessing steps and model settings in the order
         they should appear in the pipeline. Supported steps include dimension reduction, quantile
         transformation, polynomial feature generation, and standard scaling. The model is loaded
@@ -98,12 +99,12 @@
             else:
                 raise ValueError(f'Unknown step: {step_name}')
 
             pipeline_steps.append(step)
 
         return Pipeline(pipeline_steps)
 
-    def create_partial_pipeline(pipeline):
+    def create_partial_pipeline(pipeline: Pipeline) -> Pipeline:
         # Remove a última etapa se for o modelo
         if 'model' == pipeline.steps[-1][0]:
             return Pipeline(pipeline.steps[:-1])
         return pipeline
```

### Comparing `mlops_shape_project-0.1.2/pyproject.toml` & `mlops_shape_project-0.3.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlops-shape-project"
-version = "0.1.2"
+version = "0.3.2"
 description = "This project was initiated as part of Shape's Hard Skill Test for the Machine Learning Engineer role. The core objective was to take an initial script named `job_test_challenge.py` and transform it into a more organized 📐, maintainable 🛠️, and production-ready codebase."
 license = "MIT"
 authors = ["Junior Torres <galas.apps@gmail.com>"]
 readme = "README.md"
 packages = [{include = "mlops_shape_project"}]
 classifiers = [
     "Programming Language :: Python :: 3.8",
@@ -18,14 +18,18 @@
 "Documentation" = "https://mlops-shape-project.readthedocs.io/en/latest/"
 "Code" = "https://github.com/JuniorTorresMTJ/mlops_shape_project"
 
 [tool.poetry.dependencies]
 python = "^3.8.10"
 scikit-learn = "1.0.2"
 pyarrow = "^12.0.1"
+fastapi = {extras = ["all"], version = "^0.100.1"}
+uvicorn = "^0.23.2"
+pydantic = "^2.1.1"
+python-multipart = "^0.0.6"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 blue = "^0.9.1"
 isort = "^5.12.0"
 taskipy = "^1.11.0"
@@ -53,8 +57,10 @@
 [tool.taskipy.tasks]
 lint = "blue --check --diff . && isort --check --diff ."
 doc = "mkdocs serve"
 pre_test = "task lint"
 test = "pytest -s -x --cov=mlops_shape_project -vv"
 post_test = "coverate html"
 
-
+[tool.poetry.scripts]
+#run-main = "mlops_shape_project.main:main"
+run-app = "mlops_shape_project.app:app"
```

### Comparing `mlops_shape_project-0.1.2/README.md` & `mlops_shape_project-0.3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 -   Intricate or time-intensive modifications, if not instantly implementable, should be signposted within the code as TODOs. These markers should also sketch out the strategic approach intended for their eventual fulfillment 🕰️.
 
 
 ## 🚀 **Run the project**
 ***
 The provided configuration appears to be from a `pyproject.toml` file, which is a configuration file for the [Poetry](https://python-poetry.org/) dependency management and packaging tool in Python. To install and execute this project, follow the steps below:
 
+- Prerequisites:
+- Docker
+- Poetry
+- Python
+
 ### 1️⃣ Install Poetry:
 If you haven't installed Poetry yet, you can do so with the following command:
 
 ```bash
 curl -sSL https://install.python-poetry.org | python3 -
 ```
 
@@ -64,53 +69,132 @@
 ### 4️⃣ Activate the virtual environment:
 Poetry creates a virtual environment for your project. Activate it with:
 
 ```bash
 poetry shell
 ```
 
-### 5️⃣ Run the project:
+### 5️⃣ Build the Docker image:
 The exact command to run the project depends on its structure. Typically, there's a main Python script or module you'd execute to start the project. If there's a clear entry point, you can run:
 
 
 ```bash
-python mlops_shape_project\app.py
+docker build -t mlops-shape-project:latest .
 ```
 
+### 6️⃣ Build the Docker image:
+
+```bash
+docker run -p 8000:8000 mlops-shape-project:latest
+```
+API should now be running and accessible at http://localhost:8000.
 
-### 6️⃣ Additional tasks:
+###  Additional tasks:
 The provided configuration also contains some tasks defined with `taskipy`. You can run these tasks using the `poetry run task` command. For example:
 
 - To run the lint task: 
 
 ```bash
   poetry run task lint
 ```
 
 - To serve the documentation:
 
 ```bash
   poetry run task doc
 ```
 
-### 7️⃣ Expected Model Results:
-When evaluating the performance and predictions of our model, we often look at two key components:
+### 7️⃣ Endpoints:
+
+
+#### ✅ GET /data
 
-#### ✅ Expected Class Labels:
+-   Purpose:
+
+    -   This endpoint retrieves the original dataset from a predefined file location.
+-   Usage:
+
+    -   You simply send a GET request to this endpoint without any parameters.
+-   Example with `curl`:
+
+```bash
+    curl -X 'GET' http://localhost:8000/data
+```
+-   Response:
+
+![data](assets\img\data.png)
+
+If successful, you'll receive a JSON representation of the dataset. The structure will be a dictionary with columns as keys and their associated data as corresponding values.
+
+* * * * *
+
+#### ✅ POST /process_data
+
+-   Purpose:
+
+    -   Processes data from an uploaded file and returns the processed output.
+-   Usage:
+
+    -   Send a POST request to this endpoint with an attached file containing the data you want to process.
+-   Example with `curl`:
+
+```bash
+    curl -X 'POST' -F 'file=@path_to_your_file.csv' http://localhost:8000/process_data
+```
+-   Response:
 
-Class labels serve as numerical representations of the expected predictions or classifications from the model. In this context, the class labels can either be -1 or 1. These values might represent two distinct classes or categories in a binary classification scenario.
+![predict_path](assets\img\predict_path.png)
+
+If successful, you'll receive processed data (like predictions) as a JSON response.
+
+
+
+#### ✅ POST /predict
+
+-   Purpose:
+
+    -   This endpoint takes input data in the form of a JSON object and returns a prediction based on the provided data.
+-   Usage:
+
+    -   Send a POST request with a JSON payload representing the data for which you want a prediction.
+-   Example with `curl`:
+
+```bash
+    `curl -X 'POST' -H "Content-Type: application/json" -d '{"column1": "value1", "column2": "value2", ...}' http://localhost:8000/predict`
+```
+-   Response:
+
+![predict](assets\img\predict.png)
+
+If successful, you'll receive a JSON response with the prediction status and the predicted class.
+
+* * * * *
+
+#### ✅ POST /predict_batch
+
+-   Purpose:
+
+    -   Provides batch predictions based on the provided data.
+-   Usage:
+
+    -   Send a POST request with a JSON payload containing multiple rows of data for batch processing.
+-   Example with `curl`:
+
+```bash
+    curl -X 'POST' -H "Content-Type: application/json" -d '[{"column1": "value1_1", "column2": "value1_2", ...}, {"column1": "value2_1", "column2": "value2_2", ...}, ...]' http://localhost:8000/predict_batch
+```
+-   Response:
 
-![Array-output](assets\img\Output.png)
+![predict_batch](assets\img\predict_batch.png)
 
+ If successful, you'll receive a JSON response with the prediction status and the predicted classes for each input data row.
 
-#### ✅ Model Prediction DataFrame:
 
-Beyond the direct class labels, there is also a DataFrame compiled with the model's predictions. Specifically, this DataFrame contains a column named svm_predict, which displays the predicted class labels for each data instance.
+For each of the endpoints, if there's an error, the API will return a clear message indicating what went wrong, along with a status code indicating the nature of the error. Always make sure to check the returned message and status code to understand any issues.
 
-![Dataframe-output](assets\img\Output2.png)
 
 ## 📖 **Documentation**:
 
 The documentation of this project is an essential component for understanding its structure, functionalities, and usage guides. We strongly believe that comprehensive documentation can speed up the adoption, contribution, and debugging processes of the project. The documentation was crafted using [MkDocs](https://www.mkdocs.org/), a swift and straightforward tool for creating documentation websites from markdown files. It allows us to concentrate on the content while automating the process of converting Markdown into a structured and styled website.
 
 ⚠️[Documentation Link](https://mlops-shape-project.readthedocs.io/en/latest/)⚠️
```

### Comparing `mlops_shape_project-0.1.2/PKG-INFO` & `mlops_shape_project-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops-shape-project
-Version: 0.1.2
+Version: 0.3.2
 Summary: This project was initiated as part of Shape's Hard Skill Test for the Machine Learning Engineer role. The core objective was to take an initial script named `job_test_challenge.py` and transform it into a more organized 📐, maintainable 🛠️, and production-ready codebase.
 License: MIT
 Author: Junior Torres
 Author-email: galas.apps@gmail.com
 Requires-Python: >=3.8.10,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -12,16 +12,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: fastapi[all] (>=0.100.1,<0.101.0)
 Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
+Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: scikit-learn (==1.0.2)
+Requires-Dist: uvicorn (>=0.23.2,<0.24.0)
 Project-URL: Code, https://github.com/JuniorTorresMTJ/mlops_shape_project
 Project-URL: Documentation, https://mlops-shape-project.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 
 # **<p align="center" style="color: #DA1B5D;"><strong>Welcome to Shape MLOps Project</strong></p>**
 
 [![Documentation Status](https://readthedocs.org/projects/notas-musicais/badge/?version=latest)](https://mlops-shape-project.readthedocs.io/en/latest/?badge=latest)
@@ -55,14 +59,19 @@
 -   Intricate or time-intensive modifications, if not instantly implementable, should be signposted within the code as TODOs. These markers should also sketch out the strategic approach intended for their eventual fulfillment 🕰️.
 
 
 ## 🚀 **Run the project**
 ***
 The provided configuration appears to be from a `pyproject.toml` file, which is a configuration file for the [Poetry](https://python-poetry.org/) dependency management and packaging tool in Python. To install and execute this project, follow the steps below:
 
+- Prerequisites:
+- Docker
+- Poetry
+- Python
+
 ### 1️⃣ Install Poetry:
 If you haven't installed Poetry yet, you can do so with the following command:
 
 ```bash
 curl -sSL https://install.python-poetry.org | python3 -
 ```
 
@@ -88,53 +97,132 @@
 ### 4️⃣ Activate the virtual environment:
 Poetry creates a virtual environment for your project. Activate it with:
 
 ```bash
 poetry shell
 ```
 
-### 5️⃣ Run the project:
+### 5️⃣ Build the Docker image:
 The exact command to run the project depends on its structure. Typically, there's a main Python script or module you'd execute to start the project. If there's a clear entry point, you can run:
 
 
 ```bash
-python mlops_shape_project\app.py
+docker build -t mlops-shape-project:latest .
 ```
 
+### 6️⃣ Build the Docker image:
+
+```bash
+docker run -p 8000:8000 mlops-shape-project:latest
+```
+API should now be running and accessible at http://localhost:8000.
 
-### 6️⃣ Additional tasks:
+###  Additional tasks:
 The provided configuration also contains some tasks defined with `taskipy`. You can run these tasks using the `poetry run task` command. For example:
 
 - To run the lint task: 
 
 ```bash
   poetry run task lint
 ```
 
 - To serve the documentation:
 
 ```bash
   poetry run task doc
 ```
 
-### 7️⃣ Expected Model Results:
-When evaluating the performance and predictions of our model, we often look at two key components:
+### 7️⃣ Endpoints:
+
+
+#### ✅ GET /data
 
-#### ✅ Expected Class Labels:
+-   Purpose:
+
+    -   This endpoint retrieves the original dataset from a predefined file location.
+-   Usage:
+
+    -   You simply send a GET request to this endpoint without any parameters.
+-   Example with `curl`:
+
+```bash
+    curl -X 'GET' http://localhost:8000/data
+```
+-   Response:
+
+![data](assets\img\data.png)
+
+If successful, you'll receive a JSON representation of the dataset. The structure will be a dictionary with columns as keys and their associated data as corresponding values.
+
+* * * * *
+
+#### ✅ POST /process_data
+
+-   Purpose:
+
+    -   Processes data from an uploaded file and returns the processed output.
+-   Usage:
+
+    -   Send a POST request to this endpoint with an attached file containing the data you want to process.
+-   Example with `curl`:
+
+```bash
+    curl -X 'POST' -F 'file=@path_to_your_file.csv' http://localhost:8000/process_data
+```
+-   Response:
 
-Class labels serve as numerical representations of the expected predictions or classifications from the model. In this context, the class labels can either be -1 or 1. These values might represent two distinct classes or categories in a binary classification scenario.
+![predict_path](assets\img\predict_path.png)
+
+If successful, you'll receive processed data (like predictions) as a JSON response.
+
+
+
+#### ✅ POST /predict
+
+-   Purpose:
+
+    -   This endpoint takes input data in the form of a JSON object and returns a prediction based on the provided data.
+-   Usage:
+
+    -   Send a POST request with a JSON payload representing the data for which you want a prediction.
+-   Example with `curl`:
+
+```bash
+    `curl -X 'POST' -H "Content-Type: application/json" -d '{"column1": "value1", "column2": "value2", ...}' http://localhost:8000/predict`
+```
+-   Response:
+
+![predict](assets\img\predict.png)
+
+If successful, you'll receive a JSON response with the prediction status and the predicted class.
+
+* * * * *
+
+#### ✅ POST /predict_batch
+
+-   Purpose:
+
+    -   Provides batch predictions based on the provided data.
+-   Usage:
+
+    -   Send a POST request with a JSON payload containing multiple rows of data for batch processing.
+-   Example with `curl`:
+
+```bash
+    curl -X 'POST' -H "Content-Type: application/json" -d '[{"column1": "value1_1", "column2": "value1_2", ...}, {"column1": "value2_1", "column2": "value2_2", ...}, ...]' http://localhost:8000/predict_batch
+```
+-   Response:
 
-![Array-output](assets\img\Output.png)
+![predict_batch](assets\img\predict_batch.png)
 
+ If successful, you'll receive a JSON response with the prediction status and the predicted classes for each input data row.
 
-#### ✅ Model Prediction DataFrame:
 
-Beyond the direct class labels, there is also a DataFrame compiled with the model's predictions. Specifically, this DataFrame contains a column named svm_predict, which displays the predicted class labels for each data instance.
+For each of the endpoints, if there's an error, the API will return a clear message indicating what went wrong, along with a status code indicating the nature of the error. Always make sure to check the returned message and status code to understand any issues.
 
-![Dataframe-output](assets\img\Output2.png)
 
 ## 📖 **Documentation**:
 
 The documentation of this project is an essential component for understanding its structure, functionalities, and usage guides. We strongly believe that comprehensive documentation can speed up the adoption, contribution, and debugging processes of the project. The documentation was crafted using [MkDocs](https://www.mkdocs.org/), a swift and straightforward tool for creating documentation websites from markdown files. It allows us to concentrate on the content while automating the process of converting Markdown into a structured and styled website.
 
 ⚠️[Documentation Link](https://mlops-shape-project.readthedocs.io/en/latest/)⚠️
```

