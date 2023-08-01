# Comparing `tmp/sim4rec-0.0.1.tar.gz` & `tmp/sim4rec-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sim4rec-0.0.1.tar", max compression
+gzip compressed data, was "sim4rec-0.0.2.tar", max compression
```

## Comparing `sim4rec-0.0.1.tar` & `sim4rec-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-06-14 09:30:59.819918 sim4rec-0.0.1/LICENSE
--rw-r--r--   0        0        0     4039 2023-06-14 09:30:59.820130 sim4rec-0.0.1/README.md
--rw-r--r--   0        0        0      660 2023-06-14 09:30:59.884544 sim4rec-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-14 09:30:59.885236 sim4rec-0.0.1/sim4rec/__init__.py
--rw-r--r--   0        0        0      912 2023-06-14 09:30:59.885747 sim4rec-0.0.1/sim4rec/modules/__init__.py
--rw-r--r--   0        0        0     6938 2023-06-14 09:30:59.886191 sim4rec-0.0.1/sim4rec/modules/embeddings.py
--rw-r--r--   0        0        0    14003 2023-06-14 09:30:59.886642 sim4rec-0.0.1/sim4rec/modules/evaluation.py
--rw-r--r--   0        0        0    12306 2023-06-14 09:30:59.886886 sim4rec-0.0.1/sim4rec/modules/generator.py
--rw-r--r--   0        0        0     4430 2023-06-14 09:30:59.887058 sim4rec-0.0.1/sim4rec/modules/selectors.py
--rw-r--r--   0        0        0     7507 2023-06-14 09:30:59.887289 sim4rec-0.0.1/sim4rec/modules/simulator.py
--rw-r--r--   0        0        0      565 2023-06-14 09:30:59.887519 sim4rec-0.0.1/sim4rec/params/__init__.py
--rw-r--r--   0        0        0     5858 2023-06-14 09:30:59.887654 sim4rec-0.0.1/sim4rec/params/params.py
--rw-r--r--   0        0        0      397 2023-06-14 09:30:59.887835 sim4rec-0.0.1/sim4rec/response/__init__.py
--rw-r--r--   0        0        0     7294 2023-06-14 09:30:59.887971 sim4rec-0.0.1/sim4rec/response/response.py
--rw-r--r--   0        0        0      290 2023-06-14 09:30:59.888179 sim4rec-0.0.1/sim4rec/utils/__init__.py
--rw-r--r--   0        0        0      845 2023-06-14 09:30:59.888296 sim4rec-0.0.1/sim4rec/utils/convert.py
--rw-r--r--   0        0        0     2412 2023-06-14 09:30:59.888454 sim4rec-0.0.1/sim4rec/utils/uce.py
--rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 sim4rec-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-08-01 14:55:48.817603 sim4rec-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5140 2023-08-01 14:55:48.817762 sim4rec-0.0.2/README.md
+-rw-r--r--   0        0        0      854 2023-08-01 14:55:48.888363 sim4rec-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 14:55:48.889101 sim4rec-0.0.2/sim4rec/__init__.py
+-rw-r--r--   0        0        0      912 2023-08-01 14:55:48.889439 sim4rec-0.0.2/sim4rec/modules/__init__.py
+-rw-r--r--   0        0        0     7347 2023-08-01 14:55:48.889762 sim4rec-0.0.2/sim4rec/modules/embeddings.py
+-rw-r--r--   0        0        0    14302 2023-08-01 14:55:48.890187 sim4rec-0.0.2/sim4rec/modules/evaluation.py
+-rw-r--r--   0        0        0    12645 2023-08-01 14:55:48.890567 sim4rec-0.0.2/sim4rec/modules/generator.py
+-rw-r--r--   0        0        0     4654 2023-08-01 14:55:48.890874 sim4rec-0.0.2/sim4rec/modules/selectors.py
+-rw-r--r--   0        0        0     7967 2023-08-01 14:55:48.891357 sim4rec-0.0.2/sim4rec/modules/simulator.py
+-rw-r--r--   0        0        0      565 2023-08-01 14:55:48.891805 sim4rec-0.0.2/sim4rec/params/__init__.py
+-rw-r--r--   0        0        0     8294 2023-08-01 14:55:48.892207 sim4rec-0.0.2/sim4rec/params/params.py
+-rw-r--r--   0        0        0      397 2023-08-01 14:55:48.892634 sim4rec-0.0.2/sim4rec/response/__init__.py
+-rw-r--r--   0        0        0     7656 2023-08-01 14:55:48.892969 sim4rec-0.0.2/sim4rec/response/response.py
+-rw-r--r--   0        0        0      290 2023-08-01 14:55:48.893321 sim4rec-0.0.2/sim4rec/utils/__init__.py
+-rw-r--r--   0        0        0      841 2023-08-01 14:55:48.893507 sim4rec-0.0.2/sim4rec/utils/convert.py
+-rw-r--r--   0        0        0     2843 2023-08-01 14:55:48.893698 sim4rec-0.0.2/sim4rec/utils/uce.py
+-rw-r--r--   0        0        0     5786 1970-01-01 00:00:00.000000 sim4rec-0.0.2/PKG-INFO
```

### Comparing `sim4rec-0.0.1/LICENSE` & `sim4rec-0.0.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 Sber AI Lab
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `sim4rec-0.0.1/sim4rec/modules/__init__.py` & `sim4rec-0.0.2/sim4rec/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `sim4rec-0.0.1/sim4rec/modules/embeddings.py` & `sim4rec-0.0.2/sim4rec/modules/embeddings.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,89 +12,102 @@
 from pyspark.ml.util import DefaultParamsReadable, DefaultParamsWritable
 from pyspark.ml.param.shared import HasInputCols, HasOutputCols
 
 from sim4rec.params import HasDevice, HasSeed
 
 
 class Encoder(torch.nn.Module):
+    """
+    Encoder layer
+    """
     def __init__(
         self,
         input_dim : int,
         hidden_dim : int,
         latent_dim : int
     ):
         super().__init__()
 
         input_dims = [input_dim, hidden_dim, latent_dim]
         self._layers = torch.nn.ModuleList([
             torch.nn.Linear(_in, _out)
             for _in, _out in zip(input_dims[:-1], input_dims[1:])
         ])
 
-
     def forward(self, X):
+        """
+        Performs forward pass through layer
+        """
         X = F.normalize(X, p=2)
         for layer in self._layers[:-1]:
             X = layer(X)
             X = F.leaky_relu(X)
 
         X = self._layers[-1](X)
 
         return X
 
 
 class Decoder(torch.nn.Module):
+    """
+    Decoder layer
+    """
     def __init__(
         self,
         input_dim : int,
         hidden_dim : int,
         latent_dim : int
     ):
         super().__init__()
 
         input_dims = [latent_dim, hidden_dim, input_dim]
         self._layers = torch.nn.ModuleList([
             torch.nn.Linear(_in, _out)
             for _in, _out in zip(input_dims[:-1], input_dims[1:])
         ])
 
