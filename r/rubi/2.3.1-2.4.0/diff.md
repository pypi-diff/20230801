# Comparing `tmp/rubi-2.3.1.tar.gz` & `tmp/rubi-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.3.1.tar", max compression
+gzip compressed data, was "rubi-2.4.0.tar", max compression
```

## Comparing `rubi-2.3.1.tar` & `rubi-2.4.0.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0    11357 2023-07-27 16:56:45.537845 rubi-2.3.1/LICENSE
--rw-r--r--   0        0        0     2757 2023-07-27 16:56:45.537845 rubi-2.3.1/README.md
--rw-r--r--   0        0        0     6735 2023-07-27 16:56:45.537845 rubi-2.3.1/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-07-27 16:56:45.537845 rubi-2.3.1/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-07-27 16:56:45.537845 rubi-2.3.1/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-27 16:56:45.537845 rubi-2.3.1/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      833 2023-07-27 16:56:45.537845 rubi-2.3.1/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-27 16:56:45.537845 rubi-2.3.1/network_config/arbitrum_one/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-27 16:56:45.537845 rubi-2.3.1/network_config/arbitrum_one/abis/router.json
--rw-r--r--   0        0        0      840 2023-07-27 16:56:45.537845 rubi-2.3.1/network_config/arbitrum_one/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-27 16:56:45.537845 rubi-2.3.1/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-27 16:56:45.537845 rubi-2.3.1/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      858 2023-07-27 16:56:45.537845 rubi-2.3.1/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-27 16:56:45.541845 rubi-2.3.1/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-27 16:56:45.541845 rubi-2.3.1/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      760 2023-07-27 16:56:45.541845 rubi-2.3.1/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-27 16:56:45.541845 rubi-2.3.1/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-27 16:56:45.541845 rubi-2.3.1/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      832 2023-07-27 16:56:45.541845 rubi-2.3.1/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0     1746 2023-07-27 16:57:33.886614 rubi-2.3.1/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/__init__.py
--rw-r--r--   0        0        0    33458 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/client.py
--rw-r--r--   0        0        0      163 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    65755 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/contracts/aid.py
--rw-r--r--   0        0        0    15707 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       74 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    16374 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     3701 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    18883 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    25130 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/contracts/market.py
--rw-r--r--   0        0        0    15165 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/contracts/router.py
--rw-r--r--   0        0        0       77 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/data/README.md
--rw-r--r--   0        0        0       31 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/data/__init__.py
--rw-r--r--   0        0        0    17073 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/data/market.py
--rw-r--r--   0        0        0       72 2023-07-27 16:56:45.541845 rubi-2.3.1/rubi/network/__init__.py
--rw-r--r--   0        0        0     8475 2023-07-27 16:56:45.545845 rubi-2.3.1/rubi/network/network.py
--rw-r--r--   0        0        0      121 2023-07-27 16:56:45.545845 rubi-2.3.1/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    16249 2023-07-27 16:56:45.545845 rubi-2.3.1/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0    11701 2023-07-27 16:56:45.545845 rubi-2.3.1/rubi/rubicon_types/order_query.py
--rw-r--r--   0        0        0     6323 2023-07-27 16:56:45.545845 rubi-2.3.1/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2779 2023-07-27 16:56:45.545845 rubi-2.3.1/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0    11414 2023-07-27 16:56:45.545845 rubi-2.3.1/rubi/rubicon_types/trade_query.py
--rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 14:34:37.465132 rubi-2.4.0/LICENSE
+-rw-r--r--   0        0        0     2757 2023-08-01 14:34:37.465132 rubi-2.4.0/README.md
+-rw-r--r--   0        0        0     6735 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      833 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/arbitrum_one/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/arbitrum_one/abis/router.json
+-rw-r--r--   0        0        0      840 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/arbitrum_one/network.yaml
+-rw-r--r--   0        0        0    32732 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      858 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      760 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      832 2023-08-01 14:34:37.465132 rubi-2.4.0/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0     1746 2023-08-01 14:35:20.438273 rubi-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-08-01 14:34:37.469132 rubi-2.4.0/rubi/__init__.py
+-rw-r--r--   0        0        0    36583 2023-08-01 14:34:37.469132 rubi-2.4.0/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-08-01 14:34:37.469132 rubi-2.4.0/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    15707 2023-08-01 14:34:37.469132 rubi-2.4.0/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-08-01 14:34:37.469132 rubi-2.4.0/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    16374 2023-08-01 14:34:37.469132 rubi-2.4.0/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     3701 2023-08-01 14:34:37.469132 rubi-2.4.0/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    18883 2023-08-01 14:34:37.469132 rubi-2.4.0/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    25130 2023-08-01 14:34:37.469132 rubi-2.4.0/rubi/contracts/market.py
+-rw-r--r--   0        0        0    15165 2023-08-01 14:34:37.473132 rubi-2.4.0/rubi/contracts/router.py
+-rw-r--r--   0        0        0       77 2023-08-01 14:34:37.473132 rubi-2.4.0/rubi/data/README.md
+-rw-r--r--   0        0        0       31 2023-08-01 14:34:37.473132 rubi-2.4.0/rubi/data/__init__.py
+-rw-r--r--   0        0        0    17073 2023-08-01 14:34:37.473132 rubi-2.4.0/rubi/data/market.py
+-rw-r--r--   0        0        0       72 2023-08-01 14:34:37.473132 rubi-2.4.0/rubi/network/__init__.py
+-rw-r--r--   0        0        0     8475 2023-08-01 14:34:37.473132 rubi-2.4.0/rubi/network/network.py
+-rw-r--r--   0        0        0      121 2023-08-01 14:34:37.473132 rubi-2.4.0/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    18343 2023-08-01 14:34:37.473132 rubi-2.4.0/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0    11701 2023-08-01 14:34:37.473132 rubi-2.4.0/rubi/rubicon_types/order_query.py
+-rw-r--r--   0        0        0     6323 2023-08-01 14:34:37.473132 rubi-2.4.0/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2779 2023-08-01 14:34:37.473132 rubi-2.4.0/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0    11414 2023-08-01 14:34:37.473132 rubi-2.4.0/rubi/rubicon_types/trade_query.py
+-rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.4.0/PKG-INFO
```

### Comparing `rubi-2.3.1/LICENSE` & `rubi-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/README.md` & `rubi-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/ERC20.json` & `rubi-2.4.0/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/README.md` & `rubi-2.4.0/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/abitrum_goerli/abis/market.json` & `rubi-2.4.0/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/abitrum_goerli/abis/router.json` & `rubi-2.4.0/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/abitrum_goerli/network.yaml` & `rubi-2.4.0/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/arbitrum_one/abis/market.json` & `rubi-2.4.0/network_config/arbitrum_one/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/arbitrum_one/abis/router.json` & `rubi-2.4.0/network_config/arbitrum_one/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/arbitrum_one/network.yaml` & `rubi-2.4.0/network_config/arbitrum_one/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/optimism/abis/market.json` & `rubi-2.4.0/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/optimism/abis/router.json` & `rubi-2.4.0/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/optimism/network.yaml` & `rubi-2.4.0/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/optimism_goerli/abis/market.json` & `rubi-2.4.0/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/optimism_goerli/abis/router.json` & `rubi-2.4.0/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/optimism_goerli/network.yaml` & `rubi-2.4.0/network_config/optimism_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/polygon_mumbai/abis/market.json` & `rubi-2.4.0/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/polygon_mumbai/abis/router.json` & `rubi-2.4.0/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/network_config/polygon_mumbai/network.yaml` & `rubi-2.4.0/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/pyproject.toml` & `rubi-2.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.3.1"
+version = "2.4.0"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.3.1/rubi/client.py` & `rubi-2.4.0/rubi/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,17 +31,19 @@
     Pair,
     OrderBook,
     PairDoesNotExistException,
     BaseEvent,
     FeeEvent,
     OrderEvent,
     Transaction,
