# Comparing `tmp/uo_puddles-1.89.tar.gz` & `tmp/uo_puddles-1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uo_puddles-1.89.tar", last modified: Fri May 26 21:02:16 2023, max compression
+gzip compressed data, was "uo_puddles-1.90.tar", last modified: Tue Aug  1 21:00:19 2023, max compression
```

## Comparing `uo_puddles-1.89.tar` & `uo_puddles-1.90.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:02:16.582081 uo_puddles-1.89/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-26 21:02:07.000000 uo_puddles-1.89/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-26 21:02:16.582081 uo_puddles-1.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-26 21:02:07.000000 uo_puddles-1.89/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 21:02:07.000000 uo_puddles-1.89/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:02:16.582081 uo_puddles-1.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-26 21:02:07.000000 uo_puddles-1.89/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:02:16.582081 uo_puddles-1.89/uo_puddles/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-26 21:02:07.000000 uo_puddles-1.89/uo_puddles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-05-26 21:02:07.000000 uo_puddles-1.89/uo_puddles/cis423.py
--rw-r--r--   0 runner    (1001) docker     (123)    26336 2023-05-26 21:02:07.000000 uo_puddles-1.89/uo_puddles/good_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-05-26 21:02:07.000000 uo_puddles-1.89/uo_puddles/good_ai_22.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-05-26 21:02:07.000000 uo_puddles-1.89/uo_puddles/gremcat_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-26 21:02:07.000000 uo_puddles-1.89/uo_puddles/gremcat_oo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:02:16.582081 uo_puddles-1.89/uo_puddles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-26 21:02:16.000000 uo_puddles-1.89/uo_puddles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-26 21:02:16.000000 uo_puddles-1.89/uo_puddles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:02:16.000000 uo_puddles-1.89/uo_puddles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 21:02:16.000000 uo_puddles-1.89/uo_puddles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:00:19.908265 uo_puddles-1.90/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-01 21:00:09.000000 uo_puddles-1.90/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 21:00:19.908265 uo_puddles-1.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 21:00:09.000000 uo_puddles-1.90/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-01 21:00:09.000000 uo_puddles-1.90/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:00:19.908265 uo_puddles-1.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-01 21:00:09.000000 uo_puddles-1.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:00:19.908265 uo_puddles-1.90/uo_puddles/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/cis423.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26639 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/good_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/good_ai_22.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/gremcat_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/gremcat_oo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/mlops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:00:19.908265 uo_puddles-1.90/uo_puddles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 21:00:19.000000 uo_puddles-1.90/uo_puddles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-01 21:00:19.000000 uo_puddles-1.90/uo_puddles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:00:19.000000 uo_puddles-1.90/uo_puddles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 21:00:19.000000 uo_puddles-1.90/uo_puddles.egg-info/top_level.txt
```

### Comparing `uo_puddles-1.89/LICENSE.txt` & `uo_puddles-1.90/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.89/setup.py` & `uo_puddles-1.90/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="uo_puddles",
-    version="1.89",    #also change pypi_version variable at top of library
+    version="1.90",    #also change pypi_version variable at top of library
     author="Stephen Fickas",
     author_email="stephenfickas@gmail.com",
     description="for cis423 class",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `uo_puddles-1.89/uo_puddles/cis423.py` & `uo_puddles-1.90/uo_puddles/cis423.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.89/uo_puddles/good_ai.py` & `uo_puddles-1.90/uo_puddles/good_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,17 +447,19 @@
   assert isinstance(test_table, pd.core.frame.DataFrame), f'Puddles says: expecting test_table to be table but instead got a {type(test_table)}!'
   assert isinstance(architecture, list) or isinstance(architecture, tuple), f'architecture is a list or tuple, the number of nodes per layer. Instead got {type(architecture)}'
   assert architecture, f'architecture cannot be the empty list'
   assert all([isinstance(x,int) and x>0 for x in architecture]), f'Puddles says: architecture must contain integers greater than 0'
   assert target in set(train_table.columns)
   assert target in set(test_table.columns)
 
+  tf.keras.utils.set_random_seed(1234)  #need now for replication
+  tf.config.experimental.enable_op_determinism()  #https://www.tensorflow.org/api_docs/python/tf/config/experimental/enable_op_determinism
 
-  np.random.seed(seed=1234)
-  tf.random.set_seed(1234)
+  #np.random.seed(seed=1234)
+  #tf.random.set_seed(1234)
 
   columns = up_list_column_names(train_table)
   new_train = train_table.drop(columns=target).to_numpy()
   labels = np.array(up_get_column(train_table, target))
   new_test = test_table.drop(columns=target).to_numpy()
   n = len(columns)-1
 
@@ -503,14 +505,15 @@
   batch = 20
   epochs = 100
   training = model.fit(x=new_train,
                           y=labels,
                           batch_size=batch,
                           epochs=epochs,
                           verbose=0,
+                          shuffle=True,   #this is new but should be controlled by setting seed
                           callbacks=[early_stop_cb])
   print(f'Finished training with {len(training.history["loss"])} epochs ...')
   '''
   plt.plot(training.history['binary_accuracy'])
   plt.title('model accuracy')
   plt.ylabel('accuracy')
   plt.xlabel('epoch')
```

### Comparing `uo_puddles-1.89/uo_puddles/good_ai_22.py` & `uo_puddles-1.90/uo_puddles/good_ai_22.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.89/uo_puddles/gremcat_df.py` & `uo_puddles-1.90/uo_puddles/gremcat_df.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.89/uo_puddles/gremcat_oo.py` & `uo_puddles-1.90/uo_puddles/gremcat_oo.py`

 * *Files identical despite different names*