-
     def forward(self, X):
+        """
+        Performs forward pass through layer
+        """
         for layer in self._layers[:-1]:
             X = layer(X)
             X = F.leaky_relu(X)
 
         X = self._layers[-1](X)
 
         return X
 
 
+# pylint: disable=too-many-ancestors
 class EncoderEstimator(Estimator,
                        HasInputCols,
                        HasOutputCols,
                        HasDevice,
                        HasSeed,
                        DefaultParamsReadable,
                        DefaultParamsWritable):
+    """
+    Estimator for encoder part of the autoencoder pipeline. Trains
+    the encoder to process incoming data into latent representation
+    """
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         inputCols : List[str],
         outputCols : List[str],
         hidden_dim : int,
         lr : float,
         batch_size : int,
         num_loader_workers : int,
         max_iter : int = 100,
         device_name : str = 'cpu',
         seed : int = None
     ):
         """
-        Estimator for encoder part of the autoencoder pipeline. Trains
-        the encoder to process incoming data into latent representation
-
         :param inputCols: Column names to process
         :param outputCols: List of output column names per latent coordinate.
             The length of outputCols will determine the embedding dimension size
         :param hidden_dim: Size of hidden layers
         :param lr: Learning rate
         :param batch_size: Batch size during training process
         :param num_loader_workers: Number of cpus to use for data loader
@@ -113,32 +126,31 @@
         self._latent_dim = len(outputCols)
 
         self._lr = lr
         self._batch_size = batch_size
         self._num_loader_workers = num_loader_workers
         self._max_iter = max_iter
 
-        
-
+    # pylint: disable=too-many-locals, not-callable
     def _fit(
         self,
-        df : DataFrame
+        dataset : DataFrame
     ):
         inputCols = self.getInputCols()
         outputCols = self.getOutputCols()
         device_name = self.getDevice()
         seed = self.getSeed()
         device = torch.device(self.getDevice())
 
-        X = df.select(*inputCols).toPandas().values
+        X = dataset.select(*inputCols).toPandas().values
 
         torch.manual_seed(torch.seed() if seed is None else seed)
 
         train_loader = DataLoader(X, batch_size=self._batch_size,
-            shuffle=True, num_workers=self._num_loader_workers)
+                                  shuffle=True, num_workers=self._num_loader_workers)
 
         encoder = Encoder(
             input_dim=self._input_dim,
             hidden_dim=self._hidden_dim,
             latent_dim=self._latent_dim
         )
         decoder = Decoder(
@@ -148,15 +160,15 @@
         )
 
         model = torch.nn.Sequential(encoder, decoder).to(torch.device(self.getDevice()))
 
         optimizer = opt.Adam(model.parameters(), lr=self._lr)
         crit = torch.nn.MSELoss()
 
-        for i in range(self._max_iter):
+        for _ in range(self._max_iter):
             loss = 0
             for X_batch in train_loader:
                 X_batch = X_batch.float().to(device)
 
                 optimizer.zero_grad()
 
                 pred = model(X_batch)
@@ -179,26 +191,27 @@
 
 class EncoderTransformer(Transformer,
                          HasInputCols,
                          HasOutputCols,
                          HasDevice,
                          DefaultParamsReadable,
                          DefaultParamsWritable):
+    """
+    Encoder transformer that transforms incoming columns into latent
+    representation. Output data will be appended to dataframe and
+    named according to outputCols parameter
+    """
     def __init__(
         self,
         inputCols : List[str],
         outputCols : List[str],
         encoder : Encoder,
         device_name : str = 'cpu'
     ):
         """
-        Encoder transformer that transforms incoming columns into latent
-        representation. Output data will be appended to dataframe and
-        named according to outputCols parameter
-
         :param inputCols: Column names to process
         :param outputCols: List of output column names per latent coordinate.
             The length of outputCols must be equal to embedding dimension of
             a trained encoder
         :param encoder: Trained encoder
         :param device_name: PyTorch device name, defaults to 'cpu'
         """
@@ -210,17 +223,18 @@
         self.setDevice(device_name)
 
     def setDevice(self, value):
         super().setDevice(value)
 
         self._encoder.to(torch.device(value))
 
+    # pylint: disable=not-callable
     def _transform(
         self,
-        df : DataFrame
+        dataset : DataFrame
     ):
         inputCols = self.getInputCols()
         outputCols = self.getOutputCols()
         device = torch.device(self.getDevice())
 
         encoder = self._encoder
 
@@ -233,8 +247,8 @@
                     columns=outputCols
                 )
 
         schema = st.StructType(
             [st.StructField(c, st.FloatType()) for c in outputCols]
         )
 
-        return df.mapInPandas(encode, schema)
+        return dataset.mapInPandas(encode, schema)
```

### Comparing `sim4rec-0.0.1/sim4rec/modules/evaluation.py` & `sim4rec-0.0.2/sim4rec/modules/evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from abc import ABC
 from typing import List, Union, Dict, Optional
 
 import numpy as np
 from scipy.stats import kstest
+# TL;DR scipy.special is a C library, pylint needs python source code
+# https://github.com/pylint-dev/pylint/issues/3703
+# pylint: disable=no-name-in-module
 from scipy.special import kl_div
 
 import pyspark.sql.functions as sf
 from pyspark.sql import DataFrame
 from pyspark.ml.evaluation import (
     BinaryClassificationEvaluator,
     RegressionEvaluator,
@@ -24,18 +27,22 @@
     synth_df : DataFrame,
     real_df : DataFrame
 ) -> dict:
     """
     Evaluates the quality of synthetic data against real. The following
     metrics will be calculated:
 
-    - LogisticDetection: The metric evaluates how hard it is to distinguish the synthetic data from the real data by using a Logistic regression model
-    - SVCDetection: The metric evaluates how hard it is to distinguish the synthetic data from the real data by using a C-Support Vector Classification model
-    - KSTest: This metric uses the two-sample Kolmogorov-Smirnov test to compare the distributions of continuous columns using the empirical CDF
-    - ContinuousKLDivergence: This approximates the KL divergence by binning the continuous values to turn them into categorical values and then computing the relative entropy
+    - LogisticDetection: The metric evaluates how hard it is to distinguish the synthetic
+    data from the real data by using a Logistic regression model
+    - SVCDetection: The metric evaluates how hard it is to distinguish the synthetic data
+    from the real data by using a C-Support Vector Classification model
+    - KSTest: This metric uses the two-sample Kolmogorov-Smirnov test to compare
+    the distributions of continuous columns using the empirical CDF
+    - ContinuousKLDivergence: This approximates the KL divergence by binning the continuous values
+    to turn them into categorical values and then computing the relative entropy
 
     :param synth_df: Synthetic data without any identifiers
     :param real_df: Real data without any identifiers
     :return: Dictionary with metrics on synthetic data quality
     """
 
     result = evaluate(
@@ -48,16 +55,16 @@
             'ContinuousKLDivergence'
         ],
         aggregate=False
     )
 
     return {
         row['metric'] : row['normalized_score']
-            for _, row in result.iterrows()
-        }
+        for _, row in result.iterrows()
+    }
 
 
 def ks_test(
     df : DataFrame,
     predCol : str,
     labelCol : str
 ) -> float:
@@ -71,14 +78,15 @@
     """
 
     pdf = df.select(predCol, labelCol).toPandas()
     rvs, cdf = pdf[predCol].values, pdf[labelCol].values
 
     return kstest(rvs, cdf).statistic
 
