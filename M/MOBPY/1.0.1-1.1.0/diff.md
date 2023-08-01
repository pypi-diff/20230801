# Comparing `tmp/MOBPY-1.0.1.tar.gz` & `tmp/MOBPY-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MOBPY-1.0.1.tar", last modified: Sun Jul  9 08:29:17 2023, max compression
+gzip compressed data, was "MOBPY-1.1.0.tar", last modified: Tue Aug  1 12:55:00 2023, max compression
```

## Comparing `MOBPY-1.0.1.tar` & `MOBPY-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.522137 MOBPY-1.0.1/
--rw-r--r--   0 chentahung   (501) staff       (20)     1073 2023-07-04 10:05:44.000000 MOBPY-1.0.1/LICENSE
--rw-r--r--   0 chentahung   (501) staff       (20)     7993 2023-07-09 08:29:17.521984 MOBPY-1.0.1/PKG-INFO
--rw-r--r--   0 chentahung   (501) staff       (20)     7368 2023-07-05 17:45:58.000000 MOBPY-1.0.1/README.md
--rw-r--r--   0 chentahung   (501) staff       (20)      695 2023-07-09 08:11:48.000000 MOBPY-1.0.1/pyproject.toml
--rw-r--r--   0 chentahung   (501) staff       (20)       38 2023-07-09 08:29:17.522197 MOBPY-1.0.1/setup.cfg
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.517715 MOBPY-1.0.1/src/
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.519416 MOBPY-1.0.1/src/MOBPY/
--rw-r--r--   0 chentahung   (501) staff       (20)    10854 2023-07-09 08:10:21.000000 MOBPY-1.0.1/src/MOBPY/MOB.py
--rw-------   0 chentahung   (501) staff       (20)        0 2022-10-18 10:30:40.000000 MOBPY-1.0.1/src/MOBPY/__ init __.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.520211 MOBPY-1.0.1/src/MOBPY/categorical/
--rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:26.000000 MOBPY-1.0.1/src/MOBPY/categorical/__init__.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.521465 MOBPY-1.0.1/src/MOBPY/numeric/
--rw-r--r--   0 chentahung   (501) staff       (20)     5192 2023-07-09 08:03:26.000000 MOBPY-1.0.1/src/MOBPY/numeric/Monotone.py
--rw-r--r--   0 chentahung   (501) staff       (20)     3185 2023-06-11 15:50:05.000000 MOBPY-1.0.1/src/MOBPY/numeric/MonotoneNode.py
--rw-r--r--   0 chentahung   (501) staff       (20)    14951 2023-07-04 10:09:42.000000 MOBPY-1.0.1/src/MOBPY/numeric/OptimalBinning.py
--rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:33.000000 MOBPY-1.0.1/src/MOBPY/numeric/__init__.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.521819 MOBPY-1.0.1/src/MOBPY/plot/
--rw-r--r--   0 chentahung   (501) staff       (20)     3710 2023-07-04 10:29:46.000000 MOBPY-1.0.1/src/MOBPY/plot/MOB_PLOT.py
--rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:39.000000 MOBPY-1.0.1/src/MOBPY/plot/__init__.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.520039 MOBPY-1.0.1/src/MOBPY.egg-info/
--rw-r--r--   0 chentahung   (501) staff       (20)     7993 2023-07-09 08:29:17.000000 MOBPY-1.0.1/src/MOBPY.egg-info/PKG-INFO
--rw-r--r--   0 chentahung   (501) staff       (20)      423 2023-07-09 08:29:17.000000 MOBPY-1.0.1/src/MOBPY.egg-info/SOURCES.txt
--rw-r--r--   0 chentahung   (501) staff       (20)        1 2023-07-09 08:29:17.000000 MOBPY-1.0.1/src/MOBPY.egg-info/dependency_links.txt
--rw-r--r--   0 chentahung   (501) staff       (20)        6 2023-07-09 08:29:17.000000 MOBPY-1.0.1/src/MOBPY.egg-info/top_level.txt
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.704392 MOBPY-1.1.0/
+-rw-r--r--   0 chentahung   (501) staff       (20)     1073 2023-07-04 10:05:44.000000 MOBPY-1.1.0/LICENSE
+-rw-r--r--   0 chentahung   (501) staff       (20)    12304 2023-08-01 12:55:00.704179 MOBPY-1.1.0/PKG-INFO
+-rw-r--r--   0 chentahung   (501) staff       (20)    11672 2023-07-30 14:03:25.000000 MOBPY-1.1.0/README.md
+-rw-r--r--   0 chentahung   (501) staff       (20)      702 2023-08-01 12:53:56.000000 MOBPY-1.1.0/pyproject.toml
+-rw-r--r--   0 chentahung   (501) staff       (20)       38 2023-08-01 12:55:00.704441 MOBPY-1.1.0/setup.cfg
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.700839 MOBPY-1.1.0/src/
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.702030 MOBPY-1.1.0/src/MOBPY/
+-rw-r--r--   0 chentahung   (501) staff       (20)    13237 2023-07-27 09:47:44.000000 MOBPY-1.1.0/src/MOBPY/MOB.py
+-rw-r--r--   0 chentahung   (501) staff       (20)    13410 2023-07-30 13:45:11.000000 MOBPY-1.1.0/src/MOBPY/PAVA.py
+-rw-------   0 chentahung   (501) staff       (20)        0 2022-10-18 10:30:40.000000 MOBPY-1.1.0/src/MOBPY/__ init __.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.702720 MOBPY-1.1.0/src/MOBPY/categorical/
+-rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:26.000000 MOBPY-1.1.0/src/MOBPY/categorical/__init__.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.703299 MOBPY-1.1.0/src/MOBPY/numeric/
+-rw-r--r--   0 chentahung   (501) staff       (20)     5028 2023-07-22 19:06:58.000000 MOBPY-1.1.0/src/MOBPY/numeric/Monotone.py
+-rw-r--r--   0 chentahung   (501) staff       (20)     3185 2023-06-11 15:50:05.000000 MOBPY-1.1.0/src/MOBPY/numeric/MonotoneNode.py
+-rw-r--r--   0 chentahung   (501) staff       (20)    15005 2023-07-22 19:08:22.000000 MOBPY-1.1.0/src/MOBPY/numeric/OptimalBinning.py
+-rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:33.000000 MOBPY-1.1.0/src/MOBPY/numeric/__init__.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.703719 MOBPY-1.1.0/src/MOBPY/pav/
+-rw-r--r--   0 chentahung   (501) staff       (20)     7837 2023-07-27 09:47:36.000000 MOBPY-1.1.0/src/MOBPY/pav/PAV.py
+-rw-r--r--   0 chentahung   (501) staff       (20)     3248 2023-07-24 15:46:45.000000 MOBPY-1.1.0/src/MOBPY/pav/PavMonoNode.py
+-rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-16 12:44:20.000000 MOBPY-1.1.0/src/MOBPY/pav/__init__.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.703994 MOBPY-1.1.0/src/MOBPY/plot/
+-rw-r--r--   0 chentahung   (501) staff       (20)     6524 2023-07-27 09:48:36.000000 MOBPY-1.1.0/src/MOBPY/plot/MOB_PLOT.py
+-rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:39.000000 MOBPY-1.1.0/src/MOBPY/plot/__init__.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.702579 MOBPY-1.1.0/src/MOBPY.egg-info/
+-rw-r--r--   0 chentahung   (501) staff       (20)    12304 2023-08-01 12:55:00.000000 MOBPY-1.1.0/src/MOBPY.egg-info/PKG-INFO
+-rw-r--r--   0 chentahung   (501) staff       (20)      517 2023-08-01 12:55:00.000000 MOBPY-1.1.0/src/MOBPY.egg-info/SOURCES.txt
+-rw-r--r--   0 chentahung   (501) staff       (20)        1 2023-08-01 12:55:00.000000 MOBPY-1.1.0/src/MOBPY.egg-info/dependency_links.txt
+-rw-r--r--   0 chentahung   (501) staff       (20)        6 2023-08-01 12:55:00.000000 MOBPY-1.1.0/src/MOBPY.egg-info/top_level.txt
```

### Comparing `MOBPY-1.0.1/LICENSE` & `MOBPY-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MOBPY-1.0.1/pyproject.toml` & `MOBPY-1.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "MOBPY"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
-  { name="Chen, Ta-Hung", email="denny20700@gmail.com" }
+  { name="Ta-Hung (Denny) Chen", email="denny20700@gmail.com" }
 ]
 description = "MOB is a statistical approach to transform continuous variables into optimal and monotonic categorical variables."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `MOBPY-1.0.1/src/MOBPY/MOB.py` & `MOBPY-1.1.0/src/MOBPY/MOB.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class MOB:
     def __init__(self, data, var, response, exclude_value = None) :
         self._data = data
         self._var = var
         self._response = response 
         self._exclude_value = exclude_value
         self._constraintsStatus = False
+        self._outputTable = None
         '''
         _isNaExist : check Missing Existance
         _isExcValueExist : check Exclude Value Existance
         
         [attributes]
         self.df_missing : missing data subset
         self.df_excvalue : exclude value data subset
@@ -148,27 +149,32 @@
     def maximize_bins(self) -> bool :
         return self._maximize_bins
     
     @property
     def finishBinningTable(self) -> pd.DataFrame :
         return self._finishBinningTable
     
+    @property
+    def outputTable(self) -> pd.DataFrame :
+        return self._outputTable
+    
     def setBinningConstraints(self, max_bins :int = 6, min_bins :int = 4, max_samples = 0.4, min_samples = 0.05, min_bads = 0.05, init_pvalue: float = 0.4, maximize_bins :bool = True) -> None:
         self._max_bins = max_bins
         self._min_bins = min_bins
         self._init_pvalue = init_pvalue
         self._max_samples = max_samples
         self._min_samples = min_samples
         self._min_bads = min_bads
         self._maximize_bins = maximize_bins
         self._constraintsStatus = True
            
     def __summarizeBins(self, FinalOptTable) -> pd.DataFrame:
         
-        FinalOptTable = FinalOptTable[['start', 'end', 'total', 'bads', 'mean']].rename(columns = {'total': 'nsamples', 'bad' : 'bads', 'mean' : 'bad_rate'})
+        FinalOptTable = FinalOptTable[['[intervalStart', 'total', 'bads', 'mean']].rename(columns = {'total': 'nsamples', 'bad' : 'bads', 'mean' : 'bad_rate'})
+        FinalOptTable.insert(1, column = 'intervalEnd)', value = FinalOptTable['[intervalStart'].shift(-1))
         FinalOptTable['dist_obs'] = FinalOptTable['nsamples'] / FinalOptTable['nsamples'].sum()
         FinalOptTable['dist_bads'] = FinalOptTable['bads'] / FinalOptTable['bads'].sum()
         FinalOptTable['goods'] = FinalOptTable['nsamples'] - FinalOptTable['bads']
         FinalOptTable['dist_goods'] = FinalOptTable['goods'] / FinalOptTable['goods'].sum()
         FinalOptTable['woe'] = np.log(FinalOptTable['dist_goods']/FinalOptTable['dist_bads'])
         
         # adjusted woe replacement when encounter zero bads or zero goods
@@ -176,66 +182,92 @@
             adj_goods = FinalOptTable.loc[(FinalOptTable['bads'] == 0) | (FinalOptTable['goods'] == 0), 'goods'] + 0.5
             adj_bads = FinalOptTable.loc[(FinalOptTable['bads'] == 0) | (FinalOptTable['goods'] == 0), 'bads'] + 0.5
             adj_dist_goods = adj_goods / FinalOptTable['goods'].sum()
             adj_dist_bads = adj_bads / FinalOptTable['bads'].sum()
             FinalOptTable.loc[(FinalOptTable['bads'] == 0) | (FinalOptTable['goods'] == 0), 'woe'] = np.log(adj_dist_goods/adj_dist_bads)
 
         FinalOptTable['iv_grp'] = (FinalOptTable['dist_goods'] - FinalOptTable['dist_bads']) * FinalOptTable['woe']
+        # continous distribution means the value range from -inf to inf :
+        FinalOptTable.iloc[0,0] = -np.inf #first bin interval starts
+        FinalOptTable.iloc[-1,1] = np.inf #last bin interval ends
+        FinalOptTable.index.name = self.var
         return FinalOptTable      
       
     def runMOB(self, mergeMethod, sign = 'auto') -> pd.DataFrame :
-        if self.constraintsStatus == False :
-            raise Exception('Please set the constraints first by using "setBinningConstraints" method.')
-        
-        # Monotone
-        MonotoneTuner = Monotone(data = self.df_sel, var = self.var, response = self.response)
-        MonoTable = MonotoneTuner.tuneMonotone(sign = sign)
-        self.MonoTable = MonoTable
-        # Binning
-        OptimalBinningMerger = OptimalBinning(resMonotoneTable = MonoTable, 
-                                              max_bins = self.max_bins, min_bins = self.min_bins, 
-                                              max_samples = self.max_samples, min_samples = self.min_samples, 
-                                              min_bads = self.min_bads, init_pvalue = self.init_pvalue,
-                                              maximize_bins = self.maximize_bins)
-        
-        finishBinningTable = OptimalBinningMerger.monoOptBinning(mergeMethod = mergeMethod)
-        finishBinningTable['start'] = finishBinningTable['start'].astype(str)
-        finishBinningTable['end'] = finishBinningTable['end'].astype(str)
-        self._finishBinningTable = finishBinningTable
-        # Summary
-        if self.isNaExist and self.isExcValueExist : #contains missing and exclude value
-            
-            missingDF = pd.DataFrame({
-                'start' : ['Missing'],
-                'end' : ['Missing'],
-                'total' : [len(self.df_missing)],
-                'bads' : [self.df_missing[self.response].sum()],
-                'mean' : [(self.df_missing[self.response].sum()) / (len(self.df_missing))]})
-                
-            excludeValueDF = self.df_excvalue.groupby(self.var)[self.response].agg(['count', 'sum']).reset_index().fillna(0).rename(columns={self.var: 'start','count':'total', 'sum':'bads'})
-            excludeValueDF['start'] = excludeValueDF['start'].astype(str)
-            excludeValueDF.insert(1, 'end', excludeValueDF['start'])
-            excludeValueDF['mean'] = excludeValueDF['bads'] / excludeValueDF['total']
-            
-            completeBinningTable = pd.concat([finishBinningTable, missingDF, excludeValueDF], axis = 0, ignore_index = True)
-        elif self.isNaExist & ~self.isExcValueExist : # contains missing but no special values
-            missingDF = pd.DataFrame({
-                'start' : ['Missing'],
-                'end' : ['Missing'],
-                'total' : [len(self.df_missing)],
-                'bads' : [self.df_missing[self.response].sum()],
-                'mean' : [(self.df_missing[self.response].sum()) / (len(self.df_missing))]})
-            
-            completeBinningTable = pd.concat([finishBinningTable, missingDF], axis = 0, ignore_index = True)
-        elif ~self.isNaExist & self.isExcValueExist : # contains special values but no missing data
-            excludeValueDF = self.df_excvalue.groupby(self.var)[self.response].agg(['count', 'sum']).reset_index().fillna(0).rename(columns={self.var: 'start','count':'total', 'sum':'bads'})
-            excludeValueDF['start'] = excludeValueDF['start'].astype(str)
-            excludeValueDF.insert(1, 'end', excludeValueDF['start'])
-            excludeValueDF['mean'] = excludeValueDF['bads'] / excludeValueDF['total']
-            
-            completeBinningTable = pd.concat([finishBinningTable, excludeValueDF], axis = 0, ignore_index = True)
-        else : # clean data with no missing and special values
-            completeBinningTable = finishBinningTable
+        if mergeMethod in ['Stats', 'Size'] :
+            if self.constraintsStatus == False :
+                raise Exception('Please set the constraints first by using "setBinningConstraints" method.')
             
-        outputTable = self.__summarizeBins(FinalOptTable = completeBinningTable)
-        
+            # Monotone
+            MonotoneTuner = Monotone(data = self.df_sel, var = self.var, response = self.response)
+            MonoTable = MonotoneTuner.tuneMonotone(sign = sign)
+            self.MonoTable = MonoTable
+            # Binning
+            OptimalBinningMerger = OptimalBinning(resMonotoneTable = MonoTable, 
+                                                max_bins = self.max_bins, min_bins = self.min_bins, 
+                                                max_samples = self.max_samples, min_samples = self.min_samples, 
+                                                min_bads = self.min_bads, init_pvalue = self.init_pvalue,
+                                                maximize_bins = self.maximize_bins)
+            
+            finishBinningTable = OptimalBinningMerger.monoOptBinning(mergeMethod = mergeMethod)
+            finishBinningTable['[intervalStart'] = finishBinningTable['[intervalStart'].astype(str)
+            finishBinningTable['intervalEnd)'] = finishBinningTable['intervalEnd)'].astype(str)
+            self._finishBinningTable = finishBinningTable.rename(columns = {'intervalEnd)':'intervalEnd]'})
+            # Summary
+            if self.isNaExist and self.isExcValueExist : #contains missing and exclude value
+                
+                missingDF = pd.DataFrame({
+                    '[intervalStart' : ['Missing'],
+                    'intervalEnd)' : ['Missing'],
+                    'total' : [len(self.df_missing)],
+                    'bads' : [self.df_missing[self.response].sum()],
+                    'mean' : [(self.df_missing[self.response].sum()) / (len(self.df_missing))]})
+                    
+                excludeValueDF = self.df_excvalue.groupby(self.var)[self.response].agg(['count', 'sum']).reset_index().fillna(0).rename(columns={self.var: '[intervalStart','count':'total', 'sum':'bads'})
+                excludeValueDF['[intervalStart'] = excludeValueDF['[intervalStart'].astype(str)
+                excludeValueDF.insert(1, 'intervalEnd)', excludeValueDF['[intervalStart'])
+                excludeValueDF['mean'] = excludeValueDF['bads'] / excludeValueDF['total']
+                
+                completeBinningTable = pd.concat([finishBinningTable, missingDF, excludeValueDF], axis = 0, ignore_index = True)
+            elif self.isNaExist & ~self.isExcValueExist : # contains missing but no special values
+                missingDF = pd.DataFrame({
+                    '[intervalStart' : ['Missing'],
+                    'intervalEnd)' : ['Missing'],
+                    'total' : [len(self.df_missing)],
+                    'bads' : [self.df_missing[self.response].sum()],
+                    'mean' : [(self.df_missing[self.response].sum()) / (len(self.df_missing))]})
+                
+                completeBinningTable = pd.concat([finishBinningTable, missingDF], axis = 0, ignore_index = True)
+            elif ~self.isNaExist & self.isExcValueExist : # contains special values but no missing data
+                excludeValueDF = self.df_excvalue.groupby(self.var)[self.response].agg(['count', 'sum']).reset_index().fillna(0).rename(columns={self.var: '[intervalStart','count':'total', 'sum':'bads'})
+                excludeValueDF['[intervalStart'] = excludeValueDF['[intervalStart'].astype(str)
+                excludeValueDF.insert(1, 'intervalEnd', excludeValueDF['[intervalStart'])
+                excludeValueDF['mean'] = excludeValueDF['bads'] / excludeValueDF['total']
+                
+                completeBinningTable = pd.concat([finishBinningTable, excludeValueDF], axis = 0, ignore_index = True)
+            else : # clean data with no missing and special values
+                completeBinningTable = finishBinningTable
+                
+            outputTable = self.__summarizeBins(FinalOptTable = completeBinningTable)
+            # intervalStart and intervalEnd is set as string due to the concatenation of missing and exclusive dataset
+            self._outputTable = outputTable
+        else :
+            raise ValueError('mergeMethod only supports {<Stats> | <Size>} so far.')
+                
         return outputTable
+
+    def applyMOB(self, var_column : pd.Series, assign :str = 'interval') :
+        '''
+        assignment: <str> {'interval'|'start'|'end'}
+        '''
+        _MOBout = self.outputTable
+        _MOBout['[intervalStart'] = _MOBout['[intervalStart'].astype(float)
+        _MOBout['intervalEnd)'] = _MOBout['intervalEnd)'].astype(float)
+        if assign == 'interval' :
+            # include intervalStart but exclude intervalEnd :
+            MOB_Res_Series = var_column.apply(lambda row : f'[ {_MOBout.loc[(_MOBout["[intervalStart"] <= row)&(_MOBout["intervalEnd)"] > row), "[intervalStart"].values[0]} , {_MOBout.loc[(_MOBout["[intervalStart"] <= row)&(_MOBout["intervalEnd)"] > row), "intervalEnd)"].values[0]} )')
+        elif assign == 'start' :
+            MOB_Res_Series = var_column.apply(lambda row : _MOBout.loc[(_MOBout["[intervalStart"] <= row)&(_MOBout["intervalEnd)"] > row), "[intervalStart"].values[0])
+        elif assign == 'end' :
+            MOB_Res_Series = var_column.apply(lambda row : _MOBout.loc[(_MOBout["[intervalStart"] <= row)&(_MOBout["intervalEnd)"] > row), "intervalEnd)"].values[0])
+        
+        return MOB_Res_Series
```