-    BaseNewOrder,
+    BaseOrder,
     NewCancelOrder,
     UpdateLimitOrder,
+    ActiveLimitOrder,
+    OrderType,
 )
 
 
 class Client:
     """This class is a client for Rubicon. It aims to provide a simple and understandable interface when interacting
     with the Rubicon protocol. If not instantiated with a wallet and key then all the methods that require signing
     will throw an error.
@@ -74,23 +76,27 @@
         self.market = RubiconMarket.from_network(
             network=self.network, wallet=self.wallet, key=self.key
         )
         self.router = RubiconRouter.from_network(
             network=self.network, wallet=self.wallet, key=self.key
         )
 
+        # TODO a Dict of { symbol: ERC20 }, investigate
         self.tokens = self.get_network_tokens()
         self._pairs: Dict[str, Pair] = {}
 
         self.message_queue = message_queue  # type: Queue | None
 
         self.market_data = MarketData.from_network_with_tokens(
             network=self.network, network_tokens=self.tokens
         )
 
+        # Order tracking
+        self.active_limit_orders: Dict[int, ActiveLimitOrder] = {}
+
     @classmethod
     def from_http_node_url(
         cls,
         http_node_url: str,
         custom_token_addresses_file: Optional[str] = None,
         message_queue: Optional[Queue] = None,
         wallet: Optional[Union[ChecksumAddress, str]] = None,
@@ -450,14 +456,16 @@
             if isinstance(raw_event, EmitFeeEvent):
                 event = FeeEvent.from_event(pair=pair, event=raw_event)
             else:
                 event = OrderEvent.from_event(
                     pair=pair, event=raw_event, wallet=self.wallet
                 )
 
+                self._update_active_limit_orders(order_events=[event])
+
             self.message_queue.put(event)
 
     ######################################################################
     # order methods
     ######################################################################
 
     def place_market_order(self, transaction: Transaction) -> TransactionReceipt:
@@ -472,15 +480,15 @@
         :raises Exception: If the transaction contains more than one order.
         """
         if len(transaction.orders) > 1:
             raise Exception("call place_order with one order only")
 
         order: NewMarketOrder = transaction.orders[0]  # noqa
 
