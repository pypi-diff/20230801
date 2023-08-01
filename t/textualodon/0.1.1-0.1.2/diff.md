# Comparing `tmp/textualodon-0.1.1.tar.gz` & `tmp/textualodon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textualodon-0.1.1.tar", last modified: Wed Jul 12 10:22:29 2023, max compression
+gzip compressed data, was "textualodon-0.1.2.tar", last modified: Tue Aug  1 20:46:45 2023, max compression
```

## Comparing `textualodon-0.1.1.tar` & `textualodon-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 10:22:29.640456 textualodon-0.1.1/
--rw-rw-rw-   0        0        0     1071 2023-07-12 10:10:04.000000 textualodon-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4049 2023-07-12 10:22:29.639791 textualodon-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2203 2023-07-12 08:54:30.000000 textualodon-0.1.1/README.md
--rw-rw-rw-   0        0        0     1387 2023-07-12 10:22:02.000000 textualodon-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 10:22:29.641496 textualodon-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-06-26 10:54:24.000000 textualodon-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 10:22:29.560423 textualodon-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 10:22:29.616634 textualodon-0.1.1/src/textualodon/
--rw-rw-rw-   0        0        0       63 2023-07-11 19:58:48.000000 textualodon-0.1.1/src/textualodon/__init__.py
--rw-rw-rw-   0        0        0     7450 2023-07-11 19:58:48.000000 textualodon-0.1.1/src/textualodon/api.py
--rw-rw-rw-   0        0        0      220 2023-06-26 05:14:44.000000 textualodon-0.1.1/src/textualodon/app_logo.py
--rw-rw-rw-   0        0        0     4393 2023-07-11 19:58:48.000000 textualodon-0.1.1/src/textualodon/constants.py
--rw-rw-rw-   0        0        0     2680 2023-07-11 19:58:48.000000 textualodon-0.1.1/src/textualodon/login_form.py
--rw-rw-rw-   0        0        0      237 2023-07-11 19:58:48.000000 textualodon-0.1.1/src/textualodon/main.py
--rw-rw-rw-   0        0        0     6562 2023-07-11 19:58:48.000000 textualodon-0.1.1/src/textualodon/new_post_form.py
--rw-rw-rw-   0        0        0     5114 2023-07-11 19:58:48.000000 textualodon-0.1.1/src/textualodon/post_details.py
--rw-rw-rw-   0        0        0    10588 2023-07-11 19:58:48.000000 textualodon-0.1.1/src/textualodon/posts.py
--rw-rw-rw-   0        0        0     2333 2023-07-11 19:58:48.000000 textualodon-0.1.1/src/textualodon/style.css
--rw-rw-rw-   0        0        0     2114 2023-07-11 19:58:48.000000 textualodon-0.1.1/src/textualodon/textualodon.py
--rw-rw-rw-   0        0        0     5948 2023-07-11 19:58:48.000000 textualodon-0.1.1/src/textualodon/timelines.py
-drwxrwxrwx   0        0        0        0 2023-07-12 10:22:29.636785 textualodon-0.1.1/src/textualodon.egg-info/
--rw-rw-rw-   0        0        0     4049 2023-07-12 10:22:29.000000 textualodon-0.1.1/src/textualodon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2023-07-12 10:22:29.000000 textualodon-0.1.1/src/textualodon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 10:22:29.000000 textualodon-0.1.1/src/textualodon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-12 10:22:29.000000 textualodon-0.1.1/src/textualodon.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      178 2023-07-12 10:22:29.000000 textualodon-0.1.1/src/textualodon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 10:22:29.000000 textualodon-0.1.1/src/textualodon.egg-info/top_level.txt
+drwxr-xr-x   0 dawid      (501) staff       (20)        0 2023-08-01 20:46:45.424280 textualodon-0.1.2/
+-rw-r--r--   0 dawid      (501) staff       (20)     1062 2023-07-17 18:44:45.000000 textualodon-0.1.2/LICENSE
+-rw-r--r--   0 dawid      (501) staff       (20)     3953 2023-08-01 20:46:45.424145 textualodon-0.1.2/PKG-INFO
+-rw-r--r--   0 dawid      (501) staff       (20)     2136 2023-07-17 18:44:45.000000 textualodon-0.1.2/README.md
+-rw-r--r--   0 dawid      (501) staff       (20)     1319 2023-08-01 20:44:17.000000 textualodon-0.1.2/pyproject.toml
+-rw-r--r--   0 dawid      (501) staff       (20)       38 2023-08-01 20:46:45.424315 textualodon-0.1.2/setup.cfg
+-rw-r--r--   0 dawid      (501) staff       (20)       38 2023-06-29 18:43:15.000000 textualodon-0.1.2/setup.py
+drwxr-xr-x   0 dawid      (501) staff       (20)        0 2023-08-01 20:46:45.420895 textualodon-0.1.2/src/
+drwxr-xr-x   0 dawid      (501) staff       (20)        0 2023-08-01 20:46:45.423166 textualodon-0.1.2/src/textualodon/
+-rw-r--r--   0 dawid      (501) staff       (20)       62 2023-07-08 19:01:59.000000 textualodon-0.1.2/src/textualodon/__init__.py
+-rw-r--r--   0 dawid      (501) staff       (20)     9353 2023-08-01 20:44:01.000000 textualodon-0.1.2/src/textualodon/api.py
+-rw-r--r--   0 dawid      (501) staff       (20)      241 2023-08-01 20:44:01.000000 textualodon-0.1.2/src/textualodon/app_logo.py
+-rw-r--r--   0 dawid      (501) staff       (20)     4313 2023-07-17 19:42:45.000000 textualodon-0.1.2/src/textualodon/constants.py
+-rw-r--r--   0 dawid      (501) staff       (20)     2644 2023-08-01 20:44:01.000000 textualodon-0.1.2/src/textualodon/login_form.py
+-rw-r--r--   0 dawid      (501) staff       (20)      224 2023-07-08 19:01:59.000000 textualodon-0.1.2/src/textualodon/main.py
+-rw-r--r--   0 dawid      (501) staff       (20)     7575 2023-08-01 20:44:01.000000 textualodon-0.1.2/src/textualodon/new_post_form.py
+-rw-r--r--   0 dawid      (501) staff       (20)     5095 2023-08-01 20:44:01.000000 textualodon-0.1.2/src/textualodon/post_details.py
+-rw-r--r--   0 dawid      (501) staff       (20)    11191 2023-07-17 20:40:47.000000 textualodon-0.1.2/src/textualodon/posts.py
+-rw-r--r--   0 dawid      (501) staff       (20)     1259 2023-08-01 20:44:01.000000 textualodon-0.1.2/src/textualodon/screens.py
+-rw-r--r--   0 dawid      (501) staff       (20)     2490 2023-08-01 20:44:01.000000 textualodon-0.1.2/src/textualodon/style.css
+-rw-r--r--   0 dawid      (501) staff       (20)     2467 2023-08-01 20:44:01.000000 textualodon-0.1.2/src/textualodon/textualodon.py
+-rw-r--r--   0 dawid      (501) staff       (20)     7240 2023-08-01 20:44:01.000000 textualodon-0.1.2/src/textualodon/timelines.py
+-rw-r--r--   0 dawid      (501) staff       (20)     3496 2023-08-01 20:44:01.000000 textualodon-0.1.2/src/textualodon/trendings.py
+drwxr-xr-x   0 dawid      (501) staff       (20)        0 2023-08-01 20:46:45.423956 textualodon-0.1.2/src/textualodon.egg-info/
+-rw-r--r--   0 dawid      (501) staff       (20)     3953 2023-08-01 20:46:45.000000 textualodon-0.1.2/src/textualodon.egg-info/PKG-INFO
+-rw-r--r--   0 dawid      (501) staff       (20)      671 2023-08-01 20:46:45.000000 textualodon-0.1.2/src/textualodon.egg-info/SOURCES.txt
+-rw-r--r--   0 dawid      (501) staff       (20)        1 2023-08-01 20:46:45.000000 textualodon-0.1.2/src/textualodon.egg-info/dependency_links.txt
+-rw-r--r--   0 dawid      (501) staff       (20)       54 2023-08-01 20:46:45.000000 textualodon-0.1.2/src/textualodon.egg-info/entry_points.txt
+-rw-r--r--   0 dawid      (501) staff       (20)      178 2023-08-01 20:46:45.000000 textualodon-0.1.2/src/textualodon.egg-info/requires.txt
+-rw-r--r--   0 dawid      (501) staff       (20)       12 2023-08-01 20:46:45.000000 textualodon-0.1.2/src/textualodon.egg-info/top_level.txt
```

### Comparing `textualodon-0.1.1/LICENSE` & `textualodon-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-MIT License
-
-Copyright (c) 2023 djvdq
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+MIT License
+
+Copyright (c) 2023 djvdq
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `textualodon-0.1.1/PKG-INFO` & `textualodon-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1
-Name: textualodon
-Version: 0.1.1
-Summary: Mastodon client for terminal. Created with an excellent Textual framework.
-Author: djvdq
-Maintainer: djvdq
-License: MIT License
-        
-        Copyright (c) 2023 djvdq
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: repository, https://codeberg.org/djvdq/Textualodon
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: Console
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# Textualodon
-Mastodon in your CLI! Created with an excellent [Textual](https://github.com/textualize/textual) framework.
-
-## WARNING
-This project is in a very early stage of development. It will be heavily refactored in the future.
-
-## Features
-- [x] Login using own development tokens
-- [x] Show home, local and global timeline
-- [x] Visual difference between post, boost and replies
-- [x] Favourite a post
-- [x] Boost a post
-- [x] Bookmark a post
-- [x] Write new post
-- [x] Add CW to post
-- [x] Set post language
-- [x] Choose post visibility
-- [x] Add poll to post
-- [x] Open post details to see post comments and ancestors
-
-## To do
-Too much to write right now. I want to implement as much of the Mastodon API as possible and feasible for a console app.
-
-## Installation
-### From pypi
-1. 
-```python
-pip install textualodon
-```
-2. Run the app
-```bash
-textualodon
-```
-### From source
-1. Clone this repo
-```bash
-git clone https://codeberg.org/djvdq/Textualodon
-```
-2. I recommend using a virtual environment
-```bash
-python -m venv venv
-source venv/bin/activate
-```
-3. Install dependencies
-```bash
-pip install -r requirements.txt
-```
-4. Run the application
-```bash
-textual run textualodon.py
-```
-### API keys and first setup
-At first run, you will need to provide your own development tokens. To do this, follow these steps:
-1. Navigate to your Mastodon account and go to "Preferences" → "Development".
-2. On that page click "New application" in the upper right corner.
-3. In "Application name" you can write whatever you like, this field can't be empty.
-4. Scroll the page down and click "Submit". Next, you will use your own tokens to login.
-
-Now, go back to your running Textualodon app.
-1. Enter your instance url (e.g. mastodon.social)
-2. Copy the "Client key" from Mastodon to the "Client ID" field in Textualodon app.
-3. Copy the "Client secret" from Mastodon to the "Client secret" field in Textualodon app.
-4. Click "Login", a new tab will open in your browser.
-5. Copy your authorization token and paste it into the "Grant token" field in Textualodon app.
-6. Click "Login" again.
-7. Reopen the app to see your home timeline.
+Metadata-Version: 2.1
+Name: textualodon
+Version: 0.1.2
+Summary: Mastodon client for terminal. Created with an excellent Textual framework.
+Author: djvdq
+Maintainer: djvdq
+License: MIT License
+        
+        Copyright (c) 2023 djvdq
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
+Project-URL: repository, https://codeberg.org/djvdq/Textualodon
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# Textualodon
+Mastodon in your CLI! Created with an excellent [Textual](https://github.com/textualize/textual) framework.
+
+## WARNING
+This project is in a very early stage of development. It will be heavily refactored in the future.
+
+## Features
+- [x] Login using own development tokens
+- [x] Show home, local and global timeline
+- [x] Visual difference between post, boost and replies
+- [x] Favourite a post
+- [x] Boost a post
+- [x] Bookmark a post
+- [x] Write new post
+- [x] Add CW to post
+- [x] Set post language
+- [x] Choose post visibility
+- [x] Add poll to post
+- [x] Open post details to see post comments and ancestors
+
+## To do
+Too much to write right now. I want to implement as much of the Mastodon API as possible and feasible for a console app.
+
+## Installation
+### From pypi
+1.
+```python
+pip install textualodon
+```
+2. Run the app
+```bash
+textualodon
+```
+### From source
+1. Clone this repo
+```bash
+git clone https://codeberg.org/djvdq/Textualodon
+```
+2. I recommend using a virtual environment
+```bash
+python -m venv venv
+source venv/bin/activate
+```
+3. Install dependencies
+```bash
+pip install -r requirements.txt
+```
+4. Run the application
+```bash
+textual run textualodon.py
+```
+### API keys and first setup
+At first run, you will need to provide your own development tokens. To do this, follow these steps:
+1. Navigate to your Mastodon account and go to "Preferences" → "Development".
+2. On that page click "New application" in the upper right corner.
+3. In "Application name" you can write whatever you like, this field can't be empty.
+4. Scroll the page down and click "Submit". Next, you will use your own tokens to login.
+
+Now, go back to your running Textualodon app.
+1. Enter your instance url (e.g. mastodon.social)
+2. Copy the "Client key" from Mastodon to the "Client ID" field in Textualodon app.
+3. Copy the "Client secret" from Mastodon to the "Client secret" field in Textualodon app.
+4. Click "Login", a new tab will open in your browser.
+5. Copy your authorization token and paste it into the "Grant token" field in Textualodon app.
+6. Click "Login" again.
+7. Reopen the app to see your home timeline.
```

