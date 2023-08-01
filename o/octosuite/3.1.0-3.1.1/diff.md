# Comparing `tmp/octosuite-3.1.0.tar.gz` & `tmp/octosuite-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octosuite-3.1.0.tar", last modified: Sun Jan 29 08:20:22 2023, max compression
+gzip compressed data, was "octosuite-3.1.1.tar", last modified: Tue Aug  1 00:39:37 2023, max compression
```

## Comparing `octosuite-3.1.0.tar` & `octosuite-3.1.1.tar`

### file list

```diff
@@ -1,23 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 08:20:22.172359 octosuite-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35110 2023-01-29 08:20:13.000000 octosuite-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-01-29 08:20:22.172359 octosuite-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-01-29 08:20:13.000000 octosuite-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 08:20:22.172359 octosuite-3.1.0/octosuite/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 08:20:13.000000 octosuite-3.1.0/octosuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-29 08:20:13.000000 octosuite-3.1.0/octosuite/banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-01-29 08:20:13.000000 octosuite-3.1.0/octosuite/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    26391 2023-01-29 08:20:13.000000 octosuite-3.1.0/octosuite/csv_loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-01-29 08:20:13.000000 octosuite-3.1.0/octosuite/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-29 08:20:13.000000 octosuite-3.1.0/octosuite/log_roller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-01-29 08:20:13.000000 octosuite-3.1.0/octosuite/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-01-29 08:20:13.000000 octosuite-3.1.0/octosuite/message_prefixes.py
--rw-r--r--   0 runner    (1001) docker     (123)    54425 2023-01-29 08:20:13.000000 octosuite-3.1.0/octosuite/octosuite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 08:20:22.172359 octosuite-3.1.0/octosuite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-01-29 08:20:22.000000 octosuite-3.1.0/octosuite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-01-29 08:20:22.000000 octosuite-3.1.0/octosuite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 08:20:22.000000 octosuite-3.1.0/octosuite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-29 08:20:22.000000 octosuite-3.1.0/octosuite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-29 08:20:22.000000 octosuite-3.1.0/octosuite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-29 08:20:22.000000 octosuite-3.1.0/octosuite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-29 08:20:22.172359 octosuite-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-01-29 08:20:13.000000 octosuite-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:39:37.881435 octosuite-3.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:39:37.881435 octosuite-3.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:39:37.881435 octosuite-3.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-01 00:39:27.000000 octosuite-3.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 00:39:27.000000 octosuite-3.1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-01 00:39:27.000000 octosuite-3.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-01 00:39:27.000000 octosuite-3.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:39:37.881435 octosuite-3.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-01 00:39:27.000000 octosuite-3.1.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-01 00:39:27.000000 octosuite-3.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 00:39:27.000000 octosuite-3.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-01 00:39:27.000000 octosuite-3.1.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    35110 2023-08-01 00:39:27.000000 octosuite-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44939 2023-08-01 00:39:37.881435 octosuite-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-08-01 00:39:27.000000 octosuite-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:39:37.881435 octosuite-3.1.1/octosuite/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:39:27.000000 octosuite-3.1.1/octosuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-01 00:39:27.000000 octosuite-3.1.1/octosuite/banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-08-01 00:39:27.000000 octosuite-3.1.1/octosuite/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26391 2023-08-01 00:39:27.000000 octosuite-3.1.1/octosuite/csv_loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-08-01 00:39:27.000000 octosuite-3.1.1/octosuite/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-01 00:39:27.000000 octosuite-3.1.1/octosuite/log_roller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-08-01 00:39:27.000000 octosuite-3.1.1/octosuite/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-01 00:39:27.000000 octosuite-3.1.1/octosuite/message_prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53734 2023-08-01 00:39:27.000000 octosuite-3.1.1/octosuite/octosuite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:39:37.881435 octosuite-3.1.1/octosuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44939 2023-08-01 00:39:37.000000 octosuite-3.1.1/octosuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-01 00:39:37.000000 octosuite-3.1.1/octosuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:39:37.000000 octosuite-3.1.1/octosuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 00:39:37.000000 octosuite-3.1.1/octosuite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 00:39:37.000000 octosuite-3.1.1/octosuite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 00:39:37.000000 octosuite-3.1.1/octosuite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-01 00:39:27.000000 octosuite-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:39:37.881435 octosuite-3.1.1/setup.cfg
```

### Comparing `octosuite-3.1.0/LICENSE` & `octosuite-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `octosuite-3.1.0/PKG-INFO` & `octosuite-3.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,10 @@
-Metadata-Version: 2.1
-Name: octosuite
-Version: 3.1.0
-Summary: Advanced Github OSINT Framework
-Home-page: https://github.com/bellingcat/octosuite
-Author: Richard Mwewa
-Author-email: rly0nheart@duck.com
-License: GNU General Public License v3 (GPLv3)
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![logo](https://user-images.githubusercontent.com/74001397/175805580-fffc96d4-e0ef-48bb-a55c-80b2da3e714d.png)
 
-A framework for gathering open-source intelligence on GitHub users, repositories and organizations
+A framework for gathering open-source intelligence on GitHub users, repositories and organisations
 
 [![Upload Python Package](https://github.com/bellingcat/octosuite/actions/workflows/python-publish.yml/badge.svg)](https://github.com/bellingcat/octosuite/actions/workflows/python-publish.yml)
 [![CodeQL](https://github.com/bellingcat/octosuite/actions/workflows/codeql.yml/badge.svg)](https://github.com/bellingcat/octosuite/actions/workflows/codeql.yml)
 ![GitHub](https://img.shields.io/github/license/bellingcat/octosuite?style=flat)
 ![PyPI](https://img.shields.io/pypi/v/octosuite?style=flat&logo=pypi)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/octosuite?style=flat&logo=pypi)
 ![PyPI - Status](https://img.shields.io/pypi/status/octosuite?style=flat&logo=pypi)
@@ -33,45 +16,48 @@
 
 ![Screen Shot 2023-01-26 at 9 27 22 PM](https://user-images.githubusercontent.com/74001397/214932206-40ec42ba-4fe8-4115-b2dd-52c4d7be9b5c.png)
 
 # Wiki
 [Refer to the Wiki](https://github.com/bellingcat/octosuite/wiki) for installation instructions, in addition to all other documentation.
 
 # Features
-- [x] Fetches an organization's profile information
+- [x] Fetches an organisation's profile information
 - [x] Fetches an oganization's events
-- [x] Returns an organization's repositories
-- [x] Returns an organization's public members
+- [x] Returns an organisation's repositories
+- [x] Returns an organisation's public members
 - [x] Fetches a repository's information
 - [x] Returns a repository's contributors
 - [x] Returns a repository's languages
 - [x] Fetches a repository's stargazers
 - [x] Fetches a repository's forks
 - [x] Fetches a repository's releases
 - [x] Returns a list of files in a specified path of a repository
 - [x] Fetches a user's profile information
 - [x] Returns a user's gists
-- [x] Returns organizations that a user owns/belongs to
+- [x] Returns organisations that a user owns/belongs to
 - [x] Fetches a user's events
 - [x] Fetches a list of users followed by the target
 - [x] Fetches a user's followers
 - [x] Checks if user A follows user B
-- [x] Checks if  user is a public member of an organizations
-- [x] Returns a user's subscriptions
+- [x] Checks if  user is a public member of an organisations
 - [x] Gets a user's subscriptions
-- [x] Gets a user's events
 - [x] Searches users
 - [x] Searches repositories
 - [x] Searches topics
 - [x] Searches issues
 - [x] Searches commits
-- [x] Automatically logs network activity (.logs folder)
-- [x] User can view, read and delete logs
+- [x] Automatically logs network/user activity (.logs folder)
+- [x] User can manage logs (view, read, delete)
+- [x] Results can be saved to a .csv file (varies)
+- [x] User can manage csv files (view, read, delete)
 - [x] All the above can be used with command-line arguments (PyPI Package only)
-- [x] ...And more
+- [x] And more...
+
+# TODO
+- [ ] Rewrite the GUI in Visual Basic .NET (in progress)
 
 
 ## Note
 > Octosuite automatically logs network and user activity of each session, the logs are saved by date and time in the .logs folder
 
 
 # License
```

