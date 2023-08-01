# Comparing `tmp/AugmentedSocialScientist-2.0.1.tar.gz` & `tmp/AugmentedSocialScientist-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AugmentedSocialScientist-2.0.1.tar", last modified: Fri Jul 28 16:25:28 2023, max compression
+gzip compressed data, was "AugmentedSocialScientist-2.0.2.tar", last modified: Tue Aug  1 13:24:34 2023, max compression
```

## Comparing `AugmentedSocialScientist-2.0.1.tar` & `AugmentedSocialScientist-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-28 16:25:28.732818 AugmentedSocialScientist-2.0.1/
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-28 16:25:28.729346 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/
--rw-r--r--   0 rubing     (501) staff       (20)      434 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/__init__.py
--rw-r--r--   0 rubing     (501) staff       (20)     1221 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/bert_abc.py
--rw-r--r--   0 rubing     (501) staff       (20)    19661 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/bert_base.py
--rw-r--r--   0 rubing     (501) staff       (20)     4604 2023-07-28 16:13:40.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/models.py
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-28 16:25:28.732529 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/
--rw-r--r--   0 rubing     (501) staff       (20)     5735 2023-07-28 16:25:27.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/PKG-INFO
--rw-r--r--   0 rubing     (501) staff       (20)      469 2023-07-28 16:25:28.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/SOURCES.txt
--rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-28 16:25:27.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/dependency_links.txt
--rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/not-zip-safe
--rw-r--r--   0 rubing     (501) staff       (20)       63 2023-07-28 16:25:28.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/requires.txt
--rw-r--r--   0 rubing     (501) staff       (20)       25 2023-07-28 16:25:28.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/top_level.txt
--rw-r--r--   0 rubing     (501) staff       (20)     1068 2023-07-14 19:52:59.000000 AugmentedSocialScientist-2.0.1/LICENSE
--rw-r--r--   0 rubing     (501) staff       (20)     5735 2023-07-28 16:25:28.732951 AugmentedSocialScientist-2.0.1/PKG-INFO
--rw-r--r--   0 rubing     (501) staff       (20)     5269 2023-07-28 16:21:34.000000 AugmentedSocialScientist-2.0.1/README.md
--rw-r--r--   0 rubing     (501) staff       (20)       79 2023-07-28 16:25:28.733491 AugmentedSocialScientist-2.0.1/setup.cfg
--rw-r--r--   0 rubing     (501) staff       (20)      853 2023-07-28 16:16:23.000000 AugmentedSocialScientist-2.0.1/setup.py
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-08-01 13:24:34.652019 AugmentedSocialScientist-2.0.2/
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-08-01 13:24:34.647616 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/
+-rw-r--r--   0 rubing     (501) staff       (20)      434 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/__init__.py
+-rw-r--r--   0 rubing     (501) staff       (20)     1591 2023-08-01 13:14:40.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/bert_abc.py
+-rw-r--r--   0 rubing     (501) staff       (20)    20288 2023-08-01 13:15:21.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/bert_base.py
+-rw-r--r--   0 rubing     (501) staff       (20)     4605 2023-08-01 13:15:51.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/models.py
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-08-01 13:24:34.651616 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/
+-rw-r--r--   0 rubing     (501) staff       (20)     5715 2023-08-01 13:24:34.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/PKG-INFO
+-rw-r--r--   0 rubing     (501) staff       (20)      469 2023-08-01 13:24:34.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/SOURCES.txt
+-rw-r--r--   0 rubing     (501) staff       (20)        1 2023-08-01 13:24:34.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/dependency_links.txt
+-rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/not-zip-safe
+-rw-r--r--   0 rubing     (501) staff       (20)       63 2023-08-01 13:24:34.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/requires.txt
+-rw-r--r--   0 rubing     (501) staff       (20)       25 2023-08-01 13:24:34.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/top_level.txt
+-rw-r--r--   0 rubing     (501) staff       (20)     1068 2023-07-14 19:52:59.000000 AugmentedSocialScientist-2.0.2/LICENSE
+-rw-r--r--   0 rubing     (501) staff       (20)     5715 2023-08-01 13:24:34.652210 AugmentedSocialScientist-2.0.2/PKG-INFO
+-rw-r--r--   0 rubing     (501) staff       (20)     5269 2023-07-28 16:21:34.000000 AugmentedSocialScientist-2.0.2/README.md
+-rw-r--r--   0 rubing     (501) staff       (20)       79 2023-08-01 13:24:34.652886 AugmentedSocialScientist-2.0.2/setup.cfg
+-rw-r--r--   0 rubing     (501) staff       (20)      853 2023-08-01 13:17:32.000000 AugmentedSocialScientist-2.0.2/setup.py
```

### Comparing `AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/bert_base.py` & `AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/bert_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import datetime
 import random
 import time
 import os
