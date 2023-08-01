# Comparing `tmp/readmeai-0.1.1.tar.gz` & `tmp/readmeai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.1.1.tar", max compression
+gzip compressed data, was "readmeai-0.1.2.tar", max compression
```

## Comparing `readmeai-0.1.1.tar` & `readmeai-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-07-31 10:58:03.775669 readmeai-0.1.1/LICENSE
--rw-r--r--   0        0        0    17931 2023-07-31 10:58:03.775669 readmeai-0.1.1/README.md
--rw-r--r--   0        0        0     2072 2023-07-31 10:58:03.823673 readmeai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/__init__.py
--rw-r--r--   0        0        0     7736 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/builder.py
--rw-r--r--   0        0        0     6342 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/conf.py
--rw-r--r--   0        0        0     4955 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/factory.py
--rw-r--r--   0        0        0     2113 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/logger.py
--rwxr-xr-x   0        0        0     4044 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/main.py
--rw-r--r--   0        0        0     7608 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/model.py
--rw-r--r--   0        0        0     7272 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/parse.py
--rw-r--r--   0        0        0     6419 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/preprocess.py
--rw-r--r--   0        0        0     3991 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/utils.py
--rw-r--r--   0        0        0    19409 1970-01-01 00:00:00.000000 readmeai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-01 04:17:58.917739 readmeai-0.1.2/LICENSE
+-rw-r--r--   0        0        0    17592 2023-08-01 04:17:58.917739 readmeai-0.1.2/README.md
+-rw-r--r--   0        0        0     2101 2023-08-01 04:17:58.965740 readmeai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/__init__.py
+-rw-r--r--   0        0        0     2582 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/app.py
+-rw-r--r--   0        0        0     7736 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/builder.py
+-rw-r--r--   0        0        0     6342 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/conf.py
+-rw-r--r--   0        0        0     4955 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/factory.py
+-rw-r--r--   0        0        0     2113 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/logger.py
+-rwxr-xr-x   0        0        0     4044 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/main.py
+-rw-r--r--   0        0        0     7608 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/model.py
+-rw-r--r--   0        0        0     7272 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/parse.py
+-rw-r--r--   0        0        0     6419 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/preprocess.py
+-rw-r--r--   0        0        0     3991 2023-08-01 04:17:58.965740 readmeai-0.1.2/readmeai/utils.py
+-rw-r--r--   0        0        0    19062 1970-01-01 00:00:00.000000 readmeai-0.1.2/PKG-INFO
```

### Comparing `readmeai-0.1.1/LICENSE` & `readmeai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.1/README.md` & `readmeai-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,34 +12,35 @@
         <img src="https://img.shields.io/badge/OpenAI-412991.svg?stylee&logo=OpenAI&logoColor=white" alt="OpenAI" />
         <img src="https://img.shields.io/badge/Python-3776AB.svg?stylee&logo=Python&logoColor=white" alt="Python" />
         <img src="https://img.shields.io/badge/Pytest-0A9EDC.svg?stylee&logo=Pytest&logoColor=white" alt="pytest" />
         <img src="https://img.shields.io/badge/Docker-2496ED.svg?style&logo=Docker&logoColor=white" alt="Docker" />
         <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style&logo=GitHub-Actions&logoColor=white" alt="actions" />
     </p>
     <a href="https://pypi.org/project/readmeai/">
-        <img src="https://img.shields.io/pypi/v/readmeai?color=5D6D7E&logo=python" alt="PyPI - License" />
+        <img src="https://img.shields.io/pypi/v/readmeai?color=5D6D7E&logo=pypi" alt="pypi-version" />
     </a>
     <a href="https://pypi.org/project/readmeai/">
-        <img src="https://img.shields.io/pypi/pyversions/readmeai?color=5D6D7E&logo=python" alt="PyPI - Python Version" />
+        <img src="https://img.shields.io/pypi/pyversions/readmeai?color=5D6D7E&logo=python" alt="pypi-python-version" />
     </a>
     <a href="https://pypi.org/project/readmeai/">
-        <img src="https://img.shields.io/pypi/dm/readmeai?color=5D6D7E" alt="PyPI - Downloads" />
+        <img src="https://img.shields.io/pypi/dm/readmeai?color=5D6D7E" alt="pypi-downloads" />
     </a>
