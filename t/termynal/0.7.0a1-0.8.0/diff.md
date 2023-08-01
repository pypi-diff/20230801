# Comparing `tmp/termynal-0.7.0a1.tar.gz` & `tmp/termynal-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termynal-0.7.0a1.tar", max compression
+gzip compressed data, was "termynal-0.8.0.tar", max compression
```

## Comparing `termynal-0.7.0a1.tar` & `termynal-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1092 2023-07-31 06:23:26.184987 termynal-0.7.0a1/LICENSE
--rw-r--r--   0        0        0     1493 2023-07-31 06:23:26.184987 termynal-0.7.0a1/README.md
--rw-r--r--   0        0        0     2465 2023-07-31 06:23:26.184987 termynal-0.7.0a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-31 06:23:26.184987 termynal-0.7.0a1/termynal/__init__.py
--rw-r--r--   0        0        0     2379 2023-07-31 06:23:26.184987 termynal-0.7.0a1/termynal/assets/termynal.css
--rw-r--r--   0        0        0     9704 2023-07-31 06:23:26.184987 termynal-0.7.0a1/termynal/assets/termynal.js
--rw-r--r--   0        0        0     6498 2023-07-31 06:23:26.184987 termynal-0.7.0a1/termynal/markdown.py
--rw-r--r--   0        0        0     1121 2023-07-31 06:23:26.184987 termynal-0.7.0a1/termynal/plugin.py
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 termynal-0.7.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-08-01 06:55:12.472326 termynal-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1493 2023-08-01 06:55:12.472326 termynal-0.8.0/README.md
+-rw-r--r--   0        0        0     2461 2023-08-01 06:55:12.476326 termynal-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 06:55:12.476326 termynal-0.8.0/termynal/__init__.py
+-rw-r--r--   0        0        0     2379 2023-08-01 06:55:12.476326 termynal-0.8.0/termynal/assets/termynal.css
+-rw-r--r--   0        0        0     9704 2023-08-01 06:55:12.476326 termynal-0.8.0/termynal/assets/termynal.js
+-rw-r--r--   0        0        0     7459 2023-08-01 06:55:12.476326 termynal-0.8.0/termynal/markdown.py
+-rw-r--r--   0        0        0     1121 2023-08-01 06:55:12.476326 termynal-0.8.0/termynal/plugin.py
+-rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 termynal-0.8.0/PKG-INFO
```

### Comparing `termynal-0.7.0a1/LICENSE` & `termynal-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `termynal-0.7.0a1/README.md` & `termynal-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `termynal-0.7.0a1/pyproject.toml` & `termynal-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.0a1"
+version = "0.8.0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "termynal"
-version = "0.7.0a1"
+version = "0.8.0"
 description = ""
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/termynal"
 homepage = "https://pypi.org/project/termynal"
 keywords = []
```

### Comparing `termynal-0.7.0a1/termynal/assets/termynal.css` & `termynal-0.8.0/termynal/assets/termynal.css`

 * *Files identical despite different names*

### Comparing `termynal-0.7.0a1/termynal/assets/termynal.js` & `termynal-0.8.0/termynal/assets/termynal.js`

 * *Files identical despite different names*

### Comparing `termynal-0.7.0a1/termynal/markdown.py` & `termynal-0.8.0/termynal/markdown.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,155 +1,210 @@
 import re
-from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Tuple
+from textwrap import dedent
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Iterable,
+    List,
+    NamedTuple,
+    Optional,
+    Union,
+)
 
 from markdown.extensions import Extension
 from markdown.preprocessors import Preprocessor
 
 if TYPE_CHECKING:  # pragma:no cover
     from markdown import core
 
 
+class Command(NamedTuple):
+    prompt: str
+    lines: List[str]
+
+
+class Comment(NamedTuple):
+    lines: List[str]
+
+
+class Output(NamedTuple):
+    lines: List[str]
+
+
+class Progress:
+    def __repr__(self) -> str:  # pragma:no cover
+        return "Progress()"
+
+
+ParsedBlock = Union[Command, Comment, Output, Progress]
+
+
 def make_regex_prompts(prompt_literal_start: Iterable[str]) -> "re.Pattern[str]":
     prompt_literal_start = [re.escape(p).strip() for p in prompt_literal_start]
     prompt_to_replace = {
         ">": "&gt;",
         "<": "&lt;",
     }
-    for i, prompt in enumerate(prompt_literal_start):
-        if prompt in prompt_to_replace:
-            prompt_literal_start[i] = prompt_to_replace[prompt]
+    for p, code in prompt_to_replace.items():
+        for i, prompt in enumerate(prompt_literal_start):
+            prompt_literal_start[i] = prompt.replace(p, code)
     prompt_literal_start_re = "|".join(f"{p} " for p in prompt_literal_start)
     return re.compile(f"^({prompt_literal_start_re})")
 
 
 class Termynal:
