# Comparing `tmp/termynal-0.8.0.tar.gz` & `tmp/termynal-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termynal-0.8.0.tar", max compression
+gzip compressed data, was "termynal-0.9.0.tar", max compression
```

## Comparing `termynal-0.8.0.tar` & `termynal-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1092 2023-08-01 06:55:12.472326 termynal-0.8.0/LICENSE
--rw-r--r--   0        0        0     1493 2023-08-01 06:55:12.472326 termynal-0.8.0/README.md
--rw-r--r--   0        0        0     2461 2023-08-01 06:55:12.476326 termynal-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 06:55:12.476326 termynal-0.8.0/termynal/__init__.py
--rw-r--r--   0        0        0     2379 2023-08-01 06:55:12.476326 termynal-0.8.0/termynal/assets/termynal.css
--rw-r--r--   0        0        0     9704 2023-08-01 06:55:12.476326 termynal-0.8.0/termynal/assets/termynal.js
--rw-r--r--   0        0        0     7459 2023-08-01 06:55:12.476326 termynal-0.8.0/termynal/markdown.py
--rw-r--r--   0        0        0     1121 2023-08-01 06:55:12.476326 termynal-0.8.0/termynal/plugin.py
--rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 termynal-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-08-01 21:33:52.029230 termynal-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1493 2023-08-01 21:33:52.029230 termynal-0.9.0/README.md
+-rw-r--r--   0        0        0     2704 2023-08-01 21:33:52.029230 termynal-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 21:33:52.029230 termynal-0.9.0/termynal/__init__.py
+-rw-r--r--   0        0        0     2379 2023-08-01 21:33:52.029230 termynal-0.9.0/termynal/assets/termynal.css
+-rw-r--r--   0        0        0     9704 2023-08-01 21:33:52.029230 termynal-0.9.0/termynal/assets/termynal.js
+-rw-r--r--   0        0        0     8077 2023-08-01 21:33:52.029230 termynal-0.9.0/termynal/markdown.py
+-rw-r--r--   0        0        0     1085 2023-08-01 21:33:52.029230 termynal-0.9.0/termynal/plugin.py
+-rw-r--r--   0        0        0     2379 1970-01-01 00:00:00.000000 termynal-0.9.0/PKG-INFO
```

### Comparing `termynal-0.8.0/LICENSE` & `termynal-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `termynal-0.8.0/README.md` & `termynal-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `termynal-0.8.0/pyproject.toml` & `termynal-0.9.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.8.0"
+version = "0.9.0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "termynal"
-version = "0.8.0"
-description = ""
+version = "0.9.0"
+description = "A lightweight and modern animated terminal window"
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/termynal"
-homepage = "https://pypi.org/project/termynal"
-keywords = []
+homepage = "https://daxartio.github.io/termynal/"
+documentation = "https://daxartio.github.io/termynal/"
+keywords = ["mkdocs", "markdown", "plugin"]
+
+[tool.poetry.urls]
+Changelog = "https://daxartio.github.io/termynal/changelog/"
 
 [tool.poetry.plugins."mkdocs.plugins"]
 "termynal" = "termynal.plugin:TermynalPlugin"
 
 [tool.poetry.plugins."markdown.extensions"]
 "termynal" = "termynal.markdown:TermynalExtension"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 markdown = "*"
 mkdocs = {version = "^1.4", optional = true}
 
 [tool.poetry.group.dev.dependencies]
-black = "*"
-mypy = "*"
-pytest = "*"
-pytest-asyncio = "*"
-pytest-cov = "*"
-pytest-deadfixtures = "*"
-pytest-mock = "*"
+black = ">=23.7.0"
+mypy = "^1.4.1"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+pytest-deadfixtures = "^2.2.1"
+pytest-mock = "^3.11.1"
 pyyaml = "^6.0.1"
-ruff = "*"
-toml = "*"
-types-Markdown = "*"
+ruff = "^0.0.282"
+types-Markdown = "^3.4.2.10"
 types-pyyaml = "^6.0.12.11"
 
 [tool.poetry.group.docs.dependencies]
 markdown-include = "^0.8.1"
-mkdocs = "*"
-mkdocs-material = "*"
+mkdocs = "^1.4"
+mkdocs-material = "^9.1.21"
 
 [tool.poetry.group.git.dependencies]
 commitizen = "^3.5.3"
 
 [tool.poetry.extras]
 mkdocs = ["mkdocs"]
