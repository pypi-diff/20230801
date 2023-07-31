# Comparing `tmp/nlp-models-3.0.0.tar.gz` & `tmp/nlp-models-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-3.0.0.tar", last modified: Wed Jul  5 22:20:06 2023, max compression
+gzip compressed data, was "nlp-models-4.0.0.tar", last modified: Mon Jul 31 22:47:10 2023, max compression
```

## Comparing `nlp-models-3.0.0.tar` & `nlp-models-4.0.0.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.589419 nlp-models-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-05 22:19:56.000000 nlp-models-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-05 22:20:06.589419 nlp-models-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-05 22:19:56.000000 nlp-models-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-05 22:19:56.000000 nlp-models-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-05 22:20:06.589419 nlp-models-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-05 22:19:56.000000 nlp-models-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.585419 nlp-models-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.589419 nlp-models-3.0.0/src/nlp_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.589419 nlp-models-3.0.0/src/nlp_models/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.589419 nlp-models-3.0.0/src/nlp_models/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.589419 nlp-models-3.0.0/src/nlp_models/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/multi_task_model/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.589419 nlp-models-3.0.0/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-05 22:20:06.000000 nlp-models-3.0.0/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-05 22:20:06.000000 nlp-models-3.0.0/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:20:06.000000 nlp-models-3.0.0/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 22:20:06.000000 nlp-models-3.0.0/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 22:20:06.000000 nlp-models-3.0.0/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:10.662034 nlp-models-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-31 22:47:01.000000 nlp-models-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-31 22:47:10.662034 nlp-models-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-31 22:47:01.000000 nlp-models-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-31 22:47:01.000000 nlp-models-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-31 22:47:10.662034 nlp-models-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 22:47:01.000000 nlp-models-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:10.654034 nlp-models-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:10.654034 nlp-models-4.0.0/src/nlp_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:10.658034 nlp-models-4.0.0/src/nlp_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/base/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/base/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/base/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/base/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/base/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:10.662034 nlp-models-4.0.0/src/nlp_models/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:10.662034 nlp-models-4.0.0/src/nlp_models/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/llm/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/llm/llms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/llm/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:10.662034 nlp-models-4.0.0/src/nlp_models/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-31 22:47:01.000000 nlp-models-4.0.0/src/nlp_models/multi_task_model/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:47:10.658034 nlp-models-4.0.0/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-31 22:47:10.000000 nlp-models-4.0.0/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-31 22:47:10.000000 nlp-models-4.0.0/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:47:10.000000 nlp-models-4.0.0/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 22:47:10.000000 nlp-models-4.0.0/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-31 22:47:10.000000 nlp-models-4.0.0/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-3.0.0/LICENSE` & `nlp-models-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-3.0.0/PKG-INFO` & `nlp-models-4.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 3.0.0
+Version: 4.0.0
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -30,29 +30,30 @@
 
 A repository for building transformer based nlp models
 
 ## Models
 
 1. bert_classifier
    A wrapper package around BERT-based classification models
-   
-   - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_a_classification_model_training_example.ipynb)
-   - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_b_classification_inference_example.ipynb)
-   
-3. multi_task_model
+
+   - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-finetuning/01_a_classification_model_training_example.ipynb)
+   - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-finetuning/01_b_classification_inference_example.ipynb)
+2. multi_task_model
    An implementation of multi-tasking model built on encoder models
-   
-   - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_a_multitask_model_zeroshot_learning.ipynb)
-   - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_b_multitask_model_training_example.ipynb)
-   - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_c_multitask_model_inference_example.ipynb)
+
+   - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_a_multitask_model_zeroshot_learning.ipynb)
+   - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_b_multitask_model_training_example.ipynb)
+   - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_c_multitask_model_inference_example.ipynb)
+   - [Qqrant Vector DB](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_d_qdrant_vector_db.ipynb)
 
 ## Other Example Notebooks
 
