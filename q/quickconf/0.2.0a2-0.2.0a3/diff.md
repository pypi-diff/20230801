# Comparing `tmp/quickconf-0.2.0a2.tar.gz` & `tmp/quickconf-0.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickconf-0.2.0a2.tar", last modified: Tue Aug  1 08:32:01 2023, max compression
+gzip compressed data, was "quickconf-0.2.0a3.tar", last modified: Tue Aug  1 19:23:36 2023, max compression
```

## Comparing `quickconf-0.2.0a2.tar` & `quickconf-0.2.0a3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.470264 quickconf-0.2.0a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 08:31:46.000000 quickconf-0.2.0a2/.version
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/demo/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/demo/settings.toml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/demo/settings_updated.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/demo/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.470264 quickconf-0.2.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/src/quickconf/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/src/quickconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 08:31:46.000000 quickconf-0.2.0a2/src/quickconf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/src/quickconf/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/src/quickconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 08:32:01.000000 quickconf-0.2.0a2/src/quickconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-01 08:32:01.000000 quickconf-0.2.0a2/src/quickconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:32:01.000000 quickconf-0.2.0a2/src/quickconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 08:32:01.000000 quickconf-0.2.0a2/src/quickconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 08:32:01.000000 quickconf-0.2.0a2/src/quickconf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:01.474265 quickconf-0.2.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 08:31:40.000000 quickconf-0.2.0a2/tests/test_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.753342 quickconf-0.2.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.745342 quickconf-0.2.0a3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 19:23:16.000000 quickconf-0.2.0a3/.version
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/demo/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/demo/settings.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/demo/settings_updated.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/demo/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:23:36.753342 quickconf-0.2.0a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.745342 quickconf-0.2.0a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/src/quickconf/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/src/quickconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 19:23:16.000000 quickconf-0.2.0a3/src/quickconf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/src/quickconf/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/src/quickconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/tests/test_conf.py
```

### Comparing `quickconf-0.2.0a2/.github/workflows/release.yml` & `quickconf-0.2.0a3/.github/workflows/release.yml`

 * *Files 21% similar despite different names*

```diff
@@ -21,16 +21,23 @@
 
     steps:
       - name: Check version
         id: check-version
         run: |
           pattern="^refs\/tags\/v([0-9]+\.[0-9]+\.[0-9]+(-(a|alpha|b|beta|dev)[0-9]+)?)$"
           [[ "${{ github.ref }}" =~ $pattern ]]
-          echo ::set-output name=version::${BASH_REMATCH[1]}
-          [ -z "${BASH_REMATCH[2]}" ] || echo ::set-output name=prerelease::true
+          version="${BASH_REMATCH[1]}"
+          if [ ! -z "${BASH_REMATCH[2]}" ]
+          then
+              version="${version/-/}"
+              version="${version/alpha/a}"
+              version="${version/beta/b}"
+              echo ::set-output name=prerelease::true
+          fi
+          echo ::set-output name=version::$version
 
       - name: Checkout repo
         uses: actions/checkout@v3
 
       - name: Write version files
         env:
           VERSION: ${{ steps.check-version.outputs.version }}
```

### Comparing `quickconf-0.2.0a2/.github/workflows/tests.yml` & `quickconf-0.2.0a3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a2/.gitignore` & `quickconf-0.2.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a2/.pre-commit-config.yaml` & `quickconf-0.2.0a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a2/LICENSE` & `quickconf-0.2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a2/PKG-INFO` & `quickconf-0.2.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: quickconf
-Version: 0.2.0a2
+Version: 0.2.0a3
 Summary: Simple and flexible TOML-file based configurations framework
 Author-email: Kenneth Trelborg Vestergaard <mortencombat@fastmail.com>
