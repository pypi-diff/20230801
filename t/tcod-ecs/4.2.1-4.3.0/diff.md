# Comparing `tmp/tcod_ecs-4.2.1.tar.gz` & `tmp/tcod_ecs-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod_ecs-4.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tcod_ecs-4.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcod_ecs-4.2.1.tar` & `tcod_ecs-4.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1079 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/LICENSE
--rw-r--r--   0        0        0    10905 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/README.md
--rw-r--r--   0        0        0     3527 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/pyproject.toml
--rw-r--r--   0        0        0     1394 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/__init__.py
--rw-r--r--   0        0        0     1512 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/_converter.py
--rw-r--r--   0        0        0      160 2023-07-29 01:38:41.763200 tcod_ecs-4.2.1/tcod/ecs/_version.py
--rw-r--r--   0        0        0    30100 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/entity.py
--rw-r--r--   0        0        0        0 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/py.typed
--rw-r--r--   0        0        0    14844 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/query.py
--rw-r--r--   0        0        0     1113 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/typing.py
--rw-r--r--   0        0        0    11647 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/world.py
--rw-r--r--   0        0        0    12159 1970-01-01 00:00:00.000000 tcod_ecs-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-08-01 16:55:31.807826 tcod_ecs-4.3.0/LICENSE
+-rw-r--r--   0        0        0    10905 2023-08-01 16:55:31.807826 tcod_ecs-4.3.0/README.md
+-rw-r--r--   0        0        0     3527 2023-08-01 16:55:31.807826 tcod_ecs-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1394 2023-08-01 16:55:31.807826 tcod_ecs-4.3.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0     1512 2023-08-01 16:55:31.807826 tcod_ecs-4.3.0/tcod/ecs/_converter.py
+-rw-r--r--   0        0        0      160 2023-08-01 16:55:41.451897 tcod_ecs-4.3.0/tcod/ecs/_version.py
+-rw-r--r--   0        0        0     2377 2023-08-01 16:55:31.807826 tcod_ecs-4.3.0/tcod/ecs/callbacks.py
+-rw-r--r--   0        0        0    30814 2023-08-01 16:55:31.807826 tcod_ecs-4.3.0/tcod/ecs/entity.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:55:31.807826 tcod_ecs-4.3.0/tcod/ecs/py.typed
+-rw-r--r--   0        0        0    14802 2023-08-01 16:55:31.807826 tcod_ecs-4.3.0/tcod/ecs/query.py
+-rw-r--r--   0        0        0     1116 2023-08-01 16:55:31.807826 tcod_ecs-4.3.0/tcod/ecs/typing.py
+-rw-r--r--   0        0        0    11638 2023-08-01 16:55:31.807826 tcod_ecs-4.3.0/tcod/ecs/world.py
+-rw-r--r--   0        0        0    12159 1970-01-01 00:00:00.000000 tcod_ecs-4.3.0/PKG-INFO
```

### Comparing `tcod_ecs-4.2.1/LICENSE` & `tcod_ecs-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.1/README.md` & `tcod_ecs-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.1/pyproject.toml` & `tcod_ecs-4.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.1/tcod/ecs/__init__.py` & `tcod_ecs-4.3.0/tcod/ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.1/tcod/ecs/_converter.py` & `tcod_ecs-4.3.0/tcod/ecs/_converter.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.1/tcod/ecs/entity.py` & `tcod_ecs-4.3.0/tcod/ecs/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     TypeVar,
     Union,
 )
 from weakref import WeakKeyDictionary, WeakValueDictionary
 
 from typing_extensions import Self
 
+import tcod.ecs.callbacks
 import tcod.ecs.query
-from tcod.ecs.typing import _ComponentKey
+from tcod.ecs.typing import ComponentKey
 
 if TYPE_CHECKING:
     from _typeshed import SupportsKeysAndGetItem
 
     from tcod.ecs.world import World
 
 
@@ -307,57 +308,66 @@
             FutureWarning,
             stacklevel=_stacklevel + 1,
         )
         key = getattr(value, "_TCOD_BASE_COMPONENT", value.__class__)
         self[key] = value
 
     @staticmethod