+
 def kl_divergence(
     df : DataFrame,
     predCol : str,
     labelCol : str
 ) -> float:
     """
     Normalized Kullback–Leibler divergence on two dataframe columns. The normalization is
@@ -101,53 +109,56 @@
 
     f_obs = f_obs.flatten() + 1e-5
     f_exp = f_exp.flatten() + 1e-5
 
     return 1 / (1 + np.sum(kl_div(f_obs, f_exp)))
 
 
+# pylint: disable=too-few-public-methods
 class QualityControlObjective(ABC):
+    """
+    QualityControlObjective is designed to evaluate the quality of response
+    function by calculating the similarity degree between results of the
+    model, which was trained on real data and a model, trained with
+    simulator. The calculated function is
+
+    .. math::
+        1 - KS(predictionCol, labelCol) + DKL_{norm}(predictionCol, labelCol)
+
+        - \\frac{1}{N} \\sum_{n=1}^{N} |QM_{syn}^{i}(recs_{synthetic},
+        ground\_truth_{synthetic}) - QM_{real}^{i}(recs_{real}, ground\_truth_{real})|,
+
+    where
+
+    .. math::
+        KS = supx||Q(x) - P(x)||\ (i.e.\ KS\ test\ statistic)
+
+        DKL_{norm} = \\frac{1}{1 + DKL}
+
+    The greater value indicates more similarity between models' result
+    and lower value shows dissimilarity. As a predicted value for KS test
+    and KL divergence it takes the result of `response_function` on a
+    pairs from real log and compares the distributions similarity between
+    real responses and predicted. For calculating QM from formula above
+    the metrics from RePlay library are used. Those take ground truth and
+    predicted values for both models and measures how close are metric
+    values to each other.
+    """
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         userKeyCol : str,
         itemKeyCol : str,
         predictionCol : str,
         labelCol : str,
         relevanceCol : str,
         response_function : Transformer,
         replay_metrics : Optional[Dict[Metric, Union[int, List[int]]]],
     ):
         """
-        QualityControlObjective is designed to evaluate the quality of response
-        function by calculating the similarity degree between results of the
-        model, which was trained on real data and a model, trained with
-        simulator. The calculated function is
-
-        .. math::
-            1 - KS(predictionCol, labelCol) + DKL_{norm}(predictionCol, labelCol)
-
-            - \\frac{1}{N} \\sum_{n=1}^{N} |QM_{syn}^{i}(recs_{synthetic},
-            ground\_truth_{synthetic}) - QM_{real}^{i}(recs_{real}, ground\_truth_{real})|,
-
-        where
-
-        .. math::
-            KS = supx||Q(x) - P(x)||\ (i.e.\ KS\ test\ statistic)
-
-            DKL_{norm} = \\frac{1}{1 + DKL}
-
-        The greater value indicates more similarity between models' result
-        and lower value shows dissimilarity. As a predicted value for KS test
-        and KL divergence it takes the result of `response_function` on a
-        pairs from real log and compares the distributions similarity between
-        real responses and predicted. For calculating QM from formula above
-        the metrics from RePlay library are used. Those take ground truth and
-        predicted values for both models and measures how close are metric
-        values to each other.
-
         :param userKeyCol: User identifier column name
         :param itemKeyCol: Item identifier column name
         :param predictionCol: Prediction column name, which `response_function`
             will create
         :param labelCol: Column name with ground truth response values
         :param relevanceCol: Relevance column name for RePlay metrics. For
             ground truth dataframe it should be response score and for
@@ -169,14 +180,15 @@
         self._predictionCol = predictionCol
         self._relevanceCol = relevanceCol
         self._labelCol = labelCol
 
         self._resp_func = response_function
         self._replay_metrics = replay_metrics
 
