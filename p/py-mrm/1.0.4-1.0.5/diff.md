# Comparing `tmp/py_mrm-1.0.4.tar.gz` & `tmp/py_mrm-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_mrm-1.0.4.tar", last modified: Sun Jul 30 19:44:17 2023, max compression
+gzip compressed data, was "py_mrm-1.0.5.tar", last modified: Mon Jul 31 23:04:57 2023, max compression
```

## Comparing `py_mrm-1.0.4.tar` & `py_mrm-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 19:44:17.791519 py_mrm-1.0.4/
--rw-rw-rw-   0        0        0      166 2023-07-30 19:44:17.790520 py_mrm-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6332 2023-07-13 10:27:23.000000 py_mrm-1.0.4/README.md
--rw-rw-rw-   0        0        0     2003 2023-07-30 10:05:52.000000 py_mrm-1.0.4/conf.py
-drwxrwxrwx   0        0        0        0 2023-07-30 19:44:17.704521 py_mrm-1.0.4/py_mrm/
--rw-rw-rw-   0        0        0      152 2023-07-30 09:49:16.000000 py_mrm-1.0.4/py_mrm/__init__.py
--rw-rw-rw-   0        0        0    22714 2023-07-30 19:43:34.000000 py_mrm-1.0.4/py_mrm/py_mrm.py
-drwxrwxrwx   0        0        0        0 2023-07-30 19:44:17.787526 py_mrm-1.0.4/py_mrm.egg-info/
--rw-rw-rw-   0        0        0      166 2023-07-30 19:44:16.000000 py_mrm-1.0.4/py_mrm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-30 19:44:17.000000 py_mrm-1.0.4/py_mrm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 19:44:16.000000 py_mrm-1.0.4/py_mrm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-30 19:44:16.000000 py_mrm-1.0.4/py_mrm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-30 19:44:16.000000 py_mrm-1.0.4/py_mrm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 19:44:17.792518 py_mrm-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      334 2023-07-30 19:43:52.000000 py_mrm-1.0.4/setup.py
--rw-rw-rw-   0        0        0     1330 2023-07-30 08:10:02.000000 py_mrm-1.0.4/test_mrm.py
+drwxrwxrwx   0        0        0        0 2023-07-31 23:04:57.924244 py_mrm-1.0.5/
+-rw-rw-rw-   0        0        0      166 2023-07-31 23:04:57.923243 py_mrm-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6332 2023-07-13 10:27:23.000000 py_mrm-1.0.5/README.md
+-rw-rw-rw-   0        0        0     2003 2023-07-30 10:05:52.000000 py_mrm-1.0.5/conf.py
+drwxrwxrwx   0        0        0        0 2023-07-31 23:04:57.878244 py_mrm-1.0.5/py_mrm/
+-rw-rw-rw-   0        0        0      191 2023-07-31 22:15:19.000000 py_mrm-1.0.5/py_mrm/__init__.py
+-rw-rw-rw-   0        0        0    31508 2023-07-31 23:04:22.000000 py_mrm-1.0.5/py_mrm/py_mrm.py
+drwxrwxrwx   0        0        0        0 2023-07-31 23:04:57.919249 py_mrm-1.0.5/py_mrm.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-07-31 23:04:56.000000 py_mrm-1.0.5/py_mrm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-31 23:04:57.000000 py_mrm-1.0.5/py_mrm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 23:04:56.000000 py_mrm-1.0.5/py_mrm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-31 23:04:56.000000 py_mrm-1.0.5/py_mrm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 23:04:56.000000 py_mrm-1.0.5/py_mrm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 23:04:57.925248 py_mrm-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-07-30 19:55:03.000000 py_mrm-1.0.5/setup.py
+-rw-rw-rw-   0        0        0     1330 2023-07-30 08:10:02.000000 py_mrm-1.0.5/test_mrm.py
```

### Comparing `py_mrm-1.0.4/README.md` & `py_mrm-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `py_mrm-1.0.4/conf.py` & `py_mrm-1.0.5/conf.py`

 * *Files identical despite different names*

