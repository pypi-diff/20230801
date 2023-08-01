# Comparing `tmp/mango_odm-0.3.0.tar.gz` & `tmp/mango_odm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango_odm-0.3.0.tar", max compression
+gzip compressed data, was "mango_odm-0.3.1.tar", last modified: Tue Aug  1 13:20:22 2023, max compression
```

## Comparing `mango_odm-0.3.0.tar` & `mango_odm-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1085 2022-11-16 11:34:14.111392 mango_odm-0.3.0/LICENSE
--rw-r--r--   0        0        0      467 2023-01-01 12:47:01.171243 mango_odm-0.3.0/mango/__init__.py
--rw-r--r--   0        0        0     4505 2023-01-01 12:47:01.172244 mango_odm-0.3.0/mango/drive.py
--rw-r--r--   0        0        0     1145 2023-01-01 12:47:01.172244 mango_odm-0.3.0/mango/encoder.py
--rw-r--r--   0        0        0     5637 2023-01-01 12:47:01.173244 mango_odm-0.3.0/mango/expression.py
--rw-r--r--   0        0        0     3416 2023-01-01 12:47:01.173244 mango_odm-0.3.0/mango/fields.py
--rw-r--r--   0        0        0     1737 2023-01-01 12:47:01.174244 mango_odm-0.3.0/mango/index.py
--rw-r--r--   0        0        0     1015 2023-01-01 12:47:01.174244 mango_odm-0.3.0/mango/meta.py
--rw-r--r--   0        0        0     9096 2023-01-01 12:47:01.174244 mango_odm-0.3.0/mango/models.py
--rw-r--r--   0        0        0        0 2022-11-16 11:34:14.113391 mango_odm-0.3.0/mango/py.typed
--rw-r--r--   0        0        0     6716 2023-01-01 12:47:01.175244 mango_odm-0.3.0/mango/result.py
--rw-r--r--   0        0        0     2263 2023-01-01 12:47:01.175244 mango_odm-0.3.0/mango/source.py
--rw-r--r--   0        0        0    16528 2023-01-01 12:47:01.176244 mango_odm-0.3.0/mango/stage.py
--rw-r--r--   0        0        0     4546 2023-01-01 12:47:01.176244 mango_odm-0.3.0/mango/utils.py
--rw-r--r--   0        0        0     1166 2023-01-01 12:47:01.177244 mango_odm-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5644 2023-01-01 12:47:01.170245 mango_odm-0.3.0/README.md
--rw-r--r--   0        0        0     6379 1970-01-01 00:00:00.000000 mango_odm-0.3.0/setup.py
--rw-r--r--   0        0        0     6103 1970-01-01 00:00:00.000000 mango_odm-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-01 13:20:12.075699 mango_odm-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4815 2023-08-01 13:20:12.075699 mango_odm-0.3.1/README.md
+-rw-r--r--   0        0        0      445 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/__init__.py
+-rw-r--r--   0        0        0     4331 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/drive.py
+-rw-r--r--   0        0        0     1110 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/encoder.py
+-rw-r--r--   0        0        0     5639 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/expression.py
+-rw-r--r--   0        0        0     3284 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/fields.py
+-rw-r--r--   0        0        0     1665 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/index.py
+-rw-r--r--   0        0        0     1040 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/meta.py
+-rw-r--r--   0        0        0     9261 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/models.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/py.typed
+-rw-r--r--   0        0        0     6570 2023-08-01 13:20:12.079699 mango_odm-0.3.1/mango/result.py
+-rw-r--r--   0        0        0     2221 2023-08-01 13:20:12.079699 mango_odm-0.3.1/mango/source.py
+-rw-r--r--   0        0        0    16192 2023-08-01 13:20:12.079699 mango_odm-0.3.1/mango/stage.py
+-rw-r--r--   0        0        0     4391 2023-08-01 13:20:12.079699 mango_odm-0.3.1/mango/utils.py
+-rw-r--r--   0        0        0     2533 2023-08-01 13:20:22.235786 mango_odm-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6047 1970-01-01 00:00:00.000000 mango_odm-0.3.1/PKG-INFO
```

### Comparing `mango_odm-0.3.0/LICENSE` & `mango_odm-0.3.1/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Akirami
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Akirami
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `mango_odm-0.3.0/mango/drive.py` & `mango_odm-0.3.1/mango/drive.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,147 +1,144 @@
-import os
-from collections.abc import Iterator
-from typing import Any, ClassVar
-
-from motor.motor_asyncio import (
-    AsyncIOMotorClient,
-    AsyncIOMotorCollection,
-    AsyncIOMotorDatabase,
-)
-from typing_extensions import Self
-
-DEFAULT_CONNECT_URI = os.getenv("MANGO_URI") or "mongodb://localhost:27017"
-DEFAULT_DATABASE_NAME = "test"
-
-
-class Collection:
-    def __init__(self, collection: AsyncIOMotorCollection) -> None:
-        self.collection = collection
-
-    def __getattr__(self, name: str) -> Any:
-        return getattr(self.collection, name)
-
-    def __repr__(self) -> str:
-        return f"Collection(name={self.name}, db={self.full_name.split('.')[0]})"
-
-    @property
-    def name(self) -> str:
-        return self.collection.name
-
-    @property
-    def full_name(self) -> str:
-        return self.collection.full_name
-
-
-class Database:
-    def __init__(self, db: AsyncIOMotorDatabase) -> None:
-        self.db = db
-        self.collections: dict[str, Collection] = {}
-
-    def __getattr__(self, name: str) -> Collection:
-        try:
-            return self.collections[name]
-        except KeyError:
-            collection: AsyncIOMotorCollection = self.db.get_collection(name)
-            self.collections[name] = Collection(collection)
-            return self.collections[name]
-
-    def __getitem__(self, name: str) -> Collection:
-        return self.__getattr__(name)
-
-    def __iter__(self) -> Iterator[Collection]:
-        return iter(self.collections.values())
-
-    def __repr__(self) -> str:
-        return (
-            f"Database(name={self.name}, "
-            f"host={self.client.HOST}, "
-            f"port={self.client.PORT})"
-        )
-
-    async def drop_collection(self, collection: str | Collection):
-        """删除集合"""
-        name = collection if isinstance(collection, str) else collection.name
-        await self.db.drop_collection(name)
-        self.collections.pop(name, None)
-
-    @property
-    def name(self) -> str:
-        return self.db.name
-
-    @property
-    def client(self) -> AsyncIOMotorClient:
-        return self.db.client
-
-
-class Client:
-    _clients: ClassVar[set[Self]] = set()
-
-    def __init__(self, uri: str = DEFAULT_CONNECT_URI, **kwargs: Any) -> None:
-        kwargs.setdefault("host", uri)
-        self.client = AsyncIOMotorClient(**kwargs)
-        self.databases: dict[str, Database] = {}
-        self.__class__._clients.add(self)
-
-    def __getattr__(self, name: str) -> Database:
-        try:
-            return self.databases[name]
-        except KeyError:
-            db: AsyncIOMotorDatabase = self.client.get_database(name)
-            self.databases[name] = Database(db)
-            return self.databases[name]
-
-    def __getitem__(self, name: str) -> Database:
-        return self.__getattr__(name)
-
-    def __iter__(self) -> Iterator[Database]:
-        return iter(self.databases.values())
-
-    def __repr__(self) -> str:
-        return f"Client(host={self.host}, port={self.port})"
-
-    def close(self) -> None:
-        """关闭连接"""
-        self.client.close()
-        self.__class__._clients.remove(self)
-
-    async def drop_database(self, database: str | Database):
-        """删除数据库"""
-        name = database if isinstance(database, str) else database.name
-        await self.client.drop_database(name)
-        self.databases.pop(name, None)
-
-    @classmethod
-    def get_database(cls, db: Database | str | None = None) -> Database:
-        """获取数据库"""
-        try:
-            client = next(iter(cls._clients))
-        except StopIteration:
-            client = cls()
-
-        if isinstance(db, Database):
-            return db
-        elif isinstance(db, str):
-            return client[db]
-        else:
-            return client.default_database
-
-    @property
-    def default_database(self) -> Database:
-        """默认为首次调用的数据库, 如果不存在, 则创建 test 数据库"""
-        try:
-            return next(iter(self.databases.values()))
-        except StopIteration:
-            ddb = self.client.get_default_database(DEFAULT_DATABASE_NAME)
-            return self[ddb.name]
-
-    @property
-    def host(self) -> str:
-        return self.client.HOST
-
-    @property
-    def port(self) -> int:
-        return self.client.PORT
-
-    @property
-    def address(self) -> tuple[str, int]:
-        return self.client.address
+import os
+from collections.abc import Iterator
+from typing import Any, ClassVar
+
+from motor.motor_asyncio import (
+    AsyncIOMotorClient,
+    AsyncIOMotorCollection,
+    AsyncIOMotorDatabase,
+)
+from typing_extensions import Self
+
+DEFAULT_CONNECT_URI = os.getenv("MANGO_URI") or "mongodb://localhost:27017"
+DEFAULT_DATABASE_NAME = "test"
+
+
+class Collection:
+    def __init__(self, collection: AsyncIOMotorCollection) -> None:
+        self.collection = collection
+
+    def __getattr__(self, name: str) -> Any:
+        return getattr(self.collection, name)
+
+    def __repr__(self) -> str:
+        return f"Collection(name={self.name}, db={self.full_name.split('.')[0]})"
+
+    @property
+    def name(self) -> str:
+        return self.collection.name
+
+    @property
+    def full_name(self) -> str:
+        return self.collection.full_name
+
+
+class Database:
+    def __init__(self, db: AsyncIOMotorDatabase) -> None:
+        self.db = db
+        self.collections: dict[str, Collection] = {}
+
+    def __getattr__(self, name: str) -> Collection:
+        try:
+            return self.collections[name]
+        except KeyError:
+            collection: AsyncIOMotorCollection = self.db.get_collection(name)
+            self.collections[name] = Collection(collection)
+            return self.collections[name]
+
+    def __getitem__(self, name: str) -> Collection:
+        return self.__getattr__(name)
+
+    def __iter__(self) -> Iterator[Collection]:
+        return iter(self.collections.values())
+
+    def __repr__(self) -> str:
+        return (
+            f"Database(name={self.name}, "
+            f"host={self.client.HOST}, "
+            f"port={self.client.PORT})"
+        )
+
+    async def drop_collection(self, collection: str | Collection) -> None:
+        """删除集合"""
+        name = collection if isinstance(collection, str) else collection.name
+        await self.db.drop_collection(name)
+        self.collections.pop(name, None)
+
+    @property
+    def name(self) -> str:
+        return self.db.name
+
+    @property
+    def client(self) -> AsyncIOMotorClient:
+        return self.db.client
+
+
+class Client:
+    _clients: ClassVar[set[Self]] = set()
+
+    def __init__(self, uri: str = DEFAULT_CONNECT_URI, **kwargs: Any) -> None:
+        kwargs.setdefault("host", uri)
+        self.client = AsyncIOMotorClient(**kwargs)
+        self.databases: dict[str, Database] = {}
+        self.__class__._clients.add(self)
+
+    def __getattr__(self, name: str) -> Database:
+        try:
+            return self.databases[name]
+        except KeyError:
+            db: AsyncIOMotorDatabase = self.client.get_database(name)
+            self.databases[name] = Database(db)
+            return self.databases[name]
+
+    def __getitem__(self, name: str) -> Database:
+        return self.__getattr__(name)
+
+    def __iter__(self) -> Iterator[Database]:
+        return iter(self.databases.values())
+
+    def __repr__(self) -> str:
+        return f"Client(host={self.host}, port={self.port})"
+
+    def close(self) -> None:
+        """关闭连接"""
+        self.client.close()
+        self.__class__._clients.remove(self)
+
+    async def drop_database(self, database: str | Database) -> None:
+        """删除数据库"""
+        name = database if isinstance(database, str) else database.name
+        await self.client.drop_database(name)
+        self.databases.pop(name, None)
+
+    @classmethod
+    def get_database(cls, db: Database | str | None = None) -> Database:
+        """获取数据库"""
+        try:
+            client = next(iter(cls._clients))
+        except StopIteration:
+            client = cls()
+
+        if isinstance(db, Database):
+            return db
+        return client[db] if isinstance(db, str) else client.default_database
+
+    @property
+    def default_database(self) -> Database:
+        """默认为首次调用的数据库, 如果不存在, 则创建 test 数据库"""
+        try:
+            return next(iter(self.databases.values()))
+        except StopIteration:
+            ddb = self.client.get_default_database(DEFAULT_DATABASE_NAME)
+            return self[ddb.name]
+
+    @property
+    def host(self) -> str:
+        return self.client.HOST
+
+    @property
+    def port(self) -> int:
+        return self.client.PORT
+
+    @property
+    def address(self) -> tuple[str, int]:
+        return self.client.address
```