+    # pylint: disable=too-many-arguments
     def __call__(
         self,
         test_log : DataFrame,
         user_features : DataFrame,
         item_features : DataFrame,
         real_recs : DataFrame,
         real_ground_truth : DataFrame,
@@ -204,16 +216,17 @@
 
         objective = 0
 
         feature_df = test_log.join(user_features, on=self._userKeyCol, how='left')\
                              .join(item_features, on=self._itemKeyCol, how='left')
 
         pred_df = self._resp_func.transform(feature_df)
-        objective = 1 - ks_test(pred_df, self._predictionCol, self._labelCol) +\
-                    kl_divergence(pred_df, self._predictionCol, self._labelCol)
+        objective = (1
+                     - ks_test(pred_df, self._predictionCol, self._labelCol)
+                     + kl_divergence(pred_df, self._predictionCol, self._labelCol))
 
         metrics_values = []
         for r, t in zip((real_recs, synthetic_recs), (real_ground_truth, synthetic_ground_truth)):
             r = r.select(self._userKeyCol, self._itemKeyCol, self._relevanceCol)\
                  .withColumnRenamed(self._userKeyCol, 'user_idx')\
                  .withColumnRenamed(self._itemKeyCol, 'item_idx')\
                  .withColumnRenamed(self._relevanceCol, 'relevance')
@@ -227,50 +240,53 @@
             metrics_values.append(exp.results.values)
 
         objective -= np.abs(metrics_values[0] - metrics_values[1]).mean()
 
         return objective
 
 
+# pylint: disable=too-few-public-methods
 class EvaluateMetrics(ABC):
+    """
+    Recommendation systems and response function metric evaluator class.
+    The class allows you to evaluate the quality of a response function on
+    historical data or a recommender system on historical data or based on
+    the results of an experiment in a simulator. Provides simultaneous
+    calculation of several metrics using metrics from the Spark MLlib and
+    RePlay libraries.
+    A created instance is callable on a dataframe with ``user_id, item_id,
+    predicted relevance/response, true relevance/response`` format, which
+    you can usually retrieve from simulators sample_responses() or log data
+    with recommendation algorithm scores. In case when the RePlay metrics
+    are needed it additionally apply filter on a passed dataframe to take
+    only necessary responses (e.g. when response is equal to 1).
+    """
 
     REGRESSION_METRICS = set(['rmse', 'mse', 'r2', 'mae', 'var'])
     MULTICLASS_METRICS = set([
         'f1', 'accuracy', 'weightedPrecision', 'weightedRecall',
         'weightedTruePositiveRate', 'weightedFalsePositiveRate',
         'weightedFMeasure', 'truePositiveRateByLabel', 'falsePositiveRateByLabel',
         'precisionByLabel', 'recallByLabel', 'fMeasureByLabel',
         'logLoss', 'hammingLoss'
     ])
     BINARY_METRICS = set(['areaUnderROC', 'areaUnderPR'])
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         userKeyCol : str,
         itemKeyCol : str,
         predictionCol : str,
         labelCol : str,
         replay_label_filter : float = 1.0,
         replay_metrics : Optional[Dict[Metric, Union[int, List[int]]]] = None,
         mllib_metrics : Optional[Union[str, List[str]]] = None
     ):
         """
-        Recommendation systems and response function metric evaluator class.
-        The class allows you to evaluate the quality of a response function on
-        historical data or a recommender system on historical data or based on
-        the results of an experiment in a simulator. Provides simultaneous
-        calculation of several metrics using metrics from the Spark MLlib and
-        RePlay libraries.
-        A created instance is callable on a dataframe with ``user_id, item_id,
-        predicted relevance/response, true relevance/response`` format, which
-        you can usually retrieve from simulators sample_responses() or log data
-        with recommendation algorithm scores. In case when the RePlay metrics
-        are needed it additionally apply filter on a passed dataframe to take
-        only necessary responses (e.g. when response is equal to 1).
-
         :param userKeyCol: User identifier column name
         :param itemKeyCol: Item identifier column name
         :param predictionCol: Predicted scores column name
         :param labelCol: True label column name
         :param replay_label_filter: RePlay metrics assume that only positive
             responses are presented in ground truth data. All user-item pairs with
             col(labelCol) >= replay_label_filter condition are treated as positive
@@ -287,15 +303,15 @@
 
         super().__init__()
 
         self._userKeyCol = userKeyCol
         self._itemKeyCol = itemKeyCol
         self._predictionCol = predictionCol
         self._labelCol = labelCol
-        self._filter = (sf.col(self._labelCol) >= replay_label_filter)
+        self._filter = sf.col(self._labelCol) >= replay_label_filter
 
         if isinstance(mllib_metrics, str):
             mllib_metrics = [mllib_metrics]
 
         if replay_metrics is None:
             replay_metrics = {}
         if mllib_metrics is None:
@@ -319,17 +335,17 @@
         df = df.withColumnRenamed(self._userKeyCol, 'user_idx')\
                .withColumnRenamed(self._itemKeyCol, 'item_idx')
 
         result = {}
 
         if len(self._replay_metrics) > 0:
             exp = Experiment(
-                test=df.filter(self._filter)\
-                    .drop(self._predictionCol)\
-                    .withColumnRenamed(self._labelCol, 'relevance'),
+                test=df.filter(self._filter)
+                       .drop(self._predictionCol)
+                       .withColumnRenamed(self._labelCol, 'relevance'),
                 metrics=self._replay_metrics
             )
             exp.add_result(
                 '__dummy',
                 df.drop(self._labelCol).withColumnRenamed(self._predictionCol, 'relevance')
             )
             result.update(exp.results.to_dict(orient='records')[0])
@@ -353,8 +369,8 @@
         if metric in self.BINARY_METRICS:
             return BinaryClassificationEvaluator(
                 metricName=metric, **self._binary_params())
         if metric in self.MULTICLASS_METRICS:
             return MulticlassClassificationEvaluator(
                 metricName=metric, **self._reg_or_multiclass_params())
 
-        raise ValueError(f'Non existing metric was passed: {metric}')
+        raise ValueError(f'Non existing metric was passed: {metric}')
```

### Comparing `sim4rec-0.0.1/sim4rec/modules/generator.py` & `sim4rec-0.0.2/sim4rec/modules/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 from abc import ABC, abstractmethod
-from typing import Iterable, List
+from typing import Iterable, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 import torch
 
 import pyspark.sql.types as st
 from pyspark.sql import DataFrame
@@ -18,22 +18,23 @@
 )
 from sim4rec.utils import (
     NotFittedError, EmptyDataFrameError, save, load
 )
 
 
 class GeneratorBase(ABC, HasLabel, HasDataSize, HasSeedSequence):
+    """
+    Base class for data generators
+    """
     def __init__(
         self,
         label : str,
         seed : int = None
     ):
         """
-        Base class for data generators
-
         :param label: Generator string label
         :param seed: Fixes seed sequence to use during multiple
             generator calls, defaults to None
         """
         super().__init__()
         self.setLabel(label)
         self.setDataSize(0)
@@ -88,14 +89,15 @@
         return self._df.sample(sample_frac, seed=seed)
 
 
 class RealDataGenerator(GeneratorBase):
     """
     Real data generator, which can sample from existing dataframe
     """
+    _source_df : DataFrame
 
     def fit(
         self,
         df : DataFrame
     ) -> None:
         """
         :param df: Dataframe for generation and sampling
@@ -136,43 +138,50 @@
                                   .cache()
         self.setDataSize(self._df.count())
 
         return self._df
 
 
 def set_sdv_seed(seed : int = None):
-    ## this is the only way to fix seed in SDV library
+    """
+    Fixes seed for SDV
+    """
+    # this is the only way to fix seed in SDV library
     np.random.seed(seed)
     random.seed(seed)
     torch.manual_seed(torch.seed() if seed is None else seed)
 
 
+# pylint: disable=too-many-ancestors
 class SDVDataGenerator(GeneratorBase, HasParallelizationLevel, HasDevice):
+    """
+    Synthetic data generator with a bunch of models from SDV library
+    """
+    _model : Optional[Union[CopulaGAN, CTGAN, GaussianCopula, TVAE]] = None
 
     SEED_COLUMN_NAME = '__seed'
 
     _sdv_model_dict = {
         'copulagan' : CopulaGAN,
         'ctgan' : CTGAN,
         'gaussiancopula' : GaussianCopula,
         'tvae' : TVAE
     }
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         label : str,
         id_column_name : str,
         model_name : str = 'gaussiancopula',
         parallelization_level : int = 1,
         device_name : str = 'cpu',
         seed : int = None
     ):
         """
-        Synthetic data generator with a bunch of models from SDV library
-
         :param label: Generator string label
         :param id_column_name: Column name for identifier
         :param model_name: Name of a SDV model. Possible values are:
             ['copulagan', 'ctgan', 'gaussiancopula', 'tvae'],
             defaults to 'gaussiancopula'
         :param parallelization_level: Parallelization level, defaults to 1
         :param device_name: PyTorch device name, defaults to 'cpu'
@@ -182,14 +191,15 @@
 
         super().__init__(label=label, seed=seed)
 
         self.setParallelizationLevel(parallelization_level)
         self._id_col_name = id_column_name
         self._model_name = model_name
         self.setDevice(device_name)
+        self._schema = None
 
     def fit(
         self,
         df : DataFrame
     ) -> None:
         """
         Fits a generation model with a passed dataframe. The one should