### Comparing `py_mrm-1.0.4/py_mrm/py_mrm.py` & `py_mrm-1.0.5/py_mrm/py_mrm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,103 @@
 """
 Module Name: py_mrm
 Author: E.A.J.F. Peters
 License: MIT License
-Version: 1.0.0
+Version: 1.1.0
 
 This module provides functions for multiphase reactor modeling.
 
 Functions:
 
-- construct_grad(axis, sz, x_c, x_f, bc): Construct the gradient matrix.
-- construct_div(axis, sz, x_f, nu): Construct the divergence matrix based on the given parameters.
-- construct_convflux_upwind(axis, sz, x_c, x_f, bc, v): Construct the convective flux matrix based on the given parameters.
-- numjac_local(axis, f, c, eps_jac=1e-6): Compute the local numerical Jacobian matrix and function values for the given function and initial values.
-- interp_stagg_to_cntr(axis, c_f, x_c, x_f): Interpolate values at staggered positions to cell-centers using linear interpolation.
-- interp_cntr_to_stagg(axis, c_f, x_c, x_f): Interpolate values at cell-centered positions to staggered positions using linear interpolation and extrapolation at wall.
+- construct_grad(sz, x_f, x_c=None, bc=None, axis=0): Construct the gradient matrix.
+- construct_grad_int(sz, x_f, x_c=None, axis=0): Construct the gradient matrix for internal faces.
+- construct_grad_bc(sz, x_f, x_c=None, bc=None, axis=0): Construct the gradient matrix for boundary faces.
+- construct_div(sz, x_f, nu=0, axis=0): Construct the divergence matrix based on the given parameters.
+- construct_convflux_upwind(sz, x_f, x_c=None, bc=None, v=0, axis=0): Construct the convective flux matrix based on the given parameters.
+- numjac_local(f, c, eps_jac=1e-6, axis=0): Compute the local numerical Jacobian matrix and function values for the given function and initial values.
+- interp_stagg_to_cntr(c_f, x_f, x_c=None, axis=0): Interpolate values at staggered positions to cell-centers using linear interpolation.
+- interp_cntr_to_stagg(c_f, x_f, x_c=None, axis=0): Interpolate values at cell-centered positions to staggered positions using linear interpolation and extrapolation at the wall.
 - non_uniform_grid(x_L, x_R, n, dx_inf, factor): Generate a non-uniform grid of points in the interval [x_L, x_R].
-- unwrap_bc(sz, bc): Unwrap the boundary conditions for a given size.
-
-Usage:
-1. Use `construct_grad` to construct the gradient matrix.
-2. Use `construct_div` to construct the Div matrix based on the given parameters.
-3. Use `construct_convflux_upwind` to construct the Conv and conv_bc matrices based on the given parameters.
-4. Use `numjac_local` to compute the local numerical Jacobian matrix and function values for the given function and initial values.
-5. Use `interp_stagg_to_cntr` to interpolate values at staggered positions to cell-centers using linear interpolation.
-6. Use `interp_cntr_to_stagg` to interpolate values at cell-centers positions to staggered positions using linear interpolation.
-7. Use `non_uniform_grid` to generate a non-uniform grid of points in the interval [x_L, x_R].
-8. Use `unwrap_bc` to unwrap the boundary conditions for a given size. Mostly used by other functions
+- unwrap_bc(sz, bc): Unwrap the boundary conditions for a given size. Mostly used by other functions.
 
+Note: Please refer to the function descriptions for more details on their arguments and usage.
 """
 
+
 import numpy as np
 from scipy.sparse import csc_array
 import math
 
+def construct_grad(sz, x_f, x_c=None, bc=None, axis=0):
+    """
+    Construct the gradient matrix.
+
+    Args:
+        sz (tuple): Size of the domain.
+        x_f (ndarray): Face coordinates.
+        x_c (ndarray, optional): Cell center coordinates. If not provided, it will be calculated as the average of neighboring face coordinates.
+        bc (dict, optional): Boundary conditions. Default is None.
+        axis (int, optional): Dimension to construct the gradient matrix for. Default is 0.
+
+    Returns:
+        csr_array: Gradient matrix (Grad).
+        csc_array: Contribution of the inhomogeneous BC to the gradient (grad_bc).
+    """
+    if (x_c is None):
+        x_c = 0.5*(x_f[0:-1]+x_f[1:])
+    Grad = construct_grad_int(sz, x_f, x_c, axis)
+    if (bc is None):
+        sz_f = sz.copy()
+        sz_f[axis] +=1
+        grad_bc = csc_array(shape=(math.prod(sz_f),1))
+    else:
+        Grad_bc, grad_bc = construct_grad_bc(sz, x_f, x_c, bc, axis)
+        Grad += Grad_bc
+    return Grad, grad_bc
 
-def construct_grad(axis, sz, x_c, x_f, bc):
+def construct_grad_old(sz, x_f, x_c=None, bc=None, axis=0):
     """
     Construct the gradient matrix.
 
     Args:
-        axis (int): Dimension to construct the gradient matrix for.
         sz (tuple): Size of the domain.
-        x_c (ndarray): Cell center coordinates.
         x_f (ndarray): Face coordinates.
-        bc (dict): Boundary conditions.
+        x_c (ndarray, optional): Cell center coordinates. If not provided, it will be calculated as the average of neighboring face coordinates.
+        bc (dict, optional): Boundary conditions. Default is None.
+        axis (int, optional): Dimension to construct the gradient matrix for. Default is 0.
 
     Returns:
         csr_array: Gradient matrix (Grad).
         csc_array: Contribution of the inhomogeneous BC to the gradient (grad_bc).
     """
     # Trick: Reshape sizes to triplet sz_t
     if not isinstance(sz, (list, tuple)):
         sz_f = [sz]
     else:
         sz_f = list(sz)
     sz_t = [math.prod(sz_f[0:axis]), math.prod(
         sz_f[axis:axis+1]), math.prod(sz_f[axis+1:])]
 