#### html2text {}

```diff
@@ -1,53 +1,46 @@
-Metadata-Version: 2.1 Name: octosuite Version: 3.1.0 Summary: Advanced Github
-OSINT Framework Home-page: https://github.com/bellingcat/octosuite Author:
-Richard Mwewa Author-email: rly0nheart@duck.com License: GNU General Public
-License v3 (GPLv3) Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Information Technology Classifier: License ::
-OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
-System :: OS Independent Classifier: Natural Language :: English Classifier:
-Programming Language :: Python :: 3 Description-Content-Type: text/markdown
-License-File: LICENSE ![logo](https://user-images.githubusercontent.com/
-74001397/175805580-fffc96d4-e0ef-48bb-a55c-80b2da3e714d.png) A framework for
-gathering open-source intelligence on GitHub users, repositories and
-organizations [![Upload Python Package](https://github.com/bellingcat/
-octosuite/actions/workflows/python-publish.yml/badge.svg)](https://github.com/
-bellingcat/octosuite/actions/workflows/python-publish.yml) [![CodeQL](https://
-github.com/bellingcat/octosuite/actions/workflows/codeql.yml/badge.svg)](https:
-//github.com/bellingcat/octosuite/actions/workflows/codeql.yml) ![GitHub]
-(https://img.shields.io/github/license/bellingcat/octosuite?style=flat) ![PyPI]
-(https://img.shields.io/pypi/v/octosuite?style=flat&logo=pypi) ![PyPI -
-Downloads](https://img.shields.io/pypi/dw/octosuite?style=flat&logo=pypi) !
-[PyPI - Status](https://img.shields.io/pypi/status/
-octosuite?style=flat&logo=pypi) ![GitHub repo size](https://img.shields.io/
-github/repo-size/bellingcat/octosuite?style=flat&logo=github) ![2023-01-23_01-
-01](https://user-images.githubusercontent.com/74001397/213950701-44b3f98b-89e1-
-443a-abb5-1be8969b611f.png "Octosuite about") ![Screen Shot 2023-01-26 at 9 27
-22 PM](https://user-images.githubusercontent.com/74001397/214932206-40ec42ba-
-4fe8-4115-b2dd-52c4d7be9b5c.png) # Wiki [Refer to the Wiki](https://github.com/
+![logo](https://user-images.githubusercontent.com/74001397/175805580-fffc96d4-
+e0ef-48bb-a55c-80b2da3e714d.png) A framework for gathering open-source
+intelligence on GitHub users, repositories and organisations [![Upload Python
+Package](https://github.com/bellingcat/octosuite/actions/workflows/python-
+publish.yml/badge.svg)](https://github.com/bellingcat/octosuite/actions/
+workflows/python-publish.yml) [![CodeQL](https://github.com/bellingcat/
+octosuite/actions/workflows/codeql.yml/badge.svg)](https://github.com/
+bellingcat/octosuite/actions/workflows/codeql.yml) ![GitHub](https://
+img.shields.io/github/license/bellingcat/octosuite?style=flat) ![PyPI](https://
+img.shields.io/pypi/v/octosuite?style=flat&logo=pypi) ![PyPI - Downloads]
+(https://img.shields.io/pypi/dw/octosuite?style=flat&logo=pypi) ![PyPI -
+Status](https://img.shields.io/pypi/status/octosuite?style=flat&logo=pypi) !
+[GitHub repo size](https://img.shields.io/github/repo-size/bellingcat/
+octosuite?style=flat&logo=github) ![2023-01-23_01-01](https://user-
+images.githubusercontent.com/74001397/213950701-44b3f98b-89e1-443a-abb5-
+1be8969b611f.png "Octosuite about") ![Screen Shot 2023-01-26 at 9 27 22 PM]
+(https://user-images.githubusercontent.com/74001397/214932206-40ec42ba-4fe8-
+4115-b2dd-52c4d7be9b5c.png) # Wiki [Refer to the Wiki](https://github.com/
 bellingcat/octosuite/wiki) for installation instructions, in addition to all
-other documentation. # Features - [x] Fetches an organization's profile
+other documentation. # Features - [x] Fetches an organisation's profile
 information - [x] Fetches an oganization's events - [x] Returns an
-organization's repositories - [x] Returns an organization's public members -
+organisation's repositories - [x] Returns an organisation's public members -
 [x] Fetches a repository's information - [x] Returns a repository's
 contributors - [x] Returns a repository's languages - [x] Fetches a
 repository's stargazers - [x] Fetches a repository's forks - [x] Fetches a
 repository's releases - [x] Returns a list of files in a specified path of a
 repository - [x] Fetches a user's profile information - [x] Returns a user's
-gists - [x] Returns organizations that a user owns/belongs to - [x] Fetches a
+gists - [x] Returns organisations that a user owns/belongs to - [x] Fetches a
 user's events - [x] Fetches a list of users followed by the target - [x]
 Fetches a user's followers - [x] Checks if user A follows user B - [x] Checks
-if user is a public member of an organizations - [x] Returns a user's
-subscriptions - [x] Gets a user's subscriptions - [x] Gets a user's events -
-[x] Searches users - [x] Searches repositories - [x] Searches topics - [x]
-Searches issues - [x] Searches commits - [x] Automatically logs network
-activity (.logs folder) - [x] User can view, read and delete logs - [x] All the
-above can be used with command-line arguments (PyPI Package only) - [x] ...And
-more ## Note > Octosuite automatically logs network and user activity of each
-session, the logs are saved by date and time in the .logs folder # License !
-[license](https://user-images.githubusercontent.com/74001397/137917929-
-2f2cdb0c-4d1d-4e4b-9f0d-e01589e027b5.png) # Credits * The code used for finding
-emails from usernames is taken from [Somdev Sangwan](https://github.com/
-s0md3v)'s [Zen](https://github.com/s0md3v/zen) # Donations If you like
-OctoSuite and would like to show support, you can Buy A Coffee for the
-developer using the button below [Buy_Me_A_Coffee] Your support will be much
-appreciatedð
+if user is a public member of an organisations - [x] Gets a user's
+subscriptions - [x] Searches users - [x] Searches repositories - [x] Searches
+topics - [x] Searches issues - [x] Searches commits - [x] Automatically logs
+network/user activity (.logs folder) - [x] User can manage logs (view, read,
+delete) - [x] Results can be saved to a .csv file (varies) - [x] User can
+manage csv files (view, read, delete) - [x] All the above can be used with
+command-line arguments (PyPI Package only) - [x] And more... # TODO - [ ]
+Rewrite the GUI in Visual Basic .NET (in progress) ## Note > Octosuite
+automatically logs network and user activity of each session, the logs are
+saved by date and time in the .logs folder # License ![license](https://user-
+images.githubusercontent.com/74001397/137917929-2f2cdb0c-4d1d-4e4b-9f0d-
+e01589e027b5.png) # Credits * The code used for finding emails from usernames
+is taken from [Somdev Sangwan](https://github.com/s0md3v)'s [Zen](https://
+github.com/s0md3v/zen) # Donations If you like OctoSuite and would like to show
+support, you can Buy A Coffee for the developer using the button below [Buy_Me
+A_Coffee] Your support will be much appreciatedð
```

