# Comparing `tmp/SMAGrader-0.1.8.tar.gz` & `tmp/SMAGrader-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMAGrader-0.1.8.tar", last modified: Tue Aug  1 19:22:42 2023, max compression
+gzip compressed data, was "SMAGrader-0.1.9.tar", last modified: Tue Aug  1 19:32:34 2023, max compression
```

## Comparing `SMAGrader-0.1.8.tar` & `SMAGrader-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 19:22:42.473720 SMAGrader-0.1.8/
--rw-rw-rw-   0        0        0      151 2023-08-01 19:22:42.473720 SMAGrader-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 19:22:42.444673 SMAGrader-0.1.8/SMAGrader/
--rw-rw-rw-   0        0        0        0 2023-07-25 19:17:05.000000 SMAGrader-0.1.8/SMAGrader/__init__.py
--rw-rw-rw-   0        0        0    18760 2023-08-01 19:22:18.000000 SMAGrader-0.1.8/SMAGrader/checker.py
-drwxrwxrwx   0        0        0        0 2023-08-01 19:22:42.470719 SMAGrader-0.1.8/SMAGrader.egg-info/
--rw-rw-rw-   0        0        0      151 2023-08-01 19:22:42.000000 SMAGrader-0.1.8/SMAGrader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-08-01 19:22:42.000000 SMAGrader-0.1.8/SMAGrader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 19:22:42.000000 SMAGrader-0.1.8/SMAGrader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-01 19:22:42.000000 SMAGrader-0.1.8/SMAGrader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-01 19:22:42.000000 SMAGrader-0.1.8/SMAGrader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 19:22:42.474720 SMAGrader-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      408 2023-08-01 19:22:33.000000 SMAGrader-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:32:34.381184 SMAGrader-0.1.9/
+-rw-rw-rw-   0        0        0      151 2023-08-01 19:32:34.380184 SMAGrader-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 19:32:34.357181 SMAGrader-0.1.9/SMAGrader/
+-rw-rw-rw-   0        0        0        0 2023-07-25 19:17:05.000000 SMAGrader-0.1.9/SMAGrader/__init__.py
+-rw-rw-rw-   0        0        0    18594 2023-08-01 19:31:57.000000 SMAGrader-0.1.9/SMAGrader/checker.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:32:34.378185 SMAGrader-0.1.9/SMAGrader.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-08-01 19:32:34.000000 SMAGrader-0.1.9/SMAGrader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-08-01 19:32:34.000000 SMAGrader-0.1.9/SMAGrader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 19:32:34.000000 SMAGrader-0.1.9/SMAGrader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-01 19:32:34.000000 SMAGrader-0.1.9/SMAGrader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 19:32:34.000000 SMAGrader-0.1.9/SMAGrader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 19:32:34.381184 SMAGrader-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      408 2023-08-01 19:32:31.000000 SMAGrader-0.1.9/setup.py
```

### Comparing `SMAGrader-0.1.8/SMAGrader/checker.py` & `SMAGrader-0.1.9/SMAGrader/checker.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,78 +17,86 @@
 # client_secret = config.get("client_secret")
 # user_agent = config.get("user_agent")
 
 
 # import to server and then from server to database. Use DJango and mySQL database on python everywhere
 def authenticate():
     try:
-        import google.colab
+        from google.colab import auth
 
         IN_COLAB = True
     except ImportError:
         IN_COLAB = False
 
     if IN_COLAB:
-        google.colab.auth.authenticate_user()
-        gcloud_token = !gcloud auth print-access-token
-        gcloud_tokeninfo = requests.get('https://www.googleapis.com/oauth2/v3/tokeninfo?access_token=' + gcloud_token[0]).json()    
-        email = gcloud_tokeninfo['email']
-        return email
+        auth.authenticate_user()
+
+        cookie_file = os.path.join(os.environ["HOME"], ".config/gcloud/credentials.db")
+        with open(cookie_file, "r") as f:
+            content = f.read()
+
+        email_index = content.find("@")
+
+        if email_index != -1:
+            email_end_index = email_index + 1
+            while (
+                email_end_index < len(content)
+                and not content[email_end_index].isspace()
+            ):
+                email_end_index += 1
+            return content[email_index:email_end_index]
+        else:
+            return None
     else:
         print("Not running in Google Colab")
 
 
 def send_results(func_name, results):