```

### Comparing `termynal-0.8.0/termynal/assets/termynal.css` & `termynal-0.9.0/termynal/assets/termynal.css`

 * *Files identical despite different names*

### Comparing `termynal-0.8.0/termynal/assets/termynal.js` & `termynal-0.9.0/termynal/assets/termynal.js`

 * *Files identical despite different names*

### Comparing `termynal-0.8.0/termynal/markdown.py` & `termynal-0.9.0/termynal/markdown.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,21 +7,28 @@
     Iterable,
     List,
     NamedTuple,
     Optional,
     Union,
 )
 
+import yaml
+import yaml.parser
 from markdown.extensions import Extension
 from markdown.preprocessors import Preprocessor
 
 if TYPE_CHECKING:  # pragma:no cover
     from markdown import core
 
 
+class Config(NamedTuple):
+    title: str
+    prompt_literal_start: Iterable[str]
+
+
 class Command(NamedTuple):
     prompt: str
     lines: List[str]
 
 
 class Comment(NamedTuple):
     lines: List[str]
@@ -48,24 +55,42 @@
     for p, code in prompt_to_replace.items():
         for i, prompt in enumerate(prompt_literal_start):
             prompt_literal_start[i] = prompt.replace(p, code)
     prompt_literal_start_re = "|".join(f"{p} " for p in prompt_literal_start)
     return re.compile(f"^({prompt_literal_start_re})")
 
 
+def parse_config(raw: str) -> Optional[Config]:
+    try:
+        config = yaml.full_load(raw)
+    except yaml.parser.ParserError:
+        return None
+
+    if not isinstance(config, dict):
+        return None
+
+    return parse_config_from_dict(config)
+
+
+def parse_config_from_dict(config: Dict[str, Any]) -> Config:
+    return Config(
+        title=str(config.get("title", "bash")),
+        prompt_literal_start=list(config.get("prompt_literal_start", ("$",))),
+    )
+
+
 class Termynal:
     def __init__(
         self,
-        title: Optional[str] = None,
-        prompt_literal_start: Iterable[str] = ("$",),
+        config: Config,
         progress_literal_start="---&gt; 100%",
         comment_literal_start="# ",
     ):
-        self.title = title
-        self.regex_prompts = make_regex_prompts(prompt_literal_start)
+        self.config = config
+        self.regex_prompts = make_regex_prompts(config.prompt_literal_start)
         self.progress_literal_start = progress_literal_start
         self.comment_literal_start = comment_literal_start
 
     def parse(self, code_lines: List[str]) -> List[ParsedBlock]:
         parsed: List[ParsedBlock] = []
         multiline = False
         used_prompt = None
@@ -86,31 +111,27 @@
                 prev = None
                 parsed.append(Comment([line]))
 
             elif line.startswith(self.progress_literal_start):
                 prev = None
                 parsed.append(Progress())
 
+            elif prev and isinstance(prev, Output):
+                prev.lines.append(line)
             else:
-                if prev and isinstance(prev, Output):
-                    prev.lines.append(line)
-                else:
-                    prev = Output([line])
-                    parsed.append(prev)
+                prev = Output([line])
+                parsed.append(prev)
 
         return parsed
 
     def convert(self, code: str) -> str:
         code_lines: List[str] = []
