# Comparing `tmp/sihl-0.0.3.dev3.tar.gz` & `tmp/sihl-0.0.3.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sihl-0.0.3.dev3.tar", max compression
+gzip compressed data, was "sihl-0.0.3.dev4.tar", max compression
```

## Comparing `sihl-0.0.3.dev3.tar` & `sihl-0.0.3.dev4.tar`

### file list

```diff
@@ -1,15 +1,20 @@
--rw-r--r--   0        0        0     1063 2023-07-12 10:41:30.903222 sihl-0.0.3.dev3/LICENSE
--rw-r--r--   0        0        0      894 2023-07-12 10:41:30.903222 sihl-0.0.3.dev3/README.md
--rw-r--r--   0        0        0     1545 2023-07-12 10:41:47.839418 sihl-0.0.3.dev3/pyproject.toml
--rw-r--r--   0        0        0      288 2023-07-12 10:41:30.907222 sihl-0.0.3.dev3/src/sihl/__init__.py
--rw-r--r--   0        0        0   402648 2023-07-12 10:41:30.907222 sihl-0.0.3.dev3/src/sihl/heads/NotoSansMono-Bold.ttf
--rw-r--r--   0        0        0      233 2023-07-12 10:41:30.911222 sihl-0.0.3.dev3/src/sihl/heads/__init__.py
--rw-r--r--   0        0        0     3147 2023-07-12 10:41:47.839418 sihl-0.0.3.dev3/src/sihl/heads/binary_classification.py
--rw-r--r--   0        0        0     3828 2023-07-12 10:41:47.839418 sihl-0.0.3.dev3/src/sihl/heads/multiclass_classification.py
--rw-r--r--   0        0        0     4684 2023-07-12 10:41:47.839418 sihl-0.0.3.dev3/src/sihl/heads/multilabel_classification.py
--rw-r--r--   0        0        0        0 2023-07-12 10:41:30.911222 sihl-0.0.3.dev3/src/sihl/layers/__init__.py
--rw-r--r--   0        0        0     4573 2023-07-12 10:41:30.911222 sihl-0.0.3.dev3/src/sihl/lightning_module.py
--rw-r--r--   0        0        0      549 2023-07-12 10:41:30.911222 sihl-0.0.3.dev3/src/sihl/sihl_model.py
--rw-r--r--   0        0        0     2797 2023-07-12 10:41:30.911222 sihl-0.0.3.dev3/src/sihl/timm_backbone.py
--rw-r--r--   0        0        0     6460 2023-07-12 10:41:30.911222 sihl-0.0.3.dev3/src/sihl/torchvision_backbone.py
--rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-01 15:49:47.829813 sihl-0.0.3.dev4/LICENSE
+-rw-r--r--   0        0        0      894 2023-08-01 15:49:47.829813 sihl-0.0.3.dev4/README.md
+-rw-r--r--   0        0        0     1568 2023-08-01 15:50:01.426070 sihl-0.0.3.dev4/pyproject.toml
+-rw-r--r--   0        0        0   402648 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/NotoSansMono-Bold.ttf
+-rw-r--r--   0        0        0      448 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/__init__.py
+-rw-r--r--   0        0        0      289 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/heads/__init__.py
+-rw-r--r--   0        0        0     3202 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/heads/binary_classification.py
+-rw-r--r--   0        0        0     3884 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/heads/multiclass_classification.py
+-rw-r--r--   0        0        0     4748 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/heads/multilabel_classification.py
+-rw-r--r--   0        0        0    14319 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/heads/object_detection.py
+-rw-r--r--   0        0        0      189 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/layers/__init__.py
+-rw-r--r--   0        0        0     1553 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/layers/convblocks.py
+-rw-r--r--   0        0        0     2711 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/layers/fpn.py
+-rw-r--r--   0        0        0      514 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/layers/scalers.py
+-rw-r--r--   0        0        0     5215 2023-08-01 15:50:01.430070 sihl-0.0.3.dev4/src/sihl/lightning_module.py
+-rw-r--r--   0        0        0      549 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/sihl_model.py
+-rw-r--r--   0        0        0     2797 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/timm_backbone.py
+-rw-r--r--   0        0        0     6509 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/torchvision_backbone.py
+-rw-r--r--   0        0        0     1740 2023-08-01 15:49:47.833814 sihl-0.0.3.dev4/src/sihl/utils.py
+-rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev4/PKG-INFO
```

### Comparing `sihl-0.0.3.dev3/LICENSE` & `sihl-0.0.3.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev3/README.md` & `sihl-0.0.3.dev4/README.md`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev3/pyproject.toml` & `sihl-0.0.3.dev4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sihl"
-version = "0.0.3-dev3"
+version = "0.0.3-dev4"
 description = "Simple Image Heads and Layers"
 authors = ["jonregef <jon.regef@pm.me>"]
 readme = "README.md"
 license = "MIT"
 # homepage = "https://github.com/sihlAI/sihl"
 # repository = "https://github.com/sihlAI/sihl"
 
@@ -26,14 +26,15 @@
 isort = "^5.12.0"
 pyupgrade = "^3.3.2"
 kaggle = "^1.5.13"
 torchinfo = "^1.7.2"
 lightning = "^2.0.2"
 tensorboard = "^2.13.0"
 types-pyyaml = "^6.0.12.10"
+pycocotools = "^2.0.6"
 
 [tool.poetry.extras]
 lightning = ["lightning"]
 timm = ["timm"]
 all = ["lightning", "timm"]
 
 [build-system]
```

