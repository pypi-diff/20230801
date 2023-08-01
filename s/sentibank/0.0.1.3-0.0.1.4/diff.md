# Comparing `tmp/sentibank-0.0.1.3.tar.gz` & `tmp/sentibank-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentibank-0.0.1.3.tar", last modified: Mon Jul 31 17:34:32 2023, max compression
+gzip compressed data, was "sentibank-0.0.1.4.tar", last modified: Tue Aug  1 18:48:18 2023, max compression
```

## Comparing `sentibank-0.0.1.3.tar` & `sentibank-0.0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.791133 sentibank-0.0.1.3/
--rw-rw-rw-   0        0        0     1084 2023-07-31 16:51:12.000000 sentibank-0.0.1.3/LICENSE
--rw-rw-rw-   0        0        0       40 2023-07-31 16:54:25.000000 sentibank-0.0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      416 2023-07-31 17:34:32.791133 sentibank-0.0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       99 2023-07-31 16:51:12.000000 sentibank-0.0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.756132 sentibank-0.0.1.3/sentibank/
--rw-rw-rw-   0        0        0        0 2023-07-31 17:01:20.000000 sentibank-0.0.1.3/sentibank/__init__.py
--rw-rw-rw-   0        0        0     2566 2023-07-31 17:07:44.000000 sentibank-0.0.1.3/sentibank/archive.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.770131 sentibank-0.0.1.3/sentibank/dict_arXiv/
-drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.772131 sentibank-0.0.1.3/sentibank/dict_arXiv/AFINN/
--rw-rw-rw-   0        0        0    42865 2023-07-25 14:30:20.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/AFINN/AFINN_v2015.csv
--rw-rw-rw-   0        0        0    60808 2023-07-16 07:07:32.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/AFINN/AFINN_v2015.pickle
-drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.774131 sentibank-0.0.1.3/sentibank/dict_arXiv/Aigents/
--rw-rw-rw-   0        0        0   291231 2023-07-25 14:32:19.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/Aigents/Aigents+_v2022.csv
--rw-rw-rw-   0        0        0   218491 2023-07-25 14:28:33.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/Aigents/Aigents+_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.787142 sentibank-0.0.1.3/sentibank/dict_arXiv/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/MASTER/MASTER_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.790143 sentibank-0.0.1.3/sentibank/dict_arXiv/VADER/
--rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/VADER/VADER_v2014.csv
--rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/VADER/VADER_v2014_mod.pickle
--rw-rw-rw-   0        0        0     3071 2023-07-25 14:11:12.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/emos.py
--rw-rw-rw-   0        0        0     9291 2023-07-31 17:20:48.000000 sentibank-0.0.1.3/sentibank/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.769132 sentibank-0.0.1.3/sentibank.egg-info/
--rw-rw-rw-   0        0        0      416 2023-07-31 17:34:32.000000 sentibank-0.0.1.3/sentibank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2023-07-31 17:34:32.000000 sentibank-0.0.1.3/sentibank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 17:34:32.000000 sentibank-0.0.1.3/sentibank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-31 17:34:32.000000 sentibank-0.0.1.3/sentibank.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 17:34:32.000000 sentibank-0.0.1.3/sentibank.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-31 17:34:32.792143 sentibank-0.0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-07-31 17:34:20.000000 sentibank-0.0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 18:48:18.417466 sentibank-0.0.1.4/
+-rw-rw-rw-   0        0        0     1084 2023-07-31 16:51:12.000000 sentibank-0.0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       40 2023-07-31 16:54:25.000000 sentibank-0.0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      473 2023-08-01 18:48:18.417466 sentibank-0.0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2023-07-31 16:51:12.000000 sentibank-0.0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 18:48:18.269041 sentibank-0.0.1.4/sentibank/
+-rw-rw-rw-   0        0        0        0 2023-07-31 17:01:20.000000 sentibank-0.0.1.4/sentibank/__init__.py
+-rw-rw-rw-   0        0        0     2671 2023-08-01 18:42:28.000000 sentibank-0.0.1.4/sentibank/archive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 18:48:18.306990 sentibank-0.0.1.4/sentibank/dict_arXiv/
+drwxrwxrwx   0        0        0        0 2023-08-01 18:48:18.325930 sentibank-0.0.1.4/sentibank/dict_arXiv/AFINN/
+-rw-rw-rw-   0        0        0    42865 2023-07-25 14:30:20.000000 sentibank-0.0.1.4/sentibank/dict_arXiv/AFINN/AFINN_v2015.csv
+-rw-rw-rw-   0        0        0    60808 2023-07-16 07:07:32.000000 sentibank-0.0.1.4/sentibank/dict_arXiv/AFINN/AFINN_v2015.pickle
+drwxrwxrwx   0        0        0        0 2023-08-01 18:48:18.349012 sentibank-0.0.1.4/sentibank/dict_arXiv/Aigents/
+-rw-rw-rw-   0        0        0   291231 2023-07-25 14:32:19.000000 sentibank-0.0.1.4/sentibank/dict_arXiv/Aigents/Aigents+_v2022.csv
+-rw-rw-rw-   0        0        0   218491 2023-07-25 14:28:33.000000 sentibank-0.0.1.4/sentibank/dict_arXiv/Aigents/Aigents+_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-08-01 18:48:18.398446 sentibank-0.0.1.4/sentibank/dict_arXiv/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 sentibank-0.0.1.4/sentibank/dict_arXiv/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 sentibank-0.0.1.4/sentibank/dict_arXiv/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-08-01 18:48:18.415474 sentibank-0.0.1.4/sentibank/dict_arXiv/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 sentibank-0.0.1.4/sentibank/dict_arXiv/VADER/VADER_v2014.csv
+-rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 sentibank-0.0.1.4/sentibank/dict_arXiv/VADER/VADER_v2014_mod.pickle
+-rw-rw-rw-   0        0        0     3071 2023-07-25 14:11:12.000000 sentibank-0.0.1.4/sentibank/dict_arXiv/emos.py
+-rw-rw-rw-   0        0        0    10044 2023-08-01 18:42:15.000000 sentibank-0.0.1.4/sentibank/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 18:48:18.305022 sentibank-0.0.1.4/sentibank.egg-info/
+-rw-rw-rw-   0        0        0      473 2023-08-01 18:48:17.000000 sentibank-0.0.1.4/sentibank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2023-08-01 18:48:18.000000 sentibank-0.0.1.4/sentibank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 18:48:17.000000 sentibank-0.0.1.4/sentibank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-08-01 18:48:17.000000 sentibank-0.0.1.4/sentibank.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 18:48:17.000000 sentibank-0.0.1.4/sentibank.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-01 18:48:18.422756 sentibank-0.0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-08-01 18:48:02.000000 sentibank-0.0.1.4/setup.py
```

### Comparing `sentibank-0.0.1.3/LICENSE` & `sentibank-0.0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.3/sentibank/archive.py` & `sentibank-0.0.1.4/sentibank/archive.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,87 @@
-import os 
-import pickle 
+import os
+import pickle
+
 
 class load:
-    def __init__(self): 
+    def __init__(self):
         self.script_dir = os.path.dirname(os.path.abspath(__file__))
-        self.lex_dict = None 
-    
-    def dict(self, idx:str):
+        self.lex_dict = None
+
+    def dict(self, idx: str):
         """_summary_
 
         Args:
             idx (str): _description_
 
         Returns:
             _type_: _description_
         """
-        if idx == 'MASTER_v2022':   
-            file_path = os.path.join(self.script_dir, 'dict_arXiv', 'MASTER', 'MASTER_v2022.pickle')           
-            with open(file_path, 'rb') as handle: 
+        if idx == "MASTER_v2022":
+            file_path = os.path.join(
+                self.script_dir, "dict_arXiv", "MASTER", "MASTER_v2022.pickle"
+            )
+            with open(file_path, "rb") as handle:
                 self.lex_dict = pickle.load(handle)
-        
-        elif idx == "VADER_v2014_mod": 
-            file_path = os.path.join(self.script_dir, 'dict_arXiv', 'VADER', 'VADER_v2014_mod.pickle')
-            with open(file_path, 'rb') as handle: 
+
+        elif idx == "VADER_v2014_mod":
+            file_path = os.path.join(
+                self.script_dir, "dict_arXiv", "VADER", "VADER_v2014_mod.pickle"
+            )
+            with open(file_path, "rb") as handle:
                 self.lex_dict = pickle.load(handle)
-                
-        elif idx == "AFINN_v2015": 
-            file_path = os.path.join(self.script_dir, 'dict_arXiv', 'AFINN', 'AFINN_v2015.pickle')
-            with open(file_path, 'rb') as handle: 
+
+        elif idx == "AFINN_v2015":
+            file_path = os.path.join(
+                self.script_dir, "dict_arXiv", "AFINN", "AFINN_v2015.pickle"
+            )
+            with open(file_path, "rb") as handle:
                 self.lex_dict = pickle.load(handle)