### Comparing `octosuite-3.1.0/octosuite/banner.py` & `octosuite-3.1.1/octosuite/banner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import getpass
 from octosuite.config import red, white, green, reset, Tree
 
 
 # banner.py
 # This file holds the program's banner and version tag
-version_tag = "3.1.0"
+version_tag = "3.1.1"
 
 
 def banner():
     banner_tree = Tree(getpass.getuser())
     banner_tree.add(f"use ‘{green}help{reset}’ command for usage")
     banner_tree.add(f"commands are case insensitive\n")
     return f"""
```

### Comparing `octosuite-3.1.0/octosuite/config.py` & `octosuite-3.1.1/octosuite/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import os
 import psutil
 import platform
 import argparse
 from rich.tree import Tree
 from rich.text import Text
 from rich.table import Table
 from datetime import datetime
 from rich import print as xprint
+from rich.markdown import Markdown
 from rich.prompt import Prompt, Confirm
 
 
 def usage():
     return """
     Basic Usage
     ===========
@@ -20,22 +22,22 @@
 
 
         Get User Repos
         --------------
         octosuite --method user_repos --username <username>
 
 
-        Get Organi[sz]ation Profile Info
+        Get Organisation Profile Info
         -----------------------------
-        octosuite --method org_profile --organization <organization_name>
+        octosuite --method org_profile --organisation <organisation_name>
 
 
         Get Organi[sz]ation Repos
         -----------------------------
-        octosuite --method org_repos --organization <organization_name>
+        octosuite --method org_repos --organisation <organisation_name>
 
         
         Get Repo Profile Info
         ---------------------
         octosuite --method repo_profile --username <username> --repository <repo_name>
 
 
@@ -129,26 +131,48 @@
                                                                   'org_profile', 'org_repos', 'org_events', 'org_member',
                                                                   'repo_profile', 'repo_contributors', 'repo_stargazers', 'repo_forks',
                                                                   'repo_issues', 'repo_releases', 'repo_path_contents', 'users_search', 'issues_search',
                                                                   'commits_search', 'topics_search', 'repos_search', 'view_logs', 'read_log', 'delete_log', 
                                                                   'clear_logs', 'view_csv', 'read_csv', 'delete_csv', 'clear_csv', 'about', 'author'])
     parser.add_argument('-u', '--username', help='username')
     parser.add_argument('-uB', '--username_b', help='username_B (used with user_follows)')