+from typing import List, Tuple, Any
 
 import numpy as np
 import torch
 from scipy.special import softmax
+from torch.types import Device
 from torch.utils.data import TensorDataset, SequentialSampler, DataLoader
 from tqdm.auto import tqdm
 from sklearn.metrics import classification_report, precision_recall_fscore_support
 from transformers import BertForSequenceClassification, BertTokenizer, AdamW, get_linear_schedule_with_warmup,\
                             WEIGHTS_NAME, CONFIG_NAME
 
 from AugmentedSocialScientist.bert_abc import BertABC
 
 
 class BertBase(BertABC):
     def __init__(
             self,
-            model_name='bert-base-uncased',
-            tokenizer=BertTokenizer,
-            model_sequence_classifier=BertForSequenceClassification,
-            device=None,
-
+            model_name: str = 'bert-base-uncased',
+            tokenizer: Any = BertTokenizer,
+            model_sequence_classifier: Any = BertForSequenceClassification,
+            device: Device | None = None,
     ):
         """
             Parameters
             ----------
             model_name: str, default='bert-base-uncased'
                     a model name from huggingface models: https://huggingface.co/models
 
@@ -58,19 +59,20 @@
             # If not...
             else:
                 self.device = torch.device("cpu")
                 print('No GPU available, using the CPU instead.')
 
     def encode(
             self,
-            sequences,
-            labels=None,
-            batch_size=32,
-            progress_bar=True
-    ):
+            sequences: List[str],
+            labels: List[str | int] | None = None,
+            batch_size: int = 32,
+            progress_bar: bool = True,
+            add_special_tokens: bool = True
+    ) -> DataLoader:
         """
             Preprocessing of the training, test or prediction data.
             The function will:
                 (1) tokenize the sequences and map tokens to theirs IDs;
                 (2) truncate or pad to 512 tokens (limit for BERT), create corresponding attention masks;
                 (3) return a pytorch dataloader object containing token ids, labels and attention masks.
 
@@ -84,14 +86,16 @@
 
             batch_size: int, default=32
                 batch size for pytorch dataloader
 
             progress_bar: bool, default=True
                 if True, print progress bar for the processing
 
+            add_special_tokens: bool, default=True
+                if True, add '[CLS]' and '[SEP]' tokens
 
             Return
             ------
             dataloader:
                 pytorch dataloader object containing token ids, labels and attention masks
 
             """
@@ -102,19 +106,20 @@
             sent_loader = sequences
         for sent in sent_loader:
             # `encode` will:
             #   (1) Tokenize the sequence.
             #   (2) Prepend the `[CLS]` token to the start.
             #   (3) Append the `[SEP]` token to the end.
             #   (4) Map tokens to their IDs.
-            encoded_sent = self.tokenizer.encode(sent,  # Sequence to encode.
-                                            add_special_tokens=True  # Add '[CLS]' and '[SEP]'
-                                            # max_length = 128,          # Truncate all sequences.
-                                            # return_tensors = 'pt',     # Return pytorch tensors.
-                                            )
+            encoded_sent = self.tokenizer.encode(
+                sent,  # Sequence to encode.
+                add_special_tokens=add_special_tokens  # Add '[CLS]' and '[SEP]'
+                # max_length = 128,          # Truncate all sequences.
+                # return_tensors = 'pt',     # Return pytorch tensors.
+            )
             input_ids.append(encoded_sent)
 
         max_len = min(max([len(sen) for sen in input_ids]), 512)
 
         # Pad the input tokens with value 0 and truncate to MAX_LEN
         pad = np.full((len(input_ids), max_len), 0, dtype='long')
         for idx, s in enumerate(input_ids):
@@ -145,15 +150,15 @@
             # Create the DataLoader
             data = TensorDataset(inputs_tensors, masks_tensors)
             sampler = SequentialSampler(data)
             dataloader = DataLoader(data, sampler=sampler, batch_size=batch_size)
             return dataloader
         else:
 
-            label_names = np.unique(labels) # unique label names in alphabetical order
+            label_names = np.unique(labels)  # unique label names in alphabetical order
             self.dict_labels = dict(zip(label_names, range(len(label_names))))
 
             print(f"label ids: {self.dict_labels}")
 
             # Convert to pytorch tensors
             inputs_tensors = torch.tensor(input_ids)
             masks_tensors = torch.tensor(attention_masks)
@@ -163,21 +168,21 @@
             data = TensorDataset(inputs_tensors, masks_tensors, labels_tensors)
             sampler = SequentialSampler(data)
             dataloader = DataLoader(data, sampler=sampler, batch_size=batch_size)
             return dataloader
 
     def run_training(
             self,
-            train_dataloader,
-            test_dataloader,
-            n_epochs=3,
-            lr=5e-5,
-            random_state=42,
-            save_model_as=None
-    ):
+            train_dataloader: DataLoader,
+            test_dataloader: DataLoader,
+            n_epochs: int = 3,
+            lr: float = 5e-5,
+            random_state: int = 42,
+            save_model_as: str | None = None
+    ) -> Tuple[Any, Any, Any, Any]:
         """
             Train, evaluate and save a BERT model.
 
             Parameters
             ----------
             train_dataloader: torch.Dataloader 
                 training dataloader obtained with self.encode()