-        pair = self.get_pair(pair_name=order.pair)
+        pair = self.get_pair(pair_name=order.pair_name)
 
         match order.order_side:
             case OrderSide.BUY:
                 transaction_receipt = self.market.buy_all_amount(
                     buy_gem=pair.base_asset.address,
                     buy_amt=pair.base_asset.to_integer(order.size),
                     pay_gem=pair.quote_asset.address,
@@ -515,15 +523,15 @@
         :raises Exception: If the transaction contains more than one order.
         """
         if len(transaction.orders) > 1:
             raise Exception("call place_order with one order only")
 
         order: NewLimitOrder = transaction.orders[0]  # noqa
 
-        pair = self.get_pair(pair_name=order.pair)
+        pair = self.get_pair(pair_name=order.pair_name)
 
         match order.order_side:
             case OrderSide.BUY:
                 transaction_receipt = self.market.offer(
                     pay_amt=pair.quote_asset.to_integer(order.price * order.size),
                     pay_gem=pair.quote_asset.address,
                     buy_amt=pair.base_asset.to_integer(order.size),
@@ -537,15 +545,23 @@
                     buy_amt=pair.quote_asset.to_integer(order.price * order.size),
                     buy_gem=pair.quote_asset.address,
                     **transaction.args(),
                 )
             case _:
                 raise Exception("OrderSide must be BUY or SELL")
 
-        return self._handle_transaction_receipt_raw_events(transaction_receipt)
+        processed_transaction_receipt = self._handle_transaction_receipt_raw_events(
+            transaction_receipt
+        )
+
+        self._update_active_limit_orders(
+            order_events=processed_transaction_receipt.events
+        )
+
+        return processed_transaction_receipt
 
     def cancel_limit_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a limit order cancel transaction by executing the specified transaction object. The transaction object
         should contain a single order of type NewCancelOrder.
 
         :param transaction: Transaction object containing the cancel order.
         :type transaction: Transaction
@@ -558,15 +574,23 @@
 
         order: NewCancelOrder = transaction.orders[0]  # noqa
 
         transaction_receipt = self.market.cancel(
             id=order.order_id, **transaction.args()
         )
 
-        return self._handle_transaction_receipt_raw_events(transaction_receipt)
+        processed_transaction_receipt = self._handle_transaction_receipt_raw_events(
+            transaction_receipt
+        )
+
+        self._update_active_limit_orders(
+            order_events=processed_transaction_receipt.events
+        )
+
+        return processed_transaction_receipt
 
     def batch_place_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Place multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit orders.
         :type transaction: Transaction
         :return: The transaction receipt of the executed batch limit orders.
@@ -575,15 +599,15 @@
         pay_amts = []
         pay_gems = []
         buy_amts = []
         buy_gems = []
 
         for order in transaction.orders:
             order: NewLimitOrder
-            pair = self.get_pair(order.pair)
+            pair = self.get_pair(order.pair_name)
 
             match order.order_side:
                 case OrderSide.BUY:
                     pay_amts.append(
                         pair.quote_asset.to_integer(order.price * order.size)
                     )
                     pay_gems.append(pair.quote_asset.address)
@@ -601,15 +625,23 @@
             pay_amts=pay_amts,
             pay_gems=pay_gems,
             buy_amts=buy_amts,
             buy_gems=buy_gems,
             **transaction.args(),
         )
 
-        return self._handle_transaction_receipt_raw_events(transaction_receipt)
+        processed_transaction_receipt = self._handle_transaction_receipt_raw_events(
+            transaction_receipt
+        )
+
+        self._update_active_limit_orders(
+            order_events=processed_transaction_receipt.events
+        )
+
+        return processed_transaction_receipt
 
     def batch_update_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Update multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit order updates.
         :type transaction: Transaction
         :return: The transaction receipt of the executed batch limit order updates.
@@ -619,15 +651,15 @@
         pay_amts = []
         pay_gems = []
         buy_amts = []
         buy_gems = []
 
         for order in transaction.orders:
             order: UpdateLimitOrder
-            pair = self.get_pair(order.pair)
+            pair = self.get_pair(order.pair_name)
 
             order_ids.append(order.order_id)
 
             match order.order_side:
                 case OrderSide.BUY:
                     pay_amts.append(
                         pair.quote_asset.to_integer(order.price * order.size)
@@ -648,15 +680,23 @@
             pay_amts=pay_amts,
             pay_gems=pay_gems,
             buy_amts=buy_amts,
             buy_gems=buy_gems,
             **transaction.args(),
         )
 
-        return self._handle_transaction_receipt_raw_events(transaction_receipt)
+        processed_transaction_receipt = self._handle_transaction_receipt_raw_events(
+            transaction_receipt
+        )
+
+        self._update_active_limit_orders(
+            order_events=processed_transaction_receipt.events
+        )
+
+        return processed_transaction_receipt
 
     def batch_cancel_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Cancel multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit order cancellations.
         :type transaction: Transaction
         :return: The transaction receipt of the executed batch limit order cancellations.
@@ -669,15 +709,23 @@
 
             order_ids.append(order.order_id)
 
         transaction_receipt = self.market.batch_cancel(
             ids=order_ids, **transaction.args()
         )
 
-        return self._handle_transaction_receipt_raw_events(transaction_receipt)
+        processed_transaction_receipt = self._handle_transaction_receipt_raw_events(
+            transaction_receipt
+        )
+
+        self._update_active_limit_orders(
+            order_events=processed_transaction_receipt.events
+        )
+
+        return processed_transaction_receipt
 
     ######################################################################
     # data methods
     ######################################################################
 
     # TODO: i would like to remove pay_gem and buy_gem and follow the same pattern as the get_trades method but do not want to cause breaking changes
     def get_offers(
@@ -783,15 +831,15 @@
             asset.approve(
                 spender=spender, amount=asset.to_integer(number=new_allowance)
             )
         )
 
     # TODO: implement this and use check transactions before they go through to prevent failure
     @staticmethod
-    def _check_allowance(pair: Pair, order: BaseNewOrder):
+    def _check_allowance(pair: Pair, order: BaseOrder):
         pass
 
     def _handle_transaction_receipt_raw_events(
         self, transaction_receipt: TransactionReceipt
     ) -> TransactionReceipt:
         """
         Transforms the raw transaction receipt events to human-readable events
@@ -831,7 +879,46 @@
                         pair=event_pair, event=raw_event, wallet=self.wallet
                     )
                 )
 
         transaction_receipt.set_events(events=events)
 
         return transaction_receipt
