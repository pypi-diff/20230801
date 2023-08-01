# Comparing `tmp/mkdocs-markmap-2.3.0.tar.gz` & `tmp/mkdocs-markmap-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-markmap-2.3.0.tar", last modified: Thu Aug 25 17:23:49 2022, max compression
+gzip compressed data, was "mkdocs-markmap-2.4.0.tar", last modified: Tue Aug  1 21:02:42 2023, max compression
```

## Comparing `mkdocs-markmap-2.3.0.tar` & `mkdocs-markmap-2.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 17:23:49.102151 mkdocs-markmap-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-08-25 17:23:36.000000 mkdocs-markmap-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-08-25 17:23:49.102151 mkdocs-markmap-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-08-25 17:23:36.000000 mkdocs-markmap-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 17:23:49.102151 mkdocs-markmap-2.3.0/mkdocs_markmap/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-25 17:23:36.000000 mkdocs-markmap-2.3.0/mkdocs_markmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-08-25 17:23:36.000000 mkdocs-markmap-2.3.0/mkdocs_markmap/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-08-25 17:23:36.000000 mkdocs-markmap-2.3.0/mkdocs_markmap/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     4183 2022-08-25 17:23:36.000000 mkdocs-markmap-2.3.0/mkdocs_markmap/extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     5020 2022-08-25 17:23:36.000000 mkdocs-markmap-2.3.0/mkdocs_markmap/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 17:23:49.102151 mkdocs-markmap-2.3.0/mkdocs_markmap/static_files/
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-08-25 17:23:36.000000 mkdocs-markmap-2.3.0/mkdocs_markmap/static_files/mkdocs-markmap.css
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-08-25 17:23:36.000000 mkdocs-markmap-2.3.0/mkdocs_markmap/static_files/mkdocs-markmap.js
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-08-25 17:23:36.000000 mkdocs-markmap-2.3.0/mkdocs_markmap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 17:23:49.102151 mkdocs-markmap-2.3.0/mkdocs_markmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-08-25 17:23:49.000000 mkdocs-markmap-2.3.0/mkdocs_markmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-08-25 17:23:49.000000 mkdocs-markmap-2.3.0/mkdocs_markmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 17:23:49.000000 mkdocs-markmap-2.3.0/mkdocs_markmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-08-25 17:23:49.000000 mkdocs-markmap-2.3.0/mkdocs_markmap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-25 17:23:49.000000 mkdocs-markmap-2.3.0/mkdocs_markmap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-25 17:23:49.000000 mkdocs-markmap-2.3.0/mkdocs_markmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-25 17:23:49.102151 mkdocs-markmap-2.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2051 2022-08-25 17:23:36.000000 mkdocs-markmap-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:02:42.140441 mkdocs-markmap-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-01 21:02:23.000000 mkdocs-markmap-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-08-01 21:02:42.140441 mkdocs-markmap-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-08-01 21:02:23.000000 mkdocs-markmap-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:02:42.140441 mkdocs-markmap-2.4.0/mkdocs_markmap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:02:23.000000 mkdocs-markmap-2.4.0/mkdocs_markmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-01 21:02:23.000000 mkdocs-markmap-2.4.0/mkdocs_markmap/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-01 21:02:23.000000 mkdocs-markmap-2.4.0/mkdocs_markmap/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-08-01 21:02:23.000000 mkdocs-markmap-2.4.0/mkdocs_markmap/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-08-01 21:02:23.000000 mkdocs-markmap-2.4.0/mkdocs_markmap/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:02:42.140441 mkdocs-markmap-2.4.0/mkdocs_markmap/static_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 21:02:23.000000 mkdocs-markmap-2.4.0/mkdocs_markmap/static_files/mkdocs-markmap.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-01 21:02:23.000000 mkdocs-markmap-2.4.0/mkdocs_markmap/static_files/mkdocs-markmap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-08-01 21:02:23.000000 mkdocs-markmap-2.4.0/mkdocs_markmap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:02:42.140441 mkdocs-markmap-2.4.0/mkdocs_markmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-08-01 21:02:42.000000 mkdocs-markmap-2.4.0/mkdocs_markmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-01 21:02:42.000000 mkdocs-markmap-2.4.0/mkdocs_markmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:02:42.000000 mkdocs-markmap-2.4.0/mkdocs_markmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 21:02:42.000000 mkdocs-markmap-2.4.0/mkdocs_markmap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 21:02:42.000000 mkdocs-markmap-2.4.0/mkdocs_markmap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 21:02:42.000000 mkdocs-markmap-2.4.0/mkdocs_markmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:02:42.140441 mkdocs-markmap-2.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2051 2023-08-01 21:02:23.000000 mkdocs-markmap-2.4.0/setup.py
```

### Comparing `mkdocs-markmap-2.3.0/LICENSE` & `mkdocs-markmap-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-markmap-2.3.0/PKG-INFO` & `mkdocs-markmap-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-markmap
-Version: 2.3.0
+Version: 2.4.0
 Summary: MkDocs plugin and extension to creates mindmaps from markdown using markmap
 Home-page: https://github.com/markmap/mkdocs-markmap
 Author: neatc0der
 Author-email: 
 License: MIT
 Keywords: mkdocs python markdown markmap mindmap include
 Platform: UNKNOWN
