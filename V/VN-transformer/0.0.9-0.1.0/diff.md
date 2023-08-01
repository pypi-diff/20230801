# Comparing `tmp/VN-transformer-0.0.9.tar.gz` & `tmp/VN-transformer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VN-transformer-0.0.9.tar", last modified: Sat Jul 29 18:34:56 2023, max compression
+gzip compressed data, was "VN-transformer-0.1.0.tar", last modified: Tue Aug  1 14:50:04 2023, max compression
```

## Comparing `VN-transformer-0.0.9.tar` & `VN-transformer-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:34:56.502180 VN-transformer-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-29 18:34:56.502180 VN-transformer-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:34:56.498180 VN-transformer-0.0.9/VN_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/VN_transformer/VN_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/VN_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/VN_transformer/rotations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:34:56.502180 VN-transformer-0.0.9/VN_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-29 18:34:56.000000 VN-transformer-0.0.9/VN_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-29 18:34:56.000000 VN-transformer-0.0.9/VN_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:34:56.000000 VN-transformer-0.0.9/VN_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 18:34:56.000000 VN-transformer-0.0.9/VN_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 18:34:56.000000 VN-transformer-0.0.9/VN_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-29 18:34:56.502180 VN-transformer-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:34:56.502180 VN-transformer-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-29 18:34:45.000000 VN-transformer-0.0.9/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:50:04.674222 VN-transformer-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 14:49:52.000000 VN-transformer-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-01 14:50:04.674222 VN-transformer-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-08-01 14:49:52.000000 VN-transformer-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:50:04.674222 VN-transformer-0.1.0/VN_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-08-01 14:49:52.000000 VN-transformer-0.1.0/VN_transformer/VN_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-01 14:49:52.000000 VN-transformer-0.1.0/VN_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-08-01 14:49:52.000000 VN-transformer-0.1.0/VN_transformer/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-01 14:49:52.000000 VN-transformer-0.1.0/VN_transformer/rotations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:50:04.674222 VN-transformer-0.1.0/VN_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-01 14:50:04.000000 VN-transformer-0.1.0/VN_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-01 14:50:04.000000 VN-transformer-0.1.0/VN_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:50:04.000000 VN-transformer-0.1.0/VN_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 14:50:04.000000 VN-transformer-0.1.0/VN_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 14:50:04.000000 VN-transformer-0.1.0/VN_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-01 14:50:04.674222 VN-transformer-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-01 14:49:52.000000 VN-transformer-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:50:04.674222 VN-transformer-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-01 14:49:52.000000 VN-transformer-0.1.0/tests/test.py
```

### Comparing `VN-transformer-0.0.9/LICENSE` & `VN-transformer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `VN-transformer-0.0.9/PKG-INFO` & `VN-transformer-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.9
+Version: 0.1.0
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.9/README.md` & `VN-transformer-0.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 ## VN (Vector Neuron) Transformer
 
 A <a href="https://arxiv.org/abs/2206.04176">Transformer made of Rotation-equivariant Attention</a> using <a href="https://arxiv.org/abs/2104.12229">Vector Neurons</a>
 
 <a href="https://openreview.net/forum?id=EiX2L4sDPG">Open Review</a>
 
+## Appreciation
+
+- <a href="https://stability.ai/">StabilityAI</a> for the generous sponsorship, as well as my other sponsors, for affording me the independence to open source artificial intelligence.
+
 ## Install
 
 ```bash
 $ pip install VN-transformer
 ```
 
 ## Usage
@@ -23,34 +27,43 @@
     depth = 2,
     dim_head = 64,
     heads = 8,
     dim_feat = 64,       # will default to early fusion, since this was the best performing
     bias_epsilon = 1e-6  # in this paper, they propose breaking equivariance with a tiny bit of bias noise in the VN linear. they claim this leads to improved stability. setting this to 0 would turn off the epsilon approximate equivariance
 )
 
-feats = torch.randn(1, 32, 64)
 coors = torch.randn(1, 32, 3)    # (batch, sequence, spatial coordinates)
+feats = torch.randn(1, 32, 64)
 
-out = model(coors, feats = feats) # (1, 32, 64 + 3 = 67)
+coors_out, feats_out = model(coors, feats = feats) # (1, 32, 3), (1, 32, 64)
 ```
 
 ## Tests
 
 Confidence in equivariance
 
 ```bash
 $ python setup.py test
 ```
 