+
+    def _update_active_limit_orders(self, order_events: List[OrderEvent]) -> None:
+        for order_event in order_events:
+            order_event: OrderEvent
+            if order_event.limit_order_owner != self.wallet:
+                continue
+
+            match order_event.order_type:
+                case OrderType.LIMIT:
+                    if self.active_limit_orders.get(order_event.limit_order_id):
+                        # If we are already tracking the order then don't add it again
+                        continue
+
+                    self.active_limit_orders[
+                        order_event.limit_order_id
+                    ] = ActiveLimitOrder.from_order_event(order_event=order_event)
+                case OrderType.LIMIT_TAKEN:
+                    taken_order = self.active_limit_orders[order_event.limit_order_id]
+
+                    if taken_order.remaining_size - order_event.size <= Decimal("0"):
+                        self._delete_active_limit_order(
+                            order_id=order_event.limit_order_id
+                        )
+                    else:
+                        self.active_limit_orders[
+                            order_event.limit_order_id
+                        ].update_with_take(order_event=order_event)
+                case OrderType.CANCEL:
+                    self._delete_active_limit_order(order_id=order_event.limit_order_id)
+                case OrderType.LIMIT_DELETED:
+                    self._delete_active_limit_order(order_id=order_event.limit_order_id)
+
+    def _delete_active_limit_order(self, order_id: int) -> None:
+        try:
+            del self.active_limit_orders[order_id]
+        except KeyError:
+            log.debug(
+                f"Limit order {order_id} already removed from active limit orders."
+            )
```

### Comparing `rubi-2.3.1/rubi/contracts/base_contract.py` & `rubi-2.4.0/rubi/contracts/base_contract.py`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/rubi/contracts/contract_types/events.py` & `rubi-2.4.0/rubi/contracts/contract_types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.4.0/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/rubi/contracts/erc20.py` & `rubi-2.4.0/rubi/contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/rubi/contracts/market.py` & `rubi-2.4.0/rubi/contracts/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/rubi/contracts/router.py` & `rubi-2.4.0/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/rubi/data/market.py` & `rubi-2.4.0/rubi/data/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/rubi/network/network.py` & `rubi-2.4.0/rubi/network/network.py`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/rubi/rubicon_types/order.py` & `rubi-2.4.0/rubi/rubicon_types/order.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     # Only used for events coming from the RubiconMarket
     LIMIT_TAKEN = "LIMIT_TAKEN"
     LIMIT_DELETED = "LIMIT_DELETED"
     CANCEL = "CANCEL"
 
 
