# Comparing `tmp/cjm-torchvision-tfms-0.0.1.tar.gz` & `tmp/cjm-torchvision-tfms-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-torchvision-tfms-0.0.1.tar", last modified: Sun Jul 30 02:39:55 2023, max compression
+gzip compressed data, was "cjm-torchvision-tfms-0.0.2.tar", last modified: Tue Aug  1 00:03:29 2023, max compression
```

## Comparing `cjm-torchvision-tfms-0.0.1.tar` & `cjm-torchvision-tfms-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-30 02:39:55.170067 cjm-torchvision-tfms-0.0.1/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    11337 2023-04-27 10:12:58.000000 cjm-torchvision-tfms-0.0.1/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-torchvision-tfms-0.0.1/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     4597 2023-07-30 02:39:55.169828 cjm-torchvision-tfms-0.0.1/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3894 2023-07-30 02:29:12.000000 cjm-torchvision-tfms-0.0.1/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-30 02:39:55.166788 cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-30 02:35:36.000000 cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2748 2023-07-30 02:35:36.000000 cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     6667 2023-07-30 02:35:36.000000 cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms/core.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-30 02:39:55.169318 cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     4597 2023-07-30 02:39:55.000000 cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      454 2023-07-30 02:39:55.000000 cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-30 02:39:55.000000 cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       62 2023-07-30 02:39:55.000000 cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-30 02:16:00.000000 cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       77 2023-07-30 02:39:55.000000 cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       21 2023-07-30 02:39:55.000000 cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1036 2023-07-30 02:35:30.000000 cjm-torchvision-tfms-0.0.1/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-30 02:39:55.170132 cjm-torchvision-tfms-0.0.1/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-torchvision-tfms-0.0.1/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-08-01 00:03:29.674638 cjm-torchvision-tfms-0.0.2/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    11337 2023-04-27 10:12:58.000000 cjm-torchvision-tfms-0.0.2/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-torchvision-tfms-0.0.2/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     4597 2023-08-01 00:03:29.673931 cjm-torchvision-tfms-0.0.2/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3894 2023-08-01 00:03:09.000000 cjm-torchvision-tfms-0.0.2/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-08-01 00:03:29.666596 cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-08-01 00:03:04.000000 cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2748 2023-08-01 00:03:04.000000 cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     6580 2023-08-01 00:03:04.000000 cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms/core.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-08-01 00:03:29.672856 cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     4597 2023-08-01 00:03:29.000000 cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      454 2023-08-01 00:03:29.000000 cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-08-01 00:03:29.000000 cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       62 2023-08-01 00:03:29.000000 cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-30 02:16:00.000000 cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       77 2023-08-01 00:03:29.000000 cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       21 2023-08-01 00:03:29.000000 cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1036 2023-08-01 00:02:50.000000 cjm-torchvision-tfms-0.0.2/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-08-01 00:03:29.674803 cjm-torchvision-tfms-0.0.2/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-torchvision-tfms-0.0.2/setup.py
```

### Comparing `cjm-torchvision-tfms-0.0.1/LICENSE` & `cjm-torchvision-tfms-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-torchvision-tfms-0.0.1/PKG-INFO` & `cjm-torchvision-tfms-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-torchvision-tfms
-Version: 0.0.1
+Version: 0.0.2
 Summary: Some custom Torchvision tranforms.
 Home-page: https://github.com/cj-mills/cjm-torchvision-tfms
 Author: Christian Mills
 Author-email: millscj@protonmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-torchvision-tfms-0.0.1/README.md` & `cjm-torchvision-tfms-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms/_modidx.py` & `cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms/_modidx.py`

 * *Files identical despite different names*

### Comparing `cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms/core.py` & `cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,46 +32,32 @@
 
     Attributes:
     -----------
     max_sz : int
         The maximum size for any dimension (height or width) of the image.
     """
     
-    def __init__(self, max_sz=256):
+    def __init__(self, 
+                 max_sz:int=256 # The maximum size for any dimension (height or width) of the image.
+                ):
         """
         Initialize ResizeMax object with a specified max_sz. 
-
-        Parameters:
-        -----------
-        max_sz : int, optional
-            The maximum size for any dimension (height or width) of the image. 
-            Default is 256.
         """
         # Call to the parent class (Transform) constructor
         super().__init__()
 
         # Set the maximum size for any dimension of the image
         self.max_sz = max_sz
         
-    def _transform(self, inpt: Any, params: Dict[str, Any]):
+    def _transform(self, 
+                   inpt: Any, # The input image tensor to be resized.
+                   params: Dict[str, Any] # A dictionary of parameters. Not used in this method but is present for compatibility with the parent's method signature.
+                  ) -> torch.Tensor: # The resized image tensor.
         """
         Apply the ResizeMax transformation on an input image tensor.