-    progress_literal_start = "---&gt; 100%"
-    custom_literal_start = "# "
-
     def __init__(
         self,
         title: Optional[str] = None,
         prompt_literal_start: Iterable[str] = ("$",),
-        prompt_in_multiline: bool = False,
+        progress_literal_start="---&gt; 100%",
+        comment_literal_start="# ",
     ):
         self.title = title
         self.regex_prompts = make_regex_prompts(prompt_literal_start)
-        self.prompt_in_multiline = prompt_in_multiline
+        self.progress_literal_start = progress_literal_start
+        self.comment_literal_start = comment_literal_start
+
+    def parse(self, code_lines: List[str]) -> List[ParsedBlock]:
+        parsed: List[ParsedBlock] = []
+        multiline = False
+        used_prompt = None
+        prev: Optional[ParsedBlock] = None
+        for line in code_lines:
+            if match := self.regex_prompts.match(line):
+                used_prompt = match.group()
+                prev = Command(used_prompt.strip(), [line.rsplit(used_prompt)[1]])
+                parsed.append(prev)
+                multiline = bool(line.endswith("\\"))
+
+            elif multiline:
+                if prev and isinstance(prev, Command):
+                    prev.lines.append(line)
+                multiline = bool(line.endswith("\\"))
+
+            elif line.startswith(self.comment_literal_start):
+                prev = None
+                parsed.append(Comment([line]))
+
+            elif line.startswith(self.progress_literal_start):
+                prev = None
+                parsed.append(Progress())
+
+            else:
+                if prev and isinstance(prev, Output):
+                    prev.lines.append(line)
+                else:
+                    prev = Output([line])
+                    parsed.append(prev)
+
+        return parsed
 
     def convert(self, code: str) -> str:
         code_lines: List[str] = []
         if self.title is not None:
             code_lines.append(
                 f'<div class="termy" data-termynal data-ty-title="{self.title}">',
             )
         else:
             code_lines.append('<div class="termy">')
-        multiline = False
-        used_prompt = None
-        for line in code.split("\n"):
-            if match := self.regex_prompts.match(line):
-                used_prompt = match.group()
-                code_lines.append(
-                    f'<span data-ty="input" data-ty-prompt="{used_prompt.strip()}">'
-                    f"{line.rsplit(used_prompt)[1]}</span>",
-                )
-                multiline = bool(line.endswith("\\"))
-            elif multiline:
-                used_prompt = used_prompt or ""
-                if not self.prompt_in_multiline:
-                    used_prompt = ""
+
+        for block in self.parse(code.split("\n")):
+            if isinstance(block, Command):
+                lines = "\n".join(block.lines)
                 code_lines.append(
-                    f'<span data-ty="input" data-ty-prompt="{used_prompt.strip()}">'
-                    f"{line}</span>",
+                    f'<span data-ty="input" data-ty-prompt="{block.prompt}">'
+                    f"{lines}</span>",
                 )
-                multiline = bool(line.endswith("\\"))
 
-            elif line.startswith(self.custom_literal_start):
+            elif isinstance(block, Comment):
+                lines = "\n".join(block.lines)
                 code_lines.append(
-                    f'<span class="termynal-comment" data-ty>{line}</span>',
+                    f'<span class="termynal-comment" data-ty>{lines}</span>',
                 )
-            elif line.startswith(self.progress_literal_start):
+
+            elif isinstance(block, Progress):
                 code_lines.append('<span data-ty="progress"></span>')
-            else:
-                code_lines.append(f"<span data-ty>{line}</span>")
+
+            elif isinstance(block, Output):
+                lines = "<br>".join(block.lines)
+                code_lines.append(f"<span data-ty>{lines}</span>")
+
         code_lines.append("</div>")
-        return "\n".join(code_lines)
+        return "".join(code_lines)
 
 
 class TermynalPreprocessor(Preprocessor):
-    rexep = re.compile("(<code.*>)((.|\n)*?)(</code>)")
-    comment = "<!-- termynal -->"
-    language_class = 'class="language-console"'
+    ty_comment = "<!-- termynal -->"
+    marker = "9HDrdgVBNLga"
+    FENCED_BLOCK_RE = re.compile(
+        dedent(
+            r"""
+            (?P<fence>^(?:~{3,}|`{3,}))[ ]*   # opening fence
+            ((\{(?P<attrs>[^\}\n]*)\})|       # (optional {attrs} or
+            (\.?(?P<lang>[\w#.+-]*)[ ]*)?     # optional (.)lang
+            (hl_lines=(?P<quot>"|')           # optional hl_lines)
+            (?P<hl_lines>.*?)(?P=quot)[ ]*)?)
+            \n                                # newline (end of opening fence)
+            (?P<code>.*?)(?<=\n)              # the code block
+            (?P=fence)[ ]*$                   # closing fence
+        """,
+        ),
+        re.MULTILINE | re.DOTALL | re.VERBOSE,
+    )
 
     def __init__(self, config: Dict[str, Any], md: "core.Markdown"):
         self.title = config.get("title", None)
         self.prompt_literal_start = config.get("prompt_literal_start", ("$ ",))