-    email=authenticate()
+    email = authenticate()
     url = "http://arisharma.pythonanywhere.com/autograder/save_result/"  # Replace with your server URL
 
-    payload = {
-        'func_name': func_name,
-        'email': email,
-        'results': results
-    }
+    payload = {'func_name': func_name, 'email': email, 'results': results}
 
     response = requests.get(url, json=payload)
     print(response.json())
 
 
 def addition(add_func):
     for _ in range(10):
         a = random.randint(1, 100)
         b = random.randint(1, 100)
         expected_result = a + b
         result = add_func(a, b)
 
         if result == expected_result:
-            send_results(
-                "addition", (f"Addition test passed: {a} + {b} = {result}")
-            )
+            send_results("addition", (f"Addition test passed: {a} + {b} = {result}"))
         else:
             send_results(
-                "addition",(f"Addition test failed: {a} + {b} = {result}, expected {expected_result}")
+                "addition",
+                (
+                    f"Addition test failed: {a} + {b} = {result}, expected {expected_result}"
+                ),
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
-                
                 (f"Multiplication test passed: {a} * {b} = {result}"),
             )
         else:
             send_results(
                 "multiplication",
-                
                 (
                     f"Multiplication test failed: {a} * {b} = {result}, expected {expected_result}"
                 ),
             )
 
 
 def division(div_func):
@@ -100,21 +108,19 @@
             expected_result = a / b
         except ZeroDivisionError:
             expected_result = "Cannot divide by zero"
         result = div_func(a, b)
         if result == expected_result:
             send_results(
                 "multiplication",
-                
                 (f"Division test passed: {a} / {b} = {result}"),
             )
         else:
             send_results(
                 "multiplication",
-                
                 (
                     f"Division test failed: {a} / {b} = {result}, expected {expected_result}"
                 ),
             )
 
 
 def get_random_df_for_space_check():
@@ -158,21 +164,19 @@
         else:
             print("Error: 'text' column not found in the DataFrame.")
             return expected_df
 
         if dataframe_equality(expected_df, actual_df):
             send_results(
                 "replace_spaces",
-                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "replace_spaces",
-                
                 (print(f"Case {i+1} failed")),
             )
 
 
 def get_random_df_for_the_check():
     dataframes = []
     for _ in range(10):
@@ -202,22 +206,20 @@
         else:
             print("Error: 'text' column not found in the DataFrame.")
             return expected_df
 
         if dataframe_equality(expected_df, actual_df):
             send_results(
                 "replace_the",
-                
                 (f"Case {i+1} passed"),
             )
 
         else:
             send_results(
                 "replace_the",
-                
                 (f"Case {i+1} failed"),
             )
 
 
 def get_random_df_for_group_check():
     dataframes = []
     np.random.seed(42)  # Set a seed for reproducibility
@@ -238,21 +240,19 @@
     for i, df in enumerate(random_dataframes):
         expected_df = df.groupby("group")["value"].agg(["sum", "mean", "median"])
         actual_df = func(df)
 
         if dataframe_equality(expected_df, actual_df):
             send_results(
                 "group_check",
-                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "group_check",
-                
                 (f"Case {i+1} failed"),
             )
 
 
 def get_random_df_for_join_check():
     dataframes_list_1 = []
     dataframes_list_2 = []
@@ -285,21 +285,19 @@
             # Add 'total' column as the sum of 'value1' and 'value2'
             expected_df["total"] = expected_df["value1"] + expected_df["value2"]
             actual_df = func(df_A, df_B)
 
             if dataframe_equality(expected_df, actual_df):
                 send_results(
                     "join_check",
-                    
                     (f"Case {i+1} passed"),
                 )
             else:
                 send_results(
                     "join_check",
-                    
                     (f"Case {i+1} failed"),
                 )
 
 
 def left_join_check(func):
     list1, list2 = get_random_df_for_join_check()
     for i, df_A in enumerate(list1):