-- [Training GPT-2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt2_training.ipynb)
-- [Running Falcon 4b model](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_falcon_4b.ipynb)
+- [Training GPT-2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-training/gpt-2-training/03_gpt2_training.ipynb)
+- [Running Falcon 4b model](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/05_falcon_4b.ipynb)
+- [Run Llama2 chat on cpu](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
 
 ## Installation
 
 ### Install from PyPi
 
 ```
 pip install nlp-models
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlp-models Version: 3.0.0 Summary: Transformers
+Metadata-Version: 2.1 Name: nlp-models Version: 4.0.0 Summary: Transformers
 based NLP models Home-page: https://github.com/minggnim/nlp-models Author: Ming
 Gao Author-email: ming_gao@outlook.com Classifier: Development Status :: 4 -
 Beta Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
@@ -16,24 +16,29 @@
 badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/
 workflows/python-package.yml) [![Dependency Review](https://github.com/
 minggnim/nlp-classification-model/actions/workflows/dependency-review.yml/
 badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/
 workflows/dependency-review.yml) # NLP Models A repository for building
 transformer based nlp models ## Models 1. bert_classifier A wrapper package
 around BERT-based classification models - [Training example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/
-01_a_classification_model_training_example.ipynb) - [Inference example](https:/
-/github.com/minggnim/nlp-models/blob/master/notebooks/
-01_b_classification_inference_example.ipynb) 3. multi_task_model An
-implementation of multi-tasking model built on encoder models - [Zero-shot
-multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/
+github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-
+finetuning/01_a_classification_model_training_example.ipynb) - [Inference
+example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-
+classification-finetuning/01_b_classification_inference_example.ipynb) 2.
+multi_task_model An implementation of multi-tasking model built on encoder
+models - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/
+blob/master/notebooks/02_multi-task-model/
 02_a_multitask_model_zeroshot_learning.ipynb) - [Training example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/
+github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
 02_b_multitask_model_training_example.ipynb) - [Inference example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/
-02_c_multitask_model_inference_example.ipynb) ## Other Example Notebooks -
-[Training GPT-2 model](https://github.com/minggnim/nlp-models/blob/master/
-notebooks/03_gpt2_training.ipynb) - [Running Falcon 4b model](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/04_falcon_4b.ipynb) ##
-Installation ### Install from PyPi ``` pip install nlp-models ``` ### Install
-from source ``` git clone git@github.com:minggnim/nlp-models.git pip install -
-r requirements ```
+github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
+02_c_multitask_model_inference_example.ipynb) - [Qqrant Vector DB](https://
+github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
+02_d_qdrant_vector_db.ipynb) ## Other Example Notebooks - [Training GPT-
+2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-
+training/gpt-2-training/03_gpt2_training.ipynb) - [Running Falcon 4b model]
+(https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/
+05_falcon_4b.ipynb) - [Run Llama2 chat on cpu](https://github.com/minggnim/nlp-
+models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
+## Installation ### Install from PyPi ``` pip install nlp-models ``` ###
+Install from source ``` git clone git@github.com:minggnim/nlp-models.git pip
+install -r requirements ```
```

### Comparing `nlp-models-3.0.0/README.md` & `nlp-models-4.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 
 A repository for building transformer based nlp models
 
 ## Models
 
 1. bert_classifier
    A wrapper package around BERT-based classification models
-   
-   - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_a_classification_model_training_example.ipynb)
-   - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_b_classification_inference_example.ipynb)
-   
-3. multi_task_model
+
+   - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-finetuning/01_a_classification_model_training_example.ipynb)
+   - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-finetuning/01_b_classification_inference_example.ipynb)
+2. multi_task_model
    An implementation of multi-tasking model built on encoder models
-   
-   - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_a_multitask_model_zeroshot_learning.ipynb)
-   - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_b_multitask_model_training_example.ipynb)
-   - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_c_multitask_model_inference_example.ipynb)
+
+   - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_a_multitask_model_zeroshot_learning.ipynb)
+   - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_b_multitask_model_training_example.ipynb)
+   - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_c_multitask_model_inference_example.ipynb)
+   - [Qqrant Vector DB](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_d_qdrant_vector_db.ipynb)
 
 ## Other Example Notebooks
 