-Project-URL: homepage, https://github.com/mortencombat/quickconf
-Project-URL: repository, https://github.com/mortencombat/quickconf
+Project-URL: Homepage, https://github.com/mortencombat/quickconf
+Project-URL: Repository, https://github.com/mortencombat/quickconf
 Keywords: configuration,settings,options,toml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `quickconf-0.2.0a2/README.md` & `quickconf-0.2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a2/demo/example.py` & `quickconf-0.2.0a3/demo/example.py`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a2/pyproject.toml` & `quickconf-0.2.0a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 build = [ 'setuptools', 'build', 'wheel', 'twine' ]
 test = [ 'pre-commit', 'pytest', 'pytest-cov' ]
 
 [tool.setuptools.dynamic]
 version = {file = [".version"]}
 
 [project.urls]
-homepage = "https://github.com/mortencombat/quickconf"
-repository = "https://github.com/mortencombat/quickconf"
+Homepage = "https://github.com/mortencombat/quickconf"
+Repository = "https://github.com/mortencombat/quickconf"
```

### Comparing `quickconf-0.2.0a2/src/quickconf/core.py` & `quickconf-0.2.0a3/src/quickconf/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,47 @@
     except ModuleNotFoundError:
         import tomli as tomllib
 
 T = TypeVar("T")
 
 _key_pattern = re.compile("[A-Za-z0-9_-]+")
 