### Comparing `sihl-0.0.3.dev3/src/sihl/heads/NotoSansMono-Bold.ttf` & `sihl-0.0.3.dev4/src/sihl/NotoSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev3/src/sihl/heads/binary_classification.py` & `sihl-0.0.3.dev4/src/sihl/heads/binary_classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,29 +26,29 @@
     def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:
         scores = torch.sigmoid(self.net(inputs[self.level])).squeeze(-1)
         return scores, scores > 0.5
 
     def training_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        logits = self.net(inputs[self.level]).squeeze(-1)
+        logits = self.net(inputs[self.level]).squeeze(-1).float()
         labels = labels.to(logits.dtype).to(logits.device)
         loss = torch.nn.functional.binary_cross_entropy_with_logits(logits, labels)
         return loss, {}
 
     def on_validation_start(self) -> None:
         self.accuracy_computer = torchmetrics.classification.BinaryAccuracy()
         self.precision_computer = torchmetrics.classification.BinaryPrecision()
         self.recall_computer = torchmetrics.classification.BinaryRecall()
 
     def validation_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
         input = inputs[self.level]
-        logits = self.net(input).squeeze(-1)
+        logits = self.net(input).squeeze(-1).float()
         labels = labels.to(logits.dtype).to(logits.device)
         loss = torch.nn.functional.binary_cross_entropy_with_logits(logits, labels)
         self.accuracy_computer.to(input.device).update(logits, labels)
         self.precision_computer.to(input.device).update(logits, labels)
         self.recall_computer.to(input.device).update(logits, labels)
         return loss, {}
 
@@ -58,21 +58,21 @@
             "precision": self.precision_computer.compute().item(),
             "recall": self.recall_computer.compute().item(),
         }
 
     def visualize(self, inputs: list[Tensor], labels: Tensor) -> list[Tensor]:
         scores, classes = self.forward(inputs)
         visualizations: list[Tensor] = []
-        with as_file(files(__package__) / "NotoSansMono-Bold.ttf") as font:
+        with as_file(files(__package__).parent / "NotoSansMono-Bold.ttf") as font:
             for batch, image in enumerate(inputs[0]):
                 visualizations.append(
                     draw_bounding_boxes(
                         (image * 255).to(torch.uint8),
                         torch.zeros((1, 4)),
-                        [self.question + (" Yes" if classes[batch] else " No")],
+                        [self.question + "\n" + ("Yes" if classes[batch] else "No")],
                         colors="green" if classes[batch] == labels[batch] else "red",
                         width=0,
                         font=str(font),
-                        font_size=15,
+                        font_size=max(10, image.shape[1] // 10),
                     )
                 )
         return visualizations
```

### Comparing `sihl-0.0.3.dev3/src/sihl/heads/multiclass_classification.py` & `sihl-0.0.3.dev4/src/sihl/heads/multiclass_classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         class_names: tuple[str, ...] | None = None,
         label_weights: tuple[float, ...] | None = None,
         label_smoothing: float = 0.0,
     ) -> None:
         super().__init__()
         self.num_classes = num_classes
         self.level = level