@@ -91,34 +91,35 @@
 
 ```yaml
 plugins:
   - markmap:
       base_path: docs
       encoding: utf-8
       file_extension: .mm.md
-      d3_version: 6.7.0
-      lib_version: 0.14.1
-      view_version: 0.14.0
+      d3_version: 7
+      lib_version: 0.15.3
+      view_version: 0.15.3
 ```
 
 In addition, feel free to define your favourite source urls like this:
 
 ```yaml
+plugins:
+  - markmap:
+      # disable the default assets first
+      d3_version: ''
+      lib_version: ''
+      view_version: ''
+
 extra_javascript:
-  - https://unpkg.com/d3@6.7.0/dist/d3.min.js
-  - https://unpkg.com/markmap-lib@0.14.1/dist/browser/index.min.js
-  - https://unpkg.com/markmap-view@0.14.0/dist/index.min.js
+  - https://unpkg.com/d3@7/dist/d3.min.js
+  - https://unpkg.com/markmap-lib@0.15.3/dist/browser/index.js
+  - https://unpkg.com/markmap-view@0.15.3/dist/browser/index.js
 ```
 
-:warning: The urls need to contain one of these keywords to be considered as deviation from default:
-
-* `markmap-d3`
-* `markmap-lib`
-* `markmap-view`
-
 ## Troubleshooting
 
 ### Nav tree lists markmaps
 
 1. Move your markmap files to a separate folder next to `docs`, e.g. `mindmaps`
 2. Configure `base_path` accordingly (see [Advanced Settings](#advanced-settings))
```

### Comparing `mkdocs-markmap-2.3.0/README.md` & `mkdocs-markmap-2.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -68,34 +68,35 @@
 
 ```yaml
 plugins:
   - markmap:
       base_path: docs
       encoding: utf-8
       file_extension: .mm.md
-      d3_version: 6.7.0
-      lib_version: 0.14.1
-      view_version: 0.14.0
+      d3_version: 7
+      lib_version: 0.15.3
+      view_version: 0.15.3
 ```
 
 In addition, feel free to define your favourite source urls like this:
 
 ```yaml
+plugins:
+  - markmap:
+      # disable the default assets first
+      d3_version: ''
+      lib_version: ''
+      view_version: ''
+
 extra_javascript:
-  - https://unpkg.com/d3@6.7.0/dist/d3.min.js
-  - https://unpkg.com/markmap-lib@0.14.1/dist/browser/index.min.js
-  - https://unpkg.com/markmap-view@0.14.0/dist/index.min.js
+  - https://unpkg.com/d3@7/dist/d3.min.js
+  - https://unpkg.com/markmap-lib@0.15.3/dist/browser/index.js
+  - https://unpkg.com/markmap-view@0.15.3/dist/browser/index.js
 ```
 
-:warning: The urls need to contain one of these keywords to be considered as deviation from default:
-
-* `markmap-d3`
-* `markmap-lib`
-* `markmap-view`
-
 ## Troubleshooting
 
 ### Nav tree lists markmaps
 
 1. Move your markmap files to a separate folder next to `docs`, e.g. `mindmaps`
 2. Configure `base_path` accordingly (see [Advanced Settings](#advanced-settings))
```

### Comparing `mkdocs-markmap-2.3.0/mkdocs_markmap/extension.py` & `mkdocs-markmap-2.4.0/mkdocs_markmap/extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,107 +5,107 @@
 from typing import AnyStr, Dict, List, Optional
 
 from markdown import Markdown
 from markdown.extensions import Extension
 from markdown.preprocessors import Preprocessor
 
 
-log = logging.getLogger('mkdocs.markmap')
+log = logging.getLogger("mkdocs.markmap")
 
 
-INCLUDE_SYNTAX = re.compile(r'\{!\s*(?P<path>.+?)\s*!\}')
+INCLUDE_SYNTAX = re.compile(r"\{!\s*(?P<path>.+?)\s*!\}")
 
 
 class MarkmapPreprocessor(Preprocessor):
     """
     Wraps the content of the markdown with a code block for markmap.
     """
 
     def __init__(self, md: Markdown, config: Dict[str, str]):
         super(MarkmapPreprocessor, self).__init__(md)
-        self.base_path: str = config['base_path']
-        self.encoding: str = config['encoding']
-        self.file_extension: str = config['file_extension']
+        self.base_path: str = config["base_path"]
+        self.encoding: str = config["encoding"]
+        self.file_extension: str = config["file_extension"]
 
     def run(self, lines: List[str]) -> List[str]:
         done: bool = False
         included_paths: List[Path] = []
         while not done:
             for loc, line in enumerate(lines):
                 match: Optional[re.Match[AnyStr]] = INCLUDE_SYNTAX.search(line)
                 if match is None:
                     continue
 
-                path: Path = Path(match.group('path'))
+                path: Path = Path(match.group("path"))
                 if not path.name.lower().endswith(self.file_extension):
                     continue
 
                 if not path.is_absolute():
                     path = (Path(self.base_path) / path).resolve()
 
                 if path in included_paths:
                     log.warning(f"loop detected while including: {path}")
                     continue
 
                 included_paths.append(path)
                 try:
-                    with open(path, 'r', encoding=self.encoding) as r:
+                    with open(path, "r", encoding=self.encoding) as r:
                         markmap: List[str] = r.readlines()
                         
                 except Exception as e:
-                    log.error('unable to include file {}. Ignoring statement. Error: {}'.format(path, e))
-                    lines[loc] = INCLUDE_SYNTAX.sub('',line)
+                    log.error("unable to include file {}. Ignoring statement. Error: {}".format(path, e))
+                    lines[loc] = INCLUDE_SYNTAX.sub("",line)
                     break
 
                 line_split: List[str] = INCLUDE_SYNTAX.split(line)
                 if len(markmap) == 0:
-                    markmap.append('')
+                    markmap.append("")
                 else:
-                    markmap.insert(0, '```markmap')
-                    markmap.append('```')
+                    markmap.insert(0, "```markmap")
+                    markmap.append("```")
                 
-                if line_split[0].strip() != '':
+                if line_split[0].strip() != "":
                     markmap.insert(0, line_split[0])
 
-                if line_split[2].strip() != '':
+                if line_split[2].strip() != "":
                     markmap.append(line_split[2])
 
                 lines = lines[:loc] + markmap + lines[loc+1:]
                 break
                 
             else:
                 done = True
 
         return lines
 
 
 class MarkmapExtension(Extension):
     config_defaults: Dict[str, str] = {
-        'base_path': ['docs', 'Default location from which to evaluate relative paths for the include statement.'],
-        'encoding': ['utf-8', 'Encoding of the files used by the include statement.'],
-        'file_extension': ['.mm.md', 'File extension of mindmap files'],
+        "base_path": ["docs", "Default location from which to evaluate relative paths for the include statement."],
+        "encoding": ["utf-8", "Encoding of the files used by the include statement."],
+        "file_extension": [".mm.md", "File extension of mindmap files"],
     }
 
     def __init__(self, **configs: Dict[str, str]):
         self.config: Dict[str, str] = self.config_defaults
         for key, value in configs.items():
             self.setConfig(key, value)
 
     def extendMarkdown(self, md: Markdown) -> None:
-        md.preprocessors.register(MarkmapPreprocessor(md, self.getConfigs()), 'include_markmap', 102)
+        md.preprocessors.register(MarkmapPreprocessor(md, self.getConfigs()), "include_markmap", 102)
         for extension in md.registeredExtensions:
-            if extension.__class__.__name__ == 'SuperFencesCodeExtension':
-                log.info(f'superfences detected by markmap')
+            if extension.__class__.__name__ == "SuperFencesCodeExtension":
+                log.info(f"superfences detected by markmap")
                 try:
                     from pymdownx.superfences import default_validator, fence_code_format, _formatter, _validator
                     extension.extend_super_fences(
-                        'markmap',
-                        partial(_formatter, class_name='language-markmap', _fmt=fence_code_format),
+                        "markmap",
+                        partial(_formatter, class_name="language-markmap", _fmt=fence_code_format),
                         partial(_validator, validator=default_validator)
                     )
                     break
 
                 except ImportError as e:
-                    log.warning(f'markmap detected pymdownx.superfences, but import is not working: {e}')
+                    log.warning(f"markmap detected pymdownx.superfences, but import is not working: {e}")
 
                 except Exception as e:
-                    log.error(f'unexpected error: {e}')
+                    log.error(f"unexpected error: {e}")
```

### Comparing `mkdocs-markmap-2.3.0/mkdocs_markmap/plugin.py` & `mkdocs-markmap-2.4.0/mkdocs_markmap/plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,139 +1,132 @@
 import logging
-from mkdocs_markmap.extension import MarkmapExtension
-import re
 from pathlib import Path
+import re
 from typing import Dict, Tuple
 
 from bs4 import BeautifulSoup, ResultSet, Tag
-from mkdocs.plugins import BasePlugin
-from mkdocs.structure.pages import Page
+
 from mkdocs.config.base import Config, load_config
 from mkdocs.config.config_options import Type as PluginType
+from mkdocs.plugins import BasePlugin
+from mkdocs.structure.pages import Page
+from mkdocs_markmap.extension import MarkmapExtension
 
 from .defaults import MARKMAP
 from .utils import download
 
 
-log = logging.getLogger('mkdocs.markmap')
+log = logging.getLogger("mkdocs.markmap")
 
 
-STATICS_PATH: Path = Path(__file__).parent / 'static_files'
-STYLE_PATH: Path = STATICS_PATH / 'mkdocs-markmap.css'
-SCRIPT_PATH: Path = STATICS_PATH / 'mkdocs-markmap.js'
+STATICS_PATH: Path = Path(__file__).parent / "static_files"
+STYLE_PATH: Path = STATICS_PATH / "mkdocs-markmap.css"
+SCRIPT_PATH: Path = STATICS_PATH / "mkdocs-markmap.js"
+
+VERSION_KEY = "{name}_version"
 
 
 class MarkmapPlugin(BasePlugin):
     """
     Plugin for markmap support
     """
     config_scheme: Tuple[Tuple[str, PluginType]] = (
         *(
-            (f'{name}_version', PluginType(str, default=module.version))
+            (VERSION_KEY.format(name=name), PluginType(str, default=module.version))
             for name, module in MARKMAP.items()
         ),
-        ('base_path', PluginType(str, default='docs')),
-        ('encoding', PluginType(str, default='utf-8')),
-        ('file_extension', PluginType(str, default='.mm.md')),
+        ("base_path", PluginType(str, default="docs")),
+        ("encoding", PluginType(str, default="utf-8")),
+        ("file_extension", PluginType(str, default=".mm.md")),
     )
 
     def __init__(self):
         self._markmap: Dict[str, str] = None
 
     @property
     def markmap(self) -> Dict[str, str]:
         """
         Provides all markmap libraries defined in mkdocs.yml (if any)
         """
-        if self._markmap is None:            
-            extra_javascript = self.config.get('extra_javascript', [])
+        if self._markmap is None:
             self._markmap: Dict[str, str] = {}
-            for uri in extra_javascript:
-                for name in MARKMAP.keys():
-                    if f'markmap-{name}' in uri.lower():
-                        self._markmap[name] = uri
-
             for name, module in MARKMAP.items():
-                if name not in self._markmap:
-                    self._markmap[name] = module.uri.format(self.config[f'{name}_version'])
+                if self.config[VERSION_KEY.format(name=name)]:
+                    self._markmap[name] = module.uri.format(self.config[VERSION_KEY.format(name=name)])
 
         return self._markmap
 
     def _load_scripts(self, soup: BeautifulSoup, script_base_url: str, js_path: Path) -> None:
         for script_url in self.markmap.values():
             if script_url.lower().startswith("http"):
                 try:
-                    src: str = script_base_url + download(js_path, script_url)
+                    src: str = script_base_url + download(js_path, script_url, extname=".js")
                 except Exception as e:
-                    log.error(f'unable to download script: {script_url}')
+                    log.error(f"unable to download script: {script_url}")
                     src = script_url
 
             else:
                 log.info(f"static script detected: {script_url}")
                 src = script_url
-            
-            script: Tag = soup.new_tag('script', src=src, type='text/javascript')
+
+            script: Tag = soup.new_tag("script", src=src, type="text/javascript")
             soup.head.append(script)
 
     @staticmethod
     def _add_statics(soup: BeautifulSoup):
         statics = (
-            (STYLE_PATH, 'style', 'text/css', 'head'),
-            (SCRIPT_PATH, 'script', 'text/javascript', 'body'),
+            (STYLE_PATH, "style", "text/css", "head"),
+            (SCRIPT_PATH, "script", "text/javascript", "body"),
         )
 
         for path, tag_name, text_type, attribute in statics:
             tag: Tag = soup.new_tag(tag_name, type=text_type)
-            with open(path, 'r') as fp:
+            with open(path, "r") as fp:
                 tag.string = fp.read()
-            getattr(soup, attribute).append(tag)    
+            getattr(soup, attribute).append(tag)
 
     def on_config(self, config: Config) -> Config:
-        config['markdown_extensions'].append('markmap')
-        config['mdx_configs']['markmap'] = {
+        config["markdown_extensions"].append("markmap")
+        config["mdx_configs"]["markmap"] = {
             key: value
-            for key, value in config['plugins'].get('markmap').config.items()
+            for key, value in config["plugins"].get("markmap").config.items()
             if key in MarkmapExtension.config_defaults
         }
-        self.config['extra_javascript'] = config.get('extra_javascript', [])
+        self.config["extra_javascript"] = config.get("extra_javascript", [])
 
         return config
 
     def on_post_page(self, html: str, page: Page, config: Config, **kwargs) -> str:
-        if not getattr(page, '_found_markmap', False):
+        if not getattr(page, "_found_markmap", False):
             log.info(f"no markmap found: {page.file.name}")
             return html
 
-        soup: BeautifulSoup = BeautifulSoup(html, 'html.parser')
-        script_base_url: str = re.sub(r'[^/]+?/', '../', re.sub(r'/+?', '/', page.url)) + 'js/'
-        js_path: Path = Path(config['site_dir']) / 'js'
+        soup: BeautifulSoup = BeautifulSoup(html, "html.parser")
+        script_base_url: str = re.sub(r"[^/]+?/", "../", re.sub(r"/+?", "/", page.url)) + "js/"
+        js_path: Path = Path(config["site_dir"]) / "js"
         self._load_scripts(soup, script_base_url, js_path)
         self._add_statics(soup)
 
         return str(soup)
 
     def on_page_content(self, html: str, page: Page, **kwargs) -> str:
-        soup: BeautifulSoup = BeautifulSoup(html, 'html.parser')
-        markmaps: ResultSet = soup.find_all(class_='language-markmap')
-        setattr(page, '_found_markmap', any(markmaps))
+        soup: BeautifulSoup = BeautifulSoup(html, "html.parser")
+        markmaps: ResultSet = soup.find_all(class_="language-markmap")
+        setattr(page, "_found_markmap", any(markmaps))
 
         for index, markmap in enumerate(markmaps):
             markmap: Tag
-            tag_id: str = f'markmap-{index}'
+            tag_id: str = f"markmap-{index}"
             pre: Tag
             code: Tag
-            if markmap.name == 'pre':
+            if markmap.name == "pre":
                 pre = markmap
-                code = markmap.findChild('code')
+                code = markmap.findChild("code")
             else:
                 pre = markmap.parent
                 code = markmap
-            pre.name = 'div'
-            pre['class'] = pre.get('class', []) + ['mkdocs-markmap']
-            pre['data-markdown'] = code.text.replace('\n', '&#10;')
-            code.replaceWith(soup.new_tag(
-                'svg', 
-                id=tag_id, 
-                attrs={'class': 'markmap'},
-            ))
+            pre.name = "div"
+            pre["class"] = pre.get("class", []) + ["mkdocs-markmap"]
+            code.name = "script"
+            code["type"] = "text/template"
 
         return str(soup)
```

### Comparing `mkdocs-markmap-2.3.0/mkdocs_markmap/utils.py` & `mkdocs-markmap-2.4.0/mkdocs_markmap/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import logging
 import os
 from pathlib import Path
-
 from urllib.parse import unquote
-from requests.adapters import HTTPAdapter
+
 from requests import Response
+from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from requests.packages.urllib3.util.url import Url, parse_url
 from requests.sessions import Session
 
 
-log = logging.getLogger('mkdocs.markmap')
+log = logging.getLogger("mkdocs.markmap")
 
 
-def download(base_path: Path, url: str, flat: bool = False, force_reload: bool = False) -> str:
+def download(base_path: Path, url: str, flat: bool = False, force_reload: bool = False, extname: str = "") -> str:
     parsed_url: Url = parse_url(url)
-    path: str = unquote(parsed_url.request_uri.split('?')[0])
-    sub_path: str = os.path.basename(path) if flat else f'{parsed_url.hostname}{path}'
+    path: str = unquote(parsed_url.request_uri.split("?")[0])
+    sub_path: str = os.path.basename(path) if flat else f"{parsed_url.hostname}{path}"
+    if extname and not sub_path.endswith(extname):
+        sub_path += extname
     file_path: Path = base_path / sub_path
 
+
     file_path.parent.mkdir(parents=True, exist_ok=True)
     if force_reload or not file_path.exists():
         retries: Retry = Retry(connect=5, read=2, redirect=5)
         adapter: HTTPAdapter = HTTPAdapter(max_retries=retries)
         http: Session = Session()
         http.mount("https://", adapter)
         http.mount("http://", adapter)
 
         response: Response = http.get(url, allow_redirects=True, timeout=3.0)
-        with open(file_path, 'wb') as fp:
+        with open(file_path, "wb") as fp:
             for chunk in response.iter_content(chunk_size=1024): 
                 if chunk:
                     fp.write(chunk)
 
-    log.info(f'script downloaded: {url}')
+    log.info(f"script downloaded: {url}")
 
     return str(sub_path)
```

### Comparing `mkdocs-markmap-2.3.0/mkdocs_markmap.egg-info/PKG-INFO` & `mkdocs-markmap-2.4.0/mkdocs_markmap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-markmap
-Version: 2.3.0
+Version: 2.4.0
 Summary: MkDocs plugin and extension to creates mindmaps from markdown using markmap
 Home-page: https://github.com/markmap/mkdocs-markmap
 Author: neatc0der
 Author-email: 
 License: MIT
 Keywords: mkdocs python markdown markmap mindmap include
 Platform: UNKNOWN
@@ -91,34 +91,35 @@
 
 ```yaml
 plugins:
   - markmap:
       base_path: docs
       encoding: utf-8
       file_extension: .mm.md
-      d3_version: 6.7.0
-      lib_version: 0.14.1
-      view_version: 0.14.0
+      d3_version: 7
+      lib_version: 0.15.3
+      view_version: 0.15.3
 ```
 
 In addition, feel free to define your favourite source urls like this:
 
 ```yaml
+plugins:
+  - markmap:
+      # disable the default assets first
+      d3_version: ''
+      lib_version: ''
+      view_version: ''
+
 extra_javascript:
-  - https://unpkg.com/d3@6.7.0/dist/d3.min.js
-  - https://unpkg.com/markmap-lib@0.14.1/dist/browser/index.min.js
-  - https://unpkg.com/markmap-view@0.14.0/dist/index.min.js
+  - https://unpkg.com/d3@7/dist/d3.min.js
+  - https://unpkg.com/markmap-lib@0.15.3/dist/browser/index.js
+  - https://unpkg.com/markmap-view@0.15.3/dist/browser/index.js
 ```
 
-:warning: The urls need to contain one of these keywords to be considered as deviation from default:
-
-* `markmap-d3`
-* `markmap-lib`
-* `markmap-view`
-
 ## Troubleshooting
 
 ### Nav tree lists markmaps
 
 1. Move your markmap files to a separate folder next to `docs`, e.g. `mindmaps`
 2. Configure `base_path` accordingly (see [Advanced Settings](#advanced-settings))
```

### Comparing `mkdocs-markmap-2.3.0/setup.py` & `mkdocs-markmap-2.4.0/setup.py`

 * *Files identical despite different names*