-        
-        elif idx == "Aigents+_v2022": 
-            file_path = os.path.join(self.script_dir, 'dict_arXiv', 'Aigents', 'Aigents+_v2022.pickle')
-            with open(file_path, 'rb') as handle: 
+
+        elif idx == "Aigents+_v2022":
+            file_path = os.path.join(
+                self.script_dir, "dict_arXiv", "Aigents", "Aigents+_v2022.pickle"
+            )
+            with open(file_path, "rb") as handle:
                 self.lex_dict = pickle.load(handle)
-                
+
         return self.lex_dict
-    
-    def origin(self, idx:str): 
+
+    def origin(self, idx: str):
         """_summary_
 
         Args:
             idx (str): _description_
 
         Returns:
             _type_: _description_
         """
-        import pandas as pd 
-        
-        if idx == 'MASTER_v2022':   
-            file_path = os.path.join(self.script_dir, 'dict_arXiv', 'MASTER', 'MASTER_v2022.csv')           
+        import pandas as pd
+
+        if idx == "MASTER_v2022":
+            file_path = os.path.join(
+                self.script_dir, "dict_arXiv", "MASTER", "MASTER_v2022.csv"
+            )
             self.origin_df = pd.read_csv(file_path)
-        
-        elif idx == "VADER_v2014_mod": 
-            file_path = os.path.join(self.script_dir, 'dict_arXiv', 'VADER', 'VADER_v2014.csv')
+
+        elif idx == "VADER_v2014_mod":
+            file_path = os.path.join(
+                self.script_dir, "dict_arXiv", "VADER", "VADER_v2014.csv"
+            )
             self.origin_df = pd.read_csv(file_path)
-                
-        elif idx == "AFINN_v2015": 
-            file_path = os.path.join(self.script_dir, 'dict_arXiv', 'AFINN', 'AFINN_v2015.csv')
+
+        elif idx == "AFINN_v2015":
+            file_path = os.path.join(
+                self.script_dir, "dict_arXiv", "AFINN", "AFINN_v2015.csv"
+            )
             self.origin_df = pd.read_csv(file_path)
-        
-        elif idx == "Aigents+_v2022": 
-            file_path = os.path.join(self.script_dir, 'dict_arXiv', 'Aigents', 'Aigents+_v2022.csv')
+
+        elif idx == "Aigents+_v2022":
+            file_path = os.path.join(
+                self.script_dir, "dict_arXiv", "Aigents", "Aigents+_v2022.csv"
+            )
             self.origin_df = pd.read_csv(file_path)
-        
-        else: 
+
+        else:
             raise ValueError
