# Comparing `tmp/fw_classification-0.4.1-py3-none-any.whl.zip` & `tmp/fw_classification-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 30133 bytes, number of entries: 24
+Zip file size: 30334 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      220 b- defN 80-Jan-01 00:00 fw_classification/__init__.py
 -rw-r--r--  2.0 unx      622 b- defN 80-Jan-01 00:00 fw_classification/adapters/__init__.py
 -rw-r--r--  2.0 unx     1329 b- defN 80-Jan-01 00:00 fw_classification/adapters/base.py
 -rw-r--r--  2.0 unx      981 b- defN 80-Jan-01 00:00 fw_classification/adapters/deps.py
 -rw-r--r--  2.0 unx     1498 b- defN 80-Jan-01 00:00 fw_classification/adapters/dicom.py
 -rw-r--r--  2.0 unx     4485 b- defN 80-Jan-01 00:00 fw_classification/adapters/fw.py
 -rw-r--r--  2.0 unx     5504 b- defN 80-Jan-01 00:00 fw_classification/adapters/nifti.py
 -rw-r--r--  2.0 unx      995 b- defN 80-Jan-01 00:00 fw_classification/adapters/utils.py
 -rw-r--r--  2.0 unx     1027 b- defN 80-Jan-01 00:00 fw_classification/classify/__init__.py
 -rw-r--r--  2.0 unx     8416 b- defN 80-Jan-01 00:00 fw_classification/classify/block.py
 -rw-r--r--  2.0 unx     1125 b- defN 80-Jan-01 00:00 fw_classification/classify/expressions/__init__.py
--rw-r--r--  2.0 unx    12154 b- defN 80-Jan-01 00:00 fw_classification/classify/expressions/base.py
--rw-r--r--  2.0 unx    13179 b- defN 80-Jan-01 00:00 fw_classification/classify/expressions/expression.py
+-rw-r--r--  2.0 unx    12429 b- defN 80-Jan-01 00:00 fw_classification/classify/expressions/base.py
+-rw-r--r--  2.0 unx    14736 b- defN 80-Jan-01 00:00 fw_classification/classify/expressions/expression.py
 -rw-r--r--  2.0 unx     2919 b- defN 80-Jan-01 00:00 fw_classification/classify/includes.py
 -rw-r--r--  2.0 unx     8444 b- defN 80-Jan-01 00:00 fw_classification/classify/profile.py
 -rw-r--r--  2.0 unx    10859 b- defN 80-Jan-01 00:00 fw_classification/classify/rule.py
 -rw-r--r--  2.0 unx     2555 b- defN 80-Jan-01 00:00 fw_classification/classify/utils.py
 -rw-r--r--  2.0 unx     2945 b- defN 80-Jan-01 00:00 fw_classification/cli.py
 -rw-r--r--  2.0 unx      605 b- defN 80-Jan-01 00:00 fw_classification/utils.py
--rw-r--r--  2.0 unx     1077 b- defN 80-Jan-01 00:00 fw_classification-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3907 b- defN 80-Jan-01 00:00 fw_classification-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_classification-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      108 b- defN 80-Jan-01 00:00 fw_classification-0.4.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2208 b- defN 16-Jan-01 00:00 fw_classification-0.4.1.dist-info/RECORD
-24 files, 87250 bytes uncompressed, 26489 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx     1077 b- defN 80-Jan-01 00:00 fw_classification-0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3907 b- defN 80-Jan-01 00:00 fw_classification-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_classification-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      108 b- defN 80-Jan-01 00:00 fw_classification-0.4.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2208 b- defN 16-Jan-01 00:00 fw_classification-0.4.2.dist-info/RECORD
+24 files, 89082 bytes uncompressed, 26690 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -51,23 +51,23 @@
 
 Filename: fw_classification/cli.py
 Comment: 
 
 Filename: fw_classification/utils.py
 Comment: 
 