-    def __assert_key(key: _ComponentKey[Any]) -> bool:
+    def __assert_key(key: ComponentKey[Any]) -> bool:
         """Verify that abstract classes are accessed correctly."""
         if isinstance(key, tuple):
             key = key[1]
         assert (
             getattr(key, "_TCOD_BASE_COMPONENT", key) is key
         ), "Abstract components must be accessed via the base class."
         return True
 
-    def __getitem__(self, key: _ComponentKey[T]) -> T:
+    def __getitem__(self, key: ComponentKey[T]) -> T:
         """Return a component belonging to this entity."""
         assert self.__assert_key(key)
         return self.entity.world._components_by_entity[self.entity][key]  # type: ignore[no-any-return]
 
-    def __setitem__(self, key: _ComponentKey[T], value: T) -> None:
+    def __setitem__(self, key: ComponentKey[T], value: T) -> None:
         """Assign a component to an entity."""
         assert self.__assert_key(key)
 
-        if key not in self.entity.world._components_by_entity[self.entity]:
+        old_value = self.entity.world._components_by_entity[self.entity].get(key)
+
+        if old_value is None:
             tcod.ecs.query._touch_component(self.entity.world, key)  # Component added
+        elif old_value == value:
+            return
 
         self.entity.world._components_by_entity[self.entity][key] = value
         self.entity.world._components_by_type[key][self.entity] = value
 
+        tcod.ecs.callbacks._on_component_changed(key, self.entity, old_value, value)
+
     def __delitem__(self, key: type[object] | tuple[object, type[object]]) -> None:
         """Delete a component from an entity."""
         assert self.__assert_key(key)
 
+        old_value = self.entity.world._components_by_entity[self.entity].get(key)
+
         del self.entity.world._components_by_entity[self.entity][key]
         if not self.entity.world._components_by_entity[self.entity]:
             del self.entity.world._components_by_entity[self.entity]
 
         del self.entity.world._components_by_type[key][self.entity]
         if not self.entity.world._components_by_type[key]:
             del self.entity.world._components_by_type[key]
 
         tcod.ecs.query._touch_component(self.entity.world, key)  # Component removed
+        tcod.ecs.callbacks._on_component_changed(key, self.entity, old_value, None)
 
-    def __contains__(self, key: _ComponentKey[object]) -> bool:  # type: ignore[override]
+    def __contains__(self, key: ComponentKey[object]) -> bool:  # type: ignore[override]
         """Return True if this entity has the provided component."""
         return key in self.entity.world._components_by_entity.get(self.entity, ())
 
-    def __iter__(self) -> Iterator[_ComponentKey[Any]]:
+    def __iter__(self) -> Iterator[ComponentKey[Any]]:
         """Iterate over the component types belonging to this entity."""
         return iter(self.entity.world._components_by_entity.get(self.entity, ()))
 
     def __len__(self) -> int:
         """Return the number of components belonging to this entity."""
         return len(self.entity.world._components_by_entity.get(self.entity, ()))
 
@@ -384,31 +394,31 @@
             if not isinstance(key, tuple):
                 continue
             key_name, key_component = key
             if key_component is component_type and isinstance(key_name, name_type):
                 yield key_name, key_component
 
     def __ior__(
-        self, value: SupportsKeysAndGetItem[_ComponentKey[Any], Any] | Iterable[tuple[_ComponentKey[Any], Any]]
+        self, value: SupportsKeysAndGetItem[ComponentKey[Any], Any] | Iterable[tuple[ComponentKey[Any], Any]]
     ) -> Self:
         """Update components in-place.
 
         .. versionadded:: 3.4
         """
         self.update(value)
         return self
 
-    def get(self, __key: _ComponentKey[T], __default: T | None = None) -> T | None:
+    def get(self, __key: ComponentKey[T], __default: T | None = None) -> T | None:
         """Return a component, returns None or a default value when the component is missing."""
         try:
             return self[__key]
         except KeyError:
             return __default
 
-    def setdefault(self, __key: _ComponentKey[T], __default: T) -> T:  # type: ignore[override]
+    def setdefault(self, __key: ComponentKey[T], __default: T) -> T:  # type: ignore[override]
         """Assign a default value if a component is missing, then returns the current value."""
         try:
             return self[__key]
         except KeyError:
             self[__key] = __default
             return __default
 
@@ -657,29 +667,36 @@
     """An entity-component mapping to access the relation target component objects.
 
     See :any:`Entity.relation_components`.
     """
 
     __slots__ = ("entity", "key")
 
