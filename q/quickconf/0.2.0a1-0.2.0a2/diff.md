# Comparing `tmp/quickconf-0.2.0a1.tar.gz` & `tmp/quickconf-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickconf-0.2.0a1.tar", last modified: Sun Jul 30 18:52:32 2023, max compression
+gzip compressed data, was "quickconf-0.2.0a2.tar", last modified: Tue Aug  1 08:32:01 2023, max compression
```

## Comparing `quickconf-0.2.0a1.tar` & `quickconf-0.2.0a2.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:52:32.831157 quickconf-0.2.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:52:32.827157 quickconf-0.2.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:52:32.827157 quickconf-0.2.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-30 18:52:21.000000 quickconf-0.2.0a1/.github/workflows/build-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-30 18:52:21.000000 quickconf-0.2.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 18:52:25.000000 quickconf-0.2.0a1/.version
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-30 18:52:21.000000 quickconf-0.2.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-30 18:52:32.831157 quickconf-0.2.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-30 18:52:21.000000 quickconf-0.2.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:52:32.831157 quickconf-0.2.0a1/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-30 18:52:21.000000 quickconf-0.2.0a1/demo/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-30 18:52:21.000000 quickconf-0.2.0a1/demo/settings.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-30 18:52:21.000000 quickconf-0.2.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:52:32.831157 quickconf-0.2.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:52:32.827157 quickconf-0.2.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:52:32.831157 quickconf-0.2.0a1/src/quickconf/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 18:52:21.000000 quickconf-0.2.0a1/src/quickconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 18:52:25.000000 quickconf-0.2.0a1/src/quickconf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-07-30 18:52:21.000000 quickconf-0.2.0a1/src/quickconf/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:52:32.831157 quickconf-0.2.0a1/src/quickconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-30 18:52:32.000000 quickconf-0.2.0a1/src/quickconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-30 18:52:32.000000 quickconf-0.2.0a1/src/quickconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:52:32.000000 quickconf-0.2.0a1/src/quickconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-30 18:52:32.000000 quickconf-0.2.0a1/src/quickconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 18:52:32.000000 quickconf-0.2.0a1/src/quickconf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:52:32.831157 quickconf-0.2.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-30 18:52:21.000000 quickconf-0.2.0a1/tests/test_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.470264 quickconf-0.2.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 08:31:46.000000 quickconf-0.2.0a2/.version
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/demo/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/demo/settings.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/demo/settings_updated.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/demo/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.470264 quickconf-0.2.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/src/quickconf/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/src/quickconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 08:31:46.000000 quickconf-0.2.0a2/src/quickconf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/src/quickconf/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/src/quickconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 08:32:01.000000 quickconf-0.2.0a2/src/quickconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-01 08:32:01.000000 quickconf-0.2.0a2/src/quickconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:32:01.000000 quickconf-0.2.0a2/src/quickconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 08:32:01.000000 quickconf-0.2.0a2/src/quickconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 08:32:01.000000 quickconf-0.2.0a2/src/quickconf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/tests/test_conf.py
```

### Comparing `quickconf-0.2.0a1/.github/workflows/build-publish.yml` & `quickconf-0.2.0a2/.github/workflows/release.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,72 @@
-name: Build and Publish Python Package
+name: Release
 
 on:
-  release:
-    types: [published]
+  push:
+    tags:
+      - v*.*.*
 
 permissions:
   contents: read
 
 jobs:
-  prepare:
-    name: Get release version
+  # TODO: check and require that tests have completed without issue before releasing?
+
+  release:
+    name: Release
     runs-on: ubuntu-latest
-    outputs:
-      version: ${{ steps.get-version.outputs.version }}
-      publish: ${{ steps.get-version.outputs.publish }}
+    environment: release
+    permissions:
+      id-token: write
+      contents: write
+
     steps:
-      - name: Get version from tag
-        id: get-version
+      - name: Check version
+        id: check-version
         run: |
           pattern="^refs\/tags\/v([0-9]+\.[0-9]+\.[0-9]+(-(a|alpha|b|beta|dev)[0-9]+)?)$"