### Comparing `MOBPY-1.0.1/src/MOBPY/numeric/Monotone.py` & `MOBPY-1.1.0/src/MOBPY/numeric/Monotone.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 from typing import Union
 import os
 # os.chdir('/Users/chentahung/Desktop/git/mob-py/src/main/python')
 from MOBPY.numeric.MonotoneNode import MonotoneNode
 
 class Monotone :
-    def __init__(self, data, var, response, exclude_value = None, metric = 'mean') :
+    def __init__(self, data, var, response, metric = 'mean') :
         '''
         data : <pandas.DataFrame> 
         var : <string> column to generate WoE
         response : <string> column 
         '''
         
         if len(data[response].unique()) != 2:
@@ -19,15 +19,14 @@
         if data[response].dtypes == 'object' :
             raise ValueError(f'Please change the response variable into numeric with `1` represent positive and `0` represent the other')
         
         self._data = data
         self._var = var
         self._response = response
         self._metric = metric
-        self._exclude_value = exclude_value
             
 
     @property
     def data(self) -> pd.DataFrame:
         return self._data
     
     @property
@@ -38,18 +37,14 @@
     def response(self) -> str :
         return self._response
 
     @property
     def metric(self) -> str :
         return self._metric
     
-    @property
-    def exclude_value(self) -> Union[list, int, float, None]:
-        return self._exclude_value
-    
     def __selectSign(self) -> str:
         '''
         decide `sign` argument
         '''
         if self.data[[self.var, self.response]].corr().iloc[1,0] > 0 :
             sign = '+'
         else :