-    def __init__(self, entity: Entity, key: _ComponentKey[T]) -> None:
+    def __init__(self, entity: Entity, key: ComponentKey[T]) -> None:
         """Initialize this attribute for the given entity."""
         assert isinstance(entity, Entity), entity
         self.entity: Final = entity
-        self.key: _ComponentKey[T] = key
+        self.key: ComponentKey[T] = key
 
     def __getitem__(self, target: Entity) -> T:
         """Return the component related to a target entity."""
         return self.entity.world._relation_components_by_entity[self.entity][self.key][target]  # type: ignore[no-any-return]
 
     def __setitem__(self, target: Entity, component: T) -> None:
         """Assign a component to the target entity."""
         world = self.entity.world
-        if target in world._relation_components_by_entity[self.entity][self.key] is not None:
-            del self[target]
+
+        old_value = world._relation_components_by_entity[self.entity][self.key].get(target)
+        if old_value is None:  # Relation added
+            tcod.ecs.query._touch_relations(
+                world, ((self.key, target), (self.key, ...), (self.entity, self.key, None), (..., self.key, None))
+            )
+        elif old_value == component:
+            return
+
         world._relation_components_by_entity[self.entity][self.key][target] = component
 
         world._relations_lookup[(self.key, target)] = {self.entity}
         world._relations_lookup[(self.key, ...)].add(self.entity)
         world._relations_lookup[(self.entity, self.key, None)] = {target}
         world._relations_lookup[(..., self.key, None)].add(target)
 
@@ -704,77 +721,81 @@
         if not world._relations_lookup[(self.entity, self.key, None)]:
             del world._relations_lookup[(self.entity, self.key, None)]
 
         world._relations_lookup[(..., self.key, None)].discard(target)
         if not world._relations_lookup[(..., self.key, None)]:
             del world._relations_lookup[(..., self.key, None)]
 
+        tcod.ecs.query._touch_relations(
+            world, ((self.key, target), (self.key, ...), (self.entity, self.key, None), (..., self.key, None))
+        )
+
     def __iter__(self) -> Iterator[Entity]:
         """Iterate over the targets with assigned components."""
         by_entity = self.entity.world._relation_components_by_entity.get(self.entity)
         return iter(()) if by_entity is None else iter(by_entity.get(self.key, ()))
 
     def __len__(self) -> int:
         """Return the count of targets for this component relation."""
         by_entity = self.entity.world._relation_components_by_entity.get(self.entity)
         return 0 if by_entity is None else len(by_entity.get(self.key, ()))
 
 
-class EntityComponentRelations(MutableMapping[_ComponentKey[Any], EntityComponentRelationMapping[Any]]):
+class EntityComponentRelations(MutableMapping[ComponentKey[Any], EntityComponentRelationMapping[Any]]):
     """Proxy to access the component relations of an entity.
 
     See :any:`Entity.relation_components`.
 
     ..versionchanged:: 4.2.0
-        Is now a :any:`MutableMapping` subtype.
+        Is now a :any:`collections.abc.MutableMapping` subtype.
     """
 
     __slots__ = ("entity",)
 
     def __init__(self, entity: Entity) -> None:
         """Initialize this attribute for the given entity."""
         assert isinstance(entity, Entity), entity
         self.entity: Final = entity
 
-    def __getitem__(self, key: _ComponentKey[T]) -> EntityComponentRelationMapping[T]:
+    def __getitem__(self, key: ComponentKey[T]) -> EntityComponentRelationMapping[T]:
         """Access relations for this component key as a `{target: component}` dict-like object."""
         return EntityComponentRelationMapping(self.entity, key)
 
-    def __setitem__(self, __key: _ComponentKey[T], __values: Mapping[Entity, object]) -> None:
+    def __setitem__(self, __key: ComponentKey[T], __values: Mapping[Entity, object]) -> None:
         """Redefine the component relations for this entity.
 
         ..versionadded:: 4.2.0
         """
         if isinstance(__values, EntityComponentRelationMapping) and __values.entity is self.entity:
             return
         mapping: EntityComponentRelationMapping[object] = self[__key]
         mapping.clear()
         for target, component in __values.items():
             mapping[target] = component
 