-        self.prompt_in_multiline = config.get("prompt_in_multiline", False)
 
         super(TermynalPreprocessor, self).__init__(md=md)
 
     def run(self, lines: List[str]) -> List[str]:
-        content_by_placeholder = {}
-        for i in range(self.md.htmlStash.html_counter):
-            placeholder = self.md.htmlStash.get_placeholder(i)
-            content = self.md.htmlStash.rawHtmlBlocks[i]
-            content_by_placeholder[placeholder] = (content, i)
-
-        target_code_by_placeholder = self._get_lines(lines, content_by_placeholder)
-
-        new_lines = []
-        for line in lines:
-            if line in target_code_by_placeholder:
-                new_lines.append(target_code_by_placeholder[line])
+        placeholder_i = 0
+        text = "\n".join(lines)
+        store = {}
+        while 1:
+            m = self.FENCED_BLOCK_RE.search(text)
+            if m:
+                code = m.group("code")
+                placeholder = f"{self.marker}-{placeholder_i}"
+                placeholder_i += 1
+                store[placeholder] = (code, text[m.start() : m.end()])
+                text = f"{text[:m.start()]}\n{placeholder}\n{text[m.end():]}"
             else:
-                new_lines.append(line)
+                break
 
-        return new_lines
-
-    def _get_lines(
-        self,
-        lines: List[str],
-        content_by_placeholder: Dict[str, Tuple[str, int]],
-    ) -> Dict[str, str]:  # pylint:disable=too-many-nested-blocks
-        termynal_obj = Termynal(
+        termynal = Termynal(
             title=self.title,
             prompt_literal_start=self.prompt_literal_start,
-            prompt_in_multiline=self.prompt_in_multiline,
         )
-        lines_by_placeholder = {}
-        is_termynal_code = False
-        for line in lines:
-            if line in content_by_placeholder:
-                (content, i) = content_by_placeholder[line]
-
-                if not isinstance(content, str):
-                    continue
-
-                if content.startswith(self.comment):
-                    is_termynal_code = True
-                    continue
-
-                matches = self.rexep.search(content)
-                if not matches:
-                    continue
-
-                if self.language_class in matches.group(1):
-                    is_termynal_code = True
-
-                if not is_termynal_code:
-                    continue
-
-                is_termynal_code = False
-                content = matches.group(2)
-                target_code = termynal_obj.convert(code=content)
-                if target_code:
-                    self.md.htmlStash.rawHtmlBlocks[i] = ""
-                    lines_by_placeholder[line] = target_code
 
-        return lines_by_placeholder
+        new_lines: List[str] = []
+        is_ty_code = False
+        for line in text.split("\n"):
+            if line.startswith(self.ty_comment):
+                is_ty_code = True
+                continue
+
+            if is_ty_code and line in store:
+                new_lines.append(termynal.convert(self._escape(store[line][0])))
+                is_ty_code = False
+            elif line in store:
+                new_lines.append(store[line][1])
+            else:
+                new_lines.append(line)
+
+        return new_lines
+
+    def _escape(self, txt: str) -> str:
+        txt = txt.replace("&", "&amp;")
+        txt = txt.replace("<", "&lt;")
+        txt = txt.replace(">", "&gt;")
+        txt = txt.replace('"', "&quot;")
+        return txt  # noqa:RET504
 
 
 class TermynalExtension(Extension):
     def __init__(self, *args: Any, **kwargs: Any):
         self.config = {
             "title": [
                 "bash",
@@ -158,27 +213,23 @@
             "prompt_literal_start": [
                 [
                     "$",
                 ],
                 "A list of prompt characters start to consider as console - "
                 "Default: ['$']",
             ],
-            "prompt_in_multiline": [
-                False,
-                "Default: False",
-            ],
         }
 
         super(TermynalExtension, self).__init__(*args, **kwargs)
 
     def extendMarkdown(self, md: "core.Markdown") -> None:  # noqa:N802
         """Register the extension."""
         md.registerExtension(self)
         config = self.getConfigs()
-        md.preprocessors.register(TermynalPreprocessor(config, md), "termynal", 20)
+        md.preprocessors.register(TermynalPreprocessor(config, md), "termynal", 35)
 
 
 def makeExtension(  # noqa:N802  # pylint:disable=invalid-name
     *args: Any,
     **kwargs: Any,
 ) -> TermynalExtension:
     """Return extension."""
```

### Comparing `termynal-0.7.0a1/termynal/plugin.py` & `termynal-0.8.0/termynal/plugin.py`

 * *Files identical despite different names*

### Comparing `termynal-0.7.0a1/PKG-INFO` & `termynal-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termynal
-Version: 0.7.0a1
+Version: 0.8.0
 Summary: 
 Home-page: https://pypi.org/project/termynal
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

