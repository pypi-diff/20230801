# Comparing `tmp/bite_parser-0.2.2.tar.gz` & `tmp/bite_parser-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bite_parser-0.2.2.tar", max compression
+gzip compressed data, was "bite_parser-0.2.3.tar", max compression
```

## Comparing `bite_parser-0.2.2.tar` & `bite_parser-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1068 2023-02-09 19:58:23.625484 bite_parser-0.2.2/LICENSE
--rw-r--r--   0        0        0     2413 2023-02-09 19:58:23.625484 bite_parser-0.2.2/README.rst
--rw-r--r--   0        0        0       82 2023-02-09 19:58:23.625484 bite_parser-0.2.2/bite/__init__.py
--rw-r--r--   0        0        0     4075 2023-02-09 19:58:23.625484 bite_parser-0.2.2/bite/io.py
--rw-r--r--   0        0        0     3863 2023-02-09 19:58:23.625484 bite_parser-0.2.2/bite/parse_functions.py
--rw-r--r--   0        0        0    29026 2023-02-09 19:58:23.625484 bite_parser-0.2.2/bite/parsers.py
--rw-r--r--   0        0        0       27 2023-02-09 19:58:23.625484 bite_parser-0.2.2/bite/tests/__init__.py
--rw-r--r--   0        0        0     1486 2023-02-09 19:58:23.625484 bite_parser-0.2.2/bite/tests/mock_reader.py
--rw-r--r--   0        0        0     3869 2023-02-09 19:58:23.625484 bite_parser-0.2.2/bite/tests/test_io.py
--rw-r--r--   0        0        0     1101 2023-02-09 19:58:23.625484 bite_parser-0.2.2/bite/tests/test_parse_functions.py
--rw-r--r--   0        0        0    17091 2023-02-09 19:58:23.625484 bite_parser-0.2.2/bite/tests/test_parsers.py
--rw-r--r--   0        0        0     1689 2023-02-09 19:58:23.625484 bite_parser-0.2.2/bite/tests/test_transformers.py
--rw-r--r--   0        0        0     6575 2023-02-09 19:58:23.625484 bite_parser-0.2.2/bite/transformers.py
--rwxr-xr-x   0        0        0     1639 2023-02-09 19:58:23.625484 bite_parser-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3096 1970-01-01 00:00:00.000000 bite_parser-0.2.2/setup.py
--rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 bite_parser-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-01 18:13:48.517363 bite_parser-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2413 2023-08-01 18:13:48.517363 bite_parser-0.2.3/README.rst
+-rw-r--r--   0        0        0       82 2023-08-01 18:13:48.517363 bite_parser-0.2.3/bite/__init__.py
+-rw-r--r--   0        0        0     4045 2023-08-01 18:13:48.517363 bite_parser-0.2.3/bite/io.py
+-rw-r--r--   0        0        0     3863 2023-08-01 18:13:48.517363 bite_parser-0.2.3/bite/parse_functions.py
+-rw-r--r--   0        0        0    29000 2023-08-01 18:13:48.517363 bite_parser-0.2.3/bite/parsers.py
+-rw-r--r--   0        0        0       27 2023-08-01 18:13:48.517363 bite_parser-0.2.3/bite/tests/__init__.py
+-rw-r--r--   0        0        0     1486 2023-08-01 18:13:48.517363 bite_parser-0.2.3/bite/tests/mock_reader.py
+-rw-r--r--   0        0        0     3869 2023-08-01 18:13:48.517363 bite_parser-0.2.3/bite/tests/test_io.py
+-rw-r--r--   0        0        0     1101 2023-08-01 18:13:48.517363 bite_parser-0.2.3/bite/tests/test_parse_functions.py
+-rw-r--r--   0        0        0    17091 2023-08-01 18:13:48.517363 bite_parser-0.2.3/bite/tests/test_parsers.py
+-rw-r--r--   0        0        0     1689 2023-08-01 18:13:48.517363 bite_parser-0.2.3/bite/tests/test_transformers.py
+-rw-r--r--   0        0        0     6575 2023-08-01 18:13:48.517363 bite_parser-0.2.3/bite/transformers.py
+-rwxr-xr-x   0        0        0     1609 2023-08-01 18:13:48.521364 bite_parser-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3477 1970-01-01 00:00:00.000000 bite_parser-0.2.3/PKG-INFO
```

### Comparing `bite_parser-0.2.2/LICENSE` & `bite_parser-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bite_parser-0.2.2/README.rst` & `bite_parser-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `bite_parser-0.2.2/bite/io.py` & `bite_parser-0.2.3/bite/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from asyncio import IncompleteReadError, StreamReader
-from typing import Union
-
-from typing_extensions import Protocol
+from typing import Protocol, Union
 
 
 def _copy_doc(source):
     def decorate(target):
         target.__doc__ = source.__doc__
         return target
```

