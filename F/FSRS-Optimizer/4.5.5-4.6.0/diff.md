# Comparing `tmp/FSRS-Optimizer-4.5.5.tar.gz` & `tmp/FSRS-Optimizer-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FSRS-Optimizer-4.5.5.tar", last modified: Sun Jul 30 07:29:37 2023, max compression
+gzip compressed data, was "FSRS-Optimizer-4.6.0.tar", last modified: Tue Aug  1 10:16:12 2023, max compression
```

## Comparing `FSRS-Optimizer-4.5.5.tar` & `FSRS-Optimizer-4.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:29:37.190986 FSRS-Optimizer-4.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 07:29:37.190986 FSRS-Optimizer-4.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 07:29:37.194986 FSRS-Optimizer-4.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:29:37.190986 FSRS-Optimizer-4.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:29:37.190986 FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-30 07:29:37.000000 FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-30 07:29:37.000000 FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 07:29:37.000000 FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-30 07:29:37.000000 FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 07:29:37.000000 FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:29:37.190986 FSRS-Optimizer-4.5.5/src/fsrs_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/src/fsrs_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/src/fsrs_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52743 2023-07-30 07:29:23.000000 FSRS-Optimizer-4.5.5/src/fsrs_optimizer/fsrs_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:16:12.364887 FSRS-Optimizer-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-01 10:16:12.364887 FSRS-Optimizer-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:16:12.364887 FSRS-Optimizer-4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:16:12.360887 FSRS-Optimizer-4.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:16:12.364887 FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-01 10:16:12.000000 FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-01 10:16:12.000000 FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:16:12.000000 FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-01 10:16:12.000000 FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 10:16:12.000000 FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:16:12.364887 FSRS-Optimizer-4.6.0/src/fsrs_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/src/fsrs_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/src/fsrs_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52871 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/src/fsrs_optimizer/fsrs_optimizer.py
```

### Comparing `FSRS-Optimizer-4.5.5/LICENSE` & `FSRS-Optimizer-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.5.5/PKG-INFO` & `FSRS-Optimizer-4.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.5.5
+Version: 4.6.0
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
 
 The FSRS Optimizer is a Python library capable of utilizing personal spaced repetition review logs to refine the FSRS algorithm. Designed with the intent of delivering a standardized, universal optimizer to various FSRS implementations across numerous programming languages, this tool is set to establish a ubiquitous standard for spaced repetition review logs. By facilitating the uniformity of learning data among different spaced repetition softwares, it guarantees learners consistent review schedules across a multitude of platforms.
```

### Comparing `FSRS-Optimizer-4.5.5/README.md` & `FSRS-Optimizer-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.5.5/src/FSRS_Optimizer.egg-info/PKG-INFO` & `FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.5.5
+Version: 4.6.0
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
 
 The FSRS Optimizer is a Python library capable of utilizing personal spaced repetition review logs to refine the FSRS algorithm. Designed with the intent of delivering a standardized, universal optimizer to various FSRS implementations across numerous programming languages, this tool is set to establish a ubiquitous standard for spaced repetition review logs. By facilitating the uniformity of learning data among different spaced repetition softwares, it guarantees learners consistent review schedules across a multitude of platforms.
```

### Comparing `FSRS-Optimizer-4.5.5/src/fsrs_optimizer/__main__.py` & `FSRS-Optimizer-4.6.0/src/fsrs_optimizer/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,19 +114,33 @@
     if args.out:
         with open(args.out, "a+") as f:
             f.write(profile)
 
     loss_before, loss_after = optimizer.evaluate()
     print(f"Loss before training: {loss_before:.4f}")
     print(f"Loss after training: {loss_after:.4f}")
+    metrics, figures = optimizer.calibration_graph()
+    metrics['Log loss'] = loss_after
     if save_graphs:
-        for i, f in enumerate(optimizer.calibration_graph()):
+        for i, f in enumerate(figures):
             f.savefig(f"calibration_{i}.png")
-        for i, f in enumerate(optimizer.compare_with_sm2()):
+    figures = optimizer.compare_with_sm2()
+    if save_graphs:
+        for i, f in enumerate(figures):
             f.savefig(f"compare_with_sm2_{i}.png")
