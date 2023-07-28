# Comparing `tmp/aio_overpass-0.3.0.tar.gz` & `tmp/aio_overpass-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_overpass-0.3.0.tar", max compression
+gzip compressed data, was "aio_overpass-0.4.0.tar", max compression
```

## Comparing `aio_overpass-0.3.0.tar` & `aio_overpass-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2105 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/LICENSE
--rw-r--r--   0        0        0    10286 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/README.md
--rwxr-xr-x   0        0        0      316 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/__init__.py
--rw-r--r--   0        0        0      977 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/_dist.py
--rwxr-xr-x   0        0        0      971 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/_ql.py
--rwxr-xr-x   0        0        0    12078 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/client.py
--rwxr-xr-x   0        0        0    28972 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/element.py
--rwxr-xr-x   0        0        0    14070 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/error.py
--rwxr-xr-x   0        0        0    25082 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/pt.py
--rwxr-xr-x   0        0        0    22661 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/pt_ordered.py
--rwxr-xr-x   0        0        0    14918 2023-06-29 13:54:31.082120 aio_overpass-0.3.0/aio_overpass/query.py
--rwxr-xr-x   0        0        0     3398 2023-06-29 13:54:31.106119 aio_overpass-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    11866 1970-01-01 00:00:00.000000 aio_overpass-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2718 2023-07-28 14:47:53.185142 aio_overpass-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-07-28 14:47:53.185142 aio_overpass-0.4.0/LICENSE
+-rw-r--r--   0        0        0    10395 2023-07-28 14:47:53.185142 aio_overpass-0.4.0/README.md
+-rwxr-xr-x   0        0        0      316 2023-07-28 14:47:53.185142 aio_overpass-0.4.0/aio_overpass/__init__.py
+-rw-r--r--   0        0        0      977 2023-07-28 14:47:53.185142 aio_overpass-0.4.0/aio_overpass/_dist.py
+-rwxr-xr-x   0        0        0      971 2023-07-28 14:47:53.185142 aio_overpass-0.4.0/aio_overpass/_ql.py
+-rwxr-xr-x   0        0        0    12328 2023-07-28 14:47:53.189142 aio_overpass-0.4.0/aio_overpass/client.py
+-rwxr-xr-x   0        0        0    29046 2023-07-28 14:47:53.189142 aio_overpass-0.4.0/aio_overpass/element.py
+-rwxr-xr-x   0        0        0    14299 2023-07-28 14:47:53.189142 aio_overpass-0.4.0/aio_overpass/error.py
+-rwxr-xr-x   0        0        0    25454 2023-07-28 14:47:53.189142 aio_overpass-0.4.0/aio_overpass/pt.py
+-rwxr-xr-x   0        0        0    22854 2023-07-28 14:47:53.189142 aio_overpass-0.4.0/aio_overpass/pt_ordered.py
+-rwxr-xr-x   0        0        0    16767 2023-07-28 14:47:53.189142 aio_overpass-0.4.0/aio_overpass/query.py
+-rwxr-xr-x   0        0        0     3848 2023-07-28 14:47:53.209142 aio_overpass-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12146 1970-01-01 00:00:00.000000 aio_overpass-0.4.0/PKG-INFO
```

### Comparing `aio_overpass-0.3.0/CHANGELOG.md` & `aio_overpass-0.4.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
+<br>
+
+## [0.4.0] - 2023-07-28
+* Added missing docstrings
+* Slight updates to existing docstrings
+* Added optional `logger` argument to `Query`. All logging output of `aio-overpass`
+  is fed into this logger by the `Client` and query runner
+* Added and updated log messages in the client and default query runner
+* Removed `cache_dir` argument from `DefaultQueryRunner`, which now caches
+  in `tempfile.TemporaryDirectory()`
+* Added optional `cache_ttl_secs` argument to `DefaultQueryRunner`, which limits
+  the time a query is cached for
+
+<br>
+
 ## [0.3.0] - 2023-06-29
 * Drop Python 3.8 support. The Python versions supported by this release are 3.9-3.11.
 * Relaxed `networkx` dependency to `>=2.7` according to [SPEC 0]
 * Increased `joblib` dependency to `~1.3`, which makes it ready for Python 3.12 among other things
 * Fixed doc: `maxsize` is not megabytes, but mebibytes
 * `Query`: affected properties ending in `_mb` now end in `_mib`
 * Add a section on coordinates to the `README`
@@ -41,9 +56,10 @@
 * Fix wrong repository link in `pyproject.toml`
 
 [0.1.1]: https://github.com/timwie/aio-overpass/releases/tag/v0.1.1
 [0.1.2]: https://github.com/timwie/aio-overpass/releases/tag/v0.1.2
 [0.1.2.post1]: https://github.com/timwie/aio-overpass/releases/tag/v0.1.2.post1
 [0.2.0]: https://github.com/timwie/aio-overpass/releases/tag/v0.2.0
 [0.3.0]: https://github.com/timwie/aio-overpass/releases/tag/v0.3.0
+[0.4.0]: https://github.com/timwie/aio-overpass/releases/tag/v0.4.0
 
 [SPEC 0]: https://scientific-python.org/specs/spec-0000/
