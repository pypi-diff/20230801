# Comparing `tmp/polywrap_core-0.1.0a8.tar.gz` & `tmp/polywrap_core-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_core-0.1.0a8.tar", max compression
+gzip compressed data, was "polywrap_core-0.1.0b1.tar", max compression
```

## Comparing `polywrap_core-0.1.0a8.tar` & `polywrap_core-0.1.0b1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0       98 2023-02-22 15:57:14.692017 polywrap_core-0.1.0a8/polywrap_core/__init__.py
--rw-r--r--   0        0        0       38 2023-02-22 15:57:14.692337 polywrap_core-0.1.0a8/polywrap_core/algorithms/__init__.py
--rw-r--r--   0        0        0     2392 2023-02-22 15:57:14.692494 polywrap_core-0.1.0a8/polywrap_core/algorithms/build_clean_uri_history.py
--rw-r--r--   0        0        0      360 2023-02-22 15:57:14.692622 polywrap_core-0.1.0a8/polywrap_core/types/__init__.py
--rw-r--r--   0        0        0     1542 2023-02-24 15:43:21.891062 polywrap_core-0.1.0a8/polywrap_core/types/client.py
--rw-r--r--   0        0        0       51 2023-02-22 15:57:14.693626 polywrap_core-0.1.0a8/polywrap_core/types/env.py
--rw-r--r--   0        0        0      231 2023-02-22 15:57:14.693388 polywrap_core-0.1.0a8/polywrap_core/types/file_reader.py
--rw-r--r--   0        0        0     1799 2023-02-24 15:43:21.891664 polywrap_core-0.1.0a8/polywrap_core/types/invoke.py
--rw-r--r--   0        0        0     3475 2023-02-22 15:57:14.693549 polywrap_core-0.1.0a8/polywrap_core/types/uri.py
--rw-r--r--   0        0        0      208 2023-02-24 15:43:21.891172 polywrap_core-0.1.0a8/polywrap_core/types/uri_package_wrapper.py
--rw-r--r--   0        0        0      913 2023-02-22 15:57:14.693710 polywrap_core-0.1.0a8/polywrap_core/types/uri_resolution_context.py
--rw-r--r--   0        0        0      479 2023-02-22 15:57:14.694476 polywrap_core-0.1.0a8/polywrap_core/types/uri_resolution_step.py
--rw-r--r--   0        0        0     1086 2023-02-24 15:43:21.891479 polywrap_core-0.1.0a8/polywrap_core/types/uri_resolver.py
--rw-r--r--   0        0        0      446 2023-02-22 15:57:14.694185 polywrap_core-0.1.0a8/polywrap_core/types/uri_resolver_handler.py
--rw-r--r--   0        0        0      240 2023-02-22 15:57:14.694258 polywrap_core-0.1.0a8/polywrap_core/types/wasm_package.py
--rw-r--r--   0        0        0      485 2023-02-24 15:43:21.891784 polywrap_core-0.1.0a8/polywrap_core/types/wrap_package.py
--rw-r--r--   0        0        0      900 2023-02-24 15:43:21.892094 polywrap_core-0.1.0a8/polywrap_core/types/wrapper.py
--rw-r--r--   0        0        0       38 2023-02-22 15:57:14.694627 polywrap_core-0.1.0a8/polywrap_core/uri_resolution/__init__.py
--rw-r--r--   0        0        0     1675 2022-12-09 10:57:58.160601 polywrap_core-0.1.0a8/polywrap_core/uri_resolution/uri_resolution_context.py
--rw-r--r--   0        0        0      122 2022-12-10 08:39:18.501105 polywrap_core-0.1.0a8/polywrap_core/utils/__init__.py
--rw-r--r--   0        0        0      254 2023-02-22 15:57:14.694748 polywrap_core-0.1.0a8/polywrap_core/utils/get_env_from_uri_history.py
--rw-r--r--   0        0        0      246 2022-12-09 10:18:25.573666 polywrap_core-0.1.0a8/polywrap_core/utils/init_wrapper.py
--rw-r--r--   0        0        0      125 2022-10-16 06:28:28.766955 polywrap_core-0.1.0a8/polywrap_core/utils/instance_of.py
--rw-r--r--   0        0        0      438 2022-10-16 06:28:28.767147 polywrap_core-0.1.0a8/polywrap_core/utils/maybe_async.py
--rw-r--r--   0        0        0     1064 2023-03-02 20:07:34.919806 polywrap_core-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 polywrap_core-0.1.0a8/setup.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 polywrap_core-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0      132 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/py.typed
+-rw-r--r--   0        0        0      589 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/__init__.py
+-rw-r--r--   0        0        0      147 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/clean_resolution_step.py
+-rw-r--r--   0        0        0     2292 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/client.py
+-rw-r--r--   0        0        0      869 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/config.py
+-rw-r--r--   0        0        0     3980 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/errors.py
+-rw-r--r--   0        0        0      560 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/file_reader.py
+-rw-r--r--   0        0        0     1847 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/invocable.py
+-rw-r--r--   0        0        0      859 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/invoke_options.py
+-rw-r--r--   0        0        0     1716 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/invoker.py
+-rw-r--r--   0        0        0      411 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/invoker_client.py
+-rw-r--r--   0        0        0     5822 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri.py
+-rw-r--r--   0        0        0      553 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_package.py
+-rw-r--r--   0        0        0      837 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_package_wrapper.py
+-rw-r--r--   0        0        0     3668 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_resolution_context.py
+-rw-r--r--   0        0        0      822 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_resolution_step.py
+-rw-r--r--   0        0        0      989 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_resolver.py
+-rw-r--r--   0        0        0      752 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_resolver_handler.py
+-rw-r--r--   0        0        0      458 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_wrapper.py
+-rw-r--r--   0        0        0      936 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/wrap_package.py
+-rw-r--r--   0        0        0      866 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/wrapper.py
+-rw-r--r--   0        0        0      204 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/utils/__init__.py
+-rw-r--r--   0        0        0     2343 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/utils/build_clean_uri_history.py
+-rw-r--r--   0        0        0      712 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/utils/get_env_from_resolution_path.py
+-rw-r--r--   0        0        0     1980 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/utils/get_implementations.py
+-rw-r--r--   0        0        0     1059 2023-08-01 17:50:15.331996 polywrap_core-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 polywrap_core-0.1.0b1/PKG-INFO
```

### Comparing `polywrap_core-0.1.0a8/polywrap_core/algorithms/build_clean_uri_history.py` & `polywrap_core-0.1.0b1/polywrap_core/utils/build_clean_uri_history.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-import traceback
-from typing import List, Optional, Union
+"""This module contains an utility function for building a clean history of URI resolution steps."""
+from typing import List, Optional
 
