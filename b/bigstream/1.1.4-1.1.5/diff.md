# Comparing `tmp/bigstream-1.1.4.tar.gz` & `tmp/bigstream-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigstream-1.1.4.tar", last modified: Mon Jul 31 22:00:35 2023, max compression
+gzip compressed data, was "bigstream-1.1.5.tar", last modified: Mon Jul 31 23:01:31 2023, max compression
```

## Comparing `bigstream-1.1.4.tar` & `bigstream-1.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-31 22:00:23.847479 bigstream-1.1.4/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1083 2023-01-03 22:45:33.000000 bigstream-1.1.4/LICENSE.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-07-31 22:00:23.846423 bigstream-1.1.4/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8731 2023-07-11 16:34:08.000000 bigstream-1.1.4/README.md
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-31 22:00:23.824622 bigstream-1.1.4/bigstream/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.1.4/bigstream/__init__.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    40212 2023-07-31 21:53:31.000000 bigstream-1.1.4/bigstream/align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8325 2023-07-25 16:20:10.000000 bigstream-1.1.4/bigstream/application_pipelines.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7732 2023-07-31 21:53:33.000000 bigstream-1.1.4/bigstream/configure_irm.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     4460 2023-07-11 16:34:08.000000 bigstream-1.1.4/bigstream/features.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6090 2023-07-11 16:34:08.000000 bigstream-1.1.4/bigstream/level_set.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7210 2023-07-11 16:34:08.000000 bigstream-1.1.4/bigstream/metrics.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16816 2023-07-11 16:34:08.000000 bigstream-1.1.4/bigstream/motion_correct.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22197 2023-07-31 21:22:57.000000 bigstream-1.1.4/bigstream/piecewise_align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    17210 2023-07-11 16:34:08.000000 bigstream-1.1.4/bigstream/piecewise_transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16456 2023-07-21 16:14:18.000000 bigstream-1.1.4/bigstream/stitch.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    14160 2023-07-31 21:01:40.000000 bigstream-1.1.4/bigstream/transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    21904 2023-07-31 21:33:31.000000 bigstream-1.1.4/bigstream/utility.py
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-31 22:00:23.842152 bigstream-1.1.4/bigstream.egg-info/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-07-31 22:00:23.000000 bigstream-1.1.4/bigstream.egg-info/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      517 2023-07-31 22:00:23.000000 bigstream-1.1.4/bigstream.egg-info/SOURCES.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2023-07-31 22:00:23.000000 bigstream-1.1.4/bigstream.egg-info/dependency_links.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      268 2023-07-31 22:00:23.000000 bigstream-1.1.4/bigstream.egg-info/requires.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2023-07-31 22:00:23.000000 bigstream-1.1.4/bigstream.egg-info/top_level.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2023-07-31 22:00:23.848997 bigstream-1.1.4/setup.cfg
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      829 2023-07-31 21:58:05.000000 bigstream-1.1.4/setup.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-31 23:01:20.607052 bigstream-1.1.5/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1083 2023-01-03 22:45:33.000000 bigstream-1.1.5/LICENSE.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-07-31 23:01:20.606032 bigstream-1.1.5/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8731 2023-07-11 16:34:08.000000 bigstream-1.1.5/README.md
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-31 23:01:20.583721 bigstream-1.1.5/bigstream/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.1.5/bigstream/__init__.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    40218 2023-07-31 22:58:52.000000 bigstream-1.1.5/bigstream/align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8325 2023-07-25 16:20:10.000000 bigstream-1.1.5/bigstream/application_pipelines.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7732 2023-07-31 21:53:33.000000 bigstream-1.1.5/bigstream/configure_irm.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     4460 2023-07-11 16:34:08.000000 bigstream-1.1.5/bigstream/features.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6090 2023-07-11 16:34:08.000000 bigstream-1.1.5/bigstream/level_set.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7210 2023-07-11 16:34:08.000000 bigstream-1.1.5/bigstream/metrics.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16819 2023-07-31 22:57:06.000000 bigstream-1.1.5/bigstream/motion_correct.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22197 2023-07-31 21:22:57.000000 bigstream-1.1.5/bigstream/piecewise_align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    17210 2023-07-11 16:34:08.000000 bigstream-1.1.5/bigstream/piecewise_transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16456 2023-07-21 16:14:18.000000 bigstream-1.1.5/bigstream/stitch.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    14215 2023-07-31 22:47:55.000000 bigstream-1.1.5/bigstream/transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    21985 2023-07-31 22:58:23.000000 bigstream-1.1.5/bigstream/utility.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-31 23:01:20.601528 bigstream-1.1.5/bigstream.egg-info/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-07-31 23:01:20.000000 bigstream-1.1.5/bigstream.egg-info/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      517 2023-07-31 23:01:20.000000 bigstream-1.1.5/bigstream.egg-info/SOURCES.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2023-07-31 23:01:20.000000 bigstream-1.1.5/bigstream.egg-info/dependency_links.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      268 2023-07-31 23:01:20.000000 bigstream-1.1.5/bigstream.egg-info/requires.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2023-07-31 23:01:20.000000 bigstream-1.1.5/bigstream.egg-info/top_level.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2023-07-31 23:01:20.608339 bigstream-1.1.5/setup.cfg
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      829 2023-07-31 23:00:51.000000 bigstream-1.1.5/setup.py
```

### Comparing `bigstream-1.1.4/LICENSE.txt` & `bigstream-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.4/README.md` & `bigstream-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.4/bigstream/align.py` & `bigstream-1.1.5/bigstream/align.py`

 * *Files 0% similar despite different names*

```diff
@@ -561,24 +561,24 @@
             except Exception as e:
                 return WORST_POSSIBLE_SCORE
 
     # score all random affines
     current_best_score = WORST_POSSIBLE_SCORE
     scores = np.empty(random_iterations + 1, dtype=np.float64)
     for iii, ppp in enumerate(params):
