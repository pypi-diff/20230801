# Comparing `tmp/thetagang-1.7.1.tar.gz` & `tmp/thetagang-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thetagang-1.7.1.tar", max compression
+gzip compressed data, was "thetagang-1.7.2.tar", max compression
```

## Comparing `thetagang-1.7.1.tar` & `thetagang-1.7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    34523 2023-07-19 15:05:25.867614 thetagang-1.7.1/LICENSE
--rw-r--r--   0        0        0    14617 2023-07-19 15:05:25.867614 thetagang-1.7.1/README.md
--rw-r--r--   0        0        0     1660 2023-07-19 15:05:25.867614 thetagang-1.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/__init__.py
--rw-r--r--   0        0        0     9120 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/config.py
--rw-r--r--   0        0        0     1396 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/config_defaults.py
--rw-r--r--   0        0        0     1461 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/dict_merge.py
--rw-r--r--   0        0        0       59 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/entry.py
--rw-r--r--   0        0        0     1091 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/fmt.py
--rw-r--r--   0        0        0     1022 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/main.py
--rw-r--r--   0        0        0      377 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/options.py
--rw-r--r--   0        0        0    79453 2023-07-19 15:05:25.875614 thetagang-1.7.1/thetagang/portfolio_manager.py
--rw-r--r--   0        0        0     3951 2023-07-19 15:05:25.875614 thetagang-1.7.1/thetagang/test_util.py
--rwxr-xr-x   0        0        0     8433 2023-07-19 15:05:25.875614 thetagang-1.7.1/thetagang/thetagang.py
--rw-r--r--   0        0        0     5820 2023-07-19 15:05:25.875614 thetagang-1.7.1/thetagang/util.py
--rw-r--r--   0        0        0    15877 1970-01-01 00:00:00.000000 thetagang-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-08-01 12:56:18.877627 thetagang-1.7.2/LICENSE
+-rw-r--r--   0        0        0    14617 2023-08-01 12:56:18.877627 thetagang-1.7.2/README.md
+-rw-r--r--   0        0        0     1665 2023-08-01 12:56:18.877627 thetagang-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 12:56:18.881627 thetagang-1.7.2/thetagang/__init__.py
+-rw-r--r--   0        0        0     9120 2023-08-01 12:56:18.881627 thetagang-1.7.2/thetagang/config.py
+-rw-r--r--   0        0        0     1396 2023-08-01 12:56:18.881627 thetagang-1.7.2/thetagang/config_defaults.py
+-rw-r--r--   0        0        0     1461 2023-08-01 12:56:18.881627 thetagang-1.7.2/thetagang/dict_merge.py
+-rw-r--r--   0        0        0       59 2023-08-01 12:56:18.881627 thetagang-1.7.2/thetagang/entry.py
+-rw-r--r--   0        0        0     1091 2023-08-01 12:56:18.881627 thetagang-1.7.2/thetagang/fmt.py
+-rw-r--r--   0        0        0     1022 2023-08-01 12:56:18.881627 thetagang-1.7.2/thetagang/main.py
+-rw-r--r--   0        0        0      377 2023-08-01 12:56:18.885628 thetagang-1.7.2/thetagang/options.py
+-rw-r--r--   0        0        0    79544 2023-08-01 12:56:18.885628 thetagang-1.7.2/thetagang/portfolio_manager.py
+-rw-r--r--   0        0        0     3951 2023-08-01 12:56:18.885628 thetagang-1.7.2/thetagang/test_util.py
+-rwxr-xr-x   0        0        0     8433 2023-08-01 12:56:18.885628 thetagang-1.7.2/thetagang/thetagang.py
+-rw-r--r--   0        0        0     5901 2023-08-01 12:56:18.885628 thetagang-1.7.2/thetagang/util.py
+-rw-r--r--   0        0        0    15873 1970-01-01 00:00:00.000000 thetagang-1.7.2/PKG-INFO
```

### Comparing `thetagang-1.7.1/LICENSE` & `thetagang-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.1/README.md` & `thetagang-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.1/pyproject.toml` & `thetagang-1.7.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 description = "ThetaGang is an IBKR bot for getting money"
 documentation = "https://github.com/brndnmtthws/thetagang/blob/master/README.md"
 homepage = "https://github.com/brndnmtthws/thetagang"
 license = "AGPL-3.0-only"
 name = "thetagang"
 readme = "README.md"
 repository = "https://github.com/brndnmtthws/thetagang.git"
-version = "1.7.1"
+version = "1.7.2"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 click-log = "^0.4.0"
 ib_insync = "^0.9.86"
 python = ">=3.9,<4.0"
 python-dateutil = "^2.8.1"
 pytimeparse = "^1.1.8"
 schema = "^0.7.5"
 toml = "^0.10.2"
 rich = "^13.3.5"
