# Comparing `tmp/aidriver-0.1.2.1.tar.gz` & `tmp/aidriver-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aidriver-0.1.2.1.tar", last modified: Mon Jul 31 21:49:30 2023, max compression
+gzip compressed data, was "aidriver-0.1.3.tar", last modified: Tue Aug  1 19:25:21 2023, max compression
```

## Comparing `aidriver-0.1.2.1.tar` & `aidriver-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:49:30.035001 aidriver-0.1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/.envtemplate
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-31 21:49:30.039002 aidriver-0.1.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:49:30.027001 aidriver-0.1.2.1/ai_driver/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/instruct.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/langsmith_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:49:30.027001 aidriver-0.1.2.1/ai_driver/local_llm/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/local_llm/ggml_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/local_llm/ggml_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/local_llm/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/local_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/qa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:49:30.027001 aidriver-0.1.2.1/ai_driver/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/scripts/download_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/scripts/init_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:49:30.027001 aidriver-0.1.2.1/ai_driver/scripts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/scripts/tests/test_download_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:49:30.027001 aidriver-0.1.2.1/ai_driver/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/tests/local_loader_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/tests/qa_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:49:30.027001 aidriver-0.1.2.1/ai_driver/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)  2869842 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/tests/test_data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:49:30.031001 aidriver-0.1.2.1/ai_driver/vector_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/vector_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/vector_storage/faiss_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/ai_driver/vector_storage/pinecone_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:49:30.031001 aidriver-0.1.2.1/aidriver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-31 21:49:29.000000 aidriver-0.1.2.1/aidriver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-31 21:49:30.000000 aidriver-0.1.2.1/aidriver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:49:29.000000 aidriver-0.1.2.1/aidriver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-31 21:49:29.000000 aidriver-0.1.2.1/aidriver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 21:49:29.000000 aidriver-0.1.2.1/aidriver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:49:30.031001 aidriver-0.1.2.1/config/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/config/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:49:30.035001 aidriver-0.1.2.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2869842 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-31 21:49:02.000000 aidriver-0.1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 21:49:30.039002 aidriver-0.1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.192777 aidriver-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 19:24:59.000000 aidriver-0.1.3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 19:24:59.000000 aidriver-0.1.3/.envtemplate
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-01 19:24:59.000000 aidriver-0.1.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-01 19:25:21.192777 aidriver-0.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.180777 aidriver-0.1.3/ai_driver/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/instruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/langsmith_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.184777 aidriver-0.1.3/ai_driver/local_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/local_llm/ggml_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/local_llm/ggml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/local_llm/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/local_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/qa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.184777 aidriver-0.1.3/ai_driver/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/scripts/download_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/scripts/init_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.184777 aidriver-0.1.3/ai_driver/scripts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/scripts/tests/test_download_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.184777 aidriver-0.1.3/ai_driver/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.184777 aidriver-0.1.3/ai_driver/server/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.184777 aidriver-0.1.3/ai_driver/server/api/api_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/api/api_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/api/api_v1/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.184777 aidriver-0.1.3/ai_driver/server/api/api_v1/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/api/api_v1/endpoints/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/api/api_v1/endpoints/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/api/api_v1/endpoints/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/api/deps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.184777 aidriver-0.1.3/ai_driver/server/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/core/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.184777 aidriver-0.1.3/ai_driver/server/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/core/tests/auth_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.184777 aidriver-0.1.3/ai_driver/server/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/crud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/crud/crud_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.184777 aidriver-0.1.3/ai_driver/server/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/db/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/db/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/db/init_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/db/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.188777 aidriver-0.1.3/ai_driver/server/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.188777 aidriver-0.1.3/ai_driver/server/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/schemas/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/schemas/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.188777 aidriver-0.1.3/ai_driver/server/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/scripts/backend_pre_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/scripts/initial_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/scripts/prestart.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      890 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/scripts/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.188777 aidriver-0.1.3/ai_driver/server/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.188777 aidriver-0.1.3/ai_driver/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/tests/local_loader_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/tests/qa_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.188777 aidriver-0.1.3/ai_driver/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2869842 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/tests/test_data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.192777 aidriver-0.1.3/ai_driver/vector_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/vector_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/vector_storage/faiss_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-01 19:24:59.000000 aidriver-0.1.3/ai_driver/vector_storage/pinecone_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.192777 aidriver-0.1.3/aidriver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-01 19:25:21.000000 aidriver-0.1.3/aidriver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-01 19:25:21.000000 aidriver-0.1.3/aidriver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:25:21.000000 aidriver-0.1.3/aidriver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-01 19:25:21.000000 aidriver-0.1.3/aidriver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 19:25:21.000000 aidriver-0.1.3/aidriver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.192777 aidriver-0.1.3/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 19:24:59.000000 aidriver-0.1.3/alembic/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-01 19:24:59.000000 aidriver-0.1.3/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 19:24:59.000000 aidriver-0.1.3/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.192777 aidriver-0.1.3/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-01 19:24:59.000000 aidriver-0.1.3/alembic/versions/b99d93299f68_initial_db_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-01 19:24:59.000000 aidriver-0.1.3/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:21.192777 aidriver-0.1.3/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 19:24:59.000000 aidriver-0.1.3/config/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-01 19:24:59.000000 aidriver-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-01 19:25:21.192777 aidriver-0.1.3/setup.cfg
```

### Comparing `aidriver-0.1.2.1/Dockerfile` & `aidriver-0.1.3/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-FROM nvidia/cuda:11.8.0-runtime-ubuntu22.04
+FROM nvidia/cuda:12.2.0-runtime-ubuntu22.04
 
 # Install dependencies
 RUN apt-get update && \
     apt-get install --no-install-recommends -y git vim build-essential python3-dev python3-pip && \
     rm -rf /var/lib/apt/lists/*
 RUN python3 -m pip install --upgrade pip
 
 # Create appuser
 RUN groupadd -r appuser && useradd --no-log-init -r -g appuser appuser
 
 # Create app directory and change ownership to appuser
 RUN mkdir /app && \
     mkdir -p /home/appuser/.cache && \
     chown -R appuser:appuser /app /home/appuser
-
-# Set working directory to /app
+COPY ./pyproject.toml /app/pyproject.toml
+# # Set working directory to /app
 WORKDIR /app
+RUN pip install .[server]
+
 
-COPY ./ai_driver /app/ai_driver
-RUN python3 -m pip install -e /app/ai_driver
+COPY . /app/ai_driver
+RUN python3 -m pip install -e /app/ai_driver[server]
 
 # Change ownership of /app to appuser
 RUN chown -R appuser:appuser /app /home/appuser
 
 USER appuser
 WORKDIR /app/ai_driver
-CMD ["/usr/bin/python3", "/app/ai_driver/ai_driver/main.py"]
+RUN chmod +x ./ai_driver/server/scripts/run.sh
+CMD ["./ai_driver/server/scripts/run.sh"]
+# CMD ["tail", "-f", "/dev/null"]
```

### Comparing `aidriver-0.1.2.1/ai_driver/local_llm/ggml_llm.py` & `aidriver-0.1.3/ai_driver/local_llm/ggml_llm.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,32 +6,35 @@
 
 @dataclass
 class GGMLConfig:
     model_path: str
     model_type: str
     max_new_tokens: int
     temperature: float = 0.7
+    gpu_layers: int = 0
 
 
 def build_ggml_llm(config: GGMLConfig) -> CTransformers:
     llm = CTransformers(
         model=config.model_path,
         model_type=config.model_type,
         config={
             "max_new_tokens": config.max_new_tokens,
             "temperature": config.temperature,
+            "gpu_layers": config.gpu_layers,
         },
     )
     return llm
 
 
 def get_default_ggml_config():
     # Import config vars
     with open("config/config.yml", "r", encoding="utf8") as ymlfile:
         cfg = box.Box(yaml.safe_load(ymlfile))
         config = GGMLConfig(
             model_path=cfg.LLM_MODEL_BIN_PATH,
             model_type=cfg.MODEL_TYPE,
             max_new_tokens=cfg.MAX_NEW_TOKENS,
             temperature=cfg.TEMPERATURE,
+            gpu_layers=cfg.GGML_GPU_LAYERS,
         )
         return config
```

### Comparing `aidriver-0.1.2.1/ai_driver/local_llm/ggml_pipeline.py` & `aidriver-0.1.3/ai_driver/local_llm/ggml_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,19 @@
         retriever=vectordb.as_retriever(search_kwargs={"k": config.vector_count}),
         return_source_documents=config.return_source,
         chain_type_kwargs={"prompt": prompt},
     )
     return qa_chain
 
 
-def setup_local_qa_db(config: QADBConfig):
+def setup_local_qa_db(config: QADBConfig, device: str = "cuda"):
+    # Set device to cpu for cpu inference
+
     embeddings = HuggingFaceEmbeddings(
-        model_name=config.embed_model, model_kwargs={"device": "cpu"}
+        model_name=config.embed_model, model_kwargs={"device": device}
     )
     vectordb = FAISS.load_local(config.db_path, embeddings)
 
     ggml_config = get_default_ggml_config()
     llm = build_ggml_llm(ggml_config)
     qa_prompt = set_qa_prompt()
     dbqa = build_retrieval_qa(llm, qa_prompt, vectordb, config)
```

### Comparing `aidriver-0.1.2.1/ai_driver/local_loader.py` & `aidriver-0.1.3/ai_driver/local_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,13 +37,13 @@
     texts = text_splitter.split_documents(documents)
     logger.info(f"Split {len(documents)} documents into {len(texts)}")
     return texts
 
 
 def get_default_local_download() -> List[Document]:
     """Default document list for local download"""
-    dir_path = "data"
+    dir_path = "/data"  # TODO convert to config
     glob_pattern = "./*.pdf"
 
     chunks = load(dir_path, glob_pattern)
     texts = split(chunks, chunk_size=1000, chunk_overlap=200)
     return texts
```

### Comparing `aidriver-0.1.2.1/ai_driver/pipelines.py` & `aidriver-0.1.3/ai_driver/pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ai_driver.vector_storage.faiss_manager import embed_FAISS_from_documents
 from ai_driver.local_loader import get_default_local_download
 from ai_driver.qa import query_documents
 from ai_driver.instruct import get_instruct_config, InstructConfig
 from ai_driver.local_llm.ggml_pipeline import setup_local_qa_db, get_default_qa_config
 
 
-def pinecone_pipeline():
+def pinecone_pipeline(query: str):
     """Example Pinecone Pipeline"""
     logger.info("Pinecone Pipeline")
     config = PineconeConfig(
         openai_key=os.getenv("OPENAI_API_KEY"),
         pinecone_key=os.getenv("PINECONE_API_KEY"),
         pinecone_env=os.getenv("PINECONE_API_ENV"),
         index_name=os.getenv("PINECONE_INDEX_NAME"),
@@ -33,18 +33,19 @@
     qa_chain = RetrievalQA.from_chain_type(
         llm=OpenAI(client=client, temperature=0.2),
         chain_type="stuff",
         retriever=retriever,
         verbose=True,
         return_source_documents=True,
     )
-    query_documents(qa_chain, "How do saving throws work?")
+    response = query_documents(qa_chain, query)
+    return response
 
 
-def local_llm_pipeline():
+def local_llm_pipeline(query: str):
     """Example Local LLM Pipeline"""
 
     query = "How do saving throws work?"
 
     # Setup DBQA
     start = timeit.default_timer()
     config = get_default_qa_config()
@@ -61,14 +62,15 @@
         logger.info(f"\nSource Document {i+1}\n")
         logger.info(f"Source Text: {doc.page_content}")
         logger.info(f'Document Name: {doc.metadata["source"]}')
         logger.info(f'Page Number: {doc.metadata["page"]}\n')
         logger.info("=" * 60)
 
     logger.info(f"Time to retrieve response: {end - start}")
+    return response
 
 
 def local_download_pipeline(config=None):
     """Example local store pipeline"""
     logger.info("Local download pipeline: FAISS")
     texts = get_default_local_download()
     config: InstructConfig = get_instruct_config()
```

### Comparing `aidriver-0.1.2.1/ai_driver/qa.py` & `aidriver-0.1.3/ai_driver/qa.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,7 +25,8 @@
     for source in llm_response["source_documents"]:
         logger.info(source.metadata)
 
 
 def query_documents(qa_chain, query):
     llm_response = qa_chain(query)
     process_llm_response(llm_response)
+    return llm_response
```

### Comparing `aidriver-0.1.2.1/ai_driver/scripts/download_model.py` & `aidriver-0.1.3/ai_driver/scripts/download_model.py`

 * *Files identical despite different names*

### Comparing `aidriver-0.1.2.1/ai_driver/scripts/init_db.py` & `aidriver-0.1.3/ai_driver/scripts/init_db.py`

 * *Files identical despite different names*

### Comparing `aidriver-0.1.2.1/ai_driver/scripts/tests/test_download_model.py` & `aidriver-0.1.3/ai_driver/scripts/tests/test_download_model.py`

 * *Files identical despite different names*

### Comparing `aidriver-0.1.2.1/ai_driver/tests/local_loader_test.py` & `aidriver-0.1.3/ai_driver/tests/local_loader_test.py`

 * *Files identical despite different names*

### Comparing `aidriver-0.1.2.1/ai_driver/tests/qa_test.py` & `aidriver-0.1.3/ai_driver/tests/qa_test.py`

 * *Files identical despite different names*

### Comparing `aidriver-0.1.2.1/ai_driver/tests/test_data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf` & `aidriver-0.1.3/ai_driver/tests/test_data/PlayerDnDBasicRules_v0.2_PrintFriendly.pdf`

 * *Files identical despite different names*

### Comparing `aidriver-0.1.2.1/ai_driver/vector_storage/faiss_manager.py` & `aidriver-0.1.3/ai_driver/vector_storage/faiss_manager.py`

 * *Files identical despite different names*

### Comparing `aidriver-0.1.2.1/ai_driver/vector_storage/pinecone_manager.py` & `aidriver-0.1.3/ai_driver/vector_storage/pinecone_manager.py`

 * *Files identical despite different names*

### Comparing `aidriver-0.1.2.1/pyproject.toml` & `aidriver-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   "setuptools-scm",
   "pytest",
 ]
 
 [project]
 description = "AIDriver"
 name = "aidriver"
-version = "0.1.2.1"
+version = "0.1.3"
 dependencies = [
     "requests",
   "python-dotenv",
   "pandas~=2.0.0",
   "pyarrow~=12.0.0",
   "debugpy",
   "loguru",
@@ -47,21 +47,36 @@
 [tool.pytest.ini_options]
 pythonpath = [
   "ai_driver",
 ]
 
 [tool.setuptools.packages.find]
 include = ["ai_driver", "ai_driver.*", "config"]  # package names should match these glob patterns (["*"] by default)
-exclude = ["data", "vectorstore", "artifacts"]  # exclude packages matching these glob patterns (empty by default)
+exclude = []  # exclude packages matching these glob patterns (empty by default)
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "trio",
     "pytest-httpx",
 ]
 dev = [
     "ipykernel",
     "mypy >= 1.0.1",
     "black",
     "pre-commit",
 ]
+server = [
+    'uvicorn',
+    'fastapi',
+    'jose',
+    "python-multipart",
+    "pydantic[email]",
+    "Jinja2",
+    "SQLAlchemy",
+    "alembic",
+    "gunicorn",
+    "passlib",
+    "python-jose",
+    "tenacity"
+
+]
```