-        self.class_names = class_names or tuple(map(str, range(num_classes)))
+        self.class_names = class_names or tuple(str(_) for _ in range(num_classes))
         self.label_weights = torch.tensor(label_weights) if label_weights else None
         self.label_smoothing = label_smoothing
         self.net = nn.Sequential(
             nn.AdaptiveAvgPool2d(1),
             nn.Flatten(),
             nn.Linear(in_channels[self.level], num_classes),
         )
@@ -43,15 +43,15 @@
             torch.nn.functional.softmax(self.net(inputs[self.level]), dim=1), dim=1
         )
         return scores, classes
 
     def training_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        logits = self.net(inputs[self.level])
+        logits = self.net(inputs[self.level]).float()
         loss = torch.nn.functional.cross_entropy(
             logits,
             labels.to(logits.device),
             weight=self.label_weights,
             label_smoothing=self.label_smoothing,
         )
         return loss, {}
@@ -61,15 +61,15 @@
         self.precision_computer = MulticlassPrecision(num_classes=self.num_classes)
         self.recall_computer = MulticlassRecall(num_classes=self.num_classes)
 
     def validation_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
         input = inputs[self.level]
-        logits = self.net(input)
+        logits = self.net(input).float()
         labels = labels.to(logits.device)
         loss = torch.nn.functional.cross_entropy(
             logits,
             labels,
             weight=self.label_weights,
             label_smoothing=self.label_smoothing,
         )
@@ -84,21 +84,21 @@
             "precision": self.precision_computer.compute().item(),
             "recall": self.recall_computer.compute().item(),
         }
 
     def visualize(self, inputs: list[Tensor], labels: Tensor) -> list[Tensor]:
         scores, classes = self.forward(inputs)
         visualizations: list[Tensor] = []
-        with as_file(files(__package__) / "NotoSansMono-Bold.ttf") as font:
+        with as_file(files(__package__).parent / "NotoSansMono-Bold.ttf") as font:
             for batch, image in enumerate(inputs[0]):
                 visualizations.append(
                     draw_bounding_boxes(
                         (image * 255).to(torch.uint8),
                         torch.zeros((1, 4)),
                         [self.class_names[classes[batch]]],
                         colors="green" if classes[batch] == labels[batch] else "red",
                         width=0,
                         font=str(font),
-                        font_size=15,
+                        font_size=max(10, image.shape[1] // 10),
                     )
                 )
         return visualizations
```

### Comparing `sihl-0.0.3.dev3/src/sihl/heads/multilabel_classification.py` & `sihl-0.0.3.dev4/src/sihl/heads/multilabel_classification.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         level: int = -1,
         class_names: tuple[str, ...] | None = None,
         label_weights: list[float] | None = None,
     ) -> None:
         super().__init__()
         self.num_classes = num_classes
         self.level = level
-        self.class_names = class_names or tuple(map(str, range(num_classes)))
+        self.class_names = class_names or tuple(str(_) for _ in range(num_classes))
         self.label_weights = torch.tensor(label_weights) if label_weights else None
         self.net = nn.Sequential(
             nn.AdaptiveAvgPool2d(1),
             nn.Flatten(),
             nn.Linear(in_channels[self.level], num_classes),
         )
 
@@ -41,30 +41,30 @@
             torch.sigmoid(self.net(inputs[self.level])), descending=True
         )
         return scores, classes
 
     def training_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        logits = self.net(inputs[self.level])