-class BaseNewOrder:
+class BaseOrder:
     """Base class for representing a new order.
 
     :param pair_name: The name of the trading pair.
     :type pair_name: str
     :param order_type: The type of the order.
     :type order_type: OrderType
     :param order_side: The side of the order (buy or sell).
@@ -75,20 +75,20 @@
     def __init__(
         self,
         pair_name: str,
         order_type: OrderType,
         order_side: OrderSide,
     ):
         """constructor method."""
-        self.pair = pair_name
+        self.pair_name = pair_name
         self.order_side = order_side
         self.order_type = order_type
 
 
-class NewMarketOrder(BaseNewOrder):
+class NewMarketOrder(BaseOrder):
     """Class representing a new market order.
 
     :param pair_name: The name of the pair being traded e.g. WETH/USDC.
     :type pair_name: str
     :param order_side: The side of the order (BUY or SELL).
     :type order_side: OrderSide
     :param size: The size of the order.
@@ -118,15 +118,15 @@
             self.worst_execution_price = (
                 Decimal("0") if order_side.SELL else Decimal("10") ** Decimal("7")
             )
         else:
             self.worst_execution_price = worst_execution_price
 
 
-class NewLimitOrder(BaseNewOrder):
+class NewLimitOrder(BaseOrder):
     """Class representing a new limit order
 
     :param pair_name: The name of the pair being traded e.g. WETH/USDC.
     :type pair_name: str
     :param order_side: The side of the order (buy or sell).
     :type order_side: OrderSide
     :param size: The size of the order.
@@ -149,15 +149,15 @@
         self.price = price
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
 
 
-class UpdateLimitOrder(BaseNewOrder):
+class UpdateLimitOrder(BaseOrder):
     """Class representing an update to an existing limit order
 
     :param pair_name: The name of the pair being traded e.g. WETH/USDC.
     :type pair_name: str
     :param order_side: The side of the order (BUY or SELL).
     :type order_side: OrderSide
     :param order_id: The ID of the order to update.