@@ -133,15 +128,15 @@
             endValueList.append(str(cur.endValue))
             binTotalList.append(cur.cumTotal)
             binBadList.append(cur.cumBad)
             stdList.append(cur.cumStd)
             meanList.append(cur.mean)
             cur = cur.next
         
-        resDF = pd.DataFrame({'start':startValueList, 'end': endValueList, 'total': binTotalList, 'bads': binBadList, 'mean': meanList, 'std': stdList})
+        resDF = pd.DataFrame({'[intervalStart':startValueList, 'intervalEnd)': endValueList, 'total': binTotalList, 'bads': binBadList, 'mean': meanList, 'std': stdList})
         return resDF
     
 # %%
 # if __name__ == '__main__' :
 #     df = pd.read_csv('/Users/chentahung/Desktop/git/mob-py/data/german_data_credit_cat.csv')
 #     df['default'] = df['default'] - 1
```

### Comparing `MOBPY-1.0.1/src/MOBPY/numeric/MonotoneNode.py` & `MOBPY-1.1.0/src/MOBPY/numeric/MonotoneNode.py`

 * *Files identical despite different names*

### Comparing `MOBPY-1.0.1/src/MOBPY/numeric/OptimalBinning.py` & `MOBPY-1.1.0/src/MOBPY/numeric/OptimalBinning.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,24 +130,24 @@
             bin2_obs  = optTable.loc[i + 1, 'total']
             
             p_value_list.append(self.__runTwoSampleTTest(mergeMethod, bin1_mean, bin2_mean, bin1_std, bin2_std, bin1_obs, bin2_obs))
 
         return p_value_list
 
     def __mergeBinsOnce(self, optTable, mergeResult, mergeIndex) :