+        logits = self.net(inputs[self.level]).float()
         loss = torch.nn.functional.binary_cross_entropy_with_logits(
             logits, labels.to(logits.device), pos_weight=self.label_weights
         )
         return loss, {}
 
     def on_validation_start(self) -> None:
         self.accuracy_computer = MultilabelAccuracy(num_labels=self.num_classes)
         self.precision_computer = MultilabelPrecision(num_labels=self.num_classes)
         self.recall_computer = MultilabelRecall(num_labels=self.num_classes)
 
     def validation_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
         input = inputs[self.level]
-        logits = self.net(input)
+        logits = self.net(input).float()
         labels = labels.to(logits.device)
         loss = torch.nn.functional.binary_cross_entropy_with_logits(
             logits, labels, pos_weight=self.label_weights
         )
         self.accuracy_computer.to(input.device).update(logits, labels)
         self.precision_computer.to(input.device).update(logits, labels)
         self.recall_computer.to(input.device).update(logits, labels)
@@ -76,17 +76,17 @@
             "precision": self.precision_computer.compute().item(),
             "recall": self.recall_computer.compute().item(),
         }
 
     def visualize(self, inputs: list[Tensor], labels: Tensor) -> list[Tensor]:
         scores, classes = self.forward(inputs)
         visualizations: list[Tensor] = []
-        FONT_SIZE = 20
-        with as_file(files(__package__) / "NotoSansMono-Bold.ttf") as font:
+        with as_file(files(__package__).parent / "NotoSansMono-Bold.ttf") as font:
             for batch, image in enumerate(inputs[0]):