-          if [[ "${{ github.ref }}" =~ $pattern ]]
-          then
-            ver="${BASH_REMATCH[1]}"
-            pub="true"
-          else
-            ver="0.0.1dev0"
-            pub="false"
-          fi
-          echo "version=$ver" >> "$GITHUB_OUTPUT"
-          echo "publish=$pub" >> "$GITHUB_OUTPUT"
-
-  build:
-    name: Build package
-    needs: prepare
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
+          [[ "${{ github.ref }}" =~ $pattern ]]
+          echo ::set-output name=version::${BASH_REMATCH[1]}
+          [ -z "${BASH_REMATCH[2]}" ] || echo ::set-output name=prerelease::true
+
+      - name: Checkout repo
+        uses: actions/checkout@v3
+
+      - name: Write version files
+        env:
+          VERSION: ${{ steps.check-version.outputs.version }}
+        run: |
+          "$env:VERSION" | Out-File -FilePath ".version"
+          "__version__ = version = '$env:VERSION'" | Out-File -FilePath "src/quickconf/_version.py"
+        shell: pwsh
+
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.11
+
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install setuptools build wheel
-      - name: Write version files
-        env:
-          VERSION: ${{ needs.prepare.outputs.version }}
-        run: |
-          "$env:VERSION" | Out-File -FilePath ".version"
-          "__version__ = version = '$env:VERSION'" | Out-File -FilePath "src/quickconf/_version.py"
-        shell: pwsh
+
       - name: Build package
         run: |
           python -m build
+
       - name: Upload build artifacts
         uses: actions/upload-artifact@v3
         with:
           name: dist
           path: dist/
 
-  publish:
-    name: Upload release to PyPI
-    runs-on: ubuntu-latest
-    needs: [prepare, build]
-    if: needs.prepare.outputs.publish == 'true'
-    environment: release
-    permissions:
-      id-token: write
-    steps:
-      - name: Download build artifacts
-        uses: actions/download-artifact@v3
+      - name: Create release
+        uses: ncipollo/release-action@v1
         with:
-          name: dist
-          path: dist/
-      - name: Publish package distributions to PyPI
+          artifacts: "dist/*"
+          draft: false
+          allowUpdates: true
+          generateReleaseNotes: true
+          prerelease: steps.check-version.outputs.prerelease == 'true'
+
+      - name: Publish to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `quickconf-0.2.0a1/.gitignore` & `quickconf-0.2.0a2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 cover/
+tests/.coverage
+tests/.results
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
@@ -157,8 +159,8 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # These files are automatically generated in the Github workflow, and should not be tracked
 _version.py
-.version
+.version
```

### Comparing `quickconf-0.2.0a1/LICENSE` & `quickconf-0.2.0a2/LICENSE`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 mortencombat
+Copyright (c) 2023 Kenneth Trelborg Vestergaard
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `quickconf-0.2.0a1/demo/example.py` & `quickconf-0.2.0a2/demo/example.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,37 +23,44 @@
     layout_resolution: int = settings["layout.resolution"]
     layout_point_size: float = settings["layout.point.size"]
     page_dpi: int = settings["page.dpi"]
     page_margins: int = settings["page.margins"]
 
 
 data = Path("demo/settings.toml")
+data_out = Path("demo/settings_updated.toml")
 
 # Settings are defined explicitly by subclassing Configuration.
 # The settings are available as attributes (properties), includes autocomplete and typing.
 # Settings are only available as the explicitly defined class attributes of ExampleConfig,
-# fx. conf_subcl.layout_point_size
+# fx. config.layout_point_size
 print("\nEXAMPLE 1: subclassed Configuration with explicit attributes")
 config = ExampleConfig(
     data, defined_only=True, access=Configuration.SettingsAccess.ATTR_EXPLICIT
 )
 print(f"{config.layout_point_size=}")
+config.layout_point_size = 0.2
 for setting, value in config.settings.items():
     print(f"{setting} = {value}")
+config.save(data_out)
 
 # Settings are inferred from the configuration file, eg. all settings from the file are read.
-# Settings are only available using eg. conf_impl.layout.point.size
+# Settings are only available using eg. config.layout.point.size
 print("\nEXAMPLE 2: Configuration with all settings in .toml file and attribute access")
 config = Configuration(data, access=Configuration.SettingsAccess.ATTR)
 print(f"{config.layout.point.size=}")
+config.layout.point.size = 0.3
 for setting, value in config.settings.items():
     print(f"{setting} = {value}")
+config.save(data_out)
 
 # Settings are defined in options. Any settings in data that are not explicitly defined are
-# ignored. Settings are only available using eg. conf_expl["layout.point.size"]
+# ignored. Settings are only available using eg. config["layout.point.size"]
 print("\nEXAMPLE 3: Configuration with only defined settings and item access [...]")
 config = Configuration(
     data, settings=settings, defined_only=True, access=Configuration.SettingsAccess.ITEM
 )
 print(f"{config['layout.point.size']=}")
+config["layout.point.size"] = 0.4
 for setting, value in config.settings.items():
     print(f"{setting} = {value}")
+config.save(data_out)
```

