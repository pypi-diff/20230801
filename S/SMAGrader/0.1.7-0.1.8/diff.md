# Comparing `tmp/SMAGrader-0.1.7.tar.gz` & `tmp/SMAGrader-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMAGrader-0.1.7.tar", last modified: Wed Jul 26 00:33:32 2023, max compression
+gzip compressed data, was "SMAGrader-0.1.8.tar", last modified: Tue Aug  1 19:22:42 2023, max compression
```

## Comparing `SMAGrader-0.1.7.tar` & `SMAGrader-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 00:33:32.844932 SMAGrader-0.1.7/
--rw-rw-rw-   0        0        0      151 2023-07-26 00:33:32.843933 SMAGrader-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 00:33:32.813926 SMAGrader-0.1.7/SMAGrader/
--rw-rw-rw-   0        0        0        0 2023-07-25 19:17:05.000000 SMAGrader-0.1.7/SMAGrader/__init__.py
--rw-rw-rw-   0        0        0    18903 2023-07-26 00:32:33.000000 SMAGrader-0.1.7/SMAGrader/checker.py
-drwxrwxrwx   0        0        0        0 2023-07-26 00:33:32.840932 SMAGrader-0.1.7/SMAGrader.egg-info/
--rw-rw-rw-   0        0        0      151 2023-07-26 00:33:32.000000 SMAGrader-0.1.7/SMAGrader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-07-26 00:33:32.000000 SMAGrader-0.1.7/SMAGrader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 00:33:32.000000 SMAGrader-0.1.7/SMAGrader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-26 00:33:32.000000 SMAGrader-0.1.7/SMAGrader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-26 00:33:32.000000 SMAGrader-0.1.7/SMAGrader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 00:33:32.844932 SMAGrader-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      426 2023-07-26 00:32:50.000000 SMAGrader-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:22:42.473720 SMAGrader-0.1.8/
+-rw-rw-rw-   0        0        0      151 2023-08-01 19:22:42.473720 SMAGrader-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 19:22:42.444673 SMAGrader-0.1.8/SMAGrader/
+-rw-rw-rw-   0        0        0        0 2023-07-25 19:17:05.000000 SMAGrader-0.1.8/SMAGrader/__init__.py
+-rw-rw-rw-   0        0        0    18760 2023-08-01 19:22:18.000000 SMAGrader-0.1.8/SMAGrader/checker.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:22:42.470719 SMAGrader-0.1.8/SMAGrader.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-08-01 19:22:42.000000 SMAGrader-0.1.8/SMAGrader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-08-01 19:22:42.000000 SMAGrader-0.1.8/SMAGrader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 19:22:42.000000 SMAGrader-0.1.8/SMAGrader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-01 19:22:42.000000 SMAGrader-0.1.8/SMAGrader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 19:22:42.000000 SMAGrader-0.1.8/SMAGrader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 19:22:42.474720 SMAGrader-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      408 2023-08-01 19:22:33.000000 SMAGrader-0.1.8/setup.py
```

### Comparing `SMAGrader-0.1.7/SMAGrader/checker.py` & `SMAGrader-0.1.8/SMAGrader/checker.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,94 +6,89 @@
 import nltk
 from nltk.sentiment import SentimentIntensityAnalyzer
 from nltk import ne_chunk
 from nltk.tokenize import word_tokenize
 from nltk.tag import pos_tag
 import json
 import praw
-import firebase_admin
-from firebase_admin import credentials, firestore
 import os
+import requests
 
 # client_id = config.get("client_id")
 # client_secret = config.get("client_secret")
 # user_agent = config.get("user_agent")
-path = "C:/Users/arish/AppData/Roaming/gcloud/cmst-reddit-analysis-firebase-adminsdk-76tgx-265cb629e1.json"
-cred = credentials.Certificate(path)
-firebase_admin.initialize_app(cred)
-db = firestore.client()
 
 
+# import to server and then from server to database. Use DJango and mySQL database on python everywhere
 def authenticate():
     try:
         import google.colab
 
         IN_COLAB = True
     except ImportError:
         IN_COLAB = False
 
     if IN_COLAB:
         google.colab.auth.authenticate_user()