-    parser.add_argument('-o', '--organization', '--organisation', help='organi[sz]ation name')
+    parser.add_argument('-o', '--organisation', '--organization', help='organisation name')
     parser.add_argument('-r', '--repository', help='repository name')
     parser.add_argument('-p', '--path_name', help='path name (used with repo_path_contents)')
     parser.add_argument('-q', '--query', help='query (used with search methods)')
     parser.add_argument('-l', '--limit', help='output limit (used with methods that return results in bulk) (default: %(default)s)', default=10)
     parser.add_argument('-c', '--colors', '--colours', help='specify to run octosuite cli with colo[u]rs enabled', action='store_true')
     parser.add_argument('--csv_file', help='csv file (used with csv management methods)')
     parser.add_argument('--log_file', help='log file (used with logs management methods)')
     parser.add_argument('--log-to-csv', help='log output to a csv file', action='store_true', dest='log_csv')
     return parser
 
 
+# Setup readline
+def setup_readline():
+    if os.name == "nt":
+        try:
+            from pyreadline3 import Readline
+        except ImportError:
+            subprocess.run(['pip3', 'install', 'pyreadline3'], shell=False)
+        readline = Readline()
+    else:
+        import readline
+        
+        def completer(text, state):
+            options = [i for i in commands if i.startswith(text)]
+            if state < len(options):
+                return options[state]
+            else:
+                return None
+                
+        readline.parse_and_bind("tab: complete")
+        readline.set_completer(completer)
+
+
 parser = create_parser()
 args = parser.parse_args()
 
 # This file is responsible for enabling/disabling colo[u]rs and configuring argparse in OctoSuite
 # This file gets called first at start up before any other file
 # config.py is the reason why users get to choose whether to enable/disable colo[u]rs, and call the program with command line arguments
 # delete this file (I dare you), the entire program breaks
```

### Comparing `octosuite-3.1.0/octosuite/csv_loggers.py` & `octosuite-3.1.1/octosuite/csv_loggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 
 # csv_loggers.py
 # This file holds the functions for creating .csv files of each functionality in main
 def log_org_profile(response):
     org_profile_fields = ['Profile photo', 'Name', 'Username', 'ID', 'Node ID', 'Email', 'About', 'Location', 'Blog',
                           'Followers', 'Following', 'Twitter handle', 'Gists', 'Repositories', 'Account type',
-                          'Is verified?', 'Has organization projects?', 'Has repository projects?', 'Created at',
+                          'Is verified?', 'Has organisation projects?', 'Has repository projects?', 'Created at',
                           'Updated at']
     org_profile_row = [response.json()['avatar_url'], response.json()['name'], response.json()['login'],
                        response.json()['id'], response.json()['node_id'], response.json()['email'],
                        response.json()['description'], response.json()['location'], response.json()['blog'],
                        response.json()['followers'], response.json()['following'], response.json()['twitter_username'],
                        response.json()['public_gists'], response.json()['public_repos'], response.json()['type'],
-                       response.json()['is_verified'], response.json()['has_organization_projects'],
+                       response.json()['is_verified'], response.json()['has_organisation_projects'],
                        response.json()['has_repository_projects'], response.json()['created_at'],
                        response.json()['updated_at']]
     
     with open(os.path.join("output", f"{response.json()['name']}.csv"), 'w') as file:
         write_csv = csv.writer(file)
         write_csv.writerow(org_profile_fields)
         write_csv.writerow(org_profile_row)