@@ -213,27 +223,27 @@
         )
 
         self._model.fit(df.toPandas())
         self._fit_called = True
 
     def setDevice(
         self,
-        device_name : str
+        value : str
     ) -> None:
         """
         Changes the current device. Note, that for gaussiancopula
         model, only cpu is supported
 
         :param device_name: PyTorch device name
         """
 
-        super().setDevice(device_name)
+        super().setDevice(value)
 
         if self._model_name != 'gaussiancopula' and self._fit_called:
-            self._model._model.set_device(torch.device(device_name))
+            self._model._model.set_device(torch.device(value))
 
     def generate(
         self,
         num_samples : int
     ) -> DataFrame:
         """
         Generates a number of samples from fitted dataframe
@@ -323,51 +333,52 @@
         Loads the generator model from the file
 
         :param filename: Path to the file
         :return: Generator instance with restored model
         """
 
         label, id_col_name, model_name, p_level,\
-        device_name, init_seed, model, schema = load(filename)
+            device_name, init_seed, model, schema = load(filename)
 
         generator = SDVDataGenerator(
             label=label,
             id_column_name=id_col_name,
             model_name=model_name,
             parallelization_level=p_level,
             device_name=device_name,
             seed=init_seed
         )
 
         generator._model = model
         generator._fit_called = True
         generator._schema = schema
-        
+
         try:
             generator.setDevice(device_name)
         except RuntimeError:
             print(f'Cannot load model to device {device_name}. Setting cpu instead')
             generator.setDevice('cpu')
 
         return generator
 
 
-
+# pylint: disable=too-many-ancestors
 class CompositeGenerator(GeneratorBase, HasWeights):
+    """
+    Wrapper for sampling from multiple generators. Use weights
+    parameter to control the sampling fraction for each of the
+    generator
+    """
     def __init__(
         self,
         generators : List[GeneratorBase],
         label : str,
         weights : Iterable = None,
     ):
         """
-        Wrapper for sampling from multiple generators. Use weights
-        parameter to control the sampling fraction for each of the
-        generator 
-
         :param generators: List of generators
         :param label: Generator string label
         :param weights: Weights for each of the generator. Weights
             must be normalized (sums to 1), defaults to None
         """
 
         super().__init__(label=label)
@@ -392,15 +403,15 @@
     ) -> None:
         """
         For each generator calls generate() with number of samples,
         proportional to weights to generate num_samples in total. You
         can call this method to not perform generate() separately on
         each generator
 
-        :param num_samples: Total number of samples to generate 
+        :param num_samples: Total number of samples to generate
         """
 
         weights = self.getWeights()
         num_required_samples = [round(num_samples * w) for w in weights]
 
         for g, n in zip(self._generators, num_required_samples):
             _ = g.generate(n)
@@ -423,15 +434,17 @@
         data_sizes = [g.getDataSize() for g in self._generators]
         data_sizes_sum = sum(data_sizes)
 
         num_required_samples = [int(data_sizes_sum * sample_frac * w) for w in weights]
 
         for i in range(len(data_sizes)):
             if num_required_samples[i] > data_sizes[i]:
-                raise ValueError(f'Not enough samples in generator {self._generators[i].getLabel()}')
+                raise ValueError(
+                    f'Not enough samples in generator {self._generators[i].getLabel()}'
+                )
 
         generator_fracs = []
         for n, s in zip(num_required_samples, data_sizes):
             generator_fracs.append(0.0 if s == 0 else n / s)
 
         result_df = self._generators[0].sample(generator_fracs[0])
```

### Comparing `sim4rec-0.0.1/sim4rec/modules/selectors.py` & `sim4rec-0.0.2/sim4rec/modules/selectors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,80 +1,87 @@
+# pylint: disable=no-member,unused-argument,too-many-ancestors,abstract-method
 from pyspark.sql import functions as sf
 from pyspark.sql import DataFrame
 from pyspark.ml import Transformer, Estimator
 from pyspark.ml.util import DefaultParamsReadable, DefaultParamsWritable
 from pyspark import keyword_only
 from sim4rec.params import HasUserKeyColumn, HasItemKeyColumn, HasSeed, HasSeedSequence
 
 
 class ItemSelectionEstimator(Estimator,
                              HasUserKeyColumn,
                              HasItemKeyColumn,
                              DefaultParamsReadable,
                              DefaultParamsWritable):
+    """
+    Base class for item selection estimator
+    """
     @keyword_only
     def __init__(
         self,
         userKeyColumn : str = None,
         itemKeyColumn : str = None
     ):
-        """
-        Base class for item selection estimator
-        """
-
         super().__init__()
         self.setParams(**self._input_kwargs)
 
     @keyword_only
     def setParams(
         self,
         userKeyColumn : str = None,
         itemKeyColumn : str = None
     ):
+        """
+        Sets Estimator parameters
+        """
         return self._set(**self._input_kwargs)
 
 
 class ItemSelectionTransformer(Transformer,
                                HasUserKeyColumn,
                                HasItemKeyColumn,
                                DefaultParamsReadable,
                                DefaultParamsWritable):
+    """
+    Base class for item selection transformer. transform()
+    will be used to create user-item pairs
+    """
     @keyword_only
     def __init__(
         self,
         userKeyColumn : str = None,
         itemKeyColumn : str = None
     ):
-        """
-        Base class for item selection transformer. transform()
-        will be used to create user-item pairs
-        """
         super().__init__()
         self.setParams(**self._input_kwargs)
 
     @keyword_only
     def setParams(
         self,
         userKeyColumn : str = None,
         itemKeyColumn : str = None
     ):
+        """
+        Sets Transformer parameters
+        """
         self._set(**self._input_kwargs)
 
 
 class CrossJoinItemEstimator(ItemSelectionEstimator, HasSeed):
+    """
+    Assigns k items for every user from random items subsample
+    """
     def __init__(
         self,
         k : int,
         userKeyColumn : str = None,
         itemKeyColumn : str = None,
         seed : int = None
     ):
         """
-        Assigns k items for every user from random items subsample
-
         :param k: Number of items for every user
         :param userKeyColumn: Users identifier column, defaults to None
         :param itemKeyColumn: Items identifier column, defaults to None
         :param seed: Random state seed, defaults to None
         """
 
         super().__init__(userKeyColumn=userKeyColumn,
@@ -82,76 +89,76 @@
 
         self.setSeed(seed)
 
         self._k = k
 
     def _fit(
         self,
-        df : DataFrame
+        dataset : DataFrame
     ):
         """
         Fits estimator with items dataframe
 
         :param df: Items dataframe
         :returns: CrossJoinItemTransformer instance
         """
 
         userKeyColumn = self.getUserKeyColumn()
         itemKeyColumn = self.getItemKeyColumn()
         seed = self.getSeed()
-        
-        if itemKeyColumn not in df.columns:
+
+        if itemKeyColumn not in dataset.columns:
             raise ValueError(f'Dataframe has no {itemKeyColumn} column')
 
         return CrossJoinItemTransformer(
-            item_df=df,
+            item_df=dataset,
             k=self._k,
             userKeyColumn=userKeyColumn,
             itemKeyColumn=itemKeyColumn,
             seed=seed
         )
 
 
 class CrossJoinItemTransformer(ItemSelectionTransformer, HasSeedSequence):
+    """
+    Assigns k items for every user from random items subsample
+    """
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         item_df : DataFrame,
         k : int,
         userKeyColumn : str = None,
         itemKeyColumn : str = None,
         seed : int = None
     ):
