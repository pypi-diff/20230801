# Comparing `tmp/pyln_client-23.5.2.tar.gz` & `tmp/pyln_client-23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyln_client-23.5.2.tar", max compression
+gzip compressed data, was "pyln_client-23.8.tar", max compression
```

## Comparing `pyln_client-23.5.2.tar` & `pyln_client-23.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2939 2023-06-22 04:17:49.576864 pyln_client-23.5.2/README.md
--rw-r--r--   0        0        0      575 2023-06-29 17:58:23.259200 pyln_client-23.5.2/pyln/client/__init__.py
--rw-r--r--   0        0        0      889 2023-06-06 02:30:27.767370 pyln_client-23.5.2/pyln/client/clnutils.py
--rwxr-xr-x   0        0        0    26412 2023-06-22 04:17:49.576864 pyln_client-23.5.2/pyln/client/gossmap.py
--rw-r--r--   0        0        0    14744 2023-06-22 04:17:49.576864 pyln_client-23.5.2/pyln/client/gossmapstats.py
--rw-r--r--   0        0        0    53256 2023-06-29 17:58:23.259200 pyln_client-23.5.2/pyln/client/lightning.py
--rw-r--r--   0        0        0    38901 2023-06-29 17:58:23.259200 pyln_client-23.5.2/pyln/client/plugin.py
--rw-r--r--   0        0        0      617 2023-06-29 17:58:23.259200 pyln_client-23.5.2/pyproject.toml
--rw-r--r--   0        0        0     3734 1970-01-01 00:00:00.000000 pyln_client-23.5.2/setup.py
--rw-r--r--   0        0        0     3628 1970-01-01 00:00:00.000000 pyln_client-23.5.2/PKG-INFO
+-rw-r--r--   0        0        0     2940 2023-07-31 03:58:40.620735 pyln_client-23.8/README.md
+-rw-r--r--   0        0        0      573 2023-08-01 02:07:55.693063 pyln_client-23.8/pyln/client/__init__.py
+-rw-r--r--   0        0        0      889 2023-07-24 03:49:44.217083 pyln_client-23.8/pyln/client/clnutils.py
+-rwxr-xr-x   0        0        0    26412 2023-07-31 02:10:42.119109 pyln_client-23.8/pyln/client/gossmap.py
+-rw-r--r--   0        0        0    14744 2023-07-31 02:10:42.119109 pyln_client-23.8/pyln/client/gossmapstats.py
+-rw-r--r--   0        0        0    54408 2023-07-31 19:30:05.934942 pyln_client-23.8/pyln/client/lightning.py
+-rw-r--r--   0        0        0    39073 2023-07-31 03:58:40.624735 pyln_client-23.8/pyln/client/plugin.py
+-rw-r--r--   0        0        0      609 2023-08-01 02:07:55.649062 pyln_client-23.8/pyproject.toml
+-rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 pyln_client-23.8/setup.py
+-rw-r--r--   0        0        0     3575 1970-01-01 00:00:00.000000 pyln_client-23.8/PKG-INFO
```

### Comparing `pyln_client-23.5.2/README.md` & `pyln_client-23.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 def init(options, configuration, plugin):
     plugin.log("Plugin helloworld.py initialized")
     # This can also return {'disabled': <reason>} to self-disable,
 	# but normally it returns None.
 
 
 @plugin.subscribe("connect")
-def on_connect(plugin, id, address, **kwargs):
-    plugin.log("Received connect event for peer {}".format(id))
+def on_connect(plugin, connect, **kwargs):
+    plugin.log("Received connect event for peer {}".format(connect))
 
 
 plugin.add_option('greeting', 'Hello', 'The greeting I should use.')
 plugin.run()
 
 ```
```

### Comparing `pyln_client-23.5.2/pyln/client/__init__.py` & `pyln_client-23.8/pyln/client/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .lightning import LightningRpc, RpcError, Millisatoshi
 from .plugin import Plugin, monkey_patch, RpcException
 from .gossmap import Gossmap, GossmapNode, GossmapChannel, GossmapHalfchannel, GossmapNodeId, LnFeatureBits
 from .gossmapstats import GossmapStats
 