-        newStart = optTable.loc[mergeIndex, 'start']
-        newEnd   = optTable.loc[mergeIndex + 1, 'end']
+        newStart = optTable.loc[mergeIndex, '[intervalStart']
+        newEnd   = optTable.loc[mergeIndex + 1, 'intervalEnd)']
         
         newTotal = mergeResult[mergeIndex, 1]
         newMean  = mergeResult[mergeIndex, 2]
         newBads  = newTotal * newMean
         newStd   = mergeResult[mergeIndex, 3]
         
-        mergeDataFrame = pd.DataFrame({'start' : [newStart],
-                                       'end'   : [newEnd],
+        mergeDataFrame = pd.DataFrame({'[intervalStart' : [newStart],
+                                       'intervalEnd)'   : [newEnd],
                                        'total' : [newTotal],
                                        'bads'  : [newBads],
                                        'mean'  : [newMean],
                                        'std'   : [newStd]})
         
         if mergeIndex == 0 :
             return pd.concat([mergeDataFrame, optTable.iloc[mergeIndex+2:]], axis = 0, ignore_index=True)
@@ -268,15 +268,15 @@
         df = self.MonoDf.copy()
         
         if mergeMethod in ['Stats', 'Size', 'Chi'] :
             completedTable = self.__OptBinning(monoTable = df, mergeMethod = mergeMethod)
         else :
             raise('Wrong Merging Method : <Stats> / <Size> / <Chi>')
 
-        return completedTable[['start', 'end', 'total', 'bads', 'mean']]
+        return completedTable[['[intervalStart', 'intervalEnd)', 'total', 'bads', 'mean']]
     
 #%%
 
 # if __name__ == '__main__' :
 #     df = pd.read_csv('/Users/chentahung/Desktop/git/mob-py/data/german_data_credit_cat.csv')
 #     df['default'] = df['default'] - 1
 #     import os
```

