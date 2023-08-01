# Comparing `tmp/teemi-0.2.0.tar.gz` & `tmp/teemi-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teemi-0.2.0.tar", last modified: Tue May 30 12:37:19 2023, max compression
+gzip compressed data, was "teemi-0.3.2.tar", last modified: Tue Aug  1 07:51:16 2023, max compression
```

## Comparing `teemi-0.2.0.tar` & `teemi-0.3.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.976055 teemi-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-30 12:36:14.000000 teemi-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-30 12:36:14.000000 teemi-0.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-30 12:36:14.000000 teemi-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 12:36:14.000000 teemi-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-05-30 12:37:19.976055 teemi-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-05-30 12:36:14.000000 teemi-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-30 12:37:19.976055 teemi-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-30 12:36:15.000000 teemi-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.976055 teemi-0.2.0/teemi/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 12:37:19.976055 teemi-0.2.0/teemi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.972056 teemi-0.2.0/teemi/build/
--rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/build/PCR.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30079 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/build/containers_wells_picklists.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/build/robot_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/build/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.972056 teemi-0.2.0/teemi/design/
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/CRISPRsequencecutter.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)    24971 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/combinatorial_design.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/fetch_sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/retrieve_gene_homologs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/sequence_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/teselagen_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.976055 teemi-0.2.0/teemi/learn/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/learn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/learn/auto_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    22443 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/learn/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.976055 teemi-0.2.0/teemi/lims/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/lims/benchling_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/lims/csv_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.976055 teemi-0.2.0/teemi/test/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/test/data_wrangling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/test/genotyping.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.972056 teemi-0.2.0/teemi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-30 12:36:15.000000 teemi-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:51:15.997731 teemi-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-01 07:49:56.000000 teemi-0.3.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 07:49:56.000000 teemi-0.3.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-01 07:49:56.000000 teemi-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 07:49:56.000000 teemi-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17682 2023-08-01 07:51:15.997731 teemi-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-08-01 07:49:56.000000 teemi-0.3.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-01 07:51:15.997731 teemi-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-01 07:49:57.000000 teemi-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:51:15.997731 teemi-0.3.2/teemi/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-01 07:51:15.997731 teemi-0.3.2/teemi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:51:15.993731 teemi-0.3.2/teemi/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/build/PCR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30079 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/build/containers_wells_picklists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/build/robot_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/build/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:51:15.993731 teemi-0.3.2/teemi/design/
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/design/CRISPRsequencecutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/design/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19188 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/design/combinatorial_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/design/fetch_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16202 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/design/gibson_cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/design/retrieve_gene_homologs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/design/sequence_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/design/teselagen_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:51:15.993731 teemi-0.3.2/teemi/learn/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/learn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/learn/auto_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22443 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/learn/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:51:15.993731 teemi-0.3.2/teemi/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/lims/benchling_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/lims/csv_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:51:15.993731 teemi-0.3.2/teemi/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/test/data_wrangling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/test/genotyping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-08-01 07:49:57.000000 teemi-0.3.2/teemi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:51:15.993731 teemi-0.3.2/teemi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17682 2023-08-01 07:51:15.000000 teemi-0.3.2/teemi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-01 07:51:15.000000 teemi-0.3.2/teemi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 07:51:15.000000 teemi-0.3.2/teemi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-01 07:51:15.000000 teemi-0.3.2/teemi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 07:51:15.000000 teemi-0.3.2/teemi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-01 07:51:15.000000 teemi-0.3.2/teemi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 07:51:15.000000 teemi-0.3.2/teemi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-08-01 07:49:57.000000 teemi-0.3.2/versioneer.py
```

### Comparing `teemi-0.2.0/LICENSE` & `teemi-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/setup.py` & `teemi-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/build/PCR.py` & `teemi-0.3.2/teemi/build/PCR.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,64 +552,62 @@
             "concentration"
         ] = concentrations[i]
         amplicon_by_name(amplicon_names[i], amplicons).annotations["batches"][0][
             "volume"
         ] = volumes[i]
 
 