-        """
-        Assigns k items for every user from random items subsample
-        """
-
         super().__init__(userKeyColumn=userKeyColumn,
                          itemKeyColumn=itemKeyColumn)
 
         self.initSeedSequence(seed)
 
         self._item_df = item_df
         self._k = k
 
     def _transform(
         self,
-        df : DataFrame
+        dataset : DataFrame
     ):
         """
         Takes a users dataframe and assings defined number of items
 
         :param df: Users dataframe
         :returns: Users cross join on random items subsample
         """
 
         userKeyColumn = self.getUserKeyColumn()
         itemKeyColumn = self.getItemKeyColumn()
         seed = self.getNextSeed()
 
-        if userKeyColumn not in df.columns:
+        if userKeyColumn not in dataset.columns:
             raise ValueError(f'Dataframe has no {userKeyColumn} column')
 
         random_items = self._item_df.orderBy(sf.rand(seed=seed))\
                                     .limit(self._k)
 
-        return df.select(userKeyColumn)\
-                 .crossJoin(random_items.select(itemKeyColumn))
+        return dataset.select(userKeyColumn)\
+            .crossJoin(random_items.select(itemKeyColumn))
```

### Comparing `sim4rec-0.0.1/sim4rec/modules/simulator.py` & `sim4rec-0.0.2/sim4rec/modules/simulator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import pathlib
 from abc import ABC
-from typing import Tuple, Union
+from typing import Tuple, Union, Optional
 
 from pyspark.sql import SparkSession
 from pyspark.sql import DataFrame
 from pyspark.ml import Transformer, PipelineModel
 
 from replay.session_handler import State
-from sim4rec.modules import GeneratorBase
+from sim4rec.modules.generator import GeneratorBase
 
 
+# pylint: disable=too-many-instance-attributes
 class Simulator(ABC):
+    """
+    Simulator for recommendation systems, which uses the users
+    and items data passed to it, to simulate the users responses
+    to recommended items
+    """
 
     ITER_COLUMN = '__iter'
     DEFAULT_LOG_FILENAME = 'log.parquet'
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         user_gen : GeneratorBase,
         item_gen : GeneratorBase,
         data_dir : str,
         log_df : DataFrame = None,
         user_key_col : str = 'user_idx',
         item_key_col : str = 'item_idx',
         spark_session : SparkSession = None
     ):
         """
-        Simulator for recommendation systems, which uses the users
-        and items data passed to it, to simulate the users responses
-        to recommended items
-
         :param user_gen: Users data generator instance
         :param item_gen: Items data generator instance
         :param log_df: The history log with user-item pairs with other
             necessary fields. During the simulation the results will be
             appended to this log on update_log() call, defaults to None
         :param user_key_col: User identifier column name, defaults
             to 'user_idx'
@@ -58,37 +61,44 @@
 
         self._log_filename = self.DEFAULT_LOG_FILENAME
 
         self._log = None
         self._log_schema = None
         if log_df is not None:
             self.update_log(log_df, iteration='start')
-            
 
     @property
     def log(self):
+        """
+        Returns log
+        """
         return self._log
 
     @property
     def data_dir(self):
+        """
+        Returns directory with saved simulator data
+        """
         return self._data_dir
 
     @data_dir.setter
     def data_dir(self, value):
         self._data_dir = value
 
     @property
     def log_filename(self):
+        """
+        Returns name of log file
+        """
         return self._log_filename
 
     @log_filename.setter
     def log_filename(self, value):
         self._log_filename = value
 
-
     def clear_log(
         self
     ) -> None:
         """
         Clears the log
         """
 
@@ -138,37 +148,35 @@
 
         if self._log_schema is None:
             self._log_schema = log.schema.fields
         else:
             self._check_names_and_types(self._log_schema, log.schema)
 
         write_path = str(
-            pathlib.Path(self._data_dir)\
+            pathlib.Path(self._data_dir)
             .joinpath(f'{self.log_filename}/{self.ITER_COLUMN}={iteration}')
         )
         log.write.parquet(write_path)
 
         read_path = str(pathlib.Path(self._data_dir).joinpath(f'{self.log_filename}'))
         self._log = self._spark.read.parquet(read_path)
 
-
     def sample_users(
         self,
         frac_users : float
     ) -> DataFrame:
         """
         Samples a fraction of random users
 
         :param frac_users: Fractions of users to sample from user generator
         :returns: Sampled users dataframe
         """
 
         return self._user_gen.sample(frac_users)
 
-
     def sample_items(
         self,
         frac_items : float
     ) -> DataFrame:
         """
         Samples a fraction of random items
 
@@ -216,27 +224,32 @@
         pairs = selector.transform(user_df)
 
         return pairs, log
 
     def sample_responses(
         self,
         recs_df : DataFrame,
-        user_features : DataFrame,
-        item_features : DataFrame,
-        action_models : PipelineModel
+        action_models : PipelineModel,
+        user_features : Optional[DataFrame] = None,
+        item_features : Optional[DataFrame] = None
     ) -> DataFrame:
         """
         Simulates the actions users took on their recommended items
 
         :param recs_df: Dataframe with recommendations. Must contain
             user's and item's identifier columns. Other columns will
             be ignored
-        :param user_features: Users dataframe with features and identifiers
-        :param item_features: Items dataframe with features and identifiers
+        :param user_features: Users dataframe with features and identifiers,
+                              can be None
+        :param item_features: Items dataframe with features and identifiers,
+                              can be None
         :param action_models: Spark pipeline to evaluate responses
         :returns: DataFrame with user-item pairs and the respective actions
         """
 
-        user_item_df = recs_df.join(user_features, self._user_key_col, 'left')\
-                              .join(item_features, self._item_key_col, 'left')
+        if user_features is not None:
+            recs_df = recs_df.join(user_features, self._user_key_col, 'left')
+
+        if item_features is not None:
+            recs_df = recs_df.join(item_features, self._item_key_col, 'left')
 
