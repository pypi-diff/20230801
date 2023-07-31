# Comparing `tmp/SQLAlchemyExample-0.0.1.tar.gz` & `tmp/SQLAlchemyExample-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLAlchemyExample-0.0.1.tar", last modified: Thu Jan 13 01:01:09 2022, max compression
+gzip compressed data, was "SQLAlchemyExample-0.0.2.tar", last modified: Mon Jul 31 22:13:56 2023, max compression
```

## Comparing `SQLAlchemyExample-0.0.1.tar` & `SQLAlchemyExample-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 01:01:09.426201 SQLAlchemyExample-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-01-13 01:00:50.000000 SQLAlchemyExample-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-01-13 01:00:50.000000 SQLAlchemyExample-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4162 2022-01-13 01:01:09.426201 SQLAlchemyExample-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2022-01-13 01:00:50.000000 SQLAlchemyExample-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 01:01:09.426201 SQLAlchemyExample-0.0.1/SQLAlchemyExample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4162 2022-01-13 01:01:09.000000 SQLAlchemyExample-0.0.1/SQLAlchemyExample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-01-13 01:01:09.000000 SQLAlchemyExample-0.0.1/SQLAlchemyExample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-13 01:01:09.000000 SQLAlchemyExample-0.0.1/SQLAlchemyExample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-01-13 01:01:09.000000 SQLAlchemyExample-0.0.1/SQLAlchemyExample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-13 01:01:09.000000 SQLAlchemyExample-0.0.1/SQLAlchemyExample.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-01-13 01:00:50.000000 SQLAlchemyExample-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-01-13 01:00:50.000000 SQLAlchemyExample-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-01-13 01:01:09.426201 SQLAlchemyExample-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 01:01:09.426201 SQLAlchemyExample-0.0.1/sqlalchemyexample/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-01-13 01:00:50.000000 SQLAlchemyExample-0.0.1/sqlalchemyexample/SQLAlchemyExample.ini
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-01-13 01:00:50.000000 SQLAlchemyExample-0.0.1/sqlalchemyexample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11267 2022-01-13 01:00:50.000000 SQLAlchemyExample-0.0.1/sqlalchemyexample/sqlalchemyexample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:13:56.926533 SQLAlchemyExample-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/tests/test_otm_bi_single_table_inherit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/tests/test_otm_uni_single_table_inherit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/tests/test_simple.py
```

### Comparing `SQLAlchemyExample-0.0.1/LICENSE` & `SQLAlchemyExample-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.0.1/PKG-INFO` & `SQLAlchemyExample-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,30 @@
 Metadata-Version: 2.1
 Name: SQLAlchemyExample
-Version: 0.0.1
-Summary: Insert project description here
-Home-page: UNKNOWN
+Version: 0.0.2
+Summary: Exploring SQLAlchemy
 Author: Hendrik du Toit
 Author-email: hendrik@brightedge.co.za
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.0
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/status/SQLAlchemyExample
     :alt: PyPI - Status
 
 .. image:: https://img.shields.io/pypi/wheel/SQLAlchemyExample
     :alt: PyPI - Wheel
 
 .. image:: https://img.shields.io/pypi/pyversions/SQLAlchemyExample
     :alt: PyPI - Python Version
 
-.. image:: https://img.shields.io/github/v/release/hendrikdutoit/SQLAlchemyExample
-    :alt: GitHub release (latest by date)
-
 .. image:: https://img.shields.io/github/license/hendrikdutoit/SQLAlchemyExample
     :alt: License
 
 .. image:: https://img.shields.io/github/issues-raw/hendrikdutoit/SQLAlchemyExample
     :alt: GitHub issues
 
 .. image:: https://img.shields.io/pypi/dm/SQLAlchemyExample
@@ -44,51 +33,76 @@
 .. image:: https://img.shields.io/github/search/hendrikdutoit/SQLAlchemyExample/GitHub
     :alt: GitHub Searches
 
 .. image:: https://img.shields.io/codecov/c/gh/hendrikdutoit/SQLAlchemyExample
     :alt: CodeCov
     :target: https://app.codecov.io/gh/hendrikdutoit/SQLAlchemyExample
 
-.. image:: https://img.shields.io/github/workflow/status/hendrikdutoit/SQLAlchemyExample/Pre-Commit
-    :alt: GitHub Actions - Pre-Commit
-    :target: https://github.com/hendrikdutoit/SQLAlchemyExample/actions/workflows/pre-commit.yaml
-
-.. image:: https://img.shields.io/github/workflow/status/hendrikdutoit/SQLAlchemyExample/CI
-    :alt: GitHub Actions - CI
-    :target: https://github.com/hendrikdutoit/SQLAlchemyExample/actions/workflows/ci.yaml
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yaml?label=pre-commit
+    :alt: GitHub Workflow Status (with event)
+
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yaml?label=ci
+    :alt: GitHub Workflow Status (with event)
 
 .. image:: https://img.shields.io/pypi/v/SQLAlchemyExample
     :alt: PyPi
 