-- [Training GPT-2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt2_training.ipynb)
-- [Running Falcon 4b model](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_falcon_4b.ipynb)
+- [Training GPT-2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-training/gpt-2-training/03_gpt2_training.ipynb)
+- [Running Falcon 4b model](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/05_falcon_4b.ipynb)
+- [Run Llama2 chat on cpu](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
 
 ## Installation
 
 ### Install from PyPi
 
 ```
 pip install nlp-models
```

#### html2text {}

```diff
@@ -6,24 +6,29 @@
 badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/
 workflows/python-package.yml) [![Dependency Review](https://github.com/
 minggnim/nlp-classification-model/actions/workflows/dependency-review.yml/
 badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/
 workflows/dependency-review.yml) # NLP Models A repository for building
 transformer based nlp models ## Models 1. bert_classifier A wrapper package
 around BERT-based classification models - [Training example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/
-01_a_classification_model_training_example.ipynb) - [Inference example](https:/
-/github.com/minggnim/nlp-models/blob/master/notebooks/
-01_b_classification_inference_example.ipynb) 3. multi_task_model An
-implementation of multi-tasking model built on encoder models - [Zero-shot
-multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/
+github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-
+finetuning/01_a_classification_model_training_example.ipynb) - [Inference
+example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-
+classification-finetuning/01_b_classification_inference_example.ipynb) 2.
+multi_task_model An implementation of multi-tasking model built on encoder
+models - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/
+blob/master/notebooks/02_multi-task-model/
 02_a_multitask_model_zeroshot_learning.ipynb) - [Training example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/
+github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
 02_b_multitask_model_training_example.ipynb) - [Inference example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/
-02_c_multitask_model_inference_example.ipynb) ## Other Example Notebooks -
-[Training GPT-2 model](https://github.com/minggnim/nlp-models/blob/master/
-notebooks/03_gpt2_training.ipynb) - [Running Falcon 4b model](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/04_falcon_4b.ipynb) ##
-Installation ### Install from PyPi ``` pip install nlp-models ``` ### Install
-from source ``` git clone git@github.com:minggnim/nlp-models.git pip install -
-r requirements ```
+github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
+02_c_multitask_model_inference_example.ipynb) - [Qqrant Vector DB](https://
+github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
+02_d_qdrant_vector_db.ipynb) ## Other Example Notebooks - [Training GPT-
+2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-
+training/gpt-2-training/03_gpt2_training.ipynb) - [Running Falcon 4b model]
+(https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/
+05_falcon_4b.ipynb) - [Run Llama2 chat on cpu](https://github.com/minggnim/nlp-
+models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
+## Installation ### Install from PyPi ``` pip install nlp-models ``` ###
+Install from source ``` git clone git@github.com:minggnim/nlp-models.git pip
+install -r requirements ```
```

### Comparing `nlp-models-3.0.0/setup.cfg` & `nlp-models-4.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 3.0.0
+version = 4.0.0
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -25,14 +25,16 @@
 	=src
 python_requires = 
 	>=3.6
 install_requires = 
 	torch
 	torchmetrics
 	transformers
+	langchain
+	ctransformers
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 full = 
 	tqdm
```

### Comparing `nlp-models-3.0.0/src/nlp_models/base/data.py` & `nlp-models-4.0.0/src/nlp_models/base/data.py`

 * *Files identical despite different names*

### Comparing `nlp-models-3.0.0/src/nlp_models/base/io.py` & `nlp-models-4.0.0/src/nlp_models/base/io.py`

 * *Files identical despite different names*

### Comparing `nlp-models-3.0.0/src/nlp_models/base/layers.py` & `nlp-models-4.0.0/src/nlp_models/base/layers.py`

 * *Files identical despite different names*

### Comparing `nlp-models-3.0.0/src/nlp_models/base/metrics.py` & `nlp-models-4.0.0/src/nlp_models/base/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-3.0.0/src/nlp_models/base/utils.py` & `nlp-models-4.0.0/src/nlp_models/base/utils.py`

 * *Files identical despite different names*

### Comparing `nlp-models-3.0.0/src/nlp_models/bert_classifier/bert.py` & `nlp-models-4.0.0/src/nlp_models/bert_classifier/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-models-3.0.0/src/nlp_models/bert_classifier/predict.py` & `nlp-models-4.0.0/src/nlp_models/bert_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `nlp-models-3.0.0/src/nlp_models/bert_classifier/train.py` & `nlp-models-4.0.0/src/nlp_models/bert_classifier/train.py`

 * *Files identical despite different names*

### Comparing `nlp-models-3.0.0/src/nlp_models/multi_task_model/mtl.py` & `nlp-models-4.0.0/src/nlp_models/multi_task_model/mtl.py`

 * *Files identical despite different names*

### Comparing `nlp-models-3.0.0/src/nlp_models/multi_task_model/trainer.py` & `nlp-models-4.0.0/src/nlp_models/multi_task_model/trainer.py`

 * *Files identical despite different names*

### Comparing `nlp-models-3.0.0/src/nlp_models.egg-info/PKG-INFO` & `nlp-models-4.0.0/src/nlp_models.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 3.0.0
+Version: 4.0.0
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -30,29 +30,30 @@
 
 A repository for building transformer based nlp models
 
 ## Models
 
 1. bert_classifier
    A wrapper package around BERT-based classification models
-   
-   - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_a_classification_model_training_example.ipynb)
-   - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_b_classification_inference_example.ipynb)
-   
-3. multi_task_model
+
+   - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-finetuning/01_a_classification_model_training_example.ipynb)
+   - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-finetuning/01_b_classification_inference_example.ipynb)
+2. multi_task_model
    An implementation of multi-tasking model built on encoder models