-        return action_models.transform(user_item_df)
+        return action_models.transform(recs_df)
```

### Comparing `sim4rec-0.0.1/sim4rec/params/__init__.py` & `sim4rec-0.0.2/sim4rec/params/__init__.py`

 * *Files identical despite different names*

### Comparing `sim4rec-0.0.1/sim4rec/response/response.py` & `sim4rec-0.0.2/sim4rec/response/response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=no-member,unused-argument,too-many-ancestors,abstract-method
 import math
 from typing import List
 from collections.abc import Iterable
 
 import pyspark.sql.types as st
 import pyspark.sql.functions as sf
 from pyspark.ml import Transformer, Estimator
@@ -18,119 +19,130 @@
 )
 
 
 class ActionModelEstimator(Estimator,
                            HasOutputCol,
                            DefaultParamsReadable,
                            DefaultParamsWritable):
+    """
+    Base class for response estimator
+    """
     @keyword_only
     def __init__(
         self,
         outputCol : str = None
     ):
         """
-        Base class for response estimator
-
         :param outputCol: Name of the response score column, defaults
             to None
         """
 
         super().__init__()
         self.setParams(**self._input_kwargs)
 
     @keyword_only
     def setParams(
         self,
         outputCol : str = None
     ):
+        """
+        Sets parameters for response estimator
+        """
         return self._set(**self._input_kwargs)
 
 
 class ActionModelTransformer(Transformer,
                              HasOutputCol,
                              DefaultParamsReadable,
                              DefaultParamsWritable):
+    """
+    Base class for response transformer. transform() will be
+    used to calculate score based on inputCols, and write it
+    to outputCol column
+    """
     @keyword_only
     def __init__(
         self,
         outputCol : str = None
     ):
         """
-        Base class for response transformer. transform() will be
-        used to calculate score based on inputCols, and write it
-        to outputCol column
-
         :param outputCol: Name of the response score column, defaults
             to None
         """
 
         super().__init__()
         self.setParams(**self._input_kwargs)
 
     @keyword_only
     def setParams(
         self,
         outputCol : str = None
     ):
+        """
+        Sets parameters for response transformer
+        """
         return self._set(**self._input_kwargs)
 
 
 class BernoulliResponse(ActionModelTransformer,
                         HasInputCol,
                         HasSeedSequence):
+    """
+    Samples responses from probability column
+    """
     def __init__(
         self,
         inputCol : str = None,
         outputCol : str = None,
         seed : int = None
     ):
         """
-        Samples responses from probability column
-
         :param inputCol: Probability column name. Probability should
             be in range [0; 1]
         :param outputCol: Output column name
         :param seed: Random state seed, defaults to None
         """
 
         super().__init__(outputCol=outputCol)
 
         self._set(inputCol=inputCol)
         self.initSeedSequence(seed)
 
     def _transform(
         self,
-        df : DataFrame
+        dataset : DataFrame
     ):
         inputCol = self.getInputCol()
         outputCol = self.getOutputCol()
         seed = self.getNextSeed()
 
