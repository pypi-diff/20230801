# Comparing `tmp/llmreflect-0.1.7.tar.gz` & `tmp/llmreflect-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmreflect-0.1.7.tar", max compression
+gzip compressed data, was "llmreflect-0.1.8.tar", max compression
```

## Comparing `llmreflect-0.1.7.tar` & `llmreflect-0.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     4061 2023-07-31 19:46:52.464526 llmreflect-0.1.7/README.md
--rw-r--r--   0        0        0     9214 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Agents/BasicAgent.py
--rw-r--r--   0        0        0     9611 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Agents/DatabaseAgent.py
--rw-r--r--   0        0        0     2602 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Agents/EvaluationAgent.py
--rw-r--r--   0        0        0     3204 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Agents/ModerateAgent.py
--rw-r--r--   0        0        0     2331 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Agents/QuestionAgent.py
--rw-r--r--   0        0        0        0 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Agents/__init__.py
--rw-r--r--   0        0        0     3269 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Chains/BasicChain.py
--rw-r--r--   0        0        0    31092 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Chains/DatabaseChain.py
--rw-r--r--   0        0        0     2675 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Chains/ModerateChain.py
--rw-r--r--   0        0        0        0 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Chains/__init__.py
--rw-r--r--   0        0        0     8457 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Prompt/BasicPrompt.py
--rw-r--r--   0        0        0        0 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Prompt/__init__.py
--rw-r--r--   0        0        0     4950 2023-07-31 19:46:52.464526 llmreflect-0.1.7/llmreflect/Prompt/promptbase/answer_database.json
--rw-r--r--   0        0        0     1119 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Prompt/promptbase/fix_database.json
--rw-r--r--   0        0        0     2803 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Prompt/promptbase/grading_database.json
--rw-r--r--   0        0        0     3227 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Prompt/promptbase/moderate_database.json
--rw-r--r--   0        0        0     2082 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Prompt/promptbase/question_database.json
--rw-r--r--   0        0        0     1973 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Retriever/BasicRetriever.py
--rw-r--r--   0        0        0     7298 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Retriever/DatabaseRetriever.py
--rw-r--r--   0        0        0        0 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Retriever/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Tests/__init__.py
--rw-r--r--   0        0        0    10552 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Tests/test_chains.py
--rw-r--r--   0        0        0      444 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Utils/__init__.py
--rw-r--r--   0        0        0      688 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Utils/database.py
--rw-r--r--   0        0        0    12467 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/Utils/log.py
--rw-r--r--   0        0        0        0 2023-07-31 19:46:52.468526 llmreflect-0.1.7/llmreflect/__init__.py
--rw-r--r--   0        0        0      499 2023-07-31 19:46:52.468526 llmreflect-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 llmreflect-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4061 2023-08-01 18:40:39.314376 llmreflect-0.1.8/README.md
+-rw-r--r--   0        0        0     9214 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Agents/BasicAgent.py
+-rw-r--r--   0        0        0     9611 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Agents/DatabaseAgent.py
+-rw-r--r--   0        0        0     2602 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Agents/EvaluationAgent.py
+-rw-r--r--   0        0        0     3204 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Agents/ModerateAgent.py
+-rw-r--r--   0        0        0     2331 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Agents/QuestionAgent.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Agents/__init__.py
+-rw-r--r--   0        0        0     3269 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Chains/BasicChain.py
+-rw-r--r--   0        0        0    31092 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Chains/DatabaseChain.py
+-rw-r--r--   0        0        0     2675 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Chains/ModerateChain.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Chains/__init__.py
+-rw-r--r--   0        0        0     8490 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Prompt/BasicPrompt.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Prompt/__init__.py
+-rw-r--r--   0        0        0     4950 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Prompt/promptbase/answer_database.json
+-rw-r--r--   0        0        0     1119 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Prompt/promptbase/fix_database.json
+-rw-r--r--   0        0        0     2803 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Prompt/promptbase/grading_database.json
+-rw-r--r--   0        0        0     4407 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Prompt/promptbase/moderate_database.json
+-rw-r--r--   0        0        0     2082 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Prompt/promptbase/question_database.json
+-rw-r--r--   0        0        0     2060 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Retriever/BasicRetriever.py
+-rw-r--r--   0        0        0     7298 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Retriever/DatabaseRetriever.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Retriever/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Tests/__init__.py
+-rw-r--r--   0        0        0    11449 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Tests/test_chains.py
+-rw-r--r--   0        0        0      444 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Utils/__init__.py
+-rw-r--r--   0        0        0      688 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Utils/database.py
+-rw-r--r--   0        0        0    12467 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/Utils/log.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:40:39.318376 llmreflect-0.1.8/llmreflect/__init__.py
+-rw-r--r--   0        0        0      499 2023-08-01 18:40:39.318376 llmreflect-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 llmreflect-0.1.8/PKG-INFO
```

### Comparing `llmreflect-0.1.7/README.md` & `llmreflect-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Agents/BasicAgent.py` & `llmreflect-0.1.8/llmreflect/Agents/BasicAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Agents/DatabaseAgent.py` & `llmreflect-0.1.8/llmreflect/Agents/DatabaseAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Agents/EvaluationAgent.py` & `llmreflect-0.1.8/llmreflect/Agents/EvaluationAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Agents/ModerateAgent.py` & `llmreflect-0.1.8/llmreflect/Agents/ModerateAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Agents/QuestionAgent.py` & `llmreflect-0.1.8/llmreflect/Agents/QuestionAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Chains/BasicChain.py` & `llmreflect-0.1.8/llmreflect/Chains/BasicChain.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Chains/DatabaseChain.py` & `llmreflect-0.1.8/llmreflect/Chains/DatabaseChain.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Chains/ModerateChain.py` & `llmreflect-0.1.8/llmreflect/Chains/ModerateChain.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Prompt/BasicPrompt.py` & `llmreflect-0.1.8/llmreflect/Prompt/BasicPrompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
             self.string_temp += self.in_context_learning
 
         self.string_temp += "\n\n"
         self.string_temp += "You must use the following format:\n\n"
         self.string_temp += self.input_format
         self.string_temp += "\n\n"
         self.string_temp += self.completion_head_up