+    if (x_c is None):
+        x_c = 0.5*(x_f[0:-1] + x_f[1:])
+    
     # Create face arrays  
     sz_f[axis] = sz_f[axis] + 1
     sz_f_t = sz_t.copy()
     sz_f_t[1] = sz_t[1] + 1
 
     # Create boundary quantity sizes
     sz_bc = sz_f.copy()
     sz_bc[axis] = 1
     sz_bc_d = [sz_t[0], sz_t[2]]
 
     a, b, d = unwrap_bc(sz, bc)
 
     # Handle special case with one cell in the dimension axis
-    if sz_t[1] == 1:
+    if (sz_t[1] == 1):
         i_c = sz_t[2] * np.arange(sz_t[0]).reshape((-1, 1, 1)) + np.array(
             (0, 0)).reshape((1, -1, 1)) + np.arange(sz_t[2]).reshape((1, 1, -1))
         values = np.zeros(sz_f_t)
         alpha_1 = (x_f[1] - x_f[0]) / ((x_c[0] - x_f[0]) * (x_f[1] - x_c[0]))
         alpha_2L = (x_c[0] - x_f[0]) / ((x_f[1] - x_f[0]) * (x_f[1] - x_c[0]))
         alpha_0L = alpha_1 - alpha_2L
         alpha_2R = -(x_c[0] - x_f[1]) / ((x_f[0] - x_f[1]) * (x_f[0] - x_c[0]))
@@ -152,33 +175,188 @@
     num_f = math.prod(sz_f_t);
     i_f = np.repeat(np.arange(num_f),2)
     Grad = csc_array((values.flatten(), (i_f, i_c.flatten())), 
                       shape=(num_f, math.prod(sz_t)))
     Grad.sort_indices()
         
     grad_bc = csc_array((values_bc.flatten(), i_f_bc.flatten(), [
-                         0, i_f_bc.size]), shape=(math.prod(sz_f_t),))
+                         0, i_f_bc.size]), shape=(math.prod(sz_f_t),1))
 
     return Grad, grad_bc
 
