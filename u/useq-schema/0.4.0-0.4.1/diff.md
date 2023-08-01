# Comparing `tmp/useq_schema-0.4.0.tar.gz` & `tmp/useq_schema-0.4.1.tar.gz`

## Comparing `useq_schema-0.4.0.tar` & `useq_schema-0.4.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 useq_schema-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 useq_schema-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 useq_schema-0.4.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 useq_schema-0.4.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/api.md
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/index.md
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/images/favicon.ico
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/schema/axes.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/schema/event.md
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/schema/hardware_autofocus.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/schema/sequence.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/__init__.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_actions.py
--rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_base_model.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_channel.py
--rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_grid.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_hardware_autofocus.py
--rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_iter_sequence.py
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_mda_event.py
--rw-r--r--   0        0        0    16227 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_mda_sequence.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_position.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_pydantic_compat.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_time.py
--rw-r--r--   0        0        0     8219 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_utils.py
--rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_z.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/py.typed
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/pycromanager.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_autofocus.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_grid.py
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_misc.py
--rw-r--r--   0        0        0    18388 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_position_sequence.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_pycromanager.py
--rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_sequence.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_serialization.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/fixtures/mda.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/fixtures/mda.yaml
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.4.0/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.4.0/LICENSE
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 useq_schema-0.4.0/README.md
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 useq_schema-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 useq_schema-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 useq_schema-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 useq_schema-0.4.1/mkdocs.yml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.4.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 useq_schema-0.4.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 useq_schema-0.4.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/api.md
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/index.md
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/images/favicon.ico
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/schema/axes.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/schema/event.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/schema/hardware_autofocus.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/schema/sequence.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/__init__.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_actions.py
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_base_model.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_channel.py
+-rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_grid.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_hardware_autofocus.py
+-rw-r--r--   0        0        0    13309 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_iter_sequence.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_mda_event.py
+-rw-r--r--   0        0        0    15776 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_mda_sequence.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_position.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_pydantic_compat.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_time.py
+-rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_utils.py
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_z.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/py.typed
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/pycromanager.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_autofocus.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_grid.py
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_misc.py
+-rw-r--r--   0        0        0    18388 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_position_sequence.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_pycromanager.py
+-rw-r--r--   0        0        0    13451 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_sequence.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_serialization.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/fixtures/mda.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/fixtures/mda.yaml
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.4.1/LICENSE
+-rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 useq_schema-0.4.1/README.md
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 useq_schema-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 useq_schema-0.4.1/PKG-INFO
```

### Comparing `useq_schema-0.4.0/.pre-commit-config.yaml` & `useq_schema-0.4.1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -32,8 +32,9 @@
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.4.1
     hooks:
       - id: mypy
         additional_dependencies:
           - types-PyYAML
           - pydantic>=2
+          - pydantic-compat
         files: "^src/"
```

### Comparing `useq_schema-0.4.0/mkdocs.yml` & `useq_schema-0.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/.github/workflows/docs.yml` & `useq_schema-0.4.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/.github/workflows/test_and_deploy.yml` & `useq_schema-0.4.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/docs/index.md` & `useq_schema-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/docs/images/favicon.ico` & `useq_schema-0.4.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/docs/schema/axes.md` & `useq_schema-0.4.1/docs/schema/axes.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/docs/stylesheets/extra.css` & `useq_schema-0.4.1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/src/useq/__init__.py` & `useq_schema-0.4.1/src/useq/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,12 +41,10 @@
     "ZAboveBelow",
     "ZAbsolutePositions",
     "ZRangeAround",
     "ZRelativePositions",
     "ZTopBottom",
 ]
 
-from useq._pydantic_compat import model_rebuild
 
