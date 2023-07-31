# Comparing `tmp/bigstream-1.1.3.tar.gz` & `tmp/bigstream-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigstream-1.1.3.tar", last modified: Mon Jul 24 18:46:25 2023, max compression
+gzip compressed data, was "bigstream-1.1.4.tar", last modified: Mon Jul 31 22:00:35 2023, max compression
```

## Comparing `bigstream-1.1.3.tar` & `bigstream-1.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-24 18:46:15.361060 bigstream-1.1.3/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1083 2023-01-03 22:45:33.000000 bigstream-1.1.3/LICENSE.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-07-24 18:46:15.359979 bigstream-1.1.3/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8731 2023-07-11 16:34:08.000000 bigstream-1.1.3/README.md
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-24 18:46:15.336662 bigstream-1.1.3/bigstream/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/__init__.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    40044 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8325 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/application_pipelines.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7732 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/configure_irm.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     4460 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/features.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6090 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/level_set.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7210 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/metrics.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16816 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/motion_correct.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22137 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/piecewise_align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    17210 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/piecewise_transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16456 2023-07-21 16:14:18.000000 bigstream-1.1.3/bigstream/stitch.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    14133 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    21225 2023-07-11 20:23:49.000000 bigstream-1.1.3/bigstream/utility.py
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-24 18:46:15.355776 bigstream-1.1.3/bigstream.egg-info/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-07-24 18:46:15.000000 bigstream-1.1.3/bigstream.egg-info/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      517 2023-07-24 18:46:15.000000 bigstream-1.1.3/bigstream.egg-info/SOURCES.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2023-07-24 18:46:15.000000 bigstream-1.1.3/bigstream.egg-info/dependency_links.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      268 2023-07-24 18:46:15.000000 bigstream-1.1.3/bigstream.egg-info/requires.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2023-07-24 18:46:15.000000 bigstream-1.1.3/bigstream.egg-info/top_level.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2023-07-24 18:46:15.362742 bigstream-1.1.3/setup.cfg
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      829 2023-07-24 18:43:59.000000 bigstream-1.1.3/setup.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-31 22:00:23.847479 bigstream-1.1.4/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1083 2023-01-03 22:45:33.000000 bigstream-1.1.4/LICENSE.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-07-31 22:00:23.846423 bigstream-1.1.4/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8731 2023-07-11 16:34:08.000000 bigstream-1.1.4/README.md
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-31 22:00:23.824622 bigstream-1.1.4/bigstream/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.1.4/bigstream/__init__.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    40212 2023-07-31 21:53:31.000000 bigstream-1.1.4/bigstream/align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8325 2023-07-25 16:20:10.000000 bigstream-1.1.4/bigstream/application_pipelines.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7732 2023-07-31 21:53:33.000000 bigstream-1.1.4/bigstream/configure_irm.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     4460 2023-07-11 16:34:08.000000 bigstream-1.1.4/bigstream/features.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6090 2023-07-11 16:34:08.000000 bigstream-1.1.4/bigstream/level_set.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7210 2023-07-11 16:34:08.000000 bigstream-1.1.4/bigstream/metrics.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16816 2023-07-11 16:34:08.000000 bigstream-1.1.4/bigstream/motion_correct.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22197 2023-07-31 21:22:57.000000 bigstream-1.1.4/bigstream/piecewise_align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    17210 2023-07-11 16:34:08.000000 bigstream-1.1.4/bigstream/piecewise_transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16456 2023-07-21 16:14:18.000000 bigstream-1.1.4/bigstream/stitch.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    14160 2023-07-31 21:01:40.000000 bigstream-1.1.4/bigstream/transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    21904 2023-07-31 21:33:31.000000 bigstream-1.1.4/bigstream/utility.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-31 22:00:23.842152 bigstream-1.1.4/bigstream.egg-info/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-07-31 22:00:23.000000 bigstream-1.1.4/bigstream.egg-info/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      517 2023-07-31 22:00:23.000000 bigstream-1.1.4/bigstream.egg-info/SOURCES.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2023-07-31 22:00:23.000000 bigstream-1.1.4/bigstream.egg-info/dependency_links.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      268 2023-07-31 22:00:23.000000 bigstream-1.1.4/bigstream.egg-info/requires.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2023-07-31 22:00:23.000000 bigstream-1.1.4/bigstream.egg-info/top_level.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2023-07-31 22:00:23.848997 bigstream-1.1.4/setup.cfg
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      829 2023-07-31 21:58:05.000000 bigstream-1.1.4/setup.py
```

### Comparing `bigstream-1.1.3/LICENSE.txt` & `bigstream-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.3/README.md` & `bigstream-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.3/bigstream/align.py` & `bigstream-1.1.4/bigstream/align.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,20 +676,19 @@
     if initial_transform_given and np.all(default == np.eye(fix.ndim + 1)):
         default = initial_condition
 
     # specify static transform data explicitly
     static_transform_spacing = []
     for transform in static_transform_list:
         spacing = fix_spacing