-
-        Parameters:
-        -----------
-        inpt : torch.Tensor
-            The input image tensor to be resized.
-        params : dict
-            A dictionary of parameters. Not used in this method but is present for 
-            compatibility with the parent's method signature.
-
-        Returns:
-        --------
-        torch.Tensor
-            The resized image tensor.
         """
 
         # Copy the input tensor to a new variable
         x = inpt
 
         # Get the width and height of the image tensor
         spatial_size = TF.get_spatial_size(x)
@@ -82,67 +68,58 @@
 
         # Resize the image tensor with antialiasing for smoother output
         x = TF.resize(x, size=size, antialias=True)
 
         # Return the transformed (resized) image tensor
         return x
 
-# %% ../nbs/00_core.ipynb 13
+# %% ../nbs/00_core.ipynb 12
 class PadSquare(transforms.Transform):
     """
     PadSquare is a PyTorch Transform class used to pad images to make them square. 
     Depending on the configuration, padding can be applied equally on both sides, 
     or can be randomly split between the two sides.
     
     Attributes:
         padding_mode (str): The method to use for padding. Default is 'constant'.
         fill (tuple): The RGB values to use for padding if padding_mode is 'constant'. Default is (123, 117, 104).
         shift (bool): If True, padding is randomly split between the two sides. If False, padding is equally applied. Default is True.
         pad_split (float): The proportion of padding applied to one side of the image. Only used when shift is True.
     """
 
-    def __init__(self, padding_mode='constant', fill=(123, 117, 104), shift=True):
+    def __init__(self, 
+                 padding_mode:str='constant', # The method to use for padding. Default is 'constant'.
+                 fill:tuple=(123, 117, 104), # The RGB values to use for padding if padding_mode is 'constant'.
+                 shift:bool=True # If True, padding is randomly split between the two sides. If False, padding is equally applied.
+                ):
         """
         The constructor for PadSquare class.
-
-        Parameters:
-            padding_mode (str): The method to use for padding. Default is 'constant'.
-            fill (tuple): The RGB values to use for padding if padding_mode is 'constant'. Default is (123, 117, 104).
-            shift (bool): If True, padding is randomly split between the two sides. If False, padding is equally applied. Default is True.
         """
         super().__init__()
         self.padding_mode = padding_mode
         self.fill = fill
         self.shift = shift
         self.pad_split = None
 
-    def forward(self, *inputs: Any) -> Any:
+    def forward(self, 
+                *inputs: Any # The inputs to the forward method.
+               ) -> Any: # The result of the superclass forward method.
         """
         The forward method that sets up the padding split factor if 'shift' is True, 
         and then calls the superclass forward method.
-        
-        Parameters:
-            *inputs (Any): The inputs to the forward method.
-
-        Returns:
-            Any: The result of the superclass forward method.
         """
         self.pad_split = random.random() if self.shift else None
         return super().forward(*inputs)
 
-    def _transform(self, inpt: Any, params: Dict[str, Any]):
+    def _transform(self, 
+                   inpt: Any, # The input to be transformed.
+                   params: Dict[str, Any] # A dictionary of parameters for the transformation.
+                  ) -> Any: # The transformed input.
         """
         The _transform method that applies padding to the input to make it square.
-        
-        Parameters:
-            inpt (Any): The input to be transformed.
-            params (Dict[str, Any]): A dictionary of parameters for the transformation.
-
-        Returns:
-            Any: The transformed input.
         """
         x = inpt
         
         # Get the width and height of the image tensor
         h, w = TF.get_spatial_size(x)
         
         # If shift is true, padding is randomly split between two sides
@@ -160,21 +137,27 @@
             padding = [0, offset] if h < w else [offset, 0]
         
         # Apply the padding to the image
         x = TF.pad(x, padding=padding, padding_mode=self.padding_mode, fill=self.fill)
         
         return x
 
-# %% ../nbs/00_core.ipynb 16
+# %% ../nbs/00_core.ipynb 15
 class CustomTrivialAugmentWide(torchvision.transforms.TrivialAugmentWide):
+    """
+    This class extends the TrivialAugmentWide class provided by PyTorch's transforms module.
+    TrivialAugmentWide is an augmentation policy randomly applies a single augmentation to each image.
+    """
     def __init__(
         self,
         num_magnitude_bins: int = 31,
         interpolation: transforms.InterpolationMode = transforms.InterpolationMode.NEAREST,
         fill: Optional[List[float]] = None,
         op_meta: Optional[Dict[str, Tuple[torch.Tensor, bool]]] = None
     ) -> None:
         super().__init__(num_magnitude_bins, interpolation, fill)
         self.op_meta = op_meta if op_meta else super()._augmentation_space(num_bins)
 
-    def _augmentation_space(self, num_bins: int) -> Dict[str, Tuple[torch.Tensor, bool]]:
+    def _augmentation_space(self, 
+                            num_bins: int
+                           ) -> Dict[str, Tuple[torch.Tensor, bool]]:
         return self.op_meta
```

### Comparing `cjm-torchvision-tfms-0.0.1/cjm_torchvision_tfms.egg-info/PKG-INFO` & `cjm-torchvision-tfms-0.0.2/cjm_torchvision_tfms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-torchvision-tfms
-Version: 0.0.1
+Version: 0.0.2
 Summary: Some custom Torchvision tranforms.
 Home-page: https://github.com/cj-mills/cjm-torchvision-tfms
 Author: Christian Mills
 Author-email: millscj@protonmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-torchvision-tfms-0.0.1/settings.ini` & `cjm-torchvision-tfms-0.0.2/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-torchvision-tfms
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_torchvision_tfms
```

### Comparing `cjm-torchvision-tfms-0.0.1/setup.py` & `cjm-torchvision-tfms-0.0.2/setup.py`

 * *Files identical despite different names*