-model_rebuild(MDAEvent, MDASequence=MDASequence)
-model_rebuild(Position, MDASequence=MDASequence)
-del model_rebuild
+MDAEvent.model_rebuild(MDASequence=MDASequence)
+Position.model_rebuild(MDASequence=MDASequence)
```

### Comparing `useq_schema-0.4.0/src/useq/_actions.py` & `useq_schema-0.4.1/src/useq/_actions.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/src/useq/_base_model.py` & `useq_schema-0.4.1/src/useq/_base_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,111 +14,63 @@
     Type,
     TypeVar,
     Union,
 )
 
 import numpy as np
 from pydantic import BaseModel
-
-from useq._pydantic_compat import PYDANTIC2, model_dump, model_fields
+from pydantic_compat import PydanticCompatMixin
 
 if TYPE_CHECKING:
+    from pydantic import ConfigDict
+
     ReprArgs = Sequence[Tuple[Optional[str], Any]]
     IncEx = set[int] | set[str] | dict[int, Any] | dict[str, Any] | None
 
 __all__ = ["UseqModel", "FrozenModel"]
 
 _T = TypeVar("_T", bound="FrozenModel")
 _Y = TypeVar("_Y", bound="UseqModel")
 
 
-class FrozenModel(BaseModel):
-    if PYDANTIC2:
-        model_config = {
-            "populate_by_name": True,
-            "extra": "ignore",
-            "frozen": True,
-        }
-
-    else:
-
-        class Config:
-            allow_population_by_field_name = True
-            extra = "ignore"
-            frozen = True
-            json_encoders: ClassVar[dict] = {MappingProxyType: dict}
+class FrozenModel(PydanticCompatMixin, BaseModel):
+    model_config: ClassVar[ConfigDict] = {
+        "populate_by_name": True,
+        "extra": "ignore",
+        "frozen": True,
+        "json_encoders": {MappingProxyType: dict},
+    }
 
     def replace(self: _T, **kwargs: Any) -> _T:
         """Return a new instance replacing specified kwargs with new values.
 
         This model is immutable, so this method is useful for creating a new
         sequence with only a few fields changed.  The uid of the new sequence will
         be different from the original.
 
         The difference between this and `self.copy(update={...})` is that this method
         will perform validation and casting on the new values, whereas `copy` assumes
         that all objects are valid and will not perform any validation or casting.
         """
-        state = model_dump(self, exclude={"uid"})
+        state = self.model_dump(exclude={"uid"})
         return type(self)(**{**state, **kwargs})
 
-    if PYDANTIC2:
-        # retain pydantic1's json method
-        def json(
-            self,
-            *,
-            indent: int | None = None,  # type: ignore
-            include: IncEx = None,
-            exclude: IncEx = None,  # type: ignore
-            by_alias: bool = False,
-            exclude_unset: bool = False,
-            exclude_defaults: bool = False,
-            exclude_none: bool = False,  # type: ignore
-            round_trip: bool = False,
-            warnings: bool = True,
-        ) -> str:
-            return super().model_dump_json(
-                indent=indent,
-                include=include,
-                exclude=exclude,
-                by_alias=by_alias,
-                exclude_unset=exclude_unset,
-                exclude_defaults=exclude_defaults,
-                exclude_none=exclude_none,
-                round_trip=round_trip,
-                warnings=warnings,
-            )
-
-        # we let this one be deprecated
-        # def dict()
-
-    elif not TYPE_CHECKING:
-        # Backport pydantic2 methods so that useq-0.1.0 can be used with pydantic1
-
-        def model_dump_json(self, **kwargs: Any) -> str:
-            """Backport of pydantic2's model_dump_json method."""
-            return self.json(**kwargs)
-
-        def model_dump(self, **kwargs: Any) -> dict[str, Any]:
-            """Backport of pydantic2's model_dump_json method."""
-            return self.dict(**kwargs)
-
 
 class UseqModel(FrozenModel):
     def __repr_args__(self) -> ReprArgs:
         """Only show fields that are not None or equal to their default value."""
         return [
             (k, val)
             for k, val in super().__repr_args__()
-            if k in model_fields(self)
+            if k in self.model_fields
             and val
             != (
                 factory()
-                if (factory := model_fields(self)[k].default_factory) is not None
-                else model_fields(self)[k].default
+                if (factory := self.model_fields[k].default_factory) is not None
+                else self.model_fields[k].default
             )
         ]
 
     @classmethod
     def from_file(cls: Type[_Y], path: Union[str, Path]) -> _Y:
         """Return an instance of this class from a file.  Supports JSON and YAML."""
         path = Path(path)
