# Comparing `tmp/rotograd-0.1.5.2.tar.gz` & `tmp/rotograd-0.1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotograd-0.1.5.2.tar", last modified: Tue Mar  1 12:17:45 2022, max compression
+gzip compressed data, was "rotograd-0.1.6.0.tar", last modified: Tue Aug  1 15:55:48 2023, max compression
```

## Comparing `rotograd-0.1.5.2.tar` & `rotograd-0.1.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 12:17:45.435683 rotograd-0.1.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-03-01 12:17:33.000000 rotograd-0.1.5.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     4475 2022-03-01 12:17:45.435683 rotograd-0.1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3466 2022-03-01 12:17:33.000000 rotograd-0.1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 12:17:45.435683 rotograd-0.1.5.2/rotograd/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-03-01 12:17:33.000000 rotograd-0.1.5.2/rotograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17779 2022-03-01 12:17:33.000000 rotograd-0.1.5.2/rotograd/rotograd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 12:17:45.435683 rotograd-0.1.5.2/rotograd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4475 2022-03-01 12:17:45.000000 rotograd-0.1.5.2/rotograd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-03-01 12:17:45.000000 rotograd-0.1.5.2/rotograd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-01 12:17:45.000000 rotograd-0.1.5.2/rotograd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-03-01 12:17:45.000000 rotograd-0.1.5.2/rotograd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-03-01 12:17:45.000000 rotograd-0.1.5.2/rotograd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-01 12:17:45.435683 rotograd-0.1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-03-01 12:17:33.000000 rotograd-0.1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:55:48.282979 rotograd-0.1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-01 15:55:37.000000 rotograd-0.1.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-08-01 15:55:48.282979 rotograd-0.1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-01 15:55:37.000000 rotograd-0.1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:55:48.282979 rotograd-0.1.6.0/rotograd/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-01 15:55:37.000000 rotograd-0.1.6.0/rotograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20811 2023-08-01 15:55:37.000000 rotograd-0.1.6.0/rotograd/rotograd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:55:48.282979 rotograd-0.1.6.0/rotograd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-08-01 15:55:48.000000 rotograd-0.1.6.0/rotograd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-01 15:55:48.000000 rotograd-0.1.6.0/rotograd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:55:48.000000 rotograd-0.1.6.0/rotograd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-01 15:55:48.000000 rotograd-0.1.6.0/rotograd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 15:55:48.000000 rotograd-0.1.6.0/rotograd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 15:55:48.282979 rotograd-0.1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-01 15:55:37.000000 rotograd-0.1.6.0/setup.py
```

### Comparing `rotograd-0.1.5.2/LICENSE.md` & `rotograd-0.1.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rotograd-0.1.5.2/PKG-INFO` & `rotograd-0.1.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: rotograd
-Version: 0.1.5.2
+Version: 0.1.6.0
 Summary: RotoGrad: Gradient Homogenization in Multitask Learning in Pytorch
 Home-page: https://github.com/adrianjav/rotograd
 Author: Adrián Javaloy
 Author-email: adrian.javaloy@gmail.com
 License: MIT
 Keywords: Multitask Learning,Gradient Alignment,Gradient Interference,Negative Transfer,Pytorch,Positive Transfer,Gradient Conflict
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -64,39 +63,35 @@
 where you can recover the backbone and i-th head simply calling `model.backbone` and `model.heads[i]`. Even
 more, you can obtain the end-to-end model for a single task (that is, backbone + head), by typing `model[i]`.
 
 As discussed in the paper, it is advisable to have a smaller learning rate for the parameters of RotoGrad
 and GradNorm. This is as simple as doing:
 
 ```python
-optim_model = nn.Adam({'params': m.parameters() for m in [backbone, head1, head2]}, lr=learning_rate_model)
-optim_rotograd = nn.Adam({'params': model.parameters()}, lr=learning_rate_rotograd)
+optimizer = nn.Adam(
+    [{'params': m.parameters()} for m in [backbone, head1, head2]] +
+    [{'params': model.parameters(), 'lr': learning_rate_rotograd}],
+    lr=learning_rate_model)
 ```
 
 Finally, we can train the model on all tasks using a simple step function:
 ```python
 import rotograd
 
 def step(x, y1, y2):
     model.train()
     
-    optim_model.zero_grad()
-    optim_rotograd.zero_grad()
+    optimizer.zero_grad()
 
     with rotograd.cached():  # Speeds-up computations by caching Rotograd's parameters
         pred1, pred2 = model(x)
-        
-        loss1 = loss_task1(pred1, y1)
-        loss2 = loss_task2(pred2, y2)
-        
+        loss1, loss2 = loss_task1(pred1, y1), loss_task2(pred2, y2)
         model.backward([loss1, loss2])
+    optimizer.step()
     
-    optim_model.step()
-    optim_rotograd.step()
-        
     return loss1, loss2
 ```
 
 ## Example
 
 You can find a working example in the folder `example`. However, it requires some other dependencies to run (e.g., 
 ignite and seaborn). The example shows how to use RotoGrad on one of the regression problems from the manuscript.