-        scores[iii] = score_affine(ut.physical_parameters_to_affine_matrix(ppp, center))
+        scores[iii] = score_affine(ut.physical_parameters_to_affine_matrix_3d(ppp, center))
         if print_running_improvements and scores[iii] < current_best_score:
                 current_best_score = scores[iii]
                 print(iii, ': ', current_best_score, '\n', ppp)
     sys.stdout.flush()
 
     # return top results
     partition_indx = np.argpartition(scores, nreturn)[:nreturn]
     params, scores = params[partition_indx], scores[partition_indx]
-    return [ut.physical_parameters_to_affine_matrix(p, center) for p in params[np.argsort(scores)]]
+    return [ut.physical_parameters_to_affine_matrix_3d(p, center) for p in params[np.argsort(scores)]]
 
 
 def affine_align(
     fix,
     mov,
     fix_spacing,
     mov_spacing,
```

### Comparing `bigstream-1.1.4/bigstream/application_pipelines.py` & `bigstream-1.1.5/bigstream/application_pipelines.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.4/bigstream/configure_irm.py` & `bigstream-1.1.5/bigstream/configure_irm.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.4/bigstream/features.py` & `bigstream-1.1.5/bigstream/features.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.4/bigstream/level_set.py` & `bigstream-1.1.5/bigstream/level_set.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.4/bigstream/metrics.py` & `bigstream-1.1.5/bigstream/metrics.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.4/bigstream/motion_correct.py` & `bigstream-1.1.5/bigstream/motion_correct.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         coords = np.meshgrid(x, np.mgrid[:6], indexing='ij')
         params = map_coordinates(params, coords, mode='nearest')
 
     # convert to matrices
     # TODO: again this assumes rigid transforms
     transforms = np.empty((total_frames, 4, 4))
     for i in range(params.shape[0]):
-        e = ut.parameters_to_euler_transform(params[i])
+        e = ut.parameters_to_euler_transform_3d(params[i])
         t = ut.affine_transform_to_matrix(e)
         transforms[i] = t
 
     # return all transforms
     return transforms
```

### Comparing `bigstream-1.1.4/bigstream/piecewise_align.py` & `bigstream-1.1.5/bigstream/piecewise_align.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.4/bigstream/piecewise_transform.py` & `bigstream-1.1.5/bigstream/piecewise_transform.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.4/bigstream/stitch.py` & `bigstream-1.1.5/bigstream/stitch.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.4/bigstream/transform.py` & `bigstream-1.1.5/bigstream/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,18 +166,19 @@
         The given coordinates transformed by the given transform_list
     """
 
     # transform list should be a stack, last added is first applied
     for iii, transform in enumerate(transform_list[::-1]):
 
         # if transform is an affine matrix
-        if transform.shape == (4, 4):
+        if len(transform.shape) == 2:
 
             # matrix vector multiply
-            mm, tt = transform[:3, :3], transform[:3, -1]
+            ndims = transform.shape[0] - 1
+            mm, tt = transform[:ndims, :ndims], transform[:ndims, -1]
             coordinates = np.einsum('...ij,...j->...i', mm, coordinates) + tt
 
         # if transform is a deformation vector field
         else:
 
             # transform_spacing must be given
             error_message = "If transform is a displacement vector field, "
@@ -282,26 +283,26 @@
     composite_transform : nd-array
         The single transform composition of first_transform and second_transform
         If both given transforms are affine this is a 4x4 matrix. Otherwise,
         it is a displacement vector field.
     """
 
     # two affines
-    if first_transform.shape == (4, 4) and second_transform.shape == (4, 4):
+    if len(first_transform.shape) == 2 and len(second_transform.shape) == 2:
         return np.matmul(first_transform, second_transform)
 
     # one affine, two field
-    elif first_transform.shape == (4, 4):
+    elif len(first_transform.shape) == 2:
         first_transform = ut.matrix_to_displacement_field(
             first_transform, second_transform.shape[:-1], second_spacing,
         )
         first_spacing = second_spacing
 
     # one field, two affine
-    elif second_transform.shape == (4, 4):
+    elif len(second_transform.shape) == 2:
         second_transform = ut.matrix_to_displacement_field(
             second_transform, first_transform.shape[:-1], first_spacing,
         )
         second_spacing = first_spacing
 
     # compose fields
     return compose_displacement_vector_fields(
```

### Comparing `bigstream-1.1.4/bigstream/utility.py` & `bigstream-1.1.5/bigstream/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,18 @@
 
     Returns
     -------
     new_matrix : 4x4 array
         The same affine transform but encoded with respect to the given origin
     """
 
-    tl, tr = np.eye(4), np.eye(4)
+    ndims = matrix.shape[0] - 1
+    tl, tr = np.eye(ndims+1), np.eye(ndims+1)
     origin = np.array(origin)
-    tl[:3, -1], tr[:3, -1] = -origin, origin
+    tl[:ndims, -1], tr[:ndims, -1] = -origin, origin
     return np.matmul(tl, np.matmul(matrix, tr))
 
 
 def affine_transform_to_matrix(transform):
     """
     Convert sitk affine transform object to a 4x4 numpy array
 
@@ -214,15 +215,15 @@
     return np.array((transform.GetAngleX(),
                      transform.GetAngleY(),
                      transform.GetAngleZ()) +
                      transform.GetTranslation()
     )
 
 
-def parameters_to_euler_transform(params):
+def parameters_to_euler_transform_3d(params):
     """
     Convert rigid transform parameters to a sitk.Euler3DTransform object
 
     Parameters
     ----------
     rigid_parameters : 1d-array, length 6
         The rigid transform parameters: (rotX, rotY, rotZ, transX, transY, transZ)
@@ -235,15 +236,15 @@
 
     transform = sitk.Euler3DTransform()
     transform.SetRotation(*params[:3])
     transform.SetTranslation(params[3:])
     return transform
 
 
-def physical_parameters_to_affine_matrix(params, center):
+def physical_parameters_to_affine_matrix_3d(params, center):
     """
     Convert separate affine transform parameters to an affine matrix
 
     Parameters
     ----------
     params : 1d-array
         The affine transform parameters
@@ -300,19 +301,19 @@
     Returns
     -------
     displacement_vector_field : nd-array
         Field of shape + (3,) shape and given spacing
     """
 
     if spacing is None: spacing = np.ones(len(shape))
-    nrows, ncols, nstacks = shape
-    grid = np.array(np.mgrid[:nrows, :ncols, :nstacks])
-    grid = grid.transpose(1,2,3,0) * spacing
+    grid = np.array(np.mgrid[tuple(slice(None, x) for x in shape)])
+    grid = np.moveaxis(grid, 0, -1) * spacing
     if centered: grid += 0.5 * spacing
-    mm, tt = matrix[:3, :3], matrix[:3, -1]
+    ndims = matrix.shape[0] - 1
+    mm, tt = matrix[:ndims, :ndims], matrix[:ndims, -1]
     return np.einsum('...ij,...j->...i', mm, grid) + tt - grid
 
 
 def field_to_displacement_field_transform(field, spacing=None, origin=None):
     """
     Convert a displacement vector field numpy array to a sitk displacement field
     transform object
```

### Comparing `bigstream-1.1.4/bigstream.egg-info/SOURCES.txt` & `bigstream-1.1.5/bigstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.4/setup.py` & `bigstream-1.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bigstream",
-    version="1.1.4",
+    version="1.1.5",
     author="Greg M. Fleishman",
     author_email="greg.nli10me@gmail.com",
     description="Tools for distributed alignment of massive images",
     url="https://github.com/GFleishman/bigstream",
     license="MIT",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