-    def __delitem__(self, key: _ComponentKey[object]) -> None:
+    def __delitem__(self, key: ComponentKey[object]) -> None:
         """Remove all relations associated with this component key."""
         EntityComponentRelationMapping(self.entity, key).clear()
 
     def __contains__(self, key: object) -> bool:
         """Return True if this entity contains a relation component for this component key."""
-        return key in self.keys()  # noqa: SIM118 # https://github.com/astral-sh/ruff/issues/6163
+        return key in self.keys()
 
     def clear(self) -> None:
         """Clears the relation components this entity has with other entities.
 
         Does not clear relations targeting this entity.
         """
         for component_key in list(self):
             self[component_key].clear()
 
-    def keys(self) -> KeysView[_ComponentKey[object]]:
+    def keys(self) -> KeysView[ComponentKey[object]]:
         """Returns the components keys this entity has relations for."""
         return self.entity.world._relation_components_by_entity.get(self.entity, {}).keys()
 
-    def __iter__(self) -> Iterator[_ComponentKey[object]]:
+    def __iter__(self) -> Iterator[ComponentKey[object]]:
         """Iterates over the component keys this entity has relations for."""
         return iter(self.keys())
 
     def __len__(self) -> int:
         """Returns the number of unique component keys this entity has relations for."""
         return len(self.entity.world._relation_components_by_entity.get(self.entity, ()))
```

### Comparing `tcod_ecs-4.2.1/tcod/ecs/query.py` & `tcod_ecs-4.3.0/tcod/ecs/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import TYPE_CHECKING, AbstractSet, Any, Iterable, Iterator, TypeVar, overload
 from weakref import WeakKeyDictionary, WeakSet
 
 import attrs
 from typing_extensions import Self
 
 import tcod.ecs.entity
-from tcod.ecs.typing import _ComponentKey, _RelationQuery
+from tcod.ecs.typing import ComponentKey, _RelationQuery
 
 if TYPE_CHECKING:
     from tcod.ecs.entity import Entity
     from tcod.ecs.world import World
 
 _T1 = TypeVar("_T1")
 _T2 = TypeVar("_T2")
@@ -30,17 +30,15 @@
 
 @attrs.define
 class _QueryCache:
     """Main data structure for the query cache."""
 
     queries: dict[Query, set[Entity]] = attrs.field(factory=dict)
     """Table of cached queries."""
-    by_components: defaultdict[_ComponentKey[object], WeakSet[Query]] = attrs.field(
-        factory=lambda: defaultdict(WeakSet)
-    )
+    by_components: defaultdict[ComponentKey[object], WeakSet[Query]] = attrs.field(factory=lambda: defaultdict(WeakSet))
     """Which queries depend on which components."""
     by_tags: defaultdict[object, WeakSet[Query]] = attrs.field(factory=lambda: defaultdict(WeakSet))
     """Which queries depend on which tags."""
     by_relations: defaultdict[_RelationQuery, WeakSet[Query]] = attrs.field(factory=lambda: defaultdict(WeakSet))
     """Which queries depend on which relations."""
 
     dependencies: dict[Query, set[tuple[World, Query]]] = attrs.field(factory=lambda: defaultdict(set))
@@ -53,15 +51,15 @@
 def _drop_cached_query(cache: _QueryCache, query: Query) -> None:
     """Drop a cached query and all of its dependant queries."""
     cache.queries.pop(query, None)
     for sub_world, sub_query in cache.dependencies.pop(query, ()):
         _drop_cached_query(_query_caches[sub_world], sub_query)
 
 
-def _touch_component(world: World, component: _ComponentKey[object]) -> None:
+def _touch_component(world: World, component: ComponentKey[object]) -> None:
     """Drop cached queries if a component change has invalidated them."""
     cache = _get_query_cache(world)
     if component not in cache.by_components:
         return
     for touched_query in cache.by_components.pop(component, ()):
         _drop_cached_query(cache, touched_query)
 
@@ -119,15 +117,15 @@
 
     world = origin.world
     return set().union(*(world._relations_lookup.get((entity, tag, None), ()) for entity in origin))
 
 
 def _fetch_lookup_tables(
     world: World,
-    components: frozenset[_ComponentKey[object]],
+    components: frozenset[ComponentKey[object]],
     tags: frozenset[object],
     relations: frozenset[_RelationQuery],
 ) -> Iterator[AbstractSet[Entity]]:
     """Iterate over the relevant sets for this world and query."""
     for component in components:
         yield world._components_by_type.get(component, {}).keys()
     for tag in tags:
@@ -221,30 +219,30 @@
     return relation
 
 
 @attrs.define(frozen=True)
 class Query:
     """A set of conditions used to lookup entities in a World."""
 
-    _all_of_components: frozenset[_ComponentKey[object]] = frozenset()
-    _none_of_components: frozenset[_ComponentKey[object]] = frozenset()
+    _all_of_components: frozenset[ComponentKey[object]] = frozenset()
+    _none_of_components: frozenset[ComponentKey[object]] = frozenset()
     _all_of_tags: frozenset[object] = frozenset()
     _none_of_tags: frozenset[object] = frozenset()
     _all_of_relations: frozenset[_RelationQuery] = frozenset()
     _none_of_relations: frozenset[_RelationQuery] = frozenset()
 
     def __attrs_post_init__(self) -> None:
         """Verify the current state."""
         assert self._all_of_components.isdisjoint(self._none_of_components)
         assert self._all_of_tags.isdisjoint(self._none_of_tags)
         assert self._all_of_relations.isdisjoint(self._none_of_relations)
 
     def all_of(
         self,
-        components: Iterable[_ComponentKey[object]] = (),
+        components: Iterable[ComponentKey[object]] = (),
         *,
         tags: Iterable[object] = (),
         relations: Iterable[_RelationQuery] = (),
         _stacklevel: int = 1,
     ) -> Self:
         """Filter entities based on having all of the provided elements."""
         _check_suspicious_tags(tags, stacklevel=_stacklevel + 1)
@@ -255,15 +253,15 @@
             self._none_of_tags,
             self._all_of_relations.union(_normalize_query_relation(relation) for relation in relations),
             self._none_of_relations,
         )
 
     def none_of(
         self,
-        components: Iterable[_ComponentKey[object]] = (),
+        components: Iterable[ComponentKey[object]] = (),
         *,
         tags: Iterable[object] = (),
         relations: Iterable[_RelationQuery] = (),
         _stacklevel: int = 1,
     ) -> Self:
         """Filter entities based on having none of the provided elements."""
         _check_suspicious_tags(tags, stacklevel=_stacklevel + 1)
@@ -300,77 +298,77 @@
 @attrs.define(frozen=True)
 class WorldQuery:
     """Collect a set of entities with the provided conditions."""
 
     world: World
     _query: Query = attrs.field(factory=Query)
 
-    def _get_entities(self, extra_components: AbstractSet[_ComponentKey[object]] = frozenset()) -> set[Entity]:
+    def _get_entities(self, extra_components: AbstractSet[ComponentKey[object]] = frozenset()) -> set[Entity]:
         return _get_query(self.all_of(components=extra_components))
 
     def all_of(
         self,
-        components: Iterable[_ComponentKey[object]] = (),
+        components: Iterable[ComponentKey[object]] = (),
         *,
         tags: Iterable[object] = (),
         relations: Iterable[_RelationQuery] = (),
     ) -> Self:
         """Filter entities based on having all of the provided elements."""
         return self.__class__(
             self.world, self._query.all_of(components=components, tags=tags, relations=relations, _stacklevel=2)
         )
 
     def none_of(
         self,
-        components: Iterable[_ComponentKey[object]] = (),
+        components: Iterable[ComponentKey[object]] = (),
         *,
         tags: Iterable[object] = (),
         relations: Iterable[_RelationQuery] = (),
     ) -> Self:
         """Filter entities based on having none of the provided elements."""
         return self.__class__(
             self.world, self._query.none_of(components=components, tags=tags, relations=relations, _stacklevel=2)
         )
 
     def __iter__(self) -> Iterator[Entity]:
         """Iterate over the matching entities."""
         return iter(self._get_entities())
 
     @overload
-    def __getitem__(self, key: tuple[_ComponentKey[_T1]]) -> Iterable[tuple[_T1]]:
+    def __getitem__(self, key: tuple[ComponentKey[_T1]]) -> Iterable[tuple[_T1]]:
         ...
 
     @overload
