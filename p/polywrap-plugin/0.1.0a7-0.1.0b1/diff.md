# Comparing `tmp/polywrap_plugin-0.1.0a7.tar.gz` & `tmp/polywrap_plugin-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_plugin-0.1.0a7.tar", max compression
+gzip compressed data, was "polywrap_plugin-0.1.0b1.tar", max compression
```

## Comparing `polywrap_plugin-0.1.0a7.tar` & `polywrap_plugin-0.1.0b1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0        0 2023-02-22 15:57:14.698952 polywrap_plugin-0.1.0a7/README.md
--rw-r--r--   0        0        0       68 2023-02-22 15:57:14.698831 polywrap_plugin-0.1.0a7/polywrap_plugin/__init__.py
--rw-r--r--   0        0        0     1287 2023-03-02 12:38:55.321099 polywrap_plugin-0.1.0a7/polywrap_plugin/module.py
--rw-r--r--   0        0        0      851 2023-03-02 12:38:52.589154 polywrap_plugin-0.1.0a7/polywrap_plugin/package.py
--rw-r--r--   0        0        0     1577 2023-03-02 17:12:07.060382 polywrap_plugin-0.1.0a7/polywrap_plugin/wrapper.py
--rw-r--r--   0        0        0     1061 2023-03-02 20:02:49.412858 polywrap_plugin-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 polywrap_plugin-0.1.0a7/setup.py
--rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 polywrap_plugin-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0      940 2023-08-01 17:46:03.395536 polywrap_plugin-0.1.0b1/README.md
+-rw-r--r--   0        0        0      140 2023-08-01 17:46:03.395536 polywrap_plugin-0.1.0b1/polywrap_plugin/__init__.py
+-rw-r--r--   0        0        0     2964 2023-08-01 17:46:03.395536 polywrap_plugin-0.1.0b1/polywrap_plugin/module.py
+-rw-r--r--   0        0        0     1419 2023-08-01 17:46:03.395536 polywrap_plugin-0.1.0b1/polywrap_plugin/package.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:46:03.395536 polywrap_plugin-0.1.0b1/polywrap_plugin/py.typed
+-rw-r--r--   0        0        0     3178 2023-08-01 17:46:03.395536 polywrap_plugin-0.1.0b1/polywrap_plugin/resolution_context_override_client.py
+-rw-r--r--   0        0        0     3547 2023-08-01 17:46:03.395536 polywrap_plugin-0.1.0b1/polywrap_plugin/wrapper.py
+-rw-r--r--   0        0        0     1127 2023-08-01 17:52:22.893829 polywrap_plugin-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 polywrap_plugin-0.1.0b1/PKG-INFO
```

