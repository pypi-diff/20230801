# Comparing `tmp/cfinterface-1.5.0.tar.gz` & `tmp/cfinterface-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfinterface-1.5.0.tar", last modified: Mon Jul 31 14:11:13 2023, max compression
+gzip compressed data, was "cfinterface-1.5.1.tar", last modified: Mon Jul 31 19:05:45 2023, max compression
```

## Comparing `cfinterface-1.5.0.tar` & `cfinterface-1.5.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.546782 cfinterface-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 14:09:47.000000 cfinterface-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-31 14:11:13.546782 cfinterface-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-31 14:09:47.000000 cfinterface-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface/adapters/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface/adapters/components/line/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/components/line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/components/line/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/components/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface/adapters/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/reading/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.534781 cfinterface-1.5.0/cfinterface/adapters/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/writing/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.534781 cfinterface-1.5.0/cfinterface/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/datetimefield.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/defaultblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/defaultregister.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/defaultsection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/floatfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/integerfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/literalfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.534781 cfinterface-1.5.0/cfinterface/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/data/blockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/data/registerdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/data/sectiondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.534781 cfinterface-1.5.0/cfinterface/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/files/blockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/files/registerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/files/sectionfile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/cfinterface/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/reading/blockreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/reading/registerreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/reading/sectionreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/cfinterface/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/writing/blockwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/writing/registerwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/writing/sectionwriting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-31 14:11:13.000000 cfinterface-1.5.0/cfinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-31 14:11:13.000000 cfinterface-1.5.0/cfinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:11:13.000000 cfinterface-1.5.0/cfinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 14:11:13.000000 cfinterface-1.5.0/cfinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 14:11:13.000000 cfinterface-1.5.0/cfinterface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:11:13.546782 cfinterface-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-31 14:09:47.000000 cfinterface-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/tests/adapters/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/components/test_blockrepository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/components/test_linerepository.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/components/test_registerrepository.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/components/test_sectionrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/tests/adapters/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/reading/test_readingrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/tests/adapters/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/writing/test_writingrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.542782 cfinterface-1.5.0/tests/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_datetimefield.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_defaultblock.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_defaultregister.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_defaultsection.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_floatfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_integerfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_literalfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.542782 cfinterface-1.5.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/data/test_blockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/data/test_registerdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/data/test_sectiondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.542782 cfinterface-1.5.0/tests/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/files/test_blockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/files/test_registerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/files/test_sectionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.542782 cfinterface-1.5.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.542782 cfinterface-1.5.0/tests/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/reading/test_blockreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/reading/test_registerreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/reading/test_sectionreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.546782 cfinterface-1.5.0/tests/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/writing/test_blockwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/writing/test_registerwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/writing/test_sectionwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.092746 cfinterface-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:04:08.000000 cfinterface-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-31 19:05:45.092746 cfinterface-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-31 19:04:08.000000 cfinterface-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.068746 cfinterface-1.5.1/cfinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.068746 cfinterface-1.5.1/cfinterface/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.068746 cfinterface-1.5.1/cfinterface/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.068746 cfinterface-1.5.1/cfinterface/adapters/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/adapters/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.072746 cfinterface-1.5.1/cfinterface/adapters/components/line/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/adapters/components/line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/adapters/components/line/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/adapters/components/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.072746 cfinterface-1.5.1/cfinterface/adapters/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/adapters/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/adapters/reading/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.072746 cfinterface-1.5.1/cfinterface/adapters/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/adapters/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/adapters/writing/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.076746 cfinterface-1.5.1/cfinterface/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/datetimefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/defaultblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/defaultregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/defaultsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/floatfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/integerfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/literalfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/components/section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.076746 cfinterface-1.5.1/cfinterface/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/data/blockdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/data/registerdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/data/sectiondata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.076746 cfinterface-1.5.1/cfinterface/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/files/blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/files/registerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/files/sectionfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.080746 cfinterface-1.5.1/cfinterface/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/reading/blockreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/reading/registerreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/reading/sectionreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.080746 cfinterface-1.5.1/cfinterface/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/writing/blockwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/writing/registerwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-31 19:04:08.000000 cfinterface-1.5.1/cfinterface/writing/sectionwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.068746 cfinterface-1.5.1/cfinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-31 19:05:44.000000 cfinterface-1.5.1/cfinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-31 19:05:45.000000 cfinterface-1.5.1/cfinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:05:44.000000 cfinterface-1.5.1/cfinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 19:05:44.000000 cfinterface-1.5.1/cfinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 19:05:44.000000 cfinterface-1.5.1/cfinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.080746 cfinterface-1.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:05:45.092746 cfinterface-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-31 19:04:08.000000 cfinterface-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.080746 cfinterface-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.080746 cfinterface-1.5.1/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.084746 cfinterface-1.5.1/tests/adapters/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/adapters/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/adapters/components/test_blockrepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/adapters/components/test_linerepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/adapters/components/test_registerrepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/adapters/components/test_sectionrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.084746 cfinterface-1.5.1/tests/adapters/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/adapters/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/adapters/reading/test_readingrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.084746 cfinterface-1.5.1/tests/adapters/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/adapters/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/adapters/writing/test_writingrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.088746 cfinterface-1.5.1/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/test_datetimefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/test_defaultblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/test_defaultregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/test_defaultsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/test_floatfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/test_integerfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/test_literalfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/components/test_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.088746 cfinterface-1.5.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/data/test_blockdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/data/test_registerdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/data/test_sectiondata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.088746 cfinterface-1.5.1/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/files/test_blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/files/test_registerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/files/test_sectionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.088746 cfinterface-1.5.1/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.088746 cfinterface-1.5.1/tests/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/reading/test_blockreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/reading/test_registerreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/reading/test_sectionreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:05:45.092746 cfinterface-1.5.1/tests/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/writing/test_blockwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/writing/test_registerwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-31 19:04:08.000000 cfinterface-1.5.1/tests/writing/test_sectionwriting.py
```

### Comparing `cfinterface-1.5.0/LICENSE.md` & `cfinterface-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/PKG-INFO` & `cfinterface-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfinterface
-Version: 1.5.0
+Version: 1.5.1
 Summary: Interface for handling custom formatted files
 Home-page: https://github.com/rjmalves/cfi
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfinterface-1.5.0/README.md` & `cfinterface-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/adapters/components/line/repository.py` & `cfinterface-1.5.1/cfinterface/adapters/components/line/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/adapters/components/repository.py` & `cfinterface-1.5.1/cfinterface/adapters/components/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/adapters/reading/repository.py` & `cfinterface-1.5.1/cfinterface/adapters/reading/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/adapters/writing/repository.py` & `cfinterface-1.5.1/cfinterface/adapters/writing/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/components/block.py` & `cfinterface-1.5.1/cfinterface/components/block.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/components/datetimefield.py` & `cfinterface-1.5.1/cfinterface/components/datetimefield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/components/defaultblock.py` & `cfinterface-1.5.1/cfinterface/components/defaultblock.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/components/defaultregister.py` & `cfinterface-1.5.1/cfinterface/components/defaultregister.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/components/defaultsection.py` & `cfinterface-1.5.1/cfinterface/components/defaultsection.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/components/field.py` & `cfinterface-1.5.1/cfinterface/components/field.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/components/floatfield.py` & `cfinterface-1.5.1/cfinterface/components/floatfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/components/integerfield.py` & `cfinterface-1.5.1/cfinterface/components/integerfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/components/line.py` & `cfinterface-1.5.1/cfinterface/components/line.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/components/literalfield.py` & `cfinterface-1.5.1/cfinterface/components/literalfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/components/register.py` & `cfinterface-1.5.1/cfinterface/components/register.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/components/section.py` & `cfinterface-1.5.1/cfinterface/components/section.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/data/blockdata.py` & `cfinterface-1.5.1/cfinterface/data/blockdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     def __init__(self, root: Block) -> None:
         self.__root = root
         self.__head = root
 
     def __iter__(self):
         current = self.__root
         while current:
-            print(current.data)
             yield current
             current = current.next
 
     def __len__(self) -> int:
         count = 0
         for _ in self:
             count += 1
```

### Comparing `cfinterface-1.5.0/cfinterface/data/registerdata.py` & `cfinterface-1.5.1/cfinterface/data/registerdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/data/sectiondata.py` & `cfinterface-1.5.1/cfinterface/data/sectiondata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/files/blockfile.py` & `cfinterface-1.5.1/cfinterface/files/blockfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/files/registerfile.py` & `cfinterface-1.5.1/cfinterface/files/registerfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/files/sectionfile.py` & `cfinterface-1.5.1/cfinterface/files/sectionfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/reading/blockreading.py` & `cfinterface-1.5.1/cfinterface/reading/blockreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/reading/registerreading.py` & `cfinterface-1.5.1/cfinterface/reading/registerreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/reading/sectionreading.py` & `cfinterface-1.5.1/cfinterface/reading/sectionreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/writing/blockwriting.py` & `cfinterface-1.5.1/cfinterface/writing/blockwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/writing/registerwriting.py` & `cfinterface-1.5.1/cfinterface/writing/registerwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface/writing/sectionwriting.py` & `cfinterface-1.5.1/cfinterface/writing/sectionwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/cfinterface.egg-info/PKG-INFO` & `cfinterface-1.5.1/cfinterface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfinterface
-Version: 1.5.0
+Version: 1.5.1
 Summary: Interface for handling custom formatted files
 Home-page: https://github.com/rjmalves/cfi
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfinterface-1.5.0/cfinterface.egg-info/SOURCES.txt` & `cfinterface-1.5.1/cfinterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/setup.py` & `cfinterface-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/adapters/components/test_linerepository.py` & `cfinterface-1.5.1/tests/adapters/components/test_linerepository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/components/test_block.py` & `cfinterface-1.5.1/tests/components/test_block.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/components/test_datetimefield.py` & `cfinterface-1.5.1/tests/components/test_datetimefield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/components/test_defaultblock.py` & `cfinterface-1.5.1/tests/components/test_defaultblock.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/components/test_defaultregister.py` & `cfinterface-1.5.1/tests/components/test_defaultregister.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/components/test_defaultsection.py` & `cfinterface-1.5.1/tests/components/test_defaultsection.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/components/test_floatfield.py` & `cfinterface-1.5.1/tests/components/test_floatfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/components/test_integerfield.py` & `cfinterface-1.5.1/tests/components/test_integerfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/components/test_line.py` & `cfinterface-1.5.1/tests/components/test_line.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/components/test_literalfield.py` & `cfinterface-1.5.1/tests/components/test_literalfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/components/test_register.py` & `cfinterface-1.5.1/tests/components/test_register.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/components/test_section.py` & `cfinterface-1.5.1/tests/components/test_section.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/data/test_blockdata.py` & `cfinterface-1.5.1/tests/data/test_blockdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/data/test_registerdata.py` & `cfinterface-1.5.1/tests/data/test_registerdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/data/test_sectiondata.py` & `cfinterface-1.5.1/tests/data/test_sectiondata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/files/test_blockfile.py` & `cfinterface-1.5.1/tests/files/test_blockfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/files/test_registerfile.py` & `cfinterface-1.5.1/tests/files/test_registerfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/files/test_sectionfile.py` & `cfinterface-1.5.1/tests/files/test_sectionfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/mocks/mock_open.py` & `cfinterface-1.5.1/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/reading/test_blockreading.py` & `cfinterface-1.5.1/tests/reading/test_blockreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/reading/test_registerreading.py` & `cfinterface-1.5.1/tests/reading/test_registerreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/reading/test_sectionreading.py` & `cfinterface-1.5.1/tests/reading/test_sectionreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/writing/test_blockwriting.py` & `cfinterface-1.5.1/tests/writing/test_blockwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/writing/test_registerwriting.py` & `cfinterface-1.5.1/tests/writing/test_registerwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.0/tests/writing/test_sectionwriting.py` & `cfinterface-1.5.1/tests/writing/test_sectionwriting.py`

 * *Files identical despite different names*