@@ -308,21 +306,19 @@
             expected_df = expected_df[expected_df["_merge"] == "left_only"]
 
             actual_df = func(df_A, df_B)
 
             if dataframe_equality(expected_df, actual_df):
                 send_results(
                     "left_join_check",
-                    
                     (f"Case {i+1} passed"),
                 )
             else:
                 send_results(
                     "left_join_check",
-                    
                     (f"Case {i+1} failed"),
                 )
 
 
 def get_random_df_for_count_nouns_check():
     dataframes_list = []
     random.seed(42)  # Set a seed for reproducibility
@@ -383,21 +379,19 @@
             )
         )
         actual_df = func(df)
 
         if dataframe_equality(expected_df, actual_df):
             send_results(
                 "count_nouns_check",
-                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "count_nouns_check",
-                
                 (f"Case {i+1} failed"),
             )
 
 
 def get_random_str_for_count_check():
     nltk.download("words")
     english_words = set(nltk.corpus.words.words())
@@ -425,21 +419,19 @@
         expected_word_freq = {}
         for word in expected_word:
             expected_word_freq[word] = expected_word_freq.get(word, 0) + 1
 
         if expected_word_freq == actual_word_freq:
             send_results(
                 "counter_check",
-                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "counter_check",
-                
                 (f"Case {i+1} failed"),
             )
 
 
 def count_nouns_check(func):
     random_words = get_random_str_for_count_check()
     for i, word in enumerate(random_words):
@@ -451,21 +443,19 @@
 
         # Count the number of nouns
         expected_count = sum(1 for token, pos in tagged_tokens if pos.startswith("NN"))
 
         if expected_count == actual_count:
             send_results(
                 "count_nouns_check",
-                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "count_nouns_check",
-                
                 (f"Case {i+1} failed"),
             )
 
 
 def sentiment_analysis_check(func):
     random_text = get_random_str_for_count_check()
     for i, text in enumerate(random_text):
@@ -484,21 +474,19 @@
             expected_sentiment = "Negative"
         else:
             expected_sentiment = "Neutral"
 
         if expected_sentiment == actual_sentiment:
             send_results(
                 "sentiment_analysis_check",
-                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "sentiment_analysis_check",
-                
                 (f"Case {i+1} failed"),
             )
 
 
 def named_entity_recognition_check(func):
     random_text = get_random_str_for_count_check()
     for i, text in enumerate(random_text):
@@ -539,21 +527,19 @@
         # Convert the JSON dictionary to a JSON string
         expected_entities = json.dumps(entities_json)
         actual_entities = func(text)
 
         if expected_entities == actual_entities:
             send_results(
                 "named_entity_recognition_check",
-                
                 (f"Case {i+1} passed"),
             )
         else:
             send_results(
                 "named_entity_recognition_check",
-                
                 (f"Case {i+1} failed"),
             )
 
 
 # def scrape_from_reddit_check(func):
 #     subreddit_name = "ut_sma"
 #     actual_content = func(subreddit_name)
@@ -571,20 +557,20 @@
 #         submission.comments.replace_more(limit=None)
 #         for comment in submission.comments.list():
 #             expected_content.append(comment.body)
 
 #     if expected_content == actual_content:
 #         send_results(
 #             "named_entity_recognition_check",
-#             
+#
 #             ("Cases passed"),
 #         )
 #     else:
 #         send_results(
 #             "named_entity_recognition_check",
-#             
+#
 #             ("Cases failed"),
 #         )
 
 
 # TODO: Upload to the official PyPi repo and try to download in google colab notebook and check if it works
-# TODO: Change time zone in settings.py so that it corresponds to CST time zone
+# TODO: Change time zone in settings.py so that it corresponds to CST time zone
```