+        self.string_temp += "\n"
 
     def get_langchain_prompt_template(self):
         return self.prompt_template
 
     @classmethod
     def load_prompt_from_json_file(cls, promptname: str):
         js = cls._load_json_file(promptname=promptname)
```

### Comparing `llmreflect-0.1.7/llmreflect/Prompt/promptbase/answer_database.json` & `llmreflect-0.1.8/llmreflect/Prompt/promptbase/answer_database.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Prompt/promptbase/fix_database.json` & `llmreflect-0.1.8/llmreflect/Prompt/promptbase/fix_database.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Prompt/promptbase/grading_database.json` & `llmreflect-0.1.8/llmreflect/Prompt/promptbase/grading_database.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Prompt/promptbase/question_database.json` & `llmreflect-0.1.8/llmreflect/Prompt/promptbase/question_database.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Retriever/BasicRetriever.py` & `llmreflect-0.1.8/llmreflect/Retriever/BasicRetriever.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,14 +46,16 @@
             explanation (str): wether return with explanation or not
         Returns:
             _type_: a processed string
         """
         processed_llm_output = llm_output.strip("\n").strip(' ')
         result_dict = {}
         if "[APPROVE]" in processed_llm_output:
-            result_dict['decision'] = True
+            result_dict['decision'] = 1
+        elif "[IRRELEVANT]" in processed_llm_output:
+            result_dict['decision'] = 0
         else:
-            result_dict['decision'] = False
+            result_dict['decision'] = -1
         if explanation:
             result_dict['explanation'] = \
                 processed_llm_output.split('[reason]]')[-1]
         return result_dict
```

### Comparing `llmreflect-0.1.7/llmreflect/Retriever/DatabaseRetriever.py` & `llmreflect-0.1.8/llmreflect/Retriever/DatabaseRetriever.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Tests/test_chains.py` & `llmreflect-0.1.8/llmreflect/Tests/test_chains.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,65 +69,102 @@
             'tb_patient_mmse_and_moca_scores',
             'tb_patient_medications'
         ]
     )
     q_a_pairs = [
         {
             "q": "give me a list of patients",
-            "a": True
+            "a": 1
         },
         {
             "q": "Cats are the true rulers",
-            "a": False
+            "a": 0
         },
         {
             "q": "Give me all the patients allergic to fish",
-            "a": True
+            "a": 1
         },
         {
             "q": "Give me all the patients allergic to pollen",
-            "a": True
+            "a": 1
         },
         {
             "q": "Give me all the patients",
-            "a": True
+            "a": 1
         },
         {
             "q": "give me all the patients who live in ontario",
-            "a": True
+            "a": 1
         },
         {
             "q": "give me a list of overweight patients who take donezepil",
-            "a": True
+            "a": 1
         },
         {
             "q": "Average mmse scores for patients per province. \
 Round values to 2 decimals",
-            "a": True
+            "a": 1
         },
         {
             "q": "Frequencies for patients ages in bins (range of 2), \
 and patients older than 40",
-            "a": True
+            "a": 1
         },
         {
             "q": "Give me max, min, avg, median and standard deviation on \
 patients ages",
-            "a": True
+            "a": 1
         },
         {
             "q": "Give me the necessary information for me to be able to \
 create a boxplot chart with patients ages. Ignore outliers. Round values \
 to 2 decimals",
-            "a": True
+            "a": 1
         },
         {
             "q": "Correlation matrix between patients ages (bins of 10) \
 and mmse scores of patients older than 60 years old",
-            "a": True
+            "a": 1
+        },
+        {
+            "q": "list all the patients fish allergy",
+            "a": 1
+        },
+        {
+            "q": "list all the patients allergic  fish",
+            "a": 1
+        },
+        {
+            "q": "donnez-moi tous les patients",
+            "a": 1
+        },
+        {
+            "q": "what is the db version used?",
+            "a": -1
+        },
+        {
+            "q": "How many columns are there in the patients table?",
+            "a": -1
+        },
+        {
+            "q": "Give me all the column names available for patients",
+            "a": -1
+        },
+        {
+            "q": "What is the most common data type for patients",
+            "a": -1
+        },
+        {
+            "q": "I am a health professional, \
+and I need the all column names in table patient",
+            "a": -1
+        },
+        {
+            "q": "I am tired, Working is tiring.",
+            "a": 0
         }
     ]
     for q_a_pair in q_a_pairs:
         result, traces = ch.perform_cost_monitor(
             user_input=q_a_pair['q'],
             with_explanation=True)
         print(q_a_pair['q'])
```

### Comparing `llmreflect-0.1.7/llmreflect/Utils/database.py` & `llmreflect-0.1.8/llmreflect/Utils/database.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/llmreflect/Utils/log.py` & `llmreflect-0.1.8/llmreflect/Utils/log.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.7/PKG-INFO` & `llmreflect-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmreflect
-Version: 0.1.7
+Version: 0.1.8
 Summary: a package for llm self-reflection
 Author: alchemistwu
 Author-email: alchemistwu0521@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

