# Comparing `tmp/En-transformer-1.1.0.tar.gz` & `tmp/En-transformer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "En-transformer-1.1.0.tar", last modified: Mon Jul 31 20:37:14 2023, max compression
+gzip compressed data, was "En-transformer-1.2.0.tar", last modified: Tue Aug  1 03:22:45 2023, max compression
```

## Comparing `En-transformer-1.1.0.tar` & `En-transformer-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:37:14.325400 En-transformer-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:37:14.325400 En-transformer-1.1.0/En_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-31 20:37:14.000000 En-transformer-1.1.0/En_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-31 20:37:14.000000 En-transformer-1.1.0/En_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:37:14.000000 En-transformer-1.1.0/En_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 20:37:14.000000 En-transformer-1.1.0/En_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 20:37:14.000000 En-transformer-1.1.0/En_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 20:37:01.000000 En-transformer-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-31 20:37:14.325400 En-transformer-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-31 20:37:01.000000 En-transformer-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:37:14.325400 En-transformer-1.1.0/en_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 20:37:01.000000 En-transformer-1.1.0/en_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-07-31 20:37:01.000000 En-transformer-1.1.0/en_transformer/en_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-31 20:37:01.000000 En-transformer-1.1.0/en_transformer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 20:37:14.325400 En-transformer-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-31 20:37:01.000000 En-transformer-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:22:45.604334 En-transformer-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:22:45.604334 En-transformer-1.2.0/En_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-01 03:22:45.000000 En-transformer-1.2.0/En_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-01 03:22:45.000000 En-transformer-1.2.0/En_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:22:45.000000 En-transformer-1.2.0/En_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 03:22:45.000000 En-transformer-1.2.0/En_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 03:22:45.000000 En-transformer-1.2.0/En_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 03:22:32.000000 En-transformer-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-01 03:22:45.604334 En-transformer-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-08-01 03:22:32.000000 En-transformer-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:22:45.604334 En-transformer-1.2.0/en_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 03:22:32.000000 En-transformer-1.2.0/en_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-08-01 03:22:32.000000 En-transformer-1.2.0/en_transformer/en_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-01 03:22:32.000000 En-transformer-1.2.0/en_transformer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-01 03:22:45.604334 En-transformer-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-01 03:22:32.000000 En-transformer-1.2.0/setup.py
```

### Comparing `En-transformer-1.1.0/En_transformer.egg-info/PKG-INFO` & `En-transformer-1.2.0/En_transformer.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: En-transformer
-Version: 1.1.0
+Version: 1.2.0
 Summary: E(n)-Equivariant Transformer
 Home-page: https://github.com/lucidrains/En-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,transformer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `En-transformer-1.1.0/LICENSE` & `En-transformer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `En-transformer-1.1.0/PKG-INFO` & `En-transformer-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: En-transformer
-Version: 1.1.0
+Version: 1.2.0
 Summary: E(n)-Equivariant Transformer
 Home-page: https://github.com/lucidrains/En-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,transformer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `En-transformer-1.1.0/README.md` & `En-transformer-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `En-transformer-1.1.0/en_transformer/en_transformer.py` & `En-transformer-1.2.0/en_transformer/en_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 
 def default(val, d):
     return val if exists(val) else d
 
 def l2norm(t):
     return F.normalize(t, dim = -1)
 
+def small_init_(t: nn.Linear):
+    nn.init.normal_(t.weight, std = 0.02)
+    nn.init.zeros_(t.bias)
+
 def batched_index_select(values, indices, dim = 1):
     value_dims = values.shape[(dim + 1):]
     values_shape, indices_shape = map(lambda t: list(t.shape), (values, indices))
     indices = indices[(..., *((None,) * len(value_dims)))]
     indices = indices.expand(*((-1,) * len(indices_shape)), *value_dims)
     value_expand_len = len(indices_shape) - (dim + 1)
     values = values[(*((slice(None),) * dim), *((None,) * value_expand_len), ...)]