-Filename: fw_classification-0.4.1.dist-info/LICENSE
+Filename: fw_classification-0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: fw_classification-0.4.1.dist-info/METADATA
+Filename: fw_classification-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: fw_classification-0.4.1.dist-info/WHEEL
+Filename: fw_classification-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: fw_classification-0.4.1.dist-info/entry_points.txt
+Filename: fw_classification-0.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: fw_classification-0.4.1.dist-info/RECORD
+Filename: fw_classification-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_classification/classify/expressions/base.py

```diff
@@ -267,22 +267,28 @@
             try:
                 sub = self.variables[variable]
             except KeyError as e:
                 raise ValueError(f"Variable {variable} not found.") from e
             return sub + ("." + key if key else "")
         return val
 
+    def _resolve_value(self, i_dict: Dotty) -> t.Any:
+        """Get value in input-dict if exists, replacing `None` with ""."""
+        self._value = i_dict.get(self.value, "")
+
     @property
     def field(self) -> str:
         """Field property injecting variables."""
         return self._inject_variables(self._field)
 
     @property
     def value(self) -> t.Any:
         """Value property injecting variables."""
+        if isinstance(self._value, str):
+            return self._inject_variables(self._value)
         return self._value
 
     @classmethod
     def validate(  # pylint: disable=unused-argument
         cls: t.Type["BinaryExpression"],
         field: str,
         val: t.Any,
```

## fw_classification/classify/expressions/expression.py