-        return df.withColumn(
+        return dataset.withColumn(
             outputCol,
             sf.when(sf.rand(seed=seed) <= sf.col(inputCol), 1).otherwise(0)
         )
 
 
 class NoiseResponse(ActionModelTransformer,
                     HasMean,
                     HasStandardDeviation,
                     HasClipNegative,
                     HasSeedSequence):
+    # pylint: disable=too-many-arguments
+    """
+    Creates random response sampled from normal distribution
+    """
     def __init__(
         self,
         mu : float = None,
         sigma : float = None,
         outputCol : str = None,
         clipNegative : bool = True,
         seed : int = None
     ):
         """
-        Creates random response sampled from normal distribution
-
         :param mu: Mean parameter of normal distribution
         :param sigma: Standard deviation parameter of normal distribution
         :param outputCol: Output column name
         :param clip_negative: Whether to make response non-negative,
             defaults to True
         :param seed: Random state seed, defaults to None
         """
@@ -138,82 +150,84 @@
         super().__init__(outputCol=outputCol)
 
         self._set(mean=mu, std=sigma, clipNegative=clipNegative)
         self.initSeedSequence(seed)
 
     def _transform(
         self,
-        df : DataFrame
+        dataset : DataFrame
     ):
         mu = self.getMean()
         sigma = self.getStandardDeviation()
         clip_negative = self.getClipNegative()
         outputCol = self.getOutputCol()
         seed = self.getNextSeed()
 
         expr = sf.randn(seed=seed) * sigma + mu
         if clip_negative:
             expr = sf.greatest(expr, sf.lit(0))
 
-        return df.withColumn(outputCol, expr)
+        return dataset.withColumn(outputCol, expr)
 
 
 class ConstantResponse(ActionModelTransformer,
                        HasConstantValue):
+    """
+    Always returns constant valued response
+    """
     def __init__(
         self,
         value : float = 0.0,
         outputCol : str = None
     ):
         """
-        Always returns constant valued response
-
         :param value: Response value
         :param outputCol: Output column name
         """
 
         super().__init__(outputCol=outputCol)
-        
+
         self._set(constantValue=value)
 
     def _transform(
         self,
-        df : DataFrame
+        dataset : DataFrame
     ):
         value = self.getConstantValue()
         outputColumn = self.getOutputCol()
 
-        return df.withColumn(outputColumn, sf.lit(value))
+        return dataset.withColumn(outputColumn, sf.lit(value))
 
 
 class CosineSimilatiry(ActionModelTransformer,
                        HasInputCols):
+    """
+    Calculates the cosine similarity between two vectors.
+    The result is in [0; 1] range
+    """
     def __init__(
         self,
         inputCols : List[str] = None,
         outputCol : str = None
     ):
         """
-        Calculates the cosine similarity between two vectors.
-        The result is in [0; 1] range
-
         :param inputCols: Two column names with dense vectors
         :param outputCol: Output column name
         """
 
         if inputCols is not None and len(inputCols) != 2:
-            raise ValueError('There must be two array columns '\
+            raise ValueError('There must be two array columns '
                              'to calculate cosine similarity')
 
         super().__init__(outputCol=outputCol)
         self._set(inputCols=inputCols)
 
     def _transform(
         self,
-        df : DataFrame
+        dataset : DataFrame
     ):
         inputCols = self.getInputCols()
         outputCol = self.getOutputCol()
 
         def cosine_similarity(first, second):
             num = first.dot(second)
             den = first.norm(2) * second.norm(2)
@@ -222,48 +236,49 @@
                 return float(0)
 
             cosine = max(min(num / den, 1.0), -1.0)
             return float(1 - math.acos(cosine) / math.pi)
 
         cos_udf = sf.udf(cosine_similarity, st.DoubleType())
 
-        return df.withColumn(
+        return dataset.withColumn(
             outputCol,
             cos_udf(sf.col(inputCols[0]), sf.col(inputCols[1]))
         )
 
 
 class ParametricResponseFunction(ActionModelTransformer,
                                  HasInputCols,
                                  HasWeights):
+    """
+    Calculates response based on the weighted sum of input responses
+    """
     def __init__(
         self,
         inputCols : List[str] = None,
         outputCol : str = None,
         weights : Iterable = None
     ):
         """
-        Calculates response based on the weighted sum of input responses
-
         :param inputCols: Input responses column names
         :param outputCol: Output column name
         :param weights: Input responses weights
         """
 
         super().__init__(outputCol=outputCol)
         self._set(inputCols=inputCols, weights=weights)
 
     def _transform(
         self,
-        df : DataFrame
+        dataset : DataFrame
     ):
         inputCols = self.getInputCols()
         outputCol = self.getOutputCol()
         weights = self.getWeights()
 
-        return df.withColumn(
+        return dataset.withColumn(
             outputCol,
             sum([
                 sf.col(c) * weights[i]
-                    for i, c in enumerate(inputCols)
-                ])
+                for i, c in enumerate(inputCols)
+            ])
         )
```

### Comparing `sim4rec-0.0.1/sim4rec/utils/convert.py` & `sim4rec-0.0.2/sim4rec/utils/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 from pyspark.sql import SparkSession, DataFrame
 
 from replay.session_handler import State
 
 
 def pandas_to_spark(
-    df : pd.DataFrame,
-    schema = None, 
+    df: pd.DataFrame,
+    schema=None,
     spark_session : SparkSession = None) -> DataFrame:
     """
     Converts pandas DataFrame to spark DataFrame
 
     :param df: DataFrame to convert
     :param schema: Schema of the dataframe, defaults to None
     :param spark_session: Spark session to use, defaults to None
```

### Comparing `sim4rec-0.0.1/sim4rec/utils/uce.py` & `sim4rec-0.0.2/sim4rec/utils/uce.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-## Utility class extensions
-
+# Utility class extensions
+# pylint: disable=no-member,unused-argument
 import pickle
 import pyspark.sql.functions as sf
 import pyspark.sql.types as st
 
 from pyspark.sql import DataFrame
 from pyspark.ml import Transformer
 from pyspark.ml.param.shared import HasInputCol, HasOutputCol
@@ -11,76 +11,92 @@
 
 
 from pyspark.ml.param.shared import Params, Param, TypeConverters
 from pyspark import keyword_only
 
 
 class NotFittedError(Exception):
+    # pylint: disable=missing-class-docstring
     pass
 
+
 class EmptyDataFrameError(Exception):
+    # pylint: disable=missing-class-docstring
     pass
 
 
+# pylint: disable=too-many-ancestors
 class VectorElementExtractor(Transformer,
                              HasInputCol, HasOutputCol,
                              DefaultParamsReadable, DefaultParamsWritable):
+    """
+    Extracts element at index from array column
+    """
 
     index = Param(
         Params._dummy(),
         "index",
         "Array index to extract",
         typeConverter=TypeConverters.toInt
     )
 
     def setIndex(self, value):
+        """
+        Sets index to a certain value
+        :param value: Value to set index of an element
+        """
         return self._set(index=value)
 
     def getIndex(self):
+        """
+        Returns index of element
+        """
         return self.getOrDefault(self.index)
 
     @keyword_only
     def __init__(
         self,
         inputCol : str = None,
         outputCol : str = None,
         index : int = None
     ):
         """
-        Extracts element at index from array column
         :param inputCol: Input column with array
         :param outputCol: Output column name
         :param index: Index of an element within array
         """
         super().__init__()
         self.setParams(**self._input_kwargs)
 
     @keyword_only
     def setParams(
         self,
         inputCol : str = None,
         outputCol : str = None,
         index : int = None
     ):
+        """
+        Sets parameters for extractor
+        """
         return self._set(**self._input_kwargs)
 
     def _transform(
         self,
-        df : DataFrame
+        dataset : DataFrame
     ):
         index = self.getIndex()
 
         el_udf = sf.udf(
             lambda x : float(x[index]), st.DoubleType()
         )
 
         inputCol = self.getInputCol()
         outputCol = self.getOutputCol()
 
-        return df.withColumn(outputCol, el_udf(inputCol))
+        return dataset.withColumn(outputCol, el_udf(inputCol))
 
 
 def save(obj : object, filename : str):
     """
     Saves an object to pickle dump
     :param obj: Instance
     :param filename: File name of a dump
@@ -96,8 +112,8 @@
     :param filename: File name of a dump
     :return: Read instance
     """
 
     with open(filename, 'rb') as f:
         obj = pickle.load(f)
 
-    return obj
+    return obj
```

### Comparing `sim4rec-0.0.1/PKG-INFO` & `sim4rec-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: sim4rec
-Version: 0.0.1
-Summary: Simulator for recommendation algorithms
-Author: Your Name
-Author-email: you@example.com
-Requires-Python: >=3.8,<3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: numpy (>=1.20.0)
-Requires-Dist: pandas
-Requires-Dist: pyspark (>=3.0)
-Requires-Dist: replay-rec (>=0.10.0,<0.11.0)
-Requires-Dist: scipy
-Requires-Dist: sdv (==0.15.0)
-Requires-Dist: torch
-Description-Content-Type: text/markdown
-
 # Simulator
 
 Simulator is framework for training and evaluating recommendation algorithms on real or synthetic data. Framework is based on pyspark library to work with big data.
 As a part of simulation process the framework incorporates data generators, response functions and other tools, that can provide flexible usage of simulator.
 
 # Table of contents
 
@@ -33,14 +14,19 @@
 
 ## Installation
 
 ```bash
 pip install sim4rec
 ```
 
+If the installation takes too long, try
+```bash
+pip install sim4rec --use-deprecated=legacy-resolver
+```
+
 To install dependencies with poetry run
 
 ```bash
 pip install --upgrade pip wheel poetry lightfm==1.17
 poetry install
 ```
 
@@ -163,7 +149,19 @@
 
 For tests the pytest python library is used and to run tests for all modules you can run the following command from repository root directory
 
 ```bash
 pytest
 ```
 
+## Licence
+Sim4Rec is distributed under the [Apache License Version 2.0](https://github.com/sb-ai-lab/Sim4Rec/blob/main/LICENSE), 
+nevertheless the SDV package, imported by the Sim4Rec for synthetic data generation,
+is distributed under [Business Source License (BSL) 1.1](https://github.com/sdv-dev/SDV/blob/master/LICENSE).
+
+Synthetic tabular data generation not a purpose of the Sit4Rec framework. 
+The Sim4Rec offers an API and wrappers to run simulation with synthetic data, but the method of synthetic data generation is determined by the user. 
+SDV package is imported for illustration purposes and may be replaced by another synthetic data generation solution.  
+
+Thus, synthetic data generation functional and quality evaluation with SDV library, 
+namely the `SDVDataGenerator` from [generator.py](sim4rec/modules/generator.py) and `evaluate_synthetic` from [evaluation.py](sim4rec/modules/evaluation.py) 
+should be used for non-production purposes only according to the SDV License.
```