@@ -112,9 +107,7 @@
    title={RotoGrad: Gradient Homogenization in Multitask Learning},
    author={Adri{\'a}n Javaloy and Isabel Valera},
    booktitle={International Conference on Learning Representations},
    year={2022},
    url={https://openreview.net/forum?id=T8wHz4rnuGL}
 }
 ```
-
-
```

### Comparing `rotograd-0.1.5.2/README.md` & `rotograd-0.1.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -39,39 +39,35 @@
 where you can recover the backbone and i-th head simply calling `model.backbone` and `model.heads[i]`. Even
 more, you can obtain the end-to-end model for a single task (that is, backbone + head), by typing `model[i]`.
 
 As discussed in the paper, it is advisable to have a smaller learning rate for the parameters of RotoGrad
 and GradNorm. This is as simple as doing:
 
 ```python
-optim_model = nn.Adam({'params': m.parameters() for m in [backbone, head1, head2]}, lr=learning_rate_model)
-optim_rotograd = nn.Adam({'params': model.parameters()}, lr=learning_rate_rotograd)
+optimizer = nn.Adam(
+    [{'params': m.parameters()} for m in [backbone, head1, head2]] +
+    [{'params': model.parameters(), 'lr': learning_rate_rotograd}],
+    lr=learning_rate_model)
 ```
 
 Finally, we can train the model on all tasks using a simple step function:
 ```python
 import rotograd
 
 def step(x, y1, y2):
     model.train()
     
-    optim_model.zero_grad()
-    optim_rotograd.zero_grad()
+    optimizer.zero_grad()
 
     with rotograd.cached():  # Speeds-up computations by caching Rotograd's parameters
         pred1, pred2 = model(x)
-        
-        loss1 = loss_task1(pred1, y1)
-        loss2 = loss_task2(pred2, y2)
-        
+        loss1, loss2 = loss_task1(pred1, y1), loss_task2(pred2, y2)
         model.backward([loss1, loss2])
+    optimizer.step()
     
-    optim_model.step()
-    optim_rotograd.step()
-        
     return loss1, loss2
 ```
 
 ## Example
 
 You can find a working example in the folder `example`. However, it requires some other dependencies to run (e.g., 
 ignite and seaborn). The example shows how to use RotoGrad on one of the regression problems from the manuscript.
```

### Comparing `rotograd-0.1.5.2/rotograd/rotograd.py` & `rotograd-0.1.6.0/rotograd/rotograd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Sequence, List, Any, Optional
+from typing import Sequence, Union, Any, Optional
+from functools import reduce
 
 import torch
 import torch.nn as nn
 
 from geotorch import orthogonal
 from geotorch.parametrize import cached
 
@@ -97,20 +98,20 @@
 
         for h in self.heads:
             for param in h.parameters(recurse=recurse):
                 yield param
 
 
 def rotate(points, rotation, total_size):
-    if total_size != points.size(-1):
-        points_lo, points_hi = points[:, :rotation.size(1)], points[:, rotation.size(1):]
-        point_lo = torch.einsum('ij,bj->bi', rotation, points_lo)
-        return torch.cat((point_lo, points_hi), dim=-1)
+    if total_size != points.size(-2):
+        points_lo, points_hi = points[..., :rotation.size(1), :], points[..., rotation.size(1):, :]
+        point_lo = torch.einsum('ij,...jk->...ik', rotation, points_lo)
+        return torch.cat((point_lo, points_hi), dim=-2)
     else:
-        return torch.einsum('ij,bj->bi', rotation, points)
+        return torch.einsum('ij,...jk->...ik', rotation, points)
 
 
 def rotate_back(points, rotation, total_size):
     return rotate(points, rotation.t(), total_size)
 
 
 class RotateModule(nn.Module):
@@ -120,55 +121,74 @@
         self.parent = [parent]  # Dirty trick to not register parameters
         self.item = item
 
     def hook(self, g):
         self.p.grads[self.item] = g.clone()
 
     @property
-    def p(self):
+    def p(self) -> 'RotateOnly':
         return self.parent[0]
 
     @property
     def R(self):
         return self.p.rotation[self.item]
 
     @property
     def weight(self):
         return self.p.weight[self.item] if hasattr(self.p, 'weight') else 1.
 
     def rotate(self, z):
-        return rotate(z, self.R, self.p.latent_size)
+        dim_post = -len(self.p.post_shape)
+        dim_rot = -len(self.p.rotation_shape)
+        og_shape = z.shape
+        if dim_post == 0:
+            z = z.unsqueeze(dim=-1)
+            dim_post = -1
+
+        z = z.flatten(start_dim=dim_post)
+        z = z.flatten(start_dim=dim_rot - 1, end_dim=-2)
+
+        return rotate(z, self.R.detach(), self.p.rotation_size).view(og_shape)
 
     def rotate_back(self, z):
-        return rotate_back(z, self.R, self.p.latent_size)
+        return rotate_back(z, self.R, self.p.rotation_size)
 
     def forward(self, z):
-        R = self.R.clone().detach()
-        new_z = rotate(z, R, self.p.latent_size)
+        new_z = self.rotate(z)
         if self.p.training:
             new_z.register_hook(self.hook)
 
         return new_z
 
 
 class RotateOnly(nn.Module):
     r"""
     Implementation of the rotating part of RotoGrad as described in the original paper. [1]_
 
+    The module takes as input a vector of shape ... x rotation_shape x
+
     Parameters
     ----------
     backbone
         Shared module.
     heads
         Task-specific modules.
-    latent_size
-        Size of the shared representation, that is, size of the output of backbone.Z
+    rotation_shape
+        Shape of the shared representation to be rotated which, usually, is just the size of the backbone's output.
+        Passing a shape is useful, for example, if you want to rotate an image with shape width x height.
+    post_shape : optional, default=()
+        Shape of the shared representation following the part to be rotated (if any). This part will be kept as it is.
+        This is useful, for example, if you want to rotate only the channels of an image.
     normalize_losses : optional, default=False
         Whether to use this normalized losses to back-propagate through the task-specific parameters as well.
-
+    burn_in_period : optional, default=20
+        When back-propagating towards the shared parameters, *each task loss is normalized dividing by its initial
+        value*, :math:`{L_k(t)}/{L_k(t_0 = 0)}`. This parameter sets a number of iterations after which the denominator
+        will be replaced by the value of the loss at that iteration, that is, :math:`t_0 = burn\_in\_period`.
+        This is done to overcome problems with losses quickly changing in the first iterations.
 
     Attributes
     ----------
     num_tasks
         Number of tasks/heads of the module.
     backbone
         Shared module.
@@ -185,33 +205,39 @@
 
     """
     num_tasks: int
     backbone: nn.Module
     heads: Sequence[nn.Module]
     rep: Optional[torch.Tensor]
 
-    def __init__(self, backbone: nn.Module, heads: List[nn.Module], latent_size: int, *args,
-                 burn_in_period: int = 20, normalize_losses: bool = False):
+    def __init__(self, backbone: nn.Module, heads: Sequence[nn.Module], rotation_shape: Union[int, torch.Size], *args,
+                 post_shape: torch.Size = (), normalize_losses: bool = False, burn_in_period: int = 20):
         super(RotateOnly, self).__init__()
         num_tasks = len(heads)
+        if isinstance(rotation_shape, int):
+            rotation_shape = torch.Size((rotation_shape,))
+        assert len(rotation_shape) > 0
+        rotation_size = reduce(int.__mul__, rotation_shape)
 
         for i in range(num_tasks):
             heads[i] = nn.Sequential(RotateModule(self, i), heads[i])
 
         self._backbone = [backbone]
         self.heads = heads
 
         # Parameterize rotations so we can run unconstrained optimization
         for i in range(num_tasks):
-            self.register_parameter(f'rotation_{i}', nn.Parameter(torch.eye(latent_size), requires_grad=True))
+            self.register_parameter(f'rotation_{i}', nn.Parameter(torch.eye(rotation_size), requires_grad=True))
             orthogonal(self, f'rotation_{i}', triv='expm')  # uses exponential map (alternative: cayley)
 
         # Parameters
         self.num_tasks = num_tasks
-        self.latent_size = latent_size
+        self.rotation_shape = rotation_shape
+        self.rotation_size = rotation_size
+        self.post_shape = post_shape
         self.burn_in_period = burn_in_period
         self.normalize_losses = normalize_losses
 
         self.rep = None
         self.grads = [None for _ in range(num_tasks)]
         self.original_grads = [None for _ in range(num_tasks)]
         self.losses = [None for _ in range(num_tasks)]
@@ -338,29 +364,38 @@
             else:
                 backbone_loss.backward(retain_graph=True)
 
         self.rep.backward(self._rep_grad())
 
     def _rep_grad(self):
         old_grads = self.original_grads  # these grads are already rotated, we have to recover the originals
-        # with torch.no_grad():
-        #     grads = [rotate(g, R) for g, R in zip(grads, self.rotation)]
-        #
         grads = self.grads
 
         # Compute the reference vector
         mean_grad = sum([g for g in old_grads]).detach().clone() / len(grads)
         mean_norm = mean_grad.norm(p=2)
         old_grads2 = [g * divide(mean_norm, g.norm(p=2)) for g in old_grads]
         mean_grad = sum([g for g in old_grads2]).detach().clone() / len(grads)
 
+        dim_post = -len(self.post_shape)
+        dim_rot = -len(self.rotation_shape)
+        og_shape = mean_grad.shape
+        if dim_post == 0:
+            mean_grad = mean_grad.unsqueeze(dim=-1)
+            dim_post = -1
+
+        mean_grad = mean_grad.flatten(start_dim=dim_post)
+        mean_grad = mean_grad.flatten(start_dim=dim_rot - 1, end_dim=-2)
+
         for i, grad in enumerate(grads):
             R = self.rotation[i]
-            loss_rotograd = rotate(mean_grad, R, self.latent_size) - grad
-            loss_rotograd = torch.einsum('bi,bi->b', loss_rotograd, loss_rotograd)
+            loss_rotograd = rotate(mean_grad, R, self.rotation_size).view(og_shape) - grad
+            loss_rotograd = loss_rotograd.flatten(start_dim=dim_post)
+            loss_rotograd = loss_rotograd.flatten(start_dim=dim_rot - 1, end_dim=-2)
+            loss_rotograd = torch.einsum('...ij,...ij->...', loss_rotograd, loss_rotograd)
             loss_rotograd.mean().backward()
 
         return sum(old_grads)
 
     def mtl_parameters(self, recurse=True):
         return self.parameters(recurse=recurse)
 
@@ -379,51 +414,55 @@
 
     Parameters
     ----------
     backbone
         Shared module.
     heads
         Task-specific modules.
-    latent_size
-        Size of the shared representation, that is, size of the output of backbone.Z
+    rotation_shape
+        Shape of the shared representation to be rotated which, usually, is just the size of the backbone's output.
+        Passing a shape is useful, for example, if you want to rotate an image with shape width x height.
+    post_shape : optional, default=()
+        Shape of the shared representation following the part to be rotated (if any). This part will be kept as it is.
+        This is useful, for example, if you want to rotate only the channels of an image.
     burn_in_period : optional, default=20
         When back-propagating towards the shared parameters, *each task loss is normalized dividing by its initial
         value*, :math:`{L_k(t)}/{L_k(t_0 = 0)}`. This parameter sets a number of iterations after which the denominator
         will be replaced by the value of the loss at that iteration, that is, :math:`t_0 = burn\_in\_period`.
         This is done to overcome problems with losses quickly changing in the first iterations.
     normalize_losses : optional, default=False
         Whether to use this normalized losses to back-propagate through the task-specific parameters as well.
 
-
     Attributes
     ----------
     num_tasks
         Number of tasks/heads of the module.
     backbone
         Shared module.
     heads
         Sequence with the (rotated) task-specific heads.
     rep
-        Current output of the backbone (after calling forward during training).
+        Current output of the backbone (aft1er calling forward during training).
 
 
     References
     ----------
     .. [1] Javaloy, Adrián, and Isabel Valera. "RotoGrad: Gradient Homogenization in Multitask Learning."
         International Conference on Learning Representations (2022).
 
     """
     num_tasks: int
     backbone: nn.Module
     heads: Sequence[nn.Module]
     rep: torch.Tensor
 
-    def __init__(self, backbone: nn.Module, heads: Sequence[nn.Module], latent_size: int, *args,
-                 burn_in_period: int = 20, normalize_losses: bool = False):
-        super().__init__(backbone, heads, latent_size, burn_in_period, *args, normalize_losses=normalize_losses)
+    def __init__(self, backbone: nn.Module, heads: Sequence[nn.Module],  rotation_shape: Union[int, torch.Size], *args,
+                 post_shape: torch.Size = (), normalize_losses: bool = False, burn_in_period: int = 20):
+        super().__init__(backbone, heads, rotation_shape, *args,
+                         post_shape=post_shape, burn_in_period=burn_in_period, normalize_losses=normalize_losses)
 
         self.initial_grads = None
         self.counter = 0
 
     def _rep_grad(self):
         super()._rep_grad()
 
@@ -447,26 +486,30 @@
 
     Parameters
     ----------
     backbone
         Shared module.
     heads
         Task-specific modules.
-    latent_size
-        Size of the shared representation, that is, size of the output of backbone.
+    rotation_shape
+        Shape of the shared representation to be rotated which, usually, is just the size of the backbone's output.
+        Passing a shape is useful, for example, if you want to rotate an image with shape width x height.
     alpha
         :math:`\alpha` hyper-parameter as described in GradNorm, [2]_ used to compute the reference direction.
+    post_shape : optional, default=()
+        Shape of the shared representation following the part to be rotated (if any). This part will be kept as it is.
+        This is useful, for example, if you want to rotate only the channels of an image.
     burn_in_period : optional, default=20
         When back-propagating towards the shared parameters, *each task loss is normalized dividing by its initial
         value*, :math:`{L_k(t)}/{L_k(t_0 = 0)}`. This parameter sets a number of iterations after which the denominator
         will be replaced by the value of the loss at that iteration, that is, :math:`t_0 = burn\_in\_period`.
         This is done to overcome problems with losses quickly changing in the first iterations.
     normalize_losses : optional, default=False
         Whether to use this normalized losses to back-propagate through the task-specific parameters as well.
-
+    TODO
 
     Attributes
     ----------
     num_tasks
         Number of tasks/heads of the module.
     backbone
         Shared module.
@@ -482,18 +525,18 @@
         International Conference on Learning Representations (2022).
 
     .. [2] Chen, Zhao, et al. "Gradnorm: Gradient normalization for adaptive loss balancing in deep multitask networks."
         International Conference on Machine Learning. PMLR, 2018.
 
     """
 
-    def __init__(self, backbone: nn.Module, heads: Sequence[nn.Module], latent_size: int, *args, alpha: float,
-                 burn_in_period: int = 20, normalize_losses: bool = False):
-        super().__init__(backbone, heads, latent_size, *args, burn_in_period=burn_in_period,
-                         normalize_losses=normalize_losses)
+    def __init__(self, backbone: nn.Module, heads: Sequence[nn.Module],  rotation_shape: Union[int, torch.Size], *args,
+                 alpha: float, post_shape: torch.Size = (), normalize_losses: bool = False, burn_in_period: int = 20):
+        super().__init__(backbone, heads, rotation_shape, *args,
+                         post_shape=post_shape, burn_in_period=burn_in_period, normalize_losses=normalize_losses)
         self.alpha = alpha
         self.weight_ = nn.ParameterList([nn.Parameter(torch.ones([]), requires_grad=True) for _ in range(len(heads))])
 
     @property
     def weight(self) -> Sequence[torch.Tensor]:
         r"""List of task weights, one per task. These are trainable, make sure to call `detach()`."""
         ws = [w.exp() + 1e-15 for w in self.weight_]
```

### Comparing `rotograd-0.1.5.2/rotograd.egg-info/PKG-INFO` & `rotograd-0.1.6.0/rotograd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: rotograd
-Version: 0.1.5.2
+Version: 0.1.6.0
 Summary: RotoGrad: Gradient Homogenization in Multitask Learning in Pytorch
 Home-page: https://github.com/adrianjav/rotograd
 Author: Adrián Javaloy
 Author-email: adrian.javaloy@gmail.com
 License: MIT
 Keywords: Multitask Learning,Gradient Alignment,Gradient Interference,Negative Transfer,Pytorch,Positive Transfer,Gradient Conflict
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -64,39 +63,35 @@
 where you can recover the backbone and i-th head simply calling `model.backbone` and `model.heads[i]`. Even
 more, you can obtain the end-to-end model for a single task (that is, backbone + head), by typing `model[i]`.
 
 As discussed in the paper, it is advisable to have a smaller learning rate for the parameters of RotoGrad
 and GradNorm. This is as simple as doing:
 
 ```python
-optim_model = nn.Adam({'params': m.parameters() for m in [backbone, head1, head2]}, lr=learning_rate_model)
-optim_rotograd = nn.Adam({'params': model.parameters()}, lr=learning_rate_rotograd)
+optimizer = nn.Adam(
+    [{'params': m.parameters()} for m in [backbone, head1, head2]] +
+    [{'params': model.parameters(), 'lr': learning_rate_rotograd}],
+    lr=learning_rate_model)
 ```
 
 Finally, we can train the model on all tasks using a simple step function:
 ```python
 import rotograd
 
 def step(x, y1, y2):
     model.train()
     
-    optim_model.zero_grad()
-    optim_rotograd.zero_grad()
+    optimizer.zero_grad()
 
     with rotograd.cached():  # Speeds-up computations by caching Rotograd's parameters
         pred1, pred2 = model(x)
-        
-        loss1 = loss_task1(pred1, y1)
-        loss2 = loss_task2(pred2, y2)
-        
+        loss1, loss2 = loss_task1(pred1, y1), loss_task2(pred2, y2)
         model.backward([loss1, loss2])
+    optimizer.step()
     
-    optim_model.step()
-    optim_rotograd.step()
-        
     return loss1, loss2
 ```
 
 ## Example
 
 You can find a working example in the folder `example`. However, it requires some other dependencies to run (e.g., 
 ignite and seaborn). The example shows how to use RotoGrad on one of the regression problems from the manuscript.
@@ -112,9 +107,7 @@
    title={RotoGrad: Gradient Homogenization in Multitask Learning},
    author={Adri{\'a}n Javaloy and Isabel Valera},
    booktitle={International Conference on Learning Representations},
    year={2022},
    url={https://openreview.net/forum?id=T8wHz4rnuGL}
 }
 ```
-
-
```

### Comparing `rotograd-0.1.5.2/setup.py` & `rotograd-0.1.6.0/setup.py`

 * *Files identical despite different names*