-from ..types import Uri, IWrapPackage, IUriResolutionStep
-
-
-CleanResolutionStep = List[Union[str, "CleanResolutionStep"]]
+from ..types import CleanResolutionStep, UriPackage, UriResolutionStep, UriWrapper
 
 
 def build_clean_uri_history(
-    history: List[IUriResolutionStep], depth: Optional[int] = None
+    history: List[UriResolutionStep], depth: Optional[int] = None
 ) -> CleanResolutionStep:
+    """Build a clean history of the URI resolution steps.
+
+    Args:
+        history (List[UriResolutionStep]): A list of URI resolution steps.
+        depth (Optional[int]): The depth of the history to build.
+
+    Returns:
+        CleanResolutionStep: A clean history of the URI resolution steps.
+    """
     clean_history: CleanResolutionStep = []
 
     if depth is not None:
         depth -= 1
 
     if not history:
         return clean_history
@@ -31,43 +37,38 @@
         sub_history = build_clean_uri_history(step.sub_history, depth)
         if len(sub_history) > 0:
             clean_history.append(sub_history)
 
     return clean_history
 
 
-def _build_clean_history_step(step: IUriResolutionStep) -> str:
-    if step.result.is_err():
-        formatted_exc = traceback.format_tb(step.result.unwrap_err().__traceback__)
-        return (
-            f"{step.source_uri} => {step.description} => error ({''.join(formatted_exc)})"
-            if step.description
-            else f"{step.source_uri} => error ({''.join(formatted_exc)})"
-        )
+def _build_clean_history_step(step: UriResolutionStep) -> str:
+    uri_package_or_wrapper = step.result
 