@@ -191,20 +196,21 @@
             lr: float, default=5e-5
                 learning rate
 
             random_state: int, default=42
                 random state (for replicability)
 
             save_model_as: str, default=None
-                name of model to save as. The model will be saved at ./models/<model_name>. If None, not saving the model after training
+                name of model to save as. The model will be saved at ./models/<model_name>. If None, not saving the
+                model after training
 
 
             Return
             ------
-            scores: tuplet, 4 arrays of shape (n_labels,)
+            scores: tuple, 4 arrays of shape (n_labels,)
                 evaluation scores: precision, recall, f1-score and support for each label
             """
 
         # Unpack all test labels for evaluation
         test_labels = []
         for batch in test_dataloader:
             test_labels += batch[2].numpy().tolist()
@@ -358,28 +364,32 @@
             avg_test_loss = total_test_loss / len(test_dataloader)
             # Store the loss value for plotting the learning curve.
             test_loss_values.append(avg_test_loss)
 
             print("")
             print("  Average test loss: {0:.2f}".format(avg_test_loss))
             print("  Validation took: {:}".format(self.format_time(time.time() - t0)))
-            print(classification_report(test_labels, np.argmax(logits_complete, axis=1).flatten(), target_names = label_names))
+            print(classification_report(test_labels, np.argmax(logits_complete, axis=1).flatten(),
+                                        target_names=label_names))
             scores = precision_recall_fscore_support(test_labels, np.argmax(logits_complete, axis=1).flatten())
 
         # End of all epochs
         print("")
         print("Training complete!")
 
         if save_model_as is not None:
             # SAVE
             output_dir = "./models/{}".format(save_model_as)
             try:
                 os.makedirs(output_dir)
-            except:
-                pass
+            except FileExistsError:
+                raise FileExistsError(f"The directory {save_model_as} already exists.")
+            except OSError as e:
+                raise OSError(f"Error creating the directory {save_model_as}: {e}")
+
             # Step 1: Save a model, configuration and vocabulary that you have fine-tuned
 
             # If we have a distributed model, save only the encapsulated model
             # (it was wrapped in PyTorch DistributedDataParallel or DataParallel)
             model_to_save = model.module if hasattr(model, 'module') else model
 
             # If we save using the predefined names, we can load using `from_pretrained`
@@ -388,21 +398,20 @@
 
             torch.save(model_to_save.state_dict(), output_model_file)
             model_to_save.config.to_json_file(output_config_file)
             self.tokenizer.save_vocabulary(output_dir)
 
         return scores
 
-
     def predict(
             self,
-            dataloader,
-            model,
-            proba=True,
-            progress_bar=True
+            dataloader: DataLoader,
+            model: Any,
+            proba: bool = True,
+            progress_bar: bool = True
     ):
         """
         Prediction with a trained model.
 
         Parameters
         ----------
         dataloader: torch.Dataloader 
@@ -425,27 +434,26 @@
         logits_complete = []
         # Evaluate data for one epoch
         if progress_bar:
             loader = tqdm(dataloader)
         else:
             loader = dataloader
 
-        pred = None
         for batch in loader:
 
             # Add batch to GPU
             batch = tuple(t.to(self.device) for t in batch)
 
             # Unpack the inputs from our dataloader
             if len(batch) == 3:
                 b_input_ids, b_input_mask, _ = batch
             else:
                 b_input_ids, b_input_mask = batch
 