+def construct_grad_int(sz, x_f,  x_c=None, axis=0):
+    """
+    Construct the gradient matrix for internal faces.
+
+    Args:
+        sz (tuple): Size of the domain.
+        x_f (ndarray): Face coordinates.
+        x_c (ndarray, optional): Cell center coordinates. If not provided, it will be calculated as the average of neighboring face coordinates.
+        axis (int, optional): Dimension to construct the gradient matrix for. Default is 0.
+    
+    Returns:
+        csr_array: Gradient matrix (Grad).
+        csc_array: Contribution of the inhomogeneous BC to the gradient (grad_bc).
+    """
+    # Trick: Reshape sizes to triplet sz_t
+    if not isinstance(sz, (list, tuple)):
+        sz_f = [sz]
+    else:
+        sz_f = list(sz)
+    sz_t = [math.prod(sz_f[0:axis]), math.prod(
+        sz_f[axis:axis+1]), math.prod(sz_f[axis+1:])]    
+    i_f = (sz_t[1]+1) * sz_t[2] * np.arange(sz_t[0]).reshape(-1, 1, 1, 1) + sz_t[2] * np.arange(sz_t[1]).reshape((
+        1, -1, 1, 1)) + np.arange(sz_t[2]).reshape((1, 1, -1, 1)) + np.array([0, sz_t[2]]).reshape((1, 1, 1, -1))
+    if (x_c is None):
+        x_c = 0.5*(x_f[:-1] + x_f[1:])
+    dx_inv = np.tile(
+        1 / (x_c[1:] - x_c[:-1]).reshape((1, -1, 1)), (sz_t[0], 1, sz_t[2]))
+    values = np.empty(i_f.shape)
+    values[:,0,:,0] = np.zeros((sz_t[0],sz_t[2]))
+    values[:, 1:, :, 0] = dx_inv
+    values[:, :-1, :, 1] = -dx_inv
+    values[:,-1,:,1] = 0
+    Grad_int = csc_array((values.flatten(), i_f.flatten(), range(0,i_f.size + 1,2)), 
+                      shape=(sz_t[0]*(sz_t[1]+1)*sz_t[2], sz_t[0]*sz_t[1]*sz_t[2]))
+    return Grad_int
+
+def construct_grad_bc(sz, x_f, x_c=None, bc=None, axis=0):
+    """
+    Construct the gradient matrix for the boundary faces 
+
+    Args:
+        sz (tuple): Size of the domain.
+        x_f (ndarray): Face coordinates.
+        x_c (ndarray, optional): Cell center coordinates. If not provided, it will be calculated as the average of neighboring face coordinates.
+        bc (dict, optional): Boundary conditions. Default is None.
+        axis (int, optional): Dimension to construct the gradient matrix for. Default is 0.
+
+    Returns:
+        csr_array: Gradient matrix (Grad).
+        csc_array: Contribution of the inhomogeneous BC to the gradient (grad_bc).
+    """
+    # Trick: Reshape sizes to triplet sz_t
+    if not isinstance(sz, (list, tuple)):
+        sz_f = [sz]
+    else:
+        sz_f = list(sz)
+    sz_t = [math.prod(sz_f[0:axis]), math.prod(
+        sz_f[axis:axis+1]), math.prod(sz_f[axis+1:])]
+    
+    # Create face arrays  
+    sz_f[axis] = sz_f[axis] + 1
+    sz_f_t = sz_t.copy()
+    sz_f_t[1] = sz_t[1] + 1
+
+    # Create boundary quantity sizes
+    sz_bc = sz_f.copy()
+    sz_bc[axis] = 1
+    sz_bc_d = [sz_t[0], sz_t[2]]
+
+    a, b, d = unwrap_bc(sz, bc)
+
+    # Handle special case with one cell in the dimension axis
+    if (sz_t[1] == 1):
+        if (x_c is None):
+            x_c = 0.5*(x_f[0:-1] + x_f[1:])
+        i_c = sz_t[2] * np.arange(sz_t[0]).reshape((-1, 1, 1)) + np.array(
+            (0, 0)).reshape((1, -1, 1)) + np.arange(sz_t[2]).reshape((1, 1, -1))
+        values = np.zeros(sz_f_t)
+        alpha_1 = (x_f[1] - x_f[0]) / ((x_c[0] - x_f[0]) * (x_f[1] - x_c[0]))
+        alpha_2L = (x_c[0] - x_f[0]) / ((x_f[1] - x_f[0]) * (x_f[1] - x_c[0]))
+        alpha_0L = alpha_1 - alpha_2L
+        alpha_2R = -(x_c[0] - x_f[1]) / ((x_f[0] - x_f[1]) * (x_f[0] - x_c[0]))
+        alpha_0R = alpha_1 - alpha_2R
+        fctr = ((b[0] + alpha_0L * a[0]) * (b[1] +
+                    alpha_0R * a[1]) - alpha_2L * alpha_2R * a[0] * a[1])
+        np.divide(1, fctr, out=fctr, where=(fctr != 0))
+        value = alpha_1 * \
+            b[0] * (a[1] * (alpha_0R - alpha_2L) + b[1]) * fctr + np.zeros(sz)
+        values[:, 0, :] = np.reshape(value, sz_bc_d)
+        value = alpha_1 * \
+            b[1] * (a[0] * (-alpha_0L + alpha_2R) - b[0]) * fctr + np.zeros(sz)
+        values[:, 1, :] = np.reshape(value, sz_bc_d)
+
+        i_f_bc = sz_f_t[1] * sz_f_t[2] * np.arange(sz_f_t[0]).reshape((-1, 1, 1)) + sz_f_t[2] * np.array(
+            [0, sz_f_t[1]-1]).reshape((1, -1, 1)) + np.arange(sz_f_t[2]).reshape((1, 1, -1))
+        values_bc = np.zeros((sz_t[0], 2, sz_t[2]))
+        value = ((a[1] * (-alpha_0L * alpha_0R + alpha_2L * alpha_2R) - alpha_0L *
+                 b[1]) * d[0] - alpha_2L * b[0] * d[1]) * fctr + np.zeros(sz_bc)
+        values_bc[:, 0, :] = np.reshape(value, sz_bc_d)
+        value = ((a[0] * (+alpha_0L * alpha_0R - alpha_2L * alpha_2R) + alpha_0R *
+                 b[0]) * d[1] + alpha_2R * b[1] * d[0]) * fctr + np.zeros(sz_bc)
+        values_bc[:, 1, :] = np.reshape(value, sz_bc_d)
+    else:
+        i_c = sz_t[1] * sz_t[2] * np.arange(sz_t[0]).reshape(-1, 1, 1) + sz_t[2] * np.array([0,1,sz_t[1]-2, sz_t[1]-1]).reshape((
+            1, -1, 1)) + np.arange(sz_t[2]).reshape((1, 1, -1))
+        i_f = sz_f_t[1] * sz_t[2] * np.arange(sz_t[0]).reshape(-1, 1, 1) + sz_t[2] * np.array([0,0,sz_f_t[1]-1, sz_f_t[1]-1]).reshape((
+            1, -1, 1)) + np.arange(sz_t[2]).reshape((1, 1, -1))
+        i_f_bc = sz_f_t[1] * sz_f_t[2] * np.arange(sz_f_t[0]).reshape((-1, 1, 1)) + sz_f_t[2] * np.array(
+            [0, sz_f_t[1]-1]).reshape((1, -1, 1)) + np.arange(sz_f_t[2]).reshape((1, 1, -1))
+        values_bc = np.zeros((sz_t[0], 2, sz_t[2]))
+        values = np.zeros((sz_t[0], 4, sz_t[2]))
+        if (x_c is None):
+            x_c = 0.5*np.array([x_f[0] + x_f[1], x_f[1] + x_f[2], x_f[-3] + x_f[-2], x_f[-2] + x_f[-1]])
+        dx_inv = np.tile(
+            1 / (x_c[1:] - x_c[:-1]).reshape((1, -1, 1)), (sz_t[0], 1, sz_t[2]))
 