-        if self.title is not None:
-            code_lines.append(
-                f'<div class="termy" data-termynal data-ty-title="{self.title}">',
-            )
-        else:
-            code_lines.append('<div class="termy">')
+        code_lines.append(
+            f'<div class="termy" data-termynal data-ty-title="{self.config.title}">',
+        )
 
         for block in self.parse(code.split("\n")):
             if isinstance(block, Command):
                 lines = "\n".join(block.lines)
                 code_lines.append(
                     f'<span data-ty="input" data-ty-prompt="{block.prompt}">'
                     f"{lines}</span>",
@@ -130,15 +151,15 @@
                 code_lines.append(f"<span data-ty>{lines}</span>")
 
         code_lines.append("</div>")
         return "".join(code_lines)
 
 
 class TermynalPreprocessor(Preprocessor):
-    ty_comment = "<!-- termynal -->"
+    ty_comment = re.compile(r"<!--\s*termynal:?(.*)-->")
     marker = "9HDrdgVBNLga"
     FENCED_BLOCK_RE = re.compile(
         dedent(
             r"""
             (?P<fence>^(?:~{3,}|`{3,}))[ ]*   # opening fence
             ((\{(?P<attrs>[^\}\n]*)\})|       # (optional {attrs} or
             (\.?(?P<lang>[\w#.+-]*)[ ]*)?     # optional (.)lang
@@ -148,19 +169,17 @@
             (?P<code>.*?)(?<=\n)              # the code block
             (?P=fence)[ ]*$                   # closing fence
         """,
         ),
         re.MULTILINE | re.DOTALL | re.VERBOSE,
     )
 
-    def __init__(self, config: Dict[str, Any], md: "core.Markdown"):
-        self.title = config.get("title", None)
-        self.prompt_literal_start = config.get("prompt_literal_start", ("$ ",))
-
+    def __init__(self, config: Config, md: "core.Markdown"):
         super(TermynalPreprocessor, self).__init__(md=md)
+        self.config = config
 
     def run(self, lines: List[str]) -> List[str]:
         placeholder_i = 0
         text = "\n".join(lines)
         store = {}
         while 1:
             m = self.FENCED_BLOCK_RE.search(text)
@@ -169,28 +188,33 @@
                 placeholder = f"{self.marker}-{placeholder_i}"
                 placeholder_i += 1
                 store[placeholder] = (code, text[m.start() : m.end()])
                 text = f"{text[:m.start()]}\n{placeholder}\n{text[m.end():]}"
             else:
                 break
 
-        termynal = Termynal(
-            title=self.title,
-            prompt_literal_start=self.prompt_literal_start,
-        )
+        default_termynal = Termynal(self.config)
+        termynal = default_termynal
 
         new_lines: List[str] = []
         is_ty_code = False
         for line in text.split("\n"):
-            if line.startswith(self.ty_comment):
+            ty_match = self.ty_comment.match(line)
+            if ty_match:
+                configs_raw = ty_match.group(1)
+                if configs_raw and configs_raw.strip():
+                    config = parse_config(configs_raw)
+                    if config:
+                        termynal = Termynal(config)
                 is_ty_code = True
                 continue
 
             if is_ty_code and line in store:
                 new_lines.append(termynal.convert(self._escape(store[line][0])))
+                termynal = default_termynal
                 is_ty_code = False
             elif line in store:
                 new_lines.append(store[line][1])
             else:
                 new_lines.append(line)
 
         return new_lines
@@ -220,15 +244,16 @@
         }
 
         super(TermynalExtension, self).__init__(*args, **kwargs)
 
     def extendMarkdown(self, md: "core.Markdown") -> None:  # noqa:N802
         """Register the extension."""
         md.registerExtension(self)
-        config = self.getConfigs()
+        md_config = self.getConfigs()
+        config = parse_config_from_dict(md_config)
         md.preprocessors.register(TermynalPreprocessor(config, md), "termynal", 35)
 
 
 def makeExtension(  # noqa:N802  # pylint:disable=invalid-name
     *args: Any,
     **kwargs: Any,
 ) -> TermynalExtension:
```

### Comparing `termynal-0.8.0/termynal/plugin.py` & `termynal-0.9.0/termynal/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional
 
 from mkdocs import utils
 from mkdocs.plugins import BasePlugin
 
 if TYPE_CHECKING:  # pragma:no cover
-    from mkdocs.config.base import Config
     from mkdocs.config.defaults import MkDocsConfig
 
 base_path = Path(__file__).parent
 
 
 class TermynalPlugin(BasePlugin):
-    def on_config(self, config: "MkDocsConfig") -> Optional["Config"]:
+    def on_config(self, config: "MkDocsConfig") -> Optional["MkDocsConfig"]:
         if "termynal.css" not in config["extra_css"]:
             config["extra_css"].append("termynal.css")
 
         if "termynal.js" not in config["extra_javascript"]:
             config["extra_javascript"].append("termynal.js")
 
         if "termynal" not in config["markdown_extensions"]:
```

### Comparing `termynal-0.8.0/PKG-INFO` & `termynal-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: termynal
-Version: 0.8.0
-Summary: 
-Home-page: https://pypi.org/project/termynal
+Version: 0.9.0
+Summary: A lightweight and modern animated terminal window
+Home-page: https://daxartio.github.io/termynal/
 License: MIT
+Keywords: mkdocs,markdown,plugin
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: mkdocs
 Requires-Dist: markdown
 Requires-Dist: mkdocs (>=1.4,<2.0) ; extra == "mkdocs"
+Project-URL: Changelog, https://daxartio.github.io/termynal/changelog/
+Project-URL: Documentation, https://daxartio.github.io/termynal/
 Project-URL: Repository, https://github.com/daxartio/termynal
 Description-Content-Type: text/markdown
 
 # Termynal
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/daxartio/termynal/check.yml)
 [![PyPI](https://img.shields.io/pypi/v/termynal)](https://pypi.org/project/termynal/)
```