-            # Telling the model not to compute or store gradients, saving memory andspeeding up validation
+            # Telling the model not to compute or store gradients, saving memory and speeding up validation
             with torch.no_grad():
                 outputs = model(b_input_ids,
                                 token_type_ids=None,  # not a 2-sentence task
                                 attention_mask=b_input_mask)
 
             # Get the "logits" output by the model. The "logits" are the output
             # values prior to applying an activation function like the softmax.
@@ -460,18 +468,18 @@
         pred = np.concatenate(logits_complete)  # flatten batches
         print(f"label ids: {self.dict_labels}")
 
         return softmax(pred, axis=1) if proba else pred
 
     def predict_with_model(
             self,
-            dataloader,
-            model_path,
-            proba=True,
-            progress_bar=True
+            dataloader: DataLoader,
+            model_path: str,
+            proba: bool = True,
+            progress_bar: bool = True
     ):
         """
         Prediction with a locally saved model.
 
         Parameters
         ----------
         dataloader: torch.Dataloader 
@@ -492,15 +500,14 @@
             probabilities for each sequence (row) of belonging to each category (column)
         """
         model = self.model_sequence_classifier.from_pretrained(model_path)
         if torch.cuda.is_available():
             model.cuda()
         return self.predict(dataloader, model, proba, progress_bar)
 
- 
     def format_time(
             self,
             elapsed: float | int
     ):
         """
         Format a time to hh:mm:ss.
 
@@ -509,8 +516,8 @@
         elapsed: float, elapsed time
 
         Returns
         -------
 
         """
         elapsed_rounded = int(round(elapsed))
-        return str(datetime.timedelta(seconds=elapsed_rounded))  # Format as hh:mm:ss
+        return str(datetime.timedelta(seconds=elapsed_rounded))  # Format as hh:mm:ss
```

### Comparing `AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/models.py` & `AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -167,8 +167,8 @@
             device=None
     ):
         super().__init__(
             model_name=model_name,
             tokenizer=XLMRobertaTokenizer,
             device=device,
             model_sequence_classifier=XLMRobertaForSequenceClassification
-        )
+        )
```

### Comparing `AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/PKG-INFO` & `AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: AugmentedSocialScientist
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Package to Easily Train Bert-Like Models for Text Classification
 Home-page: https://github.com/rubingshen/AugmentedSocialScientist
-Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.1.tar.gz
+Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.2.tar.gz
 Author: Rubing Shen
 Author-email: shenrubing1996@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The Augmented Social Scientist
 
 **New release v2**
 
@@ -158,9 +157,7 @@
 By default, the package automatically detects the presence of a GPU and uses it to accelerate computation. You can also set your own device, by providing a `torch.Device` object to the parameter `device` when instanciating `Bert`.
 
 ```python
 from AugmentedSocialScientist.models import Bert
 
 bert = Bert(device=...)  #set your own device
 ```
-
-
```

### Comparing `AugmentedSocialScientist-2.0.1/LICENSE` & `AugmentedSocialScientist-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-2.0.1/PKG-INFO` & `AugmentedSocialScientist-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: AugmentedSocialScientist
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Package to Easily Train Bert-Like Models for Text Classification
 Home-page: https://github.com/rubingshen/AugmentedSocialScientist
-Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.1.tar.gz
+Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.2.tar.gz
 Author: Rubing Shen
 Author-email: shenrubing1996@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The Augmented Social Scientist
 
 **New release v2**
 
@@ -158,9 +157,7 @@
 By default, the package automatically detects the presence of a GPU and uses it to accelerate computation. You can also set your own device, by providing a `torch.Device` object to the parameter `device` when instanciating `Bert`.
 
 ```python
 from AugmentedSocialScientist.models import Bert
 
 bert = Bert(device=...)  #set your own device
 ```
-
-
```

### Comparing `AugmentedSocialScientist-2.0.1/README.md` & `AugmentedSocialScientist-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-2.0.1/setup.py` & `AugmentedSocialScientist-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description = fh.read()
     
 setup(name='AugmentedSocialScientist',
       author='Rubing Shen',
       license='MIT',
       author_email='shenrubing1996@gmail.com',
       url='https://github.com/rubingshen/AugmentedSocialScientist',
-      download_url='https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.1.tar.gz',
-      version='2.0.1',
+      download_url='https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.2.tar.gz',
+      version='2.0.2',
       description='A Package to Easily Train Bert-Like Models for Text Classification',
       long_description=long_description,
       long_description_content_type="text/markdown",
       packages=['AugmentedSocialScientist'],
       zip_safe=False,
       install_requires=environment)
```

