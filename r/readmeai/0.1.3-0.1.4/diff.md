# Comparing `tmp/readmeai-0.1.3.tar.gz` & `tmp/readmeai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.1.3.tar", max compression
+gzip compressed data, was "readmeai-0.1.4.tar", max compression
```

## Comparing `readmeai-0.1.3.tar` & `readmeai-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1063 2023-08-01 11:08:10.518980 readmeai-0.1.3/LICENSE
--rw-r--r--   0        0        0    17538 2023-08-01 11:08:10.518980 readmeai-0.1.3/README.md
--rw-r--r--   0        0        0     2101 2023-08-01 11:08:10.562980 readmeai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/__init__.py
--rw-r--r--   0        0        0     1169 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/app/Dockerfile
--rw-r--r--   0        0        0        0 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/app/__init__.py
--rw-r--r--   0        0        0     2659 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/app/streamlit_app.py
--rw-r--r--   0        0        0     7736 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/builder.py
--rw-r--r--   0        0        0     6368 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/conf.py
--rw-r--r--   0        0        0     4955 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/factory.py
--rw-r--r--   0        0        0     2113 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/logger.py
--rwxr-xr-x   0        0        0     4044 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/main.py
--rw-r--r--   0        0        0     7608 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/model.py
--rw-r--r--   0        0        0     7272 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/parse.py
--rw-r--r--   0        0        0     6419 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/preprocess.py
--rw-r--r--   0        0        0     3991 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/utils.py
--rw-r--r--   0        0        0    19008 1970-01-01 00:00:00.000000 readmeai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-01 11:28:49.536132 readmeai-0.1.4/LICENSE
+-rw-r--r--   0        0        0    17538 2023-08-01 11:28:49.536132 readmeai-0.1.4/README.md
+-rw-r--r--   0        0        0     2101 2023-08-01 11:28:49.584136 readmeai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/__init__.py
+-rw-r--r--   0        0        0     1075 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/app/Dockerfile
+-rw-r--r--   0        0        0        0 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/app/__init__.py
+-rw-r--r--   0        0        0     2659 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/app/streamlit_app.py
+-rw-r--r--   0        0        0     7736 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/builder.py
+-rw-r--r--   0        0        0     6368 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/conf.py
+-rw-r--r--   0        0        0     4955 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/factory.py
+-rw-r--r--   0        0        0     2113 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/logger.py
+-rwxr-xr-x   0        0        0     4044 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/main.py
+-rw-r--r--   0        0        0     7608 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/model.py
+-rw-r--r--   0        0        0     7272 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/parse.py
+-rw-r--r--   0        0        0     6419 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/preprocess.py
+-rw-r--r--   0        0        0     3991 2023-08-01 11:28:49.584136 readmeai-0.1.4/readmeai/utils.py
+-rw-r--r--   0        0        0    19008 1970-01-01 00:00:00.000000 readmeai-0.1.4/PKG-INFO
```

### Comparing `readmeai-0.1.3/LICENSE` & `readmeai-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.3/README.md` & `readmeai-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.3/pyproject.toml` & `readmeai-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.1.3"
+version = "0.1.4"
 description = "🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
```

### Comparing `readmeai-0.1.3/readmeai/app/Dockerfile` & `readmeai-0.1.4/readmeai/app/Dockerfile`

 * *Files 16% similar despite different names*

```diff
@@ -24,18 +24,15 @@
 
 # Switch to the new user
 USER tempuser
 
 # Add the directory where pip installs user scripts to the PATH
 ENV PATH=/home/tempuser/.local/bin:$PATH
 
-# Copy the Streamlit app file into the container
-COPY streamlit_app.py /app/streamlit_app.py
-
 # Install Python dependencies (including readmeai)
-RUN pip install --no-cache-dir readmeai==0.1.2
+RUN pip install --no-cache-dir readmeai==0.1.3
 
 # Expose port 8501 for Streamlit
 EXPOSE 8501
 
 # Set the command to run the Streamlit server
 CMD ["streamlit", "run", "streamlit_app.py"]
```

### Comparing `readmeai-0.1.3/readmeai/app/streamlit_app.py` & `readmeai-0.1.4/readmeai/app/streamlit_app.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.3/readmeai/builder.py` & `readmeai-0.1.4/readmeai/builder.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.3/readmeai/conf.py` & `readmeai-0.1.4/readmeai/conf.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.3/readmeai/factory.py` & `readmeai-0.1.4/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.3/readmeai/logger.py` & `readmeai-0.1.4/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.3/readmeai/main.py` & `readmeai-0.1.4/readmeai/main.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.3/readmeai/model.py` & `readmeai-0.1.4/readmeai/model.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.3/readmeai/parse.py` & `readmeai-0.1.4/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.3/readmeai/preprocess.py` & `readmeai-0.1.4/readmeai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.3/readmeai/utils.py` & `readmeai-0.1.4/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.3/PKG-INFO` & `readmeai-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.1.3
+Version: 0.1.4
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
 Keywords: readme,python-cli,readme-template,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,openai-python,chatgpt-python,gpt-35-turbo,gpt-4-api,openai-cli,llm-prompting,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
 Requires-Python: >3.9.7,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: readmeai Version: 0.1.3 Summary: ð Generate
+Metadata-Version: 2.1 Name: readmeai Version: 0.1.4 Summary: ð Generate
 awesome README.md files from the terminal, powered by OpenAI's GPT language
 model APIs ð« Home-page: https://github.com/eli64s/readme-ai License: MIT
 Keywords: readme,python-cli,readme-template,readme-md,awesome-readme,readme-
 generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,openai-
 python,chatgpt-python,gpt-35-turbo,gpt-4-api,openai-cli,llm-prompting,llm-agent
 Author: Eli Author-email: 0x.eli.64s@gmail.com Requires-Python: >3.9.7,<4.0.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
```

