# Comparing `tmp/parsuricata-0.3.3.tar.gz` & `tmp/parsuricata-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsuricata-0.3.3.tar", max compression
+gzip compressed data, was "parsuricata-0.4.0.tar", max compression
```

## Comparing `parsuricata-0.3.3.tar` & `parsuricata-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     2821 2022-07-04 18:56:16.861088 parsuricata-0.3.3/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2021-12-13 17:48:52.294931 parsuricata-0.3.3/LICENSE
--rw-r--r--   0        0        0      801 2021-12-13 17:48:52.294931 parsuricata-0.3.3/README.md
--rw-r--r--   0        0        0      190 2021-12-13 17:48:52.294931 parsuricata-0.3.3/parsuricata/__init__.py
--rw-r--r--   0        0        0     3709 2022-07-04 18:51:11.423869 parsuricata-0.3.3/parsuricata/_parser.py
--rw-r--r--   0        0        0     2904 2021-12-13 17:48:52.294931 parsuricata-0.3.3/parsuricata/rules.py
--rw-r--r--   0        0        0     2283 2022-07-04 18:22:04.077922 parsuricata-0.3.3/parsuricata/transformer.py
--rw-r--r--   0        0        0      809 2022-07-04 18:56:16.541083 parsuricata-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     6687 2022-07-04 18:51:34.704278 parsuricata-0.3.3/test_parsuricata.py
--rw-r--r--   0        0        0     1626 2022-07-04 18:56:25.541822 parsuricata-0.3.3/setup.py
--rw-r--r--   0        0        0     1647 2022-07-04 18:56:25.541998 parsuricata-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     3150 2023-08-01 20:06:52.481744 parsuricata-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2021-12-13 17:48:52.294931 parsuricata-0.4.0/LICENSE
+-rw-r--r--   0        0        0      801 2021-12-13 17:48:52.294931 parsuricata-0.4.0/README.md
+-rw-r--r--   0        0        0      190 2023-08-01 20:06:52.485745 parsuricata-0.4.0/parsuricata/__init__.py
+-rw-r--r--   0        0        0     3758 2023-08-01 20:03:42.517925 parsuricata-0.4.0/parsuricata/_parser.py
+-rw-r--r--   0        0        0     3090 2023-08-01 19:22:07.060596 parsuricata-0.4.0/parsuricata/rules.py
+-rw-r--r--   0        0        0     2397 2023-08-01 19:21:05.899553 parsuricata-0.4.0/parsuricata/transformer.py
+-rw-r--r--   0        0        0      852 2023-08-01 20:06:52.177738 parsuricata-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7751 2023-08-01 20:00:31.878069 parsuricata-0.4.0/test_parsuricata.py
+-rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 parsuricata-0.4.0/PKG-INFO
```

### Comparing `parsuricata-0.3.3/CHANGELOG.md` & `parsuricata-0.4.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
 
 
+## [0.4.0] — 2023-08-01
+### BREAKING
+ - Comma-separated settings now parsed as `Settings` tuple (previously, a `Literal` would be used, or parsing would fail, if some settings were quote-delimited strings)  [GH#15](https://github.com/theY4Kman/parsuricata/issues/15)
+
+### Added
+ - Support parsing of comma-delimited settings
+
+
 ## [0.3.3] — 2022-07-04
 ### Fixed
  - Resolve parsing failures with reduced IPv6 addresses. [GH#14](https://github.com/theY4Kman/parsuricata/issues/14)
 
 
 ## [0.3.2] — 2021-10-21
 ### Fixed
```

### Comparing `parsuricata-0.3.3/LICENSE` & `parsuricata-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parsuricata-0.3.3/README.md` & `parsuricata-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `parsuricata-0.3.3/parsuricata/_parser.py` & `parsuricata-0.4.0/parsuricata/_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,21 +77,21 @@
     // and settings, in a context-free manner.
     _COLON . 2: ":"
     _SEMICOLON . 3: ";"
 
     KEYWORD: /[a-z0-9_.\-]+/i
 
     settings: "!" settings_expr   -> negated_settings
-            | settings_expr
+            | settings_expr ("," settings_expr)*
 
-    ?settings_expr: STRING  -> string
-                  | LITERAL -> literal
+    ?settings_expr: STRING              -> string
+                  | (LITERAL | KEYWORD) -> literal
 
     STRING: /"[^\r\n]+?"(?=\s*[;])/
-    LITERAL: /(?!\s+)([^;\\"]|(?!\\)\\[;\\"])+(?=;)/
+    LITERAL: /(?!\s+)([^,;\\"]|(?!\\)\\[,;\\"])+(?=;|,)/
 '''
 
 parser = Lark(
     start='rules',
     parser='lalr',
     grammar=grammar,
     transformer=RuleTransformer(),
```

### Comparing `parsuricata-0.3.3/parsuricata/rules.py` & `parsuricata-0.4.0/parsuricata/rules.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     'RulesList',
     'Rule',
     'Option',
     'Variable',
     'String',
     'Literal',
     'Setting',
+    'Settings',
     'NegatedSetting',
     'Negated',
     'PortRange',
     'Grouping',
 ]
 
 
@@ -46,15 +47,15 @@
             body=' \\\n  '.join(str(option) for option in self.options),
         ).strip()
 
 
 @dataclass
 class Option:
     keyword: str