-Example for exploring SQLAlchemy
+====================
+Exploring SQLAlchemy
+====================
+
+    This project provide a sandbox to experiment with SQLAlchemy. This idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress.
+
+    Along the way some principles will be exhibited. The code should be self-explanatory.
+
+    The source code in ``src`` by itself does not do much, it basically only defines the tables and some setup code.  The "examples" are in the the ``pytest's`` since we are experimenting to see howe it works and if it was successfull.
+
+
+    References:
+
+    - https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm
+    - https://docs.sqlalchemy.org/en/14/orm/tutorial.html#building-a-relationship
+    - https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
+
+==================
+Get Up-and-Running
+==================
+
+    1. Set the following environment variables:
+    2. Start Docker.  The ``docker-rebuild.bat`` script will git docker up and running.
+    3. dasd
 
-    This project provide code how to use AQLAlchemy. THis idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress. Along the way some principles will be exhibited. The code should be self-explanatory without as little as possible documentation, else the project is failing. This example illustrate the following: -------------------------------------- 1. Establis a link to a MySQL or SQLite database 2. Create tables 3. Populate the tables 4. Configure a many--to-may relationship 5. Query the tables References ---------- - https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm - https://docs.sqlalchemy.org/en/13/orm/tutorial.html#building-a-relationship - https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
+``pytest``
 
 =======
 Testing
 =======
 
 This project uses ``pytest`` to run tests and also to test docstring examples.
 
 Install the test dependencies.
 
-.. code-block:: bash
+.. code-block::bash
 
     $ pip install -r requirements_test.txt
 
+
+
+
 Run the tests.
 
 .. code-block:: bash
 
     $ pytest tests
     === XXX passed in SSS seconds ===
 
 ==========
 Developing
 ==========
+    The setup and installation is for Windows.  Feel free to add contribute to get it running on Linux as well.
 
 This project uses ``black`` to format code and ``flake8`` for linting. We also support ``pre-commit`` to ensure these have been run. To configure your local environment please install these development dependencies and set up the commit hooks.
 
 .. code-block:: bash
 
     $ pip install black flake8 pre-commit
     $ pre-commit install
@@ -99,17 +113,14 @@
 
 Releases are published automatically when a tag is pushed to GitHub.
 
 .. code-block:: bash
 
     # Set next version number
     export RELEASE = x.x.x
-    
+
     # Create tags
     git commit --allow -empty -m "Release $RELEASE"
     git tag -a $RELEASE -m "Version $RELEASE"
-    
+
     # Push
     git push upstream --tags
