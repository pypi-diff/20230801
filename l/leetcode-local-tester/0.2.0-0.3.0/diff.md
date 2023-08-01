# Comparing `tmp/leetcode_local_tester-0.2.0.tar.gz` & `tmp/leetcode_local_tester-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetcode_local_tester-0.2.0.tar", max compression
+gzip compressed data, was "leetcode_local_tester-0.3.0.tar", max compression
```

## Comparing `leetcode_local_tester-0.2.0.tar` & `leetcode_local_tester-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1083 2023-07-25 13:49:39.940657 leetcode_local_tester-0.2.0/LICENSE
--rw-r--r--   0        0        0     5616 2023-07-25 14:43:00.155804 leetcode_local_tester-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-25 03:26:33.385642 leetcode_local_tester-0.2.0/leetcode_local_tester/__init__.py
--rw-r--r--   0        0        0      772 2023-07-25 08:19:15.221482 leetcode_local_tester-0.2.0/leetcode_local_tester/api.py
--rw-r--r--   0        0        0     2530 2023-07-25 14:27:07.956733 leetcode_local_tester-0.2.0/leetcode_local_tester/main.py
--rw-r--r--   0        0        0      489 2023-07-25 14:45:28.705029 leetcode_local_tester-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6563 1970-01-01 00:00:00.000000 leetcode_local_tester-0.2.0/setup.py
--rw-r--r--   0        0        0     6293 1970-01-01 00:00:00.000000 leetcode_local_tester-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-25 13:49:39.940657 leetcode_local_tester-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5734 2023-08-01 12:35:13.508175 leetcode_local_tester-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-25 03:26:33.385642 leetcode_local_tester-0.3.0/leetcode_local_tester/__init__.py
+-rw-r--r--   0        0        0      772 2023-07-25 08:19:15.221482 leetcode_local_tester-0.3.0/leetcode_local_tester/api.py
+-rw-r--r--   0        0        0     2562 2023-08-01 12:32:33.669602 leetcode_local_tester-0.3.0/leetcode_local_tester/main.py
+-rw-r--r--   0        0        0      489 2023-08-01 12:35:13.514683 leetcode_local_tester-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6683 1970-01-01 00:00:00.000000 leetcode_local_tester-0.3.0/setup.py
+-rw-r--r--   0        0        0     6411 1970-01-01 00:00:00.000000 leetcode_local_tester-0.3.0/PKG-INFO
```

### Comparing `leetcode_local_tester-0.2.0/LICENSE` & `leetcode_local_tester-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `leetcode_local_tester-0.2.0/README.md` & `leetcode_local_tester-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
   --detail TEXT    The detail of the question. If type is `contest` or
                    `problem`, the detail is the url. Such as
                    `https://leetcode.com/contest/weekly-contest-326/`,
                    `https://leetcode.con/problems/minimum-number-of-
                    operations-to-reinitialize-a-permutation/`. If type is
                    `season`, the detail is the season name. Such as
                    `2020-fall-solo` or `2020-fall-team`.
-  --language TEXT  The language of the code. Now support: `cpp`. Default is
-                   `cpp`.
+  --language TEXT  The language of the code. Now support: `cpp`, `python3`. Default is
+                   `python3`.
   --location TEXT  The location of the code. Default is `./leetcode/`.
   --help           Show this message and exit.
 ```
 
 ## Example
 ```bash
 leetcode-local-tester work --kind contest --detail https://leetcode.com/contest/weekly-contest-326/ --language cpp --location ./leetcode/
@@ -123,19 +123,21 @@
 
 ```text
 "the quick brown fox jumps over the lazy dog"
 "vkbs bs t suepuv"
 ```
 
 # TODO
-- [ ] Support `python`
+- [x] Support `python` (completed)
 
 # License
 This software is licensed under the MIT License. See the LICENSE file in the top distribution directory for the full license text.
 
 Maintaining the project is hard and time-consuming, and I've put much ❤️ and effort into this.
 
 If you've appreciated my work, you can back me up with a donation! Thank you 😊
 