-def construct_div(axis, sz, x_f, nu):
+        alpha_1 = (x_c[1] - x_f[0]) / ((x_c[0] - x_f[0]) * (x_c[1] - x_c[0]))
+        alpha_2 = (x_c[0] - x_f[0]) / ((x_c[1] - x_f[0]) * (x_c[1] - x_c[0]))
+        alpha_0 = alpha_1 - alpha_2
+        b[0] = b[0] / alpha_0
+        fctr = (a[0] + b[0])
+        np.divide(1, fctr, out=fctr, where=(fctr != 0))
+        b_fctr = b[0] * fctr
+        b_fctr = b_fctr + np.zeros(sz_bc)
+        b_fctr = np.reshape(b_fctr, sz_bc_d)
+        d_fctr = d[0] * fctr
+        d_fctr = d_fctr + np.zeros(sz_bc)
+        d_fctr = np.reshape(d_fctr, sz_bc_d)
+        values[:, 0, :] = b_fctr * alpha_1
+        values[:, 1, :] = -b_fctr * alpha_2
+        values_bc[:, 0, :] = -d_fctr
+
+        alpha_1 = -(x_c[-2] - x_f[-1]) / ((x_c[-1] - x_f[-1]) * (x_c[-2] - x_c[-1]))
+        alpha_2 = -(x_c[-1] - x_f[-1]) / ((x_c[-2] - x_f[-1]) * (x_c[-2] - x_c[-1]))
+        alpha_0 = alpha_1 - alpha_2
+        b[-1] = b[-1] / alpha_0
+        fctr = (a[-1] + b[-1])
+        np.divide(1, fctr, out=fctr, where=(fctr != 0))
+        b_fctr = b[-1] * fctr
+        b_fctr = b_fctr + np.zeros(sz_bc)
+        b_fctr = np.reshape(b_fctr, sz_bc_d)
+        d_fctr = d[-1] * fctr
+        d_fctr = d_fctr + np.zeros(sz_bc)
+        d_fctr = np.reshape(d_fctr, sz_bc_d)
+        values[:, -2, :] = b_fctr * alpha_2
+        values[:, -1, :] = -b_fctr * alpha_1
+        values_bc[:, -1, :] = d_fctr
+
+    Grad = csc_array((values.flatten(), (i_f.flatten(), i_c.flatten())), 
+                      shape=(math.prod(sz_f_t), math.prod(sz_t)))
+    grad_bc = csc_array((values_bc.flatten(), i_f_bc.flatten(), [
+                         0, i_f_bc.size]), shape=(math.prod(sz_f_t),1))
+    return Grad, grad_bc
+
+def construct_div(sz, x_f, nu=0, axis=0):
     """
     Construct the Div matrix based on the given parameters.
 
     Args:
-        axis (int): The axis along which the numerical differentiation is performed
-        sz (tuple): The size of the matrix.
-        x_f (ndarray): The face array.
+        sz (tuple): Size of the matrix.
+        x_f (ndarray): Face array.
         nu (callable or int): The function or integer representing nu.
+        axis (int): The axis along which the numerical differentiation is performed. Default is 0.
 
     Returns:
         csc_array: The Div matrix.
 
     """
+    # Rest of the function code...
+
     # Trick: Reshape sizes to triplet sz_t
     if not isinstance(sz, (list, tuple)):
         sz_f = [sz]
     else:
         sz_f = list(sz)
     sz_t = [math.prod(sz_f[0:axis]), math.prod(
         sz_f[axis:axis + 1]), math.prod(sz_f[axis + 1:])]
@@ -225,25 +403,25 @@
                            i_f.flatten())),
         shape=(num_cells, np.prod(sz_f_t, dtype=int))
     )
     Div.sort_indices()
     return Div
 
 
-def construct_convflux_upwind(axis, sz, x_c, x_f, bc, v):
+def construct_convflux_upwind(sz, x_f, x_c=None, bc=None, v=1.0, axis=0):
     """
     Construct the Conv and conv_bc matrices based on the given parameters.
 
     Args:
-        axis (int): The axis along which the numerical differentiation is performed.
-        sz (tuple): The size of the matrices.
-        x_c (ndarray): The cell array.
+        sz (tuple): Size of the matrices.
+        x_c (ndarray, optional): The cell array. If not provided, it will be calculated based on the face array.
         x_f (ndarray): The face array.
-        bc (list): The boundary conditions.
+        bc (list, optional): The boundary conditions. Default is None.
         v (ndarray): The velocity array.
+        axis (int, optional): The axis along which the numerical differentiation is performed. Default is 0.
 
     Returns:
         csc_array: The Conv matrix.
         csc_array: The conv_bc matrix.
 
     """
     if not isinstance(sz, (list, tuple)):