### Comparing `bite_parser-0.2.2/bite/parse_functions.py` & `bite_parser-0.2.3/bite/parse_functions.py`

 * *Files identical despite different names*

### Comparing `bite_parser-0.2.2/bite/parsers.py` & `bite_parser-0.2.3/bite/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 from typing import (
     Any,
     Callable,
     Generic,
     Iterable,
     NoReturn,
     Optional,
+    Protocol,
     Tuple,
     TypeVar,
     Union,
 )
 
-from typing_extensions import Protocol
-
 from bite.io import ParserBuffer
 
 T = TypeVar("T", covariant=True)
 V = TypeVar("V", covariant=True)
 
 
 class ParsedNode(Protocol[T, V]):
```

### Comparing `bite_parser-0.2.2/bite/tests/mock_reader.py` & `bite_parser-0.2.3/bite/tests/mock_reader.py`

 * *Files identical despite different names*

### Comparing `bite_parser-0.2.2/bite/tests/test_io.py` & `bite_parser-0.2.3/bite/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `bite_parser-0.2.2/bite/tests/test_parse_functions.py` & `bite_parser-0.2.3/bite/tests/test_parse_functions.py`

 * *Files identical despite different names*

### Comparing `bite_parser-0.2.2/bite/tests/test_parsers.py` & `bite_parser-0.2.3/bite/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `bite_parser-0.2.2/bite/tests/test_transformers.py` & `bite_parser-0.2.3/bite/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `bite_parser-0.2.2/bite/transformers.py` & `bite_parser-0.2.3/bite/transformers.py`

 * *Files identical despite different names*

### Comparing `bite_parser-0.2.2/pyproject.toml` & `bite_parser-0.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,31 +18,30 @@
 license = "MIT"
 name = "bite-parser"
 packages = [
   {include = "bite"},
 ]
 readme = "README.rst"
 repository = "https://github.com/jgosmann/bite-parser/"
-version = "0.2.2"
+version = "0.2.3"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-Sphinx = "^5.3.0"
-black = "^22.12.0"
+Sphinx = "^6.0.0"
+black = "^23.7.0"
 darglint = "^1.8.1"
 isort = "^5.11.4"
-mypy = "^0.991"
+mypy = "^1.4.1"
 pylint = "^2.15.10"
 pytest = "^7.2.0"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = "^0.21.1"
 pytest-cov = "^4.0.0"
 sphinx-rtd-theme = "^1.1.1"