-
-
-
```

### Comparing `SQLAlchemyExample-0.0.1/README.rst` & `SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,126 @@
-.. image:: https://img.shields.io/pypi/status/SQLAlchemyExample
-    :alt: PyPI - Status
-
-.. image:: https://img.shields.io/pypi/wheel/SQLAlchemyExample
-    :alt: PyPI - Wheel
-
-.. image:: https://img.shields.io/pypi/pyversions/SQLAlchemyExample
-    :alt: PyPI - Python Version
-
-.. image:: https://img.shields.io/github/v/release/hendrikdutoit/SQLAlchemyExample
-    :alt: GitHub release (latest by date)
-
-.. image:: https://img.shields.io/github/license/hendrikdutoit/SQLAlchemyExample
-    :alt: License
-
-.. image:: https://img.shields.io/github/issues-raw/hendrikdutoit/SQLAlchemyExample
-    :alt: GitHub issues
-
-.. image:: https://img.shields.io/pypi/dm/SQLAlchemyExample
-    :alt: PyPI - Downloads
-
-.. image:: https://img.shields.io/github/search/hendrikdutoit/SQLAlchemyExample/GitHub
-    :alt: GitHub Searches
-
-.. image:: https://img.shields.io/codecov/c/gh/hendrikdutoit/SQLAlchemyExample
-    :alt: CodeCov
-    :target: https://app.codecov.io/gh/hendrikdutoit/SQLAlchemyExample
-
-.. image:: https://img.shields.io/github/workflow/status/hendrikdutoit/SQLAlchemyExample/Pre-Commit
-    :alt: GitHub Actions - Pre-Commit
-    :target: https://github.com/hendrikdutoit/SQLAlchemyExample/actions/workflows/pre-commit.yaml
-
-.. image:: https://img.shields.io/github/workflow/status/hendrikdutoit/SQLAlchemyExample/CI
-    :alt: GitHub Actions - CI
-    :target: https://github.com/hendrikdutoit/SQLAlchemyExample/actions/workflows/ci.yaml
-
-.. image:: https://img.shields.io/pypi/v/SQLAlchemyExample
-    :alt: PyPi
-
-Example for exploring SQLAlchemy
-
-    This project provide code how to use AQLAlchemy. THis idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress. Along the way some principles will be exhibited. The code should be self-explanatory without as little as possible documentation, else the project is failing. This example illustrate the following: -------------------------------------- 1. Establis a link to a MySQL or SQLite database 2. Create tables 3. Populate the tables 4. Configure a many--to-may relationship 5. Query the tables References ---------- - https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm - https://docs.sqlalchemy.org/en/13/orm/tutorial.html#building-a-relationship - https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
-
-=======
-Testing
-=======
-
-This project uses ``pytest`` to run tests and also to test docstring examples.
-
-Install the test dependencies.
-
-.. code-block:: bash
-
-    $ pip install -r requirements_test.txt
-
-Run the tests.
-
-.. code-block:: bash
-
-    $ pytest tests
-    === XXX passed in SSS seconds ===
-
-==========
-Developing
-==========
-
-This project uses ``black`` to format code and ``flake8`` for linting. We also support ``pre-commit`` to ensure these have been run. To configure your local environment please install these development dependencies and set up the commit hooks.
-
-.. code-block:: bash
-
-    $ pip install black flake8 pre-commit
-    $ pre-commit install
-
-=========
-Releasing
-=========
-
-Releases are published automatically when a tag is pushed to GitHub.
-
-.. code-block:: bash
-
-    # Set next version number
-    export RELEASE = x.x.x
-    
-    # Create tags
-    git commit --allow -empty -m "Release $RELEASE"
-    git tag -a $RELEASE -m "Version $RELEASE"
-    
-    # Push
-    git push upstream --tags
-
+Metadata-Version: 2.1
+Name: SQLAlchemyExample
+Version: 0.0.2
+Summary: Exploring SQLAlchemy
+Author: Hendrik du Toit
+Author-email: hendrik@brightedge.co.za
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/status/SQLAlchemyExample
+    :alt: PyPI - Status
+
+.. image:: https://img.shields.io/pypi/wheel/SQLAlchemyExample
+    :alt: PyPI - Wheel
+
+.. image:: https://img.shields.io/pypi/pyversions/SQLAlchemyExample
+    :alt: PyPI - Python Version
+
+.. image:: https://img.shields.io/github/license/hendrikdutoit/SQLAlchemyExample
+    :alt: License
+
+.. image:: https://img.shields.io/github/issues-raw/hendrikdutoit/SQLAlchemyExample
+    :alt: GitHub issues
+
+.. image:: https://img.shields.io/pypi/dm/SQLAlchemyExample
+    :alt: PyPI - Downloads
+
+.. image:: https://img.shields.io/github/search/hendrikdutoit/SQLAlchemyExample/GitHub
+    :alt: GitHub Searches
+
+.. image:: https://img.shields.io/codecov/c/gh/hendrikdutoit/SQLAlchemyExample
+    :alt: CodeCov
+    :target: https://app.codecov.io/gh/hendrikdutoit/SQLAlchemyExample
+
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yaml?label=pre-commit
+    :alt: GitHub Workflow Status (with event)
+
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yaml?label=ci
+    :alt: GitHub Workflow Status (with event)
+
+.. image:: https://img.shields.io/pypi/v/SQLAlchemyExample
+    :alt: PyPi
+
+====================
+Exploring SQLAlchemy
+====================
+
+    This project provide a sandbox to experiment with SQLAlchemy. This idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress.
+
+    Along the way some principles will be exhibited. The code should be self-explanatory.
+
+    The source code in ``src`` by itself does not do much, it basically only defines the tables and some setup code.  The "examples" are in the the ``pytest's`` since we are experimenting to see howe it works and if it was successfull.
+
+
+    References:
+
+    - https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm
+    - https://docs.sqlalchemy.org/en/14/orm/tutorial.html#building-a-relationship
+    - https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
+
+==================
+Get Up-and-Running
+==================
+
+    1. Set the following environment variables:
+    2. Start Docker.  The ``docker-rebuild.bat`` script will git docker up and running.
+    3. dasd
+
+``pytest``
+
+=======
+Testing
+=======
+
+This project uses ``pytest`` to run tests and also to test docstring examples.
+
+Install the test dependencies.
+
+.. code-block::bash
+
+    $ pip install -r requirements_test.txt
+
+
+
+
+Run the tests.
+
+.. code-block:: bash
+
+    $ pytest tests
+    === XXX passed in SSS seconds ===
+
+==========
+Developing
+==========
+    The setup and installation is for Windows.  Feel free to add contribute to get it running on Linux as well.
+
+This project uses ``black`` to format code and ``flake8`` for linting. We also support ``pre-commit`` to ensure these have been run. To configure your local environment please install these development dependencies and set up the commit hooks.
+
+.. code-block:: bash
+
+    $ pip install black flake8 pre-commit
+    $ pre-commit install
+
+=========
+Releasing
+=========
+
+Releases are published automatically when a tag is pushed to GitHub.
+
+.. code-block:: bash
+
+    # Set next version number
+    export RELEASE = x.x.x
+
+    # Create tags
+    git commit --allow -empty -m "Release $RELEASE"
+    git tag -a $RELEASE -m "Version $RELEASE"
+
+    # Push
+    git push upstream --tags
```

