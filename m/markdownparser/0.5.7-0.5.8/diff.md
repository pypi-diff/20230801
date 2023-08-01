# Comparing `tmp/markdownparser-0.5.7.tar.gz` & `tmp/markdownparser-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdownparser-0.5.7.tar", max compression
+gzip compressed data, was "markdownparser-0.5.8.tar", max compression
```

## Comparing `markdownparser-0.5.7.tar` & `markdownparser-0.5.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.7/LICENSE
--rw-r--r--   0        0        0      123 2023-07-29 05:45:52.175866 markdownparser-0.5.7/MarkdownParser/__init__.py
--rw-r--r--   0        0        0     5969 2023-07-29 05:13:27.554441 markdownparser-0.5.7/MarkdownParser/base_class.py
--rw-r--r--   0        0        0    24817 2023-07-30 04:41:41.634269 markdownparser-0.5.7/MarkdownParser/block_parser.py
--rw-r--r--   0        0        0     7072 2023-07-29 05:12:59.301866 markdownparser-0.5.7/MarkdownParser/core.py
--rw-r--r--   0        0        0     3285 2023-07-29 04:08:11.133670 markdownparser-0.5.7/MarkdownParser/preprocess_parser.py
--rw-r--r--   0        0        0    21736 2023-07-29 04:08:19.718060 markdownparser-0.5.7/MarkdownParser/tree_parser.py
--rw-r--r--   0        0        0      442 2023-07-30 04:45:34.051146 markdownparser-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     4863 2023-07-29 15:49:46.355196 markdownparser-0.5.7/README.md
--rw-r--r--   0        0        0     5636 1970-01-01 00:00:00.000000 markdownparser-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.8/LICENSE
+-rw-r--r--   0        0        0      123 2023-07-29 05:45:52.175866 markdownparser-0.5.8/MarkdownParser/__init__.py
+-rw-r--r--   0        0        0     5969 2023-07-29 05:13:27.554441 markdownparser-0.5.8/MarkdownParser/base_class.py
+-rw-r--r--   0        0        0    24841 2023-08-01 01:26:27.149482 markdownparser-0.5.8/MarkdownParser/block_parser.py
+-rw-r--r--   0        0        0     7072 2023-07-29 05:12:59.301866 markdownparser-0.5.8/MarkdownParser/core.py
+-rw-r--r--   0        0        0     3285 2023-07-29 04:08:11.133670 markdownparser-0.5.8/MarkdownParser/preprocess_parser.py
+-rw-r--r--   0        0        0    21736 2023-07-29 04:08:19.718060 markdownparser-0.5.8/MarkdownParser/tree_parser.py
+-rw-r--r--   0        0        0      442 2023-08-01 01:27:20.327866 markdownparser-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     4862 2023-07-30 04:45:57.984577 markdownparser-0.5.8/README.md
+-rw-r--r--   0        0        0     5635 1970-01-01 00:00:00.000000 markdownparser-0.5.8/PKG-INFO
```

### Comparing `markdownparser-0.5.7/LICENSE` & `markdownparser-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.7/MarkdownParser/base_class.py` & `markdownparser-0.5.8/MarkdownParser/base_class.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.7/MarkdownParser/block_parser.py` & `markdownparser-0.5.8/MarkdownParser/block_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -593,17 +593,17 @@
     # 处理特殊字符
     # 不考虑 * 的多级嵌套
 
     def __init__(self) -> None:
         super().__init__()
         self.RE = re.compile(
             r"""(
-            \*{3}(.+?)\*{3}|                           # 粗体+斜体
-            \*{2}(.+?)\*{2}|                           # 粗体
-            \*(.+?)\*|                                 # 斜体
+            \*{3}[^ ](.+?)[^ ]\*{3}|                           # 粗体+斜体
+            \*{2}[^ ](.+?)[^ ]\*{2}|                           # 粗体
+            \*[^ ](.+?)[^ ]\*|                                 # 斜体
             ~~(.+?)~~|                                 # 删除线
             ``(.+?)``|                                 # 高亮
             `(.+?)`                                    # 高亮
         )""",
             re.VERBOSE,
         )
         self.groupid_tag = {
```

### Comparing `markdownparser-0.5.7/MarkdownParser/core.py` & `markdownparser-0.5.8/MarkdownParser/core.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.7/MarkdownParser/preprocess_parser.py` & `markdownparser-0.5.8/MarkdownParser/preprocess_parser.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.7/MarkdownParser/tree_parser.py` & `markdownparser-0.5.8/MarkdownParser/tree_parser.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.7/README.md` & `markdownparser-0.5.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 - Setext 形式的标题
 - 上标 / 下标 / 下划线
 - `<details><summary></summary></details>` 折叠块
 
 ## HTML 结果说明
 
 - 生成的结果如下 `<div class='markdown-body'>markdown内容</div>`
-- 代码段会根据语言为 code 加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`
+- 代码段会根据语言为 pre 加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`
 - 默认导出的HTML中层级任务列表会有显示问题,这是因为使用了ul+li+checkbox的方式,您需要添加以下css样式修正
 
   ```css
   .markdown-body > ul>li:has(input) {
     padding-left: 0;
     margin-bottom: 0;
   }
```

#### html2text {}

```diff
@@ -23,17 +23,16 @@
 (lines) # éè¡è§£æ,å¾å°ä¸é¢æªä¼åçæ  root = self.block_parser
 (lines) # root.info() # ä¼å,å¾å°æ­£ç¡®çmarkdownè§£ææ  tree =
 self.tree_parser(root) # tree.info() # è¾åºå°å±å¹ / å¯¼åºhtmlæä»¶
 return tree.toHTML() ``` ## ä¸æ¯æ - åä¸ªç©ºæ ¼åä¸ºä»£ç æ®µ -
 [^1]çå¼ç¨æ¹å¼ - Setext å½¢å¼çæ é¢ - ä¸æ  / ä¸æ  / ä¸åçº¿ - ``
 æå å ## HTML ç»æè¯´æ - çæçç»æå¦ä¸ `
 markdownåå®¹
-` - ä»£ç æ®µä¼æ ¹æ®è¯­è¨ä¸º code
-å å¥ä¸ä¸ªç±»åä¾¿äºåæé«äº®,ä¾å¦ `class="language-cpp"`,
-æªå®ä¹è¯­è¨åä¸º `language-UNKNOWN` -
+` - ä»£ç æ®µä¼æ ¹æ®è¯­è¨ä¸º pre å å¥ä¸ä¸ªç±»åä¾¿äºåæé«äº®,ä¾å¦
+`class="language-cpp"`, æªå®ä¹è¯­è¨åä¸º `language-UNKNOWN` -
 é»è®¤å¯¼åºçHTMLä¸­å±çº§ä»»å¡åè¡¨ä¼ææ¾ç¤ºé®é¢,è¿æ¯å ä¸ºä½¿ç¨äºul+li+checkboxçæ¹å¼,æ¨éè¦æ·»å ä»¥ä¸cssæ ·å¼ä¿®æ­£
 ```css .markdown-body > ul>li:has(input) { padding-left: 0; margin-bottom: 0; }
 .markdown-body ul>li:has(input)>ul { list-style-type: none; padding-left: 8px;
 } ``` - æ¨å¯ä»¥ä½¿ç¨ `parse_toc` å° HashHeadBlock
 æååºæ¥ç»æç®å½æ , å¾å°ä¸ä¸ª `
 ...
 ` å¹¶æ·»å å°è¿åç HTML åç´ ä¸­, æ¨å¯è½è¿éè¦ä¸äº js
```

### Comparing `markdownparser-0.5.7/PKG-INFO` & `markdownparser-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdownparser
-Version: 0.5.7
+Version: 0.5.8
 Summary: 
 Home-page: https://github.com/luzhixing12345/MarkdownParser
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -103,15 +103,15 @@
 - Setext 形式的标题
 - 上标 / 下标 / 下划线
 - `<details><summary></summary></details>` 折叠块
 
 ## HTML 结果说明
 
 - 生成的结果如下 `<div class='markdown-body'>markdown内容</div>`
-- 代码段会根据语言为 code 加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`
+- 代码段会根据语言为 pre 加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`
 - 默认导出的HTML中层级任务列表会有显示问题,这是因为使用了ul+li+checkbox的方式,您需要添加以下css样式修正
 
   ```css
   .markdown-body > ul>li:has(input) {
     padding-left: 0;
     margin-bottom: 0;
   }
```