-    def __getitem__(self, key: tuple[_ComponentKey[_T1], _ComponentKey[_T2]]) -> Iterable[tuple[_T1, _T2]]:
+    def __getitem__(self, key: tuple[ComponentKey[_T1], ComponentKey[_T2]]) -> Iterable[tuple[_T1, _T2]]:
         ...
 
     @overload
     def __getitem__(
-        self, key: tuple[_ComponentKey[_T1], _ComponentKey[_T2], _ComponentKey[_T3]]
+        self, key: tuple[ComponentKey[_T1], ComponentKey[_T2], ComponentKey[_T3]]
     ) -> Iterable[tuple[_T1, _T2, _T3]]:
         ...
 
     @overload
     def __getitem__(
-        self, key: tuple[_ComponentKey[_T1], _ComponentKey[_T2], _ComponentKey[_T3], _ComponentKey[_T4]]
+        self, key: tuple[ComponentKey[_T1], ComponentKey[_T2], ComponentKey[_T3], ComponentKey[_T4]]
     ) -> Iterable[tuple[_T1, _T2, _T3, _T4]]:
         ...
 
     @overload
     def __getitem__(
         self,
-        key: tuple[_ComponentKey[_T1], _ComponentKey[_T2], _ComponentKey[_T3], _ComponentKey[_T4], _ComponentKey[_T5]],
+        key: tuple[ComponentKey[_T1], ComponentKey[_T2], ComponentKey[_T3], ComponentKey[_T4], ComponentKey[_T5]],
     ) -> Iterable[tuple[_T1, _T2, _T3, _T4, _T5]]:
         ...
 
     @overload
-    def __getitem__(self, key: tuple[_ComponentKey[object], ...]) -> Iterable[tuple[Any, ...]]:
+    def __getitem__(self, key: tuple[ComponentKey[object], ...]) -> Iterable[tuple[Any, ...]]:
         ...
 
-    def __getitem__(self, key: tuple[_ComponentKey[object], ...]) -> Iterable[tuple[Any, ...]]:
+    def __getitem__(self, key: tuple[ComponentKey[object], ...]) -> Iterable[tuple[Any, ...]]:
         """Collect components from a query."""
         assert key is not None
         assert isinstance(key, tuple)
 
         Entity = tcod.ecs.entity.Entity
 
         entities = list(self._get_entities(set(key) - {Entity}))
```

### Comparing `tcod_ecs-4.2.1/tcod/ecs/typing.py` & `tcod_ecs-4.3.0/tcod/ecs/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     WorldQuery = Any
 
 if sys.version_info >= (3, 10):  # pragma: no cover
     EllipsisType: TypeAlias = types.EllipsisType
 else:  # pragma: no cover
     EllipsisType = Any
 
-T = TypeVar("T")
+_T = TypeVar("_T")
 
-_ComponentKey: TypeAlias = Union[Type[T], Tuple[object, Type[T]]]
+ComponentKey: TypeAlias = Union[Type[_T], Tuple[object, Type[_T]]]
 """ComponentKey is plain `type` or tuple `(tag, type)`."""
 
 _RelationTargetLookup: TypeAlias = Union[Entity, EllipsisType]
 """Possible target for stored relations."""
 
 _RelationQueryTarget: TypeAlias = Union[_RelationTargetLookup, WorldQuery]
 """Possible target for relation queries."""
```

### Comparing `tcod_ecs-4.2.1/tcod/ecs/world.py` & `tcod_ecs-4.3.0/tcod/ecs/world.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, DefaultDict, Dict, Iterable, Mapping, Set, TypeVar
 
 import attrs
 
 import tcod.ecs._converter
 import tcod.ecs.query
 from tcod.ecs.entity import Entity
-from tcod.ecs.typing import _ComponentKey, _RelationTargetLookup
+from tcod.ecs.typing import ComponentKey, _RelationTargetLookup
 
 _T1 = TypeVar("_T1")
 _T2 = TypeVar("_T2")
 _T3 = TypeVar("_T3")
 
 
 def _defaultdict_of_set() -> defaultdict[_T1, set[_T2]]:
@@ -24,18 +24,18 @@
 
 def _defaultdict_of_dict() -> defaultdict[_T1, dict[_T2, _T3]]:
     """Return a new defaultdict of dicts."""
     return defaultdict(dict)
 
 
 def _components_by_entity_from(
-    by_type: defaultdict[_ComponentKey[object], dict[Entity, Any]]
-) -> defaultdict[Entity, dict[_ComponentKey[object], Any]]:
+    by_type: defaultdict[ComponentKey[object], dict[Entity, Any]]
+) -> defaultdict[Entity, dict[ComponentKey[object], Any]]:
     """Return the component lookup table from the components sparse-set."""
-    by_entity: defaultdict[Entity, dict[_ComponentKey[object], Any]] = defaultdict(dict)
+    by_entity: defaultdict[Entity, dict[ComponentKey[object], Any]] = defaultdict(dict)
     for component_key, components in by_type.items():
         for entity, component in components.items():
             by_entity[entity][component_key] = component
     return by_entity
 
 
 def _tags_by_key_from_tags_by_entity(by_entity: defaultdict[Entity, set[object]]) -> defaultdict[object, set[Entity]]:
@@ -45,15 +45,15 @@
         for tag in tags:
             tags_by_key[tag].add(entity)
     return tags_by_key
 
 
 def _relations_lookup_from(
     tags_by_entity: defaultdict[Entity, defaultdict[object, set[Entity]]],
-    components_by_entity: defaultdict[Entity, defaultdict[_ComponentKey[object], dict[Entity, Any]]],
+    components_by_entity: defaultdict[Entity, defaultdict[ComponentKey[object], dict[Entity, Any]]],
 ) -> defaultdict[tuple[Any, _RelationTargetLookup] | tuple[_RelationTargetLookup, Any, None], set[Entity]]:
     """Return the relation lookup table from the relations sparse-sets."""
     relations_lookup: defaultdict[
         tuple[Any, _RelationTargetLookup] | tuple[_RelationTargetLookup, Any, None], set[Entity]
     ] = defaultdict(set)
     for origin, tags in tags_by_entity.items():
         for tag, targets in tags.items():
@@ -73,22 +73,22 @@
     return relations_lookup
 
 
 @attrs.define(eq=False)
 class World:
     """A container for entities and components."""
 
-    _components_by_entity: defaultdict[Entity, dict[_ComponentKey[object], Any]] = attrs.field(
+    _components_by_entity: defaultdict[Entity, dict[ComponentKey[object], Any]] = attrs.field(
         init=False, factory=lambda: defaultdict(dict)
     )
     """Random access entity components.
 
     dict[Entity][ComponentKey] = component_instance
     """
-    _components_by_type: defaultdict[_ComponentKey[object], dict[Entity, Any]] = attrs.field(
+    _components_by_type: defaultdict[ComponentKey[object], dict[Entity, Any]] = attrs.field(
         init=False, factory=lambda: defaultdict(dict)
     )
     """Query table entity components.
 
     dict[ComponentKey] = {entities_with_component}
     """
 
@@ -107,15 +107,15 @@
         init=False, factory=lambda: defaultdict(_defaultdict_of_set)
     )
     """Random access tag multi-relations.
 
     dict[entity][tag] = {target_entities}
     """
     _relation_components_by_entity: defaultdict[
-        Entity, defaultdict[_ComponentKey[object], dict[Entity, Any]]
+        Entity, defaultdict[ComponentKey[object], dict[Entity, Any]]
     ] = attrs.field(init=False, factory=lambda: defaultdict(_defaultdict_of_dict))
     """Random access relations owning components.
 
     dict[entity][ComponentKey][target_entity] = component
     """
     _relations_lookup: defaultdict[
         tuple[Any, _RelationTargetLookup] | tuple[_RelationTargetLookup, Any, None], set[Entity]
@@ -260,15 +260,15 @@
         .. deprecated:: 3.1
             This feature has been deprecated.
         """
         return self._names_by_name
 
     def new_entity(
         self,
-        components: Iterable[object] | Mapping[_ComponentKey[object], object] = (),
+        components: Iterable[object] | Mapping[ComponentKey[object], object] = (),
         *,
         name: object = None,
         tags: Iterable[Any] = (),
     ) -> Entity:
         """Create and return a new entity.
 
         .. versionchanged:: 3.1
```

### Comparing `tcod_ecs-4.2.1/PKG-INFO` & `tcod_ecs-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 4.2.1
+Version: 4.3.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