+If there is any problem, please create an issue. I will reply to you as soon as possible.
+
 
 [<img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" width="217px" height="51x">](https://www.buymeacoffee.com/goodstudyqaq)
```

### Comparing `leetcode_local_tester-0.2.0/leetcode_local_tester/api.py` & `leetcode_local_tester-0.3.0/leetcode_local_tester/api.py`

 * *Files identical despite different names*

### Comparing `leetcode_local_tester-0.2.0/leetcode_local_tester/main.py` & `leetcode_local_tester-0.3.0/leetcode_local_tester/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
               help="The question kind. Now support: `contest`, `problem`, `season`, and `contest` includes `weekly` "
                    "and `biweekly`. Default is `problem`.")
 @click.option("--detail",
               help="The detail of the question. If type is `contest` or `problem`, the detail is the url. Such as "
                    "`https://leetcode.com/contest/weekly-contest-326/`, "
                    "`https://leetcode.con/problems/minimum-number-of-operations-to-reinitialize-a-permutation/`. "
                    "If type is `season`, the detail is the season name. Such as `2020-fall-solo` or `2020-fall-team`.")
-@click.option("--language", default="cpp",
-              help="The language of the code. Now support: `cpp`. Default is `cpp`.")
+@click.option("--language", default="python3",
+              help="The language of the code. Now support: `cpp`, `python3`. Default is `python3`.")
 @click.option("--location", default="./leetcode/",
               help="The location of the code. Default is `./leetcode/`.")
 def work(kind, detail, language, location):
     done = False
 
     def load():
         if not os.path.exists(location):
@@ -59,14 +59,15 @@
         for i in range(1000):
             if done:
                 time.sleep(0.001)
                 bar()
                 continue
             time.sleep(0.01)
             bar()
+    t.join()
     print(f"Generate local file for {detail} done!")
 
 
 @click.group()
 def cli():
     pass
