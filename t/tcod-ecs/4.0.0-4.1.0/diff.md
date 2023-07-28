# Comparing `tmp/tcod_ecs-4.0.0.tar.gz` & `tmp/tcod_ecs-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod_ecs-4.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tcod_ecs-4.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcod_ecs-4.0.0.tar` & `tcod_ecs-4.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1079 2023-07-26 13:05:26.038310 tcod_ecs-4.0.0/LICENSE
--rw-r--r--   0        0        0    10473 2023-07-26 13:05:26.038310 tcod_ecs-4.0.0/README.md
--rw-r--r--   0        0        0     3527 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     1394 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0     1512 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/_converter.py
--rw-r--r--   0        0        0      160 2023-07-26 13:05:35.514398 tcod_ecs-4.0.0/tcod/ecs/_version.py
--rw-r--r--   0        0        0    28196 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/entity.py
--rw-r--r--   0        0        0        0 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/py.typed
--rw-r--r--   0        0        0    11466 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/query.py
--rw-r--r--   0        0        0      914 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/typing.py
--rw-r--r--   0        0        0    11638 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/world.py
--rw-r--r--   0        0        0    11727 1970-01-01 00:00:00.000000 tcod_ecs-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-28 13:55:08.163962 tcod_ecs-4.1.0/LICENSE
+-rw-r--r--   0        0        0    10905 2023-07-28 13:55:08.163962 tcod_ecs-4.1.0/README.md
+-rw-r--r--   0        0        0     3527 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1394 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0     1512 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/_converter.py
+-rw-r--r--   0        0        0      160 2023-07-28 13:55:18.652201 tcod_ecs-4.1.0/tcod/ecs/_version.py
+-rw-r--r--   0        0        0    28196 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/entity.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/py.typed
+-rw-r--r--   0        0        0    14844 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/query.py
+-rw-r--r--   0        0        0     1113 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/typing.py
+-rw-r--r--   0        0        0    11647 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/world.py
+-rw-r--r--   0        0        0    12159 1970-01-01 00:00:00.000000 tcod_ecs-4.1.0/PKG-INFO
```

### Comparing `tcod_ecs-4.0.0/LICENSE` & `tcod_ecs-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.0.0/README.md` & `tcod_ecs-4.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # About
 
 [![PyPI](https://img.shields.io/pypi/v/tcod-ecs)](https://pypi.org/project/tcod-ecs/)
 [![PyPI - License](https://img.shields.io/pypi/l/tcod-ecs)](https://github.com/HexDecimal/python-tcod-ecs/blob/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/python-tcod-ecs/badge/?version=latest)](https://python-tcod-ecs.readthedocs.io)
 [![codecov](https://codecov.io/gh/HexDecimal/python-tcod-ecs/branch/main/graph/badge.svg?token=4Ak5QpTLZB)](https://codecov.io/gh/HexDecimal/python-tcod-ecs)
+[![CommitsSinceLastRelease](https://img.shields.io/github/commits-since/HexDecimal/python-tcod-ecs/latest)](https://github.com/HexDecimal/python-tcod-ecs/blob/main/CHANGELOG.md)
 
 `tcod-ecs` is a [Sparse-set](https://skypjack.github.io/2020-08-02-ecs-baf-part-9/) [Entity-component-system](https://en.wikipedia.org/wiki/Entity_component_system) implemented using Python's `dict` and `set` types.
 See the [ECS FAQ](https://github.com/SanderMertens/ecs-faq) for more info.
 
 This implementation focuses on type-hinting, organization, and is designed to work well with Python.
 The following features are currently implemented:
 
@@ -242,10 +243,12 @@
 
 You can use the following table to help with constructing relation queries.
 `tag` is a component key if you are querying for a component relation.
 
 | Includes                                                              | Syntax |
 | --------------------------------------------------------------------- | :----: |
 | Entities with a relation tag to the given target                      | `(tag, target_entity)` |
-| Entities with a relation tag to any target                            | `(tag, ...)` |
-| Entities which are a relation target of a given entity                | `(origin_entity, tag, None)` |
-| Entities which are a target of any entity with the given relation tag | `(..., tag, None)` |
+| Entities with a relation tag to any target                            | `(tag, ...)` (Literal dot-dot-dot) |
+| Entities with a relation tag to the targets in the given query        | `(tag, world.Q.all_of(...))` |
+| The target entities of a relation of a given entity                   | `(origin_entity, tag, None)` |
+| The target entities of any entity with the given relation tag         | `(..., tag, None)` (Literal dot-dot-dot) |
+| The target entities of the queried entities with the given relation   | `(tag, world.Q.all_of(...))` |
```

### Comparing `tcod_ecs-4.0.0/pyproject.toml` & `tcod_ecs-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.0.0/tcod/ecs/__init__.py` & `tcod_ecs-4.1.0/tcod/ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.0.0/tcod/ecs/_converter.py` & `tcod_ecs-4.1.0/tcod/ecs/_converter.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.0.0/tcod/ecs/entity.py` & `tcod_ecs-4.1.0/tcod/ecs/entity.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.0.0/tcod/ecs/query.py` & `tcod_ecs-4.1.0/tcod/ecs/query.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tools for querying  World objects."""
 from __future__ import annotations
 
 import itertools
 import warnings
 from collections import defaultdict
-from typing import TYPE_CHECKING, AbstractSet, Any, Final, Iterable, Iterator, TypeVar, overload
+from typing import TYPE_CHECKING, AbstractSet, Any, Iterable, Iterator, TypeVar, overload
 from weakref import WeakKeyDictionary, WeakSet
 
 import attrs
 from typing_extensions import Self
 
 import tcod.ecs.entity
 from tcod.ecs.typing import _ComponentKey, _RelationQuery
@@ -39,47 +39,54 @@
     )
     """Which queries depend on which components."""
     by_tags: defaultdict[object, WeakSet[Query]] = attrs.field(factory=lambda: defaultdict(WeakSet))
     """Which queries depend on which tags."""
     by_relations: defaultdict[_RelationQuery, WeakSet[Query]] = attrs.field(factory=lambda: defaultdict(WeakSet))
     """Which queries depend on which relations."""
 
+    dependencies: dict[Query, set[tuple[World, Query]]] = attrs.field(factory=lambda: defaultdict(set))
+    """Tracks which queries depend on the queries of the current world.
+
+    `dependencies[dependency] = {dependant}`
+    """
+
+
+def _drop_cached_query(cache: _QueryCache, query: Query) -> None:
+    """Drop a cached query and all of its dependant queries."""
+    cache.queries.pop(query, None)
+    for sub_world, sub_query in cache.dependencies.pop(query, ()):
+        _drop_cached_query(_query_caches[sub_world], sub_query)
+
 
 def _touch_component(world: World, component: _ComponentKey[object]) -> None:
     """Drop cached queries if a component change has invalidated them."""
-    cache = _query_caches.get(world)
-    if cache is None:
-        return
+    cache = _get_query_cache(world)
     if component not in cache.by_components:
         return
     for touched_query in cache.by_components.pop(component, ()):
-        cache.queries.pop(touched_query, None)
+        _drop_cached_query(cache, touched_query)
 
 
 def _touch_tag(world: World, tag: object) -> None:
     """Drop cached queries if a tag change has invalidated them."""
-    cache = _query_caches.get(world)
-    if cache is None:
-        return
+    cache = _get_query_cache(world)
     if tag not in cache.by_tags:
         return
     for touched_query in cache.by_tags.pop(tag, ()):
-        cache.queries.pop(touched_query, None)
+        _drop_cached_query(cache, touched_query)
 
 
 def _touch_relations(world: World, relations: Iterable[_RelationQuery]) -> None:
     """Drop cached queries if a relation change has invalidated them."""
-    cache = _query_caches.get(world)
-    if cache is None:
-        return
+    cache = _get_query_cache(world)
     for relation in relations:
         if relation not in cache.by_relations:
             continue
         for touched_query in cache.by_relations.pop(relation, ()):
-            cache.queries.pop(touched_query, None)
+            _drop_cached_query(cache, touched_query)
 
 
 def _check_suspicious_tags(tags: Iterable[object], stacklevel: int = 2) -> None:
     """Warn for the common mistake of passing a string as the tags parameter."""
     if isinstance(tags, str):
         warnings.warn(
             "The tags parameter was given a str type."
@@ -87,46 +94,82 @@
             "\nAdd square brackets 'tags=[tag]' to check for a single string tag. (Recommended)"
             "\nOtherwise use 'tags=list(tags)' to suppress this warning.",
             RuntimeWarning,
             stacklevel=stacklevel + 1,
         )
 
 
+def _fetch_relation_table(world: World, relation: _RelationQuery) -> AbstractSet[Entity]:
+    """Get the entity table for this relation.
+
+    For simple cases where target/origin is `Entity | ...` this returns the set directly from the lookup table.
+
+    For advanced cases `WorldQuery` this returns the subset of entities following the query condition.
+    """
+    if len(relation) == 2:  # noqa: PLR2004
+        tag, target = relation  # type: ignore[misc] # https://github.com/python/mypy/issues/1178
+        if not isinstance(target, WorldQuery):
+            return world._relations_lookup.get((tag, target), frozenset())
+
+        world = target.world
+        return set().union(*(world._relations_lookup.get((tag, entity), ()) for entity in target))
+
+    origin, tag, target = relation  # type: ignore[misc] # https://github.com/python/mypy/issues/1178
+    if not isinstance(origin, WorldQuery):
+        return world._relations_lookup.get((origin, tag, target), frozenset())
+
+    world = origin.world
+    return set().union(*(world._relations_lookup.get((entity, tag, None), ()) for entity in origin))
+
+
 def _fetch_lookup_tables(
     world: World,
     components: frozenset[_ComponentKey[object]],
     tags: frozenset[object],
     relations: frozenset[_RelationQuery],
 ) -> Iterator[AbstractSet[Entity]]:
     """Iterate over the relevant sets for this world and query."""
     for component in components:
         yield world._components_by_type.get(component, {}).keys()
     for tag in tags:
         yield world._tags_by_key.get(tag, set())
     for relation in relations:
-        yield world._relations_lookup.get(relation, set())
+        yield _fetch_relation_table(world, relation)
 
 
-def _add_query_to_cache(world: World, query: Query, entities: set[Entity]) -> None:
-    """Adds a query."""
+def _get_query_cache(world: World) -> _QueryCache:
+    """Return the global cache for the given world, creating it if it does not exist."""
     cache = _query_caches.get(world)
     if cache is None:
         cache = _query_caches[world] = _QueryCache()
+    return cache
+
+
+def _add_query_to_cache(w_query: WorldQuery, entities: set[Entity]) -> None:
+    """Adds a query."""
+    world = w_query.world
+    query = w_query._query
+    cache = _get_query_cache(world)
 
     cache.queries[query] = entities
     for component in itertools.chain(query._all_of_components, query._none_of_components):
         cache.by_components[component].add(query)
     for tag in itertools.chain(query._all_of_tags, query._none_of_tags):
         cache.by_tags[tag].add(query)
     for relation in itertools.chain(query._all_of_relations, query._none_of_relations):
         cache.by_relations[relation].add(query)
 
+    for depends in query._iter_dependencies():
+        _get_query_cache(depends.world).dependencies[depends._query].add((world, query))
+
 
-def _collect_query(world: World, query: Query) -> set[Entity]:
+def _collect_query(w_query: WorldQuery) -> set[Entity]:
     """Return the entities matching the given query."""
+    world = w_query.world
+    query = w_query._query
     requires = sorted(  # Place the smallest sets first to speed up intersections
         _fetch_lookup_tables(world, query._all_of_components, query._all_of_tags, query._all_of_relations), key=len
     )
     excludes = list(
         _fetch_lookup_tables(world, query._none_of_components, query._none_of_tags, query._none_of_relations)
     )
 
@@ -141,37 +184,45 @@
     for require in requires[1:]:
         entities.intersection_update(require)
     for exclude in excludes:
         entities.difference_update(exclude)
     return entities
 
 
-def _get_query(world: World, query: Query) -> set[Entity]:
+def _get_query(w_query: WorldQuery) -> set[Entity]:
     """Return the entities for the given query and world."""
-    cache = _query_caches.get(world)
+    world = w_query.world
+    query = w_query._query
+    assert query == query._normalized(), "Double checks that relations are correct"
+    cache = _get_query_cache(world)
     if cache is not None:
         cached_entities = cache.queries.get(query)
         if cached_entities is not None:
             return cached_entities  # Found a cached query
     # Not in cache, build the cache and return the results
 
-    cache = _query_caches.get(world)
-    if cache is None:
-        cache = _query_caches[world] = _QueryCache()
+    entities = _collect_query(w_query)
+    _add_query_to_cache(w_query, entities)
+    return entities
 
-    cache.queries[query] = entities = _collect_query(world, query)
 
-    for component in itertools.chain(query._all_of_components, query._none_of_components):
-        cache.by_components[component].add(query)
-    for tag in itertools.chain(query._all_of_tags, query._none_of_tags):
-        cache.by_tags[tag].add(query)
-    for relation in itertools.chain(query._all_of_relations, query._none_of_relations):
-        cache.by_relations[relation].add(query)
+def _normalize_query_relation(relation: _RelationQuery) -> _RelationQuery:
+    """Normalize a relation query.
 
-    return entities
+    This adds the inverse lookup to the sub-query so that this only matches entities which have a relation.
+    """
+    if len(relation) == 2:  # noqa: PLR2004
+        tag, targets = relation  # type: ignore[misc] # https://github.com/python/mypy/issues/1178
+        if isinstance(targets, WorldQuery):  # (tag, targets)
+            return tag, targets.all_of(relations=[(..., tag, None)])
+        return relation
+    origin, tag, _ = relation  # type: ignore[misc] # https://github.com/python/mypy/issues/1178
+    if isinstance(origin, WorldQuery):  # (origins, tag, None)
+        return origin.all_of(relations=[(tag, ...)]), tag, None
+    return relation
 
 
 @attrs.define(frozen=True)
 class Query:
     """A set of conditions used to lookup entities in a World."""
 
     _all_of_components: frozenset[_ComponentKey[object]] = frozenset()
@@ -198,15 +249,15 @@
         """Filter entities based on having all of the provided elements."""
         _check_suspicious_tags(tags, stacklevel=_stacklevel + 1)
         return self.__class__(
             self._all_of_components.union(components),
             self._none_of_components,
             self._all_of_tags.union(tags),
             self._none_of_tags,
-            self._all_of_relations.union(relations),
+            self._all_of_relations.union(_normalize_query_relation(relation) for relation in relations),
             self._none_of_relations,
         )
 
     def none_of(
         self,
         components: Iterable[_ComponentKey[object]] = (),
         *,
@@ -218,50 +269,71 @@
         _check_suspicious_tags(tags, stacklevel=_stacklevel + 1)
         return self.__class__(
             self._all_of_components,
             self._none_of_components.union(components),
             self._all_of_tags,
             self._none_of_tags.union(tags),
             self._all_of_relations,
-            self._none_of_relations.union(relations),
+            self._none_of_relations.union(_normalize_query_relation(relation) for relation in relations),
+        )
+
+    def _iter_dependencies(self) -> Iterator[WorldQuery]:
+        """Extract WorldQuery's from relations."""
+        for relation in itertools.chain(self._all_of_relations, self._none_of_relations):
+            if len(relation) == 2:  # noqa: PLR2004
+                if isinstance(relation[1], WorldQuery):  # (tag, targets)
+                    yield relation[1]
+            elif isinstance(relation[0], WorldQuery):  # (origins, tag, None)
+                yield relation[0]
+
+    def _normalized(self) -> Query:
+        """Return a Query with relations normalized."""
+        return self.__class__(
+            self._all_of_components,
+            self._none_of_components,
+            self._all_of_tags,
+            self._none_of_tags,
+            frozenset(_normalize_query_relation(relation) for relation in self._all_of_relations),
+            frozenset(_normalize_query_relation(relation) for relation in self._none_of_relations),
         )
 
 
+@attrs.define(frozen=True)
 class WorldQuery:
     """Collect a set of entities with the provided conditions."""
 
-    def __init__(self, world: World) -> None:
-        """Initialize a Query."""
-        self.world: Final = world
-        self._query = Query()
+    world: World
+    _query: Query = attrs.field(factory=Query)
 
     def _get_entities(self, extra_components: AbstractSet[_ComponentKey[object]] = frozenset()) -> set[Entity]:
-        return _get_query(self.world, self._query.all_of(components=extra_components))
+        return _get_query(self.all_of(components=extra_components))
 
     def all_of(
         self,
         components: Iterable[_ComponentKey[object]] = (),
         *,
         tags: Iterable[object] = (),
         relations: Iterable[_RelationQuery] = (),
     ) -> Self:
         """Filter entities based on having all of the provided elements."""
-        self._query = self._query.all_of(components=components, tags=tags, relations=relations, _stacklevel=2)
-        return self
+        return self.__class__(
+            self.world, self._query.all_of(components=components, tags=tags, relations=relations, _stacklevel=2)
+        )
 
     def none_of(
         self,
         components: Iterable[_ComponentKey[object]] = (),
         *,
         tags: Iterable[object] = (),
         relations: Iterable[_RelationQuery] = (),
     ) -> Self:
         """Filter entities based on having none of the provided elements."""
-        self._query = self._query.none_of(components=components, tags=tags, relations=relations, _stacklevel=2)
-        return self
+        return self.__class__(
+            self.world, self._query.none_of(components=components, tags=tags, relations=relations, _stacklevel=2)
+        )
 
     def __iter__(self) -> Iterator[Entity]:
         """Iterate over the matching entities."""
         return iter(self._get_entities())
 
     @overload
     def __getitem__(self, key: tuple[_ComponentKey[_T1]]) -> Iterable[tuple[_T1]]:
```

### Comparing `tcod_ecs-4.0.0/tcod/ecs/typing.py` & `tcod_ecs-4.1.0/tcod/ecs/typing.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,31 +5,36 @@
 import types
 from typing import TYPE_CHECKING, Any, Tuple, Type, TypeVar, Union
 
 from typing_extensions import TypeAlias
 
 if TYPE_CHECKING:
     from tcod.ecs.entity import Entity
+    from tcod.ecs.query import WorldQuery
 else:
     Entity = Any
+    WorldQuery = Any
 
 if sys.version_info >= (3, 10):  # pragma: no cover
     EllipsisType: TypeAlias = types.EllipsisType
 else:  # pragma: no cover
     EllipsisType = Any
 
 T = TypeVar("T")
 
 _ComponentKey: TypeAlias = Union[Type[T], Tuple[object, Type[T]]]
 """ComponentKey is plain `type` or tuple `(tag, type)`."""
 
-_RelationTarget: TypeAlias = Union[Entity, EllipsisType]
+_RelationTargetLookup: TypeAlias = Union[Entity, EllipsisType]
+"""Possible target for stored relations."""
+
+_RelationQueryTarget: TypeAlias = Union[_RelationTargetLookup, WorldQuery]
 """Possible target for relation queries."""
 
-_RelationQuery: TypeAlias = Union[Tuple[object, _RelationTarget], Tuple[_RelationTarget, object, None]]
+_RelationQuery: TypeAlias = Union[Tuple[object, _RelationQueryTarget], Tuple[_RelationQueryTarget, object, None]]
 """Query format for relations.
 
 One of 4 formats:
 
 * (tag, target)
 * (tag, ...)
 * (origin, tag, None)
```

### Comparing `tcod_ecs-4.0.0/tcod/ecs/world.py` & `tcod_ecs-4.1.0/tcod/ecs/world.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, DefaultDict, Dict, Iterable, Mapping, Set, TypeVar
 
 import attrs
 
 import tcod.ecs._converter
 import tcod.ecs.query
 from tcod.ecs.entity import Entity
-from tcod.ecs.typing import EllipsisType, _ComponentKey
+from tcod.ecs.typing import _ComponentKey, _RelationTargetLookup
 
 _T1 = TypeVar("_T1")
 _T2 = TypeVar("_T2")
 _T3 = TypeVar("_T3")
 
 
 def _defaultdict_of_set() -> defaultdict[_T1, set[_T2]]:
@@ -46,18 +46,18 @@
             tags_by_key[tag].add(entity)
     return tags_by_key
 
 
 def _relations_lookup_from(
     tags_by_entity: defaultdict[Entity, defaultdict[object, set[Entity]]],
     components_by_entity: defaultdict[Entity, defaultdict[_ComponentKey[object], dict[Entity, Any]]],
-) -> defaultdict[tuple[Any, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None], set[Entity]]:
+) -> defaultdict[tuple[Any, _RelationTargetLookup] | tuple[_RelationTargetLookup, Any, None], set[Entity]]:
     """Return the relation lookup table from the relations sparse-sets."""
     relations_lookup: defaultdict[
-        tuple[Any, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None], set[Entity]
+        tuple[Any, _RelationTargetLookup] | tuple[_RelationTargetLookup, Any, None], set[Entity]
     ] = defaultdict(set)
     for entity, tags in tags_by_entity.items():
         for tag, targets in tags.items():
             for target in targets:
                 relations_lookup[(tag, ...)].add(target)
                 relations_lookup[(tag, entity)].add(target)
                 relations_lookup[(target, tag, None)].add(entity)
@@ -114,15 +114,15 @@
         Entity, defaultdict[_ComponentKey[object], dict[Entity, Any]]
     ] = attrs.field(init=False, factory=lambda: defaultdict(_defaultdict_of_dict))
     """Random access relations owning components.
 
     dict[entity][ComponentKey][target_entity] = component
     """
     _relations_lookup: defaultdict[
-        tuple[Any, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None], set[Entity]
+        tuple[Any, _RelationTargetLookup] | tuple[_RelationTargetLookup, Any, None], set[Entity]
     ] = attrs.field(init=False, factory=lambda: defaultdict(set))
     """Relations query table.  Tags and components are mixed together.
 
     ```
     Tag:
         dict[(tag, this_entity)] = {target_entities_for_entity}
         dict[(tag, None)] = {target_entities_for_tag}
```

### Comparing `tcod_ecs-4.0.0/PKG-INFO` & `tcod_ecs-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 4.0.0
+Version: 4.1.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -28,14 +28,15 @@
 
 # About
 
 [![PyPI](https://img.shields.io/pypi/v/tcod-ecs)](https://pypi.org/project/tcod-ecs/)
 [![PyPI - License](https://img.shields.io/pypi/l/tcod-ecs)](https://github.com/HexDecimal/python-tcod-ecs/blob/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/python-tcod-ecs/badge/?version=latest)](https://python-tcod-ecs.readthedocs.io)
 [![codecov](https://codecov.io/gh/HexDecimal/python-tcod-ecs/branch/main/graph/badge.svg?token=4Ak5QpTLZB)](https://codecov.io/gh/HexDecimal/python-tcod-ecs)
+[![CommitsSinceLastRelease](https://img.shields.io/github/commits-since/HexDecimal/python-tcod-ecs/latest)](https://github.com/HexDecimal/python-tcod-ecs/blob/main/CHANGELOG.md)
 
 `tcod-ecs` is a [Sparse-set](https://skypjack.github.io/2020-08-02-ecs-baf-part-9/) [Entity-component-system](https://en.wikipedia.org/wiki/Entity_component_system) implemented using Python's `dict` and `set` types.
 See the [ECS FAQ](https://github.com/SanderMertens/ecs-faq) for more info.
 
 This implementation focuses on type-hinting, organization, and is designed to work well with Python.
 The following features are currently implemented:
 
@@ -270,11 +271,13 @@
 
 You can use the following table to help with constructing relation queries.
 `tag` is a component key if you are querying for a component relation.
 
 | Includes                                                              | Syntax |
 | --------------------------------------------------------------------- | :----: |
 | Entities with a relation tag to the given target                      | `(tag, target_entity)` |
-| Entities with a relation tag to any target                            | `(tag, ...)` |
-| Entities which are a relation target of a given entity                | `(origin_entity, tag, None)` |
-| Entities which are a target of any entity with the given relation tag | `(..., tag, None)` |
+| Entities with a relation tag to any target                            | `(tag, ...)` (Literal dot-dot-dot) |
+| Entities with a relation tag to the targets in the given query        | `(tag, world.Q.all_of(...))` |
+| The target entities of a relation of a given entity                   | `(origin_entity, tag, None)` |
+| The target entities of any entity with the given relation tag         | `(..., tag, None)` (Literal dot-dot-dot) |
+| The target entities of the queried entities with the given relation   | `(tag, world.Q.all_of(...))` |
```