@@ -276,28 +454,28 @@
         alpha_0L = alpha_1 - alpha_2L
         alpha_2R = -(x_c[0] - x_f[1]) / ((x_f[0] - x_f[1]) * (x_f[0] - x_c[0]))
         alpha_0R = alpha_1 - alpha_2R
         fctr = ((b[0] + alpha_0L * a[0]) * (b[1] +
                      alpha_0R * a[1]) - alpha_2L * alpha_2R * a[0] * a[1])
         np.divide(1, fctr, out=fctr, where=(fctr != 0))
         values[:, 0, :] = ((alpha_1 * a[0] * (a[1] * (alpha_0R - alpha_2L) + b[1])
-                           * fctr + np.zeros(sz)).reshape(sz_bc_d) - 1) * fltr_v_pos[:, 0, :] + 1
+                           * fctr + np.zeros(sz)).reshape(sz_bc_d))
         values[:, 1, :] = ((alpha_1 * a[1] * (a[0] * (alpha_0L - alpha_2R) + b[0])
-                           * fctr + np.zeros(sz)).reshape(sz_bc_d) - 1) * ~fltr_v_pos[:, -1, :] + 1
+                           * fctr + np.zeros(sz)).reshape(sz_bc_d))
         values = values * v
         Conv = csr_array((values.flatten(), i_c.flatten(), np.arange(
             0, i_c.size + 1)), shape=(math.prod(sz_f_t), math.prod(sz_t)))
 
         i_f_bc = sz_f_t[1] * sz_f_t[2] * np.arange(sz_f_t[0]).reshape((-1, 1, 1)) + sz_f_t[2] * np.array(
             [0, sz_f_t[1] - 1]).reshape((1, -1, 1)) + np.arange(sz_f_t[2]).reshape((1, 1, -1))
         values_bc = np.zeros((sz_t[0], 2, sz_t[2]))
         values_bc[:, 0, :] = ((((a[1] * alpha_0R + b[1]) * d[0] - alpha_2L * a[0] * d[1])
-                              * fctr + np.zeros(sz_bc)).reshape(sz_bc_d)) * fltr_v_pos[:, 0, :]
+                              * fctr + np.zeros(sz_bc)).reshape(sz_bc_d))
         values_bc[:, 1, :] = ((((a[0] * alpha_0L + b[0]) * d[1] - alpha_2R * a[1] * d[0])
-                              * fctr + np.zeros(sz_bc)).reshape(sz_bc_d)) * ~fltr_v_pos[:, -1, :]
+                              * fctr + np.zeros(sz_bc)).reshape(sz_bc_d))
         values_bc = values_bc * v
     else:
         i_f = np.zeros((sz_f_t[0], sz_f_t[1] + 2, sz_f_t[2]), dtype=int)
         i_f[:, 1:-1, :] = np.arange(math.prod(sz_f_t)).reshape(sz_f_t)
         i_f[:, 0, :] = sz_f_t[1] * sz_f_t[2] * \
             np.arange(sz_f_t[0]).reshape(-1, 1) + \
             np.arange(sz_f_t[2]).reshape(1, -1)
@@ -323,18 +501,17 @@
         np.divide(1, fctr, out=fctr, where=(fctr != 0))
         a_fctr = a[0] * fctr
         a_fctr = a_fctr + np.zeros(sz_bc)
         a_fctr = np.reshape(a_fctr, sz_bc_d)
         d_fctr = d[0] * fctr
         d_fctr = d_fctr + np.zeros(sz_bc)
         d_fctr = np.reshape(d_fctr, sz_bc_d)
-        values[:, 0, :] = (1 + (a_fctr * alpha_1 - 1) *
-                           fltr_v_pos[:, 0, :]) * v[:, 0, :]
-        values[:, 1, :] = -a_fctr * alpha_2 * fltr_v_pos[:, 0, :] * v[:, 0, :]
-        values_bc[:, 0, :] = d_fctr * v[:, 0, :] * fltr_v_pos[:, 0, :]
+        values[:, 0, :] = (a_fctr * alpha_1) * v[:, 0, :]
+        values[:, 1, :] = -a_fctr * alpha_2 * v[:, 0, :]
+        values_bc[:, 0, :] = d_fctr * v[:, 0, :]
 
         alpha_1 = -(x_c[-2] - x_f[-1]) / \
             ((x_c[-1] - x_f[-1]) * (x_c[-2] - x_c[-1]))
         alpha_2 = -(x_c[-1] - x_f[-1]) / \
             ((x_c[-2] - x_f[-1]) * (x_c[-2] - x_c[-1]))
         alpha_0 = alpha_1 - alpha_2
         fctr = (alpha_0 * a[-1] + b[-1])
@@ -343,39 +520,39 @@
         a_fctr = a_fctr + np.zeros(sz_bc)
         a_fctr = np.reshape(a_fctr, sz_bc_d)
         d_fctr = d[-1] * fctr
         d_fctr = d_fctr + np.zeros(sz_bc)
         d_fctr = np.reshape(d_fctr, sz_bc_d)
         values[:, -1, :] = (1 + (a_fctr * alpha_1 - 1) * ~
                             fltr_v_pos[:, -1, :]) * v[:, -1, :]