-## Todo
+## Example
+
+First install `sidechainnet`
+
+```bash
+$ pip install sidechainnet
+```
+
+Then run the protein backbone denoising task
+
+```bash
+$ python denoise.py
+```
 
-- [x] complete the perceiver like feature aggregation
-- [x] offer early fusion within `VNTransformer` with setting of `dim_feat`
-- [ ] see if it is straightforward to make translation in/equivariant
-    - [ ] test on protein backbone denoising if above could be done
+It does not perform as well as <a href="https://github.com/lucidrains/En-transformer">En-Transformer</a>, nor <a href="https://github.com/lucidrains/equiformer-pytorch">Equiformer</a>
 
 ## Citations
 
 ```bibtex
 @inproceedings{Assaad2022VNTransformerRA,
     title   = {VN-Transformer: Rotation-Equivariant Attention for Vector Neurons},
     author  = {Serge Assaad and C. Downey and Rami Al-Rfou and Nigamaa Nayakanti and Benjamin Sapp},
@@ -64,7 +77,26 @@
     author  = {Congyue Deng and Or Litany and Yueqi Duan and Adrien Poulenard and Andrea Tagliasacchi and Leonidas J. Guibas},
     journal = {2021 IEEE/CVF International Conference on Computer Vision (ICCV)},
     year    = {2021},
     pages   = {12180-12189},
     url     = {https://api.semanticscholar.org/CorpusID:233394028}
 }
 ```
+
+```bibtex
+@inproceedings{Kim2020TheLC,
+    title   = {The Lipschitz Constant of Self-Attention},
+    author  = {Hyunjik Kim and George Papamakarios and Andriy Mnih},
+    booktitle = {International Conference on Machine Learning},
+    year    = {2020},
+    url     = {https://api.semanticscholar.org/CorpusID:219530837}
+}
+```
+
+```bibtex
+@inproceedings{dao2022flashattention,
+    title   = {Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-Awareness},
+    author  = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+    booktitle = {Advances in Neural Information Processing Systems},
+    year    = {2022}
+}
+```
```

#### html2text {}

```diff
@@ -1,25 +1,34 @@
 [./vn-transformer.png] ## VN (Vector Neuron) Transformer A Transformer_made_of