+                font_size = max(10, image.shape[1] // 10)
                 predictions = sorted(
                     self.class_names[class_idx]
                     for score, class_idx in zip(scores[batch], classes[batch])
                     if score > 0.5
                 )
                 targets = sorted(
                     self.class_names[class_idx]
@@ -99,25 +99,25 @@
                     img = draw_bounding_boxes(
                         img,
                         torch.tensor([[0, offset, 0, offset]]),
                         [target],
                         colors="green" if target in predictions else "yellow",
                         width=0,
                         font=str(font),
-                        font_size=FONT_SIZE,
+                        font_size=font_size,
                     )
-                    offset += FONT_SIZE
+                    offset += font_size
                 for pred in predictions:
                     if pred in targets:
                         continue
                     img = draw_bounding_boxes(
                         img,
                         torch.tensor([[0, offset, 0, offset]]),
                         [pred],
                         colors="red",
                         width=0,
                         font=str(font),
-                        font_size=FONT_SIZE,
+                        font_size=font_size,
                     )
-                    offset += FONT_SIZE
+                    offset += font_size
                 visualizations.append(img)
         return visualizations
```

### Comparing `sihl-0.0.3.dev3/src/sihl/lightning_module.py` & `sihl-0.0.3.dev4/src/sihl/lightning_module.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,66 +30,79 @@
         self.scheduler = scheduler
         self.scheduler_kwargs = scheduler_kwargs or {}
 
     def forward(self, x: Tensor) -> list[Tensor | tuple[Tensor, ...]]:
         return self.model(x)  # type:ignore
 
     def training_step(
-        self, batch: tuple[Tensor, list[Tensor] | Tensor], batch_idx: int
+        self, batch: tuple[Tensor, Any], batch_idx: int
     ) -> Tensor:
         x, targets = batch
+        if not isinstance(targets, list):
+            targets = [targets]  # single-headed
         head_inputs = self.model.backbone(x)
         if self.model.neck:
-            head_inputs = self.model.neck(x)
+            head_inputs = self.model.neck(head_inputs)
         losses = []
         log_options = {"on_epoch": False, "on_step": True, "prog_bar": True}
         for head_idx, (head, target) in enumerate(zip(self.model.heads, targets)):
-            loss, metrics = head.training_step(head_inputs, target)
+            if isinstance(target, dict):
+                loss, metrics = head.training_step(head_inputs, **target)
+            else:
+                loss, metrics = head.training_step(head_inputs, target)
             metrics = {f"{head_idx}/{k}": v for k, v in metrics.items()}
             try:
                 self.log(f"{head_idx}/train/loss", loss, **log_options)  # type: ignore
                 self.log_dict(metrics, **log_options)  # type: ignore
             except:
                 pass
             losses.append(loss)
-        loss = sum(losses, torch.zeros(1))
+        loss = sum(losses, torch.zeros(1, device=losses[0].device))
         scheduler = self.lr_schedulers()
         if isinstance(scheduler, _LRScheduler):
             scheduler.step()
             lr = scheduler.get_last_lr()[0]
             try:
                 self.log("lr", lr, **log_options)  # type: ignore
             except:
                 pass
         return loss  # type:ignore
 
     def validation_step(
-        self, batch: tuple[Tensor, list[Tensor] | Tensor], batch_idx: int
+        self, batch: tuple[Tensor, Any], batch_idx: int
     ) -> Tensor:
         x, targets = batch
+        if not isinstance(targets, list):
+            targets = [targets]  # single-headed
         head_inputs = self.model.backbone(x)
         if self.model.neck:
-            head_inputs = self.model.neck(x)
+            head_inputs = self.model.neck(head_inputs)
         if batch_idx == 0 and self.logger and hasattr(self.logger, "experiment"):
             for head_idx, (head, target) in enumerate(zip(self.model.heads, targets)):
                 try:
-                    images = head.visualize(head_inputs, target)  # type: ignore
+                    if isinstance(target, dict):
+                        images = head.visualize(head_inputs, **target)  # type: ignore
+                    else:
+                        images = head.visualize(head_inputs, target)
                     for sample_idx, image in enumerate(images):
                         self.logger.experiment.add_image(
                             f"{head_idx}/eval/{sample_idx}",
                             image,
                             global_step=self.global_step,
                         )
                 except Exception as e:
                     logging.warn(e)
         losses = []
         for head_idx, (head, target) in enumerate(zip(self.model.heads, targets)):
-            loss, metrics = head.validation_step(head_inputs, target)
+            if isinstance(target, dict):
+                loss, metrics = head.validation_step(head_inputs, **target)
+            else:
+                loss, metrics = head.validation_step(head_inputs, target)
             losses.append(loss)
-        loss = sum(losses, torch.zeros(1))
+        loss = sum(losses, torch.zeros(1, device=losses[0].device))
         return loss  # type:ignore
 
     def configure_optimizers(
         self,
     ) -> Optimizer | tuple[list[Optimizer], list[_LRScheduler]]:
         optimizer = self.optimizer(self.parameters(), **self.optimizer_kwargs)
         if self.scheduler:
```

### Comparing `sihl-0.0.3.dev3/src/sihl/sihl_model.py` & `sihl-0.0.3.dev4/src/sihl/sihl_model.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev3/src/sihl/timm_backbone.py` & `sihl-0.0.3.dev4/src/sihl/timm_backbone.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev3/src/sihl/torchvision_backbone.py` & `sihl-0.0.3.dev4/src/sihl/torchvision_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
             else Normalize(mean=(0.5,), std=(0.5,))
         )
         self.model = torchvision.models.get_model(
             name, weights="DEFAULT" if pretrained else None
         )
         self.model = create_feature_extractor(self.model, level_names)
         self.model = fx.symbolic_trace(self.model)  # type: ignore
+        # self.model = torch.compile(self.model)
         update_input_channels(self.model, input_channels)
         self.pad = PadToMultipleOf(32)
         # freeze modules in first `frozen_levels` levels
         self.model.eval()  # freeze batchnorms
         if frozen_levels < 0:
             for module_name, _ in self.model.named_modules():
                 for param in self.model.get_submodule(module_name).parameters():
```

### Comparing `sihl-0.0.3.dev3/PKG-INFO` & `sihl-0.0.3.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sihl
-Version: 0.0.3.dev3
+Version: 0.0.3.dev4
 Summary: Simple Image Heads and Layers
 License: MIT
 Author: jonregef
 Author-email: jon.regef@pm.me
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