```

### Comparing `aio_overpass-0.3.0/LICENSE` & `aio_overpass-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.3.0/README.md` & `aio_overpass-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <h1 align="center">
 aio-overpass
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/timwie/aio-overpass/test_and_publish.yml)](https://github.com/timwie/aio-overpass/actions/workflows/test_and_publish.yml)
 [![codecov](https://codecov.io/gh/timwie/aio-overpass/branch/main/graph/badge.svg?token=YX1218U740)](https://codecov.io/gh/timwie/aio-overpass)
 [![PyPI version](https://badge.fury.io/py/aio_overpass.svg)](https://badge.fury.io/py/aio_overpass)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aio-overpass)
+[![API reference](https://img.shields.io/badge/API%20reference-555555)](http://www.timwie.dev/aio-overpass/)
 </h1>
 
 A client for the [Overpass API], a read-only API that serves up custom selected
 parts of [OpenStreetMap] data. It is optimized for data consumers that need a few
 elements within a glimpse or up to roughly 10 million elements in some minutes,
 both selected by search criteria like location, type of objects, tag properties,
 proximity, or combinations of them. To make use of it, you should familiarize yourself
```

### Comparing `aio_overpass-0.3.0/aio_overpass/_dist.py` & `aio_overpass-0.4.0/aio_overpass/_dist.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.3.0/aio_overpass/_ql.py` & `aio_overpass-0.4.0/aio_overpass/_ql.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.3.0/aio_overpass/client.py` & `aio_overpass-0.4.0/aio_overpass/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Interface for making API calls."""
 
 import asyncio
 import logging
 import re
 import sys
+from contextlib import suppress
 from dataclasses import dataclass
 from typing import Optional
 from urllib.parse import urljoin
 
 from aio_overpass import __version__
 from aio_overpass.error import (
     CallError,
@@ -94,15 +95,16 @@
         self,
         url: str = DEFAULT_INSTANCE,
         user_agent: str = DEFAULT_USER_AGENT,
         concurrency: int = 32,
         runner: Optional[QueryRunner] = None,
     ) -> None:
         if concurrency <= 0:
-            raise ValueError("'concurrency' must be > 0")
+            msg = "'concurrency' must be > 0"
+            raise ValueError(msg)
 
         self._url = url
         self._user_agent = user_agent
         self._concurrency = concurrency
         self._runner = runner or DefaultQueryRunner()
 
         self._maybe_session: Optional[aiohttp.ClientSession] = None
@@ -131,23 +133,21 @@
         self._maybe_sem = asyncio.BoundedSemaphore(status.concurrency)
 
         return self._maybe_sem
 
     async def close(self) -> None:
         """Cancel all running queries and close the underlying session."""
         if self._maybe_session and not self._maybe_session.closed:
-            try:
+            # do not care if this fails
+            with suppress(CallError):
                 _ = await self.cancel_queries()
-            except CallError:
-                pass  # do not care if this fails
 
-            try:
+            # is raised when there are still active queries. that's ok
+            with suppress(aiohttp.ServerDisconnectedError):
                 await self._maybe_session.close()
-            except aiohttp.ServerDisconnectedError:
-                pass  # is raised when there are still active queries. that's ok
 
     async def _status(self, session: aiohttp.ClientSession, **kwargs) -> "Status":
         try:
             async with session.get(url=urljoin(self._url, "status"), **kwargs) as response:
                 text = await response.text()
         except aiohttp.ClientError as err:
             raise _to_client_error(err) from err
@@ -253,20 +253,21 @@
                 return
             await self._run_query_once(query)
 
     async def _invoke_runner(self, query: Query) -> None:
         try:
             await self._runner(query)
         except ClientError:
-            _logger.info("query runner raised; stop retrying")
             raise
         except BaseException as err:
             raise RunnerError(err) from err
 
     async def _run_query_once(self, query: Query) -> None:
+        logger = query.logger or logging.getLogger(f"{type(self).__module__}.{type(self).__name__}")
+
         if query.done:
             return
 
         loop = asyncio.get_event_loop()
 
         if query._time_start <= 0:
             query._time_start = loop.time()
@@ -285,25 +286,31 @@
                 # 'query.error' will be overwritten, which means we will not check for a
                 # cooldown in the next iteration.
                 status = await self._status(session=session, timeout=_next_timeout(query))
 
                 if (timeout := _next_timeout_secs(query)) and status.cooldown_secs > timeout:
                     raise _giveup_error(query, loop)
 
+                logger.info(f"{query} has cooldown for {status.cooldown_secs:.1f}s")
                 await asyncio.sleep(status.cooldown_secs)
 
             # Limit the concurrent query requests to the number of slots available.
+            if rate_limiter.locked():
+                logger.info(f"{query} has to wait for a slot")
+
             await asyncio.wait_for(
                 fut=rate_limiter.acquire(),
                 timeout=_next_timeout(query).total,
             )
 
             try:
                 query._time_start_try = loop.time()
 
+                logger.info(f"call api for {query}")
+
                 async with session.get(
                     url=urljoin(self._url, "interpreter"),
                     params={"data": query.code},
                     timeout=_next_timeout(query),
                 ) as response:
                     query._time_end_try = loop.time()
                     query._result_set = await _result_or_raise(response, query.kwargs)
@@ -331,10 +338,7 @@
 
 def _next_timeout(query: Query) -> aiohttp.ClientTimeout:
     return aiohttp.ClientTimeout(total=_next_timeout_secs(query))
 
 
 def _giveup_error(query: Query, loop: asyncio.AbstractEventLoop) -> GiveupError:
     return GiveupError(kwargs=query.kwargs, after_secs=loop.time() - query._time_start)
-
-
-_logger = logging.getLogger("aio-overpass")
```

### Comparing `aio_overpass-0.3.0/aio_overpass/element.py` & `aio_overpass-0.4.0/aio_overpass/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 A dictionary representing a JSON object returned by the Overpass API.
 """
 
 Bbox = tuple[float, float, float, float]
 """
 The bounding box of a spatial object.
 
-This tuple can be understood as any of 
+This tuple can be understood as any of
     - ``(s, w, n, e)``
     - ``(minlat, minlon, maxlat, maxlon)``
     - ``(minx, miny, maxx, maxy)``
 """
 
 
 class Spatial(ABC):
@@ -92,15 +92,15 @@
             - https://osmdata.openstreetmap.de/info/projections.html
             - https://tools.ietf.org/html/rfc7946#section-4
         """
         raise NotImplementedError
 
     @property
     def __geo_interface__(self) -> GeoJsonDict:
-        """See ``geojson``"""
+        """See ``geojson``."""
         return self.geojson
 
 
 @dataclass(repr=False)
 class Metadata:
     """
     Metadata concerning the most recent edit of an OSM element.
@@ -119,16 +119,17 @@
     user_name: str
     user_id: int
 
 
 @dataclass(repr=False, eq=False)
 class Element(Spatial):
     """
-    Elements are the basic components of OpenStreetMap's data,
-    and the typical members in the result set of an Overpass API query.
+    Elements are the basic components of OpenStreetMap's data.
+
+    A query's result set is made up of these elements.
 
     Objects of this class do not necessarily describe OSM elements in their entirety.
     The degrees of detail are decided by the ``out`` statements used in an Overpass query:
     using ``out ids`` f.e. would only include an element's ID, but not its tags, geometry, etc.
 
     Element geometries have coordinates in the EPSG:4326 coordinate reference system,
     meaning that the coordinates are (latitude, longitude) tuples on the WGS 84 reference ellipsoid.
@@ -195,20 +196,22 @@
             return "way"
         if isinstance(self, Relation):
             return "relation"
         raise ValueError()
 
     @property
     def link(self) -> str:
-        """This element on openstreetmap.org"""
+        """This element on openstreetmap.org."""
         return f"https://www.openstreetmap.org/{self.type}/{self.id}"
 
     @property
     def geojson(self) -> GeoJsonDict:
         """
+        A mapping of this object, using the GeoJSON format.
+
         Objects are mapped as the following:
          - ``Node`` -> ``Feature`` with optional ``Point`` geometry
          - ``Way`` -> ``Feature`` with optional ``LineString`` geometry
          - ``AreaWay`` -> ``Feature`` with optional ``Polygon`` geometry
          - ``AreaRelation`` -> ``Feature`` with optional ``Polygon`` or ``MultiPolygon`` geometry
          - ``Relation`` -> ``FeatureCollection`` (nested ``Relations`` are mapped to unlocated
            ``Features``)
@@ -350,16 +353,17 @@
     node_ids: Optional[list[int]]
     geometry: Union[LineString, LinearRing, None]
 
 
 @dataclass(repr=False, eq=False)
 class Relation(Element):
     """
-    A relation is a group of nodes and ways that have a logical or geographic relationship,
-    which is described through its tags.
+    A relation is a group of nodes and ways that have a logical or geographic relationship.
+
+    This relationship is described through its tags.
 
     For relations that describe an area, refer to the ``AreaRelation`` class.
 
     Attributes:
         members: Ordered member elements of this relation, with an optional role
 
     References:
@@ -518,15 +522,16 @@
 
     Raises:
         ValueError: If the input query is unfinished/has no result set.
         KeyError: The only times there should be missing keys is when either using ``out noids``,
                   or when building derived elements that are missing common keys.
     """
     if not query.done:
-        raise ValueError("query has no result set")
+        msg = "query has no result set"
+        raise ValueError(msg)
 
     collector = _ElementCollector()
     _collect_untyped(query, collector)
     _collect_typed(collector)
     _collect_relationships(collector)
     return collector.list
 
@@ -644,15 +649,16 @@
           Relation members that are not ways, or are not part of any polygon boundary, are
           not part of the result geometry.
 
     Raises:
         ValueError: if element is not of type 'node', 'way', 'relation', or 'area'
     """
     if raw_elem.get("type") not in _KNOWN_ELEMENTS:
-        raise ValueError("expected element of type 'node', 'way', 'relation', or 'area'")
+        msg = "expected element of type 'node', 'way', 'relation', or 'area'"
+        raise ValueError(msg)
 
     if raw_elem["type"] == "node":
         lat, lon = raw_elem.get("lat"), raw_elem.get("lon")
         if lat and lon:
             return Point(lat, lon)
 
     if raw_elem["type"] == "way":
@@ -693,32 +699,29 @@
     return None
 
 
 def _line(way: OverpassDict) -> Union[LineString, LinearRing, None]:
     """Returns the geometry of a way in the result set."""
     if "geometry" not in way or len(way["geometry"]) < 2:
         return None
-    if way["geometry"][0] == way["geometry"][-1]:
-        cls = LinearRing
-    else:
-        cls = LineString
+    is_ring = way["geometry"][0] == way["geometry"][-1]
+    cls = LinearRing if is_ring else LineString
     return cls((c["lat"], c["lon"]) for c in way["geometry"])
 
 
 def _flatten(obj: BaseGeometry) -> Iterable[BaseGeometry]:
     """Recursively flattens multipart geometries."""
     if isinstance(obj, BaseMultipartGeometry):
         return (nested for contained in obj.geoms for nested in _flatten(contained))
     return (obj,)
 
 
 def _is_area_element(el: OverpassDict) -> bool:
     """
-    Decide if the given element likely represents an area,
-    and should be viewed as a (multi-)polygon.
+    Decide if ``el`` likely represents an area, and should be viewed as a (multi-)polygon.
 
     Args:
         el: a way or relation from a query's result set
 
     Returns:
         ``False`` if the input is not a relation or closed way.
         ``False``, unless there are tags which indicate that the way represents an area.
```

### Comparing `aio_overpass-0.3.0/aio_overpass/error.py` & `aio_overpass-0.4.0/aio_overpass/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,24 +93,32 @@
 class ResponseError(ClientError):
     """
     Unexpected API response.
 
     This error is raised when a request fails, but we can't specifically say why.
     This may indicate a bug on our end, since the client is meant to process almost any
     response of an Overpass API instance.
+
+    Attributes:
+        request_info: Contains information about request.
+        history: History from failed response.
+        status: HTTP status code of response, e.g. ``400``.
+        message: Message of response, e.g. ``"OK"``.
+        headers: Headers in response, a list of pairs.
     """
 
     request_info: aiohttp.RequestInfo
     history: tuple[aiohttp.ClientResponse, ...]
     status: int
     message: str
     headers: Optional[aiohttp.typedefs.LooseHeaders]
 
     @property
     def response(self) -> aiohttp.ClientResponse:
+        """Client response returned by ``aiohttp.ClientSession.request()`` and family."""
         return self.history[-1]
 
     def __str__(self) -> str:
         return (
             f"unexpected response: {self.status}, {self.message!r}, {self.request_info.real_url!r}"
         )
 
@@ -127,19 +135,15 @@
         after_secs: the total time spent on the query
     """
 
     kwargs: dict
     after_secs: float
 
     def __str__(self) -> str:
-        if self.kwargs:
-            query = f"query {self.kwargs}"
-        else:
-            query = "query <no kwargs>"
-
+        query = f"query {self.kwargs}" if self.kwargs else "query <no kwargs>"
         return f"gave up on {query} after {self.after_secs:.01f} seconds"
 
 
 @dataclass
 class QueryError(ClientError):
     """
     Base exception for queries that failed at the Overpass API server.
@@ -149,26 +153,17 @@
         remarks: the error remarks provided by the API
     """
 
     kwargs: dict
     remarks: list[str]
 
     def __str__(self) -> str:
-        if self.kwargs:
-            query = f"query {self.kwargs}"
-        else:
-            query = "query <no kwargs>"
-
+        query = f"query {self.kwargs}" if self.kwargs else "query <no kwargs>"
         first = f"'{self.remarks[0]}'"
-
-        if len(self.remarks) > 1:
-            rest = f" (+{len(self.remarks) - 1} more)"
-        else:
-            rest = ""
-
+        rest = f" (+{len(self.remarks) - 1} more)" if len(self.remarks) > 1 else ""
         return f"{query} failed: {first}{rest}"
 
 
 @dataclass
 class QueryResponseError(ResponseError, QueryError):
     """
     Unexpected query response.
@@ -187,22 +182,20 @@
     Indicates the query's QL code is not valid.
 
     Retrying is pointless when encountering this error.
     """
 
 
 class QueryRejectCause(Enum):
-    """
-    Details why a query was rejected or cancelled by an API server.
-    """
+    """Details why a query was rejected or cancelled by an API server."""
 
     TOO_BUSY = auto()
     """
     Gateway rejection. The server has already so much load that the request cannot be executed.
-    
+
     Smaller ``[timeout:*]`` and/or ``[maxsize:*]`` values might make the request acceptable.
     """
 
     TOO_MANY_QUERIES = auto()
     """
     Gateway rejection. There are no open slots for queries from your IP address.
 
@@ -211,24 +204,24 @@
     a rare error, assuming you are not making requests through another client.
     """
 
     EXCEEDED_TIMEOUT = auto()
     """
     Runtime rejection. The query has been (or surely will be) running longer than its proposed
     ``[timeout:*]``, and has been cancelled by the server.
-    
+
     A higher ``[timeout:*]`` value might allow the query run to completion, but also makes it
     more likely to be rejected by a server under heavy load, before executing it (see ``TOO_BUSY``).
     """
 
     EXCEEDED_MAXSIZE = auto()
     """
     Runtime rejection. The memory required to execute the query has (or surely will) exceed
     its proposed ``[maxsize:*]``, and has been cancelled by the server.
-    
+
     A higher ``[maxsize:*]`` value might allow the query run to completion, but also makes it
     more likely to be rejected by a server under heavy load, before executing it (see ``TOO_BUSY``).
     """
 
     def __str__(self) -> str:
         if self == QueryRejectCause.TOO_BUSY:
             return "server too busy"
```

### Comparing `aio_overpass-0.3.0/aio_overpass/pt.py` & `aio_overpass-0.4.0/aio_overpass/pt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Classes and queries specialized on public transportation routes.
-"""
+"""Classes and queries specialized on public transportation routes."""
 
 from collections import Counter
 from collections.abc import Generator
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import Any, Optional, Union, cast
 
@@ -164,18 +162,20 @@
 
     ENTRY_AND_EXIT = auto()
     ENTRY_ONLY = auto()
     EXIT_ONLY = auto()
 
     @property
     def entry_possible(self) -> bool:
+        """``True`` if you can enter at this stop on the route."""
         return self != Connection.EXIT_ONLY
 
     @property
     def exit_possible(self) -> bool:
+        """``True`` if you can exit at this stop on the route."""
         return self != Connection.ENTRY_ONLY
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}.{self.name}"
 
 
 @dataclass
@@ -245,14 +245,15 @@
             if relship_to_route
             for relship_to_stop_area in relship_to_route.member.relations
             if relship_to_stop_area.relation.tag("public_transport") == "stop_area"
         }
 
     @property
     def geojson(self) -> GeoJsonDict:
+        """A mapping of this object, using the GeoJSON format."""
         # TODO Stop geojson
         raise NotImplementedError
 
     @property
     def _stop_point(self) -> Optional[Point]:
         """This is set if we have a point that is on the track of the route."""
         if isinstance(self.stop_coords, Node):
@@ -334,14 +335,15 @@
     ASSUME_V1 = auto()
     ASSUME_V2 = auto()
 
     OTHER = auto()
 
     @property
     def version_number(self) -> Optional[int]:
+        """Public transport tagging scheme."""
         if self in (RouteScheme.EXPLICIT_V1, RouteScheme.ASSUME_V1):
             return 1
         if self in (RouteScheme.EXPLICIT_V2, RouteScheme.ASSUME_V2):
             return 2
         return None
 
     def __repr__(self) -> str:
@@ -523,14 +525,15 @@
     def bounds(self) -> Optional[Bbox]:
         """The bounding box around all stops of this route."""
         geom = GeometryCollection([stop._geometry for stop in self.stops if stop._geometry])
         return geom.bounds or None
 
     @property
     def geojson(self) -> GeoJsonDict:
+        """A mapping of this object, using the GeoJSON format."""
         # TODO Route geojson
         raise NotImplementedError
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}(id={self.relation.id}, name='{self.name}')"
 
 
@@ -547,15 +550,15 @@
     "wheelchair",
 }
 """
 Tags that, by convention, can be applied to route masters instead of their routes,
 in order to avoid duplication.
 
 References:
-    - https://wiki.openstreetmap.org/wiki/Relation:route_master 
+    - https://wiki.openstreetmap.org/wiki/Relation:route_master
 """
 
 
 def collect_routes(query: RouteQuery, perimeter: Optional[Polygon] = None) -> list[Route]:
     # TODO the way 'perimeter' works might be confusing
     """
     Consumes the result set of a query and produces ``Route`` objects.
@@ -629,16 +632,17 @@
     )
 
     return RouteScheme.ASSUME_V1 if assume_v1 else RouteScheme.ASSUME_V2
 
 
 def _stops(route_relation: Relation) -> Generator[Stop, None, None]:
     """
-    Group route relation members so that each member belongs to the same stop along
-    the route. Typically, a stop is represented by a stop position or platform, or both.
+    Group route relation members so that each member belongs to the same stop along the route.
+
+    Typically, a stop is represented by a stop position or platform, or both.
     """
     idx = 0
 
     def to_stop(*selected: Relationship) -> Stop:
         nonlocal idx
         stop_idx = idx
         idx += 1
@@ -720,17 +724,15 @@
     if relship.member.type == "node" and relship.member.tag("public_transport"):
         return _RouteRole.STOP
 
     return _RouteRole.NONE
 
 
 def _share_stop_area(a: Relationship, b: Relationship) -> bool:
-    """
-    ``True`` if the given route members share least one common stop area.
-    """
+    """``True`` if the given route members share least one common stop area."""
     a_areas = {
         relship.relation.id
         for relship in a.member.relations
         if relship.relation.tag("public_transport") == "stop_area"
     }
     b_areas = {
         relship.relation.id
@@ -738,16 +740,19 @@
         if relship.relation.tag("public_transport") == "stop_area"
     }
     return not a_areas.isdisjoint(b_areas)
 
 
 def _connection_compatible(a: Connection, b: Connection) -> bool:
     """
-    ``False`` if one of the connections is entry-only, while the other is exit-only,
-    ``True`` otherwise.
+    Check whether two connections are compatible.
+
+    Returns:
+        ``False`` if one of the connections is entry-only, while the other is exit-only,
+        ``True`` otherwise.
     """
     if a == Connection.ENTRY_AND_EXIT or b == Connection.ENTRY_AND_EXIT:
         return True
 
     return a == b
```

### Comparing `aio_overpass-0.3.0/aio_overpass/pt_ordered.py` & `aio_overpass-0.4.0/aio_overpass/pt_ordered.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Collect the routes of a ``RouteQuery`` with optimized geometry.
-"""
+"""Collect the routes of a ``RouteQuery`` with optimized geometry."""
 
 import itertools
 from collections.abc import Generator
 from dataclasses import dataclass, replace
 from typing import Any, Callable, Optional, Union, cast
 
 from aio_overpass._dist import fast_distance
@@ -132,33 +130,35 @@
         return list(self._split(predicate=lambda a, b: b.path_idx > a.path_idx + 1))
 
     def stop_split(self) -> list["OrderedRouteView"]:
         """Split this view at every stop, returning views between every pair of stops."""
         return self._group_by(key=lambda node: node.path_idx)
 
     def take(self, first_n: int) -> "OrderedRouteView":
-        """
-        Returns the continuous view that connects a maximum number of stops at the beginning.
-        """
+        """Returns the continuous view that connects a maximum number of stops at the beginning."""
         if first_n < 2:
-            raise ValueError("cannot take less than two stops")
+            msg = "cannot take less than two stops"
+            raise ValueError(msg)
 
         pre_gap, *_ = self.gap_split()
 
         by_stop = itertools.groupby(pre_gap.ordering, key=lambda node: node.path_idx)
         by_stop_truncated = itertools.islice(by_stop, first_n - 1)
 
         ordering = [node for _, nodes in by_stop_truncated for node in nodes]
 
         return replace(self, ordering=ordering)
 
     def trim(self, distance: float) -> "OrderedRouteView":
         """
-        Returns the continuous view that is not longer than a given distance,
-        starting from the first stop.
+        Trim this view to some distance in meters.
+
+        Returns:
+            the continuous view that is not longer than a given distance,
+            starting from the first stop.
         """
         pre_gap, *_ = self.gap_split()
 
         distance_start = pre_gap.ordering[0].distance
 
         by_stop = itertools.groupby(pre_gap.ordering, key=lambda node: node.path_idx)
 
@@ -239,14 +239,15 @@
         if len(merged_lines) == 1:
             return merged_lines[0]
 
         return MultiLineString(merged_lines)
 
     @property
     def geojson(self) -> GeoJsonDict:
+        """A mapping of this object, using the GeoJSON format."""
         # TODO OrderedRouteView geojson
         raise NotImplementedError
 
 
 def collect_ordered_routes(
     query: RouteQuery, perimeter: Optional[Polygon] = None, n_jobs: int = 1
 ) -> list[OrderedRouteView]:
@@ -345,20 +346,22 @@
             seg.ordering = path
 
     return [*views, *views_empty]
 
 
 def _route_graph(rel: Relation) -> MultiDiGraph:
     """
-    Build a directed graph of a route's track where
-     - graph nodes will be a tuple of lat, lon
-     - graph nodes are every node of every way (stop positions can lie anywhere on the track)
-     - ways that are listed more than once in the relation have parallel edges
-     - inverse edges are added for each way, unless it is tagged as a oneway
-     - edges remain unweighted for now
+    Build a directed graph of a route's track.
+
+    In this graph…
+     - …nodes will be a tuple of lat, lon
+     - …nodes are every node of every way (stop positions can lie anywhere on the track)
+     - …ways that are listed more than once in the relation have parallel edges
+     - …inverse edges are added for each way, unless it is tagged as a oneway
+     - …edges remain unweighted for now
     """
     graph = MultiDiGraph()
 
     track = [relship for relship in rel.members if _is_track(relship)]
 
     for relship in track:
         way = cast(Way, relship.member)
@@ -412,25 +415,27 @@
     )
 
 
 def _find_stop_coords(
     stop: Stop, track_graph: MultiDiGraph, track_nodes: MultiPoint, track_ways: MultiLineString
 ) -> Union[Node, Point, None]:
     """
-    Find a node on the track that closesly represents the stop position:
-     - None if no appropriate node found
-     - Some Node if we found a stop position in either relation or a stop relation
-     - Some Point if we found a close node on the track, that is *probably* close to the
-       actual stop position
+    Find a node on the track that closesly represents the stop position.
 
     Args:
         stop: the stop to locate on the graph
         track_graph: the graph that represents the route's track
         track_nodes: a point for every node in the graph
         track_ways: a line string for every edge in the graph
+
+    Returns:
+     - None if no appropriate node found
+     - Some Node if we found a stop position in either relation or a stop relation
+     - Some Point if we found a close node on the track, that is *probably* close to the
+       actual stop position
     """
     # (a) check if the route relation has a stop_position for this stop
     if stop.stop_position:
         stop_node = cast(Node, stop.stop_position.member)
         if stop_node.geometry.coords[0] in track_graph:
             return stop_node
 
@@ -485,15 +490,14 @@
     Not every two stops can be connected, f.e. when they have no representative
     position on the route's track, or when that track has gaps.
 
     Args:
         route_graph: the unweighted, directed graph of the route's track
         targets: the stop positions to connect
     """
-
     # set edge weights to metric distance
     for u, v in route_graph.edges():
         if _WEIGHT_KEY in route_graph[u][v][0]:
             continue
 
         distance = fast_distance(*u, *v)  # meters
 
@@ -547,24 +551,24 @@
             path_nodes = nx.shortest_path(graph, source=u, target=v, weight=_WEIGHT_KEY)
             next_progress = _traverse_path(graph, progress, path_nodes)
             return _traverse_graph(graph, next_progress)
         except nx.NetworkXNoPath:
             pass
 
     next_progress = _Traversal(
-        ordering=progress.ordering
-        + [
+        ordering=[
+            *progress.ordering,
             OrderedRouteViewNode(
                 lon=u[1],
                 lat=u[0],
                 way_id=None,
                 path_idx=progress.path_idx,
                 n_seen_stops=len(progress.targets_visited),
                 distance=progress.distance,
-            )
+            ),
         ],
         targets_left=progress.targets_left[1:],
         targets_visited=progress.targets_visited + progress.targets_left[:1],
         distance=progress.distance,
         path_idx=progress.path_idx + 1,
     )
     return _traverse_graph(graph, next_progress)
@@ -579,15 +583,16 @@
     Repeated traversal of the edge (u, v) is discouraged by setting a large, arbitrary weight.
     Implicitly, this discourages repeated traversal of ways in a route relation. Since the path
     members are supposed to be ordered, ways that are repeatedly traversed should appear more than
     once in the relation. But since we cannot guarantee that, flat-out removal of these edges/ways
     would be too drastic.
     """
     if not path_nodes:
-        raise ValueError("expected non-empty list of nodes")
+        msg = "expected non-empty list of nodes"
+        raise ValueError(msg)
 
     edges = list(zip(path_nodes, path_nodes[1:]))
     n_seen_stops = len(progress.targets_visited)
     new_ordering = []
 
     for u, v in edges:
         # don't duplicate last visited stop position node
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aio_overpass-0.3.0/aio_overpass/query.py` & `aio_overpass-0.4.0/aio_overpass/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Query state and runner."""
 
 import asyncio
 import hashlib
 import json
 import logging
 import re
+import tempfile
+import time
 from pathlib import Path
 from typing import Optional, Protocol
 
 from aio_overpass.error import (
     ClientError,
     QueryLanguageError,
     QueryRejectCause,
@@ -43,22 +45,24 @@
 class Query:
     """
     State of a query that is either pending, successful, or failed.
 
     Args:
         input_code: The input Overpass QL code. Note that some settings might be changed
                     by query runners, notably the 'timeout' and 'maxsize' settings.
+        logger: The logger to use for all logging output related to this query.
         **kwargs: Additional keyword arguments that can be used to identify queries.
 
     References:
         - https://wiki.openstreetmap.org/wiki/Overpass_API/Overpass_QL
     """
 
-    def __init__(self, input_code: str, **kwargs) -> None:
+    def __init__(self, input_code: str, logger: Optional[logging.Logger] = None, **kwargs) -> None:
         self._input_code = input_code
+        self._logger = logger
         self._kwargs = kwargs
 
         self._settings = dict(_SETTING_PATTERN.findall(input_code))
 
         self._settings["out"] = "json"
 
         if "maxsize" not in self._settings:
@@ -77,16 +81,15 @@
         self._time_start = 0.0  # time prior to executing the first try
         self._time_start_try = 0.0  # time prior to executing the most recent try
         self._nb_tries = 0
 
     def _has_cooldown(self) -> bool:
         """When ``True``, we should query the API status to retrieve our cooldown period."""
         return (
-            self.error is not None
-            and isinstance(self.error, QueryRejectError)
+            isinstance(self.error, QueryRejectError)
             and self.error.cause == QueryRejectCause.TOO_MANY_QUERIES
         )
 
     def reset(self) -> None:
         """Reset the query to its initial state, ignoring previous tries."""
         Query.__init__(self, input_code=self._input_code, **self._kwargs)
 
@@ -101,14 +104,19 @@
         Keyword arguments that can be used to identify queries.
 
         The default query runner will log these values when a query is run.
         """
         return self._kwargs
 
     @property
+    def logger(self) -> Optional[logging.Logger]:
+        """If set, this is the logger used for logging output related to this query."""
+        return self._logger
+
+    @property
     def nb_tries(self) -> int:
         """Current number of tries."""
         return self._nb_tries
 
     @property
     def error(self) -> Optional[ClientError]:
         """
@@ -229,28 +237,25 @@
         the result is written to this query object. Although it depends on how busy
         the API instance is, this can give some indication of how long a query takes.
         """
         return max(0.0, self._time_end_try - self._time_start_try)
 
     @property
     def run_duration_secs(self) -> float:
-        """
-        The total required time for this query in seconds (so far).
-        """
-        if self._time_end_try > 0.0:
-            end = self._time_end_try
-        else:
-            end = asyncio.get_event_loop().time()
+        """The total required time for this query in seconds (so far)."""
+        end = self._time_end_try if self._time_end_try > 0.0 else asyncio.get_event_loop().time()
         return end - self._time_start
 
     @property
     def api_version(self) -> Optional[str]:
         """
-        The Overpass API version used by the queried instance,
-        f.e. ``Overpass API 0.7.56.8 7d656e78``.
+        The Overpass API version used by the queried instance.
+
+        Returns:
+            f.e. ``"Overpass API 0.7.56.8 7d656e78"``.
 
         References:
             - https://wiki.openstreetmap.org/wiki/Overpass_API/versions
         """
         if not self.result_set:
             return None
 
@@ -270,14 +275,16 @@
             return None
 
         return self.result_set["osm3s"]["timestamp_osm_base"]
 
     @property
     def timestamp_areas(self) -> Optional[str]:
         """
+        All area data edits that have been uploaded before this date are included.
+
         If the query involves area data processing, this is the date of the latest edit
         that has been considered in the most recent batch run of the area generation.
 
         The format is ``YYYY-MM-DDThh:mm:ssZ``.
         """
         if not self.result_set:
             return None
@@ -289,32 +296,30 @@
         """A copyright notice that comes with the result set."""
         if not self.result_set:
             return _COPYRIGHT
 
         return self.result_set["osm3s"].get("copyright") or _COPYRIGHT
 
     def __str__(self) -> str:
-        if self.kwargs:
-            query = f"query {self.kwargs}"
-        else:
-            query = "query <no kwargs>"
+        query = f"query {self.kwargs}" if self.kwargs else "query <no kwargs>"
 
         size = self.result_size_mib
         time_query = self.query_duration_secs
         time_total = self.run_duration_secs
 
         if self.nb_tries == 0:
             details = "pending"
         elif self.done:
             if self.nb_tries == 1:
                 details = f"{size}mb in {time_query:.01f}s"
             else:
                 details = f"{size}mb in {time_query:.01f} ({time_total:.01f})s"
         else:
-            details = f"failing after {self.nb_tries} tries, {time_total:.01f}s"
+            t = "try" if self.nb_tries == 1 else "tries"
+            details = f"failing after {self.nb_tries} {t}, {time_total:.01f}s"
 
         return f"{query} ({details})"
 
     def __repr__(self) -> str:
         cls_name = type(self).__name__
 
         details = {
@@ -340,120 +345,159 @@
         details_str = ", ".join((f"{k}={v!r}" for k, v in details.items()))
 
         return f"{cls_name}({details_str})"
 
 
 class QueryRunner(Protocol):
     """
-    A query runner is async function that is called before a client makes an API request.
+    A query runner is an async function that is called before a client makes an API request.
 
     Query runners can be used to
      - retry queries when they fail
      - modify queries, f.e. to lower/increase their maxsize/timeout
      - log query results & errors
      - implement caching
     """
 
     async def __call__(self, query: Query) -> None:
+        """Called with the current query state before the client makes an API request."""
         pass
 
 
 class DefaultQueryRunner(QueryRunner):
     """
-    A general query runner that
-        - retries with an increasing back-off period in between tries if the server is too busy
-        - retries and doubles timeout and maxsize settings if they were exceeded
-        - limits the number of tries
-        - caches query results (useful when debugging)
-
-    This runner does *not*
-        - limit the total time a query runs, including retries
-        - lower timeout and maxsize settings if the server rejected a query
+    The default query runner.
+
+    This runner…
+     - …retries with an increasing back-off period in between tries if the server is too busy
+     - …retries and doubles timeout and maxsize settings if they were exceeded
+     - …limits the number of tries
+     - …optionally caches query results in temp files
+
+    This runner does *not*…
+     - …limit the total time a query runs, including retries
+     - …lower timeout and maxsize settings if the server rejected a query
 
     Args:
         max_tries: The maximum number of times a query is tried. (5 by default)
-        cache_dir: If set, JSON result sets will be cached in this directory.
+        cache_ttl_secs: Amount of seconds a query's result set is cached for.
+                        Set to zero to disable caching. (zero by default)
     """
 
-    def __init__(self, max_tries: int = 5, cache_dir: Optional[Path] = None) -> None:
+    def __init__(self, max_tries: int = 5, cache_ttl_secs: int = 0) -> None:
+        if max_tries < 1:
+            msg = "max_tries must be >= 1"
+            raise ValueError(msg)
+
+        if cache_ttl_secs < 0:
+            msg = "cache_ttl_secs must be >= 0"
+            raise ValueError(msg)
+
         self._max_tries = max_tries
-        self._cache_dir = cache_dir
+        self._cache_ttl_secs = cache_ttl_secs
+
+    @classmethod
+    def _logger(cls, query: Query) -> logging.Logger:
+        return query.logger or logging.getLogger(f"{cls.__module__}.{cls.__name__}")
 
     def _cache_read(self, query: Query) -> None:
-        if not self._cache_dir or not self._cache_dir.is_dir():
+        logger = DefaultQueryRunner._logger(query)
+
+        if not self._cache_ttl_secs:
             return
 
-        file_path = self._cache_dir / query.cache_key
+        now = int(time.time())
 
-        try:
-            with open(file_path) as file:
-                query._result_set = json.load(file)
-        except (OSError, json.JSONDecodeError) as err:
-            _logger.error(f"failed to read cached {query}", exc_info=err)
+        with tempfile.TemporaryDirectory() as temp_dir:
+            file_path = Path(temp_dir) / query.cache_key
+
+            if not file_path.exists():
+                return
+
+            try:
+                with open(file_path) as file:
+                    result_set = json.load(file)
+            except (OSError, json.JSONDecodeError):
+                logger.exception(f"failed to read cached {query}")
+
+        if result_set.get(_EXPIRATION_KEY, 0) <= now:
+            logger.info(f"{query} cache expired")
+            return
+
+        query._result_set = result_set
+        logger.info(f"{query} was cached")
 
     def _cache_write(self, query: Query) -> None:
-        if not self._cache_dir or not self._cache_dir.is_dir():
+        logger = DefaultQueryRunner._logger(query)
+
+        if not self._cache_ttl_secs:
             return
 
-        file_path = self._cache_dir / query.cache_key
+        now = int(time.time())
+        query.result_set[_EXPIRATION_KEY] = now + self._cache_ttl_secs
 
-        try:
-            with open(file_path, "w") as file:
-                json.dump(query.result_set, file)
-        except OSError as err:
-            _logger.error(f"failed to cache {query}", exc_info=err)
+        with tempfile.TemporaryDirectory() as temp_dir:
+            file_path = Path(temp_dir) / query.cache_key
+            try:
+                with open(file_path, "w") as file:
+                    json.dump(query.result_set, file)
+            except OSError:
+                logger.exception(f"failed to cache {query}")
 
     async def __call__(self, query: Query) -> None:
+        """Called with the current query state before the client makes an API request."""
+        logger = DefaultQueryRunner._logger(query)
+
         # Check cache ahead of first try
         if query.nb_tries == 0:
             self._cache_read(query)
 
         # Success or cached
         if query.done:
             self._cache_write(query)
             return
 
         err = query.error
 
-        # Exhausted all tries; do not retry.
-        if err and query.nb_tries == self._max_tries:
-            raise err
-
-        # Response errors usually indicate a bug in the client; do not retry.
-        if isinstance(err, ResponseError):
-            raise err
+        # Do not retry if we exhausted all tries, or when a retry would not change the result.
+        failed = query.nb_tries == self._max_tries or isinstance(
+            err, (ResponseError, QueryLanguageError)
+        )
 
-        # QL error; do not retry.
-        if isinstance(err, QueryLanguageError):
+        # Exhausted all tries; do not retry.
+        if err and failed:
+            logger.error(f"give up on {query}", exc_info=err)
             raise err
 
         if isinstance(err, QueryRejectError):
             # Wait if the server is too busy.
             if err.cause == QueryRejectCause.TOO_BUSY:
                 backoff = _backoff_secs(query.nb_tries)
-                _logger.debug(f"retry {query} in {backoff:.1f}s")
+                logger.info(f"retry {query} in {backoff:.1f}s")
                 await asyncio.sleep(backoff)
 
             # Wait until a slot opens if the rate limit was exceeded.
             elif err.cause == QueryRejectCause.TOO_MANY_QUERIES:
-                return  # let client enforce cooldown
+                pass  # let client enforce cooldown
 
             # Double timeout if exceeded.
             elif err.cause == QueryRejectCause.EXCEEDED_TIMEOUT:
                 query.timeout_secs = max(query.timeout_secs * 2, DEFAULT_TIMEOUT)
+                logger.info(f"increased [timeout:*] for {query} to {query.timeout_secs:.1f}s")
 
             # Double maxsize if exceeded.
             elif err.cause == QueryRejectCause.EXCEEDED_MAXSIZE:
                 query.maxsize_mib = max(query.maxsize_mib * 2, DEFAULT_MAXSIZE)
+                logger.info(f"increased [maxsize:*] for {query} to {query.maxsize_mib:.1f}mib")
 
 
 def _backoff_secs(tries: int) -> float:
     """Fibonacci sequence: 1, 2, 3, 5, 8, etc."""
     a, b = 1.0, 2.0
 
     for _ in range(tries):
         a, b = b, a + b
 
     return a
 
 
-_logger = logging.getLogger("aio-overpass")
+_EXPIRATION_KEY = "__expiration__"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aio_overpass-0.3.0/pyproject.toml` & `aio_overpass-0.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-overpass"
-version = "0.3.0"
+version = "0.4.0"
 description = "Async client for the Overpass API"
 authors = ["Tim Wiechers <mail@timwie.dev>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/timwie/aio-overpass"
 documentation = "https://www.timwie.dev/aio-overpass/"
 packages = [{ include = "aio_overpass" }]
@@ -30,31 +30,34 @@
 
     # TODO "Development Status :: 5 - Production/Stable"
     #   - release 1.0
     #   - field-tested
     #   - no major bugs
 
     "Development Status :: 3 - Alpha",
+    "Environment :: Web Environment",
     "Framework :: aiohttp",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Internet :: WWW/HTTP",
     "Typing :: Typed",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 [tool.poetry.urls]
+"Changelog" = "https://github.com/timwie/aio-overpass/blob/main/CHANGELOG.md"
 "Coverage" = "https://codecov.io/gh/timwie/aio-overpass"
 
 [tool.poetry.dependencies]
 aiohttp = "~3.8"
 joblib = { version = "~1.3", optional = true }
 networkx = { version = ">=2.7", optional = true }
 python = "^3.9"
@@ -63,55 +66,71 @@
 [tool.poetry.extras]
 joblib = ["joblib"]
 networkx = ["networkx"]
 shapely = ["shapely"]
 
 [tool.poetry.group.dev.dependencies]
 aioresponses = "^0.7.4"
-black = "^23.3.0"
+black = "^23.7.0"
 codecov = "^2.1.13"
-invoke = "^2.1.3"
+invoke = "^2.2.0"
 isort = "^5.12.0"
 mypy = "^1.4.1"
 pdoc = "^14.0.0"
 pytest = "^7.4.0"
-pytest-asyncio = "^0.21.0"
+pytest-asyncio = "^0.21.1"
 pytest-cov = "^4.1.0"
-ruff = "^0.0.275"
+ruff = "^0.0.280"
 
 [tool.poetry.group.notebooks]
 optional = true
 
 [tool.poetry.group.notebooks.dependencies]
 folium = "^0.14.0"
-jupyterlab = "^4.0.2"
+jupyterlab = "^4.0.3"
 papermill = "^2.4.0"
 randomcolor = "^0.4.4.6"
 selenium = "^4.10.0"
 tabulate = "^0.9.0"
 
 [tool.ruff]
 # https://github.com/charliermarsh/ruff#configuration
 # https://beta.ruff.rs/docs/rules/
 line-length = 100
 target-version = "py39"
-select = ["E", "F", "N",  "UP", "ANN", "S", "B", "C4", "PL"]
-ignore = ["ANN003", "ANN101", "ANN401", "C408", "PLR2004", "PLW2901"]
+select = [
+    "F", "E", "W", "N", "D", "UP",
+    "ANN", "S", "B", "C4", "EM", "SIM", "ARG",
+    "PL", "TRY", "PERF", "RUF"
+]
+ignore = [
+    "D105", "D107", "D203", "D212",
+    "ANN003", "ANN101", "ANN102", "ANN401",
+    "C408",
+    "PLR2004", "PLW2901",
+    "TRY003",
+]
+
+# TODO can we select "FIX" with warnings instead of errors?
+#   https://github.com/astral-sh/ruff/issues/1256
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".git",
     ".ipynb_checkpoints",
     ".mypy_cache",
     ".pytest_cache",
     ".ruff_cache",
     "build",
     "doc",
 ]
 
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [tool.black]
 # https://github.com/psf/black#configuration
 line-length = 100
 
 [tool.isort]
 # https://pycqa.github.io/isort/docs/configuration/options.html
 profile = "black"
```

### Comparing `aio_overpass-0.3.0/PKG-INFO` & `aio_overpass-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 Metadata-Version: 2.1
 Name: aio-overpass
-Version: 0.3.0
+Version: 0.4.0
 Summary: Async client for the Overpass API
 Home-page: https://github.com/timwie/aio-overpass
 License: MIT
 Keywords: geojson,geospatial,gis,openstreetmap,osm,overpass-api,public-transport,spatial-analysis,spatial-data,shapely
 Author: Tim Wiechers
 Author-email: mail@timwie.dev
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: aiohttp
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: joblib
 Provides-Extra: networkx
 Provides-Extra: shapely
 Requires-Dist: aiohttp (>=3.8,<3.9)
 Requires-Dist: joblib (>=1.3,<1.4) ; extra == "joblib"
 Requires-Dist: networkx (>=2.7) ; extra == "networkx"
 Requires-Dist: shapely (>=2.0,<2.1) ; extra == "shapely"
+Project-URL: Changelog, https://github.com/timwie/aio-overpass/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://codecov.io/gh/timwie/aio-overpass
 Project-URL: Documentation, https://www.timwie.dev/aio-overpass/
 Project-URL: Repository, https://github.com/timwie/aio-overpass
 Description-Content-Type: text/markdown
 
 <h1 align="center">
 aio-overpass
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/timwie/aio-overpass/test_and_publish.yml)](https://github.com/timwie/aio-overpass/actions/workflows/test_and_publish.yml)
 [![codecov](https://codecov.io/gh/timwie/aio-overpass/branch/main/graph/badge.svg?token=YX1218U740)](https://codecov.io/gh/timwie/aio-overpass)
 [![PyPI version](https://badge.fury.io/py/aio_overpass.svg)](https://badge.fury.io/py/aio_overpass)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aio-overpass)
+[![API reference](https://img.shields.io/badge/API%20reference-555555)](http://www.timwie.dev/aio-overpass/)
 </h1>
 
 A client for the [Overpass API], a read-only API that serves up custom selected
 parts of [OpenStreetMap] data. It is optimized for data consumers that need a few
 elements within a glimpse or up to roughly 10 million elements in some minutes,
 both selected by search criteria like location, type of objects, tag properties,
 proximity, or combinations of them. To make use of it, you should familiarize yourself
```