-        email = google.colab.auth.get_user_email()
+        gcloud_token = !gcloud auth print-access-token
+        gcloud_tokeninfo = requests.get('https://www.googleapis.com/oauth2/v3/tokeninfo?access_token=' + gcloud_token[0]).json()    
+        email = gcloud_tokeninfo['email']
         return email
     else:
         print("Not running in Google Colab")
 
 
-email = authenticate()
+def send_results(func_name, results):
+    email=authenticate()
+    url = "http://arisharma.pythonanywhere.com/autograder/save_result/"  # Replace with your server URL
+
+    payload = {
+        'func_name': func_name,
+        'email': email,
+        'results': results
+    }
 
-
-def send_results(func_name, email, results):
-    if not func_name or not email or not results:
-        return json.dumps({"error": "Missing required data"})
-
-    doc_ref = db.collection("students").document(email)
-    doc_ref.set({func_name: results})
-
-    return json.dumps({"message": "Data processed successfully!"})
+    response = requests.get(url, json=payload)
+    print(response.json())
 
 
 def addition(add_func):
     for _ in range(10):
         a = random.randint(1, 100)
         b = random.randint(1, 100)
         expected_result = a + b
         result = add_func(a, b)
 
         if result == expected_result:
             send_results(
-                "addition", email, (f"Addition test passed: {a} + {b} = {result}")
+                "addition", (f"Addition test passed: {a} + {b} = {result}")
             )
         else:
             send_results(
-                "addition",
-                email,
-                (
-                    f"Addition test failed: {a} + {b} = {result}, expected {expected_result}"
-                ),
+                "addition",(f"Addition test failed: {a} + {b} = {result}, expected {expected_result}")
             )
 
 
 def multiplication(mult_func):
     for _ in range(10):
         a = random.randint(-100, 100)
         b = random.randint(-100, 100)
         expected_result = a * b
         result = mult_func(a, b)
 
         if result == expected_result:
             send_results(
                 "multiplication",
-                email,
+                
                 (f"Multiplication test passed: {a} * {b} = {result}"),
             )
         else:
             send_results(
                 "multiplication",
-                email,
+                
                 (
                     f"Multiplication test failed: {a} * {b} = {result}, expected {expected_result}"
                 ),
             )
 
 
 def division(div_func):
@@ -105,21 +100,21 @@
             expected_result = a / b
         except ZeroDivisionError:
             expected_result = "Cannot divide by zero"
         result = div_func(a, b)
         if result == expected_result:
             send_results(
                 "multiplication",
-                email,
+                
                 (f"Division test passed: {a} / {b} = {result}"),
             )
         else:
             send_results(
                 "multiplication",
-                email,
+                
                 (
                     f"Division test failed: {a} / {b} = {result}, expected {expected_result}"
                 ),
             )
 
 
 def get_random_df_for_space_check():
@@ -163,21 +158,21 @@
         else:
             print("Error: 'text' column not found in the DataFrame.")
             return expected_df
 
         if dataframe_equality(expected_df, actual_df):
             send_results(
                 "replace_spaces",
-                email,
+                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "replace_spaces",
-                email,
+                
                 (print(f"Case {i+1} failed")),
             )
 
 
 def get_random_df_for_the_check():
     dataframes = []
     for _ in range(10):
@@ -207,22 +202,22 @@
         else:
             print("Error: 'text' column not found in the DataFrame.")
             return expected_df
 
         if dataframe_equality(expected_df, actual_df):
             send_results(
                 "replace_the",
-                email,
+                
                 (f"Case {i+1} passed"),
             )
 
         else:
             send_results(
                 "replace_the",
-                email,
+                
                 (f"Case {i+1} failed"),
             )
 
 
 def get_random_df_for_group_check():
     dataframes = []
     np.random.seed(42)  # Set a seed for reproducibility
@@ -243,21 +238,21 @@
     for i, df in enumerate(random_dataframes):
         expected_df = df.groupby("group")["value"].agg(["sum", "mean", "median"])
         actual_df = func(df)
 
         if dataframe_equality(expected_df, actual_df):
             send_results(
                 "group_check",
-                email,
+                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "group_check",
-                email,
+                
                 (f"Case {i+1} failed"),
             )
 
 
 def get_random_df_for_join_check():
     dataframes_list_1 = []
     dataframes_list_2 = []