### Comparing `mango_odm-0.3.0/mango/expression.py` & `mango_odm-0.3.1/mango/expression.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,184 +1,189 @@
-from dataclasses import dataclass
-from enum import Enum, auto
-from typing import TYPE_CHECKING, Any
-
-from pydantic.fields import ModelField
-from typing_extensions import Self
-
-if TYPE_CHECKING:  # pragma: no cover
-    from mango.models import Document
-
-
-class Operators(Enum):
-    EQ = auto()
-    """等于"""
-    NE = auto()
-    """不等于"""
-    LT = auto()
-    """小于"""
-    LTE = auto()
-    """小于或等于"""
-    GT = auto()
-    """大于"""
-    GTE = auto()
-    """大于或等于"""
-    OR = auto()
-    """逻辑或"""
-    AND = auto()
-    """逻辑与"""
-    NOR = auto()
-    """逻辑非或"""
-    IN = auto()
-    """包含在"""
-    NIN = auto()
-    """不包含在"""
-    REGEX = auto()
-    """正则匹配"""
-
-    def __str__(self) -> str:
-        return f"${self.name.lower()}"
-
-
-class ExpressionField:
-    def __init__(
-        self, field: ModelField, parents: list[tuple[str, "Document"]]
-    ) -> None:
-        self.field = field
-        self.parents = parents
-
-    def __eq__(self, other: Any) -> "Expression":
-        return OPR(self).eq(other)
-
-    def __ne__(self, other: Any) -> "Expression":
-        return OPR(self).ne(other)
-
-    def __lt__(self, other: Any) -> "Expression":
-        return OPR(self).lt(other)
-
-    def __le__(self, other: Any) -> "Expression":
-        return OPR(self).lte(other)
-
-    def __gt__(self, other: Any) -> "Expression":
-        return OPR(self).gt(other)
-
-    def __ge__(self, other: Any) -> "Expression":
-        return OPR(self).gte(other)
-
-    def __hash__(self) -> int:
-        return super().__hash__()
-
-    def __repr__(self) -> str:
-        return f"ExpressionField(name={str(self)}, type={self.field.type_.__name__})"
-
-    def __str__(self) -> str:
-        names = [p[0] for p in self.parents]
-        names.append(self.field.name)
-        return ".".join(names)
-
-    def __getattr__(self, name: str) -> Any:
-        """内嵌查询反向查找分配父级"""
-        attr = getattr(self.field.outer_type_, name)
-        if isinstance(attr, self.__class__):
-            new_parent = (self.field.name, self.field.outer_type_)
-            if new_parent not in attr.parents:
-                attr.parents.append(new_parent)
-            if new_parents := list(set(self.parents) - set(attr.parents)):
-                attr.parents = new_parents + attr.parents
-        return attr
-
-
-@dataclass
-class Expression:
-    key: ExpressionField | None
-    operator: Operators
-    value: Any
-
-    def __or__(self, other: Self) -> Self:
-        return OPR.or_(self, other)
-
-    def __and__(self, other: Self) -> Self:
-        return OPR.and_(self, other)
-
-    def __repr__(self) -> str:
-        return f"Expression({self.struct()})"
-
-    def struct(self) -> dict[str, Any]:
-        """转换为 MongoDB 查询结构"""
-        value = {str(self.operator): self.unpack(self.value)}
-        return {str(self.key): value} if self.key else value
-
-    def unpack(self, value: Any):
-        # TODO: 将嵌入文档模型转换为 mongodb 文档形式
-        return value
-
-    def merge(self, operator: Operators):
-        return self.value if self.operator is operator else [self]
-
-
-class OPR:
-    def __init__(self, key: Any) -> None:
-        if not isinstance(key, ExpressionField):
-            raise TypeError("必须是有效的字段")
-        self.key = key
-
-    def eq(self, value: Any) -> Expression:
-        return Expression(self.key, Operators.EQ, value)
-
-    def ne(self, value: Any) -> Expression:
-        return Expression(self.key, Operators.NE, value)
-
-    def lt(self, value: Any) -> Expression:
-        return Expression(self.key, Operators.LT, value)
-
-    def lte(self, value: Any) -> Expression:
-        return Expression(self.key, Operators.LTE, value)
-
-    def gt(self, value: Any) -> Expression:
-        return Expression(self.key, Operators.GT, value)
-
-    def gte(self, value: Any) -> Expression:
-        return Expression(self.key, Operators.GTE, value)
-
-    def in_(self, *values: Any) -> Expression:
-        """包含在"""
-        return Expression(self.key, Operators.IN, values)
-
-    def nin(self, *values: Any) -> Expression:
-        """不包含在"""
-        return Expression(self.key, Operators.NIN, values)
-
-    def regex(self, values: str) -> Expression:
-        """正则匹配"""
-        return Expression(self.key, Operators.REGEX, values)
-
-    @classmethod
-    def or_(cls, *expressions: Expression | bool) -> Expression:
-        merge = cls._merge(Operators.OR, expressions)
-        return Expression(None, *merge)
-
-    @classmethod
-    def and_(cls, *expressions: Expression | bool) -> Expression:
-        merge = cls._merge(Operators.AND, expressions)
-        return Expression(None, *merge)
-
-    @classmethod
-    def nor(cls, *expressions: Expression | bool) -> Expression:
-        """既不……也不……"""
-        merge = cls._merge(Operators.NOR, expressions)
-        return Expression(None, *merge)
-
-    @classmethod
-    def _merge(
-        cls, operator: Operators, expressions: tuple[Expression | bool]
-    ) -> tuple[Operators, list[Expression]]:
-        merge_expr: list[Expression] = []
-        for expression in expressions:
-            if not isinstance(expression, Expression):
-                raise TypeError("必须是有效的表达式")
-
-            if expression.operator is operator:
-                merge_expr.extend(expression.value)
-            else:
-                merge_expr.append(expression)
-
-        return operator, merge_expr
+from dataclasses import dataclass
+from enum import Enum, auto
+from typing import TYPE_CHECKING, Any
+
+from pydantic.fields import ModelField
+from typing_extensions import Self
+
+from mango.fields import FieldInfo
+
+if TYPE_CHECKING:  # pragma: no cover
+    from mango.models import Document
+
+
+class Operators(Enum):
+    EQ = auto()
+    """等于"""
+    NE = auto()
+    """不等于"""
+    LT = auto()
+    """小于"""
+    LTE = auto()
+    """小于或等于"""
+    GT = auto()
+    """大于"""
+    GTE = auto()
+    """大于或等于"""
+    OR = auto()
+    """逻辑或"""
+    AND = auto()
+    """逻辑与"""
+    NOR = auto()
+    """逻辑非或"""
+    IN = auto()
+    """包含在"""
+    NIN = auto()
+    """不包含在"""
+    REGEX = auto()
+    """正则匹配"""
+
+    def __str__(self) -> str:
+        return f"${self.name.lower()}"
+
+
+class ExpressionField:
+    def __init__(
+        self, field: ModelField, parents: list[tuple[str, "Document"]]
+    ) -> None:
+        self.field = field
+        self.parents = parents
+
+    def __eq__(self, other: Any) -> "Expression":
+        return OPR(self).eq(other)
+
+    def __ne__(self, other: Any) -> "Expression":
+        return OPR(self).ne(other)
+
+    def __lt__(self, other: Any) -> "Expression":
+        return OPR(self).lt(other)
+
+    def __le__(self, other: Any) -> "Expression":
+        return OPR(self).lte(other)
+
+    def __gt__(self, other: Any) -> "Expression":
+        return OPR(self).gt(other)
+
+    def __ge__(self, other: Any) -> "Expression":
+        return OPR(self).gte(other)
+
+    def __hash__(self) -> int:
+        return super().__hash__()
+
+    def __repr__(self) -> str:
+        return f"ExpressionField(name={self!s}, type={self.field._type_display()})"
+
+    def __str__(self) -> str:
+        names = [p[0] for p in self.parents]
+        if isinstance(finfo := self.field.field_info, FieldInfo) and finfo.primary_key:
+            names.append("_id")
+        else:
+            names.append(self.field.name)
+        return ".".join(names)
+
+    def __getattr__(self, name: str) -> Any:
+        """内嵌查询反向查找分配父级"""
+        attr = getattr(self.field.outer_type_, name)
+        if isinstance(attr, self.__class__):
+            new_parent = (self.field.name, self.field.outer_type_)
+            if new_parent not in attr.parents:
+                attr.parents.append(new_parent)
+            if new_parents := list(set(self.parents) - set(attr.parents)):
+                attr.parents = new_parents + attr.parents
+        return attr
+
+
+@dataclass
+class Expression:
+    key: ExpressionField | None
+    operator: Operators
+    value: Any
+
+    def __or__(self, other: Self) -> Self:
+        return OPR.or_(self, other)
+
+    def __and__(self, other: Self) -> Self:
+        return OPR.and_(self, other)
+
+    def __repr__(self) -> str:
+        return f"Expression({self.struct()})"
+
+    def struct(self) -> dict[str, Any]:
+        """转换为 MongoDB 查询结构"""
+        value = {str(self.operator): self.unpack(self.value)}
+        return {str(self.key): value} if self.key else value
+
+    def unpack(self, value: Any) -> Any:
+        # TODO: 将嵌入文档模型转换为 mongodb 文档形式
+        return value
+
+    def merge(self, operator: Operators) -> Any:
+        return self.value if self.operator is operator else [self]
+
+
+class OPR:
+    def __init__(self, key: Any) -> None:
+        if not isinstance(key, ExpressionField):
+            raise TypeError("必须是有效的字段")
+        self.key = key
+
+    def eq(self, value: Any) -> Expression:
+        return Expression(self.key, Operators.EQ, value)
+
+    def ne(self, value: Any) -> Expression:
+        return Expression(self.key, Operators.NE, value)
+
+    def lt(self, value: Any) -> Expression:
+        return Expression(self.key, Operators.LT, value)
+
+    def lte(self, value: Any) -> Expression:
+        return Expression(self.key, Operators.LTE, value)
+
+    def gt(self, value: Any) -> Expression:
+        return Expression(self.key, Operators.GT, value)
+
+    def gte(self, value: Any) -> Expression:
+        return Expression(self.key, Operators.GTE, value)
+
+    def in_(self, *values: Any) -> Expression:
+        """包含在"""
+        return Expression(self.key, Operators.IN, values)
+
+    def nin(self, *values: Any) -> Expression:
+        """不包含在"""
+        return Expression(self.key, Operators.NIN, values)
+
+    def regex(self, values: str) -> Expression:
+        """正则匹配"""
+        return Expression(self.key, Operators.REGEX, values)
+
+    @classmethod
+    def or_(cls, *expressions: Expression | bool) -> Expression:
+        merge = cls._merge(Operators.OR, expressions)
+        return Expression(None, *merge)
+
+    @classmethod
+    def and_(cls, *expressions: Expression | bool) -> Expression:
+        merge = cls._merge(Operators.AND, expressions)
+        return Expression(None, *merge)
+
+    @classmethod
+    def nor(cls, *expressions: Expression | bool) -> Expression:
+        """既不……也不……"""
+        merge = cls._merge(Operators.NOR, expressions)
+        return Expression(None, *merge)
+
+    @classmethod
+    def _merge(
+        cls, operator: Operators, expressions: tuple[Expression | bool]
+    ) -> tuple[Operators, list[Expression]]:
+        merge_expr: list[Expression] = []
+        for expression in expressions:
+            if not isinstance(expression, Expression):
+                raise TypeError("必须是有效的表达式")
+
+            if expression.operator is operator:
+                merge_expr.extend(expression.value)
+            else:
+                merge_expr.append(expression)
+
+        return operator, merge_expr
```

### Comparing `mango_odm-0.3.0/mango/fields.py` & `mango_odm-0.3.1/mango/fields.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-from collections.abc import Callable, Generator, Mapping
-from typing import AbstractSet, Any, AnyStr
-
-from bson import ObjectId
-from pydantic.fields import FieldInfo as PDFieldInfo
-from pydantic.fields import Undefined
-from pydantic.typing import NoArgAnyCallable
-from typing_extensions import Self
-
-from mango.index import Index, IndexType
-
-
-class ObjectIdField(ObjectId):
-    @classmethod
-    def __get_validators__(cls) -> Generator[Callable[[AnyStr], Self], None, None]:
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, v: AnyStr) -> Self:
-        if cls.is_valid(v):
-            return cls(v)
-        raise ValueError("无效的 ObjectId")
-
-    @classmethod
-    def __modify_schema__(cls, field_schema: dict) -> None:
-        field_schema.update(type="string")
-
-
-class FieldInfo(PDFieldInfo):
-    def __init__(self, default: Any = Undefined, **kwargs: Any) -> None:
-        self.primary_key: bool = kwargs.pop("primary_key", False)
-        self.index: bool | IndexType | Index | None = kwargs.pop("index", None)
-        self.expire: int | None = kwargs.pop("expire", None)
-        self.unique: bool = kwargs.pop("unique", None)
-        super().__init__(default=default, **kwargs)
-
-
-def Field(
-    default: Any = Undefined,
-    *,
-    default_factory: NoArgAnyCallable | None = None,
-    alias: str | None = None,
-    title: str | None = None,
-    description: str | None = None,
-    exclude: AbstractSet[int | str] | Mapping[int | str, Any] | Any | None = None,
-    include: AbstractSet[int | str] | Mapping[int | str, Any] | Any | None = None,
-    const: bool | None = None,
-    gt: float | None = None,
-    ge: float | None = None,
-    lt: float | None = None,
-    le: float | None = None,
-    multiple_of: float | None = None,
-    max_digits: int | None = None,
-    decimal_places: int | None = None,
-    min_items: int | None = None,
-    max_items: int | None = None,
-    unique_items: bool | None = None,
-    min_length: int | None = None,
-    max_length: int | None = None,
-    allow_mutation: bool = True,
-    regex: str | None = None,
-    discriminator: str | None = None,
-    repr: bool = True,
-    primary_key: bool = False,
-    index: bool | IndexType | Index | None = None,
-    expire: int | None = None,
-    unique: bool = False,
-    **extra: Any,
-) -> Any:
-    """
-    primary_key: 主键
-    index: 索引
-    expire: 到期时间, int 表示创建后多少秒后到期, datetime 表示到期时间
-    unique: 唯一索引
-    """
-    field_info = FieldInfo(
-        default,
-        default_factory=default_factory,
-        alias=alias,
-        title=title,
-        description=description,
-        exclude=exclude,
-        include=include,
-        const=const,
-        gt=gt,
-        ge=ge,
-        lt=lt,
-        le=le,
-        multiple_of=multiple_of,
-        max_digits=max_digits,
-        decimal_places=decimal_places,
-        min_items=min_items,
-        max_items=max_items,
-        unique_items=unique_items,
-        min_length=min_length,
-        max_length=max_length,
-        allow_mutation=allow_mutation,
-        regex=regex,
-        discriminator=discriminator,
-        repr=repr,
-        primary_key=primary_key,
-        index=index,
-        expire=expire,
-        unique=unique,
-        **extra,
-    )
-    field_info._validate()
-    return field_info
+from collections.abc import Callable, Generator, Mapping, Set
+from typing import Any, AnyStr
+
+from bson import ObjectId
+from pydantic.fields import FieldInfo as PDFieldInfo
+from pydantic.fields import Undefined
+from pydantic.typing import NoArgAnyCallable
+from typing_extensions import Self
+
+from mango.index import Index, IndexType
+
+
+class ObjectIdField(ObjectId):
+    @classmethod
+    def __get_validators__(cls) -> Generator[Callable[[AnyStr], Self], None, None]:
+        yield cls.validate
+
+    @classmethod
+    def validate(cls, v: AnyStr) -> Self:
+        if cls.is_valid(v):
+            return cls(v)
+        raise ValueError("无效的 ObjectId")
+
+    @classmethod
+    def __modify_schema__(cls, field_schema: dict) -> None:
+        field_schema.update(type="string")
+
+
+class FieldInfo(PDFieldInfo):
+    def __init__(self, default: Any = Undefined, **kwargs: Any) -> None:
+        self.primary_key: bool = kwargs.pop("primary_key", False)
+        self.index: bool | IndexType | Index | None = kwargs.pop("index", None)
+        self.expire: int | None = kwargs.pop("expire", None)
+        self.unique: bool = kwargs.pop("unique", None)
+        super().__init__(default=default, **kwargs)
+
+
+def Field(
+    default: Any = Undefined,
+    *,
+    default_factory: NoArgAnyCallable | None = None,
+    alias: str | None = None,
+    title: str | None = None,
+    description: str | None = None,
+    exclude: Set[int | str] | Mapping[int | str, Any] | Any | None = None,
+    include: Set[int | str] | Mapping[int | str, Any] | Any | None = None,
+    const: bool | None = None,
+    gt: float | None = None,
+    ge: float | None = None,
+    lt: float | None = None,
+    le: float | None = None,
+    multiple_of: float | None = None,
+    max_digits: int | None = None,
+    decimal_places: int | None = None,
+    min_items: int | None = None,
+    max_items: int | None = None,
+    unique_items: bool | None = None,
+    min_length: int | None = None,
+    max_length: int | None = None,
+    allow_mutation: bool = True,
+    regex: str | None = None,
+    discriminator: str | None = None,
+    repr: bool = True,
+    primary_key: bool = False,
+    index: bool | IndexType | Index | None = None,
+    expire: int | None = None,
+    unique: bool = False,
+    **extra: Any,
+) -> Any:
+    """
+    primary_key: 主键
+    index: 索引
+    expire: 到期时间, int 表示创建后多少秒后到期, datetime 表示到期时间
+    unique: 唯一索引
+    """
+    field_info = FieldInfo(
+        default,
+        default_factory=default_factory,
+        alias=alias,
+        title=title,
+        description=description,
+        exclude=exclude,
+        include=include,
+        const=const,
+        gt=gt,
+        ge=ge,
+        lt=lt,
+        le=le,
+        multiple_of=multiple_of,
+        max_digits=max_digits,
+        decimal_places=decimal_places,
+        min_items=min_items,
+        max_items=max_items,
+        unique_items=unique_items,
+        min_length=min_length,
+        max_length=max_length,
+        allow_mutation=allow_mutation,
+        regex=regex,
+        discriminator=discriminator,
+        repr=repr,
+        primary_key=primary_key,
+        index=index,
+        expire=expire,
+        unique=unique,
+        **extra,
+    )
+    field_info._validate()
+    return field_info
```

### Comparing `mango_odm-0.3.0/mango/index.py` & `mango_odm-0.3.1/mango/index.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from collections.abc import Mapping
-from enum import Enum, unique
-from typing import Any, TypeAlias
-
-import pymongo
-
-
-class IndexEnum(Enum):
-    def __str__(self) -> str:
-        return self.name
-
-
-@unique
-class Order(int, IndexEnum):
-    ASC = pymongo.ASCENDING
-    """升序排序"""
-    DESC = pymongo.DESCENDING
-    """降序排序"""
-
-
-@unique
-class Attr(str, IndexEnum):
-    GEO2D = pymongo.GEO2D
-    """二维地理空间索引"""
-    GEOSPHERE = pymongo.GEOSPHERE
-    """球型地理空间索引"""
-    HASHED = pymongo.HASHED
-    """散列索引"""
-    TEXT = pymongo.TEXT
-    """文本索引"""
-
-
-IndexType: TypeAlias = Order | Attr
-IndexTuple: TypeAlias = tuple[str, IndexType | Mapping[str, Any]]
-
-
-class Index(pymongo.IndexModel):
-    ASC = Order.ASC
-    """升序排序"""
-    DESC = Order.DESC
-    """降序排序"""
-    GEO2D = Attr.GEO2D
-    """二维地理空间索引"""
-    GEOSPHERE = Attr.GEOSPHERE
-    """球型地理空间索引"""
-    HASHED = Attr.HASHED
-    """散列索引"""
-    TEXT = Attr.TEXT
-    """文本索引"""
-
-    def __init__(
-        self,
-        *keys: str | IndexTuple,
-        name: str | None = None,
-        unique: bool = False,
-        background: bool = False,
-        sparse: bool = False,
-        **kwargs: Any,
-    ) -> None:
-        keys = tuple((k, self.ASC) if isinstance(k, str) else k for k in keys)
-        params = {
-            "name": name,
-            "unique": unique,
-            "background": background,
-            "sparse": sparse,
-        }
-        params = {k: v for k, v in params.items() if v}
-        super().__init__(
-            keys,
-            **params,
-            **kwargs,
-        )
+from collections.abc import Mapping
+from enum import Enum, unique
+from typing import Any, TypeAlias
+
+import pymongo
+
+
+class IndexEnum(Enum):
+    def __str__(self) -> str:
+        return self.name
+
+
+@unique
+class Order(int, IndexEnum):
+    ASC = pymongo.ASCENDING
+    """升序排序"""
+    DESC = pymongo.DESCENDING
+    """降序排序"""
+
+
+@unique
+class Attr(str, IndexEnum):
+    GEO2D = pymongo.GEO2D
+    """二维地理空间索引"""
+    GEOSPHERE = pymongo.GEOSPHERE
+    """球型地理空间索引"""
+    HASHED = pymongo.HASHED
+    """散列索引"""
+    TEXT = pymongo.TEXT
+    """文本索引"""
+
+
+IndexType: TypeAlias = Order | Attr
+IndexTuple: TypeAlias = tuple[str, IndexType | Mapping[str, Any]]
+
+
+class Index(pymongo.IndexModel):
+    ASC = Order.ASC
+    """升序排序"""
+    DESC = Order.DESC
+    """降序排序"""
+    GEO2D = Attr.GEO2D
+    """二维地理空间索引"""
+    GEOSPHERE = Attr.GEOSPHERE
+    """球型地理空间索引"""
+    HASHED = Attr.HASHED
+    """散列索引"""
+    TEXT = Attr.TEXT
+    """文本索引"""
+
+    def __init__(
+        self,
+        *keys: str | IndexTuple,
+        name: str | None = None,
+        unique: bool = False,
+        background: bool = False,
+        sparse: bool = False,
+        **kwargs: Any,
+    ) -> None:
+        keys = tuple((k, self.ASC) if isinstance(k, str) else k for k in keys)
+        params = {
+            "name": name,
+            "unique": unique,
+            "background": background,
+            "sparse": sparse,
+        }
+        params = {k: v for k, v in params.items() if v}
+        super().__init__(
+            keys,
+            **params,
+            **kwargs,
+        )
```

### Comparing `mango_odm-0.3.0/mango/models.py` & `mango_odm-0.3.1/mango/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,257 +1,268 @@
-import contextlib
-from collections.abc import Mapping, MutableMapping, Sequence
-from functools import reduce
-from typing import TYPE_CHECKING, Any, ClassVar
-
-import bson
-from bson import ObjectId
-from bson.codec_options import CodecOptions
-from pydantic import BaseModel
-from pydantic.fields import ModelField
-from pydantic.main import ModelMetaclass
-from pymongo.results import DeleteResult, UpdateResult
-from typing_extensions import Self, dataclass_transform
-
-from mango.drive import Collection, Database
-from mango.encoder import Encoder
-from mango.expression import Expression, ExpressionField, Operators
-from mango.fields import Field, FieldInfo, ObjectIdField
-from mango.meta import MetaConfig, inherit_meta
-from mango.result import AggregateResult, FindMapping, FindResult
-from mango.source import Mango
-from mango.stage import Pipeline
-from mango.utils import add_fields, all_check, validate_fields
-
-operators = tuple(str(i) for i in Operators)
-
-
-def is_need_default_pk(
-    bases: tuple[type[Any], ...], annotate: dict[str, Any] | None = None
-) -> bool:
-    # 未定义任何字段
-    if not annotate:
-        return False
-
-    # 存在 id 字段但未定义主键
-    if "id" in annotate:
-        return False
-
-    # 存在 id 字段但未定义主键，且其被继承
-    return not any(getattr(base, "id", None) for base in bases)
-
-
-def set_default_pk(model: type["Document"]) -> None:
-    value = Field(default_factory=ObjectId, allow_mutation=False, init=False)
-    add_fields(model, id=(ObjectIdField, value))
-    model.__primary_key__ = "id"
-
-
-def flat_filter(data: Mapping[str, Any]) -> dict[str, Any]:
-    flatted = {}
-    for key, value in data.items():
-        if key.startswith(operators):
-            flatted |= flat_filter(reduce(lambda x, y: x | y, value))
-        elif "." in key:
-            parent, child = key.split(".", maxsplit=1)
-            flatted[parent] = flat_filter({child: value})
-        else:
-            for operator in operators:
-                if ov := value.get(operator):
-                    flatted[key] = ov
-    return flatted
-
-
-def merge_map(data: MutableMapping[Any, Any], into: Mapping[Any, Any]) -> None:
-    for k, v in into.items():
-        k = str(k)
-        if isinstance(data.get(k), dict) and isinstance(v, dict | EmbeddedDocument):
-            merge_map(data[k], v if isinstance(v, dict) else v.dict())
-        else:
-            data[k] = v
-
-
-@dataclass_transform(kw_only_default=True, field_specifiers=(Field, FieldInfo))
-class MetaDocument(ModelMetaclass):
-    def __new__(
-        cls,
-        cname: str,
-        bases: tuple[type[Any], ...],
-        attrs: dict[str, Any],
-        **kwargs: Any,
-    ):
-        meta = MetaConfig
-
-        for base in reversed(bases):
-            if base != BaseModel and issubclass(base, Document):
-                meta = inherit_meta(base.__meta__, MetaConfig)
-
-        kwargs.setdefault("database", kwargs.pop("db", None))
-
-        allowed_meta_kwargs = {
-            key
-            for key in dir(meta)
-            if not (key.startswith("__") and key.endswith("__"))
-        }
-        meta_kwargs = {
-            key: kwargs.pop(key) for key in kwargs.keys() & allowed_meta_kwargs
-        }
-
-        attrs["__meta__"] = inherit_meta(attrs.get("Meta"), meta, **meta_kwargs)
-        attrs["__encoder__"] = Encoder.create(attrs["__meta__"].bson_encoders)
-
-        scls = super().__new__(cls, cname, bases, attrs, **kwargs)
-
-        # 由于此处代码使用了 setattr，导致子类重写父类的字段时会引发错误，暂无解决办法
-        # NameError: Field name "xxx" shadows a BaseModel attribute;
-        # use a different field name with "alias='xxx'".
-        for fname, field in scls.__fields__.items():
-            setattr(scls, fname, ExpressionField(field, []))
-            if isinstance(finfo := field.field_info, FieldInfo) and finfo.primary_key:
-                pk = finfo.alias or fname
-                if getattr(scls, "__primary_key__", pk) != pk:
-                    raise ValueError("文档的主键应唯一")
-                finfo.allow_mutation = False
-                scls.__primary_key__ = pk
-
-        if not hasattr(scls, "__primary_key__") and is_need_default_pk(
-            bases, attrs.get("__annotations__")
-        ):
-            set_default_pk(scls)
-
-        Mango.register_model(scls)
-
-        return scls
-
-
-@dataclass_transform(kw_only_default=True, field_specifiers=(Field, FieldInfo))
-class MetaEmbeddedDocument(ModelMetaclass):
-    def __new__(
-        cls,
-        name: str,
-        bases: tuple[type[Any], ...],
-        attrs: dict[str, Any],
-        **kwargs: Any,
-    ):
-        scls = super().__new__(cls, name, bases, attrs, **kwargs)
-        for fname, field in scls.__fields__.items():
-            setattr(scls, fname, ExpressionField(field, []))
-            if isinstance(finfo := field.field_info, FieldInfo) and finfo.primary_key:
-                raise ValueError("内嵌文档不可设置主键")
-        return scls
-
-
-class Document(BaseModel, metaclass=MetaDocument):
-
-    if TYPE_CHECKING:  # pragma: no cover
-        id: ClassVar[ObjectId]
-        __fields__: ClassVar[dict[str, ModelField]]
-        __meta__: ClassVar[type[MetaConfig]]
-        __encoder__: ClassVar[CodecOptions]
-        __collection__: ClassVar[Collection]
-        __primary_key__: ClassVar[str]
-
-        def __init_subclass__(
-            cls,
-            *,
-            name: str | None = None,
-            db: Database | str | None = None,
-            **kwargs: Any,
-        ) -> None:
-            ...
-
-    Meta = MetaConfig
-
-    @property
-    def pk(self) -> Any:
-        """主键值"""
-        return getattr(self, self.__primary_key__)
-
-    async def save(self) -> Self:
-        """保存文档"""
-        await self.__collection__.insert_one(self.doc())
-        return self
-
-    async def update(self, **kwargs: Any) -> bool:
-        """更新文档"""
-        if kwargs:
-            values = validate_fields(self.__class__, kwargs)
-            self = self.copy(update=values)
-        result: UpdateResult = await self.__collection__.update_one(
-            {"_id": self.pk}, {"$set": self.doc(exclude={self.__primary_key__})}
-        )
-        return bool(result.modified_count)
-
-    async def delete(self) -> bool:
-        """删除文档"""
-        result: DeleteResult = await self.__collection__.delete_one({"_id": self.pk})
-        return bool(result.deleted_count)
-
-    def doc(self, **kwargs: Any) -> dict[str, Any]:
-        """转换为 MongoDB 文档"""
-        kwargs["by_alias"] = self.__meta__.by_alias
-        data = self.dict(**kwargs)
-        pk = self.__primary_key__
-        exclude = kwargs.get("exclude")
-        if not (exclude and pk in exclude):
-            data["_id"] = data.pop(pk)
-        return bson.decode(bson.encode(data, codec_options=self.__encoder__))
-
-    @classmethod
-    def from_doc(cls, document: dict[str, Any]) -> Self:
-        """从文档构建模型实例"""
-        with contextlib.suppress(KeyError):
-            document[cls.__primary_key__] = document.pop("_id")
-        return cls(**document)
-
-    @classmethod
-    async def save_all(cls, *documents: Self) -> None:
-        """保存全部文档"""
-        await cls.__collection__.insert_many(doc.doc() for doc in documents)
-
-    @classmethod
-    def aggregate(
-        cls, pipeline: Pipeline | Sequence[Mapping[str, Any]], *args: Any, **kwargs: Any
-    ) -> AggregateResult:
-        """聚合查询"""
-        cursor = cls.__collection__.aggregate(pipeline, *args, **kwargs)
-        return AggregateResult(cursor)
-
-    @classmethod
-    def find(
-        cls,
-        *args: FindMapping | Expression | bool,
-    ) -> FindResult[Self]:
-        """使用表达式查询文档"""
-        if all_check(args, Expression | Mapping):
-            return FindResult(cls, *args)  # type: ignore
-        else:
-            raise TypeError("查询表达式类型不正确")
-
-    @classmethod
-    async def get(cls, _id: Any) -> Self | None:
-        """通过主键查询文档"""
-        return await cls.find({"_id": _id}).get()
-
-    @classmethod
-    async def get_or_create(
-        cls,
-        *args: FindMapping | Expression | bool,
-        defaults: FindMapping | Self | None = None,
-    ) -> Self:
-        """获取文档, 如果不存在, 则创建"""
-        result: FindResult[Self] = FindResult(cls, *args)  # type: ignore
-        if model := await result.get():
-            return model
-        default = defaults.doc() if isinstance(defaults, Document) else defaults or {}
-        data = flat_filter(result.filter)
-        merge_map(data, default)
-        model = cls.from_doc(data)
-        return await model.save()
-
-    class Config:
-        validate_assignment = True
-
-
-class EmbeddedDocument(BaseModel, metaclass=MetaEmbeddedDocument):
-    class Config:
-        validate_assignment = True
+import contextlib
+from collections.abc import Mapping, MutableMapping, Sequence
+from functools import reduce
+from typing import TYPE_CHECKING, Any, ClassVar
+
+import bson
+from bson import ObjectId
+from pydantic import BaseModel
+from pydantic.main import ModelMetaclass
+from typing_extensions import Self, dataclass_transform
+
+from mango.encoder import Encoder
+from mango.expression import Expression, ExpressionField, Operators
+from mango.fields import Field, FieldInfo, ObjectIdField
+from mango.meta import MetaConfig, inherit_meta
+from mango.result import AggregateResult, FindMapping, FindResult
+from mango.source import Mango
+from mango.stage import Pipeline
+from mango.utils import add_fields, all_check, validate_fields
+
+if TYPE_CHECKING:
+    from bson.codec_options import CodecOptions
+    from pydantic.fields import ModelField
+    from pymongo.results import DeleteResult, UpdateResult
+
+    from mango.drive import Collection, Database
+
+operators = tuple(str(i) for i in Operators)
+
+
+def is_need_default_pk(
+    bases: tuple[type[Any], ...], annotate: dict[str, Any] | None = None
+) -> bool:
+    # 未定义任何字段
+    if not annotate:
+        return False
+
+    # 存在 id 字段但未定义主键
+    if "id" in annotate:
+        return False
+
+    # 存在 id 字段但未定义主键，且其被继承
+    return not any(getattr(base, "id", None) for base in bases)
+
+
+def set_default_pk(model: type["Document"]) -> None:
+    value = Field(default_factory=ObjectId, allow_mutation=False, init=False)
+    add_fields(model, id=(ObjectIdField, value))
+    model.__primary_key__ = "id"
+
+
+def flat_filter(data: Mapping[str, Any]) -> dict[str, Any]:
+    flatted = {}
+    for key, value in data.items():
+        if key.startswith(operators):
+            flatted |= flat_filter(reduce(lambda x, y: x | y, value))
+        elif "." in key:
+            parent, child = key.split(".", maxsplit=1)
+            flatted[parent] = flat_filter({child: value})
+        else:
+            for operator in operators:
+                if ov := value.get(operator):
+                    flatted[key] = ov
+    return flatted
+
+
+def merge_map(data: MutableMapping[Any, Any], into: Mapping[Any, Any]) -> None:
+    for k, v in into.items():
+        k = str(k)
+        if isinstance(data.get(k), dict) and isinstance(v, dict | EmbeddedDocument):
+            merge_map(data[k], v if isinstance(v, dict) else v.dict())
+        else:
+            data[k] = v
+
+
+@dataclass_transform(kw_only_default=True, field_specifiers=(Field, FieldInfo))
+class MetaDocument(ModelMetaclass):
+    def __new__(
+        cls,
+        cname: str,
+        bases: tuple[type[Any], ...],
+        attrs: dict[str, Any],
+        **kwargs: Any,
+    ) -> Any:
+        meta = MetaConfig
+
+        for base in reversed(bases):
+            if base != BaseModel and issubclass(base, Document):
+                meta = inherit_meta(base.__meta__, MetaConfig)
+
+        kwargs.setdefault("database", kwargs.pop("db", None))
+
+        allowed_meta_kwargs = {
+            key
+            for key in dir(meta)
+            if not (key.startswith("__") and key.endswith("__"))
+        }
+        meta_kwargs = {
+            key: kwargs.pop(key) for key in kwargs.keys() & allowed_meta_kwargs
+        }
+
+        attrs["__meta__"] = inherit_meta(attrs.get("Meta"), meta, **meta_kwargs)
+        attrs["__encoder__"] = Encoder.create(attrs["__meta__"].bson_encoders)
+
+        scls = super().__new__(cls, cname, bases, attrs, **kwargs)
+
+        # 由于此处代码使用了 setattr，导致子类重写父类的字段时会引发错误，暂无解决办法
+        # NameError: Field name "xxx" shadows a BaseModel attribute;
+        # use a different field name with "alias='xxx'".
+        for fname, field in scls.__fields__.items():
+            setattr(scls, fname, ExpressionField(field, []))
+            if isinstance(finfo := field.field_info, FieldInfo) and finfo.primary_key:
+                pk = finfo.alias or fname
+                if getattr(scls, "__primary_key__", pk) != pk:
+                    raise ValueError("文档的主键应唯一")
+                finfo.allow_mutation = False
+                scls.__primary_key__ = pk
+
+        if not hasattr(scls, "__primary_key__") and is_need_default_pk(
+            bases, attrs.get("__annotations__")
+        ):
+            set_default_pk(scls)
+
+        Mango.register_model(scls)
+
+        return scls
+
+
+@dataclass_transform(kw_only_default=True, field_specifiers=(Field, FieldInfo))
+class MetaEmbeddedDocument(ModelMetaclass):
+    def __new__(
+        cls,
+        name: str,
+        bases: tuple[type[Any], ...],
+        attrs: dict[str, Any],
+        **kwargs: Any,
+    ) -> Any:
+        scls = super().__new__(cls, name, bases, attrs, **kwargs)
+        for fname, field in scls.__fields__.items():
+            setattr(scls, fname, ExpressionField(field, []))
+            if isinstance(finfo := field.field_info, FieldInfo) and finfo.primary_key:
+                raise ValueError("内嵌文档不可设置主键")
+        return scls
+
+
+class Document(BaseModel, metaclass=MetaDocument):
+    if TYPE_CHECKING:  # pragma: no cover
+        id: ClassVar[ObjectId]
+        __fields__: ClassVar[dict[str, ModelField]]
+        __meta__: ClassVar[type[MetaConfig]]
+        __encoder__: ClassVar[CodecOptions]
+        __collection__: ClassVar[Collection]
+        __primary_key__: ClassVar[str]
+
+        def __init_subclass__(
+            cls,
+            *,
+            name: str | None = None,
+            db: Database | str | None = None,
+            **kwargs: Any,
+        ) -> None:
+            ...
+
+    Meta = MetaConfig
+
+    @property
+    def pk(self) -> Any:
+        """主键值"""
+        return getattr(self, self.__primary_key__)
+
+    async def insert(self) -> Self:
+        """插入文档"""
+        await self.__collection__.insert_one(self.doc())
+        return self
+
+    async def update(self, **kwargs: Any) -> bool:
+        """更新文档"""
+        if kwargs:
+            values = validate_fields(self.__class__, kwargs)
+            for field, value in values.items():
+                setattr(self, field, value)
+        result: UpdateResult = await self.__collection__.update_one(
+            {"_id": self.pk}, {"$set": self.doc(exclude={self.__primary_key__})}
+        )
+        return bool(result.modified_count)
+
+    async def save(self, **kwargs: Any) -> Self:
+        """保存文档，如果文档不存在，则插入，否则更新它。"""
+        existing_doc = await self.__collection__.find_one({"_id": self.pk})
+        if existing_doc:
+            await self.update(**kwargs)
+        else:
+            await self.insert()
+        return self
+
+    async def delete(self) -> bool:
+        """删除文档"""
+        result: DeleteResult = await self.__collection__.delete_one({"_id": self.pk})
+        return bool(result.deleted_count)
+
+    def doc(self, **kwargs: Any) -> dict[str, Any]:
+        """转换为 MongoDB 文档"""
+        kwargs["by_alias"] = self.__meta__.by_alias
+        data = self.dict(**kwargs)
+        pk = self.__primary_key__
+        exclude = kwargs.get("exclude")
+        if not (exclude and pk in exclude):
+            data["_id"] = data.pop(pk)
+        return bson.decode(bson.encode(data, codec_options=self.__encoder__))
+
+    @classmethod
+    def from_doc(cls, document: dict[str, Any]) -> Self:
+        """从文档构建模型实例"""
+        with contextlib.suppress(KeyError):
+            document[cls.__primary_key__] = document.pop("_id")
+        return cls(**document)
+
+    @classmethod
+    async def save_all(cls, *documents: Self) -> None:
+        """保存全部文档"""
+        await cls.__collection__.insert_many(doc.doc() for doc in documents)
+
+    @classmethod
+    def aggregate(
+        cls, pipeline: Pipeline | Sequence[Mapping[str, Any]], *args: Any, **kwargs: Any
+    ) -> AggregateResult:
+        """聚合查询"""
+        cursor = cls.__collection__.aggregate(pipeline, *args, **kwargs)
+        return AggregateResult(cursor)
+
+    @classmethod
+    def find(
+        cls,
+        *args: FindMapping | Expression | bool,
+    ) -> FindResult[Self]:
+        """使用表达式查询文档"""
+        if all_check(args, Expression | Mapping):
+            return FindResult(cls, *args)  # type: ignore
+        raise TypeError("查询表达式类型不正确")
+
+    @classmethod
+    async def get(cls, _id: Any) -> Self | None:
+        """通过主键查询文档"""
+        return await cls.find({"_id": _id}).get()
+
+    @classmethod
+    async def get_or_create(
+        cls,
+        *args: FindMapping | Expression | bool,
+        defaults: FindMapping | Self | None = None,
+    ) -> Self:
+        """获取文档, 如果不存在, 则创建"""
+        result: FindResult[Self] = FindResult(cls, *args)  # type: ignore
+        if model := await result.get():
+            return model
+        default = defaults.doc() if isinstance(defaults, Document) else defaults or {}
+        data = flat_filter(result.filter)
+        merge_map(data, default)
+        model = cls.from_doc(data)
+        return await model.save()
+
+    class Config:
+        validate_assignment = True
+
+
+class EmbeddedDocument(BaseModel, metaclass=MetaEmbeddedDocument):
+    class Config:
+        validate_assignment = True
```

### Comparing `mango_odm-0.3.0/mango/result.py` & `mango_odm-0.3.1/mango/result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,188 +1,190 @@
-from collections.abc import AsyncGenerator, Generator, Mapping
-from typing import TYPE_CHECKING, Any, Generic, TypeAlias, TypeVar
-
-from motor.motor_asyncio import AsyncIOMotorCursor, AsyncIOMotorLatentCommandCursor
-from pydantic import BaseModel
-from pymongo.results import DeleteResult
-
-from mango.expression import Expression, ExpressionField
-from mango.index import Order
-from mango.utils import any_check, is_sequence, validate_fields
-
-if TYPE_CHECKING:  # pragma: no cover
-    from mango.models import Document
-
-T_Model = TypeVar("T_Model", bound="Document")
-
-KeyField: TypeAlias = str | ExpressionField
-
-FindMapping: TypeAlias = Mapping[KeyField, Any]
-
-DirectionType: TypeAlias = Order
-
-SortType: TypeAlias = tuple[str, DirectionType]
-
-
-class FindOptions(BaseModel):
-    limit: int = 0
-    skip: int = 0
-    sort: list[SortType] = []
-
-    def kwdict(self, *exclude: str) -> dict[str, Any]:
-        return self.dict(exclude=set(exclude), exclude_defaults=True)
-
-
-class FindResult(Generic[T_Model]):
-    def __init__(
-        self,
-        model: type[T_Model],
-        *filter: FindMapping | Expression,
-    ) -> None:
-        self.model = model
-        self.collection = model.__collection__
-        self._filter = filter
-        self.options = FindOptions()
-
-    def __await__(self) -> Generator[None, None, list[T_Model]]:
-        """`await` : 等待时，将返回获取的模型列表"""
-        documents = yield from self.cursor.to_list(length=None).__await__()
-        instances: list[T_Model] = []
-        for document in documents:
-            instances.append(self.model.from_doc(document))
-            yield
-        return instances
-
-    async def __aiter__(self) -> AsyncGenerator[T_Model, None]:
-        """`async for`: 异步迭代查询结果"""
-        async for document in self.cursor:  # type: ignore
-            yield self.model.from_doc(document)
-
-    @property
-    def cursor(self) -> AsyncIOMotorCursor:
-        return self.collection.find(self.filter, **self.options.kwdict())
-
-    @property
-    def filter(self) -> dict[str, Any]:
-        """查询过滤条件"""
-        compiled: dict[str, Any] = {}
-        for condition in self._filter:
-            if isinstance(condition, Mapping):
-                condition = dict(condition)
-            elif isinstance(condition, Expression):
-                condition = condition.struct()
-            else:
-                raise TypeError("查询过滤条件不正确, 应为映射或表达式")
-            compiled |= self._compile(condition)
-        return compiled
-
-    def _compile(
-        self,
-        source: Mapping[KeyField, Any] | Mapping[str, Any],
-    ) -> dict[str, Any]:
-        compiled: dict[str, Any] = {}
-
-        for key, value in source.items():
-            key = str(key)
-            if isinstance(value, Expression):
-                compiled[key] = value.struct()
-            elif isinstance(value, Mapping):
-                compiled[key] = self._compile(value)
-            elif is_sequence(value):
-                compiled[key] = []
-                for i in value:
-                    if isinstance(i, Expression):
-                        i = i.struct()
-                    if isinstance(i, Mapping):
-                        i = self._compile(i)
-                    compiled[key].append(i)
-            else:
-                compiled[key] = value
-
-        return compiled
-
-    def limit(self, limit: int = 0) -> "FindResult[T_Model]":
-        """限制查询条件返回结果的数量"""
-        self.options.limit += limit
-        return self
-
-    def skip(self, skip: int = 0) -> "FindResult[T_Model]":
-        """跳过指定数目的文档"""
-        self.options.skip += skip
-        return self
-
-    def sort(self, *orders: Any) -> "FindResult[T_Model]":
-        """对查询文档流进行排序"""
-        if not (len(orders) != 2 or any_check(orders, is_sequence)):
-            orders = (orders,)
-        for order in orders:
-            direction = Order.ASC
-            if is_sequence(order):
-                key, direction = order
-            else:
-                key = order
-
-            try:
-                key, direction = str(key), Order(direction)
-            except ValueError as e:
-                raise TypeError("键应为字符串或字段, 排序方向应为 Order 枚举成员") from e
-            else:
-                self.options.sort.append((key, direction))
-
-        return self
-
-    def asc(self, *keys: Any) -> "FindResult[T_Model]":
-        """升序排列"""
-        self.options.sort.extend(self._sort_order(*keys))
-        return self
-
-    def desc(self, *keys: Any) -> "FindResult[T_Model]":
-        """降序排列"""
-        self.options.sort.extend(self._sort_order(*keys, reverse=True))
-        return self
-
-    def _sort_order(
-        self, *keys: Any, reverse: bool = False
-    ) -> Generator[SortType, None, None]:
-        direction: Order = Order.DESC if reverse else Order.ASC
-        for key in keys:
-            yield str(key), direction
-
-    async def count(self) -> int:
-        """获得符合条件的文档总数"""
-        return await self.collection.count_documents(
-            self.filter, **self.options.kwdict("sort")
-        )
-
-    async def get(self) -> T_Model | None:
-        """
-        从数据库中获取单个文档。
-        返回单个文档，如果没有找到匹配的文档，返回“None”。
-        """
-        if document := await self.collection.find_one(self.filter):
-            return self.model.from_doc(document)
-
-    async def delete(self) -> int:
-        """删除符合条件的文档"""
-        result: DeleteResult = await self.collection.delete_many(self.filter)
-        return result.deleted_count
-
-    async def update(self, **kwargs: Any) -> None:
-        """使用提供的信息更新查找到的文档"""
-        values = validate_fields(self.model, kwargs)
-        await self.collection.update_many(self.filter, {"$set": values})
-
-
-class AggregateResult:
-    def __init__(self, cursor: AsyncIOMotorLatentCommandCursor) -> None:
-        self.cursor = cursor
-
-    def __await__(self) -> Generator[None, None, list[dict[str, Any]]]:
-        """
-        `await` : 等待时，将返回聚合管道的结果文档列表
-        """
-        return (yield from self.cursor.to_list(length=None).__await__())
-
-    async def __aiter__(self) -> AsyncGenerator[dict[str, Any], None]:
-        """`async for`: 异步迭代聚合管道的结果文档"""
-        async for document in self.cursor:  # type: ignore
-            yield document
+from collections.abc import AsyncGenerator, Generator, Mapping
+from typing import TYPE_CHECKING, Any, Generic, TypeAlias, TypeVar
+
+from motor.motor_asyncio import AsyncIOMotorCursor, AsyncIOMotorLatentCommandCursor
+from pydantic import BaseModel
+
+from mango.expression import Expression, ExpressionField
+from mango.index import Order
+from mango.utils import any_check, is_sequence, validate_fields
+
+if TYPE_CHECKING:  # pragma: no cover
+    from pymongo.results import DeleteResult
+
+    from mango.models import Document
+
+T_Model = TypeVar("T_Model", bound="Document")
+
+KeyField: TypeAlias = str | ExpressionField
+
+FindMapping: TypeAlias = Mapping[KeyField, Any]
+
+DirectionType: TypeAlias = Order
+
+SortType: TypeAlias = tuple[str, DirectionType]
+
+
+class FindOptions(BaseModel):
+    limit: int = 0
+    skip: int = 0
+    sort: list[SortType] = []
+
+    def kwdict(self, *exclude: str) -> dict[str, Any]:
+        return self.dict(exclude=set(exclude), exclude_defaults=True)
+
+
+class FindResult(Generic[T_Model]):
+    def __init__(
+        self,
+        model: type[T_Model],
+        *filter: FindMapping | Expression,
+    ) -> None:
+        self.model = model
+        self.collection = model.__collection__
+        self._filter = filter
+        self.options = FindOptions()
+
+    def __await__(self) -> Generator[None, None, list[T_Model]]:
+        """`await` : 等待时，将返回获取的模型列表"""
+        documents = yield from self.cursor.to_list(length=None).__await__()
+        instances: list[T_Model] = []
+        for document in documents:
+            instances.append(self.model.from_doc(document))
+            yield
+        return instances
+
+    async def __aiter__(self) -> AsyncGenerator[T_Model, None]:
+        """`async for`: 异步迭代查询结果"""
+        async for document in self.cursor:  # type: ignore
+            yield self.model.from_doc(document)
+
+    @property
+    def cursor(self) -> AsyncIOMotorCursor:
+        return self.collection.find(self.filter, **self.options.kwdict())
+
+    @property
+    def filter(self) -> dict[str, Any]:
+        """查询过滤条件"""
+        compiled: dict[str, Any] = {}
+        for condition in self._filter:
+            if isinstance(condition, Mapping):
+                condition = dict(condition)
+            elif isinstance(condition, Expression):
+                condition = condition.struct()
+            else:
+                raise TypeError("查询过滤条件不正确, 应为映射或表达式")
+            compiled |= self._compile(condition)
+        return compiled
+
+    def _compile(
+        self,
+        source: Mapping[KeyField, Any] | Mapping[str, Any],
+    ) -> dict[str, Any]:
+        compiled: dict[str, Any] = {}
+
+        for key, value in source.items():
+            key = str(key)
+            if isinstance(value, Expression):
+                compiled[key] = value.struct()
+            elif isinstance(value, Mapping):
+                compiled[key] = self._compile(value)
+            elif is_sequence(value):
+                compiled[key] = []
+                for i in value:
+                    if isinstance(i, Expression):
+                        i = i.struct()
+                    if isinstance(i, Mapping):
+                        i = self._compile(i)
+                    compiled[key].append(i)
+            else:
+                compiled[key] = value
+
+        return compiled
+
+    def limit(self, limit: int = 0) -> "FindResult[T_Model]":
+        """限制查询条件返回结果的数量"""
+        self.options.limit += limit
+        return self
+
+    def skip(self, skip: int = 0) -> "FindResult[T_Model]":
+        """跳过指定数目的文档"""
+        self.options.skip += skip
+        return self
+
+    def sort(self, *orders: Any) -> "FindResult[T_Model]":
+        """对查询文档流进行排序"""
+        if not (len(orders) != 2 or any_check(orders, is_sequence)):  # noqa: PLR2004
+            orders = (orders,)
+        for order in orders:
+            direction = Order.ASC
+            if is_sequence(order):
+                key, direction = order
+            else:
+                key = order
+
+            try:
+                key, direction = str(key), Order(direction)
+            except ValueError as e:
+                raise TypeError("键应为字符串或字段, 排序方向应为 Order 枚举成员") from e
+            else:
+                self.options.sort.append((key, direction))
+
+        return self
+
+    def asc(self, *keys: Any) -> "FindResult[T_Model]":
+        """升序排列"""
+        self.options.sort.extend(self._sort_order(*keys))
+        return self
+
+    def desc(self, *keys: Any) -> "FindResult[T_Model]":
+        """降序排列"""
+        self.options.sort.extend(self._sort_order(*keys, reverse=True))
+        return self
+
+    def _sort_order(
+        self, *keys: Any, reverse: bool = False
+    ) -> Generator[SortType, None, None]:
+        direction: Order = Order.DESC if reverse else Order.ASC
+        for key in keys:
+            yield str(key), direction
+
+    async def count(self) -> int:
+        """获得符合条件的文档总数"""
+        return await self.collection.count_documents(
+            self.filter, **self.options.kwdict("sort")
+        )
+
+    async def get(self) -> T_Model | None:
+        """
+        从数据库中获取单个文档。
+        返回单个文档，如果没有找到匹配的文档，返回“None”。
+        """
+        if document := await self.collection.find_one(self.filter):
+            return self.model.from_doc(document)
+        return None
+
+    async def delete(self) -> int:
+        """删除符合条件的文档"""
+        result: DeleteResult = await self.collection.delete_many(self.filter)
+        return result.deleted_count
+
+    async def update(self, **kwargs: Any) -> None:
+        """使用提供的信息更新查找到的文档"""
+        values = validate_fields(self.model, kwargs)
+        await self.collection.update_many(self.filter, {"$set": values})
+
+
+class AggregateResult:
+    def __init__(self, cursor: AsyncIOMotorLatentCommandCursor) -> None:
+        self.cursor = cursor
+
+    def __await__(self) -> Generator[None, None, list[dict[str, Any]]]:
+        """
+        `await` : 等待时，将返回聚合管道的结果文档列表
+        """
+        return (yield from self.cursor.to_list(length=None).__await__())
+
+    async def __aiter__(self) -> AsyncGenerator[dict[str, Any], None]:
+        """`async for`: 异步迭代聚合管道的结果文档"""
+        async for document in self.cursor:  # type: ignore
+            yield document
```

### Comparing `mango_odm-0.3.0/mango/source.py` & `mango_odm-0.3.1/mango/source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import asyncio
-from typing import TYPE_CHECKING, Any, ClassVar
-
-from mango.drive import DEFAULT_CONNECT_URI, Client
-from mango.utils import get_indexes, to_snake_case
-
-if TYPE_CHECKING:  # pragma: no cover
-    from mango.models import Document
-
-
-async def init_model(model: type["Document"], *, revise_index=False) -> None:
-    """初始化文档模型"""
-    meta = model.__meta__
-    db = Client.get_database(meta.database)
-    model.__collection__ = db[meta.name or to_snake_case(model.__name__)]
-    await init_index(model, revise_index=revise_index)
-
-
-async def init_index(model: type["Document"], *, revise_index=False) -> None:
-    """初始化文档索引"""
-    required = ["_id_"]
-    if indexes := list(get_indexes(model)):
-        required += await model.__collection__.create_indexes(indexes)
-    if revise_index:
-        index_info = await model.__collection__.index_information()
-        for index in set(index_info) - set(required):
-            await model.__collection__.drop_index(index)
-
-
-class Mango:
-    _document_models: ClassVar[set[type["Document"]]] = set()
-
-    @classmethod
-    async def init(
-        cls,
-        db: str | None = None,
-        *,
-        uri: str = DEFAULT_CONNECT_URI,
-        revise_index=False,
-        **kwargs: Any,
-    ) -> None:
-        if db or uri or not Client._clients:
-            cls.connect(db, uri, **kwargs)
-        tasks = [
-            init_model(model, revise_index=revise_index)
-            for model in cls._document_models
-        ]
-        await asyncio.gather(*tasks)
-
-    @classmethod
-    def connect(
-        cls,
-        db: str | None = None,
-        /,
-        uri: str = DEFAULT_CONNECT_URI,
-        **kwargs: Any,
-    ) -> Client:
-        """创建连接"""
-        client = Client(uri, **kwargs)
-        client.get_database(db)
-        return client
-
-    @classmethod
-    def disconnect(cls, *clients: Client) -> None:
-        """断开连接"""
-        for client in Client._clients:
-            if not clients or client in clients:
-                client.close()
-
-    @classmethod
-    def register_model(cls, model: type["Document"]) -> None:
-        """注册模型"""
-        cls._document_models.add(model)
+import asyncio
+from typing import TYPE_CHECKING, Any, ClassVar
+
+from mango.drive import DEFAULT_CONNECT_URI, Client
+from mango.utils import get_indexes, to_snake_case
+
+if TYPE_CHECKING:  # pragma: no cover
+    from mango.models import Document
+
+
+async def init_model(model: type["Document"], *, revise_index: bool = False) -> None:
+    """初始化文档模型"""
+    meta = model.__meta__
+    db = Client.get_database(meta.database)
+    model.__collection__ = db[meta.name or to_snake_case(model.__name__)]
+    await init_index(model, revise_index=revise_index)
+
+
+async def init_index(model: type["Document"], *, revise_index: bool = False) -> None:
+    """初始化文档索引"""
+    required = ["_id_"]
+    if indexes := list(get_indexes(model)):
+        required += await model.__collection__.create_indexes(indexes)
+    if revise_index:
+        index_info = await model.__collection__.index_information()
+        for index in set(index_info) - set(required):
+            await model.__collection__.drop_index(index)
+
+
+class Mango:
+    _document_models: ClassVar[set[type["Document"]]] = set()
+
+    @classmethod
+    async def init(
+        cls,
+        db: str | None = None,
+        *,
+        uri: str = DEFAULT_CONNECT_URI,
+        revise_index: bool = False,
+        **kwargs: Any,
+    ) -> None:
+        if db or uri or not Client._clients:
+            cls.connect(db, uri, **kwargs)
+        tasks = [
+            init_model(model, revise_index=revise_index)
+            for model in cls._document_models
+        ]
+        await asyncio.gather(*tasks)
+
+    @classmethod
+    def connect(
+        cls,
+        db: str | None = None,
+        /,
+        uri: str = DEFAULT_CONNECT_URI,
+        **kwargs: Any,
+    ) -> Client:
+        """创建连接"""
+        client = Client(uri, **kwargs)
+        client.get_database(db)
+        return client
+
+    @classmethod
+    def disconnect(cls, *clients: Client) -> None:
+        """断开连接"""
+        for client in Client._clients.copy():
+            if not clients or client in clients:
+                client.close()
+
+    @classmethod
+    def register_model(cls, model: type["Document"]) -> None:
+        """注册模型"""
+        cls._document_models.add(model)
```

### Comparing `mango_odm-0.3.0/mango/stage.py` & `mango_odm-0.3.1/mango/stage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,353 +1,353 @@
-from collections.abc import Mapping, Sequence
-from typing import Any, Literal, TypeAlias
-
-from typing_extensions import Self
-
-from mango.index import Order
-
-SortOrder: TypeAlias = Order | Literal[1, -1]
-
-
-class Pipeline(list[Mapping[str, Any]]):
-    """聚合管道阶段"""
-
-    def __init__(self, *stages: Mapping[str, Any]) -> None:
-        super().__init__(stages)
-
-    def stage(self, key: str, value: Any) -> Self:
-        """添加一个阶段"""
-        key = key if key.startswith("$") else f"${key}"
-        self.append({key: value})
-        return self
-
-    def bucket(
-        self,
-        group_by: Any,
-        boundaries: Sequence[int | float],
-        default: str | None = None,
-        output: Mapping[str, Mapping[str, Any]] | None = None,
-    ) -> Self:
-        """
-        根据指定的表达式和存储桶边界将传入文档分类到称为存储桶的组中，并为每个存储桶输出一个文档。
-
-        group_by: 对文档进行分组的表达式。若要指定字段路径，请在字段名前面加上符号 `$` 。
-        boundaries: 基于 `group_by` 表达式的值数组，用于指定每个桶的边界。每对相邻的值作为桶的包含下边界和独占上边界。
-        default: 指定一个附加桶的 `_id`，该桶包含 `group_by` 表达式结果中，不属于边界指定的桶的所有文档。
-        output: 指定输出文档中除 `_id` 字段外还要包含的字段。如果未指定文档，则操作返回包含文档数的字段在每个存储桶中。
-
-        [$bucket (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/bucket/)
-        """
-        if len(boundaries) < 2:
-            raise ValueError("必须至少指定两个边界值")
-        if sorted(boundaries) != boundaries:
-            raise ValueError("指定的值必须以升序排列")
-        struct = {
-            "groupBy": group_by,
-            "boundaries": boundaries,
-        }
-        if default:
-            struct["default"] = default
-        if output:
-            struct["output"] = output
-        return self.stage("bucket", struct)
-
-    def count(self, field: str) -> Self:
-        """
-        将文档传递到下一阶段，该阶段包含输入到该阶段的文档数量的计数。
-
-        field : 输出字段的名称，其值为计数结果。必须是非空字符串，不能以 `$` 开头，也不能包含 `.` 字符。
-
-        [$count (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/count/)
-        """
-        if not field or field.startswith("$") or "." in field:
-            raise ValueError("必须是非空字符串, 不能以 `$` 开头，也不能包含 `.` 字符。")
-        return self.stage("count", field)
-
-    def documents(self, expression: Any) -> Self:
-        """
-        从输入值返回原始文档。
-
-        expression: 接受任何解析为映射数组的有效表达式。
-
-        [$documents (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/documents/)
-        """
-        return self.stage("documents", expression)
-
-    def facet(self, **fields: Self | Sequence[Mapping[str, Any]]) -> Self:
-        """
-        在同一组输入文档的单个阶段内处理多个聚合管道。每个子管道在输出文档中都有自己的字段，其结果存储为一个文档数组。
-        输入文档只被传递到 `$facet` 阶段一次。`$facet` 支持对同一组输入文档进行各种聚合，无需多次检索输入文档。
-
-        fields: 参数名为子管道输出的字段名, 参数为需要运行的子管道。
-
-        [$facet (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/facet/)
-        """
-        return self.stage("facet", fields)
-
-    def fill(
-        self,
-        output: Mapping[str, Any],
-        partition_by: Any = None,
-        partition_by_fields: Sequence[str] | None = None,
-        sort_by: Mapping[str, SortOrder] | None = None,
-    ) -> Self:
-        """
-        填充文档中的空值和缺少的字段值。
-
-        output: 指定一个字典，该字典包含要填充缺失值的每个字段输出对象的字典。对象名称是要填充的字段的名称，对象值指定如何填充该字段。
-        partition_by: 指定用于对文档进行分组的表达式。`partition_by` 和 `partition_by_fields` 是互斥的。
-        partition_by_fields: 指定字段数组，以作为文档分组的复合键。`partition_by` 和 `partition_by_fields` 是互斥的。
-        sort_by: 指定用于对每个分区内的文档进行排序的字段。
-
-        [$fill (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/fill/)
-        """
-        struct: dict[str, Any] = {
-            "output": output,
-        }
-        if partition_by:
-            struct["partitionBy"] = partition_by
-        elif partition_by_fields:
-            if isinstance(partition_by_fields, str):
-                raise TypeError("partition_by_fields 不能为字符串")
-            struct["partitionByFields"] = partition_by_fields
-        if sort_by:
-            struct["sortBy"] = sort_by
-        return self.stage("fill", struct)
-
-    def group(self, id: Any, **fields: Mapping[str, Any]) -> Self:
-        """
-        `$group` 阶段根据“组键”将文档分成多个组。
-        组键通常是一个字段或一组字段。组键也可以是表达式的结果。
-        在 `$group` 阶段的输出中，`_id` 字段被设置为该文档的组键。
-        每个输出文档的字段都包含唯一的按值分组。输出文档还可以包含包含某些累加器表达式值的计算字段。
-
-        id: 可以接受任何有效的表达式。如果指定 `id` 为 `None` 或任何其他常数值，那么此 `$group` 阶段将整体计算所有输入文档的累积值。
-        fields: 参数名为额外添加的字段, 参数为累加器表达式。
-
-        [$group (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/group/)
-        """
-        return self.stage("group", {"_id": id, **fields})
-
-    def limit(self, integer: int) -> Self:
-        """
-        限制传递到管道中下一阶段的文档数。
-
-        integer: 指定要传递的文档的最大数量。
-
-        [$limit (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/limit/)
-        """
-        return self.stage("limit", integer)
-
-    def lookup(
-        self,
-        from_: str | None = None,
-        local_field: str | None = None,
-        foreign_field: str | None = None,
-        let: Mapping[str, Any] | None = None,
-        pipeline: Self | Sequence[Mapping[str, Any]] | None = None,
-        as_: str | None = None,
-    ) -> Self:
-        """
-        对同一数据库中的集合执行左外联接，以从“联接”集合中筛选文档进行处理。
-        此 `$lookup` 阶段为每个输入文档添加一个新的数组字段，新的数组字段包含“联接”集合中的匹配文档，并将这些重新成形的文档传递到下一阶段。
-
-        from_: 指定同一数据库中要联接到当前集合的外部集合。
-        local_field: 指定当前集合的文档中的字段。
-        foreign_field: 指定外部集合的文档中的字段。
-        let: 指定要在管道阶段中使用的变量。使用变量表达式访问输入到管道的文档字段。
-        pipeline: 指定要在已联接集合上运行的管道。管道从已联接的集合中确定结果文档。若要返回所有文档，请指定空管道。
-        as_: 指定要添加到输出文档的新数组字段的名称。新的数组字段包含来自 `from_` 集合的匹配文档。如果指定的名称已经存在于输出文档中，则覆盖现有字段。
-
-        [$lookup (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/lookup/)
-        """
-        return self.stage(
-            "lookup",
-            {
-                k: v
-                for k, v in {
-                    "from": from_,
-                    "localField": local_field,
-                    "foreignField": foreign_field,
-                    "let": let,
-                    "pipeline": pipeline,
-                    "as": as_,
-                }.items()
-                if v is None
-            },
-        )
-
-    def match(self, query: Mapping[str, Any]) -> Self:
-        """
-        筛选文档流，仅将匹配指定条件的文档传递到下一个管道阶段。
-
-        query: 指定查询条件。
-
-        [$match (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/match/)
-        """
-        return self.stage("match", query)
-
-    def merge(
-        self,
-        collection: str,
-        database: str | None = None,
-        let: Mapping[str, Any] | None = None,
-        on: str | Sequence[str] | None = None,
-        matched: Literal["replace", "keepExisting", "merge", "fail"]
-        | Self
-        | Sequence[Mapping[str, Any]] = "merge",
-        not_matched: Literal["insert", "discard", "fail"] = "insert",
-    ) -> None:
-        """
-        将聚合管道的结果写入指定的集合。`$merge` 操作符必须是管道中的最后一个阶段。
-
-        collection: 输出到指定集合。如果输出集合不存在，将会创建集合。
-        database: 输出到指定数据库，不指定则默认输出到运行聚合管道的同一数据库。
-        let: 指定在 `matched` 管道中使用的变量。
-        on: 作为文档唯一标识符的一个或多个字段。该标识符用于确定结果文档是否与输出集合中的现有文档匹配。
-        matched: 如果结果文档和输出集合中的现有文档对于字段上指定的值相同，则 `$merge` 的行为。
-        not_matched: 如果结果文档与输出集合中的现有文档不匹配，则 `$merge` 的行为。
-
-        [$merge (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/merge/)
-        """
-        struct = {
-            "into": {"db": database, "coll": collection} if database else collection,
-            "whenMatched": matched,
-            "whenNotMatched": not_matched,
-        }
-        if let:
-            struct["let"] = let
-        if on:
-            struct["on"] = on
-        self.stage("merge", struct)
-
-    def out(self, collection: str, database: str | None = None) -> Self:
-        """
-        获取聚合管道返回的文档并将它们写入指定的集合。
-
-        database: 输出数据库名称。
-        collection: 输出集合名称。
-
-        [$out (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/out/)
-        """
-        return self.stage(
-            "out", {"db": database, "coll": collection} if database else collection
-        )
-
-    def project(self, **fields: bool | Mapping[str, Any]) -> Self:
-        """
-        将带有指定字段的文档传递到管道中的下一阶段。指定的字段可以是输入文档中的现有字段或新计算的字段。
-
-        fields: 参数名为指定传递的字段。参数如果为布尔值，则可以包含或排除字段；如果为表达式，则可以添加新字段或重置现有字段的值。
-
-        [$project (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/project/)
-        """
-        return self.stage("project", fields)
-
-    def redact(self, expression: Any) -> Self:
-        """
-        根据存储在文档本身中的信息限制文档的内容。
-
-        expression: 可以是任何有效的表达式，只要它解析为 `$$DESCEND`、`$$PRUNE` 或 `$$KEEP` 系统变量。
-
-        [$redact (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/redact/)
-        """
-        return self.stage("redact", expression)
-
-    def replace(self, replacement: Any) -> Self:
-        """
-        用指定的文档替换输入文档。该操作将替换输入文档中的所有现有字段，包括 `_id` 字段。
-
-        replacement: 可以是解析为文档的任何有效表达式。
-
-        [$replaceWith (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/replaceWith/)
-        """
-        return self.stage("replaceWith", replacement)
-
-    def sample(self, size: int) -> Self:
-        """
-        从输入文档中随机选择指定数量的文档。
-
-        size: 随机选择的文档数量。
-
-        [$sample (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/sample/)
-        """
-        return self.stage("sample", {"size": size})
-
-    def set(self, **fields: Any) -> Self:
-        """
-        向文档中添加新字段。输出包含来自输入文档的所有现有字段和新添加的字段的文档。
-
-        field: 参数名为需要添加的每个字段的名称，参数为聚合表达式。如果新字段的名称与现有字段名称(包括 `_id`)相同，`$set` 将使用指定表达式的值覆盖该字段的现有值。
-
-        [$set (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/set/)
-        """
-        return self.stage("set", fields)
-
-    def skip(self, integer: int) -> Self:
-        """
-        跳过传递到该阶段的指定数量的文档，并将其余文档传递到管道中的下一个阶段。
-
-        integer: 指定要跳过的文档的最大数量。
-
-        [$skip (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/skip/)
-        """
-        return self.stage("skip", integer)
-
-    def sort(self, **fields: SortOrder) -> Self:
-        """
-        对所有输入文档进行排序，并按排序顺序将它们返回给管道。
-
-        field: 参数名为指定要排序的字段，参数为字段的排序顺序。最多可以按32个字段进行排序。
-
-        [$sort (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/sort/)
-        """
-        return self.stage("sort", fields)
-
-    def union(
-        self,
-        collection: str,
-        pipeline: Self | Sequence[Mapping[str, Any]] | None = None,
-    ) -> Self:
-        """
-        执行两个集合的联合。
-        将来自两个集合的管道结果合并为一个结果集，将组合的结果集(包括重复的)输出到下一阶段
-
-        collection: 希望在结果集中包含其管道结果的集合。
-        pipeline: 应用于指定的集合的聚合管道。
-
-        [$unionWith (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/unionWith/)
-        """
-        return self.stage(
-            "unionWith",
-            {"coll": collection, "pipeline": pipeline} if pipeline else collection,
-        )
-
-    def unset(self, *fields: str) -> Self:
-        """
-        从文档中移除/排除字段。
-
-        field: 指定要删除的字段。
-
-        [$unset (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/unset/)
-        """
-        return self.stage("unset", fields)
-
-    def unwind(
-        self, path: str, index_field: str | None = None, preserve_empty: bool = False
-    ) -> Self:
-        """
-        从输入文档中解构数组字段以输出每个元素的文档。每个输出文档都是输入文档，数组字段的值由元素替换。
-
-        path: 数组字段的字段路径。若要指定字段路径，请在字段名开头加上符号 `$`。
-        index_field: 保存元素数组索引的新字段的名称。名称不能以符号 `$` 开头。
-        preserve_empty: 在文档中的指定字段路径为 null、不存在或为空数组的情况下，如果该值为 `True`，则 `$unwind` 将输出文档，否则不会输出文档。
-
-        [$unwind (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/unwind/#mongodb-pipeline-pipe.-unwind)
-        """
-        struct = {
-            "path": path,
-            "preserveNullAndEmptyArrays": preserve_empty,
-        }
-        if index_field:
-            struct["includeArrayIndex"] = index_field
-        return self.stage("unwind", struct)
+from collections.abc import Mapping, Sequence
+from typing import Any, Literal, TypeAlias
+
+from typing_extensions import Self
+
+from mango.index import Order
+
+SortOrder: TypeAlias = Order | Literal[1, -1]
+
+
+class Pipeline(list[Mapping[str, Any]]):
+    """聚合管道阶段"""
+
+    def __init__(self, *stages: Mapping[str, Any]) -> None:
+        super().__init__(stages)
+
+    def stage(self, key: str, value: Any) -> Self:
+        """添加一个阶段"""
+        key = key if key.startswith("$") else f"${key}"
+        self.append({key: value})
+        return self
+
+    def bucket(
+        self,
+        group_by: Any,
+        boundaries: Sequence[int | float],
+        default: str | None = None,
+        output: Mapping[str, Mapping[str, Any]] | None = None,
+    ) -> Self:
+        """
+        根据指定的表达式和存储桶边界将传入文档分类到称为存储桶的组中，并为每个存储桶输出一个文档。
+
+        group_by: 对文档进行分组的表达式。若要指定字段路径，请在字段名前面加上符号 `$` 。
+        boundaries: 基于 `group_by` 表达式的值数组，用于指定每个桶的边界。每对相邻的值作为桶的包含下边界和独占上边界。
+        default: 指定一个附加桶的 `_id`，该桶包含 `group_by` 表达式结果中，不属于边界指定的桶的所有文档。
+        output: 指定输出文档中除 `_id` 字段外还要包含的字段。如果未指定文档，则操作返回包含文档数的字段在每个存储桶中。
+
+        [$bucket (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/bucket/)
+        """
+        if len(boundaries) < 2:  # noqa: PLR2004
+            raise ValueError("必须至少指定两个边界值")
+        if sorted(boundaries) != boundaries:
+            raise ValueError("指定的值必须以升序排列")
+        struct = {
+            "groupBy": group_by,
+            "boundaries": boundaries,
+        }
+        if default:
+            struct["default"] = default
+        if output:
+            struct["output"] = output
+        return self.stage("bucket", struct)
+
+    def count(self, field: str) -> Self:
+        """
+        将文档传递到下一阶段，该阶段包含输入到该阶段的文档数量的计数。
+
+        field : 输出字段的名称，其值为计数结果。必须是非空字符串，不能以 `$` 开头，也不能包含 `.` 字符。
+
+        [$count (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/count/)
+        """
+        if not field or field.startswith("$") or "." in field:
+            raise ValueError("必须是非空字符串, 不能以 `$` 开头，也不能包含 `.` 字符。")
+        return self.stage("count", field)
+
+    def documents(self, expression: Any) -> Self:
+        """
+        从输入值返回原始文档。
+
+        expression: 接受任何解析为映射数组的有效表达式。
+
+        [$documents (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/documents/)
+        """
+        return self.stage("documents", expression)
+
+    def facet(self, **fields: Self | Sequence[Mapping[str, Any]]) -> Self:
+        """
+        在同一组输入文档的单个阶段内处理多个聚合管道。每个子管道在输出文档中都有自己的字段，其结果存储为一个文档数组。
+        输入文档只被传递到 `$facet` 阶段一次。`$facet` 支持对同一组输入文档进行各种聚合，无需多次检索输入文档。
+
+        fields: 参数名为子管道输出的字段名, 参数为需要运行的子管道。
+
+        [$facet (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/facet/)
+        """
+        return self.stage("facet", fields)
+
+    def fill(
+        self,
+        output: Mapping[str, Any],
+        partition_by: Any = None,
+        partition_by_fields: Sequence[str] | None = None,
+        sort_by: Mapping[str, SortOrder] | None = None,
+    ) -> Self:
+        """
+        填充文档中的空值和缺少的字段值。
+
+        output: 指定一个字典，该字典包含要填充缺失值的每个字段输出对象的字典。对象名称是要填充的字段的名称，对象值指定如何填充该字段。
+        partition_by: 指定用于对文档进行分组的表达式。`partition_by` 和 `partition_by_fields` 是互斥的。
+        partition_by_fields: 指定字段数组，以作为文档分组的复合键。`partition_by` 和 `partition_by_fields` 是互斥的。
+        sort_by: 指定用于对每个分区内的文档进行排序的字段。
+
+        [$fill (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/fill/)
+        """
+        struct: dict[str, Any] = {
+            "output": output,
+        }
+        if partition_by:
+            struct["partitionBy"] = partition_by
+        elif partition_by_fields:
+            if isinstance(partition_by_fields, str):
+                raise TypeError("partition_by_fields 不能为字符串")
+            struct["partitionByFields"] = partition_by_fields
+        if sort_by:
+            struct["sortBy"] = sort_by
+        return self.stage("fill", struct)
+
+    def group(self, id: Any, **fields: Mapping[str, Any]) -> Self:
+        """
+        `$group` 阶段根据“组键”将文档分成多个组。
+        组键通常是一个字段或一组字段。组键也可以是表达式的结果。
+        在 `$group` 阶段的输出中，`_id` 字段被设置为该文档的组键。
+        每个输出文档的字段都包含唯一的按值分组。输出文档还可以包含包含某些累加器表达式值的计算字段。
+
+        id: 可以接受任何有效的表达式。如果指定 `id` 为 `None` 或任何其他常数值，那么此 `$group` 阶段将整体计算所有输入文档的累积值。
+        fields: 参数名为额外添加的字段, 参数为累加器表达式。
+
+        [$group (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/group/)
+        """
+        return self.stage("group", {"_id": id, **fields})
+
+    def limit(self, integer: int) -> Self:
+        """
+        限制传递到管道中下一阶段的文档数。
+
+        integer: 指定要传递的文档的最大数量。
+
+        [$limit (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/limit/)
+        """
+        return self.stage("limit", integer)
+
+    def lookup(
+        self,
+        from_: str | None = None,
+        local_field: str | None = None,
+        foreign_field: str | None = None,
+        let: Mapping[str, Any] | None = None,
+        pipeline: Self | Sequence[Mapping[str, Any]] | None = None,
+        as_: str | None = None,
+    ) -> Self:
+        """
+        对同一数据库中的集合执行左外联接，以从“联接”集合中筛选文档进行处理。
+        此 `$lookup` 阶段为每个输入文档添加一个新的数组字段，新的数组字段包含“联接”集合中的匹配文档，并将这些重新成形的文档传递到下一阶段。
+
+        from_: 指定同一数据库中要联接到当前集合的外部集合。
+        local_field: 指定当前集合的文档中的字段。
+        foreign_field: 指定外部集合的文档中的字段。
+        let: 指定要在管道阶段中使用的变量。使用变量表达式访问输入到管道的文档字段。
+        pipeline: 指定要在已联接集合上运行的管道。管道从已联接的集合中确定结果文档。若要返回所有文档，请指定空管道。
+        as_: 指定要添加到输出文档的新数组字段的名称。新的数组字段包含来自 `from_` 集合的匹配文档。如果指定的名称已经存在于输出文档中，则覆盖现有字段。
+
+        [$lookup (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/lookup/)
+        """
+        return self.stage(
+            "lookup",
+            {
+                k: v
+                for k, v in {
+                    "from": from_,
+                    "localField": local_field,
+                    "foreignField": foreign_field,
+                    "let": let,
+                    "pipeline": pipeline,
+                    "as": as_,
+                }.items()
+                if v is None
+            },
+        )
+
+    def match(self, query: Mapping[str, Any]) -> Self:
+        """
+        筛选文档流，仅将匹配指定条件的文档传递到下一个管道阶段。
+
+        query: 指定查询条件。
+
+        [$match (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/match/)
+        """
+        return self.stage("match", query)
+
+    def merge(
+        self,
+        collection: str,
+        database: str | None = None,
+        let: Mapping[str, Any] | None = None,
+        on: str | Sequence[str] | None = None,
+        matched: Literal["replace", "keepExisting", "merge", "fail"]
+        | Self
+        | Sequence[Mapping[str, Any]] = "merge",
+        not_matched: Literal["insert", "discard", "fail"] = "insert",
+    ) -> None:
+        """
+        将聚合管道的结果写入指定的集合。`$merge` 操作符必须是管道中的最后一个阶段。
+
+        collection: 输出到指定集合。如果输出集合不存在，将会创建集合。
+        database: 输出到指定数据库，不指定则默认输出到运行聚合管道的同一数据库。
+        let: 指定在 `matched` 管道中使用的变量。
+        on: 作为文档唯一标识符的一个或多个字段。该标识符用于确定结果文档是否与输出集合中的现有文档匹配。
+        matched: 如果结果文档和输出集合中的现有文档对于字段上指定的值相同，则 `$merge` 的行为。
+        not_matched: 如果结果文档与输出集合中的现有文档不匹配，则 `$merge` 的行为。
+
+        [$merge (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/merge/)
+        """
+        struct = {
+            "into": {"db": database, "coll": collection} if database else collection,
+            "whenMatched": matched,
+            "whenNotMatched": not_matched,
+        }
+        if let:
+            struct["let"] = let
+        if on:
+            struct["on"] = on
+        self.stage("merge", struct)
+
+    def out(self, collection: str, database: str | None = None) -> Self:
+        """
+        获取聚合管道返回的文档并将它们写入指定的集合。
+
+        database: 输出数据库名称。
+        collection: 输出集合名称。
+
+        [$out (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/out/)
+        """
+        return self.stage(
+            "out", {"db": database, "coll": collection} if database else collection
+        )
+
+    def project(self, **fields: bool | Mapping[str, Any]) -> Self:
+        """
+        将带有指定字段的文档传递到管道中的下一阶段。指定的字段可以是输入文档中的现有字段或新计算的字段。
+
+        fields: 参数名为指定传递的字段。参数如果为布尔值，则可以包含或排除字段；如果为表达式，则可以添加新字段或重置现有字段的值。
+
+        [$project (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/project/)
+        """
+        return self.stage("project", fields)
+
+    def redact(self, expression: Any) -> Self:
+        """
+        根据存储在文档本身中的信息限制文档的内容。
+
+        expression: 可以是任何有效的表达式，只要它解析为 `$$DESCEND`、`$$PRUNE` 或 `$$KEEP` 系统变量。
+
+        [$redact (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/redact/)
+        """
+        return self.stage("redact", expression)
+
+    def replace(self, replacement: Any) -> Self:
+        """
+        用指定的文档替换输入文档。该操作将替换输入文档中的所有现有字段，包括 `_id` 字段。
+
+        replacement: 可以是解析为文档的任何有效表达式。
+
+        [$replaceWith (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/replaceWith/)
+        """
+        return self.stage("replaceWith", replacement)
+
+    def sample(self, size: int) -> Self:
+        """
+        从输入文档中随机选择指定数量的文档。
+
+        size: 随机选择的文档数量。
+
+        [$sample (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/sample/)
+        """
+        return self.stage("sample", {"size": size})
+
+    def set(self, **fields: Any) -> Self:
+        """
+        向文档中添加新字段。输出包含来自输入文档的所有现有字段和新添加的字段的文档。
+
+        field: 参数名为需要添加的每个字段的名称，参数为聚合表达式。如果新字段的名称与现有字段名称(包括 `_id`)相同，`$set` 将使用指定表达式的值覆盖该字段的现有值。
+
+        [$set (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/set/)
+        """
+        return self.stage("set", fields)
+
+    def skip(self, integer: int) -> Self:
+        """
+        跳过传递到该阶段的指定数量的文档，并将其余文档传递到管道中的下一个阶段。
+
+        integer: 指定要跳过的文档的最大数量。
+
+        [$skip (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/skip/)
+        """
+        return self.stage("skip", integer)
+
+    def sort(self, **fields: SortOrder) -> Self:
+        """
+        对所有输入文档进行排序，并按排序顺序将它们返回给管道。
+
+        field: 参数名为指定要排序的字段，参数为字段的排序顺序。最多可以按32个字段进行排序。
+
+        [$sort (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/sort/)
+        """
+        return self.stage("sort", fields)
+
+    def union(
+        self,
+        collection: str,
+        pipeline: Self | Sequence[Mapping[str, Any]] | None = None,
+    ) -> Self:
+        """
+        执行两个集合的联合。
+        将来自两个集合的管道结果合并为一个结果集，将组合的结果集(包括重复的)输出到下一阶段
+
+        collection: 希望在结果集中包含其管道结果的集合。
+        pipeline: 应用于指定的集合的聚合管道。
+
+        [$unionWith (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/unionWith/)
+        """
+        return self.stage(
+            "unionWith",
+            {"coll": collection, "pipeline": pipeline} if pipeline else collection,
+        )
+
+    def unset(self, *fields: str) -> Self:
+        """
+        从文档中移除/排除字段。
+
+        field: 指定要删除的字段。
+
+        [$unset (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/unset/)
+        """
+        return self.stage("unset", fields)
+
+    def unwind(
+        self, path: str, index_field: str | None = None, preserve_empty: bool = False
+    ) -> Self:
+        """
+        从输入文档中解构数组字段以输出每个元素的文档。每个输出文档都是输入文档，数组字段的值由元素替换。
+
+        path: 数组字段的字段路径。若要指定字段路径，请在字段名开头加上符号 `$`。
+        index_field: 保存元素数组索引的新字段的名称。名称不能以符号 `$` 开头。
+        preserve_empty: 在文档中的指定字段路径为 null、不存在或为空数组的情况下，如果该值为 `True`，则 `$unwind` 将输出文档，否则不会输出文档。
+
+        [$unwind (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/unwind/#mongodb-pipeline-pipe.-unwind)
+        """
+        struct = {
+            "path": path,
+            "preserveNullAndEmptyArrays": preserve_empty,
+        }
+        if index_field:
+            struct["includeArrayIndex"] = index_field
+        return self.stage("unwind", struct)
```

### Comparing `mango_odm-0.3.0/mango/utils.py` & `mango_odm-0.3.1/mango/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,141 +1,139 @@
-import re
-from collections.abc import Callable, Generator, Iterable, Sequence
-from types import UnionType
-from typing import TYPE_CHECKING, Any
-
-import pydantic
-from pydantic.fields import ModelField
-
-from mango.fields import FieldInfo
-from mango.index import Index, IndexType
-
-if TYPE_CHECKING:  # pragma: no cover
-    from mango.models import Document
-
-
-def to_snake_case(string: str) -> str:
-    """将字符串转换为蛇形命名法"""
-    tmp = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", string)
-    return re.sub("([a-z0-9])([A-Z])", r"\1_\2", tmp).lower()
-
-
-def all_check(
-    iter_obj: Iterable[object],
-    type_or_func: type
-    | UnionType
-    | Callable
-    | tuple[type | UnionType | tuple[Any, ...], ...],
-) -> bool:
-    """
-    如果可迭代对象中的所有元素为指定类型，则返回True。
-    如果可迭代对象为空，则返回True。
-    """
-    if isinstance(type_or_func, Callable):
-        return all(type_or_func(obj) for obj in iter_obj)
-    else:
-        return all(isinstance(obj, type_or_func) for obj in iter_obj)
-
-
-def any_check(
-    iter_obj: Iterable[object],
-    type_or_func: type
-    | UnionType
-    | Callable
-    | tuple[type | UnionType | tuple[Any, ...], ...],
-) -> bool:
-    """
-    如果可迭代对象中的任意元素为指定类型，则返回True。
-    如果可迭代对象为空，则返回False。
-    """
-    if isinstance(type_or_func, Callable):
-        return any(type_or_func(obj) for obj in iter_obj)
-    else:
-        return any(isinstance(obj, type_or_func) for obj in iter_obj)
-
-
-def is_sequence(
-    iter_obj: Sequence[object],
-) -> bool:
-    """判断是否为非字符串的序列对象"""
-    return isinstance(iter_obj, Sequence) and not isinstance(iter_obj, bytes | str)
-
-
-def validate_fields(
-    model: type["Document"], input_data: dict[str, Any]
-) -> dict[str, Any]:
-    """验证模型的指定字段"""
-    if miss := set(input_data) - set(model.__fields__):
-        raise ValueError(f"这些字段在 {model.__name__} 中不存在: {miss}")
-
-    fields = {
-        k: (v.type_, v.field_info)
-        for k, v in model.__fields__.items()
-        if k in input_data
-    }
-    new_model = pydantic.create_model(model.__name__, **fields)
-    values, _, validation_error = pydantic.validate_model(new_model, input_data)
-
-    if validation_error:
-        raise validation_error
-
-    return values
-
-
-def add_fields(model: type["Document"], **field_definitions: Any):
-    """动态添加字段
-
-    来源见: https://github.com/pydantic/pydantic/issues/1937
-    """
-    new_fields: dict[str, ModelField] = {}
-    new_annotations: dict[str, type | None] = {}
-
-    for f_name, f_def in field_definitions.items():
-        if isinstance(f_def, tuple):
-            try:
-                f_annotation, f_value = f_def
-            except ValueError as e:
-                raise ValueError(
-                    "field definitions should either be a tuple of (<type>, <default>) "
-                    "or just a default value, unfortunately this means tuples as "
-                    "default values are not allowed"
-                ) from e
-        else:
-            f_annotation, f_value = None, f_def
-
-        if f_annotation:
-            new_annotations[f_name] = f_annotation
-
-        new_fields[f_name] = ModelField.infer(
-            name=f_name,
-            value=f_value,
-            annotation=f_annotation,
-            class_validators=None,
-            config=model.__config__,
-        )
-
-    model.__fields__.update(new_fields)
-    model.__annotations__.update(new_annotations)
-
-
-def get_indexes(model: type["Document"]) -> Generator[Index, None, None]:
-    """获取模型中定义的索引, 包括字段与元配置"""
-    for name, field in model.__fields__.items():
-        finfo = field.field_info
-        if isinstance(finfo, FieldInfo):
-            if index := finfo.index:
-                if index is True:
-                    yield Index(name)
-                elif isinstance(index, IndexType):
-                    yield Index((name, index))
-                else:
-                    yield index
-            elif expire := finfo.expire:
-                yield Index(name, expireAfterSeconds=expire)
-
-    for index in model.__meta__.indexes:
-        if isinstance(index, str):
-            yield Index(index)
-        elif isinstance(index, Sequence):
-            yield Index(*index)
-        else:
-            yield index
+import re
+from collections.abc import Callable, Generator, Iterable, Sequence
+from types import UnionType
+from typing import TYPE_CHECKING, Any
+
+import pydantic
+from pydantic.fields import ModelField
+
+from mango.fields import FieldInfo
+from mango.index import Index, IndexType
+
+if TYPE_CHECKING:  # pragma: no cover
+    from mango.models import Document
+
+
+def to_snake_case(string: str) -> str:
+    """将字符串转换为蛇形命名法"""
+    tmp = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", string)
+    return re.sub("([a-z0-9])([A-Z])", r"\1_\2", tmp).lower()
+
+
+def all_check(
+    iter_obj: Iterable[object],
+    type_or_func: type
+    | UnionType
+    | Callable
+    | tuple[type | UnionType | tuple[Any, ...], ...],
+) -> bool:
+    """
+    如果可迭代对象中的所有元素为指定类型，则返回True。
+    如果可迭代对象为空，则返回True。
+    """
+    if isinstance(type_or_func, Callable):
+        return all(type_or_func(obj) for obj in iter_obj)
+    return all(isinstance(obj, type_or_func) for obj in iter_obj)
+
+
+def any_check(
+    iter_obj: Iterable[object],
+    type_or_func: type
+    | UnionType
+    | Callable
+    | tuple[type | UnionType | tuple[Any, ...], ...],
+) -> bool:
+    """
+    如果可迭代对象中的任意元素为指定类型，则返回True。
+    如果可迭代对象为空，则返回False。
+    """
+    if isinstance(type_or_func, Callable):
+        return any(type_or_func(obj) for obj in iter_obj)
+    return any(isinstance(obj, type_or_func) for obj in iter_obj)
+
+
+def is_sequence(
+    iter_obj: Sequence[object],
+) -> bool:
+    """判断是否为非字符串的序列对象"""
+    return isinstance(iter_obj, Sequence) and not isinstance(iter_obj, bytes | str)
+
+
+def validate_fields(
+    model: type["Document"], input_data: dict[str, Any]
+) -> dict[str, Any]:
+    """验证模型的指定字段"""
+    if miss := set(input_data) - set(model.__fields__):
+        raise ValueError(f"这些字段在 {model.__name__} 中不存在: {miss}")
+
+    fields = {
+        k: (v.outer_type_, v.field_info)
+        for k, v in model.__fields__.items()
+        if k in input_data
+    }
+    new_model = pydantic.create_model(model.__name__, **fields)
+    values, _, validation_error = pydantic.validate_model(new_model, input_data)
+
+    if validation_error:
+        raise validation_error
+
+    return values
+
+
+def add_fields(model: type["Document"], **field_definitions: Any) -> None:
+    """动态添加字段
+
+    来源见: https://github.com/pydantic/pydantic/issues/1937
+    """
+    new_fields: dict[str, ModelField] = {}
+    new_annotations: dict[str, type | None] = {}
+
+    for f_name, f_def in field_definitions.items():
+        if isinstance(f_def, tuple):
+            try:
+                f_annotation, f_value = f_def
+            except ValueError as e:
+                raise ValueError(
+                    "field definitions should either be a tuple of (<type>, <default>) "
+                    "or just a default value, unfortunately this means tuples as "
+                    "default values are not allowed"
+                ) from e
+        else:
+            f_annotation, f_value = None, f_def
+
+        if f_annotation:
+            new_annotations[f_name] = f_annotation
+
+        new_fields[f_name] = ModelField.infer(
+            name=f_name,
+            value=f_value,
+            annotation=f_annotation,
+            class_validators=None,
+            config=model.__config__,
+        )
+
+    model.__fields__.update(new_fields)
+    model.__annotations__.update(new_annotations)
+
+
+def get_indexes(model: type["Document"]) -> Generator[Index, None, None]:
+    """获取模型中定义的索引, 包括字段与元配置"""
+    for name, field in model.__fields__.items():
+        finfo = field.field_info
+        if isinstance(finfo, FieldInfo):
+            if index := finfo.index:
+                if index is True:
+                    yield Index(name)
+                elif isinstance(index, IndexType):
+                    yield Index((name, index))
+                else:
+                    yield index
+            elif expire := finfo.expire:
+                yield Index(name, expireAfterSeconds=expire)
+
+    for index in model.__meta__.indexes:
+        if isinstance(index, str):
+            yield Index(index)
+        elif isinstance(index, Sequence):
+            yield Index(*index)
+        else:
+            yield index
```

### Comparing `mango_odm-0.3.0/setup.py` & `mango_odm-0.3.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,399 +1,378 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 276d 616e 676f 275d 0a0a 7061   \.['mango']..pa
-00000050: 636b 6167 655f 6461 7461 203d 205c 0a7b  ckage_data = \.{
-00000060: 2727 3a20 5b27 2a27 5d7d 0a0a 6d6f 6475  '': ['*']}..modu
-00000070: 6c65 7320 3d20 5c0a 5b27 7079 275d 0a69  les = \.['py'].i
-00000080: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-00000090: 3d20 5c0a 5b27 6d6f 746f 723e 3d33 2e30  = \.['motor>=3.0
-000000a0: 2e30 2c3c 342e 302e 3027 2c20 2770 7964  .0,<4.0.0', 'pyd
-000000b0: 616e 7469 633e 3d31 2e31 302e 302c 3c32  antic>=1.10.0,<2
-000000c0: 2e30 2e30 275d 0a0a 7365 7475 705f 6b77  .0.0']..setup_kw
-000000d0: 6172 6773 203d 207b 0a20 2020 2027 6e61  args = {.    'na
-000000e0: 6d65 273a 2027 6d61 6e67 6f2d 6f64 6d27  me': 'mango-odm'
-000000f0: 2c0a 2020 2020 2776 6572 7369 6f6e 273a  ,.    'version':
-00000100: 2027 302e 332e 3027 2c0a 2020 2020 2764   '0.3.0',.    'd
-00000110: 6573 6372 6970 7469 6f6e 273a 2027 f09f  escription': '..
-00000120: a5ad 2041 7379 6e63 204d 6f6e 676f 4442  .. Async MongoDB
-00000130: 204f 444d 2077 6974 6820 7479 7065 2068   ODM with type h
-00000140: 696e 7473 2069 6e20 5079 7468 6f6e 272c  ints in Python',
-00000150: 0a20 2020 2027 6c6f 6e67 5f64 6573 6372  .    'long_descr
-00000160: 6970 7469 6f6e 273a 2027 3c70 2061 6c69  iption': '<p ali
-00000170: 676e 3d22 6365 6e74 6572 223e 5c6e 2020  gn="center">\n  
-00000180: 2020 3c61 206e 616d 653d 2272 6561 646d    <a name="readm
-00000190: 652d 746f 7022 3e3c 2f61 3e5c 6e20 2020  e-top"></a>\n   
-000001a0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-000001b0: 2f2f 6769 7468 7562 2e63 6f6d 2f41 2d6b  //github.com/A-k
-000001c0: 6972 616d 692f 6d61 6e67 6f22 3e5c 6e20  irami/mango">\n 
-000001d0: 2020 2020 2020 203c 696d 6720 7769 6474         <img widt
-000001e0: 683d 2231 3430 7078 2220 7372 633d 2268  h="140px" src="h
-000001f0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00000200: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000210: 2f41 2d6b 6972 616d 692f 6d61 6e67 6f2f  /A-kirami/mango/
-00000220: 6d61 696e 2f61 7373 6574 732f 6d61 6e67  main/assets/mang
-00000230: 6f2d 6c6f 676f 2e73 7667 2220 616c 6967  o-logo.svg" alig
-00000240: 6e3d 2263 656e 7465 7222 2061 6c74 3d22  n="center" alt="
-00000250: 4d61 6e67 6f22 202f 3e5c 6e20 2020 203c  Mango" />\n    <
-00000260: 2f61 3e5c 6e20 2020 203c 6831 2061 6c69  /a>\n    <h1 ali
-00000270: 676e 3d22 6365 6e74 6572 223e 4d61 6e67  gn="center">Mang
-00000280: 6f3c 2f68 313e 5c6e 2020 2020 3c70 2061  o</h1>\n    <p a
-00000290: 6c69 676e 3d22 6365 6e74 6572 223e f09f  lign="center">..
-000002a0: a5ad 20e5 b8a6 e69c 89e7 b1bb e59e 8be6  .. .............
-000002b0: 8f90 e7a4 bae7 9a84 2050 7974 686f 6e20  ........ Python 
-000002c0: e5bc 82e6 ada5 204d 6f6e 676f 4442 20e5  ...... MongoDB .
-000002d0: afb9 e8b1 a1e6 9687 e6a1 a3e6 98a0 e5b0  ................
-000002e0: 84e5 99a8 3c2f 703e 5c6e 3c2f 703e 5c6e  ....</p>\n</p>\n
-000002f0: 2020 2020 3c70 2061 6c69 676e 3d22 6365      <p align="ce
-00000300: 6e74 6572 223e 5c6e 2020 2020 2020 2020  nter">\n        
-00000310: 3c61 2068 7265 663d 222e 2f4c 4943 454e  <a href="./LICEN
-00000320: 5345 223e 5c6e 2020 2020 2020 2020 2020  SE">\n          
-00000330: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000340: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000350: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
-00000360: 652f 412d 6b69 7261 6d69 2f6d 616e 676f  e/A-kirami/mango
-00000370: 2e73 7667 2220 616c 743d 226c 6963 656e  .svg" alt="licen
-00000380: 7365 223e 5c6e 2020 2020 2020 2020 3c2f  se">\n        </
-00000390: 613e 5c6e 2020 2020 2020 2020 3c61 2068  a>\n        <a h
-000003a0: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
-000003b0: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
-000003c0: 692f 6d61 6e67 6f2d 6f64 6d22 3e5c 6e20  i/mango-odm">\n 
-000003d0: 2020 2020 2020 2020 2020 203c 696d 6720             <img 
-000003e0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000003f0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000400: 2f76 2f6d 616e 676f 2d6f 646d 2e73 7667  /v/mango-odm.svg
-00000410: 2220 616c 743d 2270 7970 6922 3e5c 6e20  " alt="pypi">\n 
-00000420: 2020 2020 2020 203c 2f61 3e5c 6e20 2020         </a>\n   
-00000430: 2020 2020 203c 6120 6872 6566 3d22 6874       <a href="ht
-00000440: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
-00000450: 2e6f 7267 2f22 3e5c 6e20 2020 2020 2020  .org/">\n       
-00000460: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
-00000470: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000480: 6473 2e69 6f2f 6261 6467 652f 7079 7468  ds.io/badge/pyth
-00000490: 6f6e 2d33 2e31 302b 2d62 6c75 652e 7376  on-3.10+-blue.sv
-000004a0: 6722 2061 6c74 3d22 7079 7468 6f6e 223e  g" alt="python">
-000004b0: 5c6e 2020 2020 2020 2020 3c2f 613e 5c6e  \n        </a>\n
-000004c0: 2020 2020 3c2f 703e 5c6e 2020 2020 3c70      </p>\n    <p
-000004d0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-000004e0: 5c6e 2020 2020 2020 2020 3c61 2068 7265  \n        <a hre
-000004f0: 663d 2223 2de7 a4ba e4be 8b22 3ee6 9fa5  f="#-......">...
-00000500: e79c 8be6 bc94 e7a4 ba3c 2f61 3e5c 6e20  .........</a>\n 
-00000510: 2020 2020 2020 20c2 b75c 6e20 2020 2020         ..\n     
-00000520: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
-00000530: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
-00000540: 2d6b 6972 616d 692f 6d61 6e67 6f2f 6973  -kirami/mango/is
-00000550: 7375 6573 2f6e 6577 3f61 7373 6967 6e65  sues/new?assigne
-00000560: 6573 3d26 6c61 6265 6c73 3d62 7567 2674  es=&labels=bug&t
-00000570: 656d 706c 6174 653d 6275 675f 7265 706f  emplate=bug_repo
-00000580: 7274 2e79 6d6c 2674 6974 6c65 3d25 3542  rt.yml&title=%5B
-00000590: 4255 4725 3544 2533 412b 223e e994 99e8  BUG%5D%3A+">....
-000005a0: afaf e68a a5e5 918a 3c2f 613e 5c6e 2020  ........</a>\n  
-000005b0: 2020 2020 2020 c2b7 5c6e 2020 2020 2020        ..\n      
-000005c0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-000005d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 412d  ://github.com/A-
-000005e0: 6b69 7261 6d69 2f6d 616e 676f 2f69 7373  kirami/mango/iss
-000005f0: 7565 732f 6e65 773f 6173 7369 676e 6565  ues/new?assignee
-00000600: 733d 266c 6162 656c 733d 656e 6861 6e63  s=&labels=enhanc
-00000610: 656d 656e 7426 7465 6d70 6c61 7465 3d66  ement&template=f
-00000620: 6561 7475 7265 5f72 6571 7565 7374 2e79  eature_request.y
-00000630: 6d6c 2674 6974 6c65 3d25 3542 4665 6174  ml&title=%5BFeat
-00000640: 7572 6525 3544 2533 412b 223e e58a 9fe8  ure%5D%3A+">....
-00000650: 83bd e8af b7e6 b182 3c2f 613e 5c6e 2020  ........</a>\n  
-00000660: 2020 3c2f 703e 5c6e 2020 2020 3c70 2061    </p>\n    <p a
-00000670: 6c69 676e 3d22 6365 6e74 6572 223e 5c6e  lign="center">\n
-00000680: 2020 2020 2020 2020 3c73 7472 6f6e 673e          <strong>
-00000690: e7ae 80e4 bd93 e4b8 ade6 9687 3c2f 7374  ............</st
-000006a0: 726f 6e67 3e5c 6e20 2020 2020 2020 20c2  rong>\n        .
-000006b0: b75c 6e20 2020 2020 2020 203c 6120 6872  .\n        <a hr
-000006c0: 6566 3d22 2f64 6f63 732f 5245 4144 4d45  ef="/docs/README
-000006d0: 5f45 4e2e 6d64 223e 456e 676c 6973 683c  _EN.md">English<
-000006e0: 2f61 3e5c 6e20 2020 2020 2020 20c2 b75c  /a>\n        ..\
-000006f0: 6e20 2020 2020 2020 203c 6120 6872 6566  n        <a href
-00000700: 3d22 2f64 6f63 732f 5245 4144 4d45 5f4a  ="/docs/README_J
-00000710: 412e 6d64 223e e697 a5e6 9cac e8aa 9e3c  A.md">.........<
-00000720: 2f61 3e5c 6e20 2020 203c 2f70 3e5c 6e3c  /a>\n    </p>\n<
-00000730: 2f70 3e5c 6e3c 7020 616c 6967 6e3d 2263  /p>\n<p align="c
-00000740: 656e 7465 7222 3e5c 6e5c 6e23 2320 f09f  enter">\n\n## ..
-00000750: 9496 20e7 9bae e5bd 955c 6e5c 6e3c 6465  .. ......\n\n<de
-00000760: 7461 696c 7320 6f70 656e 3d22 6f70 656e  tails open="open
-00000770: 223e 5c6e 2020 3c73 756d 6d61 7279 3ee7  ">\n  <summary>.
-00000780: 9bae e5bd 953c 2f73 756d 6d61 7279 3e5c  .....</summary>\
-00000790: 6e20 203c 756c 3e5c 6e20 2020 203c 6c69  n  <ul>\n    <li
-000007a0: 3e5c 6e20 2020 2020 2020 203c 6120 6872  >\n        <a hr
-000007b0: 6566 3d22 232d e7ae 80e4 bb8b 223e e7ae  ef="#-......">..
-000007c0: 80e4 bb8b 3c2f 613e 5c6e 2020 2020 2020  ....</a>\n      
-000007d0: 2020 3c75 6c3e 5c6e 2020 2020 2020 2020    <ul>\n        
-000007e0: 2020 2020 3c6c 693e 3c61 2068 7265 663d      <li><a href=
-000007f0: 2223 2de6 a0b8 e5bf 83e7 89b9 e680 a722  "#-............"
-00000800: 3ee6 a0b8 e5bf 83e7 89b9 e680 a73c 2f61  >............</a
-00000810: 3e3c 2f6c 693e 5c6e 2020 2020 2020 2020  ></li>\n        
-00000820: 3c2f 756c 3e5c 6e20 2020 203c 2f6c 693e  </ul>\n    </li>
-00000830: 5c6e 2020 2020 3c6c 693e 5c6e 2020 2020  \n    <li>\n    
-00000840: 2020 2020 3c61 2068 7265 663d 2223 2de5      <a href="#-.
-00000850: ae89 e8a3 8522 3ee5 ae89 e8a3 853c 2f61  .....">......</a
-00000860: 3e5c 6e20 2020 2020 2020 203c 756c 3e5c  >\n        <ul>\
-00000870: 6e20 2020 2020 2020 2020 2020 203c 6c69  n            <li
-00000880: 3e3c 6120 6872 6566 3d22 2350 4950 223e  ><a href="#PIP">
-00000890: 5049 503c 2f61 3e3c 2f6c 693e 5c6e 2020  PIP</a></li>\n  
-000008a0: 2020 2020 2020 2020 2020 3c6c 693e 3c61            <li><a
-000008b0: 2068 7265 663d 2223 506f 6574 7279 223e   href="#Poetry">
-000008c0: 506f 6574 7279 3c2f 613e 3c2f 6c69 3e5c  Poetry</a></li>\
-000008d0: 6e20 2020 2020 2020 203c 2f75 6c3e 5c6e  n        </ul>\n
-000008e0: 2020 2020 3c2f 6c69 3e5c 6e20 2020 203c      </li>\n    <
-000008f0: 6c69 3e5c 6e20 2020 2020 2020 203c 6120  li>\n        <a 
-00000900: 6872 6566 3d22 232d e7a4 bae4 be8b 223e  href="#-......">
-00000910: e7a4 bae4 be8b 3c2f 613e 5c6e 2020 2020  ......</a>\n    
-00000920: 2020 2020 3c75 6c3e 5c6e 2020 2020 2020      <ul>\n      
-00000930: 2020 2020 2020 3c6c 693e 3c61 2068 7265        <li><a hre
-00000940: 663d 2223 e588 9be5 bbba e682 a8e7 9a84  f="#............
-00000950: e7ac ace4 b880 e4b8 aae6 a8a1 e59e 8b22  ..............."
-00000960: 3ee5 889b e5bb bae6 82a8 e79a 84e7 acac  >...............
-00000970: e4b8 80e4 b8aa e6a8 a1e5 9e8b 3c2f 613e  ............</a>
-00000980: 3c2f 6c69 3e5c 6e20 2020 2020 2020 2020  </li>\n         
-00000990: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
-000009a0: 23e5 b086 e695 b0e6 8dae e4bf 9de5 ad98  #...............
-000009b0: e588 b0e6 95b0 e68d aee5 ba93 223e e5b0  ............">..
-000009c0: 86e6 95b0 e68d aee4 bf9d e5ad 98e5 88b0  ................
-000009d0: e695 b0e6 8dae e5ba 933c 2f61 3e3c 2f6c  .........</a></l
-000009e0: 693e 5c6e 2020 2020 2020 2020 2020 2020  i>\n            
-000009f0: 3c6c 693e 3c61 2068 7265 663d 2223 e69f  <li><a href="#..
-00000a00: a5e6 89be e7ac a6e5 9088 e69d a1e4 bbb6  ................
-00000a10: e79a 84e6 9687 e6a1 a322 3ee6 9fa5 e689  .........">.....
-00000a20: bee7 aca6 e590 88e6 9da1 e4bb b6e7 9a84  ................
-00000a30: e696 87e6 a1a3 3c2f 613e 3c2f 6c69 3e5c  ......</a></li>\
-00000a40: 6e20 2020 2020 2020 2020 2020 203c 6c69  n            <li
-00000a50: 3e3c 6120 6872 6566 3d22 23e4 bfae e694  ><a href="#.....
-00000a60: b9e6 95b0 e68d aee5 ba93 e4b8 ade7 9a84  ................
-00000a70: e696 87e6 a1a3 223e e4bf aee6 94b9 e695  ......">........
-00000a80: b0e6 8dae e5ba 93e4 b8ad e79a 84e6 9687  ................
-00000a90: e6a1 a33c 2f61 3e3c 2f6c 693e 5c6e 2020  ...</a></li>\n  
-00000aa0: 2020 2020 2020 2020 2020 3c6c 693e 3c61            <li><a
-00000ab0: 2068 7265 663d 2223 e5b5 8ce5 85a5 e5bc   href="#........
-00000ac0: 8fe6 a8a1 e59e 8b22 3ee5 b58c e585 a5e5  .......">.......
-00000ad0: bc8f e6a8 a1e5 9e8b 3c2f 613e 3c2f 6c69  ........</a></li
-00000ae0: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
-00000af0: 6c69 3e3c 6120 6872 6566 3d22 23e8 bf9e  li><a href="#...
-00000b00: e68e a5e6 95b0 e68d aee5 ba93 223e e8bf  ............">..
-00000b10: 9ee6 8ea5 e695 b0e6 8dae e5ba 933c 2f61  .............</a
-00000b20: 3e3c 2f6c 693e 5c6e 2020 2020 2020 2020  ></li>\n        
-00000b30: 3c2f 756c 3e5c 6e20 2020 203c 2f6c 693e  </ul>\n    </li>
-00000b40: 5c6e 2020 2020 3c6c 693e 5c6e 2020 2020  \n    <li>\n    
-00000b50: 2020 2020 3c61 2068 7265 663d 2223 2de8      <a href="#-.
-00000b60: b4a1 e78c ae22 3ee8 b4a1 e78c ae3c 2f61  .....">......</a
-00000b70: 3e5c 6e20 2020 2020 2020 203c 756c 3e5c  >\n        <ul>\
-00000b80: 6e20 2020 2020 2020 2020 2020 203c 6c69  n            <li
-00000b90: 3e3c 6120 6872 6566 3d22 232d e9b8 a3e8  ><a href="#-....
-00000ba0: b0a2 223e e9b8 a3e8 b0a2 3c2f 613e 3c2f  ..">......</a></
-00000bb0: 6c69 3e5c 6e20 2020 2020 2020 203c 2f75  li>\n        </u
-00000bc0: 6c3e 5c6e 2020 2020 3c2f 6c69 3e5c 6e20  l>\n    </li>\n 
-00000bd0: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
-00000be0: 232d e694 afe6 8c81 223e e694 afe6 8c81  #-......">......
-00000bf0: 3c2f 613e 3c2f 6c69 3e5c 6e20 2020 203c  </a></li>\n    <
-00000c00: 6c69 3e3c 6120 6872 6566 3d22 232d e8ae  li><a href="#-..
-00000c10: b8e5 8faf e8af 8122 3ee8 aeb8 e58f afe8  .......">.......
-00000c20: af81 3c2f 613e 3c2f 6c69 3e5c 6e20 203c  ..</a></li>\n  <
-00000c30: 2f75 6c3e 5c6e 3c2f 6465 7461 696c 733e  /ul>\n</details>
-00000c40: 5c6e 5c6e 2323 20f0 9f93 9620 e7ae 80e4  \n\n## .... ....
-00000c50: bb8b 5c6e 5c6e 4d61 6e67 6f20 e698 afe4  ..\n\nMango ....
-00000c60: b880 e4b8 aae5 b8a6 e69c 89e7 b1bb e59e  ................
-00000c70: 8be6 8f90 e7a4 bae7 9a84 2050 7974 686f  .......... Pytho
-00000c80: 6e20 e5bc 82e6 ada5 204d 6f6e 676f 4442  n ...... MongoDB
-00000c90: 20e5 afb9 e8b1 a1e6 9687 e6a1 a3e6 98a0   ...............
-00000ca0: e5b0 84e5 99a8 284f 444d 29ef bc8c e5ae  ......(ODM).....
-00000cb0: 83e6 9e84 e5bb bae5 9ca8 205b 4d6f 746f  .......... [Moto
-00000cc0: 725d 2868 7474 7073 3a2f 2f6d 6f74 6f72  r](https://motor
-00000cd0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00000ce0: 656e 2f73 7461 626c 652f 2920 e592 8c20  en/stable/) ... 
-00000cf0: 5b50 7964 616e 7469 635d 2868 7474 7073  [Pydantic](https
-00000d00: 3a2f 2f70 7964 616e 7469 632d 646f 6373  ://pydantic-docs
-00000d10: 2e68 656c 706d 616e 7561 6c2e 696f 2f29  .helpmanual.io/)
-00000d20: 20e4 b98b e4b8 8ae3 8082 5c6e 5c6e 4d61   .........\n\nMa
-00000d30: 6e67 6f20 e4bd bfe5 be97 e695 b0e6 8dae  ngo ............
-00000d40: e5bb bae6 a8a1 e592 8ce6 9fa5 e8af a2e5  ................
-00000d50: 8f98 e5be 97e9 9d9e e5b8 b8e5 aeb9 e698  ................
-00000d60: 93ef bc8c e5b8 aee5 8aa9 e682 a8e5 85b3  ................
-00000d70: e6b3 a8e5 ba94 e794 a8e7 a88b e5ba 8fe4  ................
-00000d80: b8ad e79c 9fe6 ada3 e987 8de8 a681 e79a  ................
-00000d90: 84e9 83a8 e588 86e3 8082 5c6e 5c6e 2323  ..........\n\n##
-00000da0: 2320 e29c a820 e6a0 b8e5 bf83 e789 b9e6  # ... ..........
-00000db0: 80a7 efbc 9a5c 6e5c 6e2d 202a 2ae5 ae8c  .....\n\n- **...
-00000dc0: e596 84e7 9a84 e7b1 bbe5 9e8b e6a0 87e6  ................
-00000dd0: b3a8 2a2a efbc 9ae5 88a9 e794 a8e9 9d99  ..**............
-00000de0: e680 81e5 8886 e69e 90e6 9da5 e587 8fe5  ................
-00000df0: b091 e8bf 90e8 a18c e697 b6e9 97ae e9a2  ................
-00000e00: 985c 6e2d 202a 2ae7 ae80 e6b4 81e6 b581  .\n- **.........
-00000e10: e795 85e7 9a84 2041 5049 2a2a efbc 9ae6  ...... API**....
-00000e20: 9bb4 e698 93e4 ba8e e5ad a6e4 b9a0 e592  ................
-00000e30: 8ce4 bdbf e794 a8ef bc8c e68f 90e9 ab98  ................
-00000e40: e5bc 80e5 8f91 e695 88e7 8e87 5c6e 2d20  ............\n- 
-00000e50: 2a2a e4bc 98e9 9b85 e79a 84e7 bc96 e8be  **..............
-00000e60: 91e5 99a8 e694 afe6 8c81 2a2a efbc 9ae8  ..........**....
-00000e70: 87aa e58a a8e5 ae8c e688 90e6 97a0 e5a4  ................
-00000e80: 84e4 b88d e59c a8ef bc8c e4bb 8ee5 afb9  ................
-00000e90: e8b1 a1e5 889b e5bb bae5 88b0 e69f a5e8  ................
-00000ea0: afa2 e7bb 93e6 9e9c 5c6e 5c6e 3c70 2061  ........\n\n<p a
-00000eb0: 6c69 676e 3d22 7269 6768 7422 3e5b 3c61  lign="right">[<a
-00000ec0: 2068 7265 663d 2223 7265 6164 6d65 2d74   href="#readme-t
-00000ed0: 6f70 223e e2ac 86e5 9b9e e588 b0e9 a1b6  op">............
-00000ee0: e983 a83c 2f61 3e5d 3c2f 703e 5c6e 5c6e  ...</a>]</p>\n\n
-00000ef0: 2323 20f0 9f9a 8020 e5ae 89e8 a385 5c6e  ## .... ......\n
-00000f00: 5c6e 2323 2320 5049 505c 6e5c 6e60 6060  \n### PIP\n\n```
-00000f10: 7368 656c 6c5c 6e70 6970 2069 6e73 7461  shell\npip insta
-00000f20: 6c6c 206d 616e 676f 2d6f 646d 5c6e 6060  ll mango-odm\n``
-00000f30: 605c 6e23 2323 2050 6f65 7472 795c 6e5c  `\n### Poetry\n\
-00000f40: 6e60 6060 7368 656c 6c5c 6e70 6f65 7472  n```shell\npoetr
-00000f50: 7920 6164 6420 6d61 6e67 6f2d 6f64 6d5c  y add mango-odm\
-00000f60: 6e60 6060 5c6e 5c6e 3c70 2061 6c69 676e  n```\n\n<p align
-00000f70: 3d22 7269 6768 7422 3e5b 3c61 2068 7265  ="right">[<a hre
-00000f80: 663d 2223 7265 6164 6d65 2d74 6f70 223e  f="#readme-top">
-00000f90: e2ac 86e5 9b9e e588 b0e9 a1b6 e983 a83c  ...............<
-00000fa0: 2f61 3e5d 3c2f 703e 5c6e 5c6e 2323 20f0  /a>]</p>\n\n## .
-00000fb0: 9f8c 9f20 e7a4 bae4 be8b 5c6e 5c6e 6060  ... ......\n\n``
-00000fc0: 6070 7974 686f 6e5c 6e69 6d70 6f72 7420  `python\nimport 
-00000fd0: 6173 796e 6369 6f5c 6e5c 6e66 726f 6d20  asyncio\n\nfrom 
-00000fe0: 6d61 6e67 6f20 696d 706f 7274 2044 6f63  mango import Doc
-00000ff0: 756d 656e 742c 2045 6d62 6564 6465 6444  ument, EmbeddedD
-00001000: 6f63 756d 656e 742c 2046 6965 6c64 2c20  ocument, Field, 
-00001010: 4d61 6e67 6f5c 6e5c 6e5c 6e23 20e5 b58c  Mango\n\n\n# ...
-00001020: e585 a5e5 bc8f e696 87e6 a1a3 5c6e 636c  ............\ncl
-00001030: 6173 7320 4175 7468 6f72 2845 6d62 6564  ass Author(Embed
-00001040: 6465 6444 6f63 756d 656e 7429 3a5c 6e20  dedDocument):\n 
-00001050: 2020 206e 616d 653a 2073 7472 5c6e 2020     name: str\n  
-00001060: 2020 7072 6f66 696c 653a 2073 7472 207c    profile: str |
-00001070: 204e 6f6e 6520 3d20 4e6f 6e65 5c6e 5c6e   None = None\n\n
-00001080: 5c6e 2320 4d61 6e67 6f20 e696 87e6 a1a3  \n# Mango ......
-00001090: e6a8 a1e5 9e8b 5c6e 636c 6173 7320 426f  ......\nclass Bo
-000010a0: 6f6b 2844 6f63 756d 656e 7429 3a5c 6e20  ok(Document):\n 
-000010b0: 2020 206e 616d 653a 2073 7472 203d 2046     name: str = F
-000010c0: 6965 6c64 2870 7269 6d61 7279 5f6b 6579  ield(primary_key
-000010d0: 3d54 7275 6529 2020 2320 e5b0 86e5 ad97  =True)  # ......
-000010e0: e6ae b5e8 aebe e7bd aee4 b8ba e4b8 bbe9  ................
-000010f0: 94ae efbc 8ce5 a682 e69e 9ce4 b88d e698  ................
-00001100: bee5 bc8f e68c 87e5 ae9a e4b8 bbe9 94ae  ................
-00001110: efbc 8ce5 8899 e4bc 9ae8 87aa e58a a8e5  ................
-00001120: 889b e5bb ba20 6964 20e5 ad97 e6ae b5e4  ..... id .......
-00001130: bd9c e4b8 bae4 b8bb e994 ae5c 6e20 2020  ...........\n   
-00001140: 2073 756d 6d61 7279 3a20 7374 7220 7c20   summary: str | 
-00001150: 4e6f 6e65 203d 204e 6f6e 655c 6e20 2020  None = None\n   
-00001160: 2061 7574 686f 723a 2041 7574 686f 7220   author: Author 
-00001170: 2023 20e5 b58c e585 a5e6 9687 e6a1 a35c   # ............\
-00001180: 6e20 2020 2070 7269 6365 3a20 696e 7420  n    price: int 
-00001190: 3d20 4669 656c 6428 696e 6465 783d 5472  = Field(index=Tr
-000011a0: 7565 2920 2023 20e4 b8ba e5ad 97e6 aeb5  ue)  # .........
-000011b0: e6b7 bbe5 8aa0 e7b4 a2e5 bc95 5c6e 5c6e  ............\n\n
-000011c0: 5c6e 6173 796e 6320 6465 6620 6d61 696e  \nasync def main
-000011d0: 2829 3a5c 6e20 2020 2023 20e5 889d e5a7  ():\n    # .....
-000011e0: 8be5 8c96 204d 616e 676f efbc 8ce5 ae83  .... Mango......
-000011f0: e4bc 9ae5 889b e5bb bae8 bf9e e68e a5e5  ................
-00001200: b9b6 e588 9de5 a78b e58c 96e6 9687 e6a1  ................
-00001210: a3e6 a8a1 e59e 8bef bc8c e4bd a0e5 8faf  ................
-00001220: e4bb a5e4 bca0 e585 a520 6462 20e6 8896  ......... db ...
-00001230: e880 8520 7572 6920 e58f 82e6 95b0 e69d  ... uri ........
-00001240: a5e6 8c87 e5ae 9ae8 bf9e e68e a55c 6e20  .............\n 
-00001250: 2020 2061 7761 6974 204d 616e 676f 2e69     await Mango.i
-00001260: 6e69 7428 295c 6e5c 6e20 2020 2023 20e5  nit()\n\n    # .
-00001270: 838f 2070 7964 616e 7469 6320 e79a 84e6  .. pydantic ....
-00001280: a8a1 e59e 8be4 b880 e6a0 b7e4 bdbf e794  ................
-00001290: a85c 6e20 2020 2062 6f6f 6b20 3d20 426f  .\n    book = Bo
-000012a0: 6f6b 286e 616d 653d 2262 6f6f 6b22 2c20  ok(name="book", 
-000012b0: 6175 7468 6f72 3d41 7574 686f 7228 6e61  author=Author(na
-000012c0: 6d65 3d22 6175 7468 6f72 2229 2c20 7072  me="author"), pr
-000012d0: 6963 653d 3130 295c 6e20 2020 2023 20e5  ice=10)\n    # .
-000012e0: b086 e5ae 83e6 8f92 e585 a5e5 88b0 e695  ................
-000012f0: b0e6 8dae e5ba 93e4 b8ad 5c6e 2020 2020  ..........\n    
-00001300: 6177 6169 7420 626f 6f6b 2e73 6176 6528  await book.save(
-00001310: 295c 6e5c 6e20 2020 2023 204d 616e 676f  )\n\n    # Mango
-00001320: 20e6 8f90 e4be 9be4 ba86 e4b8 b0e5 af8c   ...............
-00001330: e79a 84e6 9fa5 e8af a2e8 afad e8a8 80ef  ................
-00001340: bc8c e585 81e8 aeb8 e682 a8e4 bdbf e794  ................
-00001350: a820 5079 7468 6f6e 20e8 a1a8 e8be bee5  . Python .......
-00001360: bc8f e69d a5e6 9fa5 e8af a25c 6e20 2020  ...........\n   
-00001370: 2069 6620 626f 6f6b 203a 3d20 6177 6169   if book := awai
-00001380: 7420 426f 6f6b 2e66 696e 6428 426f 6f6b  t Book.find(Book
-00001390: 2e70 7269 6365 203c 3d20 3230 2c20 426f  .price <= 20, Bo
-000013a0: 6f6b 2e61 7574 686f 722e 6e61 6d65 203d  ok.author.name =
-000013b0: 3d20 2261 7574 686f 7222 292e 6765 7428  = "author").get(
-000013c0: 293a 5c6e 2020 2020 2020 2020 2320 e69b  ):\n        # ..
-000013d0: b4e6 96b0 e696 87e6 a1a3 e79a 8420 7375  ............. su
-000013e0: 6d6d 6172 7920 e5ad 97e6 aeb5 5c6e 2020  mmary ......\n  
-000013f0: 2020 2020 2020 626f 6f6b 2e73 756d 6d61        book.summa
-00001400: 7279 203d 2022 7375 6d6d 6172 7922 5c6e  ry = "summary"\n
-00001410: 2020 2020 2020 2020 6177 6169 7420 626f          await bo
-00001420: 6f6b 2e75 7064 6174 6528 295c 6e5c 6e5c  ok.update()\n\n\
-00001430: 6e69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  nif __name__ == 
-00001440: 225f 5f6d 6169 6e5f 5f22 3a5c 6e20 2020  "__main__":\n   
-00001450: 2061 7379 6e63 696f 2e72 756e 286d 6169   asyncio.run(mai
-00001460: 6e28 2929 5c6e 5c6e 6060 605c 6e5c 6e3c  n())\n\n```\n\n<
-00001470: 7020 616c 6967 6e3d 2272 6967 6874 223e  p align="right">
-00001480: 5b3c 6120 6872 6566 3d22 2372 6561 646d  [<a href="#readm
-00001490: 652d 746f 7022 3ee2 ac86 e59b 9ee5 88b0  e-top">.........
-000014a0: e9a1 b6e9 83a8 3c2f 613e 5d3c 2f70 3e5c  ......</a>]</p>\
-000014b0: 6e5c 6e23 2320 f09f a49d 20e8 b4a1 e78c  n\n## .... .....
-000014c0: ae5c 6e5c 6ee6 83b3 e4b8 bae8 bf99 e4b8  .\n\n...........
-000014d0: aae9 a1b9 e79b aee5 819a e587 bae4 b880  ................
-000014e0: e4bb bde8 b4a1 e78c aee5 9097 efbc 9f5b  ...............[
-000014f0: e782 b9e5 87bb e8bf 99e9 878c 5d28 29e9  ............]().
-00001500: 9885 e8af bbe5 b9b6 e4ba 86e8 a7a3 e5a6  ................
-00001510: 82e4 bd95 e8b4 a1e7 8cae e380 825c 6e5c  .............\n\
-00001520: 6e23 2323 20f0 9f8e 8920 e9b8 a3e8 b0a2  n### .... ......
-00001530: 5c6e 5c6e e684 9fe8 b0a2 e4bb a5e4 b88b  \n\n............
-00001540: e5bc 80e5 8f91 e880 85e5 afb9 e8af a5e9  ................
-00001550: a1b9 e79b aee5 819a e587 bae7 9a84 e8b4  ................
-00001560: a1e7 8cae efbc 9a5c 6e5c 6e3c 6120 6872  .......\n\n<a hr
-00001570: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00001580: 7562 2e63 6f6d 2f41 2d6b 6972 616d 692f  ub.com/A-kirami/
-00001590: 6d61 6e67 6f2f 6772 6170 6873 2f63 6f6e  mango/graphs/con
-000015a0: 7472 6962 7574 6f72 7322 3e5c 6e20 203c  tributors">\n  <
-000015b0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000015c0: 2f63 6f6e 7472 6962 2e72 6f63 6b73 2f69  /contrib.rocks/i
-000015d0: 6d61 6765 3f72 6570 6f3d 412d 6b69 7261  mage?repo=A-kira
-000015e0: 6d69 2f6d 616e 676f 2220 2f3e 5c6e 3c2f  mi/mango" />\n</
-000015f0: 613e 5c6e 5c6e 3c70 2061 6c69 676e 3d22  a>\n\n<p align="
-00001600: 7269 6768 7422 3e5b 3c61 2068 7265 663d  right">[<a href=
-00001610: 2223 7265 6164 6d65 2d74 6f70 223e e2ac  "#readme-top">..
-00001620: 86e5 9b9e e588 b0e9 a1b6 e983 a83c 2f61  .............</a
-00001630: 3e5d 3c2f 703e 5c6e 5c6e 2323 20f0 9f92  >]</p>\n\n## ...
-00001640: 9620 e694 afe6 8c81 5c6e 5c6e e596 9ce6  . ......\n\n....
-00001650: aca2 e8bf 99e4 b8aa e9a1 b9e7 9bae efbc  ................
-00001660: 9fe8 afb7 e782 b9e4 baae 2073 7461 7220  .......... star 
-00001670: e5b9 b6e5 8886 e4ba abe5 ae83 efbc 815c  ...............\
-00001680: 6e5c 6e3c 7020 616c 6967 6e3d 2272 6967  n\n<p align="rig
-00001690: 6874 223e 5b3c 6120 6872 6566 3d22 2372  ht">[<a href="#r
-000016a0: 6561 646d 652d 746f 7022 3ee2 ac86 e59b  eadme-top">.....
-000016b0: 9ee5 88b0 e9a1 b6e9 83a8 3c2f 613e 5d3c  ..........</a>]<
-000016c0: 2f70 3e5c 6e5c 6e23 2320 f09f 939d 20e8  /p>\n\n## .... .
-000016d0: aeb8 e58f afe8 af81 5c6e 5c6e e59c a820  ........\n\n... 
-000016e0: 604d 4954 6020 e8ae b8e5 8faf e8af 81e4  `MIT` ..........
-000016f0: b88b e588 86e5 8f91 e380 82e8 afb7 e58f  ................
-00001700: 82e9 9885 205b 4c49 4345 4e53 455d 282e  .... [LICENSE](.
-00001710: 2f4c 4943 454e 5345 2920 e4bb a5e8 8eb7  /LICENSE) ......
-00001720: e58f 96e6 9bb4 e5a4 9ae4 bfa1 e681 afe3  ................
-00001730: 8082 5c6e 5c6e 3c70 2061 6c69 676e 3d22  ..\n\n<p align="
-00001740: 7269 6768 7422 3e5b 3c61 2068 7265 663d  right">[<a href=
-00001750: 2223 7265 6164 6d65 2d74 6f70 223e e2ac  "#readme-top">..
-00001760: 86e5 9b9e e588 b0e9 a1b6 e983 a83c 2f61  .............</a
-00001770: 3e5d 3c2f 703e 272c 0a20 2020 2027 6175  >]</p>',.    'au
-00001780: 7468 6f72 273a 2027 416b 6972 616d 6927  thor': 'Akirami'
-00001790: 2c0a 2020 2020 2761 7574 686f 725f 656d  ,.    'author_em
-000017a0: 6169 6c27 3a20 2761 6b69 7261 6d69 6179  ail': 'akiramiay
-000017b0: 6140 6f75 746c 6f6f 6b2e 636f 6d27 2c0a  a@outlook.com',.
-000017c0: 2020 2020 276d 6169 6e74 6169 6e65 7227      'maintainer'
-000017d0: 3a20 274e 6f6e 6527 2c0a 2020 2020 276d  : 'None',.    'm
-000017e0: 6169 6e74 6169 6e65 725f 656d 6169 6c27  aintainer_email'
-000017f0: 3a20 274e 6f6e 6527 2c0a 2020 2020 2775  : 'None',.    'u
-00001800: 726c 273a 2027 6874 7470 733a 2f2f 6769  rl': 'https://gi
-00001810: 7468 7562 2e63 6f6d 2f41 2d6b 6972 616d  thub.com/A-kiram
-00001820: 692f 6d61 6e67 6f27 2c0a 2020 2020 2770  i/mango',.    'p
-00001830: 6163 6b61 6765 7327 3a20 7061 636b 6167  ackages': packag
-00001840: 6573 2c0a 2020 2020 2770 6163 6b61 6765  es,.    'package
-00001850: 5f64 6174 6127 3a20 7061 636b 6167 655f  _data': package_
-00001860: 6461 7461 2c0a 2020 2020 2770 795f 6d6f  data,.    'py_mo
-00001870: 6475 6c65 7327 3a20 6d6f 6475 6c65 732c  dules': modules,
-00001880: 0a20 2020 2027 696e 7374 616c 6c5f 7265  .    'install_re
-00001890: 7175 6972 6573 273a 2069 6e73 7461 6c6c  quires': install
-000018a0: 5f72 6571 7569 7265 732c 0a20 2020 2027  _requires,.    '
-000018b0: 7079 7468 6f6e 5f72 6571 7569 7265 7327  python_requires'
-000018c0: 3a20 273e 3d33 2e31 302c 3c34 2e30 272c  : '>=3.10,<4.0',
-000018d0: 0a7d 0a0a 0a73 6574 7570 282a 2a73 6574  .}...setup(**set
-000018e0: 7570 5f6b 7761 7267 7329 0a              up_kwargs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6d61 6e67  : 2.1.Name: mang
+00000020: 6f2d 6f64 6d0a 5665 7273 696f 6e3a 2030  o-odm.Version: 0
+00000030: 2e33 2e31 0a53 756d 6d61 7279 3a20 f09f  .3.1.Summary: ..
+00000040: a5ad 2041 7379 6e63 204d 6f6e 676f 4442  .. Async MongoDB
+00000050: 204f 444d 2077 6974 6820 7479 7065 2068   ODM with type h
+00000060: 696e 7473 2069 6e20 5079 7468 6f6e 0a4b  ints in Python.K
+00000070: 6579 776f 7264 733a 206d 6f6e 676f 206d  eywords: mongo m
+00000080: 6f6e 676f 6462 2061 7379 6e63 2061 7379  ongodb async asy
+00000090: 6e63 696f 206f 646d 2074 7970 6573 2070  ncio odm types p
+000000a0: 7964 616e 7469 6320 6d6f 746f 720a 4175  ydantic motor.Au
+000000b0: 7468 6f72 2d45 6d61 696c 3a20 416b 6972  thor-Email: Akir
+000000c0: 616d 6920 3c61 6b69 7261 6d69 6179 6140  ami <akiramiaya@
+000000d0: 6f75 746c 6f6f 6b2e 636f 6d3e 0a4c 6963  outlook.com>.Lic
+000000e0: 656e 7365 3a20 4d49 540a 436c 6173 7369  ense: MIT.Classi
+000000f0: 6669 6572 3a20 4465 7665 6c6f 706d 656e  fier: Developmen
+00000100: 7420 5374 6174 7573 203a 3a20 3420 2d20  t Status :: 4 - 
+00000110: 4265 7461 0a43 6c61 7373 6966 6965 723a  Beta.Classifier:
+00000120: 2046 7261 6d65 776f 726b 203a 3a20 4173   Framework :: As
+00000130: 796e 6349 4f0a 436c 6173 7369 6669 6572  yncIO.Classifier
+00000140: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
+00000150: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+00000160: 730a 436c 6173 7369 6669 6572 3a20 4c69  s.Classifier: Li
+00000170: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000180: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+00000190: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
+000001a0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
+000001b0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+000001c0: 656e 740a 436c 6173 7369 6669 6572 3a20  ent.Classifier: 
+000001d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001e0: 7561 6765 203a 3a20 5079 7468 6f6e 0a43  uage :: Python.C
+000001f0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000200: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000210: 3a3a 2050 7974 686f 6e20 3a3a 2033 0a43  :: Python :: 3.C
+00000220: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000230: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000240: 3a3a 2050 7974 686f 6e20 3a3a 2033 203a  :: Python :: 3 :
+00000250: 3a20 4f6e 6c79 0a43 6c61 7373 6966 6965  : Only.Classifie
+00000260: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000270: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000280: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
+00000290: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000002a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000002b0: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
+000002c0: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
+000002d0: 3a20 4461 7461 6261 7365 0a43 6c61 7373  : Database.Class
+000002e0: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+000002f0: 4461 7461 6261 7365 203a 3a20 4672 6f6e  Database :: Fron
+00000300: 742d 456e 6473 0a43 6c61 7373 6966 6965  t-Ends.Classifie
+00000310: 723a 2054 6f70 6963 203a 3a20 536f 6674  r: Topic :: Soft
+00000320: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+00000330: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000340: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
+00000350: 6576 656c 6f70 6d65 6e74 203a 3a20 4f62  evelopment :: Ob
+00000360: 6a65 6374 2042 726f 6b65 7269 6e67 0a43  ject Brokering.C
+00000370: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+00000380: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
+00000390: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
+000003a0: 6172 6965 730a 436c 6173 7369 6669 6572  aries.Classifier
+000003b0: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
+000003c0: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
+000003d0: 3a3a 204c 6962 7261 7269 6573 203a 3a20  :: Libraries :: 
+000003e0: 5079 7468 6f6e 204d 6f64 756c 6573 0a43  Python Modules.C
+000003f0: 6c61 7373 6966 6965 723a 2054 7970 696e  lassifier: Typin
+00000400: 6720 3a3a 2054 7970 6564 0a50 726f 6a65  g :: Typed.Proje
+00000410: 6374 2d55 524c 3a20 5265 706f 7369 746f  ct-URL: Reposito
+00000420: 7279 2c20 6874 7470 733a 2f2f 6769 7468  ry, https://gith
+00000430: 7562 2e63 6f6d 2f41 2d6b 6972 616d 692f  ub.com/A-kirami/
+00000440: 6d61 6e67 6f0a 5265 7175 6972 6573 2d50  mango.Requires-P
+00000450: 7974 686f 6e3a 203c 342e 302c 3e3d 332e  ython: <4.0,>=3.
+00000460: 3130 0a52 6571 7569 7265 732d 4469 7374  10.Requires-Dist
+00000470: 3a20 6d6f 746f 723e 3d33 2e32 2e30 0a52  : motor>=3.2.0.R
+00000480: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000490: 6461 6e74 6963 3c32 2e30 2e30 2c3e 3d31  dantic<2.0.0,>=1
+000004a0: 2e31 302e 3132 0a44 6573 6372 6970 7469  .10.12.Descripti
+000004b0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+000004c0: 2074 6578 742f 6d61 726b 646f 776e 0a0a   text/markdown..
+000004d0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+000004e0: 223e 0a20 2020 203c 6120 6e61 6d65 3d22  ">.    <a name="
+000004f0: 7265 6164 6d65 2d74 6f70 223e 3c2f 613e  readme-top"></a>
+00000500: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000510: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000520: 2f41 2d6b 6972 616d 692f 6d61 6e67 6f22  /A-kirami/mango"
+00000530: 3e0a 2020 2020 2020 2020 3c69 6d67 2077  >.        <img w
+00000540: 6964 7468 3d22 3134 3070 7822 2073 7263  idth="140px" src
+00000550: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+00000560: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000570: 636f 6d2f 412d 6b69 7261 6d69 2f6d 616e  com/A-kirami/man
+00000580: 676f 2f6d 6169 6e2f 6173 7365 7473 2f6d  go/main/assets/m
+00000590: 616e 676f 2d6c 6f67 6f2e 7376 6722 2061  ango-logo.svg" a
+000005a0: 6c69 676e 3d22 6365 6e74 6572 2220 616c  lign="center" al
+000005b0: 743d 224d 616e 676f 2220 2f3e 0a20 2020  t="Mango" />.   
+000005c0: 203c 2f61 3e0a 2020 2020 3c68 3120 616c   </a>.    <h1 al
+000005d0: 6967 6e3d 2263 656e 7465 7222 3e4d 616e  ign="center">Man
+000005e0: 676f 3c2f 6831 3e0a 2020 2020 3c70 2061  go</h1>.    <p a
+000005f0: 6c69 676e 3d22 6365 6e74 6572 223e f09f  lign="center">..
+00000600: a5ad 20e5 b8a6 e69c 89e7 b1bb e59e 8be6  .. .............
+00000610: 8f90 e7a4 bae7 9a84 2050 7974 686f 6e20  ........ Python 
+00000620: e5bc 82e6 ada5 204d 6f6e 676f 4442 20e5  ...... MongoDB .
+00000630: afb9 e8b1 a1e6 9687 e6a1 a3e6 98a0 e5b0  ................
+00000640: 84e5 99a8 3c2f 703e 0a3c 2f70 3e0a 3c70  ....</p>.</p>.<p
+00000650: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000660: 0a20 2020 203c 6120 6872 6566 3d22 2e2f  .    <a href="./
+00000670: 4c49 4345 4e53 4522 3e0a 2020 2020 2020  LICENSE">.      
+00000680: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000690: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000006a0: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
+000006b0: 652f 412d 6b69 7261 6d69 2f6d 616e 676f  e/A-kirami/mango
+000006c0: 2e73 7667 2220 616c 743d 226c 6963 656e  .svg" alt="licen
+000006d0: 7365 223e 0a20 2020 203c 2f61 3e0a 2020  se">.    </a>.  
+000006e0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000006f0: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+00000700: 7267 2f70 7970 692f 6d61 6e67 6f2d 6f64  rg/pypi/mango-od
+00000710: 6d22 3e0a 2020 2020 2020 2020 3c69 6d67  m">.        <img
+00000720: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000730: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000740: 692f 762f 6d61 6e67 6f2d 6f64 6d2e 7376  i/v/mango-odm.sv
+00000750: 6722 2061 6c74 3d22 7079 7069 223e 0a20  g" alt="pypi">. 
+00000760: 2020 203c 2f61 3e0a 2020 2020 3c61 2068     </a>.    <a h
+00000770: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+00000780: 2e70 7974 686f 6e2e 6f72 672f 223e 0a20  .python.org/">. 
+00000790: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+000007a0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+000007b0: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
+000007c0: 7468 6f6e 2d33 2e31 302b 2d62 6c75 652e  thon-3.10+-blue.
+000007d0: 7376 6722 2061 6c74 3d22 7079 7468 6f6e  svg" alt="python
+000007e0: 223e 0a20 2020 203c 2f61 3e0a 3c2f 703e  ">.    </a>.</p>
+000007f0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000800: 7222 3e0a 2020 2020 3c61 2068 7265 663d  r">.    <a href=
+00000810: 2223 2de7 a4ba e4be 8b22 3ee6 9fa5 e79c  "#-......">.....
+00000820: 8be6 bc94 e7a4 ba3c 2f61 3e0a 2020 2020  .......</a>.    
+00000830: c2b7 0a20 2020 203c 6120 6872 6566 3d22  ...    <a href="
+00000840: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000850: 6f6d 2f41 2d6b 6972 616d 692f 6d61 6e67  om/A-kirami/mang
+00000860: 6f2f 6973 7375 6573 2f6e 6577 3f61 7373  o/issues/new?ass
+00000870: 6967 6e65 6573 3d26 6c61 6265 6c73 3d62  ignees=&labels=b
+00000880: 7567 2674 656d 706c 6174 653d 6275 675f  ug&template=bug_
+00000890: 7265 706f 7274 2e79 6d6c 2674 6974 6c65  report.yml&title
+000008a0: 3d25 3542 4255 4725 3544 2533 412b 223e  =%5BBUG%5D%3A+">
+000008b0: e994 99e8 afaf e68a a5e5 918a 3c2f 613e  ............</a>
+000008c0: 0a20 2020 20c2 b70a 2020 2020 3c61 2068  .    ...    <a h
+000008d0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+000008e0: 6875 622e 636f 6d2f 412d 6b69 7261 6d69  hub.com/A-kirami
+000008f0: 2f6d 616e 676f 2f69 7373 7565 732f 6e65  /mango/issues/ne
+00000900: 773f 6173 7369 676e 6565 733d 266c 6162  w?assignees=&lab
+00000910: 656c 733d 656e 6861 6e63 656d 656e 7426  els=enhancement&
+00000920: 7465 6d70 6c61 7465 3d66 6561 7475 7265  template=feature
+00000930: 5f72 6571 7565 7374 2e79 6d6c 2674 6974  _request.yml&tit
+00000940: 6c65 3d25 3542 4665 6174 7572 6525 3544  le=%5BFeature%5D
+00000950: 2533 412b 223e e58a 9fe8 83bd e8af b7e6  %3A+">..........
+00000960: b182 3c2f 613e 0a3c 2f70 3e0a 3c70 2061  ..</a>.</p>.<p a
+00000970: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+00000980: 2020 203c 7374 726f 6e67 3ee7 ae80 e4bd     <strong>.....
+00000990: 93e4 b8ad e696 873c 2f73 7472 6f6e 673e  .......</strong>
+000009a0: 0a20 2020 20c2 b70a 2020 2020 3c61 2068  .    ...    <a h
+000009b0: 7265 663d 222f 646f 6373 2f52 4541 444d  ref="/docs/READM
+000009c0: 455f 454e 2e6d 6422 3e45 6e67 6c69 7368  E_EN.md">English
+000009d0: 3c2f 613e 0a20 2020 20c2 b70a 2020 2020  </a>.    ...    
+000009e0: 3c61 2068 7265 663d 222f 646f 6373 2f52  <a href="/docs/R
+000009f0: 4541 444d 455f 4a41 2e6d 6422 3ee6 97a5  EADME_JA.md">...
+00000a00: e69c ace8 aa9e 3c2f 613e 0a3c 2f70 3e0a  ......</a>.</p>.
+00000a10: 0a23 2320 f09f 9496 20e7 9bae e5bd 950a  .## .... .......
+00000a20: 0a3c 6465 7461 696c 7320 6f70 656e 3d22  .<details open="
+00000a30: 6f70 656e 223e 0a20 203c 7375 6d6d 6172  open">.  <summar
+00000a40: 793e e79b aee5 bd95 3c2f 7375 6d6d 6172  y>......</summar
+00000a50: 793e 0a20 203c 756c 3e0a 2020 2020 3c6c  y>.  <ul>.    <l
+00000a60: 693e 0a20 2020 2020 2020 203c 6120 6872  i>.        <a hr
+00000a70: 6566 3d22 232d e7ae 80e4 bb8b 223e e7ae  ef="#-......">..
+00000a80: 80e4 bb8b 3c2f 613e 0a20 2020 2020 2020  ....</a>.       
+00000a90: 203c 756c 3e0a 2020 2020 2020 2020 2020   <ul>.          
+00000aa0: 2020 3c6c 693e 3c61 2068 7265 663d 2223    <li><a href="#
+00000ab0: 2de6 a0b8 e5bf 83e7 89b9 e680 a722 3ee6  -............">.
+00000ac0: a0b8 e5bf 83e7 89b9 e680 a73c 2f61 3e3c  ...........</a><
+00000ad0: 2f6c 693e 0a20 2020 2020 2020 203c 2f75  /li>.        </u
+00000ae0: 6c3e 0a20 2020 203c 2f6c 693e 0a20 2020  l>.    </li>.   
+00000af0: 203c 6c69 3e0a 2020 2020 2020 2020 3c61   <li>.        <a
+00000b00: 2068 7265 663d 2223 2de5 ae89 e8a3 8522   href="#-......"
+00000b10: 3ee5 ae89 e8a3 853c 2f61 3e0a 2020 2020  >......</a>.    
+00000b20: 2020 2020 3c75 6c3e 0a20 2020 2020 2020      <ul>.       
+00000b30: 2020 2020 203c 6c69 3e3c 6120 6872 6566       <li><a href
+00000b40: 3d22 2350 4950 223e 5049 503c 2f61 3e3c  ="#PIP">PIP</a><
+00000b50: 2f6c 693e 0a20 2020 2020 2020 2020 2020  /li>.           
+00000b60: 203c 6c69 3e3c 6120 6872 6566 3d22 2350   <li><a href="#P
+00000b70: 6f65 7472 7922 3e50 6f65 7472 793c 2f61  oetry">Poetry</a
+00000b80: 3e3c 2f6c 693e 0a20 2020 2020 2020 203c  ></li>.        <
+00000b90: 2f75 6c3e 0a20 2020 203c 2f6c 693e 0a20  /ul>.    </li>. 
+00000ba0: 2020 203c 6c69 3e0a 2020 2020 2020 2020     <li>.        
+00000bb0: 3c61 2068 7265 663d 2223 2de7 a4ba e4be  <a href="#-.....
+00000bc0: 8b22 3ee7 a4ba e4be 8b3c 2f61 3e0a 2020  .">......</a>.  
+00000bd0: 2020 3c2f 6c69 3e0a 2020 2020 3c6c 693e    </li>.    <li>
+00000be0: 0a20 2020 2020 2020 203c 6120 6872 6566  .        <a href
+00000bf0: 3d22 232d e8b4 a1e7 8cae 223e e8b4 a1e7  ="#-......">....
+00000c00: 8cae 3c2f 613e 0a20 2020 2020 2020 203c  ..</a>.        <
+00000c10: 756c 3e0a 2020 2020 2020 2020 2020 2020  ul>.            
+00000c20: 3c6c 693e 3c61 2068 7265 663d 2223 2de9  <li><a href="#-.
+00000c30: b8a3 e8b0 a222 3ee9 b8a3 e8b0 a23c 2f61  .....">......</a
+00000c40: 3e3c 2f6c 693e 0a20 2020 2020 2020 203c  ></li>.        <
+00000c50: 2f75 6c3e 0a20 2020 203c 2f6c 693e 0a20  /ul>.    </li>. 
+00000c60: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
+00000c70: 232d e694 afe6 8c81 223e e694 afe6 8c81  #-......">......
+00000c80: 3c2f 613e 3c2f 6c69 3e0a 2020 2020 3c6c  </a></li>.    <l
+00000c90: 693e 3c61 2068 7265 663d 2223 2de8 aeb8  i><a href="#-...
+00000ca0: e58f afe8 af81 223e e8ae b8e5 8faf e8af  ......">........
+00000cb0: 813c 2f61 3e3c 2f6c 693e 0a20 203c 2f75  .</a></li>.  </u
+00000cc0: 6c3e 0a3c 2f64 6574 6169 6c73 3e0a 0a23  l>.</details>..#
+00000cd0: 2320 f09f 9396 20e7 ae80 e4bb 8b0a 0a4d  # .... ........M
+00000ce0: 616e 676f 20e6 98af e4b8 80e4 b8aa e5b8  ango ...........
+00000cf0: a6e6 9c89 e7b1 bbe5 9e8b e68f 90e7 a4ba  ................
+00000d00: e79a 8420 5079 7468 6f6e 20e5 bc82 e6ad  ... Python .....
+00000d10: a520 4d6f 6e67 6f44 4220 e5af b9e8 b1a1  . MongoDB ......
+00000d20: e696 87e6 a1a3 e698 a0e5 b084 e599 a828  ...............(
+00000d30: 4f44 4d29 efbc 8ce5 ae83 e69e 84e5 bbba  ODM)............
+00000d40: e59c a820 5b4d 6f74 6f72 5d28 6874 7470  ... [Motor](http
+00000d50: 733a 2f2f 6d6f 746f 722e 7265 6164 7468  s://motor.readth
+00000d60: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+00000d70: 6c65 2f29 20e5 928c 205b 5079 6461 6e74  le/) ... [Pydant
+00000d80: 6963 5d28 6874 7470 733a 2f2f 7079 6461  ic](https://pyda
+00000d90: 6e74 6963 2d64 6f63 732e 6865 6c70 6d61  ntic-docs.helpma
+00000da0: 6e75 616c 2e69 6f2f 2920 e4b9 8be4 b88a  nual.io/) ......
+00000db0: e380 820a 0a4d 616e 676f 20e4 bdbf e5be  .....Mango .....
+00000dc0: 97e6 95b0 e68d aee5 bbba e6a8 a1e5 928c  ................
+00000dd0: e69f a5e8 afa2 e58f 98e5 be97 e99d 9ee5  ................
+00000de0: b8b8 e5ae b9e6 9893 efbc 8ce5 b8ae e58a  ................
+00000df0: a9e6 82a8 e585 b3e6 b3a8 e5ba 94e7 94a8  ................
+00000e00: e7a8 8be5 ba8f e4b8 ade7 9c9f e6ad a3e9  ................
+00000e10: 878d e8a6 81e7 9a84 e983 a8e5 8886 e380  ................
+00000e20: 820a 0a23 2323 20e2 9ca8 20e6 a0b8 e5bf  ...### ... .....
+00000e30: 83e7 89b9 e680 a7ef bc9a 0a0a 2d20 2a2a  ............- **
+00000e40: e5ae 8ce5 9684 e79a 84e7 b1bb e59e 8be6  ................
+00000e50: a087 e6b3 a82a 2aef bc9a e588 a9e7 94a8  .....**.........
+00000e60: e99d 99e6 8081 e588 86e6 9e90 e69d a5e5  ................
+00000e70: 878f e5b0 91e8 bf90 e8a1 8ce6 97b6 e997  ................
+00000e80: aee9 a298 0a2d 202a 2ae7 ae80 e6b4 81e6  .....- **.......
+00000e90: b581 e795 85e7 9a84 2041 5049 2a2a efbc  ........ API**..
+00000ea0: 9ae6 9bb4 e698 93e4 ba8e e5ad a6e4 b9a0  ................
+00000eb0: e592 8ce4 bdbf e794 a8ef bc8c e68f 90e9  ................
+00000ec0: ab98 e5bc 80e5 8f91 e695 88e7 8e87 0a2d  ...............-
+00000ed0: 202a 2ae4 bc98 e99b 85e7 9a84 e7bc 96e8   **.............
+00000ee0: be91 e599 a8e6 94af e68c 812a 2aef bc9a  ...........**...
+00000ef0: e887 aae5 8aa8 e5ae 8ce6 8890 e697 a0e5  ................
+00000f00: a484 e4b8 8de5 9ca8 efbc 8ce4 bb8e e5af  ................
+00000f10: b9e8 b1a1 e588 9be5 bbba e588 b0e6 9fa5  ................
+00000f20: e8af a2e7 bb93 e69e 9c0a 0a3c 7020 616c  ...........<p al
+00000f30: 6967 6e3d 2272 6967 6874 223e 5b3c 6120  ign="right">[<a 
+00000f40: 6872 6566 3d22 2372 6561 646d 652d 746f  href="#readme-to
+00000f50: 7022 3ee2 ac86 e59b 9ee5 88b0 e9a1 b6e9  p">.............
+00000f60: 83a8 3c2f 613e 5d3c 2f70 3e0a 0a23 2320  ..</a>]</p>..## 
+00000f70: f09f 9a80 20e5 ae89 e8a3 850a 0a23 2323  .... ........###
+00000f80: 2050 4950 0a0a 6060 6073 6865 6c6c 0a70   PIP..```shell.p
+00000f90: 6970 2069 6e73 7461 6c6c 206d 616e 676f  ip install mango
+00000fa0: 2d6f 646d 0a60 6060 0a23 2323 2050 6f65  -odm.```.### Poe
+00000fb0: 7472 790a 0a60 6060 7368 656c 6c0a 706f  try..```shell.po
+00000fc0: 6574 7279 2061 6464 206d 616e 676f 2d6f  etry add mango-o
+00000fd0: 646d 0a60 6060 0a0a 3c70 2061 6c69 676e  dm.```..<p align
+00000fe0: 3d22 7269 6768 7422 3e5b 3c61 2068 7265  ="right">[<a hre
+00000ff0: 663d 2223 7265 6164 6d65 2d74 6f70 223e  f="#readme-top">
+00001000: e2ac 86e5 9b9e e588 b0e9 a1b6 e983 a83c  ...............<
+00001010: 2f61 3e5d 3c2f 703e 0a0a 2323 20f0 9f8c  /a>]</p>..## ...
+00001020: 9f20 e7a4 bae4 be8b 0a0a 6060 6070 7974  . ........```pyt
+00001030: 686f 6e0a 696d 706f 7274 2061 7379 6e63  hon.import async
+00001040: 696f 0a0a 6672 6f6d 206d 616e 676f 2069  io..from mango i
+00001050: 6d70 6f72 7420 446f 6375 6d65 6e74 2c20  mport Document, 
+00001060: 456d 6265 6464 6564 446f 6375 6d65 6e74  EmbeddedDocument
+00001070: 2c20 4669 656c 642c 204d 616e 676f 0a0a  , Field, Mango..
+00001080: 0a23 20e5 b58c e585 a5e5 bc8f e696 87e6  .# .............
+00001090: a1a3 0a63 6c61 7373 2041 7574 686f 7228  ...class Author(
+000010a0: 456d 6265 6464 6564 446f 6375 6d65 6e74  EmbeddedDocument
+000010b0: 293a 0a20 2020 206e 616d 653a 2073 7472  ):.    name: str
+000010c0: 0a20 2020 2070 726f 6669 6c65 3a20 7374  .    profile: st
+000010d0: 7220 7c20 4e6f 6e65 203d 204e 6f6e 650a  r | None = None.
+000010e0: 0a0a 2320 4d61 6e67 6f20 e696 87e6 a1a3  ..# Mango ......
+000010f0: e6a8 a1e5 9e8b 0a63 6c61 7373 2042 6f6f  .......class Boo
+00001100: 6b28 446f 6375 6d65 6e74 293a 0a20 2020  k(Document):.   
+00001110: 206e 616d 653a 2073 7472 203d 2046 6965   name: str = Fie
+00001120: 6c64 2870 7269 6d61 7279 5f6b 6579 3d54  ld(primary_key=T
+00001130: 7275 6529 2020 2320 e5b0 86e5 ad97 e6ae  rue)  # ........
+00001140: b5e8 aebe e7bd aee4 b8ba e4b8 bbe9 94ae  ................
+00001150: efbc 8ce5 a682 e69e 9ce4 b88d e698 bee5  ................
+00001160: bc8f e68c 87e5 ae9a e4b8 bbe9 94ae efbc  ................
+00001170: 8ce5 8899 e4bc 9ae8 87aa e58a a8e5 889b  ................
+00001180: e5bb ba20 6964 20e5 ad97 e6ae b5e4 bd9c  ... id .........
+00001190: e4b8 bae4 b8bb e994 ae0a 2020 2020 7375  ..........    su
+000011a0: 6d6d 6172 793a 2073 7472 207c 204e 6f6e  mmary: str | Non
+000011b0: 6520 3d20 4e6f 6e65 0a20 2020 2061 7574  e = None.    aut
+000011c0: 686f 723a 2041 7574 686f 7220 2023 20e5  hor: Author  # .
+000011d0: b58c e585 a5e6 9687 e6a1 a30a 2020 2020  ............    
+000011e0: 7072 6963 653a 2069 6e74 203d 2046 6965  price: int = Fie
+000011f0: 6c64 2869 6e64 6578 3d54 7275 6529 2020  ld(index=True)  
+00001200: 2320 e4b8 bae5 ad97 e6ae b5e6 b7bb e58a  # ..............
+00001210: a0e7 b4a2 e5bc 950a 0a0a 6173 796e 6320  ..........async 
+00001220: 6465 6620 6d61 696e 2829 3a0a 2020 2020  def main():.    
+00001230: 2320 e588 9de5 a78b e58c 9620 4d61 6e67  # ......... Mang
+00001240: 6fef bc8c e5ae 83e4 bc9a e588 9be5 bbba  o...............
+00001250: e8bf 9ee6 8ea5 e5b9 b6e5 889d e5a7 8be5  ................
+00001260: 8c96 e696 87e6 a1a3 e6a8 a1e5 9e8b efbc  ................
+00001270: 8ce4 bda0 e58f afe4 bba5 e4bc a0e5 85a5  ................
+00001280: 2064 6220 e688 96e8 8085 2075 7269 20e5   db ...... uri .
+00001290: 8f82 e695 b0e6 9da5 e68c 87e5 ae9a e8bf  ................
+000012a0: 9ee6 8ea5 0a20 2020 2061 7761 6974 204d  .....    await M
+000012b0: 616e 676f 2e69 6e69 7428 290a 0a20 2020  ango.init()..   
+000012c0: 2023 20e5 838f 2070 7964 616e 7469 6320   # ... pydantic 
+000012d0: e79a 84e6 a8a1 e59e 8be4 b880 e6a0 b7e4  ................
+000012e0: bdbf e794 a80a 2020 2020 626f 6f6b 203d  ......    book =
+000012f0: 2042 6f6f 6b28 6e61 6d65 3d22 626f 6f6b   Book(name="book
+00001300: 222c 2061 7574 686f 723d 4175 7468 6f72  ", author=Author
+00001310: 286e 616d 653d 2261 7574 686f 7222 292c  (name="author"),
+00001320: 2070 7269 6365 3d31 3029 0a20 2020 2023   price=10).    #
+00001330: 20e5 b086 e5ae 83e6 8f92 e585 a5e5 88b0   ...............
+00001340: e695 b0e6 8dae e5ba 93e4 b8ad 0a20 2020  .............   
+00001350: 2061 7761 6974 2062 6f6f 6b2e 7361 7665   await book.save
+00001360: 2829 0a0a 2020 2020 2320 4d61 6e67 6f20  ()..    # Mango 
+00001370: e68f 90e4 be9b e4ba 86e4 b8b0 e5af 8ce7  ................
+00001380: 9a84 e69f a5e8 afa2 e8af ade8 a880 efbc  ................
+00001390: 8ce5 8581 e8ae b8e6 82a8 e4bd bfe7 94a8  ................
+000013a0: 2050 7974 686f 6e20 e8a1 a8e8 bebe e5bc   Python ........
+000013b0: 8fe6 9da5 e69f a5e8 afa2 0a20 2020 2069  ...........    i
+000013c0: 6620 626f 6f6b 203a 3d20 6177 6169 7420  f book := await 
+000013d0: 426f 6f6b 2e66 696e 6428 426f 6f6b 2e70  Book.find(Book.p
+000013e0: 7269 6365 203c 3d20 3230 2c20 426f 6f6b  rice <= 20, Book
+000013f0: 2e61 7574 686f 722e 6e61 6d65 203d 3d20  .author.name == 
+00001400: 2261 7574 686f 7222 292e 6765 7428 293a  "author").get():
+00001410: 0a20 2020 2020 2020 2023 20e6 9bb4 e696  .        # .....
+00001420: b0e6 9687 e6a1 a3e7 9a84 2073 756d 6d61  .......... summa
+00001430: 7279 20e5 ad97 e6ae b50a 2020 2020 2020  ry .......      
+00001440: 2020 626f 6f6b 2e73 756d 6d61 7279 203d    book.summary =
+00001450: 2022 7375 6d6d 6172 7922 0a20 2020 2020   "summary".     
+00001460: 2020 2061 7761 6974 2062 6f6f 6b2e 7570     await book.up
+00001470: 6461 7465 2829 0a0a 0a69 6620 5f5f 6e61  date()...if __na
+00001480: 6d65 5f5f 203d 3d20 225f 5f6d 6169 6e5f  me__ == "__main_
+00001490: 5f22 3a0a 2020 2020 6173 796e 6369 6f2e  _":.    asyncio.
+000014a0: 7275 6e28 6d61 696e 2829 290a 0a60 6060  run(main())..```
+000014b0: 0a0a 3c70 2061 6c69 676e 3d22 7269 6768  ..<p align="righ
+000014c0: 7422 3e5b 3c61 2068 7265 663d 2223 7265  t">[<a href="#re
+000014d0: 6164 6d65 2d74 6f70 223e e2ac 86e5 9b9e  adme-top">......
+000014e0: e588 b0e9 a1b6 e983 a83c 2f61 3e5d 3c2f  .........</a>]</
+000014f0: 703e 0a0a 2323 20f0 9fa4 9d20 e8b4 a1e7  p>..## .... ....
+00001500: 8cae 0a0a e683 b3e4 b8ba e8bf 99e4 b8aa  ................
+00001510: e9a1 b9e7 9bae e581 9ae5 87ba e4b8 80e4  ................
+00001520: bbbd e8b4 a1e7 8cae e590 97ef bc9f 5be7  ..............[.
+00001530: 82b9 e587 bbe8 bf99 e987 8c5d 2829 e998  ...........]()..
+00001540: 85e8 afbb e5b9 b6e4 ba86 e8a7 a3e5 a682  ................
+00001550: e4bd 95e8 b4a1 e78c aee3 8082 0a0a 2323  ..............##
+00001560: 2320 f09f 8e89 20e9 b8a3 e8b0 a20a 0ae6  # .... .........
+00001570: 849f e8b0 a2e4 bba5 e4b8 8be5 bc80 e58f  ................
+00001580: 91e8 8085 e5af b9e8 afa5 e9a1 b9e7 9bae  ................
+00001590: e581 9ae5 87ba e79a 84e8 b4a1 e78c aeef  ................
+000015a0: bc9a 0a0a 3c61 2068 7265 663d 2268 7474  ....<a href="htt
+000015b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000015c0: 412d 6b69 7261 6d69 2f6d 616e 676f 2f67  A-kirami/mango/g
+000015d0: 7261 7068 732f 636f 6e74 7269 6275 746f  raphs/contributo
+000015e0: 7273 223e 0a20 203c 696d 6720 7372 633d  rs">.  <img src=
+000015f0: 2268 7474 7073 3a2f 2f63 6f6e 7472 6962  "https://contrib
+00001600: 2e72 6f63 6b73 2f69 6d61 6765 3f72 6570  .rocks/image?rep
+00001610: 6f3d 412d 6b69 7261 6d69 2f6d 616e 676f  o=A-kirami/mango
+00001620: 2220 2f3e 0a3c 2f61 3e0a 0a3c 7020 616c  " />.</a>..<p al
+00001630: 6967 6e3d 2272 6967 6874 223e 5b3c 6120  ign="right">[<a 
+00001640: 6872 6566 3d22 2372 6561 646d 652d 746f  href="#readme-to
+00001650: 7022 3ee2 ac86 e59b 9ee5 88b0 e9a1 b6e9  p">.............
+00001660: 83a8 3c2f 613e 5d3c 2f70 3e0a 0a23 2320  ..</a>]</p>..## 
+00001670: f09f 9296 20e6 94af e68c 810a 0ae5 969c  .... ...........
+00001680: e6ac a2e8 bf99 e4b8 aae9 a1b9 e79b aeef  ................
+00001690: bc9f e8af b7e7 82b9 e4ba ae20 7374 6172  ........... star
+000016a0: 20e5 b9b6 e588 86e4 baab e5ae 83ef bc81   ...............
+000016b0: 0a0a 3c70 2061 6c69 676e 3d22 7269 6768  ..<p align="righ
+000016c0: 7422 3e5b 3c61 2068 7265 663d 2223 7265  t">[<a href="#re
+000016d0: 6164 6d65 2d74 6f70 223e e2ac 86e5 9b9e  adme-top">......
+000016e0: e588 b0e9 a1b6 e983 a83c 2f61 3e5d 3c2f  .........</a>]</
+000016f0: 703e 0a0a 2323 20f0 9f93 9d20 e8ae b8e5  p>..## .... ....
+00001700: 8faf e8af 810a 0ae5 9ca8 2060 4d49 5460  .......... `MIT`
+00001710: 20e8 aeb8 e58f afe8 af81 e4b8 8be5 8886   ...............
+00001720: e58f 91e3 8082 e8af b7e5 8f82 e998 8520  ............... 
+00001730: 5b4c 4943 454e 5345 5d28 2e2f 4c49 4345  [LICENSE](./LICE
+00001740: 4e53 4529 20e4 bba5 e88e b7e5 8f96 e69b  NSE) ...........
+00001750: b4e5 a49a e4bf a1e6 81af e380 820a 0a3c  ...............<
+00001760: 7020 616c 6967 6e3d 2272 6967 6874 223e  p align="right">
+00001770: 5b3c 6120 6872 6566 3d22 2372 6561 646d  [<a href="#readm
+00001780: 652d 746f 7022 3ee2 ac86 e59b 9ee5 88b0  e-top">.........
+00001790: e9a1 b6e9 83a8 3c2f 613e 5d3c 2f70 3e    ......</a>]</p>
```

### Comparing `mango_odm-0.3.0/PKG-INFO` & `mango_odm-0.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,40 @@
-Metadata-Version: 2.1
-Name: mango-odm
-Version: 0.3.0
-Summary: 🥭 Async MongoDB ODM with type hints in Python
-Home-page: https://github.com/A-kirami/mango
-License: MIT
-Author: Akirami
-Author-email: akiramiaya@outlook.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: motor (>=3.0.0,<4.0.0)
-Requires-Dist: pydantic (>=1.10.0,<2.0.0)
-Project-URL: Repository, https://github.com/A-kirami/mango
-Description-Content-Type: text/markdown
-
 <p align="center">
     <a name="readme-top"></a>
     <a href="https://github.com/A-kirami/mango">
         <img width="140px" src="https://raw.githubusercontent.com/A-kirami/mango/main/assets/mango-logo.svg" align="center" alt="Mango" />
     </a>
     <h1 align="center">Mango</h1>
     <p align="center">🥭 带有类型提示的 Python 异步 MongoDB 对象文档映射器</p>
 </p>
-    <p align="center">
-        <a href="./LICENSE">
-            <img src="https://img.shields.io/github/license/A-kirami/mango.svg" alt="license">
-        </a>
-        <a href="https://pypi.python.org/pypi/mango-odm">
-            <img src="https://img.shields.io/pypi/v/mango-odm.svg" alt="pypi">
-        </a>
-        <a href="https://www.python.org/">
-            <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
-        </a>
-    </p>
-    <p align="center">
-        <a href="#-示例">查看演示</a>
-        ·
-        <a href="https://github.com/A-kirami/mango/issues/new?assignees=&labels=bug&template=bug_report.yml&title=%5BBUG%5D%3A+">错误报告</a>
-        ·
-        <a href="https://github.com/A-kirami/mango/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature%5D%3A+">功能请求</a>
-    </p>
-    <p align="center">
-        <strong>简体中文</strong>
-        ·
-        <a href="/docs/README_EN.md">English</a>
-        ·
-        <a href="/docs/README_JA.md">日本語</a>
-    </p>
+<p align="center">
+    <a href="./LICENSE">
+        <img src="https://img.shields.io/github/license/A-kirami/mango.svg" alt="license">
+    </a>
+    <a href="https://pypi.python.org/pypi/mango-odm">
+        <img src="https://img.shields.io/pypi/v/mango-odm.svg" alt="pypi">
+    </a>
+    <a href="https://www.python.org/">
+        <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
+    </a>
 </p>
 <p align="center">
+    <a href="#-示例">查看演示</a>
+    ·
+    <a href="https://github.com/A-kirami/mango/issues/new?assignees=&labels=bug&template=bug_report.yml&title=%5BBUG%5D%3A+">错误报告</a>
+    ·
+    <a href="https://github.com/A-kirami/mango/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature%5D%3A+">功能请求</a>
+</p>
+<p align="center">
+    <strong>简体中文</strong>
+    ·
+    <a href="/docs/README_EN.md">English</a>
+    ·
+    <a href="/docs/README_JA.md">日本語</a>
+</p>
 
 ## 🔖 目录
 
 <details open="open">
   <summary>目录</summary>
   <ul>
     <li>
@@ -68,22 +48,14 @@
         <ul>
             <li><a href="#PIP">PIP</a></li>
             <li><a href="#Poetry">Poetry</a></li>
         </ul>
     </li>
     <li>
         <a href="#-示例">示例</a>
-        <ul>
-            <li><a href="#创建您的第一个模型">创建您的第一个模型</a></li>
-            <li><a href="#将数据保存到数据库">将数据保存到数据库</a></li>
-            <li><a href="#查找符合条件的文档">查找符合条件的文档</a></li>
-            <li><a href="#修改数据库中的文档">修改数据库中的文档</a></li>
-            <li><a href="#嵌入式模型">嵌入式模型</a></li>
-            <li><a href="#连接数据库">连接数据库</a></li>
-        </ul>
     </li>
     <li>
         <a href="#-贡献">贡献</a>
         <ul>
             <li><a href="#-鸣谢">鸣谢</a></li>
         </ul>
     </li>
@@ -186,8 +158,8 @@
 
 <p align="right">[<a href="#readme-top">⬆回到顶部</a>]</p>
 
 ## 📝 许可证
 
 在 `MIT` 许可证下分发。请参阅 [LICENSE](./LICENSE) 以获取更多信息。
 
-<p align="right">[<a href="#readme-top">⬆回到顶部</a>]</p>
+<p align="right">[<a href="#readme-top">⬆回到顶部</a>]</p>
```