-        values[:, -2, :] = a_fctr * alpha_2 * \
-            ~fltr_v_pos[:, -1, :] * v[:, -1, :]
-        values_bc[:, -1, :] = d_fctr * v[:, -1, :] * ~fltr_v_pos[:, -1, :]
+        values[:, -2, :] = a_fctr * alpha_2 * v[:, -1, :]
+        values_bc[:, -1, :] = d_fctr * v[:, -1, :]
         Conv = csc_array((values.flatten(), (i_f.flatten(), i_c.flatten())), shape=(
             math.prod(sz_f_t), math.prod(sz_t)))
         Conv.sort_indices()
 
     conv_bc = csc_array((values_bc.flatten(), i_f_bc.flatten(), [
-                         0, i_f_bc.size]), shape=(math.prod(sz_f_t),))
+                         0, i_f_bc.size]), shape=(math.prod(sz_f_t),1))
     return Conv, conv_bc
 
-def numjac_local(axis, f, c, eps_jac=1e-6):
+def numjac_local(f, c, eps_jac=1e-6, axis=0):
     """
     Compute the local numerical Jacobian matrix and function values for the given function and initial values.
-    The function f is assumed local, f can be dependent on other components in the array dimension 'axis'.
-    numjac_local can be used to compute Jacobians of e.g. reaction, accumulation or mass transfer terms, where there 
-    is a only dependence of local components in a spatial cell.
-    The best choice is to set up the problem such that axis is the last dimension of the multidimensional array, 
-    because this will give to a nicely block structured Jacoian matrix.  
+    
+    The function 'f' is assumed to be local, meaning it can be dependent on other components in the array along the 'axis' dimension.
+    numjac_local can be used to compute Jacobians of functions like reaction, accumulation, or mass transfer terms, where there 
+    is a dependence only on local components in a spatial cell.
+    The best choice is to set up the problem such that 'axis' is the last dimension of the multidimensional array, 
+    as this will result in a nicely block-structured Jacobian matrix.
 
     Args:
-        axis (int): The axis along which components are coupled.
         f (callable): The function for which to compute the Jacobian.
         c (ndarray): The value at which the Jacobian should be evaluated.
         eps_jac (float, optional): The perturbation value for computing the Jacobian. Defaults to 1e-6.
+        axis (int, optional): The axis along which components are coupled. Default is 0.
 
     Returns:
         csc_array: The Jacobian matrix.
         ndarray: The function values.
 
     """
     sz = c.shape
@@ -395,15 +572,15 @@
         f_perturb = f(c_perturb.reshape(sz)).reshape(sz_t)
         values[:, k, :, :] = np.transpose((f_perturb - f_value) / dc[:, [k], :],(0,2,1))
     Jac = csc_array((values.flatten(), i.flatten(), np.arange(
         0, i.size + sz_t[1], sz_t[1])), shape=(np.prod(sz_t), np.prod(sz_t)))
     return Jac, f_value.reshape(sz)
 
 
-def interp_stagg_to_cntr(axis, c_f, x_c, x_f):
+def interp_stagg_to_cntr(c_f, x_f, x_c = None, axis = 0):
     """
     Interpolate values at staggered positions to cell-centers using linear interpolation.
 
     Args:
         axis (int): Dimension that is interpolated.
         c_f (ndarray): Quantities at staggered positions.
         x_c (ndarray): Cell-centered positions.
@@ -416,42 +593,47 @@
     sz_f = list(c_f.shape)
     sz_f = sz_f + [1,] * (1 + axis - len(sz_f))  # size padded with extra 1's if needed
     sz_f_t = [math.prod(sz_f[:axis]), sz_f[axis], math.prod(sz_f[axis + 1:])]  # sizes for reshape as a triplet
     sz = sz_f.copy()
     sz[axis] = sz[axis] - 1
     sz_t = sz_f_t.copy()
     sz_t[1] = sz[axis]
-    wght = (x_c - x_f[:-1]) / (x_f[1:] - x_f[:-1])
     c_f = c_f.reshape(sz_f_t)
-    c_c = c_f[:, :-1, :] + wght.reshape((1,-1,1)) * (c_f[:, 1:, :] - c_f[:, :-1, :])
+    if (x_c is None):
+        c_c =  0.5 * (c_f[:, 1:, :] + c_f[:, :-1, :])
+    else:
+        wght = (x_c - x_f[:-1]) / (x_f[1:] - x_f[:-1])
+        c_c = c_f[:, :-1, :] + wght.reshape((1,-1,1)) * (c_f[:, 1:, :] - c_f[:, :-1, :])
     c_c = c_c.reshape(sz)
 
     return c_c
 
-def interp_cntr_to_stagg(axis, c_c, x_c, x_f):
+def interp_stagg_to_cntr(c_f, x_f, x_c=None, axis=0):
     """