@@ -30,15 +30,15 @@
         logging.info(logged_to_csv.format(file.name))
         xprint(f"{POSITIVE} {logged_to_csv.format(file.name)}")
 
     
 # Creating a .csv file of a user' profile
 def log_user_profile(response):
     user_profile_fields = ['Profile photo', 'Name', 'Username', 'ID', 'Node ID', 'Bio', 'Blog', 'Location', 'Followers',
-                           'Following', 'Twitter handle', 'Gists', 'Repositories', 'Organization', 'Is hireable?',
+                           'Following', 'Twitter handle', 'Gists', 'Repositories', 'organisation', 'Is hireable?',
                            'Is site admin?', 'Joined at', 'Updated at']
     user_profile_row = [response.json()['avatar_url'], response.json()['name'], response.json()['login'],
                         response.json()['id'], response.json()['node_id'], response.json()['bio'],
                         response.json()['blog'], response.json()['location'], response.json()['followers'],
                         response.json()['following'], response.json()['twitter_username'],
                         response.json()['public_gists'], response.json()['public_repos'], response.json()['company'],
                         response.json()['hireable'], response.json()['site_admin'], response.json()['created_at'],
@@ -180,44 +180,44 @@
         write_csv.writerow(repo_contributor_fields)
         write_csv.writerow(repo_contributor_row)
 
         logging.info(logged_to_csv.format(file.name))
         xprint(f"{POSITIVE} {logged_to_csv.format(file.name)}")
 
    
-# Create .csv for organization' events
-def log_repo_events(event, organization):
+# Create .csv for organisation' events
+def log_repo_events(event, organisation):
     org_event_fields = ['ID', 'Type', 'Created at', 'Payload']
     org_event_row = [event['id'], event['type'], event['created_at'], event['payload']]
     
-    with open(os.path.join("output", f"{organization}_event_{event['id']}.csv"), 'w') as file:
+    with open(os.path.join("output", f"{organisation}_event_{event['id']}.csv"), 'w') as file:
         write_csv = csv.writer(file)
         write_csv.writerow(org_event_fields)
         write_csv.writerow(org_event_row)
 
         logging.info(logged_to_csv.format(file.name))
         xprint(f"{POSITIVE} {logged_to_csv.format(file.name)}")
 
     
-# Create .csv for organization' repositories
-def log_org_repos(repository, organization):
+# Create .csv for organisation' repositories
+def log_org_repos(repository, organisation):
     org_repo_fields = ['Name', 'ID', 'About', 'Forks', 'Stars', 'Watchers', 'License', 'Branch', 'Visibility',
                        'Language(s)', 'Open issues', 'Topics', 'Homepage', 'Clone URL', 'SSH URL', 'Is fork?',
                        'Is forkable?', 'Is private?', 'Is archived?', 'Is template?', 'Has wiki?', 'Has pages?',
                        'Has projects?', 'Has issues?', 'Has downloads?', 'Pushed at', 'Created at', 'Updated at']
     org_repo_row = [repository['full_name'], repository['id'], repository['description'], repository['forks'],
                     repository['stargazers_count'], repository['watchers'], repository['license'],
                     repository['default_branch'], repository['visibility'], repository['language'],
                     repository['open_issues'], repository['topics'], repository['homepage'], repository['clone_url'],
                     repository['ssh_url'], repository['fork'], repository['allow_forking'], repository['private'],
                     repository['archived'], repository['is_template'], repository['has_wiki'], repository['has_pages'],
                     repository['has_projects'], repository['has_issues'], repository['has_downloads'],
                     repository['pushed_at'], repository['created_at'], repository['updated_at']]
     
-    with open(os.path.join("output", f"{repository['name']}_repository_of_{organization}.csv"), 'w') as file:
+    with open(os.path.join("output", f"{repository['name']}_repository_of_{organisation}.csv"), 'w') as file:
         write_csv = csv.writer(file)
         write_csv.writerow(org_repo_fields)
         write_csv.writerow(org_repo_row)
 
         logging.info(logged_to_csv.format(file.name))
         xprint(f"{POSITIVE} {logged_to_csv.format(file.name)}")
 
@@ -331,21 +331,21 @@
         write_csv.writerow(user_subscription_fields)
         write_csv.writerow(user_subscription_row)
 
         logging.info(logged_to_csv.format(file.name))
         xprint(f"{POSITIVE} {logged_to_csv.format(file.name)}")
 
     
-# .csv for user organizations
-def log_user_orgs(organization, username):
+# .csv for user organisations
+def log_user_orgs(organisation, username):
     user_org_fields = ['Profile photo', 'Name', 'ID', 'Node ID', 'URL', 'About']
-    user_org_row = [organization['avatar_url'], organization['login'], organization['id'], organization['node_id'],
-                    organization['url'], organization['description']]
+    user_org_row = [organisation['avatar_url'], organisation['login'], organisation['id'], organisation['node_id'],
+                    organisation['url'], organisation['description']]
     
-    with open(os.path.join("output", f"{organization['login']}_{username}.csv"), 'w') as file:
+    with open(os.path.join("output", f"{organisation['login']}_{username}.csv"), 'w') as file:
         write_csv = csv.writer(file)
         write_csv.writerow(user_org_fields)
         write_csv.writerow(user_org_row)
 
         logging.info(logged_to_csv.format(file.name))
         xprint(f"{POSITIVE} {logged_to_csv.format(file.name)}")
```

### Comparing `octosuite-3.1.0/octosuite/helper.py` & `octosuite-3.1.1/octosuite/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 def user_command():
     user_cmd_table = Table(show_header=True, header_style=header_title)
     user_cmd_table.add_column("Command", style="dim")
     user_cmd_table.add_column("Description")
     user_cmd_table.add_row("email", "Return a target's email")
     user_cmd_table.add_row("profile", "Get a target's profile info")
     user_cmd_table.add_row("gists", "Return a users's gists")
-    user_cmd_table.add_row("org", "Return organizations that a target belongs to/owns")
+    user_cmd_table.add_row("orgs", "Return organisations that a target belongs to/owns")
     user_cmd_table.add_row("repos", "Return a target's repositories")
     user_cmd_table.add_row("events", "Return a target's events")
     user_cmd_table.add_row("follows", "Check if user(A) follows user(B)")
     user_cmd_table.add_row("followers", "Return a target's followers")
     user_cmd_table.add_row("following", "Return a list of users the target is following")
     user_cmd_table.add_row("subscriptions", "Return a target's subscriptions")
 
@@ -83,21 +83,21 @@
     xprint(user_cmd_table)
 
 
 def org_command():
     org_cmd_table = Table(show_header=True, header_style=header_title)
     org_cmd_table.add_column("Command", style="dim")
     org_cmd_table.add_column("Description")
-    org_cmd_table.add_row("profile", "Get a target organization' profile info")
-    org_cmd_table.add_row("repos", "Return a target organization' repositories")
-    org_cmd_table.add_row("events", "Return a target organization' events")
-    org_cmd_table.add_row("member", "Check if a specified user is a public member of the target organization")
+    org_cmd_table.add_row("profile", "Get a target organisation' profile info")
+    org_cmd_table.add_row("repos", "Return a target organisation' repositories")
+    org_cmd_table.add_row("events", "Return a target organisation' events")
+    org_cmd_table.add_row("member", "Check if a specified user is a public member of the target organisation")
 
     syntax = f"{green}org:<command>{reset}"
-    xprint(f"{usage_text.format(syntax, 'organization investigation(s)')}")
+    xprint(f"{usage_text.format(syntax, 'organisation investigation(s)')}")
     xprint(org_cmd_table)
 
 
 def repo_command():
     repo_cmd_table = Table(show_header=True, header_style=header_title)
     repo_cmd_table.add_column("Command", style="dim")
     repo_cmd_table.add_column("Description")
@@ -155,15 +155,15 @@
     core_cmd_table.add_row("author", "Developer's info")
 
     help_sub_cmd_table = Table(show_header=True, header_style=header_title)
     help_sub_cmd_table.add_column("Command", style="dim", width=12)
     help_sub_cmd_table.add_column("Description")
     help_sub_cmd_table.add_row("csv", "List all csv management commands")
     help_sub_cmd_table.add_row("logs", "List all logs management commands")
-    help_sub_cmd_table.add_row("org", "List all organization investigation commands")
+    help_sub_cmd_table.add_row("org", "List all organisation investigation commands")
     help_sub_cmd_table.add_row("user", "List all users investigation commands")
     help_sub_cmd_table.add_row("repo", "List all repository investigation commands")
     help_sub_cmd_table.add_row("search", "List all target discovery commands")
     help_sub_cmd_table.add_row("source", "List all source code download commands (for developers)")
 
     syntax = f"{green}help:<command>{reset}"
     xprint(core_cmd_table)
```

### Comparing `octosuite-3.1.0/octosuite/log_roller.py` & `octosuite-3.1.1/octosuite/log_roller.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 viewing_csv = "Viewing CSV file(s)..."
 deleted = "Deleted: {}"
 reading = "Reading: {}"
 file_downloading = "Downloading: {}"
 file_downloaded = "Downloaded: downloads/{}"
 info_not_found = "Information not found: {}, {}, {}"
 user_not_found = "User not found: @{}"
-org_not_found = "Organization not found: @{}"
+org_not_found = "organisation not found: @{}"
 repo_or_user_not_found = "Repository or User not found: {}, @{}"
 prompt_log_csv = "Would you like to log this output to a .csv file?"
 logged_to_csv = "Output logged: {}"
 limit_output = "Limit '{}' output to how many? (1-100)"
```

### Comparing `octosuite-3.1.0/octosuite/main.py` & `octosuite-3.1.1/octosuite/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # import everything from the octosuite.py file
 from octosuite.octosuite import *  # I drifted away from the 'pythonic way' here
 
 
 def octosuite():
+    setup_readline()
     try:
         run = Octosuite()
         path_finder()
         configure_logging()
         check_updates()
         if args.method:
             """
```

### Comparing `octosuite-3.1.0/octosuite/message_prefixes.py` & `octosuite-3.1.1/octosuite/message_prefixes.py`

 * *Files identical despite different names*

### Comparing `octosuite-3.1.0/octosuite/octosuite.py` & `octosuite-3.1.1/octosuite/octosuite.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,49 +8,28 @@
 import getpass
 import requests
 import platform
 import subprocess
 from datetime import datetime
 from requests.auth import HTTPBasicAuth
 from octosuite.banner import version_tag, banner
-from octosuite.config import Tree, Text, Table, Prompt, Confirm, xprint, create_parser, args, red, white, green, yellow, header_title, reset
-from octosuite.message_prefixes import ERROR, WARNING, PROMPT, POSITIVE, NEGATIVE, INFO  # wondering why I name all the variables instead of just using the * wildcard?, because it's the pythonic way lol
-# seriously now, the reason why I am doing this, is so that you know exactly what I am importing from a named module :)
+from octosuite.config import Tree, Text, Table, Prompt, Confirm, Markdown, xprint, create_parser, setup_readline, args, red, white, green, yellow, header_title, reset
+from octosuite.message_prefixes import ERROR, WARNING, PROMPT, POSITIVE, NEGATIVE, INFO
 from octosuite.helper import help_command, source_command, search_command, user_command, repo_command, \
     logs_command, csv_command, org_command, source, org, repo, user, search, logs, csv
 from octosuite.log_roller import ctrl_c, error, session_opened, session_closed, viewing_logs, viewing_csv, \
     deleted, reading, file_downloading, file_downloaded, info_not_found, \
     user_not_found, org_not_found, repo_or_user_not_found, limit_output, prompt_log_csv
 from octosuite.csv_loggers import log_org_profile, log_user_profile, log_repo_profile, log_repo_path_contents, \
     log_repo_contributors, log_repo_stargazers, log_repo_forks, log_repo_issues, log_repo_releases, log_org_repos, \
     log_org_profile, log_user_repos, log_user_gists, log_user_orgs, log_user_events, log_user_subscriptions, \
     log_user_following, log_user_followers, log_repos_search, log_users_search, log_topics_search, log_issues_search, \
     log_commits_search
 
 
-if os.name == "nt":
-    try:
-        from pyreadline3 import Readline
-    except ImportError:
-        subprocess.run(['pip3', 'install', 'pyreadline3'], shell=False)
-    readline = Readline()
-else:
-    import readline
-
-    def completer(text, state):
-        options = [i for i in commands if i.startswith(text)]
-        if state < len(options):
-            return options[state]
-        else:
-            return None
-
-    readline.parse_and_bind("tab: complete")
-    readline.set_completer(completer)
-
-
 # path_finder()
 # This function is responsible for creating/checking the availability of  the (.logs, output, downloads) folders,
 # enabling logging to automatically log network/user activity to a file, and logging the start of a session.
 def path_finder():
     """
     Check 3 directories (.logs, output, downloads) on startup
     If they exist, ignore, otherwise, create them
@@ -70,23 +49,28 @@
     logging.info(session_opened.format(platform.node(), getpass.getuser()))
 
 
 # Check if the remote tag_name from the latest release matches the one in the program
 # if it does, it means the program is up-to-date.
 # If it doesn't match, notify the user about a new release
 def check_updates():
+    global markdown_release_notes
+    
     response = requests.get("https://api.github.com/repos/bellingcat/octosuite/releases/latest").json()
     if response['tag_name'] == version_tag:
         pass
     else:
-        xprint(f"[{green}UPDATE{reset}] A new release of Octosuite is available ({response['tag_name']}). Run 'pip install --upgrade octosuite' to get the updates.\n")
+        raw_release_notes = response['body']
+        markdown_release_notes = Markdown(raw_release_notes)
+        xprint(f"[{green}UPDATE{reset}] A new release of Octosuite is available ({response['tag_name']}).\n")
+        xprint(markdown_release_notes)
 
 
 def list_dir_and_files():
-    os.system('dir' if os.name == 'nt' else 'ls')
+    subprocess.call('cmd.exe /c dir' if os.name == "nt" else 'ls')
 
 
 # Delete a specified csv file
 def delete_csv():
     if args.csv_file:
         csv_file = args.csv_file
     else:
@@ -186,31 +170,29 @@
         pass
 
 
 # Clear screen
 def clear_screen():
     # Using 'cls' on Windows machines to clear the screen,
     # otherwise, use 'clear'
-    os.system('cls' if os.name == 'nt' else 'clear')
+    subprocess.call('cmd.exe /c cls' if os.name == "nt" else 'clear')
 
 
 def about():
     about_text = f"""
     OCTOSUITE © 2023 Richard Mwewa
         
-An advanced and lightning fast framework for gathering open-source intelligence on GitHub users and organizations.
-
-
-Whats new in v{version_tag}?
-[{green}IMPROVED{reset}] Added a subcommand to the 'user' commands, that will be used to get a user's email 'user:email' (CLI only)
+An advanced and lightning fast framework for gathering open-source intelligence on GitHub users and organisations.
 
 Read the wiki: https://github.com/bellingcat/octosuite/wiki
 GitHub REST API documentation: https://docs.github.com/rest
+
 """
     xprint(about_text)
+    xprint(markdown_release_notes)
 
 
 def get_email_from_contributor(username, repo, contributor):
     response = requests.get(f"https://github.com/{username}/{repo}/commits?author={contributor}",
                             auth=HTTPBasicAuth(username, '')).text
     latest_commit = re.search(rf'href="/{username}/{repo}/commit/(.*?)"', response)
     if latest_commit:
@@ -331,20 +313,20 @@
         # Path attribute dictionary
         self.path_attr_dict = {'size': 'Size (bytes)',
                                'type': 'Type',
                                'path': 'Path',
                                'sha': 'SHA',
                                'html_url': 'URL'}
 
-        # Organization attributes
+        # organisation attributes
         self.org_attrs = ['avatar_url', 'login', 'id', 'node_id', 'email', 'description', 'blog', 'location',
                           'followers',
                           'following', 'twitter_username', 'public_gists', 'public_repos', 'type', 'is_verified',
-                          'has_organization_projects', 'has_repository_projects', 'created_at', 'updated_at']
-        # Organization attribute dictionary
+                          'has_organisation_projects', 'has_repository_projects', 'created_at', 'updated_at']
+        # organisation attribute dictionary
         self.org_attr_dict = {'avatar_url': 'Profile Photo',
                               'login': 'Username',
                               'id': 'ID',
                               'node_id': 'Node ID',
                               'email': 'Email',
                               'description': 'About',
                               'location': 'Location',
@@ -352,15 +334,15 @@
                               'followers': 'Followers',
                               'following': 'Following',
                               'twitter_username': 'Twitter handle',
                               'public_gists': 'Gists',
                               'public_repos': 'Repositories',
                               'type': 'Account type',
                               'is_verified': 'Is verified?',
-                              'has_organization_projects': 'Has organization projects?',
+                              'has_organisation_projects': 'Has organisation projects?',
                               'has_repository_projects': 'Has repository projects?',
                               'created_at': 'Created at',
                               'updated_at': 'Updated at'}
 
         # Repository attributes
         self.repo_attrs = ['id', 'description', 'forks', 'stargazers_count', 'watchers', 'license', 'default_branch',
                            'visibility',
@@ -428,15 +410,15 @@
                                   'blog': 'Blog',
                                   'location': 'Location',
                                   'followers': 'Followers',
                                   'following': 'Following',
                                   'twitter_username': 'Twitter Handle',
                                   'public_gists': 'Gists (public)',
                                   'public_repos': 'Repositories (public)',
-                                  'company': 'Organization',
+                                  'company': 'organisation',
                                   'hireable': 'Is hireable?',
                                   'site_admin': 'Is site admin?',
                                   'created_at': 'Joined at',
                                   'updated_at': 'Updated at'}
 
         # User attributes
         self.user_attrs = ['avatar_url', 'id', 'node_id', 'gravatar_id', 'site_admin', 'type', 'html_url']