-Rotation-equivariant_Attention using Vector_Neurons Open_Review ## Install
-```bash $ pip install VN-transformer ``` ## Usage ```python import torch from
-VN_transformer import VNTransformer model = VNTransformer( dim = 64, depth = 2,
-dim_head = 64, heads = 8, dim_feat = 64, # will default to early fusion, since
-this was the best performing bias_epsilon = 1e-6 # in this paper, they propose
-breaking equivariance with a tiny bit of bias noise in the VN linear. they
-claim this leads to improved stability. setting this to 0 would turn off the
-epsilon approximate equivariance ) feats = torch.randn(1, 32, 64) coors =
-torch.randn(1, 32, 3) # (batch, sequence, spatial coordinates) out = model
-(coors, feats = feats) # (1, 32, 64 + 3 = 67) ``` ## Tests Confidence in
-equivariance ```bash $ python setup.py test ``` ## Todo - [x] complete the
-perceiver like feature aggregation - [x] offer early fusion within
-`VNTransformer` with setting of `dim_feat` - [ ] see if it is straightforward
-to make translation in/equivariant - [ ] test on protein backbone denoising if
-above could be done ## Citations ```bibtex @inproceedings
-{Assaad2022VNTransformerRA, title = {VN-Transformer: Rotation-Equivariant
-Attention for Vector Neurons}, author = {Serge Assaad and C. Downey and Rami
-Al-Rfou and Nigamaa Nayakanti and Benjamin Sapp}, year = {2022} } ``` ```bibtex
-@article{Deng2021VectorNA, title = {Vector Neurons: A General Framework for SO
-(3)-Equivariant Networks}, author = {Congyue Deng and Or Litany and Yueqi Duan
-and Adrien Poulenard and Andrea Tagliasacchi and Leonidas J. Guibas}, journal =
-{2021 IEEE/CVF International Conference on Computer Vision (ICCV)}, year =
-{2021}, pages = {12180-12189}, url = {https://api.semanticscholar.org/CorpusID:
-233394028} } ```
+Rotation-equivariant_Attention using Vector_Neurons Open_Review ## Appreciation
+- StabilityAI for the generous sponsorship, as well as my other sponsors, for
+affording me the independence to open source artificial intelligence. ##
+Install ```bash $ pip install VN-transformer ``` ## Usage ```python import
+torch from VN_transformer import VNTransformer model = VNTransformer( dim = 64,
+depth = 2, dim_head = 64, heads = 8, dim_feat = 64, # will default to early
+fusion, since this was the best performing bias_epsilon = 1e-6 # in this paper,
+they propose breaking equivariance with a tiny bit of bias noise in the VN
+linear. they claim this leads to improved stability. setting this to 0 would
+turn off the epsilon approximate equivariance ) coors = torch.randn(1, 32, 3) #
+(batch, sequence, spatial coordinates) feats = torch.randn(1, 32, 64)
+coors_out, feats_out = model(coors, feats = feats) # (1, 32, 3), (1, 32, 64)
+``` ## Tests Confidence in equivariance ```bash $ python setup.py test ``` ##
+Example First install `sidechainnet` ```bash $ pip install sidechainnet ```
+Then run the protein backbone denoising task ```bash $ python denoise.py ``` It
+does not perform as well as En-Transformer, nor Equiformer ## Citations
+```bibtex @inproceedings{Assaad2022VNTransformerRA, title = {VN-Transformer:
+Rotation-Equivariant Attention for Vector Neurons}, author = {Serge Assaad and
+C. Downey and Rami Al-Rfou and Nigamaa Nayakanti and Benjamin Sapp}, year =
+{2022} } ``` ```bibtex @article{Deng2021VectorNA, title = {Vector Neurons: A
+General Framework for SO(3)-Equivariant Networks}, author = {Congyue Deng and
+Or Litany and Yueqi Duan and Adrien Poulenard and Andrea Tagliasacchi and
+Leonidas J. Guibas}, journal = {2021 IEEE/CVF International Conference on
+Computer Vision (ICCV)}, year = {2021}, pages = {12180-12189}, url = {https://
+api.semanticscholar.org/CorpusID:233394028} } ``` ```bibtex @inproceedings
+{Kim2020TheLC, title = {The Lipschitz Constant of Self-Attention}, author =
+{Hyunjik Kim and George Papamakarios and Andriy Mnih}, booktitle =
+{International Conference on Machine Learning}, year = {2020}, url = {https://
+api.semanticscholar.org/CorpusID:219530837} } ``` ```bibtex @inproceedings
+{dao2022flashattention, title = {Flash{A}ttention: Fast and Memory-Efficient
+Exact Attention with {IO}-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and
+Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher}, booktitle = {Advances
+in Neural Information Processing Systems}, year = {2022} } ```
```

### Comparing `VN-transformer-0.0.9/VN_transformer/VN_transformer.py` & `VN-transformer-0.1.0/VN_transformer/VN_transformer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum, Tensor
 
 from einops import rearrange, repeat, reduce
 from einops.layers.torch import Rearrange, Reduce
 
+from VN_transformer.attend import Attend
+
 # helper
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
@@ -84,61 +86,65 @@
     def __init__(
         self,
         dim,
         dim_head = 64,
         heads = 8,
         dim_coor = 3,
         bias_epsilon = 0.,
+        l2_dist_attn = False,
+        flash = False,
         num_latents = None   # setting this would enable perceiver-like cross attention from latents to sequence, with the latents derived from VNWeightedPool
     ):
         super().__init__()
+        assert not (l2_dist_attn and flash), 'l2 distance attention is not compatible with flash attention'
+
         self.scale = (dim_coor * dim_head) ** -0.5
         dim_inner = dim_head * heads
         self.heads = heads
 
         self.to_q_input = None
         if exists(num_latents):
             self.to_q_input = VNWeightedPool(dim, num_pooled_tokens = num_latents, squeeze_out_pooled_dim = False)
 
         self.to_q = VNLinear(dim, dim_inner, bias_epsilon = bias_epsilon)