```

### Comparing `leetcode_local_tester-0.2.0/setup.py` & `leetcode_local_tester-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['alive-progress>=3.1.4,<4.0.0', 'click==8.1.4', 'requests>=2.31.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['leetcode-local-tester = leetcode_local_tester.main:cli']}
 
 setup_kwargs = {
     'name': 'leetcode-local-tester',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': '',
-    'long_description': '# Leetcode-local-tester\n[![Maintenance](https://img.shields.io/badge/maintained-yes-brightgreen.svg)](https://github.com/goodstudyqaq/leetcode-local-tester/graphs/commit-activity)\n[![PyPI version](https://img.shields.io/pypi/v/leetcode-local-tester.svg)](https://pypi.python.org/pypi/leetcode-local-tester/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/leetcode-local-tester.svg)](https://pypi.python.org/pypi/leetcode-local-tester/)\n[![Downloads](https://static.pepy.tech/personalized-badge/leetcode-local-tester?period=month&units=international_system&left_color=grey&right_color=orange&left_text=downloads/month)](https://pepy.tech/project/leetcode-local-tester)\n[![Downloads](https://static.pepy.tech/personalized-badge/leetcode-local-tester?period=total&units=international_system&left_color=grey&right_color=orange&left_text=downloads)](https://pepy.tech/project/leetcode-local-tester)\n![GitHub Sponsors](https://img.shields.io/github/sponsors/goodstudyqaq)\n\n\nLeetcode test utils for local environment\n\n# Background\nBecause of Leetcode\'s special design for test cases, if you want to test your code locally, you need to write some boilerplate code to read the test cases from the file and parse them into the format that your code can understand, which is very annoying. Especially in a contest, you may not have enough time to write the boilerplate code. So I wrote this tool to help me generate the boilerplate code automatically. It will improve your efficiency in a contest.\n\nThe design is really like TopCoder\'s test cases, but TopCoder has a very good tool ([TZTester](https://community.topcoder.com/contest/classes/TZTester/TZTester.html)) to generate the boilerplate code for you, which is very convenient.\n\n# Usage\n\n## Install\n```bash\npip install leetcode-local-tester\n```\n\n## Command\n```bash\nleetcode-local-tester work --help\n\nOptions:\n  --kind TEXT      The question kind. Now support: `contest`, `problem`,\n                   `season`, and `contest` includes `weekly` and `biweekly`.\n                   Default is `problem`.\n  --detail TEXT    The detail of the question. If type is `contest` or\n                   `problem`, the detail is the url. Such as\n                   `https://leetcode.com/contest/weekly-contest-326/`,\n                   `https://leetcode.con/problems/minimum-number-of-\n                   operations-to-reinitialize-a-permutation/`. If type is\n                   `season`, the detail is the season name. Such as\n                   `2020-fall-solo` or `2020-fall-team`.\n  --language TEXT  The language of the code. Now support: `cpp`. Default is\n                   `cpp`.\n  --location TEXT  The location of the code. Default is `./leetcode/`.\n  --help           Show this message and exit.\n```\n\n## Example\n```bash\nleetcode-local-tester work --kind contest --detail https://leetcode.com/contest/weekly-contest-326/ --language cpp --location ./leetcode/\n```\nAfter running the command, you will get the following files:\n\n\n![dir.jpg](https://s2.loli.net/2023/07/25/APhmjgsIa9G3BSw.jpg)\n\n`weekly-contest-326`: The folder of the contest. It contains all test cases and the code file.\n\n`utils`: The folder of the utils. It contains code that is used to parse the test cases. \n\n**Pay attention: `utils` folder is only generated once. After generated the first time, it will not be updated. So you can add your own code in it.**\n\nYou can write your code in `solution.h`. We take the first question in `weekly-contest-300` as an example.\nThe `solution.h` file is like this:\n\n```cpp\n/*\nCode generated by https://github.com/goodstudyqaq/leetcode-local-tester\n*/\n#if __has_include("../utils/cpp/help.hpp")\n#include "../utils/cpp/help.hpp"\n#elif __has_include("../../utils/cpp/help.hpp")\n#include "../../utils/cpp/help.hpp"\n#else\n#define debug(...) 42\n#endif\n\nclass Solution {\n   public:\n    string decodeMessage(string key, string message) {\n        int res[26];\n        memset(res, -1, sizeof(res));\n        int cnt = 0;\n        for (auto v : key) {\n            int cur = v - \'a\';\n            if (cur >= 0 && cur < 26) {\n                if (res[cur] != -1) continue;\n                res[cur] = cnt++;\n            }\n        }\n        string fin;\n        for (auto v : message) {\n            if (v == \' \')\n                fin += \' \';\n            else {\n                char cur = \'a\' + res[v - \'a\'];\n                fin += cur;\n            }\n        }\n        return fin;\n    }\n};\n```\n\nAfter you finish your own code, you can run `main.cpp` to test your code.\n    \n```bash\ng++ main.cpp -std=c++11 -o main && ./main\n\nCase 1 testing...\n[my_ans]: "this is a secret"\n[result]: "this is a secret"\nCase 1 passed!\nCase 2 testing...\n[my_ans]: "the five boxing wizards jump quickly"\n[result]: "the five boxing wizards jump quickly"\nCase 2 passed!\nThe number of test cases: 2\nThe number of test cases failed: 0\n```\n\nIf you get `Wrong answer`, you can snip the test case and paste it into `data` to debug your code.\n**Pay attention: `data`\'s format is Input + Output.**\n\nIn this example, the test case is:\n\n```text\n"the quick brown fox jumps over the lazy dog"\n"vkbs bs t suepuv"\n```\n\n# TODO\n- [ ] Support `python`\n\n# License\nThis software is licensed under the MIT License. See the LICENSE file in the top distribution directory for the full license text.\n\nMaintaining the project is hard and time-consuming, and I\'ve put much ❤️ and effort into this.\n\nIf you\'ve appreciated my work, you can back me up with a donation! Thank you 😊\n\n\n[<img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" width="217px" height="51x">](https://www.buymeacoffee.com/goodstudyqaq)\n\n',
+    'long_description': '# Leetcode-local-tester\n[![Maintenance](https://img.shields.io/badge/maintained-yes-brightgreen.svg)](https://github.com/goodstudyqaq/leetcode-local-tester/graphs/commit-activity)\n[![PyPI version](https://img.shields.io/pypi/v/leetcode-local-tester.svg)](https://pypi.python.org/pypi/leetcode-local-tester/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/leetcode-local-tester.svg)](https://pypi.python.org/pypi/leetcode-local-tester/)\n[![Downloads](https://static.pepy.tech/personalized-badge/leetcode-local-tester?period=month&units=international_system&left_color=grey&right_color=orange&left_text=downloads/month)](https://pepy.tech/project/leetcode-local-tester)\n[![Downloads](https://static.pepy.tech/personalized-badge/leetcode-local-tester?period=total&units=international_system&left_color=grey&right_color=orange&left_text=downloads)](https://pepy.tech/project/leetcode-local-tester)\n![GitHub Sponsors](https://img.shields.io/github/sponsors/goodstudyqaq)\n\n\nLeetcode test utils for local environment\n\n# Background\nBecause of Leetcode\'s special design for test cases, if you want to test your code locally, you need to write some boilerplate code to read the test cases from the file and parse them into the format that your code can understand, which is very annoying. Especially in a contest, you may not have enough time to write the boilerplate code. So I wrote this tool to help me generate the boilerplate code automatically. It will improve your efficiency in a contest.\n\nThe design is really like TopCoder\'s test cases, but TopCoder has a very good tool ([TZTester](https://community.topcoder.com/contest/classes/TZTester/TZTester.html)) to generate the boilerplate code for you, which is very convenient.\n\n# Usage\n\n## Install\n```bash\npip install leetcode-local-tester\n```\n\n## Command\n```bash\nleetcode-local-tester work --help\n\nOptions:\n  --kind TEXT      The question kind. Now support: `contest`, `problem`,\n                   `season`, and `contest` includes `weekly` and `biweekly`.\n                   Default is `problem`.\n  --detail TEXT    The detail of the question. If type is `contest` or\n                   `problem`, the detail is the url. Such as\n                   `https://leetcode.com/contest/weekly-contest-326/`,\n                   `https://leetcode.con/problems/minimum-number-of-\n                   operations-to-reinitialize-a-permutation/`. If type is\n                   `season`, the detail is the season name. Such as\n                   `2020-fall-solo` or `2020-fall-team`.\n  --language TEXT  The language of the code. Now support: `cpp`, `python3`. Default is\n                   `python3`.\n  --location TEXT  The location of the code. Default is `./leetcode/`.\n  --help           Show this message and exit.\n```\n\n## Example\n```bash\nleetcode-local-tester work --kind contest --detail https://leetcode.com/contest/weekly-contest-326/ --language cpp --location ./leetcode/\n```\nAfter running the command, you will get the following files:\n\n\n![dir.jpg](https://s2.loli.net/2023/07/25/APhmjgsIa9G3BSw.jpg)\n\n`weekly-contest-326`: The folder of the contest. It contains all test cases and the code file.\n\n`utils`: The folder of the utils. It contains code that is used to parse the test cases. \n\n**Pay attention: `utils` folder is only generated once. After generated the first time, it will not be updated. So you can add your own code in it.**\n\nYou can write your code in `solution.h`. We take the first question in `weekly-contest-300` as an example.\nThe `solution.h` file is like this:\n\n```cpp\n/*\nCode generated by https://github.com/goodstudyqaq/leetcode-local-tester\n*/\n#if __has_include("../utils/cpp/help.hpp")\n#include "../utils/cpp/help.hpp"\n#elif __has_include("../../utils/cpp/help.hpp")\n#include "../../utils/cpp/help.hpp"\n#else\n#define debug(...) 42\n#endif\n\nclass Solution {\n   public:\n    string decodeMessage(string key, string message) {\n        int res[26];\n        memset(res, -1, sizeof(res));\n        int cnt = 0;\n        for (auto v : key) {\n            int cur = v - \'a\';\n            if (cur >= 0 && cur < 26) {\n                if (res[cur] != -1) continue;\n                res[cur] = cnt++;\n            }\n        }\n        string fin;\n        for (auto v : message) {\n            if (v == \' \')\n                fin += \' \';\n            else {\n                char cur = \'a\' + res[v - \'a\'];\n                fin += cur;\n            }\n        }\n        return fin;\n    }\n};\n```\n\nAfter you finish your own code, you can run `main.cpp` to test your code.\n    \n```bash\ng++ main.cpp -std=c++11 -o main && ./main\n\nCase 1 testing...\n[my_ans]: "this is a secret"\n[result]: "this is a secret"\nCase 1 passed!\nCase 2 testing...\n[my_ans]: "the five boxing wizards jump quickly"\n[result]: "the five boxing wizards jump quickly"\nCase 2 passed!\nThe number of test cases: 2\nThe number of test cases failed: 0\n```\n\nIf you get `Wrong answer`, you can snip the test case and paste it into `data` to debug your code.\n**Pay attention: `data`\'s format is Input + Output.**\n\nIn this example, the test case is:\n\n```text\n"the quick brown fox jumps over the lazy dog"\n"vkbs bs t suepuv"\n```\n\n# TODO\n- [x] Support `python` (completed)\n\n# License\nThis software is licensed under the MIT License. See the LICENSE file in the top distribution directory for the full license text.\n\nMaintaining the project is hard and time-consuming, and I\'ve put much ❤️ and effort into this.\n\nIf you\'ve appreciated my work, you can back me up with a donation! Thank you 😊\n\nIf there is any problem, please create an issue. I will reply to you as soon as possible.\n\n\n[<img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" width="217px" height="51x">](https://www.buymeacoffee.com/goodstudyqaq)\n\n',
     'author': 'shen',
     'author_email': 'goodstudyQAQ@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `leetcode_local_tester-0.2.0/PKG-INFO` & `leetcode_local_tester-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leetcode-local-tester
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: shen
 Author-email: goodstudyQAQ@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -52,16 +52,16 @@
   --detail TEXT    The detail of the question. If type is `contest` or
                    `problem`, the detail is the url. Such as
                    `https://leetcode.com/contest/weekly-contest-326/`,
                    `https://leetcode.con/problems/minimum-number-of-
                    operations-to-reinitialize-a-permutation/`. If type is
                    `season`, the detail is the season name. Such as
                    `2020-fall-solo` or `2020-fall-team`.
-  --language TEXT  The language of the code. Now support: `cpp`. Default is
-                   `cpp`.
+  --language TEXT  The language of the code. Now support: `cpp`, `python3`. Default is
+                   `python3`.
   --location TEXT  The location of the code. Default is `./leetcode/`.
   --help           Show this message and exit.
 ```
 
 ## Example
 ```bash
 leetcode-local-tester work --kind contest --detail https://leetcode.com/contest/weekly-contest-326/ --language cpp --location ./leetcode/
@@ -143,20 +143,22 @@
 
 ```text
 "the quick brown fox jumps over the lazy dog"
 "vkbs bs t suepuv"
 ```
 
 # TODO
-- [ ] Support `python`
+- [x] Support `python` (completed)
 
 # License
 This software is licensed under the MIT License. See the LICENSE file in the top distribution directory for the full license text.
 
 Maintaining the project is hard and time-consuming, and I've put much ❤️ and effort into this.
 
 If you've appreciated my work, you can back me up with a donation! Thank you 😊
 
+If there is any problem, please create an issue. I will reply to you as soon as possible.
+
 
 [<img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" width="217px" height="51x">](https://www.buymeacoffee.com/goodstudyqaq)
```