-    settings: 'Setting' = None
+    settings: Union['Setting', 'KeyValue'] = None
 
     def __str__(self):
         if self.settings is None:
             return f'{self.keyword};'
         else:
             return f'{self.keyword}: {self.settings!r};'
 
@@ -93,14 +94,22 @@
     def is_negated(self):
         return False
 
     def __repr__(self):
         return repr(self.orig_value)
 
 
+class Settings(tuple):
+    def __str__(self):
+        return ', '.join(str(item) for item in self)
+
+    def __repr__(self):
+        return str(self)
+
+
 class NegatedSetting(Setting):
     @property
     def is_negated(self):
         return True
 
     def __repr__(self):
         return f'!{super().__repr__()}'
```

### Comparing `parsuricata-0.3.3/parsuricata/transformer.py` & `parsuricata-0.4.0/parsuricata/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Negated,
     NegatedSetting,
     Option,
     PortRange,
     Rule,
     RulesList,
     Setting,
+    Settings,
     String,
     Variable,
 )
 
 
 class RuleTransformer(InlineTransformer):
     str = str
@@ -69,16 +70,19 @@
         if settings is not None:
             value = settings
         else:
             value = None
 
         return Option(str(keyword), value)
 
-    def settings(self, value: Any):
-        return Setting(value)
+    def settings(self, *values: Any):
+        if len(values) == 1:
+            return Setting(values[0])
+
+        return Settings(Setting(value) for value in values)
 
     def negated_settings(self, value: Any):
         return NegatedSetting(value)
 
     def variable(self, variable: Token):
         identifier = str(variable)[1:]
         return Variable(identifier)