-        
-        return self.origin_df
+
+        return self.origin_df
```

### Comparing `sentibank-0.0.1.3/sentibank/dict_arXiv/AFINN/AFINN_v2015.csv` & `sentibank-0.0.1.4/sentibank/dict_arXiv/AFINN/AFINN_v2015.csv`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.3/sentibank/dict_arXiv/AFINN/AFINN_v2015.pickle` & `sentibank-0.0.1.4/sentibank/dict_arXiv/AFINN/AFINN_v2015.pickle`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.3/sentibank/dict_arXiv/Aigents/Aigents+_v2022.csv` & `sentibank-0.0.1.4/sentibank/dict_arXiv/Aigents/Aigents+_v2022.csv`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.3/sentibank/dict_arXiv/Aigents/Aigents+_v2022.pickle` & `sentibank-0.0.1.4/sentibank/dict_arXiv/Aigents/Aigents+_v2022.pickle`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.3/sentibank/dict_arXiv/MASTER/MASTER_v2022.csv` & `sentibank-0.0.1.4/sentibank/dict_arXiv/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.3/sentibank/dict_arXiv/MASTER/MASTER_v2022.pickle` & `sentibank-0.0.1.4/sentibank/dict_arXiv/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.3/sentibank/dict_arXiv/VADER/VADER_v2014.csv` & `sentibank-0.0.1.4/sentibank/dict_arXiv/VADER/VADER_v2014.csv`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.3/sentibank/dict_arXiv/VADER/VADER_v2014_mod.pickle` & `sentibank-0.0.1.4/sentibank/dict_arXiv/VADER/VADER_v2014_mod.pickle`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.3/sentibank/dict_arXiv/emos.py` & `sentibank-0.0.1.4/sentibank/dict_arXiv/emos.py`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.3/sentibank/utils.py` & `sentibank-0.0.1.4/sentibank/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class analysis:
     def __init__(self):
         self.spacy_nlp = spacy.load(
             "en_core_web_sm",
             exclude=["parser", "senter", "attribute_ruler", "lemmatizer", "ner"],
         )
-        #self.spacy_nlp.add_pipe("sentencizer")
+        # self.spacy_nlp.add_pipe("sentencizer")
         self.spacy_nlp.add_pipe("emoji", first=True)
 
     def count_categorical_labels(self, dictionary):
         label_counts = Counter()
         multi_label_counts = Counter()
 
         for sublist in track(
@@ -168,15 +168,20 @@
         # Sentiment Lexicon (Part-of-Speech Tag) Summary
         pos_tags = []
         general_dict = {
             "verbs": 0,
             "adjectives": 0,
             "adverbs": 0,
             "prepositions": 0,
+            "conjunctions": 0,
+            "determiners": 0,
+            "pronouns": 0,
+            "numerals": 0,
             "nouns": 0,
+            "particles": 0,
             "emos": 0,
             "miscellaneous": 0,
         }
         granular_dict = {}
         misc = []
 
         for key in track(
@@ -209,34 +214,51 @@
                 general_dict["adjectives"] += value
             elif key.startswith("RB"):
                 general_dict["adverbs"] += value
             elif key.startswith("IN"):
                 general_dict["prepositions"] += value
             elif key.startswith("N"):
                 general_dict["nouns"] += value
+            elif key.startswith("PRP") or key.startswith("WP"):
+                general_dict["pronouns"] += value
+            elif key == "CD":
+                general_dict["numerals"] += value
+            elif key == "CC":
+                general_dict["conjunctions"] += value
+            elif key == "DT" or key == "WDT":
+                general_dict["determiners"] += value
+            elif key == "RP":
+                general_dict["particles"] += value
             elif key == "EMOTICON":
                 general_dict["emos"] += value
             elif key == "EMOJI":
                 general_dict["emos"] += value
             else:
                 misc.append(key)
                 general_dict["miscellaneous"] += value
 
-        granular_dict_adv = {} 
-        
-        if "EMOTICON" or "EMOJI" in granular_dict.keys(): 
-            for key, value in granular_dict.items(): 
-                if key == "EMOTICON": 
-                    granular_dict_adv["EMOTICON (textual representations of emotions)"] = value
-                elif key == "EMOJI": 
-                    granular_dict_adv["EMOJI (pictorial symbols of emotions, objects, or concepts)"] = value 
-                else: 
-                    granular_dict_adv["{} ({})".format(key,spacy.explain(key))] = value
-        else: 
-            granular_dict_adv = dict(("{} ({})".format(key,spacy.explain(key)), value) for (key, value) in granular_dict.items())
+        granular_dict_adv = {}
+
+        if "EMOTICON" or "EMOJI" in granular_dict.keys():
+            for key, value in granular_dict.items():
+                if key == "EMOTICON":
+                    granular_dict_adv[
+                        "EMOTICON (textual representations of emotions)"
+                    ] = value
+                elif key == "EMOJI":
+                    granular_dict_adv[
+                        "EMOJI (pictorial symbols of emotions, objects, or concepts)"
+                    ] = value
+                else:
+                    granular_dict_adv["{} ({})".format(key, spacy.explain(key))] = value
+        else:
+            granular_dict_adv = dict(
+                ("{} ({})".format(key, spacy.explain(key)), value)
+                for (key, value) in granular_dict.items()
+            )
 
         part_of_speech = {
             "general": self.sort_dict(general_dict),
             "granular": self.sort_dict(granular_dict_adv),
             "misc": misc,
         }
 
@@ -244,14 +266,15 @@
             "Dictionary Type": lex_dict_type,
             "Sentiment Score": score_summary,
             "Sentiment Lexicon": part_of_speech,
         }
 
         return pprint(summary)
 
-class lexical_overview: 
-    def __init__(self, dictionary:dict=None): 
-        #dict:str = Consider if users simply come up with the lex_dict_idx
-        if dict is None: 
+
+class lexical_overview:
+    def __init__(self, dictionary: dict = None):
+        # dict:str = Consider if users simply come up with the lex_dict_idx
+        if dict is None:
             raise ValueError
         else:
-            analysis().summarise_lex_dict(dictionary)
+            analysis().summarise_lex_dict(dictionary)
```

### Comparing `sentibank-0.0.1.3/sentibank.egg-info/SOURCES.txt` & `sentibank-0.0.1.4/sentibank.egg-info/SOURCES.txt`

 * *Files identical despite different names*