-        self.to_kv = VNLinear(dim, dim_inner * 2, bias_epsilon = bias_epsilon)
+        self.to_k = VNLinear(dim, dim_inner, bias_epsilon = bias_epsilon)
+        self.to_v = VNLinear(dim, dim_inner, bias_epsilon = bias_epsilon)
         self.to_out = VNLinear(dim_inner, dim, bias_epsilon = bias_epsilon)
 
+        if l2_dist_attn and not exists(num_latents):
+            # tied queries and keys for l2 distance attention, and not perceiver-like attention
+            self.to_k = self.to_q
+
+        self.attend = Attend(flash = flash, l2_dist = l2_dist_attn)
+
     def forward(self, x, mask = None):
         """
         einstein notation
         b - batch
         n - sequence
         h - heads
         d - feature dimension (channels)
         c - coordinate dimension (3 for 3d space)
         i - source sequence dimension
         j - target sequence dimension
         """
 
         c = x.shape[-1]
 
-        q_input = self.to_q_input(x) if exists(self.to_q_input) else x
-
-        q, k, v = (self.to_q(q_input), *self.to_kv(x).chunk(2, dim = -2))
-        q, k, v = map(lambda t: rearrange(t, 'b n (h d) c -> b h n d c', h = self.heads), (q, k, v))
-
-        q = q * self.scale
-
-        sim = einsum('b h i d c, b h j d c -> b h i j', q, k)
-
-        if exists(mask):
-            mask = rearrange(mask, 'b j -> b 1 1 j')
-            sim = sim.masked_fill(~mask, -torch.finfo(sim.dtype).max)
+        if exists(self.to_q_input):
+            q_input = self.to_q_input(x, mask = mask)
+        else:
+            q_input = x
 
-        attn = sim.softmax(dim = -1)
+        q, k, v = self.to_q(q_input), self.to_k(x), self.to_v(x)
+        q, k, v = map(lambda t: rearrange(t, 'b n (h d) c -> b h n (d c)', h = self.heads), (q, k, v))
 
-        out = einsum('b h i j, b h j d c -> b h i d c', attn, v)
+        out = self.attend(q, k, v, mask = mask)
 
-        out = rearrange(out, 'b h n d c -> b n (h d) c')
+        out = rearrange(out, 'b h n (d c) -> b n (h d) c', c = c)
         return self.to_out(out)
 
 def VNFeedForward(dim, mult = 4, bias_epsilon = 0.):
     dim_inner = int(dim * mult)
     return nn.Sequential(
         VNLinear(dim, dim_inner, bias_epsilon = bias_epsilon),
         VNReLU(dim_inner),
@@ -166,16 +172,25 @@
         squeeze_out_pooled_dim = True
     ):
         super().__init__()
         dim_out = default(dim_out, dim)
         self.weight = nn.Parameter(torch.randn(num_pooled_tokens, dim, dim_out))
         self.squeeze_out_pooled_dim = num_pooled_tokens == 1 and squeeze_out_pooled_dim
 
-    def forward(self, x):
-        out = einsum('b n d c, m d e -> b m e c', x, self.weight)
+    def forward(self, x, mask = None):
+        if exists(mask):
+            mask = rearrange(mask, 'b n -> b n 1 1')
+            x = x.masked_fill(~mask, 0.)
+            numer = reduce(x, 'b n d c -> b d c', 'sum')
+            denom = mask.sum(dim = 1)
+            mean_pooled = numer / denom.clamp(min = 1e-6)
+        else:
+            mean_pooled = reduce(x, 'b n d c -> b d c', 'mean')
+
+        out = einsum('b d c, m d e -> b m e c', mean_pooled, self.weight)
 
         if not self.squeeze_out_pooled_dim:
             return out
 
         out = rearrange(out, 'b 1 d c -> b d c')
         return out
 
@@ -188,25 +203,27 @@
         *,
         depth,
         dim_head = 64,
         heads = 8,
         dim_coor = 3,
         ff_mult = 4,
         final_norm = False,
-        bias_epsilon = 0.
+        bias_epsilon = 0.,
+        l2_dist_attn = False,
+        flash_attn = False
     ):
         super().__init__()
         self.dim = dim
         self.dim_coor = dim_coor
 
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
-                VNAttention(dim = dim, dim_head = dim_head, heads = heads, bias_epsilon = bias_epsilon),
+                VNAttention(dim = dim, dim_head = dim_head, heads = heads, bias_epsilon = bias_epsilon, l2_dist_attn = l2_dist_attn, flash = flash_attn),
                 VNLayerNorm(dim),
                 VNFeedForward(dim = dim, mult = ff_mult, bias_epsilon = bias_epsilon),
                 VNLayerNorm(dim)
             ]))
 
         self.norm = VNLayerNorm(dim) if final_norm else nn.Identity()
 