### Comparing `quickconf-0.2.0a1/pyproject.toml` & `quickconf-0.2.0a2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -16,22 +16,23 @@
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "attrs",
+    'attrs',
+    'tomli>=2.0;python_version<"3.11"',
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 save = [ 'tomlkit>=0.12.1,<1.0' ]
 build = [ 'setuptools', 'build', 'wheel', 'twine' ]
-test = [ 'pytest' ]
+test = [ 'pre-commit', 'pytest', 'pytest-cov' ]
 
 [tool.setuptools.dynamic]
 version = {file = [".version"]}
 
 [project.urls]
 homepage = "https://github.com/mortencombat/quickconf"
-repository = "https://github.com/mortencombat/quickconf"
+repository = "https://github.com/mortencombat/quickconf"
```

### Comparing `quickconf-0.2.0a1/src/quickconf/core.py` & `quickconf-0.2.0a2/src/quickconf/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import re
+from collections.abc import Iterable
+from datetime import date, datetime, time
 from enum import Flag, auto
 from inspect import getmembers
 from itertools import chain
 from pathlib import Path
-from typing import Any, Generic, Iterable, TypeVar
+from typing import Any, Generic, TypeVar
 
 try:
     import tomlkit as tomllib
+
+    _USE_TOMLKIT = True
 except ModuleNotFoundError:
-    import tomllib
+    _USE_TOMLKIT = False
+    try:
+        import tomllib
+    except ModuleNotFoundError:
+        import tomli as tomllib
 
 T = TypeVar("T")
 
 _key_pattern = re.compile("[A-Za-z0-9_-]+")
 
 
 def parse_key(key: str) -> tuple[str]:
@@ -53,40 +61,51 @@
 
     def _get_generic_type(self) -> None:
         self._type = self.__orig_class__.__args__[0]
 
     def _load(self, config: "Configuration") -> None:
         """Retrieves settings value from configuration"""
 
-        v = config._get_value(self._keys, default=self._default)
+        value = config._get_value(self._keys, default=self._default)
 
         self._get_generic_type()
-        if not isinstance(v, self._type):
+        if not isinstance(value, self._type):
             raise TypeError(
-                f"{self.name} should be {self._type.__name__}, got '{v}' ({type(v).__name__})"
+                f"{self.name} should be {self._type.__name__}, got '{value}' ({type(value).__name__})"
             )
 
         # TODO: Add validation support
 
-        self._value = v
+        self._value = value
         self._loaded = True
 
-    def _dump(self, config: "Configuration") -> None:
-        raise NotImplementedError
+    def _dump(self, config: "Configuration", value: T) -> None:
+        if not self._loaded:
+            self._get_generic_type()
+
+        if not isinstance(value, self._type):
+            raise TypeError(
+                f"{self.name} should be {self._type.__name__}, got '{value}' ({type(value).__name__})"
+            )
+
+        # TODO: Check validation
+
+        config._set_value(self._keys, value)
 
     def __get__(self, instance: "Configuration", owner: "Configuration" = None) -> T:
         if not instance:
             return self
         if not self._loaded:
             self._load(instance)
         return self._value
 
     def __set__(self, instance: "Configuration", value: T) -> None:
-        if not instance or instance._read_only:
+        if not instance or instance.is_readonly:
             raise AttributeError(self.name)
+        self._dump(instance, value)
         self._value = value
 
     def __delete__(self, instance: "Configuration") -> None:
         self._reset()
 
     def __hash__(self) -> int:
         return self._name
@@ -95,35 +114,35 @@
 class Settings:
     def __init__(self, settings: Iterable[Setting] = None):
         self.clear()
         if settings:
             self.extend(settings)
 
     def append(self, setting: Setting) -> bool:
-        if not setting.name in self._settings:
+        if setting.name not in self._settings:
             self._settings[setting.name] = setting
             return True
         else:
             return False
 
     def extend(self, settings: Iterable[Setting]) -> int:
         n = 0
         for setting in settings:
             if self.append(setting):
                 n += 1
         return n
 
     def clear(self) -> None:
-        self._settings = dict()
+        self._settings = {}
 
     def __contains__(self, name: str) -> bool:
         return name in self._settings
 
     def __getitem__(self, name: str) -> Setting:
-        if not name in self._settings:
+        if name not in self._settings:
             raise KeyError(name)
         return self._settings[name]
 
     def __iter__(self):
         return iter(self._settings.values())
 
 
@@ -135,97 +154,145 @@
         ANY = ATTR_EXPLICIT | ATTR | ITEM
 
     class _Proxy:
         def __init__(self, config: "Configuration", name: str):
             self._config = config
             self._name = name
 