@@ -512,15 +494,15 @@
                                       'labels': 'Labels',
                                       'locked': 'Is locked?',
                                       'active_lock_reason': 'Lock reason',
                                       'closed_at': 'Closed at',
                                       'created_at': 'Created at',
                                       'updated_at': 'Updated at'}
 
-        # User organizations attributes
+        # User organisations attributes
         self.user_orgs_attrs = ['avatar_url', 'id', 'node_id', 'url', 'description']
         self.user_orgs_attr_dict = {'avatar_url': 'Profile Photo',
                                     'id': 'ID',
                                     'node_id': 'Node ID',
                                     'url': 'URL',
                                     'description': 'About'}
 
@@ -548,25 +530,25 @@
         repos = self.get_repos_from_username(username)
         for repo in repos:
             email = get_email_from_contributor(username, repo, username)
             if email:
                 xprint(f"{username}: {email}")
                 break
 
-    # Fetching organization info
+    # Fetching organisation info
     def org_profile(self):
-        if args.organization:
-            organization = args.organization
+        if args.organisation:
+            organisation = args.organisation
         else:
-            organization = Prompt.ask(f"{white}@{green}Organi[sz]ation{reset}")
-        response = requests.get(f"{self.endpoint}/orgs/{organization}")
+            organisation = Prompt.ask(f"{white}@{green}Organisation{reset}")
+        response = requests.get(f"{self.endpoint}/orgs/{organisation}")
         if response.status_code == 404:
-            xprint(f"{NEGATIVE} {org_not_found.format(organization)}")
+            xprint(f"{NEGATIVE} {org_not_found.format(organisation)}")
         elif response.status_code == 200:
-            org_profile_tree = Tree("\n{response.json()['name']}")
+            org_profile_tree = Tree(f"\n{response.json()['name']}")
             for attr in self.org_attrs:
                 org_profile_tree.add(f"{self.org_attr_dict[attr]}: {response.json()[attr]}")
             xprint(org_profile_tree)
 
             if args.log_csv or Confirm.ask(f"\n{PROMPT} {prompt_log_csv}"):
                 log_org_profile(response)
         else:
@@ -768,70 +750,70 @@
                 xprint(release['body'])
 
                 if args.log_csv or Confirm.ask(f"\n{PROMPT} {prompt_log_csv}"):
                     log_repo_releases(release, repo_name)
         else:
             xprint(response.json())
 
-    # Fetching organization repositories
+    # Fetching organisation repositories
     def org_repos(self):
-        if args.organization and args.limit:
-            organization = args.organization
+        if args.organisation and args.limit:
+            organisation = args.organisation
             limit = args.limit
         else:
-            organization = Prompt.ask(f"{white}@{green}Organi[sz]ation{reset}")
-            limit = Prompt.ask(limit_output.format("organization repositories"))
-        response = requests.get(f"{self.endpoint}/orgs/{organization}/repos?per_page={limit}")
+            organisation = Prompt.ask(f"{white}@{green}Organisation{reset}")
+            limit = Prompt.ask(limit_output.format("organisation repositories"))
+        response = requests.get(f"{self.endpoint}/orgs/{organisation}/repos?per_page={limit}")
         if response.status_code == 404:
-            xprint(f"{NEGATIVE} {org_not_found.format(organization)}")
+            xprint(f"{NEGATIVE} {org_not_found.format(organisation)}")
         elif response.status_code == 200:
             for repository in response.json():
                 repos_tree = Tree("\n" + repository['full_name'])
                 for attr in self.repo_attrs:
                     repos_tree.add(f"{self.repo_attr_dict[attr]}: {repository[attr]}")
                 xprint(repos_tree)
                 
                 if args.log_csv or Prompt.ask(f"{PROMPT} {prompt_log_csv}") == "yes":
-                    log_org_repos(repository, organization)
+                    log_org_repos(repository, organisation)
         else:
             xprint(response.json())
 
-    # organization events
+    # organisation events
     def org_events(self):
-        if args.organization and args.limit:
-            organization = args.organization
+        if args.organisation and args.limit:
+            organisation = args.organisation
             limit = args.limit
         else:
-            organization = Prompt.ask(f"{white}@{green}Organi[sz]ation{reset}")
-            limit = Prompt.ask(limit_output.format("organization events"))
-        response = requests.get(f"{self.endpoint}/orgs/{organization}/events?per_page={limit}")
+            organisation = Prompt.ask(f"{white}@{green}Organisation{reset}")
+            limit = Prompt.ask(limit_output.format("organisation events"))
+        response = requests.get(f"{self.endpoint}/orgs/{organisation}/events?per_page={limit}")
         if response.status_code == 404:
-            xprint(f"{NEGATIVE} {org_not_found.format(organization)}")
+            xprint(f"{NEGATIVE} {org_not_found.format(organisation)}")
         elif response.status_code == 200:
             for event in response.json():
                 events_tree = Tree("\n" + event['id'])
                 events_tree.add(f"Type: {event['type']}")
                 events_tree.add(f"Created at: {event['created_at']}")
                 xprint(events_tree)
                 xprint(event['payload'])
-            # log_org_events(event, organization)
+            # log_org_events(event, organisation)
         else:
             xprint(response.json())
 
-    # organization member
+    # organisation member
     def org_member(self):
-        if args.organization and args.username:
-            organization = args.organization
+        if args.organisation and args.username:
+            organisation = args.organisation
             username = args.username
         else:
-            organization = Prompt.ask(f"{white}@{green}Organi[sz]ation{reset}")
+            organisation = Prompt.ask(f"{white}@{green}Organisation{reset}")
             username = Prompt.ask(f"{white}@{green}Username{reset}")
-        response = requests.get(f"{self.endpoint}/orgs/{organization}/public_members/{username}")
+        response = requests.get(f"{self.endpoint}/orgs/{organisation}/public_members/{username}")
         if response.status_code == 204:
-            xprint(f"{POSITIVE} User ({username}) is a public member of the organization -> ({organization})")
+            xprint(f"{POSITIVE} User ({username}) is a public member of the organisation -> ({organisation})")
         else:
             xprint(f"{NEGATIVE} {response.json()['message']}")
 
     # Fetching user repositories
     def user_repos(self):
         if args.username and args.limit:
             username = args.username
@@ -875,36 +857,36 @@
                 xprint(gists_tree)
                 
                 if args.log_csv or Confirm.ask(f"\n{PROMPT} {prompt_log_csv}"):
                     log_user_gists(gist)
         else:
             xprint(response.json())
 
-    # Fetching a list of organizations that a user owns or belongs to
+    # Fetching a list of organisations that a user owns or belongs to
     def user_orgs(self):
         if args.username and args.limit:
             username = args.username
             limit = args.limit
         else:
             username = Prompt.ask(f"{white}@{green}Username{reset}")
-            limit = Prompt.ask(limit_output.format("user organizations"))
+            limit = Prompt.ask(limit_output.format("user organisations"))
         response = requests.get(f"{self.endpoint}/users/{username}/orgs?per_page={limit}")
         if not response.json():
-            xprint(f"{NEGATIVE} User ({username}) does not (belong to/own) any organizations.")
+            xprint(f"{NEGATIVE} User ({username}) does not (belong to/own) any organisations.")
         elif response.status_code == 404:
             xprint(f"{NEGATIVE} {user_not_found.format(username)}")
         elif response.status_code == 200:
-            for organization in response.json():
-                org_tree = Tree("\n" + organization['login'])
+            for organisation in response.json():
+                org_tree = Tree("\n" + organisation['login'])
                 for attr in self.user_orgs_attrs:
-                    org_tree.add(f"{self.user_orgs_attr_dict[attr]}: {organization[attr]}")
+                    org_tree.add(f"{self.user_orgs_attr_dict[attr]}: {organisation[attr]}")
                 xprint(org_tree)
                 
                 if args.log_csv or Confirm.ask(f"\n{PROMPT} {prompt_log_csv}"):
-                    log_user_orgs(organization, username)
+                    log_user_orgs(organisation, username)
         else:
             xprint(response.json())
 
     # Fetching a users events 
     def user_events(self):
         if args.username and args.limit:
             username = args.username
```