@@ -184,15 +184,83 @@
         )
 
         self.order_id = order_id
         self.size = size
         self.price = price
 
 
-class NewCancelOrder(BaseNewOrder):
+class ActiveLimitOrder(BaseOrder):
+    """Class representing an existing limit order
+
+    :param pair_name: The name of the pair being traded e.g. WETH/USDC.
+    :type pair_name: str
+    :param order_side: The side of the order (BUY or SELL).
+    :type order_side: OrderSide
+    :param order_id: The ID of the order to update.
+    :type order_id: int
+    :param order_owner: The address of the owner of the order
+    :type order_owner: ChecksumAddress
+    :param size: The updated size of the order.
+    :type size: Decimal
+    :param price: The updated price of the order.
+    :type price: Decimal
+    :param filled_size: The amount of the order that has been filled
+    :type filled_size: Decimal
+    """
+
+    def __init__(
+        self,
+        pair_name: str,
+        order_side: OrderSide,
+        order_id: int,
+        order_owner: ChecksumAddress,
+        size: Decimal,
+        price: Decimal,
+        filled_size: Decimal = Decimal("0"),
+    ):
+        """constructor method"""
+        super().__init__(
+            pair_name=pair_name,
+            order_type=OrderType.LIMIT,
+            order_side=order_side,
+        )
+
+        self.order_id = order_id
+        self.order_owner = order_owner
+        self.size = size
+        self.price = price
+        self.filled_size = filled_size
+
+    @property
+    def remaining_size(self) -> Decimal:
+        return self.size - self.filled_size
+
+    @classmethod
+    def from_order_event(cls, order_event: "OrderEvent") -> "ActiveLimitOrder":
+        if order_event.order_type != OrderType.LIMIT:
+            raise Exception("event must have LIMIT as order_type.")
+
+        return cls(
+            pair_name=order_event.pair_name,
+            order_side=order_event.order_side,
+            order_id=order_event.limit_order_id,
+            order_owner=order_event.limit_order_owner,
+            size=order_event.size,
+            price=order_event.price,
+        )
+
+    def update_with_take(self, order_event: "OrderEvent"):
+        self.filled_size += order_event.size
+
+    def __repr__(self):
+        items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
+        return "{}({})".format(type(self).__name__, ", ".join(items))
+
+
+class NewCancelOrder(BaseOrder):
     """Class representing a limit order cancellation
 
     :param pair_name: The name of the trading pair.
     :type pair_name: str
     :param order_id: The ID of the order to cancel.
     :type order_id: int
     """
@@ -204,36 +272,33 @@
             order_type=OrderType.LIMIT,
             order_side=OrderSide.NEUTRAL,
         )
 
         self.order_id = order_id
 
 
-# TODO: add a new class for a limit order object that is returned from the subgraph
-
-
 class Transaction:
     """
     Class representing a transaction to be executed on chain
 
     :param orders: The list of orders to include in the transaction.
-    :type orders: List[BaseNewOrder]
+    :type orders: List[BaseOrder]
     :param nonce: The nonce for the transaction (optional).
     :type nonce: int
     :param gas: The gas limit for the transaction (optional).
     :type gas: int
     :param max_fee_per_gas: The maximum fee per gas for the transaction (optional).
     :type max_fee_per_gas: int
     :param max_priority_fee_per_gas: The maximum priority fee per gas for the transaction (optional).
     :type max_priority_fee_per_gas: int
     """
 
     def __init__(
         self,
-        orders: List[BaseNewOrder],
+        orders: List[BaseOrder],
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None,
     ):
         """constructor method"""
         if len(orders) < 1:
```

### Comparing `rubi-2.3.1/rubi/rubicon_types/order_query.py` & `rubi-2.4.0/rubi/rubicon_types/order_query.py`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/rubi/rubicon_types/orderbook.py` & `rubi-2.4.0/rubi/rubicon_types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/rubi/rubicon_types/pair.py` & `rubi-2.4.0/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/rubi/rubicon_types/trade_query.py` & `rubi-2.4.0/rubi/rubicon_types/trade_query.py`

 * *Files identical despite different names*

### Comparing `rubi-2.3.1/PKG-INFO` & `rubi-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.3.1
+Version: 2.4.0
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