+_FIXED_ATTR = (
+    "_defined_only",
+    "_access",
+    "_allow_changes",
+    "_settings",
+    "_settings_flex",
+    "_data",
+)
+
+# RESERVED_CONFIG = (
+#     "__defined_only",
+#     "__access",
+#     "__allow_changes",
+#     "__settings",
+#     "__settings_flex",
+#     "__data",
+#     "__TYPE_MAP",
+#     "load",
+#     "reset",
+#     "save",
+#     "__has_section",
+#     "__load_toml",
+#     "__load_dict",
+#     "__get_settings_from_dict",
+#     "",
+#     "",
+#     "",
+# )
+# RESERVED_PROXY = (
+#     "__name",
+#     "__config",
+# )
+
 
 def parse_key(key: str) -> tuple[str]:
     keys = key.split(".")
     for k in keys:
         if not _key_pattern.match(k):
             raise ValueError(
                 f"{key} is invalid/unsupported. Only bare TOML keys are supported."
@@ -33,27 +66,31 @@
     return tuple(keys)
 
 
 class Setting(Generic[T]):
     # NOTE: This is a 'descriptor class', similar to using property()
     # https://docs.python.org/3/reference/datamodel.html?highlight=__get__#implementing-descriptors
 
-    def __init__(self, name: str, *, default: T = None, doc: str = None) -> None:
+    def __init__(
+        self,
+        name: str,
+        *,
+        default: T = None,
+        doc: str = None,
+    ) -> None:
         super().__init__()
 
         self._name = name.replace(" ", "")
         self._keys = parse_key(self._name)
         self._default = default
         self._type = None
         self.__doc__ = doc
         self._reset()
 
-    # TODO: implement name validator, does tomllib have a method we can use?
-
-    # Add support for validators, and a couple of stock validators
+    # TODO: Add support for validators, and a couple of stock validators
 
     @property
     def name(self) -> str:
         return self._name
 
     def _reset(self) -> None:
         self._value = None
@@ -215,35 +252,45 @@
         # Misc. config
         self._defined_only = defined_only
         self._access = access
         self._allow_changes = allow_changes
 
         # Assemble options from arg and class attributes.
         self._settings = Settings(settings)
+        for setting in self._settings:
+            self._check_setting_name(setting._name)
         self._settings_flex = Settings()
         for _, obj in getmembers(type(self)):
             if not isinstance(obj, Setting):
                 continue
             self._settings.append(obj)
+
+        # Misc helpers
         self.__TYPE_MAP = None
+        self.__RESERVED = (
+            dir(self) if Configuration.SettingsAccess.ATTR in access else None
+        )
 
         # Load configuration
         self.load(config)
 
-    def __get_base_type(self, cls) -> type:
+    def _get_base_type(self, cls) -> type:
         if _USE_TOMLKIT:
             if not self.__TYPE_MAP:
                 self.__TYPE_MAP = {
                     tomllib.items.Float: float,
                     tomllib.items.Integer: int,
                     tomllib.items.String: str,
                     tomllib.items.DateTime: datetime,
                     tomllib.items.Date: date,
                     tomllib.items.Time: time,
                     tomllib.items.Bool: bool,
+                    tomllib.items.Array: list,
+                    tomllib.items.AbstractTable: dict,
+                    tomllib.items.Table: dict,
                 }
             if cls in self.__TYPE_MAP:
                 return self.__TYPE_MAP[cls]
             raise TypeError(cls)
         else:
             return cls
 
@@ -301,23 +348,31 @@
         """Load configuration settings from a dict."""
         self.reset()
         self._data = config
         if not self._defined_only:
             # Add settings to self._settings_flex for each item in self._data,
             # unless it is already defined in self._settings
             for setting, value in self._get_settings_from_dict(config).items():
+                self._check_setting_name(setting)
                 if setting not in self._settings:
                     self._settings_flex.append(
-                        Setting[self.__get_base_type(type(value))](setting)
+                        Setting[self._get_base_type(type(value))](setting)
                     )
 
     @property
     def is_readonly(self) -> bool:
         return not _USE_TOMLKIT or not self._allow_changes
 
+    def _check_setting_name(self, name: str) -> None:
+        if Configuration.SettingsAccess.ATTR not in self._access:
+            return
+        for key in name.split("."):
+            if key in self.__RESERVED:
+                raise ValueError(f"'{key}' is a reserved keyword/attribute")
+
     @property
     def settings(self) -> dict[str, Any]:
         r = {}
         for s in chain(self._settings, self._settings_flex):
             r[s.name] = s.__get__(self)
         return dict(sorted(r.items()))
 
@@ -357,42 +412,28 @@
         else:
             if n == 1:
                 container[keys[0]] = value
             else:
                 Configuration.__set_value(container[keys[0]], keys[1:], value)
 
     def __getattr__(self, name: str) -> Any:
-        if name in (
-            "_defined_only",
-            "_access",
-            "_allow_changes",
-            "_settings",
-            "_settings_flex",
-            "_data",
-        ):
+        if name in _FIXED_ATTR:
             raise AttributeError(name)
 
         if Configuration.SettingsAccess.ATTR in self._access:
             if name in self._settings:
                 return self._settings[name]
             elif not self._defined_only and name in self._settings_flex:
                 return self._settings_flex[name]
             elif self._has_section(name):
                 return Configuration._Proxy(self, name)
         raise AttributeError(name)
 
     def __setattr__(self, name: str, value: Any) -> None:
-        if name in (
-            "_defined_only",
-            "_access",
-            "_allow_changes",
-            "_settings",
-            "_settings_flex",
-            "_data",
-        ):
+        if name in _FIXED_ATTR:
             return super().__setattr__(name, value)
 
         if Configuration.SettingsAccess.ATTR in self._access:
             if name in self._settings:
                 self._settings[name] = value
                 return
             elif not self._defined_only and name in self._settings_flex:
```

### Comparing `quickconf-0.2.0a2/src/quickconf.egg-info/PKG-INFO` & `quickconf-0.2.0a3/src/quickconf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: quickconf
-Version: 0.2.0a2
+Version: 0.2.0a3
 Summary: Simple and flexible TOML-file based configurations framework
 Author-email: Kenneth Trelborg Vestergaard <mortencombat@fastmail.com>
-Project-URL: homepage, https://github.com/mortencombat/quickconf
-Project-URL: repository, https://github.com/mortencombat/quickconf
+Project-URL: Homepage, https://github.com/mortencombat/quickconf
+Project-URL: Repository, https://github.com/mortencombat/quickconf
 Keywords: configuration,settings,options,toml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `quickconf-0.2.0a2/src/quickconf.egg-info/SOURCES.txt` & `quickconf-0.2.0a3/src/quickconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