+        # NOTE! There could be name clashes with the current implementation, both in Configuration and in _Proxy,
+        #       if a settings key has the same name as a class attribute
+        #       Raise an error if ATTR access is enabled and a setting is defined or loaded that clashes with a class attribute/method.
+
         def __getattr__(self, key: str):
+            if key in ("_config", "_name"):
+                raise AttributeError(key)
+
             setting = f"{self._name}.{key}"
             if setting in self._config._settings:
                 return self._config.settings[setting].__get__(self._config)
             elif (
                 not self._config._defined_only
                 and setting in self._config._settings_flex
             ):
                 return self._config._settings_flex[setting].__get__(self._config)
             if not self._config._has_section(setting):
                 raise AttributeError(setting)
 
             return Configuration._Proxy(self._config, setting)
 
+        def __setattr__(self, key: str, value: str) -> None:
+            if key in ("_config", "_name"):
+                return super().__setattr__(key, value)
+
+            setting = f"{self._name}.{key}"
+            if setting in self._config._settings:
+                return self._config.settings[setting].__set__(self._config, value)
+            elif (
+                not self._config._defined_only
+                and setting in self._config._settings_flex
+            ):
+                return self._config._settings_flex[setting].__set__(self._config, value)
+            raise AttributeError(setting)
+
     def __init__(
         self,
         config: Path | str | dict = None,
         *,
         settings: Settings | Iterable[Setting] = None,
         defined_only: bool = False,
         access: SettingsAccess = SettingsAccess.ANY,
+        allow_changes: bool = True,
     ) -> None:
         """Returns a Configuration instance.
 
         :param config: If a valid path (Path or str), load config from file (toml-format). If a dict, load config from dict. If a str (not filepath), attempt to parse as toml., defaults to None
         :type config: Path | dict[str, object], optional
 
         If config is a filepath, read configuration from that file (toml format).
         If config is a dict, read configuration from dict.
         If none of the above, configuration will use all defaults.
         """
 
         # Misc. config
         self._defined_only = defined_only
         self._access = access
-        self._read_only = True  # Only read-only supported at the moment
+        self._allow_changes = allow_changes
 
         # Assemble options from arg and class attributes.
         self._settings = Settings(settings)
         self._settings_flex = Settings()
         for _, obj in getmembers(type(self)):
             if not isinstance(obj, Setting):
                 continue
             self._settings.append(obj)
+        self.__TYPE_MAP = None
 
         # Load configuration
         self.load(config)
 
+    def __get_base_type(self, cls) -> type:
+        if _USE_TOMLKIT:
+            if not self.__TYPE_MAP:
+                self.__TYPE_MAP = {
+                    tomllib.items.Float: float,
+                    tomllib.items.Integer: int,
+                    tomllib.items.String: str,
+                    tomllib.items.DateTime: datetime,
+                    tomllib.items.Date: date,
+                    tomllib.items.Time: time,
+                    tomllib.items.Bool: bool,
+                }
+            if cls in self.__TYPE_MAP:
+                return self.__TYPE_MAP[cls]
+            raise TypeError(cls)
+        else:
+            return cls
+
     def reset(self) -> None:
         """Resets all settings to their default values."""
         for setting in self._settings:
             del setting
         self._settings_flex.clear()
+        self._data = {}
 
     def load(self, config: Path | str | dict = None) -> None:
         self.reset()
         if config is None:
             return
         if isinstance(config, dict):
             self._load_dict(config)
         else:
             self._load_toml(config)
 
+    def save(self, path: Path | str) -> None:
+        if self.is_readonly:
+            raise OSError("Configuration is read-only")
+        with open(path, "w") as f:
+            f.write(tomllib.dumps(self._data))
+
     def _has_section(self, section: str) -> bool:
         s = section + "."
-        for setting in chain(self._settings, self._settings_flex):
-            if setting.name.startswith(s):
-                return True
-        return False
+        return any(
+            setting.name.startswith(s)
+            for setting in chain(self._settings, self._settings_flex)
+        )
 
     def _load_toml(self, config: Path | str) -> None:
         """Load configuration settings from a path pointing to a toml-file or
         directly from a toml-formatted string."""
         try:
             with open(config, "rb") as f:
                 data = tomllib.load(f)
         except OSError:
             data = tomllib.loads(config)
         return self._load_dict(data)
 
     @staticmethod
     def _get_settings_from_dict(data: dict, section: str = None) -> dict:
-        r = dict()
+        r = {}
         for name, value in data.items():
             s = f"{section}.{name}" if section else name
             if isinstance(value, dict):
                 r.update(Configuration._get_settings_from_dict(data[name], s))
             else:
                 r[s] = value
         return r
@@ -234,52 +301,117 @@
         """Load configuration settings from a dict."""
         self.reset()
         self._data = config
         if not self._defined_only:
             # Add settings to self._settings_flex for each item in self._data,
             # unless it is already defined in self._settings
             for setting, value in self._get_settings_from_dict(config).items():
-                if not setting in self._settings:
-                    self._settings_flex.append(Setting[type(value)](setting))
+                if setting not in self._settings:
+                    self._settings_flex.append(
+                        Setting[self.__get_base_type(type(value))](setting)
+                    )
+
+    @property
+    def is_readonly(self) -> bool:
+        return not _USE_TOMLKIT or not self._allow_changes
 
     @property
     def settings(self) -> dict[str, Any]:
-        r = dict()
+        r = {}
         for s in chain(self._settings, self._settings_flex):
             r[s.name] = s.__get__(self)
         return dict(sorted(r.items()))
 
     def _get_value(self, keys: tuple[str], default: Any = None) -> Any:
         try:
             return self.__get_value(self._data, keys, 0)
         except KeyError as e:
-            if not default is None:
+            if default is not None:
                 return default
             raise e
 
     @staticmethod
     def __get_value(data: dict, keys: tuple[str], level: int) -> Any:
         if not keys[level] in data:
             raise KeyError(".".join(keys))
         return (
             Configuration.__get_value(data[keys[level]], keys, level + 1)
             if level + 1 < len(keys)
             else data[keys[level]]
         )
 
+    def _set_value(self, keys: tuple[str], value: T) -> None:
+        Configuration.__set_value(self._data, keys, value)
+
+    @staticmethod
+    def __set_value(container, keys: tuple[str], value: T) -> None:
+        n = len(keys)
+        container.update()
+        if keys[0] not in container:
+            if n == 1:
+                container.add(keys[0], value)
+            else:
+                t = tomllib.table()
+                t.add(keys[-1], value)
+                container.add(".".join(keys[:-1]), t)
+                container.add(tomllib.nl())
+        else:
+            if n == 1:
+                container[keys[0]] = value
+            else:
+                Configuration.__set_value(container[keys[0]], keys[1:], value)
+
     def __getattr__(self, name: str) -> Any:
-        if not Configuration.SettingsAccess.ATTR in self._access:
-            raise AttributeError(name)
-        if name in self._settings:
-            return self._settings[name]
-        if not self._has_section(name):
+        if name in (
+            "_defined_only",
+            "_access",
+            "_allow_changes",
+            "_settings",
+            "_settings_flex",
+            "_data",
+        ):
             raise AttributeError(name)
 
-        return Configuration._Proxy(self, name)
+        if Configuration.SettingsAccess.ATTR in self._access:
+            if name in self._settings:
+                return self._settings[name]
+            elif not self._defined_only and name in self._settings_flex:
+                return self._settings_flex[name]
+            elif self._has_section(name):
+                return Configuration._Proxy(self, name)
+        raise AttributeError(name)
+
+    def __setattr__(self, name: str, value: Any) -> None:
+        if name in (
+            "_defined_only",
+            "_access",
+            "_allow_changes",
+            "_settings",
+            "_settings_flex",
+            "_data",
+        ):
+            return super().__setattr__(name, value)
+
+        if Configuration.SettingsAccess.ATTR in self._access:
+            if name in self._settings:
+                self._settings[name] = value
+                return
+            elif not self._defined_only and name in self._settings_flex:
+                self._settings_flex[name] = value
+                return
+        super().__setattr__(name, value)
 
     def __getitem__(self, name: str) -> Any:
-        if (
-            not Configuration.SettingsAccess.ITEM in self._access
-            or not name in self._settings
-        ):
-            raise KeyError(name)
-        return self._settings[name].__get__(self)
+        if Configuration.SettingsAccess.ITEM in self._access:
+            if name in self._settings:
+                return self._settings[name].__get__(self)
+            elif not self._defined_only and name in self._settings_flex:
+                return self._settings_flex[name].__get__(self)
+        raise KeyError(name)
+
+    def __setitem__(self, name: str, value: Any) -> None:
+        if Configuration.SettingsAccess.ITEM in self._access:
+            if name in self._settings:
+                return self._settings[name].__set__(self, value)
+            elif not self._defined_only and name in self._settings_flex:
+                return self._settings_flex[name].__set__(self, value)
+        raise KeyError(name)
```