```

### Comparing `parsuricata-0.3.3/pyproject.toml` & `parsuricata-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'parsuricata'
-version = "0.3.3"
+version = "0.4.0"
 description = 'Parse Suricata rules'
 authors = ['Zach "theY4Kman" Kanzler <they4kman@gmail.com>']
 license = 'MIT'
 packages = [
   { include = "parsuricata" },
   { include = "test_parsuricata.py", format = "sdist" },
   { include = "LICENSE", format = "sdist" },
@@ -22,10 +22,13 @@
 [tool.poetry.dependencies]
 python = '^3.6'
 lark-parser = '^0.12.0'
 
 [tool.poetry.dev-dependencies]
 pytest = '^6.2'
 
+[tool.pytest.ini_options]
+addopts = '-vv'
+
 [build-system]
 requires = ['poetry>=0.12']
 build-backend = 'poetry.masonry.api'
```

### Comparing `parsuricata-0.3.3/test_parsuricata.py` & `parsuricata-0.4.0/test_parsuricata.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from parsuricata import Option, parse_rules, Rule, Setting
+from parsuricata import Option, parse_rules, Rule, Setting, Settings
 
 
 def test_content():
     rules = parse_rules('''
         alert ip any any -> any any (content: "heymum";)
     ''')
 
@@ -65,14 +65,32 @@
 
     option = rule.options[0]
     assert option.settings == 'heymum'
     assert not option.settings.is_negated
     assert repr(option.settings) == '"heymum"'
 
 
+def test_multi_value_setting():
+    rules = parse_rules('''
+        alert ip any any -> any any ( \\
+            reference: url, "heymum"; \\
+        )
+    ''')
+
+    assert len(rules) == 1
+
+    rule = rules[0]
+    assert len(rule.options) == 1
+
+    option = rule.options[0]
+    assert isinstance(option.settings, Settings)
+    assert option.settings == ('url', 'heymum')
+    assert repr(option.settings) == 'url, heymum'
+
+
 def test_multiple_rules():
     rules = parse_rules('''
         alert ip any any -> any any (content: "a";)
         alert ip any any -> any any ( content: "b"; \\
         )
         alert ip any any -> any any ( \\
             content: "c"; \\
@@ -162,14 +180,15 @@
 alert ip any :100 -> any any ( msg:"Fart"; )
 alert ip any any -> any any ( msg:"Test rule"; tls.cert_subject; content:"CN=*.googleusercontent.com"; sid:12345678; rev:1; )
 
 # These rules come from Emerging Threats
 alert ip any any -> any any (msg:"SURICATA Applayer Mismatch protocol both directions"; flow:established; app-layer-event:applayer_mismatch_protocol_both_directions; flowint:applayer.anomaly.count,+,1; classtype:protocol-command-decode; sid:2260000; rev:1;)
 alert tcp $EXTERNAL_NET any -> $HOME_NET 445 (msg:"GPL NETBIOS SMB-DS Session Setup NTMLSSP asn1 overflow attempt"; flow:established,to_server; content:"|00|"; depth:1; content:"|FF|SMBs"; within:5; distance:3; byte_test:1,!&,128,6,relative; byte_test:4,&,2147483648,48,relative,little; content:!"NTLMSSP"; within:7; distance:54; asn1:double_overflow, bitstring_overflow, relative_offset 54, oversize_length 2048; reference:bugtraq,9633; reference:bugtraq,9635; reference:cve,2003-0818; reference:nessus,12052; reference:nessus,12065; reference:url,www.microsoft.com/technet/security/bulletin/MS04-007.mspx; classtype:protocol-command-decode; sid:2102383; rev:21; metadata:created_at 2010_09_23, updated_at 2010_09_23;)
 alert http $EXTERNAL_NET any -> $HOME_NET any (msg:"ET PHISHING Common Unhidebody Function Observed in Phishing Landing"; flow:established,to_client; file.data; content:"function unhideBody()"; nocase; fast_pattern; content:"var bodyElems = document.getElementsByTagName(|22|body|22|)|3b|"; nocase; content:"bodyElems[0].style.visibility =|20 22|visible|22 3b|"; nocase; distance:0; content:"onload=|22|unhideBody()|22|"; content:"method="; nocase; pcre:"/^["']?post/Ri"; classtype:social-engineering; sid:2029732; rev:2; metadata:affected_product Web_Browsers, attack_target Client_Endpoint, created_at 2020_03_24, deployment Perimeter, signature_severity Minor, tag Phishing, updated_at 2020_03_24;)
+alert http $HOME_NET any -> $EXTERNAL_NET any (msg:"ET EXPLOIT PHP Melody v3.0 SQL Injection Attempt"; flow:established,to_server; http.method; content:"GET"; http.uri; content:".php?vid="; content:"|2d 27 20|AND|20 28|SELECT|20|"; content:"|28|SELECT|28|SLEEP|28 5b|SLEEPTIME|5d 29 29 29 2d 2d|"; distance:9; fast_pattern; reference:url,"vulnerability-lab.com/get_content.php?id=2295"; classtype:trojan-activity; sid:2034270; rev:1; metadata:affected_product Web_Server_Applications, attack_target Web_Server, created_at 2021_10_27, deployment Perimeter, former_category EXPLOIT, signature_severity Major, updated_at 2021_10_27;)
 
 # IPv6 rules — https://github.com/theY4Kman/parsuricata/issues/14
 alert ip $HOME_NET any -> [2a00:1450:4010:0c0e:0000:0000:0000:005e] any (msg:"msg";)
 alert ip $HOME_NET any -> [2a00:1450:4010:0c0e::005e] any (msg:"msg";)
 '''
 
 EXAMPLE_RULES = [
```

### Comparing `parsuricata-0.3.3/PKG-INFO` & `parsuricata-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: parsuricata
-Version: 0.3.3
+Version: 0.4.0
 Summary: Parse Suricata rules
 Home-page: https://github.com/theY4Kman/parsuricata
 License: MIT
 Keywords: suricata,security
 Author: Zach "theY4Kman" Kanzler
 Author-email: they4kman@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lark-parser (>=0.12.0,<0.13.0)
 Project-URL: Issues, https://github.com/theY4Kman/parsuricata/issues
 Project-URL: Repository, https://github.com/theY4Kman/parsuricata
 Description-Content-Type: text/markdown
 
 # parsuricata
```