@@ -290,21 +285,21 @@
             # Add 'total' column as the sum of 'value1' and 'value2'
             expected_df["total"] = expected_df["value1"] + expected_df["value2"]
             actual_df = func(df_A, df_B)
 
             if dataframe_equality(expected_df, actual_df):
                 send_results(
                     "join_check",
-                    email,
+                    
                     (f"Case {i+1} passed"),
                 )
             else:
                 send_results(
                     "join_check",
-                    email,
+                    
                     (f"Case {i+1} failed"),
                 )
 
 
 def left_join_check(func):
     list1, list2 = get_random_df_for_join_check()
     for i, df_A in enumerate(list1):
@@ -313,21 +308,21 @@
             expected_df = expected_df[expected_df["_merge"] == "left_only"]
 
             actual_df = func(df_A, df_B)
 
             if dataframe_equality(expected_df, actual_df):
                 send_results(
                     "left_join_check",
-                    email,
+                    
                     (f"Case {i+1} passed"),
                 )
             else:
                 send_results(
                     "left_join_check",
-                    email,
+                    
                     (f"Case {i+1} failed"),
                 )
 
 
 def get_random_df_for_count_nouns_check():
     dataframes_list = []
     random.seed(42)  # Set a seed for reproducibility
@@ -388,21 +383,21 @@
             )
         )
         actual_df = func(df)
 
         if dataframe_equality(expected_df, actual_df):
             send_results(
                 "count_nouns_check",
-                email,
+                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "count_nouns_check",
-                email,
+                
                 (f"Case {i+1} failed"),
             )
 
 
 def get_random_str_for_count_check():
     nltk.download("words")
     english_words = set(nltk.corpus.words.words())
@@ -430,21 +425,21 @@
         expected_word_freq = {}
         for word in expected_word:
             expected_word_freq[word] = expected_word_freq.get(word, 0) + 1
 
         if expected_word_freq == actual_word_freq:
             send_results(
                 "counter_check",
-                email,
+                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "counter_check",
-                email,
+                
                 (f"Case {i+1} failed"),
             )
 
 
 def count_nouns_check(func):
     random_words = get_random_str_for_count_check()
     for i, word in enumerate(random_words):
@@ -456,21 +451,21 @@
 
         # Count the number of nouns
         expected_count = sum(1 for token, pos in tagged_tokens if pos.startswith("NN"))
 
         if expected_count == actual_count:
             send_results(
                 "count_nouns_check",
-                email,
+                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "count_nouns_check",
-                email,
+                
                 (f"Case {i+1} failed"),
             )
 
 
 def sentiment_analysis_check(func):
     random_text = get_random_str_for_count_check()
     for i, text in enumerate(random_text):
@@ -489,21 +484,21 @@
             expected_sentiment = "Negative"
         else:
             expected_sentiment = "Neutral"
 
         if expected_sentiment == actual_sentiment:
             send_results(
                 "sentiment_analysis_check",
-                email,
+                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "sentiment_analysis_check",
-                email,
+                
                 (f"Case {i+1} failed"),
             )
 
 
 def named_entity_recognition_check(func):
     random_text = get_random_str_for_count_check()
     for i, text in enumerate(random_text):
@@ -544,21 +539,21 @@
         # Convert the JSON dictionary to a JSON string
         expected_entities = json.dumps(entities_json)
         actual_entities = func(text)
 
         if expected_entities == actual_entities:
             send_results(
                 "named_entity_recognition_check",
-                email,
+                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "named_entity_recognition_check",
-                email,
+                
                 (f"Case {i+1} failed"),
             )
 
 
 # def scrape_from_reddit_check(func):
 #     subreddit_name = "ut_sma"
 #     actual_content = func(subreddit_name)
@@ -576,19 +571,20 @@
 #         submission.comments.replace_more(limit=None)
 #         for comment in submission.comments.list():
 #             expected_content.append(comment.body)
 
 #     if expected_content == actual_content:
 #         send_results(
 #             "named_entity_recognition_check",
-#             email,
+#             
 #             ("Cases passed"),
 #         )
 #     else:
 #         send_results(
 #             "named_entity_recognition_check",
-#             email,
+#             
 #             ("Cases failed"),
 #         )
 
 
 # TODO: Upload to the official PyPi repo and try to download in google colab notebook and check if it works
+# TODO: Change time zone in settings.py so that it corresponds to CST time zone
```