-        if transform.shape != (4, 4) and len(transform.shape) != 1:
+        if transform.shape not in [(3, 3), (4, 4)] and len(transform.shape) != 1:
             spacing = ut.relative_spacing(transform, fix, fix_spacing)
         static_transform_spacing.append(spacing)
-    static_transform_origin = [fix_origin,]*len(static_transform_list)
     static_transform_spacing = tuple(static_transform_spacing)
-    static_transform_origin = tuple(static_transform_origin)
+    static_transform_origin = (fix_origin,)*len(static_transform_list)
 
     # skip sample and convert inputs to sitk images
     X = resolve_sampling(
         fix, mov,
         fix_mask, mov_mask,
         fix_spacing, mov_spacing,
         alignment_spacing,
@@ -708,26 +707,31 @@
     if static_transform_list:
         T = ut.transform_list_to_composite_transform(
             static_transform_list,
             static_transform_spacing,
             static_transform_origin,
         )
         irm.SetMovingInitialTransform(T)
+
+    # distinguish between 2D and 3D for rigid transforms
+    ndims = fix.GetDimension()
+    rigid_transform_constructor = sitk.Euler2DTransform if ndims == 2 else sitk.Euler3DTransform
+
     # set transform to optimize
     if isinstance(initial_condition, str) and initial_condition == "CENTER":
         a, b = fix, mov
         if fix_mask is not None and mov_mask is not None:
             a, b = fix_mask, mov_mask
-        x = sitk.CenteredTransformInitializer(a, b, sitk.Euler3DTransform())
-        x = sitk.Euler3DTransform(x).GetTranslation()[::-1]
-        initial_condition = np.eye(4)
-        initial_condition[:3, -1] = x
+        x = sitk.CenteredTransformInitializer(a, b, rigid_transform_constructor())
+        x = rigid_transform_constructor(x).GetTranslation()[::-1]
+        initial_condition = np.eye(ndims+1)
+        initial_condition[:ndims, -1] = x
         initial_transform_given = True
     if rigid and not initial_transform_given:
-        transform = sitk.Euler3DTransform()
+        transform = rigid_transform_constructor()
     elif rigid and initial_transform_given:
         transform = ut.matrix_to_euler_transform(initial_condition)
     elif not rigid and not initial_transform_given:
         transform = sitk.AffineTransform(fix.GetDimension())
     elif not rigid and initial_transform_given:
         transform = ut.matrix_to_affine_transform(initial_condition)
     irm.SetInitialTransform(transform, inPlace=True)
```

### Comparing `bigstream-1.1.3/bigstream/application_pipelines.py` & `bigstream-1.1.4/bigstream/application_pipelines.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.3/bigstream/configure_irm.py` & `bigstream-1.1.4/bigstream/configure_irm.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.3/bigstream/features.py` & `bigstream-1.1.4/bigstream/features.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.3/bigstream/level_set.py` & `bigstream-1.1.4/bigstream/level_set.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.3/bigstream/metrics.py` & `bigstream-1.1.4/bigstream/metrics.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.3/bigstream/motion_correct.py` & `bigstream-1.1.4/bigstream/motion_correct.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.3/bigstream/piecewise_align.py` & `bigstream-1.1.4/bigstream/piecewise_align.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,13 +511,16 @@
             mov_mask=mov_mask_zarr,
             write_path=local_write_path,
             cluster=cluster,
             **kwargs,
         )
         # TODO: THIS DOES NOT WORK WITH LARGER THAN MEMORY TRANSFORMS
         if iii > 0:
-            deform = compose_transforms(static_transform_list.pop(), deform, fix_spacing)
+            deform = compose_transforms(
+                static_transform_list.pop(), deform,
+                fix_spacing, fix_spacing,
+            )
         static_transform_list.append(deform)
 
     # return in the requested format
     return static_transform_list.pop()
```

### Comparing `bigstream-1.1.3/bigstream/piecewise_transform.py` & `bigstream-1.1.4/bigstream/piecewise_transform.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.3/bigstream/stitch.py` & `bigstream-1.1.4/bigstream/stitch.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.3/bigstream/transform.py` & `bigstream-1.1.4/bigstream/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,19 +387,19 @@
     root = _displacement_field_composition_nth_square_root(
         field, spacing, order, sqrt_iterations,
     )
     inv = - np.copy(root)
 
     # iterate to invert
     for i in range(iterations):
-        inv -= compose_transforms(root, inv, spacing)
+        inv -= compose_transforms(root, inv, spacing, spacing)
 
     # square-compose inv order times
     for i in range(order):
-        inv = compose_transforms(inv, inv, spacing)
+        inv = compose_transforms(inv, inv, spacing, spacing)
 
     # return result
     return inv
 
 
 def _displacement_field_composition_nth_square_root(
     field,
@@ -432,14 +432,14 @@
     """
 
     # container to hold root
     root = 0.5 * field
 
     # iterate
     for i in range(iterations):
-        residual = (field - compose_transforms(root, root, spacing))
+        residual = (field - compose_transforms(root, root, spacing, spacing))
         root += 0.5 * residual
 
     # return result
     return root
```

### Comparing `bigstream-1.1.3/bigstream/utility.py` & `bigstream-1.1.4/bigstream/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,17 +92,18 @@
 
     Returns
     -------
     permuted_matrix : 4x4 array
         The same matrix but with the axis order inverted
     """
 
-    corrected = np.eye(4)
-    corrected[:3, :3] = matrix[:3, :3][::-1, ::-1]
-    corrected[:3, -1] = matrix[:3, -1][::-1]
+    ndims = matrix.shape[0] - 1
+    corrected = np.eye(ndims + 1)
+    corrected[:ndims, :ndims] = matrix[:ndims, :ndims][::-1, ::-1]
+    corrected[:ndims, -1] = matrix[:ndims, -1][::-1]
     return corrected
 
 
 def change_affine_matrix_origin(matrix, origin):
     """
     Affine matrix change of origin
 
@@ -137,17 +138,18 @@
 
     Returns
     -------
     matrix : 4x4 numpy array
         The same transform as a 4x4 matrix
     """
 
-    matrix = np.eye(4)
-    matrix[:3, :3] = np.array(transform.GetMatrix()).reshape((3,3))
-    matrix[:3, -1] = np.array(transform.GetTranslation())
+    ndims = transform.GetDimension()
+    matrix = np.eye(ndims+1)
+    matrix[:ndims, :ndims] = np.array(transform.GetMatrix()).reshape((ndims,ndims))
+    matrix[:ndims, -1] = np.array(transform.GetTranslation())
     return invert_matrix_axes(matrix)
 
 
 def matrix_to_affine_transform(matrix):
     """
     Convert 4x4 numpy array to sitk.AffineTransform object
 
@@ -158,18 +160,19 @@
 
     Returns
     -------
     affine_transform : sitk.AffineTransform
         The same affine but as a sitk.AffineTransform object
     """
 
+    ndims = matrix.shape[0] - 1
     matrix_sitk = invert_matrix_axes(matrix)
-    transform = sitk.AffineTransform(3)
-    transform.SetMatrix(matrix_sitk[:3, :3].flatten())
-    transform.SetTranslation(matrix_sitk[:3, -1].squeeze())
+    transform = sitk.AffineTransform(ndims)
+    transform.SetMatrix(matrix_sitk[:ndims, :ndims].flatten())
+    transform.SetTranslation(matrix_sitk[:ndims, -1].squeeze())
     return transform
 
 
 def matrix_to_euler_transform(matrix):
     """
     Convert 4x4 numpy array to sitk.Euler3DTransform (rigid transform)
 
@@ -180,18 +183,19 @@
 
     Returns
     -------
     rigid_transform : sitk.Euler3DTransform object
         The same rigid transform but as a sitk object
     """
 
+    ndims = matrix.shape[0] - 1
     matrix_sitk = invert_matrix_axes(matrix)
-    transform = sitk.Euler3DTransform()
-    transform.SetMatrix(matrix_sitk[:3, :3].flatten())
-    transform.SetTranslation(matrix_sitk[:3, -1].squeeze())
+    transform = sitk.Euler2DTransform if ndims == 2 else sitk.Euler3DTransform()
+    transform.SetMatrix(matrix_sitk[:ndims, :ndims].flatten())
+    transform.SetTranslation(matrix_sitk[:ndims, -1].squeeze())
     return transform
 
 
 def euler_transform_to_parameters(transform):
     """
     Convert a sitk.Euler3DTransform object to a list of rigid transform
     parameters
@@ -347,17 +351,19 @@
 
     Returns
     -------
     trasnform_object : sitk.BSplineTransform
         A sitk.BSplineTransform object
     """
 
-    t = sitk.BSplineTransform(3, 3)
-    t.SetFixedParameters(parameters[:18])
-    t.SetParameters(parameters[18:])
+    # number of fixed parameters depends on dimension, stored in parameters[0]
+    nfp = 10 if parameters[0] == 2 else 18
+    t = sitk.BSplineTransform(parameters[0], 3)
+    t.SetFixedParameters(parameters[1:nfp+1])
+    t.SetParameters(parameters[nfp+1:])
     return t
 
 
 def bspline_to_displacement_field(
     bspline, shape, spacing=None, origin=None, direction=None,
 ):
     """
@@ -449,17 +455,25 @@
 
     Returns
     -------
     composite_transform : sitk.CompositeTransform object
         All transforms in the given list compressed into a sitk.CompositTransform 
     """
 
-    transform = sitk.CompositeTransform(3)
+    # determine dimension
+    if len(transform_list[0].shape) == 2:
+        ndims = 2 if transform_list[0].shape == (3, 3) else 3
+    elif len(transform_list[0].shape) > 2:
+        ndims = transform_list[0].ndim - 1
+    else:
+        ndims = transform_list[0][0]
+
+    transform = sitk.CompositeTransform(ndims)
     for iii, t in enumerate(transform_list):
-        if t.shape == (4, 4):
+        if t.shape in [(3, 3), (4, 4)]:
             t = matrix_to_affine_transform(t)
         elif len(t.shape) == 1:
             t = bspline_parameters_to_transform(t)
         else:
             a = spacing[iii] if isinstance(spacing, tuple) else spacing
             b = origin[iii] if isinstance(origin, tuple) else origin
             t = field_to_displacement_field_transform(t, a, b)
```

### Comparing `bigstream-1.1.3/bigstream.egg-info/SOURCES.txt` & `bigstream-1.1.4/bigstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.3/setup.py` & `bigstream-1.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bigstream",
-    version="1.1.3",
+    version="1.1.4",
     author="Greg M. Fleishman",
     author_email="greg.nli10me@gmail.com",
     description="Tools for distributed alignment of massive images",
     url="https://github.com/GFleishman/bigstream",
     license="MIT",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