-    <img src="https://img.shields.io/github/license/eli64s/README-AI?color=5D6D7E" alt="GitHub license" />
+    <img src="https://img.shields.io/github/license/eli64s/readme-ai?color=5D6D7E" alt="github-license" />
 </div>
 
 ---
 
 ## 📖 Table of Contents
 
 - [📖 Table of Contents](#-table-of-contents)
 - [📍 Overview](#-overview)
     - [🎯 *Motivation*](#-motivation)
     - [⚠️ *Disclaimer*](#️-disclaimer)
 - [👾 Demo](#-demo)
+    - [*🤖 Streamlit UI (experimental)*](#-streamlit-ui-experimental)
 - [⚙️ Features](#️-features)
 - [🚀 Getting Started](#-getting-started)
   - [✔️ Dependencies](#️-dependencies)
     - [📂 Repository](#-repository)
     - [🔐 OpenAI API](#-openai-api)
   - [📦 Installation](#-installation)
   - [🎮 Using *README-AI*](#-using-readme-ai)
@@ -66,17 +67,21 @@
 Additionally, frequently monitor your API usage and costs by visiting the [OpenAI API Usage Dashboard](https://platform.openai.com/account/usage).
 
 ---
 
 ## 👾 Demo
 
 <a href="https://youtu.be/pl-VcVfGbbk">
-    <img src="https://raw.githubusercontent.com/eli64s/readme-ai/f0c5a038f63ae04b2d4452974676a92db42be8ce/examples/imgs/demo.png" alt="demo video">
+    <img src="https://raw.githubusercontent.com/eli64s/readme-ai/f0c5a038f63ae04b2d4452974676a92db42be8ce/examples/imgs/demo.png" alt="demo-video">
 </a>
 
+#### *🤖 Streamlit UI (experimental)*
+
+> Try out the *readme-ai* app in your browser using this [link!](https://readme-ai.streamlit.app/)
+
 ---
 
 ## ⚙️ Features
 
 <h1 align="center">1.<br>👇<br><br>📑 Codebase Documentation</h1>
 <table>
     <tr>
@@ -166,113 +171,103 @@
     <tr>
         <td>
             <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/imgs/getting_started.png" alt="getting_started">
         </td>
     </tr>
 </table>
 
-<h1 align="center">⒍<br>👇<br><br>👩‍💻Contributing Guidelines & more!</h1>
+<h1 align="center">⒍<br>👇<br><br>👩‍💻 Contributing Guidelines & more!</h1>
 
 | |
 |-----------------------------------------------|
 | ![contribute](https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/imgs/closing.png) |
 
 <h1 align="center">⒎<br>👇<br><br>💥 Example Files</h1>
-<p align="center">Markdown example files generated by the README-AI app!</p>
-<div align="center">
-    <table align="center">
-        <tr>
-            <th></th>
-            <th>Example File</th>
-            <th>Repository</th>
-            <th>Language</th>
-            <th>Bytes</th>
-        </tr>
-        <tr>
-            <td>1️⃣</td>
-            <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-python.md">readme-python.md</a></td>
-            <td><a href="https://github.com/eli64s/readme-ai">readme-ai</a></td>
-            <td>Python</td>
-            <td>
-                <p>19,839</p>
-        </tr>
+<p align="center">Markdown example files generated by the <i>readme-ai</i> app!</p>
+<table align="center">
+    <tr>
+        <th></th>
+        <th>Example File</th>
+        <th>Repository</th>
+        <th>Language</th>
+        <th>Bytes</th>
+    </tr>
+    <tr>
+        <td>1️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-python.md">readme-python.md</a></td>
+        <td><a href="https://github.com/eli64s/readme-ai">readme-ai</a></td>
+        <td>Python</td>
+        <td>
+            <p>19,839</p>
+        </td>
+    </tr>
+    <tr>
         <td>2️⃣</td>
         <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-typescript.md">readme-typescript.md</a></td>
         <td><a href="https://github.com/Yuberley/ChatGPT-App-React-Native-TypeScript">chatgpt-app-react-typescript</a></td>
         <td>TypeScript, React</td>
-        <td>
-            <p>988</p>
-            </tr>
-            <tr>
-                <td>3️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-javascript.md">readme-javascript.md</a></td>
-                <td><a href="https://github.com/idosal/assistant-chat-gpt">assistant-chat-gpt-javascript</a></td>
-                <td>JavaScript, React</td>
-                <td>
-                    <p>212</p>
-            </tr>
-            <tr>
-                <td>4️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-kotlin.md">readme-kotlin.md</a></td>
-                <td><a href="https://github.com/rumaan/file.io-Android-Client">file.io-android-client</a></td>
-                <td>Kotlin, Java, Android</td>
-                <td>
-                    <p>113,649</p>
-            </tr>
-            <tr>
-                <td>5️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-rust-c.md">readme-rust-c.md</a></td>
-                <td><a href="https://github.com/DownWithUp/CallMon">rust-c-app</a></td>
-                <td>C, Rust</td>
-                <td>
-                    <p>72</p>
-            </tr>
-            <tr>
-                <td>6️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-go.md">readme-go.md</a></td>
-                <td><a href="https://github.com/olliefr/docker-gs-ping">go-docker-app</a></td>
-                <td>Go</td>
-                <td>
-                    <p>41</p>
-            </tr>
-            <tr>
-                <td>7️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-java.md">readme-java.md</a></td>
-                <td><a href="https://github.com/avjinder/Minimal-Todo">java-minimal-todo</a></td>
-                <td>Java</td>
-                <td>
-                    <p>17,725</p>
-            </tr>
-            <tr>
-                <td>8️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-fastapi-redis.md">readme-fastapi-redis.md</a></td>
-                <td><a href="https://github.com/FerrariDG/async-ml-inference">async-ml-inference</a></td>
-                <td>Python, FastAPI, Redis</td>
-                <td>
-                    <p>355</p>
-            </tr>
-            <tr>
-                <td>9️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-mlops.md">readme-mlops.md</a></td>
-                <td><a href="https://github.com/GokuMohandas/mlops-course">mlops-course</a></td>
-                <td>Python, Jupyter</td>
-                <td>
-                    <p>8,524</p>
-            </tr>
-            <tr>
-                <td>🔟</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-pyflink.md">readme-pyflink.md</a></td>
-                <td><a href="https://github.com/eli64s/flink-flow">flink-flow</a></td>
-                <td>PyFlink</td>
-                <td>
-                    <p>32</p>
-            </tr>
-    </table>
-</div>
-
+        <td><p>988</p></td>
+    </tr>
+    <tr>
+        <td>3️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-javascript.md">readme-javascript.md</a></td>
+        <td><a href="https://github.com/idosal/assistant-chat-gpt">assistant-chat-gpt-javascript</a></td>
+        <td>JavaScript, React</td>
+        <td><p>212</p></td>
+    </tr>
+    <tr>
+        <td>4️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-kotlin.md">readme-kotlin.md</a></td>
+        <td><a href="https://github.com/rumaan/file.io-Android-Client">file.io-android-client</a></td>
+        <td>Kotlin, Java, Android</td>
+        <td><p>113,649</p></td>
+    </tr>
+    <tr>
+        <td>5️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-rust-c.md">readme-rust-c.md</a></td>
+        <td><a href="https://github.com/DownWithUp/CallMon">rust-c-app</a></td>
+        <td>C, Rust</td>
+        <td><p>72</p></td>
+    </tr>
+    <tr>
+        <td>6️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-go.md">readme-go.md</a></td>
+        <td><a href="https://github.com/olliefr/docker-gs-ping">go-docker-app</a></td>
+        <td>Go</td>
+        <td><p>41</p></td>
+    </tr>
+    <tr>
+        <td>7️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-java.md">readme-java.md</a></td>
+        <td><a href="https://github.com/avjinder/Minimal-Todo">java-minimal-todo</a></td>
+        <td>Java</td>
+        <td><p>17,725</p></td>
+    </tr>
+    <tr>
+        <td>8️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-fastapi-redis.md">readme-fastapi-redis.md</a></td>
+        <td><a href="https://github.com/FerrariDG/async-ml-inference">async-ml-inference</a></td>
+        <td>Python, FastAPI, Redis</td>
+        <td><p>355</p></td>
+    </tr>
+    <tr>
+        <td>9️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-mlops.md">readme-mlops.md</a></td>
+        <td><a href="https://github.com/GokuMohandas/mlops-course">mlops-course</a></td>
+        <td>Python, Jupyter</td>
+        <td><p>8,524</p></td>
+    </tr>
+    <tr>
+        <td>🔟</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-pyflink.md">readme-pyflink.md</a></td>
+        <td><a href="https://github.com/eli64s/flink-flow">flink-flow</a></td>
+        <td>PyFlink</td>
+        <td><p>32</p></td>
+    </tr>
+</table>
 
 <h1 align="center">⒏<br>👇<br><br>📜 Custom README templates coming soon!</h1>
 <p align="center">Developing a feature that allows users to select from a variety of README formats and styles.</p>
 <p align="center">Custom templates will be tailored for use-cases such as data, ai & ml, research, minimal, and more!</p>
 
 <p align="right">
     <a href="#top"><b>🔝 Return </b></a>
@@ -282,17 +277,17 @@
 
 ## 🚀 Getting Started
 
 ### ✔️ Dependencies
 
 Before you begin, ensure that you have the following prerequisites installed:
 
-- Python 3.9 or higher
-- Conda or Poetry package manager (recommended)
-- Access to the OpenAI API (see the setup guide below)
+- Python 3.9, 3.10, 3.11
+- Pip, Poetry, Conda, or Docker (see installation methods below)
+- OpenAI API account and api key (see setup instructions below)
 
 #### 📂 Repository
 
 Most user's will run *README-AI* using the command-line, specifying their repository on run-time. However, if you would like to use the default configuration, you will need to update the [configuration file](./conf/conf.toml) with your repository's remote URL or a local path to your codebase.
 
 ```toml
 [git]
@@ -324,36 +319,40 @@
 > - The generation of the README.md file should typically complete in under 1 minute. If it takes longer than a few minutes, please terminate the process.
 >
 
 ---
 
 ### 📦 Installation
 
-1. Clone the *readme-ai* repository to your machine.
+Use any of the following methods to install project dependencies.
+
+> *Pip ([PyPI Package](https://pypi.org/project/readmeai/))*
 ```sh
-git clone https://github.com/eli64s/readme-ai
+pip install readmeai
 ```
 
-2. Navigate to the *readme-ai* directory.
+> *Docker ([Docker Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-ai/general))*
 ```sh
-cd readme-ai
+docker pull zeroxeli/readme-ai:latest
 ```
 
-3. Use any of the following methods to install project dependencies.
+If you prefer to install the project dependencies locally, follow the steps below.
 
-> *Pip ([PyPI Package](https://pypi.org/project/readmeai/))*
+1. Clone the *readme-ai* repository to your machine.
 ```sh
-pip install readmeai
+git clone https://github.com/eli64s/readme-ai
 ```
 
-> *Docker ([Docker Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-ai/general))*
+2. Navigate to the *readme-ai* directory.
 ```sh
-docker pull zeroxeli/readme-ai:latest
+cd readme-ai
 ```
 
+3. Install the project dependencies using one of the following methods.
+
 > *Bash*
 ```sh
 bash setup/setup.sh
 ```
 
 > *Conda*
 ```sh
@@ -425,18 +424,18 @@
 </p>
 
 ---
 
 ## 🛠 Future Development
 
 - [X] Add additional language support for populating the *installation*, *usage*, and *test* README sections.
-- [X] Upload the *readme-ai* CLI tool to PyPI under the module name [readmeai](https://pypi.org/project/readmeai/).
+- [X] Publish the *readme-ai* CLI app to PyPI [readmeai](https://pypi.org/project/readmeai/).
+- [ ] Create user interface and serve the *readme-ai* app via streamlit.
 - [ ] Design and implement a variety of README template formats for different use-cases.
 - [ ] Add support for writing the README in any language (i.e. CN, ES, FR, JA, KO, RU).
-- [ ] Create UI with [Textual](https://github.com/Textualize/textual) or another framework to improve user experience.
 
 ---
 
 ## 📒 Changelog
 
 [Changelog](./CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
     ****** [https://img.icons8.com/?size=512&id=55494&format=png] [https://
              img.icons8.com/?size=512&id=kTuxVYRKeKEY&format=png]
                                README-AI ******
      **** â¦ Generate beautiful and informative README.md documents. ****
         **** â¦ Developed with OpenAI's GPT language model APIs. ****
 
            [Markdown] [OpenAI] [Python] [pytest] [Docker] [actions]
- [PyPI_-_License] [PyPI_-_Python_Version] [PyPI_-_Downloads] [GitHub license]
+    [pypi-version] [pypi-python-version] [pypi-downloads] [github-license]
 --- ## ð Table of Contents - [ð Table of Contents](#-table-of-contents) -
 [ð Overview](#-overview) - [ð¯ *Motivation*](#-motivation) - [â ï¸
-*Disclaimer*](#ï¸-disclaimer) - [ð¾ Demo](#-demo) - [âï¸ Features](#ï¸-
+*Disclaimer*](#ï¸-disclaimer) - [ð¾ Demo](#-demo) - [*ð¤ Streamlit UI
+(experimental)*](#-streamlit-ui-experimental) - [âï¸ Features](#ï¸-
 features) - [ð Getting Started](#-getting-started) - [âï¸ Dependencies]
 (#ï¸-dependencies) - [ð Repository](#-repository) - [ð OpenAI API](#-
 openai-api) - [ð¦ Installation](#-installation) - [ð® Using *README-AI*](#-
 using-readme-ai) - [ð§ª Running Tests](#-running-tests) - [ð  Future
 Development](#-future-development) - [ð Changelog](#-changelog) - [ð¤
 Contributing](#-contributing) - [ð License](#-license) - [ð
 Acknowledgments](#-acknowledgments) --- ## ð Overview *README-AI* is a
@@ -28,16 +29,18 @@
 to better understand and use open-source tools. #### â ï¸ *Disclaimer*
 *README-AI* is currently under development and has an opinionated configuration
 and setup. While this tool provides an excellent starting point for
 documentation, its important to review all text generated by the OpenAI API to
 ensure it accurately represents your codebase. Ensure all content in your
 repository is free of sensitive information before executing. Additionally,
 frequently monitor your API usage and costs by visiting the [OpenAI API Usage
-Dashboard](https://platform.openai.com/account/usage). --- ## ð¾ Demo [demo
-video] --- ## âï¸ Features
+Dashboard](https://platform.openai.com/account/usage). --- ## ð¾ Demo [demo-
+video] #### *ð¤ Streamlit UI (experimental)* > Try out the *readme-ai* app in
+your browser using this [link!](https://readme-ai.streamlit.app/) --- ## âï¸
+Features
                                    ****** 1.
                                      ð
 
                       ð Codebase Documentation ******
 **** â¦ Repository File Summaries ****
     * Code summaries are generated for each file via OpenAI's gpt-3.5-turbo
       engine.
@@ -79,24 +82,26 @@
     * Generates instructions for installing, using, and testing your codebase.
     * README-AI currently supports this feature for code written with:
           o Python, Rust, Go, C, Kotlin, Java, JavaScript, TypeScript.
 [getting_started]
                                   ****** â
                                      ð
 
-               ð©âð»Contributing Guidelines & more! ******
+              ð©âð» Contributing Guidelines & more! ******
 | | |-----------------------------------------------| | ![contribute](https://
 raw.githubusercontent.com/eli64s/readme-ai/main/examples/imgs/closing.png) |
                                   ****** â
                                      ð
 
                            ð¥ Example Files ******
-            Markdown example files generated by the README-AI app!
+            Markdown example files generated by the readme-ai app!
         Example File         Repository          Language               Bytes
 1ï¸�readme-python.md     readme-ai           Python                 19,839
+2ï¸�readme-typescript.md chatgpt-app-react-  TypeScript, React      988
+                             typescript
 3ï¸�readme-javascript.md assistant-chat-gpt- JavaScript, React      212
                              javascript
 4ï¸�readme-kotlin.md     file.io-android-    Kotlin, Java, Android  113,649
                              client
 5ï¸�readme-rust-c.md     rust-c-app          C, Rust                72
 6ï¸�readme-go.md         go-docker-app       Go                     41
 7ï¸�readme-java.md       java-minimal-todo   Java                   17,725
@@ -110,47 +115,50 @@
                ð Custom README templates coming soon! ******
    Developing a feature that allows users to select from a variety of README
                               formats and styles.
     Custom templates will be tailored for use-cases such as data, ai & ml,
                          research, minimal, and more!
                                                                     ð_Return
 --- ## ð Getting Started ### âï¸ Dependencies Before you begin, ensure
-that you have the following prerequisites installed: - Python 3.9 or higher -
-Conda or Poetry package manager (recommended) - Access to the OpenAI API (see
-the setup guide below) #### ð Repository Most user's will run *README-AI*
-using the command-line, specifying their repository on run-time. However, if
-you would like to use the default configuration, you will need to update the
-[configuration file](./conf/conf.toml) with your repository's remote URL or a
-local path to your codebase. ```toml [git] repository = "Insert your repository
-URL or local path here!" ``` #### ð OpenAI API To use the *README-AI* app,
-you must create an OpenAI API account and generate an API key. The steps below
-outline this process: OpenAI API User Guide 1. Go to the [OpenAI website]
-(https://platform.openai.com/). 2. Click the "Sign up for free" button. 3. Fill
-out the registration form with your information and agree to the terms of
-service. 4. Once logged in, click on the "API" tab. 5. Follow the instructions
-to create a new API key. 6. Copy the API key and keep it in a secure place.
+that you have the following prerequisites installed: - Python 3.9, 3.10, 3.11 -
+Pip, Poetry, Conda, or Docker (see installation methods below) - OpenAI API
+account and api key (see setup instructions below) #### ð Repository Most
+user's will run *README-AI* using the command-line, specifying their repository
+on run-time. However, if you would like to use the default configuration, you
+will need to update the [configuration file](./conf/conf.toml) with your
+repository's remote URL or a local path to your codebase. ```toml [git]
+repository = "Insert your repository URL or local path here!" ``` #### ð
+OpenAI API To use the *README-AI* app, you must create an OpenAI API account
+and generate an API key. The steps below outline this process: OpenAI API User
+Guide 1. Go to the [OpenAI website](https://platform.openai.com/). 2. Click the
+"Sign up for free" button. 3. Fill out the registration form with your
+information and agree to the terms of service. 4. Once logged in, click on the
+"API" tab. 5. Follow the instructions to create a new API key. 6. Copy the API
+key and keep it in a secure place.
 > **â ï¸ Note** > > - To maximize your experience with README-AI, it is
 recommended to set up a payment method on OpenAI's website. By doing so, you
 gain access to more powerful language models like gpt-3.5-turbo. Without a
 payment method, your usage will be restricted to the base gpt-3 models. This
 limitation might lead to less precise README files or potential errors during
 the generation process. > > - When using a payment method, make sure you have
 sufficient credits to run the README-AI application. Additionally, remember to
 regularly monitor your API usage and costs by visiting the [OpenAI API Usage
 Dashboard](https://platform.openai.com/account/usage). Please note that this
 API is not free and you will be charged for each request made, which can
 accumulate rapidly. > > - The generation of the README.md file should typically
 complete in under 1 minute. If it takes longer than a few minutes, please
-terminate the process. > --- ### ð¦ Installation 1. Clone the *readme-ai*
+terminate the process. > --- ### ð¦ Installation Use any of the following
+methods to install project dependencies. > *Pip ([PyPI Package](https://
+pypi.org/project/readmeai/))* ```sh pip install readmeai ``` > *Docker ([Docker
+Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-ai/general))*
+```sh docker pull zeroxeli/readme-ai:latest ``` If you prefer to install the
+project dependencies locally, follow the steps below. 1. Clone the *readme-ai*
 repository to your machine. ```sh git clone https://github.com/eli64s/readme-ai
-``` 2. Navigate to the *readme-ai* directory. ```sh cd readme-ai ``` 3. Use any
-of the following methods to install project dependencies. > *Pip ([PyPI
-Package](https://pypi.org/project/readmeai/))* ```sh pip install readmeai ``` >
-*Docker ([Docker Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-
-ai/general))* ```sh docker pull zeroxeli/readme-ai:latest ``` > *Bash* ```sh
+``` 2. Navigate to the *readme-ai* directory. ```sh cd readme-ai ``` 3. Install
+the project dependencies using one of the following methods. > *Bash* ```sh
 bash setup/setup.sh ``` > *Conda* ```sh conda create -n readmeai python=3.9 -
 y && \ conda activate readmeai && \ pip install -r requirements.txt ``` >
 *Poetry* ```sh poetry install ``` ### ð® Using *README-AI* Use the command-
 line to provide the OpenAI API key (if not already set) and specify an output
 path for your README file, along with the path to your local repository or
 remote code repository. You can also provide the output path in the
 [configuration file](./conf/conf.toml) Command-Line Arguments: - `-k` or `--
@@ -172,20 +180,19 @@
 ``` > *Poetry* ```sh poetry shell export OPENAI_API_KEY="YOUR_API_KEY" poetry
 run python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/
 readme-ai ``` ### ð§ª Running Tests Execute the following command to run the
 test suite. ```sh bash scripts/test.sh ```
                                                                     ð_Return
 --- ## ð  Future Development - [X] Add additional language support for
 populating the *installation*, *usage*, and *test* README sections. - [X]
-Upload the *readme-ai* CLI tool to PyPI under the module name [readmeai](https:
-//pypi.org/project/readmeai/). - [ ] Design and implement a variety of README
-template formats for different use-cases. - [ ] Add support for writing the
-README in any language (i.e. CN, ES, FR, JA, KO, RU). - [ ] Create UI with
-[Textual](https://github.com/Textualize/textual) or another framework to
-improve user experience. --- ## ð Changelog [Changelog](./CHANGELOG.md) --
-- ## ð¤ Contributing [Contributing Guidelines](./CONTRIBUTING.md) --- ## ð
-License [MIT](./LICENSE) --- ## ð Acknowledgments *Badges* - [Shields.io]
-(https://shields.io/) - [Aveek-Saha/GitHub-Profile-Badges](https://github.com/
-Aveek-Saha/GitHub-Profile-Badges) - [Ileriayo/Markdown-Badges](https://
-github.com/Ileriayo/markdown-badges)
+Publish the *readme-ai* CLI app to PyPI [readmeai](https://pypi.org/project/
+readmeai/). - [ ] Create user interface and serve the *readme-ai* app via
+streamlit. - [ ] Design and implement a variety of README template formats for
+different use-cases. - [ ] Add support for writing the README in any language
+(i.e. CN, ES, FR, JA, KO, RU). --- ## ð Changelog [Changelog](./
+CHANGELOG.md) --- ## ð¤ Contributing [Contributing Guidelines](./
+CONTRIBUTING.md) --- ## ð License [MIT](./LICENSE) --- ## ð
+Acknowledgments *Badges* - [Shields.io](https://shields.io/) - [Aveek-Saha/
+GitHub-Profile-Badges](https://github.com/Aveek-Saha/GitHub-Profile-Badges) -
+[Ileriayo/Markdown-Badges](https://github.com/Ileriayo/markdown-badges)
                                                                     ð_Return
 ---
```

### Comparing `readmeai-0.1.1/pyproject.toml` & `readmeai-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.1.1"
+version = "0.1.2"
 description = "🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
@@ -39,29 +39,30 @@
 isort = "*"
 pytest = "*"
 pytest-cov = "*"
 pre-commit = "*"
 ruff = "*"
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = ">3.9.7,<4.0.0"
 colorlog = "^6.7.0"
 cachetools = "^5.3.1"
 gitpython = "^3.1.31"
 httpx = "^0.24.1"
 h2 = "^4.1.0"
 openai = "^0.27.8"
 pyyaml = "^6.0"
 responses = "^0.23.1"
 tabulate = "^0.9.0"
 tenacity = "^8.2.2"
 tiktoken = "^0.4.0"
 toml = "^0.10.2"
 pydantic = "^1.10.9"
 click = "^8.1.6"
+streamlit = "^1.25.0"
 
 [tool.poetry.scripts]
 readmeai = "readmeai.main:cli"
 
 [tool.ruff]
 line-length = 88
 target-version = "py39"
```

### Comparing `readmeai-0.1.1/readmeai/builder.py` & `readmeai-0.1.2/readmeai/builder.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.1/readmeai/conf.py` & `readmeai-0.1.2/readmeai/conf.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.1/readmeai/factory.py` & `readmeai-0.1.2/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.1/readmeai/logger.py` & `readmeai-0.1.2/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.1/readmeai/main.py` & `readmeai-0.1.2/readmeai/main.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.1/readmeai/model.py` & `readmeai-0.1.2/readmeai/model.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.1/readmeai/parse.py` & `readmeai-0.1.2/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.1/readmeai/preprocess.py` & `readmeai-0.1.2/readmeai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.1/readmeai/utils.py` & `readmeai-0.1.2/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.1/PKG-INFO` & `readmeai-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.1.1
+Version: 0.1.2
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
 Keywords: readme,python-cli,readme-template,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,openai-python,chatgpt-python,gpt-35-turbo,gpt-4-api,openai-cli,llm-prompting,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >3.9.7,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cachetools (>=5.3.1,<6.0.0)
 Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: h2 (>=4.1.0,<5.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: responses (>=0.23.1,<0.24.0)
+Requires-Dist: streamlit (>=1.25.0,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://github.com/eli64s/readme-ai/blob/main/README.md
 Description-Content-Type: text/markdown
 
@@ -44,34 +44,35 @@
         <img src="https://img.shields.io/badge/OpenAI-412991.svg?stylee&logo=OpenAI&logoColor=white" alt="OpenAI" />
         <img src="https://img.shields.io/badge/Python-3776AB.svg?stylee&logo=Python&logoColor=white" alt="Python" />
         <img src="https://img.shields.io/badge/Pytest-0A9EDC.svg?stylee&logo=Pytest&logoColor=white" alt="pytest" />
         <img src="https://img.shields.io/badge/Docker-2496ED.svg?style&logo=Docker&logoColor=white" alt="Docker" />
         <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style&logo=GitHub-Actions&logoColor=white" alt="actions" />
     </p>
     <a href="https://pypi.org/project/readmeai/">
-        <img src="https://img.shields.io/pypi/v/readmeai?color=5D6D7E&logo=python" alt="PyPI - License" />
+        <img src="https://img.shields.io/pypi/v/readmeai?color=5D6D7E&logo=pypi" alt="pypi-version" />
     </a>
     <a href="https://pypi.org/project/readmeai/">
-        <img src="https://img.shields.io/pypi/pyversions/readmeai?color=5D6D7E&logo=python" alt="PyPI - Python Version" />
+        <img src="https://img.shields.io/pypi/pyversions/readmeai?color=5D6D7E&logo=python" alt="pypi-python-version" />
     </a>
     <a href="https://pypi.org/project/readmeai/">
-        <img src="https://img.shields.io/pypi/dm/readmeai?color=5D6D7E" alt="PyPI - Downloads" />
+        <img src="https://img.shields.io/pypi/dm/readmeai?color=5D6D7E" alt="pypi-downloads" />
     </a>
-    <img src="https://img.shields.io/github/license/eli64s/README-AI?color=5D6D7E" alt="GitHub license" />
+    <img src="https://img.shields.io/github/license/eli64s/readme-ai?color=5D6D7E" alt="github-license" />
 </div>
 
 ---
 
 ## 📖 Table of Contents
 
 - [📖 Table of Contents](#-table-of-contents)
 - [📍 Overview](#-overview)
     - [🎯 *Motivation*](#-motivation)
     - [⚠️ *Disclaimer*](#️-disclaimer)
 - [👾 Demo](#-demo)
+    - [*🤖 Streamlit UI (experimental)*](#-streamlit-ui-experimental)
 - [⚙️ Features](#️-features)
 - [🚀 Getting Started](#-getting-started)
   - [✔️ Dependencies](#️-dependencies)
     - [📂 Repository](#-repository)
     - [🔐 OpenAI API](#-openai-api)
   - [📦 Installation](#-installation)
   - [🎮 Using *README-AI*](#-using-readme-ai)
@@ -98,17 +99,21 @@
 Additionally, frequently monitor your API usage and costs by visiting the [OpenAI API Usage Dashboard](https://platform.openai.com/account/usage).
 
 ---
 
 ## 👾 Demo
 
 <a href="https://youtu.be/pl-VcVfGbbk">
-    <img src="https://raw.githubusercontent.com/eli64s/readme-ai/f0c5a038f63ae04b2d4452974676a92db42be8ce/examples/imgs/demo.png" alt="demo video">
+    <img src="https://raw.githubusercontent.com/eli64s/readme-ai/f0c5a038f63ae04b2d4452974676a92db42be8ce/examples/imgs/demo.png" alt="demo-video">
 </a>
 
+#### *🤖 Streamlit UI (experimental)*
+
+> Try out the *readme-ai* app in your browser using this [link!](https://readme-ai.streamlit.app/)
+
 ---
 
 ## ⚙️ Features
 
 <h1 align="center">1.<br>👇<br><br>📑 Codebase Documentation</h1>
 <table>
     <tr>
@@ -198,113 +203,103 @@
     <tr>
         <td>
             <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/imgs/getting_started.png" alt="getting_started">
         </td>
     </tr>
 </table>
 
-<h1 align="center">⒍<br>👇<br><br>👩‍💻Contributing Guidelines & more!</h1>
+<h1 align="center">⒍<br>👇<br><br>👩‍💻 Contributing Guidelines & more!</h1>
 
 | |
 |-----------------------------------------------|
 | ![contribute](https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/imgs/closing.png) |
 
 <h1 align="center">⒎<br>👇<br><br>💥 Example Files</h1>
-<p align="center">Markdown example files generated by the README-AI app!</p>
-<div align="center">
-    <table align="center">
-        <tr>
-            <th></th>
-            <th>Example File</th>
-            <th>Repository</th>
-            <th>Language</th>
-            <th>Bytes</th>
-        </tr>
-        <tr>
-            <td>1️⃣</td>
-            <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-python.md">readme-python.md</a></td>
-            <td><a href="https://github.com/eli64s/readme-ai">readme-ai</a></td>
-            <td>Python</td>
-            <td>
-                <p>19,839</p>
-        </tr>
+<p align="center">Markdown example files generated by the <i>readme-ai</i> app!</p>
+<table align="center">
+    <tr>
+        <th></th>
+        <th>Example File</th>
+        <th>Repository</th>
+        <th>Language</th>
+        <th>Bytes</th>
+    </tr>
+    <tr>
+        <td>1️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-python.md">readme-python.md</a></td>
+        <td><a href="https://github.com/eli64s/readme-ai">readme-ai</a></td>
+        <td>Python</td>
+        <td>
+            <p>19,839</p>
+        </td>
+    </tr>
+    <tr>
         <td>2️⃣</td>
         <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-typescript.md">readme-typescript.md</a></td>
         <td><a href="https://github.com/Yuberley/ChatGPT-App-React-Native-TypeScript">chatgpt-app-react-typescript</a></td>
         <td>TypeScript, React</td>
-        <td>
-            <p>988</p>
-            </tr>
-            <tr>
-                <td>3️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-javascript.md">readme-javascript.md</a></td>
-                <td><a href="https://github.com/idosal/assistant-chat-gpt">assistant-chat-gpt-javascript</a></td>
-                <td>JavaScript, React</td>
-                <td>
-                    <p>212</p>
-            </tr>
-            <tr>
-                <td>4️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-kotlin.md">readme-kotlin.md</a></td>
-                <td><a href="https://github.com/rumaan/file.io-Android-Client">file.io-android-client</a></td>
-                <td>Kotlin, Java, Android</td>
-                <td>
-                    <p>113,649</p>
-            </tr>
-            <tr>
-                <td>5️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-rust-c.md">readme-rust-c.md</a></td>
-                <td><a href="https://github.com/DownWithUp/CallMon">rust-c-app</a></td>
-                <td>C, Rust</td>
-                <td>
-                    <p>72</p>
-            </tr>
-            <tr>
-                <td>6️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-go.md">readme-go.md</a></td>
-                <td><a href="https://github.com/olliefr/docker-gs-ping">go-docker-app</a></td>
-                <td>Go</td>
-                <td>
-                    <p>41</p>
-            </tr>
-            <tr>
-                <td>7️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-java.md">readme-java.md</a></td>
-                <td><a href="https://github.com/avjinder/Minimal-Todo">java-minimal-todo</a></td>
-                <td>Java</td>
-                <td>
-                    <p>17,725</p>
-            </tr>
-            <tr>
-                <td>8️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-fastapi-redis.md">readme-fastapi-redis.md</a></td>
-                <td><a href="https://github.com/FerrariDG/async-ml-inference">async-ml-inference</a></td>
-                <td>Python, FastAPI, Redis</td>
-                <td>
-                    <p>355</p>
-            </tr>
-            <tr>
-                <td>9️⃣</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-mlops.md">readme-mlops.md</a></td>
-                <td><a href="https://github.com/GokuMohandas/mlops-course">mlops-course</a></td>
-                <td>Python, Jupyter</td>
-                <td>
-                    <p>8,524</p>
-            </tr>
-            <tr>
-                <td>🔟</td>
-                <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-pyflink.md">readme-pyflink.md</a></td>
-                <td><a href="https://github.com/eli64s/flink-flow">flink-flow</a></td>
-                <td>PyFlink</td>
-                <td>
-                    <p>32</p>
-            </tr>
-    </table>
-</div>
-
+        <td><p>988</p></td>
+    </tr>
+    <tr>
+        <td>3️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-javascript.md">readme-javascript.md</a></td>
+        <td><a href="https://github.com/idosal/assistant-chat-gpt">assistant-chat-gpt-javascript</a></td>
+        <td>JavaScript, React</td>
+        <td><p>212</p></td>
+    </tr>
+    <tr>
+        <td>4️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-kotlin.md">readme-kotlin.md</a></td>
+        <td><a href="https://github.com/rumaan/file.io-Android-Client">file.io-android-client</a></td>
+        <td>Kotlin, Java, Android</td>
+        <td><p>113,649</p></td>
+    </tr>
+    <tr>
+        <td>5️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-rust-c.md">readme-rust-c.md</a></td>
+        <td><a href="https://github.com/DownWithUp/CallMon">rust-c-app</a></td>
+        <td>C, Rust</td>
+        <td><p>72</p></td>
+    </tr>
+    <tr>
+        <td>6️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-go.md">readme-go.md</a></td>
+        <td><a href="https://github.com/olliefr/docker-gs-ping">go-docker-app</a></td>
+        <td>Go</td>
+        <td><p>41</p></td>
+    </tr>
+    <tr>
+        <td>7️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-java.md">readme-java.md</a></td>
+        <td><a href="https://github.com/avjinder/Minimal-Todo">java-minimal-todo</a></td>
+        <td>Java</td>
+        <td><p>17,725</p></td>
+    </tr>
+    <tr>
+        <td>8️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-fastapi-redis.md">readme-fastapi-redis.md</a></td>
+        <td><a href="https://github.com/FerrariDG/async-ml-inference">async-ml-inference</a></td>
+        <td>Python, FastAPI, Redis</td>
+        <td><p>355</p></td>
+    </tr>
+    <tr>
+        <td>9️⃣</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-mlops.md">readme-mlops.md</a></td>
+        <td><a href="https://github.com/GokuMohandas/mlops-course">mlops-course</a></td>
+        <td>Python, Jupyter</td>
+        <td><p>8,524</p></td>
+    </tr>
+    <tr>
+        <td>🔟</td>
+        <td><a href="https://github.com/eli64s/readme-ai/blob/main/examples/readme-pyflink.md">readme-pyflink.md</a></td>
+        <td><a href="https://github.com/eli64s/flink-flow">flink-flow</a></td>
+        <td>PyFlink</td>
+        <td><p>32</p></td>
+    </tr>
+</table>
 
 <h1 align="center">⒏<br>👇<br><br>📜 Custom README templates coming soon!</h1>
 <p align="center">Developing a feature that allows users to select from a variety of README formats and styles.</p>
 <p align="center">Custom templates will be tailored for use-cases such as data, ai & ml, research, minimal, and more!</p>
 
 <p align="right">
     <a href="#top"><b>🔝 Return </b></a>
@@ -314,17 +309,17 @@
 
 ## 🚀 Getting Started
 
 ### ✔️ Dependencies
 
 Before you begin, ensure that you have the following prerequisites installed:
 
-- Python 3.9 or higher
-- Conda or Poetry package manager (recommended)
-- Access to the OpenAI API (see the setup guide below)
+- Python 3.9, 3.10, 3.11
+- Pip, Poetry, Conda, or Docker (see installation methods below)
+- OpenAI API account and api key (see setup instructions below)
 
 #### 📂 Repository
 
 Most user's will run *README-AI* using the command-line, specifying their repository on run-time. However, if you would like to use the default configuration, you will need to update the [configuration file](./conf/conf.toml) with your repository's remote URL or a local path to your codebase.
 
 ```toml
 [git]
@@ -356,36 +351,40 @@
 > - The generation of the README.md file should typically complete in under 1 minute. If it takes longer than a few minutes, please terminate the process.
 >
 
 ---
 
 ### 📦 Installation
 
-1. Clone the *readme-ai* repository to your machine.
+Use any of the following methods to install project dependencies.
+
+> *Pip ([PyPI Package](https://pypi.org/project/readmeai/))*
 ```sh
-git clone https://github.com/eli64s/readme-ai
+pip install readmeai
 ```
 
-2. Navigate to the *readme-ai* directory.
+> *Docker ([Docker Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-ai/general))*
 ```sh
-cd readme-ai
+docker pull zeroxeli/readme-ai:latest
 ```
 
-3. Use any of the following methods to install project dependencies.
+If you prefer to install the project dependencies locally, follow the steps below.
 
-> *Pip ([PyPI Package](https://pypi.org/project/readmeai/))*
+1. Clone the *readme-ai* repository to your machine.
 ```sh
-pip install readmeai
+git clone https://github.com/eli64s/readme-ai
 ```
 
-> *Docker ([Docker Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-ai/general))*
+2. Navigate to the *readme-ai* directory.
 ```sh
-docker pull zeroxeli/readme-ai:latest
+cd readme-ai
 ```
 
+3. Install the project dependencies using one of the following methods.
+
 > *Bash*
 ```sh
 bash setup/setup.sh
 ```
 
 > *Conda*
 ```sh
@@ -457,18 +456,18 @@
 </p>
 
 ---
 
 ## 🛠 Future Development
 
 - [X] Add additional language support for populating the *installation*, *usage*, and *test* README sections.
-- [X] Upload the *readme-ai* CLI tool to PyPI under the module name [readmeai](https://pypi.org/project/readmeai/).
+- [X] Publish the *readme-ai* CLI app to PyPI [readmeai](https://pypi.org/project/readmeai/).
+- [ ] Create user interface and serve the *readme-ai* app via streamlit.
 - [ ] Design and implement a variety of README template formats for different use-cases.
 - [ ] Add support for writing the README in any language (i.e. CN, ES, FR, JA, KO, RU).
-- [ ] Create UI with [Textual](https://github.com/Textualize/textual) or another framework to improve user experience.
 
 ---
 
 ## 📒 Changelog
 
 [Changelog](./CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,38 +1,39 @@
-Metadata-Version: 2.1 Name: readmeai Version: 0.1.1 Summary: ð Generate
+Metadata-Version: 2.1 Name: readmeai Version: 0.1.2 Summary: ð Generate
 awesome README.md files from the terminal, powered by OpenAI's GPT language
 model APIs ð« Home-page: https://github.com/eli64s/readme-ai License: MIT
 Keywords: readme,python-cli,readme-template,readme-md,awesome-readme,readme-
 generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,openai-
 python,chatgpt-python,gpt-35-turbo,gpt-4-api,openai-cli,llm-prompting,llm-agent
-Author: Eli Author-email: 0x.eli.64s@gmail.com Requires-Python: >=3.8.1,<4.0.0
+Author: Eli Author-email: 0x.eli.64s@gmail.com Requires-Python: >3.9.7,<4.0.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: cachetools (>=5.3.1,<6.0.0) Requires-
-Dist: click (>=8.1.6,<9.0.0) Requires-Dist: colorlog (>=6.7.0,<7.0.0) Requires-
-Dist: gitpython (>=3.1.31,<4.0.0) Requires-Dist: h2 (>=4.1.0,<5.0.0) Requires-
-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pydantic (>=1.10.9,<2.0.0) Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: responses (>=0.23.1,<0.24.0) Requires-Dist: tabulate
-(>=0.9.0,<0.10.0) Requires-Dist: tenacity (>=8.2.2,<9.0.0) Requires-Dist:
-tiktoken (>=0.4.0,<0.5.0) Requires-Dist: toml (>=0.10.2,<0.11.0) Project-URL:
-Documentation, https://github.com/eli64s/readme-ai/blob/main/README.md
-Description-Content-Type: text/markdown
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: cachetools
+(>=5.3.1,<6.0.0) Requires-Dist: click (>=8.1.6,<9.0.0) Requires-Dist: colorlog
+(>=6.7.0,<7.0.0) Requires-Dist: gitpython (>=3.1.31,<4.0.0) Requires-Dist: h2
+(>=4.1.0,<5.0.0) Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: openai
+(>=0.27.8,<0.28.0) Requires-Dist: pydantic (>=1.10.9,<2.0.0) Requires-Dist:
+pyyaml (>=6.0,<7.0) Requires-Dist: responses (>=0.23.1,<0.24.0) Requires-Dist:
+streamlit (>=1.25.0,<2.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-
+Dist: tenacity (>=8.2.2,<9.0.0) Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0) Project-URL: Documentation, https://
+github.com/eli64s/readme-ai/blob/main/README.md Description-Content-Type: text/
+markdown
     ****** [https://img.icons8.com/?size=512&id=55494&format=png] [https://
              img.icons8.com/?size=512&id=kTuxVYRKeKEY&format=png]
                                README-AI ******
      **** â¦ Generate beautiful and informative README.md documents. ****
         **** â¦ Developed with OpenAI's GPT language model APIs. ****
 
            [Markdown] [OpenAI] [Python] [pytest] [Docker] [actions]
- [PyPI_-_License] [PyPI_-_Python_Version] [PyPI_-_Downloads] [GitHub license]
+    [pypi-version] [pypi-python-version] [pypi-downloads] [github-license]
 --- ## ð Table of Contents - [ð Table of Contents](#-table-of-contents) -
 [ð Overview](#-overview) - [ð¯ *Motivation*](#-motivation) - [â ï¸
-*Disclaimer*](#ï¸-disclaimer) - [ð¾ Demo](#-demo) - [âï¸ Features](#ï¸-
+*Disclaimer*](#ï¸-disclaimer) - [ð¾ Demo](#-demo) - [*ð¤ Streamlit UI
+(experimental)*](#-streamlit-ui-experimental) - [âï¸ Features](#ï¸-
 features) - [ð Getting Started](#-getting-started) - [âï¸ Dependencies]
 (#ï¸-dependencies) - [ð Repository](#-repository) - [ð OpenAI API](#-
 openai-api) - [ð¦ Installation](#-installation) - [ð® Using *README-AI*](#-
 using-readme-ai) - [ð§ª Running Tests](#-running-tests) - [ð  Future
 Development](#-future-development) - [ð Changelog](#-changelog) - [ð¤
 Contributing](#-contributing) - [ð License](#-license) - [ð
 Acknowledgments](#-acknowledgments) --- ## ð Overview *README-AI* is a
@@ -48,16 +49,18 @@
 to better understand and use open-source tools. #### â ï¸ *Disclaimer*
 *README-AI* is currently under development and has an opinionated configuration
 and setup. While this tool provides an excellent starting point for
 documentation, its important to review all text generated by the OpenAI API to
 ensure it accurately represents your codebase. Ensure all content in your
 repository is free of sensitive information before executing. Additionally,
 frequently monitor your API usage and costs by visiting the [OpenAI API Usage
-Dashboard](https://platform.openai.com/account/usage). --- ## ð¾ Demo [demo
-video] --- ## âï¸ Features
+Dashboard](https://platform.openai.com/account/usage). --- ## ð¾ Demo [demo-
+video] #### *ð¤ Streamlit UI (experimental)* > Try out the *readme-ai* app in
+your browser using this [link!](https://readme-ai.streamlit.app/) --- ## âï¸
+Features
                                    ****** 1.
                                      ð
 
                       ð Codebase Documentation ******
 **** â¦ Repository File Summaries ****
     * Code summaries are generated for each file via OpenAI's gpt-3.5-turbo
       engine.
@@ -99,24 +102,26 @@
     * Generates instructions for installing, using, and testing your codebase.
     * README-AI currently supports this feature for code written with:
           o Python, Rust, Go, C, Kotlin, Java, JavaScript, TypeScript.
 [getting_started]
                                   ****** â
                                      ð
 
-               ð©âð»Contributing Guidelines & more! ******
+              ð©âð» Contributing Guidelines & more! ******
 | | |-----------------------------------------------| | ![contribute](https://
 raw.githubusercontent.com/eli64s/readme-ai/main/examples/imgs/closing.png) |
                                   ****** â
                                      ð
 
                            ð¥ Example Files ******
-            Markdown example files generated by the README-AI app!
+            Markdown example files generated by the readme-ai app!
         Example File         Repository          Language               Bytes
 1ï¸�readme-python.md     readme-ai           Python                 19,839
+2ï¸�readme-typescript.md chatgpt-app-react-  TypeScript, React      988
+                             typescript
 3ï¸�readme-javascript.md assistant-chat-gpt- JavaScript, React      212
                              javascript
 4ï¸�readme-kotlin.md     file.io-android-    Kotlin, Java, Android  113,649
                              client
 5ï¸�readme-rust-c.md     rust-c-app          C, Rust                72
 6ï¸�readme-go.md         go-docker-app       Go                     41
 7ï¸�readme-java.md       java-minimal-todo   Java                   17,725
@@ -130,47 +135,50 @@
                ð Custom README templates coming soon! ******
    Developing a feature that allows users to select from a variety of README
                               formats and styles.
     Custom templates will be tailored for use-cases such as data, ai & ml,
                          research, minimal, and more!
                                                                     ð_Return
 --- ## ð Getting Started ### âï¸ Dependencies Before you begin, ensure
-that you have the following prerequisites installed: - Python 3.9 or higher -
-Conda or Poetry package manager (recommended) - Access to the OpenAI API (see
-the setup guide below) #### ð Repository Most user's will run *README-AI*
-using the command-line, specifying their repository on run-time. However, if
-you would like to use the default configuration, you will need to update the
-[configuration file](./conf/conf.toml) with your repository's remote URL or a
-local path to your codebase. ```toml [git] repository = "Insert your repository
-URL or local path here!" ``` #### ð OpenAI API To use the *README-AI* app,
-you must create an OpenAI API account and generate an API key. The steps below
-outline this process: OpenAI API User Guide 1. Go to the [OpenAI website]
-(https://platform.openai.com/). 2. Click the "Sign up for free" button. 3. Fill
-out the registration form with your information and agree to the terms of
-service. 4. Once logged in, click on the "API" tab. 5. Follow the instructions
-to create a new API key. 6. Copy the API key and keep it in a secure place.
+that you have the following prerequisites installed: - Python 3.9, 3.10, 3.11 -
+Pip, Poetry, Conda, or Docker (see installation methods below) - OpenAI API
+account and api key (see setup instructions below) #### ð Repository Most
+user's will run *README-AI* using the command-line, specifying their repository
+on run-time. However, if you would like to use the default configuration, you
+will need to update the [configuration file](./conf/conf.toml) with your
+repository's remote URL or a local path to your codebase. ```toml [git]
+repository = "Insert your repository URL or local path here!" ``` #### ð
+OpenAI API To use the *README-AI* app, you must create an OpenAI API account
+and generate an API key. The steps below outline this process: OpenAI API User
+Guide 1. Go to the [OpenAI website](https://platform.openai.com/). 2. Click the
+"Sign up for free" button. 3. Fill out the registration form with your
+information and agree to the terms of service. 4. Once logged in, click on the
+"API" tab. 5. Follow the instructions to create a new API key. 6. Copy the API
+key and keep it in a secure place.
 > **â ï¸ Note** > > - To maximize your experience with README-AI, it is
 recommended to set up a payment method on OpenAI's website. By doing so, you
 gain access to more powerful language models like gpt-3.5-turbo. Without a
 payment method, your usage will be restricted to the base gpt-3 models. This
 limitation might lead to less precise README files or potential errors during
 the generation process. > > - When using a payment method, make sure you have
 sufficient credits to run the README-AI application. Additionally, remember to
 regularly monitor your API usage and costs by visiting the [OpenAI API Usage
 Dashboard](https://platform.openai.com/account/usage). Please note that this
 API is not free and you will be charged for each request made, which can
 accumulate rapidly. > > - The generation of the README.md file should typically
 complete in under 1 minute. If it takes longer than a few minutes, please
-terminate the process. > --- ### ð¦ Installation 1. Clone the *readme-ai*
+terminate the process. > --- ### ð¦ Installation Use any of the following
+methods to install project dependencies. > *Pip ([PyPI Package](https://
+pypi.org/project/readmeai/))* ```sh pip install readmeai ``` > *Docker ([Docker
+Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-ai/general))*
+```sh docker pull zeroxeli/readme-ai:latest ``` If you prefer to install the
+project dependencies locally, follow the steps below. 1. Clone the *readme-ai*
 repository to your machine. ```sh git clone https://github.com/eli64s/readme-ai
-``` 2. Navigate to the *readme-ai* directory. ```sh cd readme-ai ``` 3. Use any
-of the following methods to install project dependencies. > *Pip ([PyPI
-Package](https://pypi.org/project/readmeai/))* ```sh pip install readmeai ``` >
-*Docker ([Docker Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-
-ai/general))* ```sh docker pull zeroxeli/readme-ai:latest ``` > *Bash* ```sh
+``` 2. Navigate to the *readme-ai* directory. ```sh cd readme-ai ``` 3. Install
+the project dependencies using one of the following methods. > *Bash* ```sh
 bash setup/setup.sh ``` > *Conda* ```sh conda create -n readmeai python=3.9 -
 y && \ conda activate readmeai && \ pip install -r requirements.txt ``` >
 *Poetry* ```sh poetry install ``` ### ð® Using *README-AI* Use the command-
 line to provide the OpenAI API key (if not already set) and specify an output
 path for your README file, along with the path to your local repository or
 remote code repository. You can also provide the output path in the
 [configuration file](./conf/conf.toml) Command-Line Arguments: - `-k` or `--
@@ -192,20 +200,19 @@
 ``` > *Poetry* ```sh poetry shell export OPENAI_API_KEY="YOUR_API_KEY" poetry
 run python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/
 readme-ai ``` ### ð§ª Running Tests Execute the following command to run the
 test suite. ```sh bash scripts/test.sh ```
                                                                     ð_Return
 --- ## ð  Future Development - [X] Add additional language support for
 populating the *installation*, *usage*, and *test* README sections. - [X]
-Upload the *readme-ai* CLI tool to PyPI under the module name [readmeai](https:
-//pypi.org/project/readmeai/). - [ ] Design and implement a variety of README
-template formats for different use-cases. - [ ] Add support for writing the
-README in any language (i.e. CN, ES, FR, JA, KO, RU). - [ ] Create UI with
-[Textual](https://github.com/Textualize/textual) or another framework to
-improve user experience. --- ## ð Changelog [Changelog](./CHANGELOG.md) --
-- ## ð¤ Contributing [Contributing Guidelines](./CONTRIBUTING.md) --- ## ð
-License [MIT](./LICENSE) --- ## ð Acknowledgments *Badges* - [Shields.io]
-(https://shields.io/) - [Aveek-Saha/GitHub-Profile-Badges](https://github.com/
-Aveek-Saha/GitHub-Profile-Badges) - [Ileriayo/Markdown-Badges](https://
-github.com/Ileriayo/markdown-badges)
+Publish the *readme-ai* CLI app to PyPI [readmeai](https://pypi.org/project/
+readmeai/). - [ ] Create user interface and serve the *readme-ai* app via
+streamlit. - [ ] Design and implement a variety of README template formats for
+different use-cases. - [ ] Add support for writing the README in any language
+(i.e. CN, ES, FR, JA, KO, RU). --- ## ð Changelog [Changelog](./
+CHANGELOG.md) --- ## ð¤ Contributing [Contributing Guidelines](./
+CONTRIBUTING.md) --- ## ð License [MIT](./LICENSE) --- ## ð
+Acknowledgments *Badges* - [Shields.io](https://shields.io/) - [Aveek-Saha/
+GitHub-Profile-Badges](https://github.com/Aveek-Saha/GitHub-Profile-Badges) -
+[Ileriayo/Markdown-Badges](https://github.com/Ileriayo/markdown-badges)
                                                                     ð_Return
 ---
```

