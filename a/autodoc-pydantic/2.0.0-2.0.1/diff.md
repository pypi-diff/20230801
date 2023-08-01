# Comparing `tmp/autodoc_pydantic-2.0.0.tar.gz` & `tmp/autodoc_pydantic-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodoc_pydantic-2.0.0.tar", max compression
+gzip compressed data, was "autodoc_pydantic-2.0.1.tar", max compression
```

## Comparing `autodoc_pydantic-2.0.0.tar` & `autodoc_pydantic-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1071 2023-07-24 20:07:57.450222 autodoc_pydantic-2.0.0/LICENSE
--rw-r--r--   0        0        0    17990 2023-07-24 20:07:57.450222 autodoc_pydantic-2.0.0/README.md
--rw-r--r--   0        0        0     1944 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/__init__.py
--rw-r--r--   0        0        0     6075 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/__init__.py
--rw-r--r--   0        0        0      181 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/css/autodoc_pydantic.css
--rw-r--r--   0        0        0        0 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/__init__.py
--rw-r--r--   0        0        0    30118 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/autodocumenters.py
--rw-r--r--   0        0        0     8884 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/directives.py
--rw-r--r--   0        0        0        0 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/__init__.py
--rw-r--r--   0        0        0     9253 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/composites.py
--rw-r--r--   0        0        0     3484 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/definition.py
--rw-r--r--   0        0        0      452 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/enums.py
--rw-r--r--   0        0        0     1814 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/validators.py
--rw-r--r--   0        0        0      838 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/templates.py
--rw-r--r--   0        0        0     1957 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/utility.py
--rw-r--r--   0        0        0      946 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/events.py
--rw-r--r--   0        0        0    17697 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/inspection.py
--rw-r--r--   0        0        0     1736 2023-07-24 20:07:57.466222 autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/utility.py
--rw-r--r--   0        0        0    19874 1970-01-01 00:00:00.000000 autodoc_pydantic-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-01 21:53:05.924861 autodoc_pydantic-2.0.1/LICENSE
+-rw-r--r--   0        0        0    19092 2023-08-01 21:53:05.924861 autodoc_pydantic-2.0.1/README.md
+-rw-r--r--   0        0        0     1944 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/__init__.py
+-rw-r--r--   0        0        0     6075 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/__init__.py
+-rw-r--r--   0        0        0      181 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/css/autodoc_pydantic.css
+-rw-r--r--   0        0        0        0 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/__init__.py
+-rw-r--r--   0        0        0    30118 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/autodocumenters.py
+-rw-r--r--   0        0        0     8884 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/directives.py
+-rw-r--r--   0        0        0        0 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/__init__.py
+-rw-r--r--   0        0        0     9253 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/composites.py
+-rw-r--r--   0        0        0     3484 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/definition.py
+-rw-r--r--   0        0        0      452 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/enums.py
+-rw-r--r--   0        0        0     1814 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/validators.py
+-rw-r--r--   0        0        0      838 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/templates.py
+-rw-r--r--   0        0        0     1977 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/utility.py
+-rw-r--r--   0        0        0      946 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/events.py
+-rw-r--r--   0        0        0    15925 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/inspection.py
+-rw-r--r--   0        0        0     1736 2023-08-01 21:53:05.936861 autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/utility.py
+-rw-r--r--   0        0        0    20976 1970-01-01 00:00:00.000000 autodoc_pydantic-2.0.1/PKG-INFO
```

### Comparing `autodoc_pydantic-2.0.0/LICENSE` & `autodoc_pydantic-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.0/README.md` & `autodoc_pydantic-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![PyPI version](https://img.shields.io/pypi/v/autodoc_pydantic?style=for-the-badge)](https://pypi.org/project/autodoc-pydantic/)
 ![Python](https://img.shields.io/badge/python-3.7+-blue.svg?style=for-the-badge)
 
 [![Master](https://img.shields.io/github/actions/workflow/status/mansenfranzen/autodoc_pydantic/tests.yml?branch=main&style=for-the-badge)](https://github.com/mansenfranzen/autodoc_pydantic/actions/workflows/tests.yml)
 [![Coverage](https://img.shields.io/codecov/c/gh/mansenfranzen/autodoc_pydantic?style=for-the-badge)](https://app.codecov.io/gh/mansenfranzen/autodoc_pydantic)
 
 [![Downloads](https://img.shields.io/pypi/dm/autodoc_pydantic?color=fe7d37&style=for-the-badge)](https://pypistats.org/packages/autodoc-pydantic)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-34-orange.svg?style=for-the-badge)](#contributors)
+[![All Contributors](https://img.shields.io/badge/all_contributors-37-orange.svg?style=for-the-badge)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 
 You love [pydantic](https://pydantic-docs.helpmanual.io/) ❤ and you want to
 document your models and configuration settings with [sphinx](https://www.sphinx-doc.org/en/master/)?
 
 Perfect, let's go. But wait, sphinx' [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html)
@@ -98,14 +98,19 @@
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://jon-e.net"><img src="https://avatars.githubusercontent.com/u/12961499?v=4?s=100" width="100px;" alt="Jonny Saunders"/><br /><sub><b>Jonny Saunders</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Asneakers-the-rat" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://charlie.machalow.com"><img src="https://avatars.githubusercontent.com/u/5749838?v=4?s=100" width="100px;" alt="Charles Machalow"/><br /><sub><b>Charles Machalow</b></sub></a><br /><a href="#question-csm10495" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/tkaraouzene"><img src="https://avatars.githubusercontent.com/u/20064077?v=4?s=100" width="100px;" alt="Thomas Karaouzene"/><br /><sub><b>Thomas Karaouzene</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Atkaraouzene" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/caseyzak24"><img src="https://avatars.githubusercontent.com/u/29411281?v=4?s=100" width="100px;" alt="caseyzak24"/><br /><sub><b>caseyzak24</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=caseyzak24" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/PriOliveira"><img src="https://avatars.githubusercontent.com/u/13801839?v=4?s=100" width="100px;" alt="Priscila Oliveira"/><br /><sub><b>Priscila Oliveira</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3APriOliveira" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-PriOliveira" title="User Testing">📓</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/awoimbee"><img src="https://avatars.githubusercontent.com/u/22431493?v=4?s=100" width="100px;" alt="Arthur Woimbée"/><br /><sub><b>Arthur Woimbée</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3Aawoimbee" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-awoimbee" title="User Testing">📓</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=awoimbee" title="Code">💻</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=awoimbee" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/effigies"><img src="https://avatars.githubusercontent.com/u/83442?v=4?s=100" width="100px;" alt="Chris Markiewicz"/><br /><sub><b>Chris Markiewicz</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Aeffigies" title="Bug reports">🐛</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nagledb"><img src="https://avatars.githubusercontent.com/u/727435?v=4?s=100" width="100px;" alt="David B. Nagle"/><br /><sub><b>David B. Nagle</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Anagledb" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jerryjiahaha"><img src="https://avatars.githubusercontent.com/u/3163720?v=4?s=100" width="100px;" alt="JerryJia"/><br /><sub><b>JerryJia</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=jerryjiahaha" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 github/actions/workflow/status/mansenfranzen/autodoc_pydantic/
 tests.yml?branch=main&style=for-the-badge)](https://github.com/mansenfranzen/
 autodoc_pydantic/actions/workflows/tests.yml) [![Coverage](https://
 img.shields.io/codecov/c/gh/mansenfranzen/autodoc_pydantic?style=for-the-
 badge)](https://app.codecov.io/gh/mansenfranzen/autodoc_pydantic) [![Downloads]
 (https://img.shields.io/pypi/dm/autodoc_pydantic?color=fe7d37&style=for-the-
 badge)](https://pypistats.org/packages/autodoc-pydantic) [![All Contributors]
-(https://img.shields.io/badge/all_contributors-34-orange.svg?style=for-the-
+(https://img.shields.io/badge/all_contributors-37-orange.svg?style=for-the-
 badge)](#contributors)  You love [pydantic](https://pydantic-
 docs.helpmanual.io/) â¤ and you want to document your models and configuration
 settings with [sphinx](https://www.sphinx-doc.org/en/master/)? Perfect, let's
 go. But wait, sphinx' [autodoc](https://www.sphinx-doc.org/en/master/usage/
 extensions/autodoc.html) does not integrate too well with pydantic models ð.
 Don't worry - just `pip install autodoc_pydantic` âº. ## Features - ð¬
 provides default values, alias and constraints for model fields - ð adds
@@ -53,13 +53,17 @@
              [j-carson]                     [Jakob_Lykke_Andersen]   [Juan_Luis_Cano_RodrÃ­guez   [Mikalai_Chaly]       [Stig_Korsnes]                     [Ilia_Kurenkov]       [Grzegorz_Bokota]
               j-carson                       Jakob_Lykke_Andersen     Juan_Luis_Cano_RodrÃ­guez    Mikalai_Chaly         Stig_Korsnes                       Ilia_Kurenkov         Grzegorz_Bokota
           ð ð» â ï¸             ð»                   ð              ð â ï      ð ð¤                    ð               ð
                    [jgunstone]                      [iwyrkore]           [spacemanspiff2007]           [Luke_Hsiao]        [Daniel_Walker]                 [Evgeniy_Lupashin]        [Jan-Hendrik
                     jgunstone                        iwyrkore             spacemanspiff2007             Luke_Hsiao          Daniel_Walker                   Evgeniy_Lupashin            Ewers]
                       ð                         ð»               ð ð¤            ð             ð                          ð         Jan-Hendrik_Ewers
                                                                                                                                                                                          ð
-               [Jonny_Saunders]                [Charles_Machalow]          [Thomas_Karaouzene]         [caseyzak24]     [Priscila_Oliveira]            [Arthur_WoimbÃ©e]
-                Jonny_Saunders                  Charles_Machalow            Thomas_Karaouzene           caseyzak24       Priscila_Oliveira              Arthur_WoimbÃ©e
-                     ð                         ð¬                    ð                 ð          ð ð�        ð ð ð» â ï¸
+               [Jonny_Saunders]                [Charles_Machalow]          [Thomas_Karaouzene]         [caseyzak24]     [Priscila_Oliveira]            [Arthur_WoimbÃ©e]              [Chris
+                Jonny_Saunders                  Charles_Machalow            Thomas_Karaouzene           caseyzak24       Priscila_Oliveira              Arthur_WoimbÃ©e             Markiewicz]
+                     ð                         ð¬                    ð                 ð          ð ð�        ð ð ð» â�Chris_Markiewicz
+                                                                                                                                                                                         ð
+               [David_B._Nagle]                     [JerryJia]
+                David_B._Nagle                       JerryJia
+                     ð                          ð»
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `autodoc_pydantic-2.0.0/pyproject.toml` & `autodoc_pydantic-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autodoc_pydantic"
-version = "2.0.0"
+version = "2.0.1"
 description = "Seamlessly integrate pydantic models in your Sphinx documentation."
 authors = ["mansenfranzen <franz.woellert@gmail.com>"]
 packages = [{ include = "sphinxcontrib" }]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mansenfranzen/autodoc_pydantic"
 repository = "https://github.com/mansenfranzen/autodoc_pydantic"
```

### Comparing `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/__init__.py` & `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/autodocumenters.py` & `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/autodocumenters.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/directives.py` & `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/directives.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/composites.py` & `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/composites.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/definition.py` & `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/definition.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/options/validators.py` & `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/options/validators.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/templates.py` & `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/templates.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/directives/utility.py` & `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/directives/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import re
 from typing import List
 
 from docutils.nodes import emphasis
 from sphinx.addnodes import pending_xref
 from sphinx.environment import BuildEnvironment
 
-REGEX_TYPE_ANNOT = re.compile(r"\s+:type:\s([a-zA-Z1-9]+)\[([a-zA-Z1-9]+)\]")
+REGEX_TYPE_ANNOT = re.compile(
+    r"\s+:type:\s([a-zA-Z1-9\._\[]+\]?)\[([a-zA-Z1-9\._\[\]]+)\]")
 
 
 class NullType:
     """Helper class to present a Null value which is not the same
     as python's `None`. This represents a missing value, or no
     value at all by convention. It should be used as a singleton.
```

### Comparing `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/events.py` & `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/events.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/inspection.py` & `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/inspection.py`

 * *Files 14% similar despite different names*

```diff
@@ -143,84 +143,38 @@
         """Get specific property value from pydantic's field info.
 
         """
 
         field = self.get(field_name)
         return getattr(field, property_name, None)
 
-    def get_constraint_items(self, field_name: str) -> Dict[str, str]:
-        """Extract all possible constraints along with their default values
-        from a fields meta attribute.
-
-        """
-
-        metadata = self.model.model_fields[field_name].metadata
-        available = [meta for meta in metadata if meta is not None]
-
-        return {key: getattr(meta, key)
-                for meta in available
-                for key, value in self._get_meta_items(meta).items()}
-
     @staticmethod
     def _get_meta_items(meta_class: Any) -> Dict[str, str]:
         """Helper method to extract constraint names and values from different
         pydantic Metadata objects such as `pydantic.types.Strict`.
 
         """
 
         try:
             return meta_class.__dataclass_fields__
         except AttributeError:
             return meta_class.__dict__
 
-    def get_given_constraint_keys(self, field_name: str) -> Set[str]:
-        """Retrieves all schema attribute keys that have been set.
-        This information is relevant to distinguish given values that are
-        equivalent to their default values. Otherwise, there is no chance
-        to determine if a constraint was actually given by the user or set as
-        a default value.
-
-        Note: Accessing private attributes with many levels of nesting is far
-        from being desired but currently there is no proper solution around
-        this. Accessing the `properties` via the `model_schema_json` may fail
-        in cases where fields are not serializable.
-
-        """
-
-        definition = self.model.__pydantic_core_schema__["definitions"][0]
-
-        # account for varying levels of nesting :-(
-        try:
-            field_schemas = definition["schema"]["fields"]
-        except KeyError:
-            field_schemas = definition["schema"]["schema"]["fields"]
-
-        # account for generics and other non-native fields without schema info
-        try:
-            schema = field_schemas[field_name]["schema"]
-        except KeyError:
-            return set()
-
-        # account for yet another level on model-field :-(
-        if "schema" in schema:
-            schema = schema["schema"]
-
-        return set(schema.keys())
-
     def get_constraints(self, field_name: str) -> Dict[str, Any]:
         """Get constraints for given `field_name`.
 
         """
 
-        constraint_items = self.get_constraint_items(field_name).items()
-        given_constraint_keys = self.get_given_constraint_keys(field_name)
+        metadata = self.model.model_fields[field_name].metadata
+        available = [meta for meta in metadata if meta is not None]
 
-        return {key: value
-                for key, value in constraint_items
-                if key in given_constraint_keys}
+        return {key: getattr(meta, key)
+                for meta in available
+                for key, value in self._get_meta_items(meta).items()
+                if getattr(meta, key) is not None}
 
     def is_required(self, field_name: str) -> bool:
         """Check if a given pydantic field is required/mandatory. Returns True,
         if a value for this field needs to provided upon model creation.
 
         """
```

### Comparing `autodoc_pydantic-2.0.0/sphinxcontrib/autodoc_pydantic/utility.py` & `autodoc_pydantic-2.0.1/sphinxcontrib/autodoc_pydantic/utility.py`

 * *Files identical despite different names*

### Comparing `autodoc_pydantic-2.0.0/PKG-INFO` & `autodoc_pydantic-2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodoc-pydantic
-Version: 2.0.0
+Version: 2.0.1
 Summary: Seamlessly integrate pydantic models in your Sphinx documentation.
 Home-page: https://github.com/mansenfranzen/autodoc_pydantic
 License: MIT
 Keywords: sphinx,pydantic,autodoc,documentation,extension
 Author: mansenfranzen
 Author-email: franz.woellert@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
@@ -43,15 +43,15 @@
 [![PyPI version](https://img.shields.io/pypi/v/autodoc_pydantic?style=for-the-badge)](https://pypi.org/project/autodoc-pydantic/)
 ![Python](https://img.shields.io/badge/python-3.7+-blue.svg?style=for-the-badge)
 
 [![Master](https://img.shields.io/github/actions/workflow/status/mansenfranzen/autodoc_pydantic/tests.yml?branch=main&style=for-the-badge)](https://github.com/mansenfranzen/autodoc_pydantic/actions/workflows/tests.yml)
 [![Coverage](https://img.shields.io/codecov/c/gh/mansenfranzen/autodoc_pydantic?style=for-the-badge)](https://app.codecov.io/gh/mansenfranzen/autodoc_pydantic)
 
 [![Downloads](https://img.shields.io/pypi/dm/autodoc_pydantic?color=fe7d37&style=for-the-badge)](https://pypistats.org/packages/autodoc-pydantic)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-34-orange.svg?style=for-the-badge)](#contributors)
+[![All Contributors](https://img.shields.io/badge/all_contributors-37-orange.svg?style=for-the-badge)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 
 You love [pydantic](https://pydantic-docs.helpmanual.io/) ❤ and you want to
 document your models and configuration settings with [sphinx](https://www.sphinx-doc.org/en/master/)?
 
 Perfect, let's go. But wait, sphinx' [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html)
@@ -138,14 +138,19 @@
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://jon-e.net"><img src="https://avatars.githubusercontent.com/u/12961499?v=4?s=100" width="100px;" alt="Jonny Saunders"/><br /><sub><b>Jonny Saunders</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Asneakers-the-rat" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://charlie.machalow.com"><img src="https://avatars.githubusercontent.com/u/5749838?v=4?s=100" width="100px;" alt="Charles Machalow"/><br /><sub><b>Charles Machalow</b></sub></a><br /><a href="#question-csm10495" title="Answering Questions">💬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/tkaraouzene"><img src="https://avatars.githubusercontent.com/u/20064077?v=4?s=100" width="100px;" alt="Thomas Karaouzene"/><br /><sub><b>Thomas Karaouzene</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Atkaraouzene" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/caseyzak24"><img src="https://avatars.githubusercontent.com/u/29411281?v=4?s=100" width="100px;" alt="caseyzak24"/><br /><sub><b>caseyzak24</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=caseyzak24" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/PriOliveira"><img src="https://avatars.githubusercontent.com/u/13801839?v=4?s=100" width="100px;" alt="Priscila Oliveira"/><br /><sub><b>Priscila Oliveira</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3APriOliveira" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-PriOliveira" title="User Testing">📓</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/awoimbee"><img src="https://avatars.githubusercontent.com/u/22431493?v=4?s=100" width="100px;" alt="Arthur Woimbée"/><br /><sub><b>Arthur Woimbée</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/pulls?q=is%3Apr+reviewed-by%3Aawoimbee" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-awoimbee" title="User Testing">📓</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=awoimbee" title="Code">💻</a> <a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=awoimbee" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/effigies"><img src="https://avatars.githubusercontent.com/u/83442?v=4?s=100" width="100px;" alt="Chris Markiewicz"/><br /><sub><b>Chris Markiewicz</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Aeffigies" title="Bug reports">🐛</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nagledb"><img src="https://avatars.githubusercontent.com/u/727435?v=4?s=100" width="100px;" alt="David B. Nagle"/><br /><sub><b>David B. Nagle</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/issues?q=author%3Anagledb" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jerryjiahaha"><img src="https://avatars.githubusercontent.com/u/3163720?v=4?s=100" width="100px;" alt="JerryJia"/><br /><sub><b>JerryJia</b></sub></a><br /><a href="https://github.com/mansenfranzen/autodoc_pydantic/commits?author=jerryjiahaha" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