-## Maybe redundant
-# def get_amplicons_by_row(row, amplicon_df, amplicons):
-#    """Returns a list of amplicons in a given gel row.
-#
-#    Parameters
-#    ----------
-#    row : str
-#        Name of the gel row.
-#    amplicon_df : pandas DataFrame
-#        DataFrame with amplicon information, including the column 'prow' indicating the gel row.
-#    amplicons : list of Amplicon
-#        List of Amplicon objects.
-#
-#    Returns
-#    -------
-#    list of Amplicon
-#        List of Amplicon objects in the given gel row.
-#    """
-#    row_names = amplicon_df[amplicon_df['prow']==row][['name']]['name'].tolist()
-#
-#    row_amplicons = []
-#    for name in row_names:
-#        for amplicon in amplicons:
-#            if amplicon.name == name:
-#                row_amplicons.append([amplicon])
-#
-#    return(row_amplicons)
-#
-#
-#
-# def get_amplicons_by_column(col, amplicon_df, amplicons):
-#    """
-#    Returns a list of amplicons in a given gel column.
-#
-#    Parameters
-#    ----------
-#    col : str
-#        Name of the gel column.
-#    amplicon_df : pandas DataFrame
-#        DataFrame with amplicon information, including the column 'pcol' indicating the gel column.
-#    amplicons : list of Amplicon
-#        List of Amplicon objects.
-#
-#    Returns
-#    -------
-#    list of Amplicon
-#        List of Amplicon objects in the given gel column.
-#    """
-#    col_names = amplicon_df[amplicon_df['pcol']==col][['name']]['name'].tolist()
-#
-#    col_amplicons = []
-#    for name in col_names:
-#        for amplicon in amplicons:
-#            if amplicon.name == name:
-#                col_amplicons.append([amplicon])
-#
-#    return(col_amplicons)
+def get_amplicons_by_row(row, amplicon_df, amplicons):
+   """Returns a list of amplicons in a given gel row.
+
+   Parameters
+   ----------
+   row : str
+       Name of the gel row.
+   amplicon_df : pandas DataFrame
+       DataFrame with amplicon information, including the column 'prow' indicating the gel row.
+   amplicons : list of Amplicon
+       List of Amplicon objects.
+
+   Returns
+   -------
+   list of Amplicon
+       List of Amplicon objects in the given gel row.
+   """
+   row_names = amplicon_df[amplicon_df['prow']==row][['name']]['name'].tolist()
+
+   row_amplicons = []
+   for name in row_names:
+       for amplicon in amplicons:
+           if amplicon.name == name:
+               row_amplicons.append([amplicon])
+
+   return(row_amplicons)
+
+
+def get_amplicons_by_column(col, amplicon_df, amplicons):
+   """
+   Returns a list of amplicons in a given gel column.
+
+   Parameters
+   ----------
+   col : str
+       Name of the gel column.
+   amplicon_df : pandas DataFrame
+       DataFrame with amplicon information, including the column 'pcol' indicating the gel column.
+   amplicons : list of Amplicon
+       List of Amplicon objects.
+
+   Returns
+   -------
+   list of Amplicon
+       List of Amplicon objects in the given gel column.
+   """
+   col_names = amplicon_df[amplicon_df['pcol']==col][['name']]['name'].tolist()
+
+   col_amplicons = []
+   for name in col_names:
+       for amplicon in amplicons:
+           if amplicon.name == name:
+               col_amplicons.append([amplicon])
+
+   return(col_amplicons)
```

### Comparing `teemi-0.2.0/teemi/build/containers_wells_picklists.py` & `teemi-0.3.2/teemi/build/containers_wells_picklists.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/build/robot_assembly.py` & `teemi-0.3.2/teemi/build/robot_assembly.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
     destination_plate = Plate96(name="5")
     picklist = PickList()
     counter = 0
 
     # FIRST WE CHECK WICH COMPONENTS WE NEED FOR THE PCRs
     for index, row in PCR_dataframe.iterrows():