-    uri_package_or_wrapper = step.result.unwrap()
-
-    if isinstance(uri_package_or_wrapper, Uri):
-        if step.source_uri == uri_package_or_wrapper:
+    match uri_package_or_wrapper:
+        case UriPackage(uri=uri):
             return (
-                f"{step.source_uri} => {step.description}"
+                f"{step.source_uri} => {step.description} => package ({uri})"
                 if step.description
-                else f"{step.source_uri}"
+                else f"{step.source_uri} => package ({uri})"
             )
-        else:
+        case UriWrapper(uri=uri):
             return (
-                f"{step.source_uri} => {step.description} => uri ({uri_package_or_wrapper.uri})"
+                f"{step.source_uri} => {step.description} => wrapper ({uri})"
                 if step.description
-                else f"{step.source_uri} => uri ({uri_package_or_wrapper})"
+                else f"{step.source_uri} => wrapper ({uri})"
             )
-    elif isinstance(uri_package_or_wrapper, IWrapPackage):
-        return (
-            f"{step.source_uri} => {step.description} => package ({uri_package_or_wrapper})"
-            if step.description
-            else f"{step.source_uri} => package ({uri_package_or_wrapper})"
-        )
-    else:
-        return (
-            f"{step.source_uri} => {step.description} => wrapper ({uri_package_or_wrapper})"
-            if step.description
-            else f"{step.source_uri} => wrapper ({uri_package_or_wrapper})"
-        )
+        case uri:
+            if step.source_uri == uri:
+                return (
+                    f"{step.source_uri} => {step.description}"
+                    if step.description
+                    else f"{step.source_uri}"
+                )
+            return (
+                f"{step.source_uri} => {step.description} => uri ({uri})"
+                if step.description
+                else f"{step.source_uri} => uri ({uri})"
+            )
+
+
+__all__ = ["build_clean_uri_history"]
```

### Comparing `polywrap_core-0.1.0a8/polywrap_core/types/invoke.py` & `polywrap_core-0.1.0b1/polywrap_core/types/invocable.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,58 @@
-from __future__ import annotations
+"""This module contains the interface for invoking any invocables."""
+# pylint: disable=too-many-arguments
 
-from abc import ABC, abstractmethod
-from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, Union
+from __future__ import annotations
 
-from polywrap_result import Result
+from dataclasses import dataclass
+from typing import Any, Optional, Protocol
 
-from .env import Env
+from .invoker_client import InvokerClient
 from .uri import Uri
-from .uri_resolution_context import IUriResolutionContext
-
-
-@dataclass(slots=True, kw_only=True)
-class InvokeOptions:
-    """
-    Options required for a wrapper invocation.
-
-    Args:
-        uri: Uri of the wrapper
-        method: Method to be executed
-        args: Arguments for the method, structured as a dictionary
-        config: Override the client's config for all invokes within this invoke.
-        context_id: Invoke id used to track query context data set internally.
-    """
-
-    uri: Uri
-    method: str
-    args: Optional[Union[Dict[str, Any], bytes]] = field(default_factory=dict)
-    env: Optional[Env] = None
-    resolution_context: Optional[IUriResolutionContext] = None
+from .uri_resolution_context import UriResolutionContext
 
 
 @dataclass(slots=True, kw_only=True)
 class InvocableResult:
-    """
-    Result of a wrapper invocation
+    """Result of a wrapper invocation.
 
     Args:
-        data: Invoke result data. The type of this value is the return type of the method.
-        encoded: It will be set true if result is encoded
+        result (Any): Invocation result. The type of this value is \
+            the return type of the method.
+        encoded (Optional[bool]): It will be set true if result is encoded
     """
 
-    result: Optional[Any] = None
+    result: Any
     encoded: Optional[bool] = None
 
 
-@dataclass(slots=True, kw_only=True)
-class InvokerOptions(InvokeOptions):
-    encode_result: Optional[bool] = False
+class Invocable(Protocol):
+    """Defines Invocable protocol."""
+
+    def invoke(
+        self,
+        uri: Uri,
+        method: str,
+        args: Optional[Any] = None,
+        env: Optional[Any] = None,
+        resolution_context: Optional[UriResolutionContext] = None,
+        client: Optional[InvokerClient] = None,
+    ) -> InvocableResult:
+        """Invoke the Wrapper based on the provided InvokeOptions.
+
+        Args:
+            uri (Uri): Uri of the wrapper
+            method (str): Method to be executed
+            args (Optional[Any]) : Arguments for the method, structured as a dictionary
+            env (Optional[Any]): Override the client's config for all invokes within this invoke.
+            resolution_context (Optional[UriResolutionContext]): A URI resolution context
+            client (Optional[InvokerClient]): The invoker client instance requesting\
+                this invocation. This invoker client will be used for any subinvocation\
+                that may occur.
+
+        Returns:
+            InvocableResult: Result of the invocation.
+        """
+        ...
 
 
-class Invoker(ABC):
-    @abstractmethod
-    async def invoke(self, options: InvokerOptions) -> Result[Any]:
-        pass
-
-    @abstractmethod
-    def get_implementations(self, uri: Uri) -> Result[Union[List[Uri], None]]:
-        pass
-
-
-class Invocable(ABC):
-    @abstractmethod
-    async def invoke(
-        self, options: InvokeOptions, invoker: Invoker
-    ) -> Result[InvocableResult]:
-        pass
+__all__ = ["Invocable", "InvocableResult"]
```

### Comparing `polywrap_core-0.1.0a8/polywrap_core/types/uri_resolver.py` & `polywrap_core-0.1.0b1/polywrap_core/types/uri_resolution_step.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,28 @@
+"""This module contains implementation of IUriResolutionStep interface."""
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Optional
-
-from polywrap_result import Result
+from typing import Any, List, Optional
 
 from .uri import Uri
-from .uri_resolution_context import IUriResolutionContext
-
-if TYPE_CHECKING:
-    from .client import Client
-    from .uri_package_wrapper import UriPackageOrWrapper
 
 
 @dataclass(slots=True, kw_only=True)
-class TryResolveUriOptions:
-    """
+class UriResolutionStep:
+    """Represents a single step in the resolution of a uri.
+
     Args:
-        no_cache_read: If set to true, the resolveUri function will not use the cache to resolve the uri.
-        no_cache_write: If set to true, the resolveUri function will not cache the results
-        config: Override the client's config for all resolutions.
-        context_id: Id used to track context data set internally.
+        source_uri (Uri): The uri that was resolved.
+        result (Any): The result of the resolution.
+        description (Optional[str]): A description of the resolution step.
+        sub_history (Optional[List[UriResolutionStep]]): A list of sub steps\
+            that were taken to resolve the uri.
     """
 
-    uri: Uri
-    resolution_context: Optional[IUriResolutionContext] = None
+    source_uri: Uri
+    result: Any
+    description: Optional[str] = None
+    sub_history: Optional[List[UriResolutionStep]] = None
 
 
-class IUriResolver(ABC):
-    @abstractmethod
-    async def try_resolve_uri(
-        self, uri: Uri, client: "Client", resolution_context: IUriResolutionContext
-    ) -> Result["UriPackageOrWrapper"]:
-        pass
+__all__ = ["UriResolutionStep"]
```

### Comparing `polywrap_core-0.1.0a8/pyproject.toml` & `polywrap_core-0.1.0b1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-core"
-version = "0.1.0a8"
+version = "0.1.0b1"
 description = ""
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-gql = "3.4.0"
-graphql-core = "^3.2.1"
-polywrap-manifest = "0.1.0a7"
-polywrap-result = "0.1.0a7"
-pydantic = "^1.10.2"
+polywrap-msgpack = "^0.1.0b1"
+polywrap-manifest = "^0.1.0b1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+pycln = "^2.1.3"
 pytest = "^7.1.2"
-pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 isort = "^5.10.1"
 pyright = "^1.1.275"
@@ -35,22 +32,24 @@
 target-version = ["py310"]
 
 [tool.pyright]
 typeCheckingMode = "strict"
 reportShadowedImports = false
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
 testpaths = [
     "tests"
 ]
 
 [tool.pylint]
 disable = [
+    "invalid-name",
     "too-many-return-statements",
+    "too-few-public-methods",
+    "unnecessary-ellipsis"
 ]
 ignore = [
     "tests/"
 ]
 
 [tool.isort]
 profile = "black"
```