@@ -243,27 +247,31 @@
         else:
             self.coors_mlp = nn.Sequential(
                 nn.Linear(heads, coors_hidden_dim, bias = False),
                 nn.GELU(),
                 nn.Linear(coors_hidden_dim, heads, bias = False)
             )
 
-        self.coors_gate = nn.Sequential(
-            nn.Linear(heads, heads),
-            nn.Tanh()
-        )
+        self.coors_gate = nn.Linear(heads, heads)
+        small_init_(self.coors_gate)
 
         self.use_cross_product = use_cross_product
         if use_cross_product:
             self.cross_coors_mlp = nn.Sequential(
                 nn.Linear(heads, coors_hidden_dim, bias = False),
                 nn.GELU(),
                 nn.Linear(coors_hidden_dim, heads * 2, bias = False)
             )
 
+            self.cross_coors_gate_i = nn.Linear(heads, heads)
+            self.cross_coors_gate_j = nn.Linear(heads, heads)
+
+            small_init_(self.cross_coors_gate_i)
+            small_init_(self.cross_coors_gate_j)
+
         self.norm_rel_coors = CoorsNorm(scale_init = norm_coors_scale_init) if norm_rel_coors else nn.Identity()
 
         num_coors_combine_heads = (2 if use_cross_product else 1) * heads
         self.coors_combine = nn.Parameter(torch.randn(num_coors_combine_heads))
 
         # positional embedding
         # for both along the sequence (if specified by rel_pos_emb) and the relative distance between each residue / atom
@@ -378,15 +386,15 @@
             mask = q_mask * k_mask
 
             if exists(nbhd_masks):
                 mask &= rearrange(nbhd_masks, 'b i j -> b 1 i j')
 
         # generate and apply rotary embeddings
 
-        rel_dist = -rel_dist
+        rel_dist = -(rel_dist ** 2)
         rel_dist = rearrange(rel_dist, 'b i j -> b 1 i j 1')
 
         if self.rel_pos_emb:
             seq = torch.arange(n, device = device, dtype = q.dtype)
             seq_target_pos = nbhd_indices if exists(nbhd_indices) else rearrange(seq, 'j -> 1 1 j')
             seq_rel_dist = rearrange(seq, 'i -> 1 i 1') - seq_target_pos
             seq_rel_dist = repeat(seq_rel_dist, 'b i j -> b 1 i j 1', b = b)
@@ -443,14 +451,22 @@
             rel_coors_j = repeat(rel_coors, 'b n j c -> b n (i j) c', i = j)
 
             cross_coors = torch.cross(rel_coors_i, rel_coors_j, dim = -1)
 
             cross_coors = self.norm_rel_coors(cross_coors)
             cross_coors = repeat(cross_coors, 'b i j c -> b i j c h', h = h)
 
+            cross_coors_sign_i = self.cross_coors_gate_i(coors_mlp_input)
+            cross_coors_sign_j = self.cross_coors_gate_j(coors_mlp_input)
+
+            cross_coors_sign = rearrange(cross_coors_sign_i, 'b n i h -> b n i 1 h') * rearrange(cross_coors_sign_j, 'b n j h -> b n 1 j h')
+            cross_coors_sign = rearrange(cross_coors_sign, 'b n i j h -> b n (i j) 1 h')
+
+            cross_coors = cross_coors * cross_coors_sign
+
         rel_coors = self.norm_rel_coors(rel_coors)
         rel_coors = repeat(rel_coors, 'b i j c -> b i j c h', h = h)
 
         rel_coors = rel_coors * rel_coors_sign
 
         # cross product
```

### Comparing `En-transformer-1.1.0/setup.py` & `En-transformer-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'En-transformer',
   packages = find_packages(),
-  version = '1.1.0',
+  version = '1.2.0',
   license='MIT',
   description = 'E(n)-Equivariant Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/En-transformer',
   keywords = [
     'artificial intelligence',
```