-        templates = row["Template"]
+        templates = row["template"]
         f_primers = row["forward_primer"]
         r_primers = row["reverse_primer"]
 
         # FORWARD PRIMERS
         # we see if we can find the primer we need in the primer plate and if we find it we will add it to the picklist
         for index1, row1 in FORWARD_PRIMERS.iterrows():
             for k, v in row1["content"]["quantities"].items():
```

### Comparing `teemi-0.2.0/teemi/build/transformation.py` & `teemi-0.3.2/teemi/build/transformation.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/design/CRISPRsequencecutter.py` & `teemi-0.3.2/teemi/design/CRISPRsequencecutter.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/design/cloning.py` & `teemi-0.3.2/teemi/design/cloning.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/design/fetch_sequences.py` & `teemi-0.3.2/teemi/design/fetch_sequences.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,33 @@
     ncbi_hits = []
     for seq_record in SeqIO.parse(path, format="fasta"):
         ncbi_hits.append(seq_record)
 
     return ncbi_hits
 
 
+def read_genbank_files(path):
+    """Reads single Genbank files.
+    Parameters
+    ----------
+    path: str
+        path to the genbank file you want to read.
+
+    Returns
+    -------
+    list of Bio.SeqRecord.SeqRecord
+    """
+
+    ncbi_hits = []
+    for seq_record in SeqIO.parse(path, format="gb"):
+        ncbi_hits.append(seq_record)
+
+    return ncbi_hits
+
+
 def retrieve_sequences_from_PDB(query: list):
     """Retrieves sequences from PDB.
     Parameters
     ----------
     query: list
         list of accession numbers in the form of strings
 
@@ -164,24 +183,8 @@
 
         # Append to list
         LIST_OF_BIOrecord_objects.append(promoters_seq)
 
     return LIST_OF_BIOrecord_objects
 
 
-def read_genbank_files(path):
-    """Reads single Genbank files.
-    Parameters
-    ----------
-    path: str
-        path to the genbank file you want to read.
 
-    Returns
-    -------
-    list of Bio.SeqRecord.SeqRecord
-    """
-
-    ncbi_hits = []
-    for seq_record in SeqIO.parse(path, format="gb"):
-        ncbi_hits.append(seq_record)
-
-    return ncbi_hits
```

### Comparing `teemi-0.2.0/teemi/design/retrieve_gene_homologs.py` & `teemi-0.3.2/teemi/design/retrieve_gene_homologs.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/design/sequence_finder.py` & `teemi-0.3.2/teemi/design/sequence_finder.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/design/teselagen_helpers.py` & `teemi-0.3.2/teemi/design/teselagen_helpers.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/learn/auto_ml.py` & `teemi-0.3.2/teemi/learn/auto_ml.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/learn/plotting.py` & `teemi-0.3.2/teemi/learn/plotting.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/lims/benchling_api.py` & `teemi-0.3.2/teemi/lims/benchling_api.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/lims/csv_database.py` & `teemi-0.3.2/teemi/lims/csv_database.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/test/data_wrangling.py` & `teemi-0.3.2/teemi/test/data_wrangling.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/test/genotyping.py` & `teemi-0.3.2/teemi/test/genotyping.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi/utils.py` & `teemi-0.3.2/teemi/utils.py`

 * *Files identical despite different names*

### Comparing `teemi-0.2.0/teemi.egg-info/SOURCES.txt` & `teemi-0.3.2/teemi.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 teemi/build/robot_assembly.py
 teemi/build/transformation.py
 teemi/design/CRISPRsequencecutter.py
 teemi/design/__init__.py
 teemi/design/cloning.py
 teemi/design/combinatorial_design.py
 teemi/design/fetch_sequences.py
+teemi/design/gibson_cloning.py
 teemi/design/retrieve_gene_homologs.py
 teemi/design/sequence_finder.py
 teemi/design/teselagen_helpers.py
 teemi/learn/__init__.py
 teemi/learn/auto_ml.py
 teemi/learn/plotting.py
 teemi/lims/__init__.py
```

### Comparing `teemi-0.2.0/versioneer.py` & `teemi-0.3.2/versioneer.py`

 * *Files identical despite different names*