-typing-extensions = "^4.0.1"
 
 [tool.isort]
 force_grid_wrap = 0
 include_trailing_comma = true
 line_length = 88
 multi_line_output = 3
 skip = [
```

### Comparing `bite_parser-0.2.2/setup.py` & `bite_parser-0.2.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,87 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: bite-parser
+Version: 0.2.3
+Summary: Asynchronous parser taking incremental bites out of your byte input stream.
+Home-page: https://github.com/jgosmann/bite-parser/
+License: MIT
+Keywords: asyncio,parser,PEG,incremental,parser expression grammar
+Author: Jan Gosmann
+Author-email: jan@hyper-world.de
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Compilers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Repository, https://github.com/jgosmann/bite-parser/
+Description-Content-Type: text/x-rst
 
-packages = \
-['bite', 'bite.tests']
+.. image:: https://github.com/jgosmann/bite-parser/actions/workflows/ci.yml/badge.svg
+  :target: https://github.com/jgosmann/bite-parser/actions/workflows/ci.yml
+  :alt: CI and release pipeline
+.. image:: https://codecov.io/gh/jgosmann/bite-parser/branch/main/graph/badge.svg?token=O4M05YWNQK
+  :target: https://codecov.io/gh/jgosmann/bite-parser
+  :alt: Codecov coverage
+.. image:: https://img.shields.io/pypi/v/bite-parser
+  :target: https://pypi.org/project/bite-parser/
+  :alt: PyPI
+.. image:: https://img.shields.io/pypi/pyversions/bite-parser
+  :target: https://pypi.org/project/bite-parser/
+  :alt: PyPI - Python Version
+.. image:: https://img.shields.io/pypi/l/bite-parser
+  :target: https://pypi.org/project/bite-parser/
+  :alt: PyPI - License
 
-package_data = \
-{'': ['*']}
+Welcome to bite-parser
+======================
 
-setup_kwargs = {
-    'name': 'bite-parser',
-    'version': '0.2.2',
-    'description': 'Asynchronous parser taking incremental bites out of your byte input stream.',
-    'long_description': '.. image:: https://github.com/jgosmann/bite-parser/actions/workflows/ci.yml/badge.svg\n  :target: https://github.com/jgosmann/bite-parser/actions/workflows/ci.yml\n  :alt: CI and release pipeline\n.. image:: https://codecov.io/gh/jgosmann/bite-parser/branch/main/graph/badge.svg?token=O4M05YWNQK\n  :target: https://codecov.io/gh/jgosmann/bite-parser\n  :alt: Codecov coverage\n.. image:: https://img.shields.io/pypi/v/bite-parser\n  :target: https://pypi.org/project/bite-parser/\n  :alt: PyPI\n.. image:: https://img.shields.io/pypi/pyversions/bite-parser\n  :target: https://pypi.org/project/bite-parser/\n  :alt: PyPI - Python Version\n.. image:: https://img.shields.io/pypi/l/bite-parser\n  :target: https://pypi.org/project/bite-parser/\n  :alt: PyPI - License\n\nWelcome to bite-parser\n======================\n\n   Asynchronous parser taking incremental bites out of your byte input stream.\n\nThe bite-parser is a parser combinator library for Python.\nIt is similar to `PyParsing <https://github.com/pyparsing/pyparsing>`_\nin that it allows the construction of grammars for parsing\nfrom simple building blocks in pure Python.\nThis approach is also known as `Parsing Expression Grammar (PEG)\n<https://en.wikipedia.org/wiki/Parsing_expression_grammar>`_.\nWhile PyParsing\n(and many other Python parsing libraries)\nonly support string,\nbite-parser operates on bytes.\nIn addition,\nbite-parser makes use of `asyncio`\nand can asynchronously generate parsed items\nfrom an input stream.\n\nA typical use-case would be the parsing of a network protocol\nlike IMAP.\nIn fact,\nI wrote this library for the IMAP implementation of my\n`dmarc-metrics-exporter <https://github.com/jgosmann/dmarc-metrics-exporter>`_.\n\n.. note::\n   I have implemented the fundamental set of parsers,\n   which should allow constructing most or all grammars\n   recognizable by this type of parser.\n   However, many convenience or higher level parsers are not yet implemented.\n\n   Other areas that still need improvement are:\n\n   * Abilitiy to debug the parsing.\n   * Better error messages.\n   * Performance: Currently, only a basic recursive descent parser is\n     implemented which can exhibit exponential worst case performance.\n     This could be improved by implementing a packrat parser.\n\nImportant links\n---------------\n\n* `Documentation <https://jgosmann.github.io/bite-parser/docs/en/main/>`_\n* `GitHub repository <https://github.com/jgosmann/bite-parser>`_\n',
-    'author': 'Jan Gosmann',
-    'author_email': 'jan@hyper-world.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/jgosmann/bite-parser/',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+   Asynchronous parser taking incremental bites out of your byte input stream.
 
+The bite-parser is a parser combinator library for Python.
+It is similar to `PyParsing <https://github.com/pyparsing/pyparsing>`_
+in that it allows the construction of grammars for parsing
+from simple building blocks in pure Python.
+This approach is also known as `Parsing Expression Grammar (PEG)
+<https://en.wikipedia.org/wiki/Parsing_expression_grammar>`_.
+While PyParsing
+(and many other Python parsing libraries)
+only support string,
+bite-parser operates on bytes.
+In addition,
+bite-parser makes use of `asyncio`
+and can asynchronously generate parsed items
+from an input stream.
+
+A typical use-case would be the parsing of a network protocol
+like IMAP.
+In fact,
+I wrote this library for the IMAP implementation of my
+`dmarc-metrics-exporter <https://github.com/jgosmann/dmarc-metrics-exporter>`_.
+
+.. note::
+   I have implemented the fundamental set of parsers,
+   which should allow constructing most or all grammars
+   recognizable by this type of parser.
+   However, many convenience or higher level parsers are not yet implemented.
+
+   Other areas that still need improvement are:
+
+   * Abilitiy to debug the parsing.
+   * Better error messages.
+   * Performance: Currently, only a basic recursive descent parser is
+     implemented which can exhibit exponential worst case performance.
+     This could be improved by implementing a packrat parser.
+
+Important links
+---------------
+
+* `Documentation <https://jgosmann.github.io/bite-parser/docs/en/main/>`_
+* `GitHub repository <https://github.com/jgosmann/bite-parser>`_
 
-setup(**setup_kwargs)
```