-    Interpolate values at cell-centers to staggered positions using linear interpolation and extrapolation at the wall.
+    Interpolate values at staggered positions to cell-centers using linear interpolation.
 
     Args:
-        axis (int): Dimension that is interpolated.
         c_f (ndarray): Quantities at staggered positions.
-        x_c (ndarray): Cell-centered positions.
         x_f (ndarray): Positions of cell-faces (numel(x_f) = numel(x_c) + 1).
+        x_c (ndarray, optional): Cell-centered positions. If not provided, the interpolated values will be averaged between adjacent staggered positions.
+        axis (int, optional): Dimension along which interpolation is performed. Default is 0.
 
     Returns:
         ndarray: Interpolated concentrations at the cell-centered positions.
 
     """
     sz = list(c_c.shape)
     sz = sz + [1,] * (1 + axis - len(sz))  # size padded with extra 1's if needed
     sz_t = [math.prod(sz[:axis]), sz[axis], math.prod(sz[axis + 1:])]  # sizes for reshape as a triplet
     sz_f = sz.copy()
     sz_f[axis] = sz[axis] + 1
     sz_f_t = sz_t.copy()
     sz_f_t[1] = sz_f[axis]
+    if (x_c is None):
+        x_c = 0.5*(x_f[:-1]+x_f[1:])
     wght = (x_f[1:-1] - x_c[:-1]) / (x_c[1:] - x_c[:-1])
     c_c = c_c.reshape(sz_t)
     c_f = np.empty(sz_f_t)
     c_f[:,1:-1,:] = c_c[:, :-1, :] + wght.reshape((1,-1,1)) * (c_c[:, 1:, :] - c_c[:, :-1, :])
     c_f[:,0,:] = (c_c[:,0,:]*(x_c[1]-x_f[0]) - c_c[:,1,:]*(x_c[0]-x_f[0]))/(x_c[1]-x_c[0])
     c_f[:,-1,:] = (c_c[:,-1,:]*(x_f[-1]-x_c[-2]) - c_c[:,-2,:]*(x_f[-1]-x_c[-1]))/(x_c[-1]-x_c[-2])
     c_f = c_f.reshape(sz_f)
@@ -493,24 +675,33 @@
     Returns:
         tuple: Unwrapped boundary conditions (a, b, d).
     """
     if not isinstance(sz, (list,tuple)):
         lgth_sz = 1
     else:
         lgth_sz = len(sz)
-    
+      
     a = [None, None]
-    a[0] = np.array(bc['a'][0])
-    a[0] = a[0][(..., *([np.newaxis]*(lgth_sz-a[0].ndim)))]
-    a[1] = np.array(bc['a'][1])
-    a[1] = a[1][(..., *([np.newaxis]*(lgth_sz-a[1].ndim)))]
     b = [None, None]
-    b[0] = np.array(bc['b'][0])
-    b[0] = b[0][(..., *([np.newaxis]*(lgth_sz-b[0].ndim)))]
-    b[1] = np.array(bc['b'][1])
-    b[1] = b[1][(..., *([np.newaxis]*(lgth_sz-b[1].ndim)))]
     d = [None, None]
-    d[0] = np.array(bc['d'][0])
-    d[0] = d[0][(..., *([np.newaxis]*(lgth_sz-d[0].ndim)))]
-    d[1] = np.array(bc['d'][1])
-    d[1] = d[1][(..., *([np.newaxis]*(lgth_sz-d[1].ndim)))]
+    
+    if (bc is None):
+        a[0] = np.zeros((1,) * lgth_sz)
+        a[1] = np.zeros((1,) * lgth_sz)
+        b[0] = np.zeros((1,) * lgth_sz)
+        b[1] = np.zeros((1,) * lgth_sz)
+        d[0] = np.zeros((1,) * lgth_sz)
+        d[1] = np.zeros((1,) * lgth_sz)
+    else:
+        a[0] = np.array(bc['a'][0])
+        a[0] = a[0][(..., *([np.newaxis]*(lgth_sz-a[0].ndim)))]
+        a[1] = np.array(bc['a'][1])
+        a[1] = a[1][(..., *([np.newaxis]*(lgth_sz-a[1].ndim)))]
+        b[0] = np.array(bc['b'][0])
+        b[0] = b[0][(..., *([np.newaxis]*(lgth_sz-b[0].ndim)))]
+        b[1] = np.array(bc['b'][1])
+        b[1] = b[1][(..., *([np.newaxis]*(lgth_sz-b[1].ndim)))]
+        d[0] = np.array(bc['d'][0])
+        d[0] = d[0][(..., *([np.newaxis]*(lgth_sz-d[0].ndim)))]
+        d[1] = np.array(bc['d'][1])
+        d[1] = d[1][(..., *([np.newaxis]*(lgth_sz-d[1].ndim)))]
     return a, b, d
```

### Comparing `py_mrm-1.0.4/test_mrm.py` & `py_mrm-1.0.5/test_mrm.py`

 * *Files identical despite different names*