```diff
@@ -95,34 +95,44 @@
         float(val)
     except (ValueError, TypeError):
         return False
     return True
 
 
 class Contains(MatchExpression):
-    """Returns True if `value` is in the `field`."""
+    """Returns True if `value` is in the `field`.
+
+    Config Options:
+    resolve (bool, default false) Resolves "value" as a key from i_dict
+    """
 
     op = "contains"
 
     def matches(self, i_dict: Dotty) -> bool:
         """Evaluate match."""
+        if "resolve" in self.config and self.config["resolve"]:
+            self._resolve_value(i_dict)
+            if not self._value:
+                log.debug(f"_resolve_value returns empty!")
         val = self.get_value(i_dict)
+
         return self.value in val
 
     def __repr__(self):
         """Implement `repr()`."""
         return f"{self.value} is in {self._field}"
 
 
 class Is(MatchExpression):
     """Returns True if the `field`'s value equals `value`.
 
     Config Options:
         approximate (int, default 0): Allow approximate values to n decimals if
             n > 0
+        resolve (bool, default false) Resolves "value" as a key from i_dict
     """
 
     op = "is"
 
     @staticmethod
     def validate(
         field: str,
@@ -133,42 +143,59 @@
         """Validate regex config option(s)."""
         err = super(Is, Is).validate(field, val, variables, **kwargs)
         if "approximate" in kwargs:
             if not isinstance(kwargs["approximate"], int):
                 err.append(
                     f"Is: approximate must be int, found '{kwargs['approximate']}'"
                 )
-            if not is_numeric(val):
-                err.append(f"Value must be numeric if using approximate, found '{val}'")
+            if "resolve" not in kwargs:
+                if not is_numeric(val):
+                    err.append(
+                        f"Value must be numeric if using approximate, found '{val}'"
+                    )
         return err
 
     def matches(self, i_dict: Dotty) -> bool:
         """Evaluate match."""
+        if "resolve" in self.config and self.config["resolve"]:
+            self._resolve_value(i_dict)
+            if not self._value:
+                log.debug(f"_resolve_value returns empty!")
         val = self.get_value(i_dict)
+
         if "approximate" in self.config and self.config["approximate"]:
             dig = self.config["approximate"]
             return round(val, ndigits=dig) == round(self.value, ndigits=dig)
         return val == self.value
 
     def __repr__(self):
         """Implement `repr()`."""
         base = f"{self._field} is {self.value}"
         if "approximate" in self.config and self.config["approximate"]:
             base += f" when rounding to {self.config['approximate']} digits"
         return base
 
 
 class In(MatchExpression):
-    """Return True if `field`'s value is in the list `value`."""
+    """Return True if `field`'s value is in the list `value`.
+
+    Config Options:
+    resolve (bool, default false) Resolves "value" as a key from i_dict
+    """
 
     op = "in"
 
     def matches(self, i_dict: Dotty) -> bool:
         """Evaluate match."""
+        if "resolve" in self.config and self.config["resolve"]:
+            self._resolve_value(i_dict)
+            if not self._value:
+                log.debug(f"_resolve_value returns empty!")
         val = self.get_value(i_dict)
+
         return val in self.value
 
     def __repr__(self):
         """Implement `repr()`."""
         return f"{self._field} is in {self.value}"
 
 
@@ -269,15 +296,16 @@
         field: str,
         val: t.Any,
         variables: t.Optional[t.Dict[str, str]] = None,
         **kwargs,
     ) -> None:
         """Init numeric expression."""
         super().__init__(field, val, variables, **kwargs)
-        self._value = float(val)
+        if not isinstance(val, str):
+            self._value = float(val)
 
     @classmethod
     def validate(
         cls: t.Type["NumericMatchExpression"],
         field: str,
         val: t.Any,
         variables: t.Optional[t.Dict[str, str]] = None,
@@ -295,22 +323,33 @@
                     f"{cls.op}: approximate must be int, "
                     f"found '{kwargs['approximate']}'"
                 )
         return err
 
     def matches(self, i_dict: Dotty) -> bool:
         """Evaluate match."""
+        if "resolve" in self.config and self.config["resolve"]:
+            self._resolve_value(i_dict)
+            if not self._value:
+                log.debug(f"_resolve_value returns empty!")
         val = self.get_value(i_dict)
+
         if not is_numeric(val):
             log.warning(
                 f"{self.op}: Found non-numeric input for field "
                 f"'{self.field}': '{val}'"
             )
             return False
-        res = self.func(float(val), self.value)
+        try:
+            res = self.func(float(val), float(self.value))
+        except ValueError:
+            log.warning(
+                f"{self.op}: Cannot convert val: {val} or self.value {self.value} to float"
+            )
+            return False
         if not res and self.config.get("approximate"):
             dig = self.config["approximate"]
             return round(val, ndigits=dig) == round(self.value, ndigits=dig)
         return res
 
 
 class LessThan(NumericMatchExpression):
@@ -325,14 +364,16 @@
             - key: file.info.header.dicom.EchoTime
               less_than: 15.5
               approximate: 1
 
             this would match if the echo time was 15, but also would match
             if echo time was 15.54, since:
             round(15.54, ndigits=1) == round(15.5, ndigits=1)
+
+        resolve (bool, default false) Resolves "value" as a key from i_dict
     """
 
     op = "less_than"
     func = operator.lt
 
     def __repr__(self):
         """Implement `repr()`."""
@@ -354,14 +395,17 @@
             - key: file.info.header.dicom.EchoTime
               greater_than: 15.5
               approximate: 1
 
             this would match if the echo time was 15.6, but also would match
             if echo time was 15.49, since:
             round(15.49, ndigits=1) == round(15.5, ndigits=1)
+
+        resolve (bool, default false) Resolves "value" as a key from i_dict
+
     """
 
     op = "greater_than"
     func = operator.gt
 
     def __repr__(self):
         """Implement `repr()`."""
```

