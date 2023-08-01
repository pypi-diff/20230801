# Comparing `tmp/tag-aaron-alphabet-0.0.3.tar.gz` & `tmp/tag-aaron-alphabet-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tag-aaron-alphabet-0.0.3.tar", last modified: Mon Mar 27 08:57:09 2023, max compression
+gzip compressed data, was "tag-aaron-alphabet-0.0.6.tar", last modified: Tue Aug  1 12:05:18 2023, max compression
```

## Comparing `tag-aaron-alphabet-0.0.3.tar` & `tag-aaron-alphabet-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,16 @@
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-27 08:57:09.781309 tag-aaron-alphabet-0.0.3/
--rw-rw-r--   0 lk        (1002) lk        (1002)      261 2023-03-27 08:57:09.781309 tag-aaron-alphabet-0.0.3/PKG-INFO
--rwxrwxrwx   0 lk        (1002) lk        (1002)      502 2023-03-27 08:39:32.000000 tag-aaron-alphabet-0.0.3/pyproject.toml
--rw-rwxr--   0 lk        (1002) lk        (1002)       38 2023-03-27 08:57:09.781309 tag-aaron-alphabet-0.0.3/setup.cfg
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-27 08:57:09.781309 tag-aaron-alphabet-0.0.3/src/
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-27 08:57:09.781309 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet/
--rw-rw-r--   0 lk        (1002) lk        (1002)     3141 2023-03-27 08:34:49.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet/TaggedFile.py
--rwxrwxrwx   0 lk        (1002) lk        (1002)      880 2023-03-27 07:59:47.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet/__init__.py
--rw-rw-r--   0 lk        (1002) lk        (1002)       74 2023-03-27 00:19:25.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet/__main__.py
--rw-rw-r--   0 lk        (1002) lk        (1002)      454 2023-03-27 00:30:52.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet/boolean.py
--rw-rw-r--   0 lk        (1002) lk        (1002)      137 2023-03-27 07:45:31.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet/iterable.py
--rw-rw-r--   0 lk        (1002) lk        (1002)      419 2023-03-27 07:47:10.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet/path.py
--rw-rw-r--   0 lk        (1002) lk        (1002)     3148 2023-03-27 08:35:02.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet/tagging.py
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-27 08:57:09.781309 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet.egg-info/
--rw-rw-r--   0 lk        (1002) lk        (1002)      261 2023-03-27 08:57:09.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet.egg-info/PKG-INFO
--rw-rw-r--   0 lk        (1002) lk        (1002)      543 2023-03-27 08:57:09.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet.egg-info/SOURCES.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)        1 2023-03-27 08:57:09.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet.egg-info/dependency_links.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)       42 2023-03-27 08:57:09.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet.egg-info/entry_points.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)       15 2023-03-27 08:57:09.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet.egg-info/requires.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)       19 2023-03-27 08:57:09.000000 tag-aaron-alphabet-0.0.3/src/tag_aaron_alphabet.egg-info/top_level.txt
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 12:05:18.047014 tag-aaron-alphabet-0.0.6/
+-rwxrwxrwx   0 jo        (1000) jo        (1000)     1065 2023-08-01 11:48:10.000000 tag-aaron-alphabet-0.0.6/LICENSE
+-rw-rw-r--   0 jo        (1000) jo        (1000)     1418 2023-08-01 12:05:18.047014 tag-aaron-alphabet-0.0.6/PKG-INFO
+-rwxrwxrwx   0 jo        (1000) jo        (1000)      506 2023-08-01 12:04:17.000000 tag-aaron-alphabet-0.0.6/pyproject.toml
+-rw-rwxr--   0 jo        (1000) jo        (1000)       38 2023-08-01 12:05:18.047014 tag-aaron-alphabet-0.0.6/setup.cfg
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 12:05:18.043014 tag-aaron-alphabet-0.0.6/src/
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 12:05:18.047014 tag-aaron-alphabet-0.0.6/src/tag_aaron_alphabet/
+-rwxrwxrwx   0 jo        (1000) jo        (1000)    11594 2023-08-01 12:05:12.000000 tag-aaron-alphabet-0.0.6/src/tag_aaron_alphabet/__init__.py
+-rw-rw-r--   0 jo        (1000) jo        (1000)       75 2023-08-01 12:05:12.000000 tag-aaron-alphabet-0.0.6/src/tag_aaron_alphabet/__main__.py
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 12:05:18.047014 tag-aaron-alphabet-0.0.6/src/tag_aaron_alphabet.egg-info/
+-rw-rw-r--   0 jo        (1000) jo        (1000)     1418 2023-08-01 12:05:18.000000 tag-aaron-alphabet-0.0.6/src/tag_aaron_alphabet.egg-info/PKG-INFO
+-rw-rw-r--   0 jo        (1000) jo        (1000)      380 2023-08-01 12:05:18.000000 tag-aaron-alphabet-0.0.6/src/tag_aaron_alphabet.egg-info/SOURCES.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)        1 2023-08-01 12:05:18.000000 tag-aaron-alphabet-0.0.6/src/tag_aaron_alphabet.egg-info/dependency_links.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)       42 2023-08-01 12:05:18.000000 tag-aaron-alphabet-0.0.6/src/tag_aaron_alphabet.egg-info/entry_points.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)       15 2023-08-01 12:05:18.000000 tag-aaron-alphabet-0.0.6/src/tag_aaron_alphabet.egg-info/requires.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)       19 2023-08-01 12:05:18.000000 tag-aaron-alphabet-0.0.6/src/tag_aaron_alphabet.egg-info/top_level.txt
```