### Comparing `textualodon-0.1.1/README.md` & `textualodon-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-# Textualodon
-Mastodon in your CLI! Created with an excellent [Textual](https://github.com/textualize/textual) framework.
-
-## WARNING
-This project is in a very early stage of development. It will be heavily refactored in the future.
-
-## Features
-- [x] Login using own development tokens
-- [x] Show home, local and global timeline
-- [x] Visual difference between post, boost and replies
-- [x] Favourite a post
-- [x] Boost a post
-- [x] Bookmark a post
-- [x] Write new post
-- [x] Add CW to post
-- [x] Set post language
-- [x] Choose post visibility
-- [x] Add poll to post
-- [x] Open post details to see post comments and ancestors
-
-## To do
-Too much to write right now. I want to implement as much of the Mastodon API as possible and feasible for a console app.
-
-## Installation
-### From pypi
-1. 
-```python
-pip install textualodon
-```
-2. Run the app
-```bash
-textualodon
-```
-### From source
-1. Clone this repo
-```bash
-git clone https://codeberg.org/djvdq/Textualodon
-```
-2. I recommend using a virtual environment
-```bash
-python -m venv venv
-source venv/bin/activate
-```
-3. Install dependencies
-```bash
-pip install -r requirements.txt
-```
-4. Run the application
-```bash
-textual run textualodon.py
-```
-### API keys and first setup
-At first run, you will need to provide your own development tokens. To do this, follow these steps:
-1. Navigate to your Mastodon account and go to "Preferences" → "Development".
-2. On that page click "New application" in the upper right corner.
-3. In "Application name" you can write whatever you like, this field can't be empty.
-4. Scroll the page down and click "Submit". Next, you will use your own tokens to login.
-
-Now, go back to your running Textualodon app.
-1. Enter your instance url (e.g. mastodon.social)
-2. Copy the "Client key" from Mastodon to the "Client ID" field in Textualodon app.
-3. Copy the "Client secret" from Mastodon to the "Client secret" field in Textualodon app.
-4. Click "Login", a new tab will open in your browser.
-5. Copy your authorization token and paste it into the "Grant token" field in Textualodon app.
-6. Click "Login" again.
-7. Reopen the app to see your home timeline.
+# Textualodon
+Mastodon in your CLI! Created with an excellent [Textual](https://github.com/textualize/textual) framework.
+
+## WARNING
+This project is in a very early stage of development. It will be heavily refactored in the future.
+
+## Features
+- [x] Login using own development tokens
+- [x] Show home, local and global timeline
+- [x] Visual difference between post, boost and replies
+- [x] Favourite a post
+- [x] Boost a post
+- [x] Bookmark a post
+- [x] Write new post
+- [x] Add CW to post
+- [x] Set post language
+- [x] Choose post visibility
+- [x] Add poll to post
+- [x] Open post details to see post comments and ancestors
+
+## To do
+Too much to write right now. I want to implement as much of the Mastodon API as possible and feasible for a console app.
+
+## Installation
+### From pypi
+1.
+```python
+pip install textualodon
+```
+2. Run the app
+```bash
+textualodon
+```
+### From source
+1. Clone this repo
+```bash
+git clone https://codeberg.org/djvdq/Textualodon
+```
+2. I recommend using a virtual environment
+```bash
+python -m venv venv
+source venv/bin/activate
+```
+3. Install dependencies
+```bash
+pip install -r requirements.txt
+```
+4. Run the application
+```bash
+textual run textualodon.py
+```
+### API keys and first setup
+At first run, you will need to provide your own development tokens. To do this, follow these steps:
+1. Navigate to your Mastodon account and go to "Preferences" → "Development".
+2. On that page click "New application" in the upper right corner.
+3. In "Application name" you can write whatever you like, this field can't be empty.
+4. Scroll the page down and click "Submit". Next, you will use your own tokens to login.
+
+Now, go back to your running Textualodon app.
+1. Enter your instance url (e.g. mastodon.social)
+2. Copy the "Client key" from Mastodon to the "Client ID" field in Textualodon app.
+3. Copy the "Client secret" from Mastodon to the "Client secret" field in Textualodon app.
+4. Click "Login", a new tab will open in your browser.
+5. Copy your authorization token and paste it into the "Grant token" field in Textualodon app.
+6. Click "Login" again.
+7. Reopen the app to see your home timeline.
```

### Comparing `textualodon-0.1.1/src/textualodon/api.py` & `textualodon-0.1.2/src/textualodon/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,193 +1,273 @@
-import json
-import webbrowser
-from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
-
-import requests
-
-
-class MastoAPI:
-    client_id = None
-    client_secret = None
-    grant_token = None
-    instance_url = None
-
-    def __init__(self):
-        self.access_token = None
-        self.api_keys = None
-        self.read_config()
-
-    def get_grant_token(self) -> None:
-        url = f"{self.instance_url}/oauth/authorize?client_id={self.client_id}&scope=read+write+follow&redirect_uri=urn:ietf:wg:oauth:2.0:oob&response_type=code"  # noqa: E501
-        webbrowser.open_new_tab(url)
-
-    def write_config(self) -> None:
-        with open(Path(__file__).parent / "api_keys.json", "w") as f:
-            self.api_keys["client_id"] = self.client_id
-            self.api_keys["client_secret"] = self.client_secret
-            self.api_keys["grant_token"] = self.grant_token
-            self.api_keys["instance_url"] = self.instance_url
-            self.api_keys["access_token"] = self.access_token
-            json.dump(self.api_keys, f)
-
-    def read_config(self) -> None:
-        try:
-            with open(Path(__file__).parent / "api_keys.json", "r") as f:
-                self.api_keys = json.load(f)
-        except FileNotFoundError:
-            self.api_keys = {}
-        self.client_id = self.api_keys.get("client_id")
-        self.client_secret = self.api_keys.get("client_secret")
-        self.grant_token = self.api_keys.get("grant_token")
-        self.instance_url = self.api_keys.get("instance_url")
-        if self.instance_url and not self.instance_url.startswith("https://"):
-            self.instance_url = f"https://{self.instance_url}"
-        self.access_token = self.api_keys.get("access_token")
-
-    def verify_keys(self) -> bool:
-        return self.api_keys and all(self.api_keys[elem] for elem in self.api_keys)
-
-    def get_home_timeline(
-        self, load_from: Optional[str] = None
-    ) -> List[Dict[str, str]]:
-        if load_from is not None:
-            payload = {
-                "max_id": load_from,
-            }
-        else:
-            payload = {}
-        resp = requests.get(
-            f"{self.instance_url}/api/v1/timelines/home",
-            headers={"Authorization": f"Bearer {self.access_token}"},
-            params=payload,
-        )
-        return resp.json()
-
-    def get_public_timeline(
-        self,
-        load_from: Optional[str] = None,
-        local: bool = True,
-    ) -> List[Dict[str, str]]:
-        if local:
-            url = f"{self.instance_url}/api/v1/timelines/public?local=true"
-        else:
-            url = f"{self.instance_url}/api/v1/timelines/public"
-        if load_from is not None:
-            payload = {
-                "max_id": load_from,
-            }
-        else:
-            payload = {}
-        resp = requests.get(
-            url,
-            headers={"Authorization": f"Bearer {self.access_token}"},
-            params=payload,
-        )
-        return resp.json()
-
-    def get_local_timeline(
-        self, load_from: Optional[str] = None
-    ) -> List[Dict[str, str]]:
-        return self.get_public_timeline()
-
-    def get_global_timeline(
-        self, load_from: Optional[str] = None
-    ) -> List[Dict[str, str]]:
-        return self.get_public_timeline(local=False)
-
-    def get_access_token(self) -> None:
-        url = f"{self.instance_url}/oauth/token"
-        data = {
-            "grant_type": "authorization_code",
-            "code": self.grant_token,
-            "redirect_uri": "urn:ietf:wg:oauth:2.0:oob",
-            "client_id": self.client_id,
-            "client_secret": self.client_secret,
-            "scope": "read write follow",
-        }
-        response = self.__call_url_post(url=url, data=data)
-        self.api_keys["access_token"] = response.get("access_token")
-        self.access_token = response.get("access_token")
-        self.write_config()
-
-    def __call_url_post(
-        self,
-        url: str,
-        headers: Optional[Dict[str, str]] = None,
-        data: Optional[Dict[str, Union[str, Any, None]]] = None,
-    ) -> Dict[str, Union[str, Any, None]]:
-        response = requests.post(
-            url=url, headers={"Authorization": f"Bearer {self.access_token}"}, data=data
-        )
-        return response.status_code, response.json()
-
-    def __call_url_get(self, url: str, headers: Optional[Dict[str, str]] = None):
-        response = requests.get(
-            url=url, headers={"Authorization": f"Bearer {self.access_token}"}
-        )
-        return response.status_code, response.json()
-
-    def favourite_post(self, post_id: str) -> Dict[str, Union[str, Any, None]]:
-        url = f"{self.instance_url}/api/v1/statuses/{post_id}/favourite"
-        return self.__call_url_post(url=url)
-
-    def boost_post(self, post_id: str) -> Dict[str, Union[str, Any, None]]:
-        url = f"{self.instance_url}/api/v1/statuses/{post_id}/reblog"
-        return self.__call_url_post(url=url)
-
-    def unfavourite_post(self, post_id: str) -> Dict[str, Union[str, Any, None]]:
-        url = f"{self.instance_url}/api/v1/statuses/{post_id}/unfavourite"
-        return self.__call_url_post(url=url)
-
-    def unboost_post(self, post_id: str) -> Dict[str, Union[str, Any, None]]:
-        url = f"{self.instance_url}/api/v1/statuses/{post_id}/unreblog"
-        return self.__call_url_post(url=url)
-
-    def bookmark_post(self, post_id: str) -> Dict[str, Union[str, Any, None]]:
-        url = f"{self.instance_url}/api/v1/statuses/{post_id}/bookmark"
-        return self.__call_url_post(url=url)
-
-    def unbookmark_post(self, post_id: str) -> Dict[str, Union[str, Any, None]]:
-        url = f"{self.instance_url}/api/v1/statuses/{post_id}/unbookmark"
-        return self.__call_url_post(url=url)
-
-    def get_account_by_id(self, account_id: str) -> Dict[str, str]:
-        url = f"{self.instance_url}/api/v1/accounts/{account_id}"
-        return self.__call_url_get(url=url)
-
-    def get_post_by_id(self, post_id: str) -> Dict[str, Union[str, Any, None]]:
-        url = f"{self.instance_url}/api/v1/statuses/{post_id}"
-        return self.__call_url_get(url=url)
-
-    def get_post_context(self, post_id: str) -> Dict[str, Union[str, Any, None]]:
-        url = f"{self.instance_url}/api/v1/statuses/{post_id}/context"
-        return self.__call_url_get(url=url)
-
-    def add_post(
-        self,
-        post_content: str,
-        visibility: str,
-        sensitive: bool = False,
-        content_warning: Optional[str] = None,
-        poll_options: Optional[List[str]] = None,
-        multiple_choice: bool = False,
-        hide_total: bool = False,
-        poll_expiration: int = 300,
-    ) -> Dict[str, Union[str, Any, None]]:
-        url = f"{self.instance_url}/api/v1/statuses"
-        data: Dict[str, Union[str, Any, None]] = {
-            "status": post_content,
-            "visibility": visibility,
-        }
-        if sensitive:
-            data["sensitive"] = sensitive
-            data["spoiler_text"] = content_warning
-        if poll_options:
-            data["poll[options][]"] = poll_options
-            data["poll[expires_in]"] = poll_expiration
-            data["poll[hide_totals]"] = hide_total
-        return self.__call_url_post(url=url, data=data)
-
-
-if __name__ == "__main__":
-    api = MastoAPI()
+import json
+import webbrowser
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Tuple, Union
+
+import requests
+
+
+class MastoAPI:
+    client_id = None
+    client_secret = None
+    grant_token = None
+    instance_url = None
+
+    def __init__(self):
+        self.access_token = None
+        self.api_keys = None
+        self.read_config()
+
+    def get_grant_token(self) -> None:
+        url = f"{self.instance_url}/oauth/authorize?client_id={self.client_id}&scope=read+write+follow&redirect_uri=urn:ietf:wg:oauth:2.0:oob&response_type=code"  # noqa: E501
+        webbrowser.open_new_tab(url)
+
+    def write_config(self) -> None:
+        with open(Path(__file__).parent / "api_keys.json", "w") as f:
+            self.api_keys["client_id"] = self.client_id
+            self.api_keys["client_secret"] = self.client_secret
+            self.api_keys["grant_token"] = self.grant_token
+            self.api_keys["instance_url"] = self.instance_url
+            self.api_keys["access_token"] = self.access_token
+            json.dump(self.api_keys, f)
+
+    def read_config(self) -> None:
+        try:
+            with open(Path(__file__).parent / "api_keys.json", "r") as f:
+                self.api_keys = json.load(f)
+        except FileNotFoundError:
+            self.api_keys = {}
+        self.client_id = self.api_keys.get("client_id")
+        self.client_secret = self.api_keys.get("client_secret")
+        self.grant_token = self.api_keys.get("grant_token")
+        self.instance_url = self.api_keys.get("instance_url")
+        if self.instance_url and not self.instance_url.startswith("https://"):
+            self.instance_url = f"https://{self.instance_url}"
+        self.access_token = self.api_keys.get("access_token")
+
+    def verify_keys(self) -> bool:
+        return self.api_keys and all(self.api_keys[elem] for elem in self.api_keys)
+
+    def get_home_timeline(
+        self, load_from: Optional[str] = None
+    ) -> List[Dict[str, str]]:
+        if load_from is not None:
+            payload = {
+                "max_id": load_from,
+            }
+        else:
+            payload = {}
+        resp = requests.get(
+            f"{self.instance_url}/api/v1/timelines/home",
+            headers={"Authorization": f"Bearer {self.access_token}"},
+            params=payload,
+        )
+        return resp.json()
+
+    def get_public_timeline(
+        self,
+        load_from: Optional[str] = None,
+        local: bool = True,
+    ) -> List[Dict[str, str]]:
+        if local:
+            url = f"{self.instance_url}/api/v1/timelines/public?local=true"
+        else:
+            url = f"{self.instance_url}/api/v1/timelines/public"
+        if load_from is not None:
+            payload = {
+                "max_id": load_from,
+            }
+        else:
+            payload = {}
+        resp = requests.get(
+            url,
+            headers={"Authorization": f"Bearer {self.access_token}"},
+            params=payload,
+        )
+        return resp.json()
+
+    def get_local_timeline(
+        self, load_from: Optional[str] = None
+    ) -> List[Dict[str, str]]:
+        return self.get_public_timeline()
+
+    def get_global_timeline(
+        self, load_from: Optional[str] = None
+    ) -> List[Dict[str, str]]:
+        return self.get_public_timeline(local=False)
+
+    def get_access_token(self) -> None:
+        url = f"{self.instance_url}/oauth/token"
+        data = {
+            "grant_type": "authorization_code",
+            "code": self.grant_token,
+            "redirect_uri": "urn:ietf:wg:oauth:2.0:oob",
+            "client_id": self.client_id,
+            "client_secret": self.client_secret,
+            "scope": "read write follow",
+        }
+        _, response = self.__call_url_post(url=url, data=data)
+        self.api_keys["access_token"] = response.get("access_token")
+        self.access_token = response.get("access_token")
+        self.write_config()
+
+    def __call_url_post(
+        self,
+        url: str,
+        headers: Optional[Dict[str, str]] = None,
+        data: Optional[Dict[str, Union[str, Any, None]]] = None,
+    ) -> Tuple[int, Dict[str, Union[str, Any, None]]]:
+        response = requests.post(
+            url=url, headers={"Authorization": f"Bearer {self.access_token}"}, data=data
+        )
+        return response.status_code, response.json()
+
+    def __call_url_get(self, url: str, headers: Optional[Dict[str, str]] = None):
+        response = requests.get(
+            url=url, headers={"Authorization": f"Bearer {self.access_token}"}
+        )
+        return response.status_code, response.json()
+
+    def favourite_post(
+        self, post_id: str
+    ) -> Tuple[int, Dict[str, Union[str, Any, None]]]:
+        url = f"{self.instance_url}/api/v1/statuses/{post_id}/favourite"
+        return self.__call_url_post(url=url)
+
+    def boost_post(self, post_id: str) -> Tuple[int, Dict[str, Union[str, Any, None]]]:
+        url = f"{self.instance_url}/api/v1/statuses/{post_id}/reblog"
+        return self.__call_url_post(url=url)
+
+    def unfavourite_post(
+        self, post_id: str
+    ) -> Tuple[int, Dict[str, Union[str, Any, None]]]:
+        url = f"{self.instance_url}/api/v1/statuses/{post_id}/unfavourite"
+        return self.__call_url_post(url=url)
+
+    def unboost_post(
+        self, post_id: str
+    ) -> Tuple[int, Dict[str, Union[str, Any, None]]]:
+        url = f"{self.instance_url}/api/v1/statuses/{post_id}/unreblog"
+        return self.__call_url_post(url=url)
+
+    def bookmark_post(
+        self, post_id: str
+    ) -> Tuple[int, Dict[str, Union[str, Any, None]]]:
+        url = f"{self.instance_url}/api/v1/statuses/{post_id}/bookmark"
+        return self.__call_url_post(url=url)
+
+    def unbookmark_post(
+        self, post_id: str
+    ) -> Tuple[int, Dict[str, Union[str, Any, None]]]:
+        url = f"{self.instance_url}/api/v1/statuses/{post_id}/unbookmark"
+        return self.__call_url_post(url=url)
+
+    def get_account_by_id(self, account_id: str) -> Dict[str, str]:
+        url = f"{self.instance_url}/api/v1/accounts/{account_id}"
+        return self.__call_url_get(url=url)
+
+    def get_post_by_id(
+        self, post_id: str
+    ) -> Tuple[int, Dict[str, Union[str, Any, None]]]:
+        url = f"{self.instance_url}/api/v1/statuses/{post_id}"
+        return self.__call_url_get(url=url)
+
+    def get_post_context(
+        self, post_id: str
+    ) -> Tuple[int, Dict[str, Union[str, Any, None]]]:
+        url = f"{self.instance_url}/api/v1/statuses/{post_id}/context"
+        return self.__call_url_get(url=url)
+
+    def add_post(
+        self,
+        post_content: str,
+        visibility: str,
+        sensitive: bool = False,
+        content_warning: Optional[str] = None,
+        poll_options: Optional[List[str]] = None,
+        multiple_choice: bool = False,
+        hide_total: bool = False,
+        poll_expiration: int = 300,
+        in_reply_to: Optional[str] = None,
+    ) -> Tuple[int, Dict[str, Union[str, Any, None]]]:
+        url = f"{self.instance_url}/api/v1/statuses"
+        data: Dict[str, Union[str, Any, None]] = {
+            "status": post_content,
+            "visibility": visibility,
+        }
+        if sensitive:
+            data["sensitive"] = sensitive
+            data["spoiler_text"] = content_warning
+        if poll_options:
+            data["poll[options][]"] = poll_options
+            data["poll[expires_in]"] = poll_expiration
+            data["poll[hide_totals]"] = hide_total
+        if in_reply_to is not None:
+            data["in_reply_to_id"] = in_reply_to
+        return self.__call_url_post(url=url, data=data)
+
+    def get_trending_posts(
+        self,
+        offset: Optional[int] = 0,
+    ) -> List[Dict[str, str]]:
+        url = f"{self.instance_url}/api/v1/trends/statuses"
+        payload = {
+            "offset": offset,
+        }
+        resp = requests.get(
+            url,
+            headers={"Authorization": f"Bearer {self.access_token}"},
+            params=payload,
+        )
+        return resp.json()
+
+    def get_posts_with_tag(
+        self,
+        tag_name: str,
+        load_from: Optional[int] = None,
+    ) -> List[Dict[str, str]]:
+        if load_from is not None:
+            payload = {
+                "max_id": load_from,
+            }
+        else:
+            payload = {}
+        resp = requests.get(
+            f"{self.instance_url}/api/v1/timelines/tag/{tag_name}",
+            headers={"Authorization": f"Bearer {self.access_token}"},
+            params=payload,
+        )
+        return resp.json()
+
+    def get_trending_tags(
+        self,
+        offset: Optional[int] = 0,
+    ) -> List[Dict[str, str]]:
+        url = f"{self.instance_url}/api/v1/trends/tags"
+        payload = {
+            "offset": offset,
+        }
+        resp = requests.get(
+            url,
+            headers={"Authorization": f"Bearer {self.access_token}"},
+            params=payload,
+        )
+        return resp.json()
+
+    def get_trending_links(
+        self,
+        offset: Optional[int] = 0,
+    ) -> List[Dict[str, str]]:
+        url = f"{self.instance_url}/api/v1/trends/links"
+        payload = {
+            "offset": offset,
+        }
+        resp = requests.get(
+            url,
+            headers={"Authorization": f"Bearer {self.access_token}"},
+            params=payload,
+        )
+        return resp.json()
+
+
+if __name__ == "__main__":
+    api = MastoAPI()
```

### Comparing `textualodon-0.1.1/src/textualodon/login_form.py` & `textualodon-0.1.2/src/textualodon/login_form.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,66 @@
-from textual import on  # type: ignore[attr-defined]
-from textual.app import ComposeResult
-from textual.containers import Center
-from textual.screen import Screen
-from textual.widgets import Header, Footer, Static, Label, Input, Button
-
-try:
-    from .api import MastoAPI
-    from .app_logo import AppLogo
-except ImportError:
-    from api import MastoAPI  # type: ignore[no-redef]
-    from app_logo import AppLogo  # type: ignore[no-redef]
-
-
-class LoginForm(Screen):
-    def __init__(self) -> None:
-        super().__init__()
-        self.masto_api = MastoAPI()
-
-    def compose(self) -> ComposeResult:
-        yield Header()
-        yield AppLogo()
-        yield Center(
-            Label("Instance URL", classes="login-form"),
-            Input(id="url", classes="login-form", value=self.masto_api.instance_url),
-            Label("Client ID", classes="login-form"),
-            Input(id="client_id", classes="login-form", value=self.masto_api.client_id),
-            Label("Client Secret", classes="login-form"),
-            Input(
-                id="client_secret",
-                password=True,
-                classes="login-form",
-                value=self.masto_api.client_secret,
-            ),
-            Button("Login", id="loginButton", classes="login-form"),
-            Label("Grant Token", classes="login-form grant_token"),
-            Input(id="grant_token", password=True, classes="login-form grant_token"),
-            Static(
-                "Login successful! Reopen the app to continue.",
-                classes="login-form login-success",
-                id="login-success",
-            ),
-            id="login-form",
-        )
-        yield Footer()
-
-    @on(Button.Pressed, "#loginButton")
-    def login_pressed(self) -> None:
-        instance_url = self.query_one("#url").value
-        if instance_url and not instance_url.startswith("https://"):
-            instance_url = "https://" + instance_url
-        self.masto_api.instance_url = instance_url
-        self.masto_api.client_id = self.query_one("#client_id").value
-        self.masto_api.client_secret = self.query_one("#client_secret").value
-        self.masto_api.grant_token = self.query_one("#grant_token").value
-        if not self.masto_api.grant_token:
-            self.masto_api.get_grant_token()
-            for elem in self.query(".grant_token"):
-                elem.display = "block"
-        if not self.masto_api.access_token:
-            self.masto_api.get_access_token()
-        self.masto_api.write_config()
-        if self.masto_api.verify_keys():
-            self.query_one("#login-success").display = "block"
+from textual import on  # type: ignore[attr-defined]
+from textual.app import ComposeResult
+from textual.containers import Center
+from textual.screen import Screen
+from textual.widgets import Header, Footer, Static, Label, Input, Button
+
+try:
+    from .api import MastoAPI
+    from .app_logo import AppLogo
+except ImportError:
+    from api import MastoAPI  # type: ignore[no-redef]
+    from app_logo import AppLogo  # type: ignore[no-redef]
+
+
+class LoginForm(Screen):
+    CSS_PATH = "style.css"
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.masto_api = MastoAPI()
+
+    def compose(self) -> ComposeResult:
+        yield Header()
+        yield AppLogo()
+        yield Center(
+            Label("Instance URL", classes="login-form"),
+            Input(id="url", classes="login-form", value=self.masto_api.instance_url),
+            Label("Client ID", classes="login-form"),
+            Input(id="client_id", classes="login-form", value=self.masto_api.client_id),
+            Label("Client Secret", classes="login-form"),
+            Input(
+                id="client_secret",
+                password=True,
+                classes="login-form",
+                value=self.masto_api.client_secret,
+            ),
+            Button("Login", id="loginButton", classes="login-form"),
+            Label("Grant Token", classes="login-form grant_token"),
+            Input(id="grant_token", password=True, classes="login-form grant_token"),
+            Static(
+                "Login successful! Reopen the app to continue.",
+                classes="login-form login-success",
+                id="login-success",
+            ),
+            id="login-form",
+        )
+        yield Footer()
+
+    @on(Button.Pressed, "#loginButton")
+    def login_pressed(self) -> None:
+        instance_url = self.query_one("#url").value
+        if instance_url and not instance_url.startswith("https://"):
+            instance_url = "https://" + instance_url
+        self.masto_api.instance_url = instance_url
+        self.masto_api.client_id = self.query_one("#client_id").value
+        self.masto_api.client_secret = self.query_one("#client_secret").value
+        self.masto_api.grant_token = self.query_one("#grant_token").value
+        if not self.masto_api.grant_token:
+            self.masto_api.get_grant_token()
+            for elem in self.query(".grant_token"):
+                elem.display = "block"
+        if not self.masto_api.access_token:
+            self.masto_api.get_access_token()
+        self.masto_api.write_config()
+        if self.masto_api.verify_keys():
+            self.query_one("#login-success").display = "block"
```

### Comparing `textualodon-0.1.1/src/textualodon/post_details.py` & `textualodon-0.1.2/src/textualodon/post_details.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-from typing import Any, Dict, List, Union
-
-from textual.app import ComposeResult
-from textual.containers import ScrollableContainer, Center
-from textual.widgets import Header, Footer
-from textual.screen import Screen
-
-try:
-    from .posts import Post
-    from .api import MastoAPI
-except ImportError:
-    from posts import Post  # type: ignore[no-redef]
-    from api import MastoAPI  # type: ignore[no-redef]
-
-
-class PostDetails(Screen):
-    BINDINGS = [
-        ("b", "go_back", "Go back"),
-    ]
-
-    def __init__(self, post_id) -> None:
-        super().__init__()
-        self.post_id = post_id
-        self.masto_api = MastoAPI()
-        _, self.post_context = self.masto_api.get_post_context(post_id=self.post_id)
-        _, self.post = self.masto_api.get_post_by_id(post_id=self.post_id)
-        post_widget = self.prepare_post_widgets(posts=[self.post], main_post=True)
-        self.post_ancestors = self.post_context["ancestors"]  # type: ignore[arg-type]
-        post_ancestors_widgets = self.prepare_post_widgets(self.post_ancestors)  # type: ignore[arg-type]
-        self.post_descendants = self.post_context["descendants"]  # type: ignore[arg-type]
-        post_descendants_widgets = self.prepare_post_widgets(self.post_descendants)  # type: ignore[arg-type]
-        self.posts_widgets = (
-            post_ancestors_widgets + post_widget + post_descendants_widgets
-        )
-
-    def compose(self) -> ComposeResult:
-        yield ScrollableContainer(
-            Header(),
-            Center(*self.posts_widgets, classes="posts"),
-            Footer(),
-        )
-
-    def action_go_back(self) -> None:
-        self.app.pop_screen()
-
-    def prepare_post_widgets(
-        self, posts: List[Dict[str, Union[str, Any, None]]], main_post: bool = False
-    ) -> ComposeResult:
-        posts_widgets = []
-        for post in posts:
-            reblogger = None
-            reblogger_handle = None
-            reply_post_url = None
-            reply_to_post_author = None
-            original_post_id = None
-            is_with_spoiler = post["sensitive"]
-            spoiler_text = post["spoiler_text"]
-            if post["reblog"] is not None:
-                author = post["reblog"]["account"]["username"]  # type: ignore[index]
-                author_url = post["reblog"]["account"]["url"]  # type: ignore[index]
-                author_handle = f"{author} ({author_url})"
-                reblogger = post["account"]["username"]  # type: ignore[index]
-                reblogger_url = post["account"]["url"]  # type: ignore[index]
-                reblogger_handle = f"{reblogger} ({reblogger_url})"
-                content = post["reblog"]["content"]  # type: ignore[index]
-                media_attachments = post["reblog"]["media_attachments"]  # type: ignore[arg-type, index]
-                original_post_id = post["reblog"]["id"]  # type: ignore[index]
-            else:
-                author = post["account"]["username"]  # type: ignore[index]
-                author_url = post["account"]["url"]  # type: ignore[index]
-                author_handle = f"{author} ({author_url})"
-                content = post["content"]
-                media_attachments = post["media_attachments"]
-            if (reply_to_id := post["in_reply_to_id"]) is not None and (
-                reply_to_account_id := post["in_reply_to_account_id"]
-            ) is not None:
-                _, reply_to_user = self.masto_api.get_account_by_id(reply_to_account_id)
-                _, reply_to_post = self.masto_api.get_post_by_id(reply_to_id)
-                reply_post_url = reply_to_post["url"]
-                reply_to_post_author = (
-                    f"{reply_to_user['acct']} ({reply_to_user['url']})"
-                )
-            posts_widgets.append(
-                Post(
-                    author=author_handle,
-                    content=content,
-                    favourites_count=post["favourites_count"],  # type:ignore[arg-type]
-                    reblogs_count=post["reblogs_count"],  # type:ignore[arg-type]
-                    replies_count=post["replies_count"],  # type:ignore[arg-type]
-                    url=post["url"],  # type:ignore[arg-type]
-                    reblogger=reblogger_handle,  # type:ignore[arg-type]
-                    post_id=post["id"],  # type:ignore[arg-type]
-                    original_post_id=original_post_id,
-                    favourited=post["favourited"],  # type:ignore[arg-type]
-                    boosted=post["reblogged"],  # type:ignore[arg-type]
-                    bookmarked=post["bookmarked"],  # type:ignore[arg-type]
-                    reply_to_url=reply_post_url,
-                    reply_to_author=reply_to_post_author,
-                    media_attachments=media_attachments,  # type:ignore[arg-type]
-                    is_with_spoiler=is_with_spoiler,  # type:ignore[arg-type]
-                    spoiler_text=spoiler_text,
-                    is_details_open=main_post,
-                )
-            )
-        return posts_widgets
+from typing import Any, Dict, List, Union
+
+from textual.app import ComposeResult
+from textual.containers import ScrollableContainer, Center
+from textual.widgets import Header, Footer
+from textual.screen import Screen
+
+try:
+    from .posts import Post
+    from .api import MastoAPI
+except ImportError:
+    from posts import Post  # type: ignore[no-redef]
+    from api import MastoAPI  # type: ignore[no-redef]
+
+
+class PostDetails(Screen):
+    BINDINGS = [
+        ("b", "go_back", "Go back"),
+    ]
+    CSS_PATH = "style.css"
+
+    def __init__(self, post_id) -> None:
+        super().__init__()
+        self.post_id = post_id
+        self.masto_api = MastoAPI()
+        _, self.post_context = self.masto_api.get_post_context(post_id=self.post_id)
+        _, self.post = self.masto_api.get_post_by_id(post_id=self.post_id)
+        post_widget = self.prepare_post_widgets(posts=[self.post], main_post=True)
+        self.post_ancestors = self.post_context["ancestors"]  # type: ignore[arg-type]
+        post_ancestors_widgets = self.prepare_post_widgets(self.post_ancestors)  # type: ignore[arg-type]
+        self.post_descendants = self.post_context["descendants"]  # type: ignore[arg-type]
+        post_descendants_widgets = self.prepare_post_widgets(self.post_descendants)  # type: ignore[arg-type]
+        self.posts_widgets = (
+            post_ancestors_widgets + post_widget + post_descendants_widgets
+        )
+
+    def compose(self) -> ComposeResult:
+        yield ScrollableContainer(
+            Header(),
+            Center(*self.posts_widgets, classes="posts"),
+            Footer(),
+        )
+
+    def action_go_back(self) -> None:
+        self.app.pop_screen()
+
+    def prepare_post_widgets(
+        self, posts: List[Dict[str, Union[str, Any, None]]], main_post: bool = False
+    ) -> ComposeResult:
+        posts_widgets = []
+        for post in posts:
+            reblogger = None
+            reblogger_handle = None
+            reply_post_url = None
+            reply_to_post_author = None
+            original_post_id = None
+            is_with_spoiler = post["sensitive"]
+            spoiler_text = post["spoiler_text"]
+            if post["reblog"] is not None:
+                author = post["reblog"]["account"]["username"]  # type: ignore[index]
+                author_url = post["reblog"]["account"]["url"]  # type: ignore[index]
+                author_handle = f"{author} ({author_url})"
+                reblogger = post["account"]["username"]  # type: ignore[index]
+                reblogger_url = post["account"]["url"]  # type: ignore[index]
+                reblogger_handle = f"{reblogger} ({reblogger_url})"
+                content = post["reblog"]["content"]  # type: ignore[index]
+                media_attachments = post["reblog"]["media_attachments"]  # type: ignore[arg-type, index]
+                original_post_id = post["reblog"]["id"]  # type: ignore[index]
+            else:
+                author = post["account"]["username"]  # type: ignore[index]
+                author_url = post["account"]["url"]  # type: ignore[index]
+                author_handle = f"{author} ({author_url})"
+                content = post["content"]
+                media_attachments = post["media_attachments"]
+            if (reply_to_id := post["in_reply_to_id"]) is not None and (
+                reply_to_account_id := post["in_reply_to_account_id"]
+            ) is not None:
+                _, reply_to_user = self.masto_api.get_account_by_id(reply_to_account_id)
+                _, reply_to_post = self.masto_api.get_post_by_id(reply_to_id)
+                reply_post_url = reply_to_post["url"]
+                reply_to_post_author = f"{reply_to_user['acct']} ({reply_to_user['url']})"  # type: ignore[index]
+            posts_widgets.append(
+                Post(
+                    author=author_handle,
+                    content=content,
+                    favourites_count=post["favourites_count"],  # type:ignore[arg-type]
+                    reblogs_count=post["reblogs_count"],  # type:ignore[arg-type]
+                    replies_count=post["replies_count"],  # type:ignore[arg-type]
+                    url=post["url"],  # type:ignore[arg-type]
+                    reblogger=reblogger_handle,  # type:ignore[arg-type]
+                    post_id=post["id"],  # type:ignore[arg-type]
+                    original_post_id=original_post_id,
+                    favourited=post["favourited"],  # type:ignore[arg-type]
+                    boosted=post["reblogged"],  # type:ignore[arg-type]
+                    bookmarked=post["bookmarked"],  # type:ignore[arg-type]
+                    visibility=post["visibility"],  # type:ignore[arg-type]
+                    reply_to_url=reply_post_url,
+                    reply_to_author=reply_to_post_author,
+                    media_attachments=media_attachments,  # type:ignore[arg-type]
+                    is_with_spoiler=is_with_spoiler,  # type:ignore[arg-type]
+                    spoiler_text=spoiler_text,
+                    is_details_open=main_post,
+                )
+            )
+        return posts_widgets
```

### Comparing `textualodon-0.1.1/src/textualodon/posts.py` & `textualodon-0.1.2/src/textualodon/posts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,272 +1,296 @@
-import re
-from typing import Any, Dict, List, Optional, Union
-
-from bs4 import BeautifulSoup
-from textual import on  # type: ignore[attr-defined]
-from textual.app import ComposeResult
-from textual.containers import Center, Horizontal
-from textual.widgets import Static, Button
-
-try:
-    from .api import MastoAPI
-except ImportError:
-    from api import MastoAPI  # type: ignore[no-redef]
-
-
-class Post(Static):
-    CSS_PATH = "style.css"
-
-    def __init__(
-        self,
-        author: str,
-        content: str,
-        favourites_count: int,
-        reblogs_count: int,
-        replies_count: int,
-        url: str,
-        reblogger: str,
-        post_id: str,
-        favourited: bool,
-        bookmarked: bool,
-        boosted: bool,
-        reply_to_url: Optional[str] = None,
-        reply_to_author: Optional[str] = None,
-        media_attachments: Optional[List[Dict[str, Union[str, Any, None]]]] = None,
-        is_with_spoiler: bool = False,
-        spoiler_text: Optional[str] = None,
-        original_post_id: Optional[str] = None,
-        is_details_open: bool = False,
-    ) -> None:
-        super().__init__()
-        self.author = author
-        self.content = self.__parse_content(content)
-        self.favourites_count = favourites_count
-        self.reblogs_count = reblogs_count
-        self.replies_count = replies_count
-        self.url = url
-        self.reblogger = reblogger
-        self.post_id = post_id
-        self.masto_api = MastoAPI()
-        self.favourited = favourited
-        self.bookmarked = bookmarked
-        self.boosted = boosted
-        self.reply_to_url = reply_to_url
-        self.reply_to_author = reply_to_author
-        self.media_attachments = media_attachments
-        if self.media_attachments is None:
-            self.media_attachments = []
-        self.is_with_spoiler = is_with_spoiler
-        self.spoiler_text = spoiler_text
-        self.original_post_id = original_post_id
-        self.is_details_open = is_details_open
-
-    @staticmethod
-    def __parse_content(html_text) -> List[str]:
-        soup = BeautifulSoup(html_text, "html.parser")
-
-        def __parse_tags(soup) -> BeautifulSoup:
-            a_tags = soup.find_all("a", {"class": "hashtag"})
-            for a_tag in a_tags:
-                href_content = a_tag.get("href", "")
-                hashtag = re.sub("https://.*/tags/", " #", href_content)
-                a_tag.replace_with(f" {hashtag}")
-            return soup
-
-        def __parse_links(soup) -> BeautifulSoup:
-            a_hrefs = soup.find_all("a")
-            for a_href in a_hrefs:
-                href_content = a_href.get("href", "")
-                a_href.replace_with(f"[u]{href_content}[/]")
-            return soup
-
-        def __parse_p(soup) -> List[str]:
-            p_tags = soup.find_all("p")
-            return [p_tag.get_text() for p_tag in p_tags]
-
-        soup = __parse_tags(soup)
-        soup = __parse_links(soup)
-        soup = __parse_p(soup)
-
-        return [str(s) for s in soup]
-
-    def compose(self) -> ComposeResult:
-        if len(self.content) > 1:
-            content = [Static(line, classes="post_content") for line in self.content]
-        else:
-            try:
-                content = [Static(self.content[0], classes="post_content")]
-            except IndexError:
-                content = []
-        if self.reblogger:
-            author = Horizontal(
-                Static(
-                    f"Reblogged by {self.reblogger}, Author: {self.author}",
-                    classes="author",
-                ),
-            )
-        elif self.reply_to_url and self.reply_to_author:
-            author = Center(
-                Static(
-                    f"Author: {self.author}, Replied to {self.reply_to_author}",
-                    classes="author",
-                ),
-                Static(f"Replied to url: {self.reply_to_url}", classes="author"),
-            )
-        else:
-            author = Static(f"Author: {self.author}", classes="author")
-        favourite_button_class = "favourited" if self.favourited else ""
-        boost_button_class = "boosted" if self.boosted else ""
-        bookmark_button_class = "bookmarked" if self.bookmarked else ""
-        if self.reblogger:
-            post_class = "reblog"
-        elif self.reply_to_url and self.reply_to_author:
-            post_class = "comment"
-        else:
-            post_class = "post"
-        spoiler = Center(
-            Static(f"CW: {self.spoiler_text}", classes="spoiler_text"),
-            Button("Show more", classes="spoiler_button", id="hide_spoiler"),
-            classes="spoiler",
-            id="spoiler",
-        )
-        if not self.is_with_spoiler:
-            spoiler.styles.display = "none"
-        comments_button = Button(
-            f"Comment {self.replies_count}", classes="button", id="reply"
-        )
-        if self.is_details_open:
-            comments_button.styles.display = "none"
-        media_attachments_widgets = []
-        for media in self.media_attachments:  # type: ignore[union-attr]
-            media_type: str = media["type"]  # type: ignore[assignment]
-            media_url: str = media["url"]  # type: ignore[assignment]
-            media_description: str = media["description"]  # type: ignore[assignment]
-            media_attachments_widgets.append(
-                Media(
-                    media_type=media_type,
-                    url=media_url,
-                    description=media_description,
-                )
-            )
-
-        yield Center(
-            spoiler,
-            author,
-            *content,
-            *media_attachments_widgets,
-            Horizontal(
-                Button(
-                    f"Like {self.favourites_count}",
-                    classes=f"button {favourite_button_class}",
-                    id="favourite",
-                ),
-                Button(
-                    f"Boost {self.reblogs_count}",
-                    classes=f"button {boost_button_class}",
-                    id="boost",
-                ),
-                comments_button,
-                Button(
-                    "Bookmark",
-                    classes=f"button {bookmark_button_class}",
-                    id="bookmark",
-                ),
-                classes="buttons",
-            ),
-            classes=post_class,
-        )
-
-    @on(Button.Pressed, "#favourite")
-    def favourite_post(self) -> None:
-        if not self.favourited:
-            _, response = self.masto_api.favourite_post(post_id=self.post_id)
-            if response["favourited"]:
-                self.favourited = True
-                self.query_one("#favourite").add_class("favourited")
-                self.favourites_count += 1
-                self.query_one("#favourite").update(f"Like {self.favourites_count}")
-                self.query_one("#favourite").refresh()
-        else:
-            _, response = self.masto_api.unfavourite_post(post_id=self.post_id)
-            if not response["favourited"]:
-                self.favourited = False
-                self.query_one("#favourite").remove_class("favourited")
-                self.favourites_count -= 1
-                self.query_one("#favourite").update(f"Like {self.favourites_count}")
-                self.query_one("#favourite").refresh()
-
-    @on(Button.Pressed, "#boost")
-    def boost_post(self) -> None:
-        if not self.boosted:
-            _, response = self.masto_api.boost_post(post_id=self.post_id)
-            if response.get("reblogged"):
-                self.boosted = True
-                self.query_one("#boost").add_class("boosted")
-                self.reblogs_count += 1
-                self.query_one("#boost").update(f"Boost {self.reblogs_count}")
-                self.query_one("#boost").refresh()
-        else:
-            _, response = self.masto_api.unboost_post(post_id=self.post_id)
-            if not response["reblogged"]:
-                self.boosted = False
-                self.query_one("#boost").remove_class("boosted")
-                self.reblogs_count -= 1
-                self.query_one("#boost").update(f"Boost {self.reblogs_count}")
-                self.query_one("#boost").refresh()
-
-    @on(Button.Pressed, "#bookmark")
-    def bookmark_post(self) -> None:
-        if self.reblogger:
-            post_id = self.original_post_id
-        else:
-            post_id = self.post_id
-        if not self.bookmarked:
-            _, response = self.masto_api.bookmark_post(post_id=post_id)  # type: ignore[arg-type]
-            print(response)
-            if response["bookmarked"]:
-                self.bookmarked = True
-                self.query_one("#bookmark").add_class("bookmarked")
-                self.query_one("#bookmark").refresh()
-        else:
-            _, response = self.masto_api.unbookmark_post(post_id=post_id)  # type: ignore[arg-type]
-            if not response["bookmarked"]:
-                self.bookmarked = False
-                self.query_one("#bookmark").remove_class("bookmarked")
-                self.query_one("#bookmark").refresh()
-
-    @on(Button.Pressed, "#hide_spoiler")
-    def hide_spoiler_alert(self) -> None:
-        self.query_one("#spoiler").remove()
-
-    @on(Button.Pressed, "#reply")
-    def go_to_post_details(self) -> None:
-        try:
-            from .post_details import PostDetails
-        except ImportError:
-            from post_details import PostDetails  # type: ignore[no-redef]
-        if self.original_post_id is not None:
-            post_id = self.original_post_id
-        else:
-            post_id = self.post_id
-        self.app.push_screen(PostDetails(post_id=post_id))
-
-
-class Media(Static):
-    def __init__(self, media_type: str, url: str, description: str) -> None:
-        super().__init__()
-        self.media_type = media_type
-        self.url = url
-        self.description = description
-
-    def compose(self) -> ComposeResult:
-        if self.description:
-            yield Center(
-                Static(f"{self.media_type.title()}: [u]{self.url}[/]", classes="media"),
-                Static(f"ALT: {self.description}", classes="media"),
-                classes="media_attachment",
-            )
-        else:
-            yield Center(
-                Static(f"{self.media_type.title()}: {self.url}", classes="media"),
-                classes="media_attachment",
-            )
+import re
+from typing import Any, Dict, List, Optional, Union
+
+from bs4 import BeautifulSoup
+from textual import on  # type: ignore[attr-defined]
+from textual.app import ComposeResult
+from textual.containers import Center, Horizontal
+from textual.widgets import Static, Button
+
+try:
+    from .api import MastoAPI
+    from .constants import visibility_emojis
+except ImportError:
+    from api import MastoAPI  # type: ignore[no-redef]
+    from constants import visibility_emojis  # type: ignore[no-redef]
+
+
+class Post(Static):
+    CSS_PATH = "style.css"
+
+    def __init__(
+        self,
+        author: str,
+        content: str,
+        favourites_count: int,
+        reblogs_count: int,
+        replies_count: int,
+        url: str,
+        reblogger: str,
+        post_id: str,
+        favourited: bool,
+        bookmarked: bool,
+        boosted: bool,
+        visibility: str,
+        reply_to_url: Optional[str] = None,
+        reply_to_author: Optional[str] = None,
+        media_attachments: Optional[List[Dict[str, Union[str, Any, None]]]] = None,
+        is_with_spoiler: bool = False,
+        spoiler_text: Optional[str] = None,
+        original_post_id: Optional[str] = None,
+        is_details_open: bool = False,
+    ) -> None:
+        super().__init__()
+        self.author = author
+        self.content = self.__parse_content(content)
+        self.favourites_count = favourites_count
+        self.reblogs_count = reblogs_count
+        self.replies_count = replies_count
+        self.url = url
+        self.reblogger = reblogger
+        self.post_id = post_id
+        self.masto_api = MastoAPI()
+        self.favourited = favourited
+        self.bookmarked = bookmarked
+        self.visibility = visibility
+        self.boosted = boosted
+        self.reply_to_url = reply_to_url
+        self.reply_to_author = reply_to_author
+        self.media_attachments = media_attachments
+        if self.media_attachments is None:
+            self.media_attachments = []
+        self.is_with_spoiler = is_with_spoiler
+        self.spoiler_text = spoiler_text
+        self.original_post_id = original_post_id
+        self.is_details_open = is_details_open
+
+    @staticmethod
+    def __parse_content(html_text) -> List[str]:
+        soup = BeautifulSoup(html_text, "html.parser")
+
+        def __parse_tags(soup) -> BeautifulSoup:
+            a_tags = soup.find_all("a", {"class": "hashtag"})
+            for a_tag in a_tags:
+                href_content = a_tag.get("href", "")
+                hashtag = re.sub("https://.*/tags/", " #", href_content)
+                a_tag.replace_with(f" {hashtag}")
+            return soup
+
+        def __parse_links(soup) -> BeautifulSoup:
+            a_hrefs = soup.find_all("a")
+            for a_href in a_hrefs:
+                href_content = a_href.get("href", "")
+                a_href.replace_with(f"[u]{href_content}[/]")
+            return soup
+
+        def __parse_p(soup) -> List[str]:
+            p_tags = soup.find_all("p")
+            return [p_tag.get_text() for p_tag in p_tags]
+
+        soup = __parse_tags(soup)
+        soup = __parse_links(soup)
+        soup = __parse_p(soup)
+
+        return [str(s) for s in soup]
+
+    def compose(self) -> ComposeResult:
+        if len(self.content) > 1:
+            content = [Static(line, classes="post_content") for line in self.content]
+        else:
+            try:
+                content = [Static(self.content[0], classes="post_content")]
+            except IndexError:
+                content = []
+        if self.reblogger:
+            author = Horizontal(
+                Static(
+                    f"Reblogged by {self.reblogger}, Author: {self.author}",
+                    classes="author",
+                ),
+            )
+        elif self.reply_to_url and self.reply_to_author:
+            author = Center(
+                Static(
+                    f"Author: {self.author}, Replied to {self.reply_to_author}",
+                    classes="author",
+                ),
+                Static(f"Replied to url: {self.reply_to_url}", classes="author"),
+            )
+        else:
+            author = Static(f"Author: {self.author}", classes="author")
+        favourite_button_class = "favourited" if self.favourited else ""
+        boost_button_class = "boosted" if self.boosted else ""
+        bookmark_button_class = "bookmarked" if self.bookmarked else ""
+        if self.reblogger:
+            post_class = "reblog"
+        elif self.reply_to_url and self.reply_to_author:
+            post_class = "comment"
+        else:
+            post_class = "post"
+        spoiler = Center(
+            Static(f"CW: {self.spoiler_text}", classes="spoiler_text"),
+            Button("Show more", classes="spoiler_button", id="hide_spoiler"),
+            classes="spoiler",
+            id="spoiler",
+        )
+        if not self.is_with_spoiler:
+            spoiler.styles.display = "none"
+        comments_button = Button(
+            f"Comments {self.replies_count}", classes="button", id="details"
+        )
+        if self.is_details_open:
+            comments_button.styles.display = "none"
+        media_attachments_widgets = []
+        for media in self.media_attachments:  # type: ignore[union-attr]
+            media_type: str = media["type"]  # type: ignore[assignment]
+            media_url: str = media["url"]  # type: ignore[assignment]
+            media_description: str = media["description"]  # type: ignore[assignment]
+            media_attachments_widgets.append(
+                Media(
+                    media_type=media_type,
+                    url=media_url,
+                    description=media_description,
+                )
+            )
+
+        yield Center(
+            spoiler,
+            Static(visibility_emojis[self.visibility], classes="visibility"),
+            author,
+            *content,
+            *media_attachments_widgets,
+            Horizontal(
+                Button(
+                    f"Like {self.favourites_count}",
+                    classes=f"button {favourite_button_class}",
+                    id="favourite",
+                ),
+                Button(
+                    f"Boost {self.reblogs_count}",
+                    classes=f"button {boost_button_class}",
+                    id="boost",
+                ),
+                comments_button,
+                Button("Reply", classes="button", id="reply"),
+                Button(
+                    "Bookmark",
+                    classes=f"button {bookmark_button_class}",
+                    id="bookmark",
+                ),
+                classes="buttons",
+            ),
+            classes=post_class,
+        )
+
+    @on(Button.Pressed, "#favourite")
+    def favourite_post(self) -> None:
+        if not self.favourited:
+            _, response = self.masto_api.favourite_post(post_id=self.post_id)
+            if response["favourited"]:
+                self.favourited = True
+                self.query_one("#favourite").add_class("favourited")
+                self.favourites_count += 1
+                self.query_one("#favourite").update(f"Like {self.favourites_count}")
+                self.query_one("#favourite").refresh()
+        else:
+            _, response = self.masto_api.unfavourite_post(post_id=self.post_id)
+            if not response["favourited"]:
+                self.favourited = False
+                self.query_one("#favourite").remove_class("favourited")
+                self.favourites_count -= 1
+                self.query_one("#favourite").update(f"Like {self.favourites_count}")
+                self.query_one("#favourite").refresh()
+
+    @on(Button.Pressed, "#boost")
+    def boost_post(self) -> None:
+        if not self.boosted:
+            _, response = self.masto_api.boost_post(post_id=self.post_id)
+            if response.get("reblogged"):
+                self.boosted = True
+                self.query_one("#boost").add_class("boosted")
+                self.reblogs_count += 1
+                self.query_one("#boost").update(f"Boost {self.reblogs_count}")
+                self.query_one("#boost").refresh()
+        else:
+            _, response = self.masto_api.unboost_post(post_id=self.post_id)
+            if not response["reblogged"]:
+                self.boosted = False
+                self.query_one("#boost").remove_class("boosted")
+                self.reblogs_count -= 1
+                self.query_one("#boost").update(f"Boost {self.reblogs_count}")
+                self.query_one("#boost").refresh()
+
+    @on(Button.Pressed, "#bookmark")
+    def bookmark_post(self) -> None:
+        if self.reblogger:
+            post_id = self.original_post_id
+        else:
+            post_id = self.post_id
+        if not self.bookmarked:
+            _, response = self.masto_api.bookmark_post(post_id=post_id)  # type: ignore[arg-type]
+            print(response)
+            if response["bookmarked"]:
+                self.bookmarked = True
+                self.query_one("#bookmark").add_class("bookmarked")
+                self.query_one("#bookmark").refresh()
+        else:
+            _, response = self.masto_api.unbookmark_post(post_id=post_id)  # type: ignore[arg-type]
+            if not response["bookmarked"]:
+                self.bookmarked = False
+                self.query_one("#bookmark").remove_class("bookmarked")
+                self.query_one("#bookmark").refresh()
+
+    @on(Button.Pressed, "#hide_spoiler")
+    def hide_spoiler_alert(self) -> None:
+        self.query_one("#spoiler").remove()
+
+    @on(Button.Pressed, "#details")
+    def go_to_post_details(self) -> None:
+        try:
+            from .post_details import PostDetails
+        except ImportError:
+            from post_details import PostDetails  # type: ignore[no-redef]
+        if self.original_post_id is not None:
+            post_id = self.original_post_id
+        else:
+            post_id = self.post_id
+        self.app.push_screen(PostDetails(post_id=post_id))
+
+    @on(Button.Pressed, "#reply")
+    def reply_to_post(self):
+        try:
+            from .new_post_form import NewPostForm
+        except ImportError:
+            from new_post_form import NewPostForm
+        if self.original_post_id is not None:
+            post_id = self.original_post_id
+        else:
+            post_id = self.post_id
+        self.app.push_screen(
+            NewPostForm(
+                in_reply_to=post_id,
+                reply_to_content=self.content,
+                visibility=self.visibility,
+            )
+        )
+
+
+class Media(Static):
+    def __init__(self, media_type: str, url: str, description: str) -> None:
+        super().__init__()
+        self.media_type = media_type
+        self.url = url
+        self.description = description
+
+    def compose(self) -> ComposeResult:
+        if self.description:
+            yield Center(
+                Static(f"{self.media_type.title()}: [u]{self.url}[/]", classes="media"),
+                Static(f"ALT: {self.description}", classes="media"),
+                classes="media_attachment",
+            )
+        else:
+            yield Center(
+                Static(f"{self.media_type.title()}: {self.url}", classes="media"),
+                classes="media_attachment",
+            )
```

### Comparing `textualodon-0.1.1/src/textualodon.egg-info/PKG-INFO` & `textualodon-0.1.2/src/textualodon.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1
-Name: textualodon
-Version: 0.1.1
-Summary: Mastodon client for terminal. Created with an excellent Textual framework.
-Author: djvdq
-Maintainer: djvdq
-License: MIT License
-        
-        Copyright (c) 2023 djvdq
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: repository, https://codeberg.org/djvdq/Textualodon
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: Console
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# Textualodon
-Mastodon in your CLI! Created with an excellent [Textual](https://github.com/textualize/textual) framework.
-
-## WARNING
-This project is in a very early stage of development. It will be heavily refactored in the future.
-
-## Features
-- [x] Login using own development tokens
-- [x] Show home, local and global timeline
-- [x] Visual difference between post, boost and replies
-- [x] Favourite a post
-- [x] Boost a post
-- [x] Bookmark a post
-- [x] Write new post
-- [x] Add CW to post
-- [x] Set post language
-- [x] Choose post visibility
-- [x] Add poll to post
-- [x] Open post details to see post comments and ancestors
-
-## To do
-Too much to write right now. I want to implement as much of the Mastodon API as possible and feasible for a console app.
-
-## Installation
-### From pypi
-1. 
-```python
-pip install textualodon
-```
-2. Run the app
-```bash
-textualodon
-```
-### From source
-1. Clone this repo
-```bash
-git clone https://codeberg.org/djvdq/Textualodon
-```
-2. I recommend using a virtual environment
-```bash
-python -m venv venv
-source venv/bin/activate
-```
-3. Install dependencies
-```bash
-pip install -r requirements.txt
-```
-4. Run the application
-```bash
-textual run textualodon.py
-```
-### API keys and first setup
-At first run, you will need to provide your own development tokens. To do this, follow these steps:
-1. Navigate to your Mastodon account and go to "Preferences" → "Development".
-2. On that page click "New application" in the upper right corner.
-3. In "Application name" you can write whatever you like, this field can't be empty.
-4. Scroll the page down and click "Submit". Next, you will use your own tokens to login.
-
-Now, go back to your running Textualodon app.
-1. Enter your instance url (e.g. mastodon.social)
-2. Copy the "Client key" from Mastodon to the "Client ID" field in Textualodon app.
-3. Copy the "Client secret" from Mastodon to the "Client secret" field in Textualodon app.
-4. Click "Login", a new tab will open in your browser.
-5. Copy your authorization token and paste it into the "Grant token" field in Textualodon app.
-6. Click "Login" again.
-7. Reopen the app to see your home timeline.
+Metadata-Version: 2.1
+Name: textualodon
+Version: 0.1.2
+Summary: Mastodon client for terminal. Created with an excellent Textual framework.
+Author: djvdq
+Maintainer: djvdq
+License: MIT License
+        
+        Copyright (c) 2023 djvdq
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
+Project-URL: repository, https://codeberg.org/djvdq/Textualodon
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# Textualodon
+Mastodon in your CLI! Created with an excellent [Textual](https://github.com/textualize/textual) framework.
+
+## WARNING
+This project is in a very early stage of development. It will be heavily refactored in the future.
+
+## Features
+- [x] Login using own development tokens
+- [x] Show home, local and global timeline
+- [x] Visual difference between post, boost and replies
+- [x] Favourite a post
+- [x] Boost a post
+- [x] Bookmark a post
+- [x] Write new post
+- [x] Add CW to post
+- [x] Set post language
+- [x] Choose post visibility
+- [x] Add poll to post
+- [x] Open post details to see post comments and ancestors
+
+## To do
+Too much to write right now. I want to implement as much of the Mastodon API as possible and feasible for a console app.
+
+## Installation
+### From pypi
+1.
+```python
+pip install textualodon
+```
+2. Run the app
+```bash
+textualodon
+```
+### From source
+1. Clone this repo
+```bash
+git clone https://codeberg.org/djvdq/Textualodon
+```
+2. I recommend using a virtual environment
+```bash
+python -m venv venv
+source venv/bin/activate
+```
+3. Install dependencies
+```bash
+pip install -r requirements.txt
+```
+4. Run the application
+```bash
+textual run textualodon.py
+```
+### API keys and first setup
+At first run, you will need to provide your own development tokens. To do this, follow these steps:
+1. Navigate to your Mastodon account and go to "Preferences" → "Development".
+2. On that page click "New application" in the upper right corner.
+3. In "Application name" you can write whatever you like, this field can't be empty.
+4. Scroll the page down and click "Submit". Next, you will use your own tokens to login.
+
+Now, go back to your running Textualodon app.
+1. Enter your instance url (e.g. mastodon.social)
+2. Copy the "Client key" from Mastodon to the "Client ID" field in Textualodon app.
+3. Copy the "Client secret" from Mastodon to the "Client secret" field in Textualodon app.
+4. Click "Login", a new tab will open in your browser.
+5. Copy your authorization token and paste it into the "Grant token" field in Textualodon app.
+6. Click "Login" again.
+7. Reopen the app to see your home timeline.
```

### Comparing `textualodon-0.1.1/src/textualodon.egg-info/SOURCES.txt` & `textualodon-0.1.2/src/textualodon.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 src/textualodon/app_logo.py
 src/textualodon/constants.py
 src/textualodon/login_form.py
 src/textualodon/main.py
 src/textualodon/new_post_form.py
 src/textualodon/post_details.py
 src/textualodon/posts.py
+src/textualodon/screens.py
 src/textualodon/style.css
 src/textualodon/textualodon.py
 src/textualodon/timelines.py
+src/textualodon/trendings.py
 src/textualodon.egg-info/PKG-INFO
 src/textualodon.egg-info/SOURCES.txt
 src/textualodon.egg-info/dependency_links.txt
 src/textualodon.egg-info/entry_points.txt
 src/textualodon.egg-info/requires.txt
 src/textualodon.egg-info/top_level.txt
```