## Comparing `fw_classification-0.4.1.dist-info/LICENSE` & `fw_classification-0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_classification-0.4.1.dist-info/METADATA` & `fw_classification-0.4.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-classification
-Version: 0.4.1
+Version: 0.4.2
 Summary: Flywheel classification toolkit.
 Home-page: https://gitlab.com/flywheel-io/public/classification-toolkit
 License: MIT
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `fw_classification-0.4.1.dist-info/RECORD` & `fw_classification-0.4.2.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 fw_classification/adapters/dicom.py,sha256=peyvT4CzmiQsBqzkgLslqpWNT11a5QGmrBrnsm8SGZM,1498
 fw_classification/adapters/fw.py,sha256=BndjgHnMuO7z9iJZ7gUUVhA-fVpUgKLJnemvTZtEfW4,4485
 fw_classification/adapters/nifti.py,sha256=dh3_f5YOOGnSLIiS_t6KsaNHvhQnhPO1dJR3PmPRqTk,5504
 fw_classification/adapters/utils.py,sha256=0mWQJbcRPjGV_jAoB69ysJhECo1sAl3oWojQmaHbMwY,995
 fw_classification/classify/__init__.py,sha256=3rxsLgmwxl4m_pMBHZwEwBmioMEI7By8C2LPRr7TWZs,1027
 fw_classification/classify/block.py,sha256=mYZXAwqtUsjAOpH3EBdBPOjTtwyBxLGrQVMH4qziyEM,8416
 fw_classification/classify/expressions/__init__.py,sha256=eyOhQSKwd1IhmY3aP-CFiGrdihgQc-6chhOj5EtwBEA,1125
-fw_classification/classify/expressions/base.py,sha256=Mu-H-bS9kHYJMtrKbA6hrrQzVq3OOcibF0OcbcmIgbQ,12154
-fw_classification/classify/expressions/expression.py,sha256=xDxLlenh5WVAukzYRUnPbY46UawwhhSVZx4Exg83PF4,13179
+fw_classification/classify/expressions/base.py,sha256=PgXZ8KKn0RfjIUoiiQelREtRArWcUAk5i4be-nkLtLQ,12429
+fw_classification/classify/expressions/expression.py,sha256=vUZuQJY-RoZEk4xOO6023esMMImrAgaQArJBez5bRuo,14736
 fw_classification/classify/includes.py,sha256=6RKiFpl0Mr0hvTXgNfQWXSp_-SobxQDZ2zVP62KtqLk,2919
 fw_classification/classify/profile.py,sha256=-uHR1_p1E4fgVtZ_BitYYtT7_EP9EKRaOYy40DDOXvc,8444
 fw_classification/classify/rule.py,sha256=Ly6NVQk-4OnWvIOgl2hKMYJqFyf5U4__pM5Z0Dfbdm8,10859
 fw_classification/classify/utils.py,sha256=WE2EUM4aHJts7xuDT_-6Gd1XDYhN_XFxnNsx7XMoZZc,2555
 fw_classification/cli.py,sha256=0ImcEIb3vBnMIiUUYkFlba3ECP2C0z3oJ793-4EhgCk,2945
 fw_classification/utils.py,sha256=CCu7yx7i1WA6EfCswQB886tiCbMdc5zF7LJJFbpDGRE,605
-fw_classification-0.4.1.dist-info/LICENSE,sha256=EmDQE8zHgRCuAaYxpDVanIo1Nmn7VUdxGHD17LXcjYY,1077
-fw_classification-0.4.1.dist-info/METADATA,sha256=0tGJpXMMQdCltpIHHvwCdAs0ZEBAqpERXGWuV-hqVqo,3907
-fw_classification-0.4.1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fw_classification-0.4.1.dist-info/entry_points.txt,sha256=RyLEV0GDVT8CzEXFkhUktLw24ywdokP6zjVuDUxYTOI,108
-fw_classification-0.4.1.dist-info/RECORD,,
+fw_classification-0.4.2.dist-info/LICENSE,sha256=EmDQE8zHgRCuAaYxpDVanIo1Nmn7VUdxGHD17LXcjYY,1077
+fw_classification-0.4.2.dist-info/METADATA,sha256=XU2w5SVqgb1189FJmnH_TCITP1a4yHpUfcSBFXuExLA,3907
+fw_classification-0.4.2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fw_classification-0.4.2.dist-info/entry_points.txt,sha256=RyLEV0GDVT8CzEXFkhUktLw24ywdokP6zjVuDUxYTOI,108
+fw_classification-0.4.2.dist-info/RECORD,,
```