-more-itertools = "^9.1.0"
+more-itertools = ">=9.1,<11.0"
 
 [tool.poetry.group.dev.dependencies]
 autoflake = "^2.0"
 autohooks = "^23.4.0"
 autohooks-plugin-black = ">=22.11,<24.0"
 autohooks-plugin-isort = ">=22.8,<24.0"
 autohooks-plugin-pylint = ">=22.8.1,<24.0.0"
```

### Comparing `thetagang-1.7.1/thetagang/config.py` & `thetagang-1.7.2/thetagang/config.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.1/thetagang/config_defaults.py` & `thetagang-1.7.2/thetagang/config_defaults.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.1/thetagang/dict_merge.py` & `thetagang-1.7.2/thetagang/dict_merge.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.1/thetagang/fmt.py` & `thetagang-1.7.2/thetagang/fmt.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.1/thetagang/main.py` & `thetagang-1.7.2/thetagang/main.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.1/thetagang/portfolio_manager.py` & `thetagang-1.7.2/thetagang/portfolio_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1731,15 +1731,15 @@
 
     def do_cashman(self, account_summary, portfolio_positions):
         to_print = []
 
         def inner_handler():
             if not self.config["cash_management"]["enabled"]:
                 to_print.append(
-                    "[red]🛑 Cash managementnot enabled, skipping",
+                    "[red]🛑 Cash management not enabled, skipping",
                 )
                 return
 
             target_cash_balance = self.config["cash_management"]["target_cash_balance"]
             buy_threshold = self.config["cash_management"]["buy_threshold"]
             sell_threshold = self.config["cash_management"]["sell_threshold"]
             cash_balance = math.floor(float(account_summary["TotalCashValue"].value))
@@ -1762,15 +1762,15 @@
                     algo = (
                         self.config["cash_management"]["orders"]["algo"]
                         if "orders" in self.config["cash_management"]
                         else self.config["orders"]["algo"]
                     )
 
                     amount = cash_balance - target_cash_balance
-                    price = ticker.ask
+                    price = ticker.ask if amount > 0 else ticker.bid
                     qty = amount // price
 
                     if qty > 0:
                         to_print.append(
                             f"[green]cash_balance={cash_balance} which exceeds "
                             f"(target_cash_balance + buy_threshold)={(target_cash_balance + buy_threshold)}"
                         )
@@ -1948,15 +1948,17 @@
                             order.algoStrategy = ""
                             order.algoParams = []
                             order.tif = ""
                             order.account = ""
 
                         # put the trade back from whence it came
                         self.trades[idx] = self.ib.placeOrder(contract, order)
-                        console.print(f"[blue]Order updated, trade={self.trades[idx]}")
+                        console.print(
+                            f"[blue]Order updated, order={self.trades[idx].order}"
+                        )
                 else:
                     console.print(
                         f"[red]Couldn't get midpoint price for {trade.contract}, skipping"
                     )
             except RuntimeError:
                 console.print_exception()
```

### Comparing `thetagang-1.7.1/thetagang/test_util.py` & `thetagang-1.7.2/thetagang/test_util.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.1/thetagang/thetagang.py` & `thetagang-1.7.2/thetagang/thetagang.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.1/thetagang/util.py` & `thetagang-1.7.2/thetagang/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         return math.floor(
             sum(
                 [
                     p.position
                     for p in portfolio_positions[symbol]
                     if isinstance(p.contract, Option)
                     and p.contract.right.upper().startswith(right.upper())
+                    and option_dte(p.contract.lastTradeDateOrContractMonth) >= 0
                     and (
                         not ignore_zero_dte
                         or option_dte(p.contract.lastTradeDateOrContractMonth) > 0
                     )
                 ]
             )
         )
```

### Comparing `thetagang-1.7.1/PKG-INFO` & `thetagang-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: thetagang
-Version: 1.7.1
+Version: 1.7.2
 Summary: ThetaGang is an IBKR bot for getting money
 Home-page: https://github.com/brndnmtthws/thetagang
 License: AGPL-3.0-only
 Author: Brenden Matthews
 Author-email: brenden@brndn.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
 Requires-Dist: ib_insync (>=0.9.86,<0.10.0)
-Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
+Requires-Dist: more-itertools (>=9.1,<11.0)
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: pytimeparse (>=1.1.8,<2.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: schema (>=0.7.5,<0.8.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Bug Tracker, https://github.com/brndnmtthws/thetagang/issues
 Project-URL: Documentation, https://github.com/brndnmtthws/thetagang/blob/master/README.md
```