@@ -248,38 +265,51 @@
 
 class VNTransformer(nn.Module):
     def __init__(
         self,
         *,
         dim,
         depth,
+        num_tokens = None,
         dim_feat = None,
         dim_head = 64,
         heads = 8,
         dim_coor = 3,
         reduce_dim_out = True,
-        bias_epsilon = 0.
+        bias_epsilon = 0.,
+        l2_dist_attn = False,
+        flash_attn = False,
+        translation_equivariance = False,
+        translation_invariant = False
     ):
         super().__init__()
+        self.token_emb = nn.Embedding(num_tokens, dim) if exists(num_tokens) else None
+
         dim_feat = default(dim_feat, 0)
         self.dim_feat = dim_feat
         self.dim_coor_total = dim_coor + dim_feat
 
+        assert (int(translation_equivariance) + int(translation_invariant)) <= 1
+        self.translation_equivariance = translation_equivariance
+        self.translation_invariant = translation_invariant
+
         self.vn_proj_in = nn.Sequential(
             Rearrange('... c -> ... 1 c'),
             VNLinear(1, dim, bias_epsilon = bias_epsilon)
         )
 
         self.encoder = VNTransformerEncoder(
             dim = dim,
             depth = depth,
             dim_head = dim_head,
             heads = heads,
             bias_epsilon = bias_epsilon,
-            dim_coor = self.dim_coor_total
+            dim_coor = self.dim_coor_total,
+            l2_dist_attn = l2_dist_attn,
+            flash_attn = flash_attn
         )
 
         if reduce_dim_out:
             self.vn_proj_out = nn.Sequential(
                 VNLayerNorm(dim),
                 VNLinear(dim, 1, bias_epsilon = bias_epsilon),
                 Rearrange('... 1 c -> ... c')
@@ -288,20 +318,42 @@
             self.vn_proj_out = nn.Identity()
 
     def forward(
         self,
         coors,
         *,
         feats = None,
-        mask = None
+        mask = None,
+        return_concatted_coors_and_feats = False
     ):
+        if self.translation_equivariance or self.translation_invariant:
+            coors_mean = reduce(coors, '... c -> c', 'mean')
+            coors = coors - coors_mean
+
+        x = coors
+
         if exists(feats):
-            assert feats.ndim == 3
+            if feats.dtype == torch.long:
+                assert exists(self.token_emb), 'num_tokens must be given to the VNTransformer (to build the Embedding), if the features are to be given as indices'
+                feats = self.token_emb(feats)
+
             assert feats.shape[-1] == self.dim_feat, f'dim_feat should be set to {feats.shape[-1]}'
-            coors = torch.cat((coors, feats), dim = -1)
+            x = torch.cat((x, feats), dim = -1)
+
+        assert x.shape[-1] == self.dim_coor_total
+
+        x = self.vn_proj_in(x)
+        x = self.encoder(x, mask = mask)
+        x = self.vn_proj_out(x)
+
+        coors_out, feats_out = x[..., :3], x[..., 3:]
+
+        if self.translation_equivariance:
+            coors_out = coors_out + coors_mean
+
+        if not exists(feats):
+            return coors_out
 
-        assert coors.shape[-1] == self.dim_coor_total
+        if return_concatted_coors_and_feats:
+            return torch.cat((coors_out, feats_out), dim = -1)
 
-        coors = self.vn_proj_in(coors)
-        coors = self.encoder(coors, mask = mask)
-        coors = self.vn_proj_out(coors)
-        return coors
+        return coors_out, feats_out
```

### Comparing `VN-transformer-0.0.9/VN_transformer.egg-info/PKG-INFO` & `VN-transformer-0.1.0/VN_transformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.9
+Version: 0.1.0
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.9/setup.py` & `VN-transformer-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'VN-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.9',
+  version = '0.1.0',
   license='MIT',
   description = 'Vector Neuron Transformer (VN-Transformer)',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/VN-transformer',
   keywords = [
```