-   
-   - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_a_multitask_model_zeroshot_learning.ipynb)
-   - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_b_multitask_model_training_example.ipynb)
-   - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_c_multitask_model_inference_example.ipynb)
+
+   - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_a_multitask_model_zeroshot_learning.ipynb)
+   - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_b_multitask_model_training_example.ipynb)
+   - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_c_multitask_model_inference_example.ipynb)
+   - [Qqrant Vector DB](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_d_qdrant_vector_db.ipynb)
 
 ## Other Example Notebooks
 
-- [Training GPT-2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt2_training.ipynb)
-- [Running Falcon 4b model](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_falcon_4b.ipynb)
+- [Training GPT-2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-training/gpt-2-training/03_gpt2_training.ipynb)
+- [Running Falcon 4b model](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/05_falcon_4b.ipynb)
+- [Run Llama2 chat on cpu](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
 
 ## Installation
 
 ### Install from PyPi
 
 ```
 pip install nlp-models
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlp-models Version: 3.0.0 Summary: Transformers
+Metadata-Version: 2.1 Name: nlp-models Version: 4.0.0 Summary: Transformers
 based NLP models Home-page: https://github.com/minggnim/nlp-models Author: Ming
 Gao Author-email: ming_gao@outlook.com Classifier: Development Status :: 4 -
 Beta Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
@@ -16,24 +16,29 @@
 badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/
 workflows/python-package.yml) [![Dependency Review](https://github.com/
 minggnim/nlp-classification-model/actions/workflows/dependency-review.yml/
 badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/
 workflows/dependency-review.yml) # NLP Models A repository for building
 transformer based nlp models ## Models 1. bert_classifier A wrapper package
 around BERT-based classification models - [Training example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/
-01_a_classification_model_training_example.ipynb) - [Inference example](https:/
-/github.com/minggnim/nlp-models/blob/master/notebooks/
-01_b_classification_inference_example.ipynb) 3. multi_task_model An
-implementation of multi-tasking model built on encoder models - [Zero-shot
-multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/
+github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-
+finetuning/01_a_classification_model_training_example.ipynb) - [Inference
+example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-
+classification-finetuning/01_b_classification_inference_example.ipynb) 2.
+multi_task_model An implementation of multi-tasking model built on encoder
+models - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/
+blob/master/notebooks/02_multi-task-model/
 02_a_multitask_model_zeroshot_learning.ipynb) - [Training example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/
+github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
 02_b_multitask_model_training_example.ipynb) - [Inference example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/
-02_c_multitask_model_inference_example.ipynb) ## Other Example Notebooks -
-[Training GPT-2 model](https://github.com/minggnim/nlp-models/blob/master/
-notebooks/03_gpt2_training.ipynb) - [Running Falcon 4b model](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/04_falcon_4b.ipynb) ##
-Installation ### Install from PyPi ``` pip install nlp-models ``` ### Install
-from source ``` git clone git@github.com:minggnim/nlp-models.git pip install -
-r requirements ```
+github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
+02_c_multitask_model_inference_example.ipynb) - [Qqrant Vector DB](https://
+github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
+02_d_qdrant_vector_db.ipynb) ## Other Example Notebooks - [Training GPT-
+2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-
+training/gpt-2-training/03_gpt2_training.ipynb) - [Running Falcon 4b model]
+(https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/
+05_falcon_4b.ipynb) - [Run Llama2 chat on cpu](https://github.com/minggnim/nlp-
+models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
+## Installation ### Install from PyPi ``` pip install nlp-models ``` ###
+Install from source ``` git clone git@github.com:minggnim/nlp-models.git pip
+install -r requirements ```
```

### Comparing `nlp-models-3.0.0/src/nlp_models.egg-info/SOURCES.txt` & `nlp-models-4.0.0/src/nlp_models.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -16,10 +16,14 @@
 src/nlp_models/base/loss.py
 src/nlp_models/base/metrics.py
 src/nlp_models/base/utils.py
 src/nlp_models/bert_classifier/__init__.py
 src/nlp_models/bert_classifier/bert.py
 src/nlp_models/bert_classifier/predict.py
 src/nlp_models/bert_classifier/train.py
+src/nlp_models/llm/__init__.py
+src/nlp_models/llm/base.py
+src/nlp_models/llm/llms.py
+src/nlp_models/llm/prompts.py
 src/nlp_models/multi_task_model/__init__.py
 src/nlp_models/multi_task_model/mtl.py
 src/nlp_models/multi_task_model/trainer.py
```

