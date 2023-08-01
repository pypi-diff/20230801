# Comparing `tmp/readmeai-0.1.2.tar.gz` & `tmp/readmeai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.1.2.tar", max compression
+gzip compressed data, was "readmeai-0.1.3.tar", max compression
```

## Comparing `readmeai-0.1.2.tar` & `readmeai-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     1063 2023-08-01 04:17:58.917739 readmeai-0.1.2/LICENSE
--rw-r--r--   0        0        0    17592 2023-08-01 04:17:58.917739 readmeai-0.1.2/README.md
--rw-r--r--   0        0        0     2101 2023-08-01 04:17:58.965740 readmeai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/__init__.py
--rw-r--r--   0        0        0     2582 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/app.py
--rw-r--r--   0        0        0     7736 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/builder.py
--rw-r--r--   0        0        0     6342 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/conf.py
--rw-r--r--   0        0        0     4955 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/factory.py
--rw-r--r--   0        0        0     2113 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/logger.py
--rwxr-xr-x   0        0        0     4044 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/main.py
--rw-r--r--   0        0        0     7608 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/model.py
--rw-r--r--   0        0        0     7272 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/parse.py
--rw-r--r--   0        0        0     6419 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/preprocess.py
--rw-r--r--   0        0        0     3991 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/utils.py
--rw-r--r--   0        0        0    19062 1970-01-01 00:00:00.000000 readmeai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-01 11:08:10.518980 readmeai-0.1.3/LICENSE
+-rw-r--r--   0        0        0    17538 2023-08-01 11:08:10.518980 readmeai-0.1.3/README.md
+-rw-r--r--   0        0        0     2101 2023-08-01 11:08:10.562980 readmeai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/__init__.py
+-rw-r--r--   0        0        0     1169 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/app/Dockerfile
+-rw-r--r--   0        0        0        0 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/app/__init__.py
+-rw-r--r--   0        0        0     2659 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/app/streamlit_app.py
+-rw-r--r--   0        0        0     7736 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/builder.py
+-rw-r--r--   0        0        0     6368 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/conf.py
+-rw-r--r--   0        0        0     4955 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/factory.py
+-rw-r--r--   0        0        0     2113 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/logger.py
+-rwxr-xr-x   0        0        0     4044 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/main.py
+-rw-r--r--   0        0        0     7608 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/model.py
+-rw-r--r--   0        0        0     7272 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/parse.py
+-rw-r--r--   0        0        0     6419 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/preprocess.py
+-rw-r--r--   0        0        0     3991 2023-08-01 11:08:10.562980 readmeai-0.1.3/readmeai/utils.py
+-rw-r--r--   0        0        0    19008 1970-01-01 00:00:00.000000 readmeai-0.1.3/PKG-INFO
```

### Comparing `readmeai-0.1.2/LICENSE` & `readmeai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.2/README.md` & `readmeai-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 ## 📖 Table of Contents
 
 - [📖 Table of Contents](#-table-of-contents)
 - [📍 Overview](#-overview)
     - [🎯 *Motivation*](#-motivation)
     - [⚠️ *Disclaimer*](#️-disclaimer)
 - [👾 Demo](#-demo)
-    - [*🤖 Streamlit UI (experimental)*](#-streamlit-ui-experimental)
 - [⚙️ Features](#️-features)
 - [🚀 Getting Started](#-getting-started)
   - [✔️ Dependencies](#️-dependencies)
     - [📂 Repository](#-repository)
     - [🔐 OpenAI API](#-openai-api)
   - [📦 Installation](#-installation)
   - [🎮 Using *README-AI*](#-using-readme-ai)
@@ -70,17 +69,18 @@
 
 ## 👾 Demo
 
 <a href="https://youtu.be/pl-VcVfGbbk">
     <img src="https://raw.githubusercontent.com/eli64s/readme-ai/f0c5a038f63ae04b2d4452974676a92db42be8ce/examples/imgs/demo.png" alt="demo-video">
 </a>
 
-#### *🤖 Streamlit UI (experimental)*
+<!-- #### *🤖 Streamlit UI (experimental)*
 
 > Try out the *readme-ai* app in your browser using this [link!](https://readme-ai.streamlit.app/)
+-->
 
 ---
 
 ## ⚙️ Features
 
 <h1 align="center">1.<br>👇<br><br>📑 Codebase Documentation</h1>
 <table>
@@ -334,38 +334,43 @@
 ```sh
 docker pull zeroxeli/readme-ai:latest
 ```
 
 If you prefer to install the project dependencies locally, follow the steps below.
 
 1. Clone the *readme-ai* repository to your machine.
+
 ```sh
 git clone https://github.com/eli64s/readme-ai
 ```
 
 2. Navigate to the *readme-ai* directory.
+
 ```sh
 cd readme-ai
 ```
 
 3. Install the project dependencies using one of the following methods.
 
 > *Bash*
+
 ```sh
 bash setup/setup.sh
 ```
 
 > *Conda*
+
 ```sh
 conda create -n readmeai python=3.9 -y && \
 conda activate readmeai && \
 pip install -r requirements.txt
 ```
 
 > *Poetry*
+
 ```sh
 poetry install
 ```
 
 ### 🎮 Using *README-AI*
 
 Use the command-line to provide the OpenAI API key (if not already set) and specify an output path for your README file, along with the path to your local repository or remote code repository. You can also provide the output path in the [configuration file](./conf/conf.toml)
@@ -377,38 +382,42 @@
 - `-r` or `--repository`: The URL or path to your code repository.
 - `-t` or `--template`: The README template format to use. (coming soon!)
 - `l` or `--language`: The language of text written in the README file (coming soon!)
 
 Use any of the following methods to run the *readme-ai* CLI application.
 
 > *Pip ([PyPI Package](https://pypi.org/project/readmeai/))*
+
 ```sh
 readmeai --api-key "YOUR_API_KEY" --output readme-ai.md --repository https://github.com/eli64s/readme-ai
 
 # Or export your OpenAI API key as an environment variable
 export OPENAI_API_KEY="YOUR_API_KEY"
 readmeai -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 > *Docker ([Docker Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-ai/general))*
+
 ```sh
 docker run -it \
 -e OPENAI_API_KEY="YOUR_API_KEY" \
 -v "$(pwd)":/app zeroxeli/readme-ai:latest \
 readmeai -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 > *Conda*
+
 ```sh
 conda activate readmeai
 export OPENAI_API_KEY="YOUR_API_KEY"
 python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 > *Poetry*
+
 ```sh
 poetry shell
 export OPENAI_API_KEY="YOUR_API_KEY"
 poetry run python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 ### 🧪 Running Tests
```

#### html2text {}

```diff
@@ -4,16 +4,15 @@
      **** â¦ Generate beautiful and informative README.md documents. ****
         **** â¦ Developed with OpenAI's GPT language model APIs. ****
 
            [Markdown] [OpenAI] [Python] [pytest] [Docker] [actions]
     [pypi-version] [pypi-python-version] [pypi-downloads] [github-license]
 --- ## ð Table of Contents - [ð Table of Contents](#-table-of-contents) -
 [ð Overview](#-overview) - [ð¯ *Motivation*](#-motivation) - [â ï¸
-*Disclaimer*](#ï¸-disclaimer) - [ð¾ Demo](#-demo) - [*ð¤ Streamlit UI
-(experimental)*](#-streamlit-ui-experimental) - [âï¸ Features](#ï¸-
+*Disclaimer*](#ï¸-disclaimer) - [ð¾ Demo](#-demo) - [âï¸ Features](#ï¸-
 features) - [ð Getting Started](#-getting-started) - [âï¸ Dependencies]
 (#ï¸-dependencies) - [ð Repository](#-repository) - [ð OpenAI API](#-
 openai-api) - [ð¦ Installation](#-installation) - [ð® Using *README-AI*](#-
 using-readme-ai) - [ð§ª Running Tests](#-running-tests) - [ð  Future
 Development](#-future-development) - [ð Changelog](#-changelog) - [ð¤
 Contributing](#-contributing) - [ð License](#-license) - [ð
 Acknowledgments](#-acknowledgments) --- ## ð Overview *README-AI* is a
@@ -30,17 +29,15 @@
 *README-AI* is currently under development and has an opinionated configuration
 and setup. While this tool provides an excellent starting point for
 documentation, its important to review all text generated by the OpenAI API to
 ensure it accurately represents your codebase. Ensure all content in your
 repository is free of sensitive information before executing. Additionally,
 frequently monitor your API usage and costs by visiting the [OpenAI API Usage
 Dashboard](https://platform.openai.com/account/usage). --- ## ð¾ Demo [demo-
-video] #### *ð¤ Streamlit UI (experimental)* > Try out the *readme-ai* app in
-your browser using this [link!](https://readme-ai.streamlit.app/) --- ## âï¸
-Features
+video]  --- ## âï¸ Features
                                    ****** 1.
                                      ð
 
                       ð Codebase Documentation ******
 **** â¦ Repository File Summaries ****
     * Code summaries are generated for each file via OpenAI's gpt-3.5-turbo
       engine.
```

### Comparing `readmeai-0.1.2/pyproject.toml` & `readmeai-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.1.2"
+version = "0.1.3"
 description = "🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
```

### Comparing `readmeai-0.1.2/readmeai/app.py` & `readmeai-0.1.3/readmeai/app/streamlit_app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """Streamlit app for README-AI."""
 
+import os
 import subprocess
 import time
-import os
 
 import streamlit as st
 
 
-def run_readmeai(api_key, output, repository):
+def run_cli(openai_api_key, output_path, repository_path):
     """Run the README-AI CLI."""
-    if not output or not repository:
+    if not output_path or not repository_path:
         st.error("Output path and repository path must be provided.")
         return
 
     command = [
         "readmeai",
         "-k",
-        api_key,
+        openai_api_key,
         "-o",
-        output,
+        output_path,
         "-r",
-        repository,
+        repository_path,
     ]
 
     st.session_state.generating = True
 
     with st.spinner("Generating README..."):
         try:
             result = subprocess.run(command, check=True, capture_output=True, text=True)
             time.sleep(1)
 
             if result.returncode == 0:
                 st.success("README-AI executed successfully!")
                 try:
-                    with open(output, "r", encoding="utf-8") as readme_file:
+                    with open(output_path, "r", encoding="utf-8") as readme_file:
                         readme_content = readme_file.read()
                         st.subheader("Generated README.md:")
                         st.code(readme_content, language="markdown")
                         st.download_button(
                             "Download README.md",
                             data=readme_content,
                             file_name="README.md",
@@ -54,24 +54,27 @@
             st.session_state.generating = False
 
 
 def main():
     """Streamlit app entrypoint."""
     st.title("🤖 README-AI")
     st.write(
-        "Provide your OpenAI API key, the output path and the repository path...and we'll do the rest! 🚀"
+        "Enter your repository details and click run...we'll generate a README.md for you!"
     )
 
-    api_key = st.text_input("OpenAI API Key", type="password")
-    os.environ["OPENAI_API_KEY"] = api_key
-    output_path = st.text_input("Output File:")
-    repository_path = st.text_input("Repository:")
-
-    if st.button("Run"):
-        run_readmeai(api_key, output_path, repository_path)
+    openai_api_key = st.text_input("OpenAI API Key:", type="password")
+    output_path = st.text_input("Output file path:")
+    repository_path = st.text_input("Repository url or path:")
+
+    if st.button(
+        "Run",
+        key="run_button",
+        on_click=run_cli,
+        args=(openai_api_key, output_path, repository_path),
+    ):
         if "generating" not in st.session_state or not st.session_state.generating:
             st.session_state.generating = False
             with st.empty():
                 progress_bar = st.progress(0)
                 for i in range(1, 101):
                     time.sleep(0.02)
                     progress_bar.progress(i)
```

### Comparing `readmeai-0.1.2/readmeai/builder.py` & `readmeai-0.1.3/readmeai/builder.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.2/readmeai/conf.py` & `readmeai-0.1.3/readmeai/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,23 @@
     endpoint: str
     engine: str
     encoding: str
     rate_limit: int
     tokens: int
     tokens_max: int
     temperature: float
-    api_key: SecretStr = Field(default_factory=lambda: os.environ["OPENAI_API_KEY"])
+    api_key: SecretStr = Field(
+        default_factory=lambda: os.environ.get("OPENAI_API_KEY", "")
+    )
 
     @validator("api_key")
     def validate_api_key(cls, api_key) -> None:
         """Validate the OpenAI API key."""
         if not api_key:
-            api_key = os.environ.get("OPENAI_API_KEY")
+            api_key = os.environ.get("OPENAI_API_KEY", "")
         if not api_key:
             raise ValueError("Exception: invalid OpenAI API key.")
 
         os.environ["OPENAI_API_KEY"] = api_key
 
         try:
             cls._set_openai_api_key()
```

### Comparing `readmeai-0.1.2/readmeai/factory.py` & `readmeai-0.1.3/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.2/readmeai/logger.py` & `readmeai-0.1.3/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.2/readmeai/main.py` & `readmeai-0.1.3/readmeai/main.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.2/readmeai/model.py` & `readmeai-0.1.3/readmeai/model.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.2/readmeai/parse.py` & `readmeai-0.1.3/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.2/readmeai/preprocess.py` & `readmeai-0.1.3/readmeai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.2/readmeai/utils.py` & `readmeai-0.1.3/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.2/PKG-INFO` & `readmeai-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.1.2
+Version: 0.1.3
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
 Keywords: readme,python-cli,readme-template,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,openai-python,chatgpt-python,gpt-35-turbo,gpt-4-api,openai-cli,llm-prompting,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
 Requires-Python: >3.9.7,<4.0.0
@@ -64,15 +64,14 @@
 ## 📖 Table of Contents
 
 - [📖 Table of Contents](#-table-of-contents)
 - [📍 Overview](#-overview)
     - [🎯 *Motivation*](#-motivation)
     - [⚠️ *Disclaimer*](#️-disclaimer)
 - [👾 Demo](#-demo)
-    - [*🤖 Streamlit UI (experimental)*](#-streamlit-ui-experimental)
 - [⚙️ Features](#️-features)
 - [🚀 Getting Started](#-getting-started)
   - [✔️ Dependencies](#️-dependencies)
     - [📂 Repository](#-repository)
     - [🔐 OpenAI API](#-openai-api)
   - [📦 Installation](#-installation)
   - [🎮 Using *README-AI*](#-using-readme-ai)
@@ -102,17 +101,18 @@
 
 ## 👾 Demo
 
 <a href="https://youtu.be/pl-VcVfGbbk">
     <img src="https://raw.githubusercontent.com/eli64s/readme-ai/f0c5a038f63ae04b2d4452974676a92db42be8ce/examples/imgs/demo.png" alt="demo-video">
 </a>
 
-#### *🤖 Streamlit UI (experimental)*
+<!-- #### *🤖 Streamlit UI (experimental)*
 
 > Try out the *readme-ai* app in your browser using this [link!](https://readme-ai.streamlit.app/)
+-->
 
 ---
 
 ## ⚙️ Features
 
 <h1 align="center">1.<br>👇<br><br>📑 Codebase Documentation</h1>
 <table>
@@ -366,38 +366,43 @@
 ```sh
 docker pull zeroxeli/readme-ai:latest
 ```
 
 If you prefer to install the project dependencies locally, follow the steps below.
 
 1. Clone the *readme-ai* repository to your machine.
+
 ```sh
 git clone https://github.com/eli64s/readme-ai
 ```
 
 2. Navigate to the *readme-ai* directory.
+
 ```sh
 cd readme-ai
 ```
 
 3. Install the project dependencies using one of the following methods.
 
 > *Bash*
+
 ```sh
 bash setup/setup.sh
 ```
 
 > *Conda*
+
 ```sh
 conda create -n readmeai python=3.9 -y && \
 conda activate readmeai && \
 pip install -r requirements.txt
 ```
 
 > *Poetry*
+
 ```sh
 poetry install
 ```
 
 ### 🎮 Using *README-AI*
 
 Use the command-line to provide the OpenAI API key (if not already set) and specify an output path for your README file, along with the path to your local repository or remote code repository. You can also provide the output path in the [configuration file](./conf/conf.toml)
@@ -409,38 +414,42 @@
 - `-r` or `--repository`: The URL or path to your code repository.
 - `-t` or `--template`: The README template format to use. (coming soon!)
 - `l` or `--language`: The language of text written in the README file (coming soon!)
 
 Use any of the following methods to run the *readme-ai* CLI application.
 
 > *Pip ([PyPI Package](https://pypi.org/project/readmeai/))*
+
 ```sh
 readmeai --api-key "YOUR_API_KEY" --output readme-ai.md --repository https://github.com/eli64s/readme-ai
 
 # Or export your OpenAI API key as an environment variable
 export OPENAI_API_KEY="YOUR_API_KEY"
 readmeai -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 > *Docker ([Docker Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-ai/general))*
+
 ```sh
 docker run -it \
 -e OPENAI_API_KEY="YOUR_API_KEY" \
 -v "$(pwd)":/app zeroxeli/readme-ai:latest \
 readmeai -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 > *Conda*
+
 ```sh
 conda activate readmeai
 export OPENAI_API_KEY="YOUR_API_KEY"
 python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 > *Poetry*
+
 ```sh
 poetry shell
 export OPENAI_API_KEY="YOUR_API_KEY"
 poetry run python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 ### 🧪 Running Tests
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: readmeai Version: 0.1.2 Summary: ð Generate
+Metadata-Version: 2.1 Name: readmeai Version: 0.1.3 Summary: ð Generate
 awesome README.md files from the terminal, powered by OpenAI's GPT language
 model APIs ð« Home-page: https://github.com/eli64s/readme-ai License: MIT
 Keywords: readme,python-cli,readme-template,readme-md,awesome-readme,readme-
 generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,openai-
 python,chatgpt-python,gpt-35-turbo,gpt-4-api,openai-cli,llm-prompting,llm-agent
 Author: Eli Author-email: 0x.eli.64s@gmail.com Requires-Python: >3.9.7,<4.0.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
@@ -24,16 +24,15 @@
      **** â¦ Generate beautiful and informative README.md documents. ****
         **** â¦ Developed with OpenAI's GPT language model APIs. ****
 
            [Markdown] [OpenAI] [Python] [pytest] [Docker] [actions]
     [pypi-version] [pypi-python-version] [pypi-downloads] [github-license]
 --- ## ð Table of Contents - [ð Table of Contents](#-table-of-contents) -
 [ð Overview](#-overview) - [ð¯ *Motivation*](#-motivation) - [â ï¸
-*Disclaimer*](#ï¸-disclaimer) - [ð¾ Demo](#-demo) - [*ð¤ Streamlit UI
-(experimental)*](#-streamlit-ui-experimental) - [âï¸ Features](#ï¸-
+*Disclaimer*](#ï¸-disclaimer) - [ð¾ Demo](#-demo) - [âï¸ Features](#ï¸-
 features) - [ð Getting Started](#-getting-started) - [âï¸ Dependencies]
 (#ï¸-dependencies) - [ð Repository](#-repository) - [ð OpenAI API](#-
 openai-api) - [ð¦ Installation](#-installation) - [ð® Using *README-AI*](#-
 using-readme-ai) - [ð§ª Running Tests](#-running-tests) - [ð  Future
 Development](#-future-development) - [ð Changelog](#-changelog) - [ð¤
 Contributing](#-contributing) - [ð License](#-license) - [ð
 Acknowledgments](#-acknowledgments) --- ## ð Overview *README-AI* is a
@@ -50,17 +49,15 @@
 *README-AI* is currently under development and has an opinionated configuration
 and setup. While this tool provides an excellent starting point for
 documentation, its important to review all text generated by the OpenAI API to
 ensure it accurately represents your codebase. Ensure all content in your
 repository is free of sensitive information before executing. Additionally,
 frequently monitor your API usage and costs by visiting the [OpenAI API Usage
 Dashboard](https://platform.openai.com/account/usage). --- ## ð¾ Demo [demo-
-video] #### *ð¤ Streamlit UI (experimental)* > Try out the *readme-ai* app in
-your browser using this [link!](https://readme-ai.streamlit.app/) --- ## âï¸
-Features
+video]  --- ## âï¸ Features
                                    ****** 1.
                                      ð
 
                       ð Codebase Documentation ******
 **** â¦ Repository File Summaries ****
     * Code summaries are generated for each file via OpenAI's gpt-3.5-turbo
       engine.
```