+    
+    evaluation = {
+        "filename": filename,
+        "size": optimizer.dataset.shape[0],
+        "parameters": optimizer.w,
+        "metrics": metrics
+    }
+
+    with open("evaluation.json", "w+") as f:
+        json.dump(evaluation, f)
 
 if __name__ == "__main__":
 
     config_save = os.path.expanduser(".fsrs_optimizer")
 
     parser = argparse.ArgumentParser()
     parser.add_argument("filenames", nargs='+')
@@ -137,15 +151,15 @@
     parser.add_argument("-o","--out",
                         help="File to APPEND the automatically generated profile to."
                         )
     args = parser.parse_args()
     curdir = os.getcwd()
     for filename in args.filenames:
         if os.path.isdir(filename):
-            files = [f for f in os.listdir(filename) if f.lower().endswith('.apkg')]
+            files = [f for f in os.listdir(filename) if f.lower().endswith('.apkg') or f.lower().endswith('.colpkg')]
             files = [os.path.join(filename, f) for f in files]
             for file_path in files:
                 try:
                     print(f"Processing {file_path}")
                     process(file_path)
                 except Exception as e:
                     print(e)
```

### Comparing `FSRS-Optimizer-4.5.5/src/fsrs_optimizer/fsrs_optimizer.py` & `FSRS-Optimizer-4.6.0/src/fsrs_optimizer/fsrs_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -833,15 +833,15 @@
         tmp.rename(columns={"p": "retrievability"}, inplace=True)
         tmp[['review_time', 'card_id', 'review_date', 'r_history', 't_history', 'delta_t', 'review_rating', 'stability', 'difficulty', 'retrievability', 'log_loss']].to_csv("./evaluation.tsv", sep='\t', index=False)
         del tmp
         return loss_before, loss_after
 
     def calibration_graph(self):
         fig1 = plt.figure()
-        plot_brier(self.dataset['p'], self.dataset['y'], bins=40, ax=fig1.add_subplot(111))
+        metrics = plot_brier(self.dataset['p'], self.dataset['y'], bins=40, ax=fig1.add_subplot(111))
         fig2 = plt.figure(figsize=(16, 12))
         for last_rating in ("1","2","3","4"):
             calibration_data = self.dataset[self.dataset['r_history'].str.endswith(last_rating)]
             if calibration_data.empty:
                 continue
             tqdm.write(f"\nLast rating: {last_rating}")
             plot_brier(calibration_data['p'], calibration_data['y'], bins=40, ax=fig2.add_subplot(2, 2, int(last_rating)), title=f"Last rating: {last_rating}")
@@ -906,15 +906,15 @@
 
         labs = [l.get_label() for l in lns]
         ax2.legend(lns, labs, loc='lower right')
         ax2.grid(linestyle='--')
         ax2.yaxis.set_major_formatter(ticker.FuncFormatter(to_percent))
         ax2.xaxis.set_major_formatter(ticker.FormatStrFormatter('%d'))
 
-        return fig1, fig2, fig3, fig4
+        return metrics, (fig1, fig2, fig3, fig4)
 
     def bw_matrix(self):
         B_W_Metric_raw = self.dataset[['difficulty', 'stability', 'p', 'y']].copy()
         B_W_Metric_raw['s_bin'] = B_W_Metric_raw['stability'].map(lambda x: round(math.pow(1.4, math.floor(math.log(x, 1.4))), 2))
         B_W_Metric_raw['d_bin'] = B_W_Metric_raw['difficulty'].map(lambda x: int(round(x)))
         B_W_Metric = B_W_Metric_raw.groupby(by=['s_bin', 'd_bin']).agg('mean').reset_index()
         B_W_Metric_count = B_W_Metric_raw.groupby(by=['s_bin', 'd_bin']).agg('count').reset_index()
@@ -1021,14 +1021,20 @@
     ax.set_ylabel('Actual R')
     ax2 = ax.twinx()
     ax2.set_ylabel('Number of reviews')
     ax2.bar(bins, counts, width=(0.8 / bin_count), ec='k', lw=.2, alpha=0.5, label='Number of reviews')
     ax2.legend(loc='lower center')
     if title:
         ax.set_title(title)
+    metrics = {
+        "R-squared": r2,
+        "RMSE": rmse,
+        "MAE": mae
+    }
+    return metrics
 
 def sm2(history):
     ivl = 0
     ef = 2.5
     reps = 0
     for delta_t, rating in history:
         delta_t = delta_t.item()
```