@@ -129,15 +81,15 @@
         elif path.suffix == ".json":
             import json
 
             obj = json.loads(path.read_bytes())
         else:  # pragma: no cover
             raise ValueError(f"Unknown file type: {path.suffix}")
 
-        return cls.model_validate(obj) if PYDANTIC2 else cls.parse_obj(obj)
+        return cls.model_validate(obj)
 
     @classmethod
     def parse_file(cls: Type[_Y], path: Union[str, Path], **kwargs: Any) -> _Y:
         warnings.warn(  # pragma: no cover
             "parse_file is deprecated. Use from_file instead.",
             DeprecationWarning,
             stacklevel=2,
@@ -176,16 +128,15 @@
         yaml.SafeDumper.add_multi_representer(
             MappingProxyType, lambda dumper, data: dumper.represent_dict(data)
         )
         yaml.SafeDumper.add_multi_representer(
             np.floating, lambda dumper, d: dumper.represent_float(float(d))
         )
 
-        data = model_dump(
-            self,
+        data = self.model_dump(
             include=include,
             exclude=exclude,
             by_alias=by_alias,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
             exclude_none=exclude_none,
         )
```

### Comparing `useq_schema-0.4.0/src/useq/_channel.py` & `useq_schema-0.4.1/src/useq/_channel.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/src/useq/_grid.py` & `useq_schema-0.4.1/src/useq/_grid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 from __future__ import annotations
 
 import contextlib
 import math
 from enum import Enum
 from functools import partial
-from typing import Any, Callable, Iterator, NamedTuple, Optional, Sequence, Tuple, Union
+from typing import (
+    Any,
+    Callable,
+    ClassVar,
+    Iterator,
+    NamedTuple,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 import numpy as np
-from pydantic import Field
+from pydantic import ConfigDict, Field
+from pydantic_compat import field_validator
 
 from useq._base_model import FrozenModel
-from useq._pydantic_compat import FROZEN, PYDANTIC2, field_validator
+from useq._pydantic_compat import FROZEN
 
 
 class RelativeTo(Enum):
     center = "center"
     top_left = "top_left"
 
 
@@ -119,21 +130,15 @@
     fov_height : Optional[float]
         Height of the field of view in microns. If not provided, acquisition engines
         should use current height of the FOV based on the current objective and camera.
         Engines MAY override this even if provided.
     """
 
     # Overriding FrozenModel to make fov_width and fov_height mutable.
-    if PYDANTIC2:
-        model_config = {"validate_assignment": True, "frozen": False}
-    else:
-
-        class Config:
-            validate_assignment = True
-            frozen = False
+    model_config: ClassVar[ConfigDict] = {"validate_assignment": True, "frozen": False}
 
     overlap: Tuple[float, float] = Field((0.0, 0.0), **FROZEN)  # type: ignore
     mode: OrderMode = Field(OrderMode.row_wise_snake, **FROZEN)  # type: ignore
     fov_width: Optional[float] = Field(None)
     fov_height: Optional[float] = Field(None)
 
     @field_validator("overlap", mode="before")
```

### Comparing `useq_schema-0.4.0/src/useq/_hardware_autofocus.py` & `useq_schema-0.4.1/src/useq/_hardware_autofocus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any, Optional, Tuple
 
 from pydantic import PrivateAttr
 
 from useq._actions import HardwareAutofocus
 from useq._base_model import FrozenModel
 from useq._mda_event import MDAEvent
-from useq._pydantic_compat import model_copy
 
 
 class AutoFocusPlan(FrozenModel):
     """Base class for hardware autofocus plans.
 
     Attributes
     ----------
@@ -42,15 +41,15 @@
 
         updates: dict[str, Any] = {"action": self.as_action()}
         if event.z_pos is not None and event.sequence is not None:
             zplan = event.sequence.z_plan
             if zplan and zplan.is_relative and "z" in event.index:
                 updates["z_pos"] = event.z_pos - list(zplan)[event.index["z"]]
 
-        return model_copy(event, update=updates)
+        return event.model_copy(update=updates)
 
     def should_autofocus(self, event: MDAEvent) -> bool:
         """Method that must be implemented by a subclass.
 
         Should return True if autofocus should be performed (see
         [`useq.AxesBasedAF`][]).
         """
```

### Comparing `useq_schema-0.4.0/src/useq/_iter_sequence.py` & `useq_schema-0.4.1/src/useq/_iter_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 from useq._channel import Channel  # noqa: TCH001  # noqa: TCH001
 from useq._grid import (  # noqa: TCH001
     GridPosition,
 )
 from useq._mda_event import Channel as EventChannel
 from useq._mda_event import MDAEvent
-from useq._pydantic_compat import model_construct, model_copy
 from useq._utils import AXES, Axis, _has_axes
 from useq._z import AnyZPlan  # noqa: TCH001  # noqa: TCH001
 
 if TYPE_CHECKING:
     from useq._mda_sequence import MDASequence
     from useq._position import Position
 
@@ -96,15 +95,15 @@
         # set `keep_shutter_open` to `True` if and only if ALL axes whose index
         # changes betwee this_event and next_event are in `keep_shutter_open_axes`
         if all(
             axis in keep_shutter_open_axes
             for axis, idx in this_e.index.items()
             if idx != next_e.index[axis]
         ):
-            this_e = model_copy(this_e, update={"keep_shutter_open": True})
+            this_e = this_e.model_copy(update={"keep_shutter_open": True})
         yield this_e
         this_e = next_e
     yield this_e
 
 
 def _iter_sequence(
     sequence: MDASequence,
@@ -165,16 +164,16 @@
             {**event_kwargs.get("index", {}), **index}  # type: ignore
         )
         # determine x, y, z positions
         event_kwargs.update(_xyzpos(position, channel, sequence.z_plan, grid, z_pos))
         if position and position.name:
             event_kwargs["pos_name"] = position.name
         if channel:
-            event_kwargs["channel"] = model_construct(
-                EventChannel, config=channel.config, group=channel.group
+            event_kwargs["channel"] = EventChannel.model_construct(
+                config=channel.config, group=channel.group
             )
             if channel.exposure is not None:
                 event_kwargs["exposure"] = channel.exposure
         if time is not None:
             event_kwargs["min_start_time"] = time
 
         # apply any overrides
@@ -201,16 +200,16 @@
                 if position.name:
                     pos_overrides["pos_name"] = position.name
 
                 sub_seq = position.sequence
                 # if the sub-sequence doe not have an autofocus plan, we override it
                 # with the parent sequence's autofocus plan
                 if not sub_seq.autofocus_plan:
-                    sub_seq = model_copy(
-                        sub_seq, update={"autofocus_plan": autofocus_plan}
+                    sub_seq = sub_seq.model_copy(
+                        update={"autofocus_plan": autofocus_plan}
                     )
 
                 # recurse into the sub-sequence
                 yield from _iter_sequence(
                     sub_seq,
                     base_event_kwargs=event_kwargs.copy(),
                     event_kwarg_overrides=pos_overrides,
@@ -219,15 +218,15 @@
                 continue
             # note that position.sequence may be Falsey even if not None, for example
             # if all it has is an autofocus plan.  In that case, we don't recurse.
             # and we don't hit the continue statement, but we can use the autofocus plan
             elif position.sequence is not None and position.sequence.autofocus_plan:
                 autofocus_plan = position.sequence.autofocus_plan
 
-        event = model_construct(MDAEvent, **event_kwargs)
+        event = MDAEvent.model_construct(**event_kwargs)
         if autofocus_plan:
             af_event = autofocus_plan.event(event)
             if af_event:
                 yield af_event
         yield event
```

### Comparing `useq_schema-0.4.0/src/useq/_mda_event.py` & `useq_schema-0.4.1/src/useq/_mda_event.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,19 @@
     Tuple,
 )
 
 from pydantic import Field
 
 from useq._actions import AcquireImage, AnyAction
 from useq._base_model import UseqModel
-from useq._pydantic_compat import PYDANTIC2, field_serializer
+
+try:
+    from pydantic import field_serializer
+except ImportError:
+    field_serializer = None  # type: ignore
 
 if TYPE_CHECKING:
     from useq._mda_sequence import MDASequence
     from useq.pycromanager import PycroManagerEvent
 
     ReprArgs = Sequence[Tuple[Optional[str], Any]]
 
@@ -162,12 +166,12 @@
             "future version. Useq useq.pycromanager.to_pycromanager(event) instead.",
             FutureWarning,
             stacklevel=2,
         )
 
         return to_pycromanager(self)
 
-    if PYDANTIC2:
+    if field_serializer is not None:
         _si = field_serializer("index", mode="plain")(lambda v: dict(v))
         _sx = field_serializer("x_pos", mode="plain")(_float_or_none)
         _sy = field_serializer("y_pos", mode="plain")(_float_or_none)
         _sz = field_serializer("z_pos", mode="plain")(_float_or_none)
```

### Comparing `useq_schema-0.4.0/src/useq/_mda_sequence.py` & `useq_schema-0.4.1/src/useq/_mda_sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,22 @@
 import warnings
 from typing import TYPE_CHECKING, Any, Dict, Iterator, Optional, Sequence, Tuple
 from uuid import UUID, uuid4
 from warnings import warn
 
 import numpy as np
 from pydantic import Field, PrivateAttr
+from pydantic_compat import field_validator, model_validator
 
 from useq._base_model import UseqModel
 from useq._channel import Channel
 from useq._grid import AnyGridPlan, GridPosition  # noqa: TCH001
 from useq._hardware_autofocus import AnyAutofocusPlan, AxesBasedAF
 from useq._iter_sequence import iter_sequence
 from useq._position import Position
-from useq._pydantic_compat import (
-    field_validator,
-    model_construct,
-    model_dump,
-    model_validator,
-    pydantic_1_style_root_dict,
-)
 from useq._time import AnyTimePlan  # noqa: TCH001
 from useq._utils import AXES, Axis, TimeEstimate, estimate_sequence_duration
 from useq._z import AnyZPlan  # noqa: TCH001
 
 if TYPE_CHECKING:
     from useq._mda_event import MDAEvent
     from useq.pycromanager import PycroManagerEvent
@@ -172,15 +166,15 @@
         ):  # pragma: no cover
             raise ValueError(f"channels must be a sequence, got {type(value)}")
         channels = []
         for v in value:
             if isinstance(v, Channel):
                 channels.append(v)
             elif isinstance(v, str):
-                channels.append(model_construct(Channel, config=v))
+                channels.append(Channel.model_construct(config=v))
             elif isinstance(v, dict):
                 channels.append(Channel(**v))
             else:  # pragma: no cover
                 raise ValueError(f"Invalid Channel argument: {value!r}")
         return tuple(channels)
 
     @field_validator("stage_positions", mode="before")
@@ -226,44 +220,39 @@
             raise ValueError(f"Duplicate entries found in acquisition order: {order}")
 
         return order
 
     @model_validator(mode="after")
     @classmethod
     def _validate_mda(cls, values: Any) -> Any:
-        # this strange bit here is to deal with the fact that in pydantic1
-        # root_validator after returned a dict of {field_name -> validated_value}
-        # but in pydantic2 it returns the complete validated model instance
-        _values = pydantic_1_style_root_dict(cls, values)
-
-        if "axis_order" in _values:
+        if values.axis_order:
             cls._check_order(
-                _values["axis_order"],
-                z_plan=_values.get("z_plan"),
-                stage_positions=_values.get("stage_positions", ()),
-                channels=_values.get("channels", ()),
-                grid_plan=_values.get("grid_plan"),
-                autofocus_plan=_values.get("autofocus_plan"),
+                values.axis_order,
+                z_plan=values.z_plan,
+                stage_positions=values.stage_positions,
+                channels=values.channels,
+                grid_plan=values.grid_plan,
+                autofocus_plan=values.autofocus_plan,
             )
-        if "stage_positions" in _values:
-            for p in _values["stage_positions"]:
+        if values.stage_positions:
+            for p in values.stage_positions:
                 if hasattr(p, "sequence") and getattr(
                     p.sequence, "keep_shutter_open_across", None
                 ):  # pragma: no cover
                     raise ValueError(
                         "keep_shutter_open_across cannot currently be set on a "
                         "Position sequence"
                     )
         return values
 
     def __eq__(self, other: Any) -> bool:
         """Return `True` if two `MDASequences` are equal (uid is excluded)."""
         if isinstance(other, MDASequence):
             return bool(
-                model_dump(self, exclude={"uid"}) == model_dump(other, exclude={"uid"})
+                self.model_dump(exclude={"uid"}) == other.model_dump(exclude={"uid"})
             )
         else:
             return False
 
     @staticmethod
     def _check_order(
         order: str,
```

### Comparing `useq_schema-0.4.0/src/useq/_position.py` & `useq_schema-0.4.1/src/useq/_position.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/src/useq/_time.py` & `useq_schema-0.4.1/src/useq/_time.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/src/useq/_utils.py` & `useq_schema-0.4.1/src/useq/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import annotations
 
 import re
 from datetime import timedelta
 from typing import TYPE_CHECKING, Literal, NamedTuple, TypeVar
 
-from useq._pydantic_compat import model_copy
-
 if TYPE_CHECKING:
     from typing import Final
 
     from typing_extensions import TypeGuard
 
     import useq
     from useq._time import SinglePhaseTimePlan
@@ -100,15 +98,15 @@
             sub_seq = parent_seq
         else:
             updates = {
                 field: getattr(parent_seq, field)
                 for field in ("time_plan", "z_plan", "grid_plan", "channels")
                 if getattr(parent_seq, field) and not getattr(p.sequence, field)
             }
-            sub_seq = model_copy(p.sequence, update=updates)
+            sub_seq = p.sequence.model_copy(update=updates)
         estimate += _estimate_simple_sequence_duration(sub_seq)
     return estimate
 
 
 def _estimate_simple_sequence_duration(seq: useq.MDASequence) -> TimeEstimate:
     """Estimate the duration of an MDASequence with no sub-pos axes to iterate over.
```

### Comparing `useq_schema-0.4.0/src/useq/_z.py` & `useq_schema-0.4.1/src/useq/_z.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import math
-from typing import Any, Callable, Iterator, List, Sequence, Union
+from typing import Callable, Iterator, List, Sequence, Union
 
 import numpy as np
+from pydantic_compat import field_validator
 
 from useq._base_model import FrozenModel
-from useq._pydantic_compat import field_validator
 
 
-def _list_cast(field: str) -> Callable[[Any], Any]:
-    v = field_validator(field, mode="before", allow_reuse=True, check_fields=False)
+def _list_cast(field: str) -> Callable:
+    v = field_validator(field, mode="before", check_fields=False)
     return v(list)
 
 
 class ZPlan(FrozenModel):
     go_up: bool = True
 
     def __iter__(self) -> Iterator[float]:  # type: ignore
```

### Comparing `useq_schema-0.4.0/src/useq/pycromanager.py` & `useq_schema-0.4.1/src/useq/pycromanager.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/tests/conftest.py` & `useq_schema-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/tests/test_autofocus.py` & `useq_schema-0.4.1/tests/test_autofocus.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,30 @@
 
 from typing import Iterable
 
 import pytest
 
 import useq
 from useq import AxesBasedAF, HardwareAutofocus, MDASequence
-from useq._pydantic_compat import model_copy
 
 ZRANGE2 = useq.ZRangeAround(range=2, step=1)
 ZPOS_30 = useq.Position(z=30.0)
 ZPOS_200 = useq.Position(z=200.0)
 GRID_PLAN = useq.GridRelative(rows=2, columns=1)
 TWO_CH = MDASequence(stage_positions=[ZPOS_30], channels=["DAPI", "FITC"])
 TWO_CH_TWO_P = TWO_CH.replace(stage_positions=[ZPOS_30, ZPOS_200])
 TWO_CH_TWO_P_GRID = TWO_CH_TWO_P.replace(grid_plan=GRID_PLAN)
 TWO_CH_TWO_P_T = TWO_CH_TWO_P.replace(time_plan={"interval": 1, "loops": 2})
 NO_CH_ZSTACK = MDASequence(stage_positions=[ZPOS_30], z_plan=ZRANGE2)
 TWO_CH_ZSTACK = NO_CH_ZSTACK.replace(channels=["DAPI", "FITC"])
 AF = AxesBasedAF(autofocus_device_name="Z", autofocus_motor_offset=40, axes=())
-AF_C = model_copy(AF, update={"axes": ("c",)})
-AF_G = model_copy(AF, update={"axes": ("g",)})
-AF_P = model_copy(AF, update={"axes": ("p",)})
-AF_Z = model_copy(AF, update={"axes": ("z",)})
+AF_C = AF.model_copy(update={"axes": ("c",)})
+AF_G = AF.model_copy(update={"axes": ("g",)})
+AF_P = AF.model_copy(update={"axes": ("p",)})
+AF_Z = AF.model_copy(update={"axes": ("z",)})
 AF_SEQ_C = MDASequence(autofocus_plan=AF_C)
 SUB_P_AF_C = useq.Position(z=10, sequence=AF_SEQ_C)
 SUB_P_AF_G = useq.Position(z=10, sequence=MDASequence(autofocus_plan=AF_G))
 SUB_P_AF_P = useq.Position(z=10, sequence=MDASequence(autofocus_plan=AF_P))
 SUB_P_AF_Z = useq.Position(z=10, sequence=MDASequence(autofocus_plan=AF_Z))
 TWO_CH_SUBPAF_C = TWO_CH.replace(stage_positions=[ZPOS_30, SUB_P_AF_C])
 TWO_CH_SUBPAF_Z = TWO_CH.replace(stage_positions=[ZPOS_30, SUB_P_AF_Z])
@@ -66,15 +65,15 @@
 @pytest.mark.parametrize("mda, af_axes, expected_af_indices", AF_TESTS)
 def test_autofocus(
     mda: MDASequence,
     af_axes: tuple[str, ...],
     expected_af_indices: Iterable[int],
 ) -> None:
     if af_axes:
-        mda = mda.replace(autofocus_plan=model_copy(AF, update={"axes": af_axes}))
+        mda = mda.replace(autofocus_plan=AF.model_copy(update={"axes": af_axes}))
         assert isinstance(mda.autofocus_plan, AxesBasedAF)
         assert mda.autofocus_plan.axes == af_axes
 
     actual = [i for i, e in enumerate(mda) if isinstance(e.action, HardwareAutofocus)]
     expected = list(expected_af_indices)
     assert expected == actual, "Unexpected AF indices"
```

### Comparing `useq_schema-0.4.0/tests/test_grid.py` & `useq_schema-0.4.1/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/tests/test_misc.py` & `useq_schema-0.4.1/tests/test_misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from __future__ import annotations
 
-from contextlib import nullcontext
-
 import numpy as np
 import pytest
 
 import useq
-from useq._pydantic_compat import PYDANTIC2
 
 
 def test_from_numpy() -> None:
     useq.ZRelativePositions(relative=np.arange(-1.5, 1.5, 0.5))
 
 
 DAPI_10 = useq.Channel(config="DAPI", exposure=10)
@@ -148,10 +145,8 @@
 
 def test_pydantic_compat(mda1: useq.MDASequence) -> None:
     # testing names of deprecated methods and cross-compatible API
     assert mda1.json()
     assert mda1.model_dump_json()
 
     assert mda1.model_dump()
-    ctx = pytest.warns(DeprecationWarning) if PYDANTIC2 else nullcontext()
-    with ctx:  # type: ignore
-        assert mda1.dict()
+    assert mda1.dict()
```

### Comparing `useq_schema-0.4.0/tests/test_position_sequence.py` & `useq_schema-0.4.1/tests/test_position_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/tests/test_sequence.py` & `useq_schema-0.4.1/tests/test_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     TIntervalLoops,
     ZAboveBelow,
     ZAbsolutePositions,
     ZRangeAround,
     ZRelativePositions,
 )
 from useq._grid import GridPosition
-from useq._pydantic_compat import PYDANTIC2
 
 _T = List[Tuple[Any, Sequence[float]]]
 
 z_as_class: _T = [
     (ZAboveBelow(above=8, below=4, step=2), [-4, -2, 0, 2, 4, 6, 8]),
     (ZAbsolutePositions(absolute=[0, 0.5, 5]), [0, 0.5, 5]),
     (ZRelativePositions(relative=[0, 0.5, 5]), [0, 0.5, 5]),
@@ -275,21 +274,17 @@
     assert (mda.channels[0].group, mda.channels[0].config) == cexpectation
     position = mda.stage_positions[0]
     assert (position.x, position.y, position.z) == pexpectation
 
 
 @pytest.mark.parametrize("cls", [MDASequence, MDAEvent])
 def test_schema(cls: BaseModel) -> None:
-    if PYDANTIC2:
-        schema = cls.model_json_schema()
-        assert schema
-        assert json.dumps(schema)
-    else:
-        assert cls.schema()
-        assert cls.schema_json()
+    schema = cls.model_json_schema()
+    assert schema
+    assert json.dumps(schema)
 
 
 def test_z_position() -> None:
     mda = MDASequence(axis_order="tpcz", stage_positions=[(222, 1, 10), (111, 1, 20)])
     assert not mda.z_plan
     for event in mda:
         assert event.z_pos
```

### Comparing `useq_schema-0.4.0/tests/test_serialization.py` & `useq_schema-0.4.1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/tests/fixtures/mda.json` & `useq_schema-0.4.1/tests/fixtures/mda.json`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/tests/fixtures/mda.yaml` & `useq_schema-0.4.1/tests/fixtures/mda.yaml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/.gitignore` & `useq_schema-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/LICENSE` & `useq_schema-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/README.md` & `useq_schema-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.0/pyproject.toml` & `useq_schema-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Software Development",
     "Topic :: System :: Hardware",
     "Typing :: Typed",
 ]
 dynamic = ["version"]
-dependencies = ["pydantic >=1.7", "numpy"]
+dependencies = ["pydantic >=1.7", "numpy", "pydantic-compat >=0.0.1"]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 yaml = ["PyYAML"]
 test = ["pytest>=6.0", "pytest-cov", "PyYAML"]
 dev = [
```

### Comparing `useq_schema-0.4.0/PKG-INFO` & `useq_schema-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useq-schema
-Version: 0.4.0
+Version: 0.4.1
 Summary: Schema for multi-dimensional microscopy experiments
 Project-URL: Source, https://github.com/pymmcore-plus/useq-schema
 Project-URL: Tracker, https://github.com/pymmcore-plus/useq-schema/issues
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Keywords: microscopy,schema
@@ -23,14 +23,15 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Hardware
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: numpy
+Requires-Dist: pydantic-compat>=0.0.1
 Requires-Dist: pydantic>=1.7
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
```