-__version__ = "23.05.2"
+__version__ = "23.08"
 
 __all__ = [
     "LightningRpc",
     "Plugin",
     "RpcError",
     "RpcException",
     "Millisatoshi",
```

### Comparing `pyln_client-23.5.2/pyln/client/clnutils.py` & `pyln_client-23.8/pyln/client/clnutils.py`

 * *Files identical despite different names*

### Comparing `pyln_client-23.5.2/pyln/client/gossmap.py` & `pyln_client-23.8/pyln/client/gossmap.py`

 * *Files identical despite different names*

### Comparing `pyln_client-23.5.2/pyln/client/gossmapstats.py` & `pyln_client-23.8/pyln/client/gossmapstats.py`

 * *Files identical despite different names*

### Comparing `pyln_client-23.5.2/pyln/client/lightning.py` & `pyln_client-23.8/pyln/client/lightning.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,14 +506,15 @@
                     # Objects ending in msat are not treated specially!
                     if k.endswith('msat') and not isinstance(v, dict):
                         if isinstance(v, list):
                             obj[k] = [Millisatoshi(e) for e in v]
                         # FIXME: Deprecated "listconfigs" gives two 'null' fields:
                         #            "lease-fee-base-msat": null,
                         #            "channel-fee-max-base-msat": null,
+                        # FIXME: Removed for v23.08, delete this code in 24.08?
                         elif v is None:
                             obj[k] = None
                         else:
                             obj[k] = Millisatoshi(v)
                     else:
                         obj[k] = LightningRpc.LightningJSONDecoder.replace_amounts(v)
             elif isinstance(obj, list):
@@ -1018,26 +1019,29 @@
 
     def listtransactions(self):
         """
         Show wallet history.
         """
         return self.call("listtransactions")
 
-    def listinvoices(self, label=None, payment_hash=None, invstring=None, offer_id=None):
+    def listinvoices(self, label=None, payment_hash=None, invstring=None, offer_id=None, index=None, start=None, limit=None):
         """Query invoices
 
         Show invoice matching {label}, {payment_hash}, {invstring} or {offer_id}
         (or all, if no filters are present).
 
         """
         payload = {
             "label": label,
             "payment_hash": payment_hash,
             "invstring": invstring,
             "offer_id": offer_id,
+            "index": index,
+            "start": start,
+            "limit": limit,
         }
         return self.call("listinvoices", payload)
 
     def listnodes(self, node_id=None):
         """
         Show all nodes in our local network view, filter on node {id}
         if provided.
@@ -1204,14 +1208,40 @@
     def openchannel_abort(self, channel_id):
         """ Abort a channel open """
         payload = {
             "channel_id": channel_id,
         }
         return self.call("openchannel_abort", payload)
 
+    def splice_init(self, chan_id, amount, initialpsbt=None, feerate_per_kw=None):
+        """ Initiate a splice """
+        payload = {
+            "channel_id": chan_id,
+            "relative_amount": amount,
+            "initialpsbt": initialpsbt,
+            "feerate_per_kw": feerate_per_kw,
+        }
+        return self.call("splice_init", payload)
+
+    def splice_update(self, chan_id, psbt):
+        """ Update a splice """
+        payload = {
+            "channel_id": chan_id,
+            "psbt": psbt
+        }
+        return self.call("splice_update", payload)
+
+    def splice_signed(self, chan_id, psbt):
+        """ Initiate a splice """
+        payload = {
+            "channel_id": chan_id,
+            "psbt": psbt
+        }
+        return self.call("splice_signed", payload)
+
     def paystatus(self, bolt11=None):
         """Detail status of attempts to pay {bolt11} or any."""
         payload = {
             "bolt11": bolt11
         }
         return self.call("paystatus", payload)
 
@@ -1316,15 +1346,15 @@
             "partid": partid,
             "bolt11": bolt11,
             "amount_msat": amount_msat,
             "destination": destination,
         }
         return self.call("sendonion", payload)
 
-    def setchannel(self, id, feebase=None, feeppm=None, htlcmin=None, htlcmax=None, enforcedelay=None):
+    def setchannel(self, id, feebase=None, feeppm=None, htlcmin=None, htlcmax=None, enforcedelay=None, ignorefeelimits=None):
         """Set configuration a channel/peer {id} (or 'all').
 
         {feebase} is a value in millisatoshi that is added as base fee
         to any routed payment.
 
         {feeppm} is a value added proportionally per-millionths to any
         routed payment volume in satoshi.
@@ -1334,22 +1364,25 @@
 
         {htlcmax} is the maximum (outgoing) htlc amount to allow and
         advertize.
 
         {enforcedelay} is the number of seconds before enforcing this
         change.
 
+        {ignorefeelimits} is a flag to indicate peer can set any feerate (dangerous!)
+
         """
         payload = {
             "id": id,
             "feebase": feebase,
             "feeppm": feeppm,
             "htlcmin": htlcmin,
             "htlcmax": htlcmax,
             "enforcedelay": enforcedelay,
+            "ignorefeelimits": ignorefeelimits,
         }
         return self.call("setchannel", payload)
 
     def stop(self):
         """
         Shut down the lightningd process.
         """
```

### Comparing `pyln_client-23.5.2/pyln/client/plugin.py` & `pyln_client-23.8/pyln/client/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -655,18 +655,21 @@
 
                 request.set_result(response)
             else:
                 request.set_exception(e)
             self.log(traceback.format_exc())
 
     def _dispatch_notification(self, request: Request) -> None:
-        if request.method not in self.subscriptions:
-            raise ValueError("No subscription for {name} found.".format(
-                name=request.method))
-        func = self.subscriptions[request.method]
+        if request.method in self.subscriptions:
+            func = self.subscriptions[request.method]
+        # Wildcard 'all' subscriptions using asterisk
+        elif '*' in self.subscriptions:
+            func = self.subscriptions['*']
+        else:
+            raise ValueError(f"No subscription for {request.method} found.")
 
         try:
             self._exec_func(func, request)
         except Exception:
             self.log(traceback.format_exc())
 
     def _write_locked(self, obj: JSONType) -> None:
@@ -908,15 +911,15 @@
                 'description': doc if not method.desc else method.desc
             })
             if method.long_desc:
                 m = methods[len(methods) - 1]
                 m["long_description"] = method.long_desc
 
         manifest = {
-            'options': list(self.options.values()),
+            'options': list({k: v for k, v in d.items() if v is not None} for d in self.options.values()),
             'rpcmethods': methods,
             'subscriptions': list(self.subscriptions.keys()),
             'hooks': hooks,
             'dynamic': self.dynamic,
             'nonnumericids': True,
             'notifications': [
                 {"method": name} for name in self.notification_topics
```

### Comparing `pyln_client-23.5.2/pyproject.toml` & `pyln_client-23.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "pyln-client"
-version = "23.05.2"
+version = "23.08"
 description = "Client library and plugin library for Core Lightning"
 authors = ["Christian Decker <decker.christian@gmail.com>"]
 license = "BSD-MIT"
 readme = "README.md"
 
 packages = [
   { include = "pyln/client" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pyln-proto = ">=0.12"
+python = "^3.8"
+pyln-proto = ">=23"
 pyln-bolt7 = ">=1.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0.1"
+pytest = "^7"
 pyln-bolt7 = { path = "../pyln-spec/bolt7", develop = true }
 pyln-proto = { path = "../pyln-proto", develop = true}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyln_client-23.5.2/setup.py` & `pyln_client-23.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['client']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pyln-bolt7>=1.0', 'pyln-proto>=0.12']
+['pyln-bolt7>=1.0', 'pyln-proto>=23']
 
 setup_kwargs = {
     'name': 'pyln-client',
-    'version': '23.5.2',
+    'version': '23.8',
     'description': 'Client library and plugin library for Core Lightning',
-    'long_description': '# pyln-client: A python client library for lightningd\n\nThis package implements the Unix socket based JSON-RPC protocol that\n`lightningd` exposes to the rest of the world. It can be used to call\narbitrary functions on the RPC interface, and serves as a basis for plugins\nwritten in python.\n\n\n## Installation\n\n`pyln-client` is available on `pip`:\n\n```\npip install pyln-client\n```\n\nAlternatively you can also install the development version to get access to\ncurrently unreleased features by checking out the Core Lightning source code and\ninstalling into your python3 environment:\n\n```bash\ngit clone https://github.com/ElementsProject/lightning.git\ncd lightning/contrib/pyln-client\npoetry install\n```\n\nThis will add links to the library into your environment so changing the\nchecked out source code will also result in the environment picking up these\nchanges. Notice however that unreleased versions may change API without\nwarning, so test thoroughly with the released version.\n\n## Examples\n\n\n### Using the JSON-RPC client\n```py\n"""\nGenerate invoice on one daemon and pay it on the other\n"""\nfrom pyln.client import LightningRpc\nimport random\n\n# Create two instances of the LightningRpc object using two different Core Lightning daemons on your computer\nl1 = LightningRpc("/tmp/lightning1/lightning-rpc")\nl5 = LightningRpc("/tmp/lightning5/lightning-rpc")\n\ninfo5 = l5.getinfo()\nprint(info5)\n\n# Create invoice for test payment\ninvoice = l5.invoice(100, "lbl{}".format(random.random()), "testpayment")\nprint(invoice)\n\n# Get route to l1\nroute = l1.getroute(info5[\'id\'], 100, 1)\nprint(route)\n\n# Pay invoice\nprint(l1.sendpay(route[\'route\'], invoice[\'payment_hash\']))\n```\n\n### Writing a plugin\n\nPlugins are programs that `lightningd` can be configured to execute alongside\nthe main daemon. They allow advanced interactions with and customizations to\nthe daemon.\n\n```python\n#!/usr/bin/env python3\nfrom pyln.client import Plugin\n\nplugin = Plugin()\n\n@plugin.method("hello")\ndef hello(plugin, name="world"):\n    """This is the documentation string for the hello-function.\n\n    It gets reported as the description when registering the function\n    as a method with `lightningd`.\n\n    If this returns (a dict), that\'s the JSON "result" returned.  If\n    it raises an exception, that causes a JSON "error" return (raising\n    pyln.client.RpcException allows finer control over the return).\n    """\n    greeting = plugin.get_option(\'greeting\')\n    s = \'{} {}\'.format(greeting, name)\n    plugin.log(s)\n    return s\n\n\n@plugin.init()\ndef init(options, configuration, plugin):\n    plugin.log("Plugin helloworld.py initialized")\n    # This can also return {\'disabled\': <reason>} to self-disable,\n\t# but normally it returns None.\n\n\n@plugin.subscribe("connect")\ndef on_connect(plugin, id, address, **kwargs):\n    plugin.log("Received connect event for peer {}".format(id))\n\n\nplugin.add_option(\'greeting\', \'Hello\', \'The greeting I should use.\')\nplugin.run()\n\n```\n',
+    'long_description': '# pyln-client: A python client library for lightningd\n\nThis package implements the Unix socket based JSON-RPC protocol that\n`lightningd` exposes to the rest of the world. It can be used to call\narbitrary functions on the RPC interface, and serves as a basis for plugins\nwritten in python.\n\n\n## Installation\n\n`pyln-client` is available on `pip`:\n\n```\npip install pyln-client\n```\n\nAlternatively you can also install the development version to get access to\ncurrently unreleased features by checking out the Core Lightning source code and\ninstalling into your python3 environment:\n\n```bash\ngit clone https://github.com/ElementsProject/lightning.git\ncd lightning/contrib/pyln-client\npoetry install\n```\n\nThis will add links to the library into your environment so changing the\nchecked out source code will also result in the environment picking up these\nchanges. Notice however that unreleased versions may change API without\nwarning, so test thoroughly with the released version.\n\n## Examples\n\n\n### Using the JSON-RPC client\n```py\n"""\nGenerate invoice on one daemon and pay it on the other\n"""\nfrom pyln.client import LightningRpc\nimport random\n\n# Create two instances of the LightningRpc object using two different Core Lightning daemons on your computer\nl1 = LightningRpc("/tmp/lightning1/lightning-rpc")\nl5 = LightningRpc("/tmp/lightning5/lightning-rpc")\n\ninfo5 = l5.getinfo()\nprint(info5)\n\n# Create invoice for test payment\ninvoice = l5.invoice(100, "lbl{}".format(random.random()), "testpayment")\nprint(invoice)\n\n# Get route to l1\nroute = l1.getroute(info5[\'id\'], 100, 1)\nprint(route)\n\n# Pay invoice\nprint(l1.sendpay(route[\'route\'], invoice[\'payment_hash\']))\n```\n\n### Writing a plugin\n\nPlugins are programs that `lightningd` can be configured to execute alongside\nthe main daemon. They allow advanced interactions with and customizations to\nthe daemon.\n\n```python\n#!/usr/bin/env python3\nfrom pyln.client import Plugin\n\nplugin = Plugin()\n\n@plugin.method("hello")\ndef hello(plugin, name="world"):\n    """This is the documentation string for the hello-function.\n\n    It gets reported as the description when registering the function\n    as a method with `lightningd`.\n\n    If this returns (a dict), that\'s the JSON "result" returned.  If\n    it raises an exception, that causes a JSON "error" return (raising\n    pyln.client.RpcException allows finer control over the return).\n    """\n    greeting = plugin.get_option(\'greeting\')\n    s = \'{} {}\'.format(greeting, name)\n    plugin.log(s)\n    return s\n\n\n@plugin.init()\ndef init(options, configuration, plugin):\n    plugin.log("Plugin helloworld.py initialized")\n    # This can also return {\'disabled\': <reason>} to self-disable,\n\t# but normally it returns None.\n\n\n@plugin.subscribe("connect")\ndef on_connect(plugin, connect, **kwargs):\n    plugin.log("Received connect event for peer {}".format(connect))\n\n\nplugin.add_option(\'greeting\', \'Hello\', \'The greeting I should use.\')\nplugin.run()\n\n```\n',
     'author': 'Christian Decker',
     'author_email': 'decker.christian@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pyln_client-23.5.2/PKG-INFO` & `pyln_client-23.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pyln-client
-Version: 23.5.2
+Version: 23.8
 Summary: Client library and plugin library for Core Lightning
 License: BSD-MIT
 Author: Christian Decker
 Author-email: decker.christian@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyln-bolt7 (>=1.0)
-Requires-Dist: pyln-proto (>=0.12)
+Requires-Dist: pyln-proto (>=23)
 Description-Content-Type: text/markdown
 
 # pyln-client: A python client library for lightningd
 
 This package implements the Unix socket based JSON-RPC protocol that
 `lightningd` exposes to the rest of the world. It can be used to call
 arbitrary functions on the RPC interface, and serves as a basis for plugins
@@ -111,16 +110,16 @@
 def init(options, configuration, plugin):
     plugin.log("Plugin helloworld.py initialized")
     # This can also return {'disabled': <reason>} to self-disable,
 	# but normally it returns None.
 
 
 @plugin.subscribe("connect")
-def on_connect(plugin, id, address, **kwargs):
-    plugin.log("Received connect event for peer {}".format(id))
+def on_connect(plugin, connect, **kwargs):
+    plugin.log("Received connect event for peer {}".format(connect))
 
 
 plugin.add_option('greeting', 'Hello', 'The greeting I should use.')
 plugin.run()
 
 ```
```

