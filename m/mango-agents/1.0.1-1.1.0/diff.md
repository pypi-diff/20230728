# Comparing `tmp/mango-agents-1.0.1.tar.gz` & `tmp/mango-agents-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-agents-1.0.1.tar", last modified: Thu Apr 20 09:23:20 2023, max compression
+gzip compressed data, was "mango-agents-1.1.0.tar", last modified: Fri Jul 28 08:54:57 2023, max compression
```

## Comparing `mango-agents-1.0.1.tar` & `mango-agents-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.700207 mango-agents-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-20 09:22:58.000000 mango-agents-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8272 2023-04-20 09:23:20.700207 mango-agents-1.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.688206 mango-agents-1.0.1/mango/
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.689206 mango-agents-1.0.1/mango/agent/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17913 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/agent/core.py
--rw-rw-rw-   0 root         (0) root         (0)    15150 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/agent/role.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.692206 mango-agents-1.0.1/mango/container/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10475 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/core.py
--rw-rw-rw-   0 root         (0) root         (0)     8981 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     5557 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/mosaik.py
--rw-rw-rw-   0 root         (0) root         (0)     9654 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/mqtt.py
--rw-rw-rw-   0 root         (0) root         (0)     4486 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     4343 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/tcp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.694207 mango-agents-1.0.1/mango/messages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/messages/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14633 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/messages/acl_message_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10753 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/messages/codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     6006 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/messages/message.py
--rw-rw-rw-   0 root         (0) root         (0)     2686 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/messages/other_proto_msgs_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.696207 mango-agents-1.0.1/mango/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2591 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/modules/base_module.py
--rw-rw-rw-   0 root         (0) root         (0)     4167 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/modules/mqtt_module.py
--rw-rw-rw-   0 root         (0) root         (0)     4180 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/modules/rabbit_module.py
--rw-rw-rw-   0 root         (0) root         (0)     2827 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/modules/zero_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.698207 mango-agents-1.0.1/mango/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2670 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/util/clock.py
--rw-rw-rw-   0 root         (0) root         (0)     4211 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/util/distributed_clock.py
--rw-rw-rw-   0 root         (0) root         (0)    26401 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/util/scheduling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.700207 mango-agents-1.0.1/mango_agents.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8272 2023-04-20 09:23:20.000000 mango-agents-1.0.1/mango_agents.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      852 2023-04-20 09:23:20.000000 mango-agents-1.0.1/mango_agents.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 09:23:20.000000 mango-agents-1.0.1/mango_agents.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-20 09:23:20.000000 mango-agents-1.0.1/mango_agents.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-20 09:23:20.000000 mango-agents-1.0.1/mango_agents.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 09:23:20.701207 mango-agents-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4079 2023-04-20 09:22:58.000000 mango-agents-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:54:57.561686 mango-agents-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-07-28 08:54:39.000000 mango-agents-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8272 2023-07-28 08:54:57.561686 mango-agents-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:54:57.553686 mango-agents-1.1.0/mango/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:54:57.554686 mango-agents-1.1.0/mango/agent/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18262 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/agent/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    15443 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/agent/role.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:54:57.556686 mango-agents-1.1.0/mango/container/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/container/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32370 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/container/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     8904 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/container/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5042 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/container/mosaik.py
+-rw-rw-rw-   0 root         (0) root         (0)     9918 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/container/mqtt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/container/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     9980 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/container/tcp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:54:57.557686 mango-agents-1.1.0/mango/messages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/messages/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/messages/acl_message_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    11319 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/messages/codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     6006 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/messages/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/messages/other_proto_msgs_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:54:57.558686 mango-agents-1.1.0/mango/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2591 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/modules/base_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     4167 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/modules/mqtt_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     4180 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/modules/rabbit_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     2827 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/modules/zero_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:54:57.559686 mango-agents-1.1.0/mango/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2670 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/util/clock.py
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/util/distributed_clock.py
+-rw-rw-rw-   0 root         (0) root         (0)     9179 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/util/multiprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)    28096 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/util/scheduling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1999 2023-07-28 08:54:39.000000 mango-agents-1.1.0/mango/util/termination_detection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:54:57.560686 mango-agents-1.1.0/mango_agents.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8272 2023-07-28 08:54:57.000000 mango-agents-1.1.0/mango_agents.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      918 2023-07-28 08:54:57.000000 mango-agents-1.1.0/mango_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 08:54:57.000000 mango-agents-1.1.0/mango_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-28 08:54:57.000000 mango-agents-1.1.0/mango_agents.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-28 08:54:57.000000 mango-agents-1.1.0/mango_agents.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 08:54:57.561686 mango-agents-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2023-07-28 08:54:39.000000 mango-agents-1.1.0/setup.py
```

### Comparing `mango-agents-1.0.1/LICENSE` & `mango-agents-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.1/PKG-INFO` & `mango-agents-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-agents
-Version: 1.0.1
+Version: 1.1.0
 Summary: Modular Python Agent Framework
 Author: mango Team
 Author-email: mango@offis.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mango-agents-1.0.1/mango/agent/core.py` & `mango-agents-1.1.0/mango/agent/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,21 +411,31 @@
         """
         await self._scheduler.tasks_complete(timeout=timeout)
 
 
 class Agent(ABC, AgentDelegates):
     """Base class for all agents."""
 
-    def __init__(self, container: Container, suggested_aid: str = None):
+    def __init__(
+        self,
+        container: Container,
+        suggested_aid: str = None,
+        suspendable_tasks=True,
+        observable_tasks=True,
+    ):
         """Initialize an agent and register it with its container
         :param container: The container that the agent lives in. Must be a Container
         :param suggested_aid: (Optional) suggested aid, if the aid is already taken, a generated aid is used.
                               Using the generated aid-style ("agentX") is not allowed.
         """
-        scheduler = Scheduler(clock=container.clock)
+        scheduler = Scheduler(
+            clock=container.clock,
+            suspendable=suspendable_tasks,
+            observable=observable_tasks,
+        )
         context = AgentContext(container)
         self.aid = context.register_agent(self, suggested_aid)
         self.inbox = asyncio.Queue()
 
         super().__init__(context, scheduler)
 
         self._check_inbox_task = asyncio.create_task(self._check_inbox())
@@ -444,28 +454,31 @@
                 f"Agent {self.aid}: Caught the following exception in _check_inbox: {fut.exception()}"
             )
             raise fut.exception()
 
     async def _check_inbox(self):
         """Task for waiting on new message in the inbox"""
 
-        logger.debug("Agent %s: Start waiting for messages", self.aid)
-        while True:
-            # run in infinite loop until it is cancelled from outside
-            message = await self.inbox.get()
-            logger.debug("Agent %s: Received message;%s", self.aid, message)
-
-            # message should be tuples of (priority, content, meta)
-            priority, content, meta = message
-            meta["priority"] = priority
-            
-            self.handle_message(content=content, meta=meta)
-
-            # signal to the Queue that the message is handled
-            self.inbox.task_done()
+        try:
+            logger.debug("Agent %s: Start waiting for messages", self.aid)
+            while True:
+                # run in infinite loop until it is cancelled from outside
+                message = await self.inbox.get()
+                logger.debug("Agent %s: Received message;%s", self.aid, message)
+
+                # message should be tuples of (priority, content, meta)
+                priority, content, meta = message
+                meta["priority"] = priority
+
+                self.handle_message(content=content, meta=meta)
+
+                # signal to the Queue that the message is handled
+                self.inbox.task_done()
+        except Exception:
+            logger.exception("The check inbox task of %s failed!", self.aid)
 
     def handle_message(self, content, meta: Dict[str, Any]):
         """
 
         Has to be implemented by the user.
         This method is called when a message is received at the agents inbox.
         :param content: The deserialized message object
```

### Comparing `mango-agents-1.0.1/mango/agent/role.py` & `mango-agents-1.1.0/mango/agent/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 from mango.util.scheduling import Scheduler
 
 
 class DataContainer:
     def __getitem__(self, key):
         return self.__getattribute__(key)
 
+    def __contains__(self, key):
+        return hasattr(self, key)
+
 
 class RoleContext:
     pass
 
 
 class Role(ABC):
     """General role class, defining the API every role can use. A role implements one responsibility
@@ -398,22 +401,33 @@
 
 
 class RoleAgent(Agent):
     """Agent, which support the role API-system. When you want to use the role-api you always need
     a RoleAgent as base for your agents. A role can be added with :func:`RoleAgent.add_role`.
     """
 
-    def __init__(self, container, suggested_aid: str = None):
+    def __init__(
+        self,
+        container,
+        suggested_aid: str = None,
+        suspendable_tasks=True,
+        observable_tasks=True,
+    ):
         """Create a role-agent
 
         :param container: container the agent lives in
         :param suggested_aid: (Optional) suggested aid, if the aid is already taken, a generated aid is used.
                               Using the generated aid-style ("agentX") is not allowed.
         """
-        super().__init__(container, suggested_aid=suggested_aid)
+        super().__init__(
+            container,
+            suggested_aid=suggested_aid,
+            suspendable_tasks=suspendable_tasks,
+            observable_tasks=observable_tasks,
+        )
 
         self._role_handler = RoleHandler(self._context, self._scheduler)
         self._role_context = RoleContext(
             self._context, self._scheduler, self._role_handler, self.aid, self.inbox
         )
 
     def add_role(self, role: Role):
```

### Comparing `mango-agents-1.0.1/mango/container/core.py` & `mango-agents-1.1.0/mango/container/mqtt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,284 +1,284 @@
 import asyncio
-import copy
 import logging
-import warnings
-from abc import ABC, abstractmethod
-from typing import Any, Dict, Optional, Tuple, Union
+from typing import Any, Dict, Optional, Set, Tuple, Union
+
+import paho.mqtt.client as paho
+
+from mango.container.core import Container, ContainerMirrorData
 
 from ..messages.codecs import ACLMessage, Codec
 from ..util.clock import Clock
 
 logger = logging.getLogger(__name__)
 
-AGENT_PATTERN_NAME_PRE = "agent"
-
 
-class Container(ABC):
-    """Superclass for a mango container"""
+class MQTTContainer(Container):
+    """
+    Container for agents.
+
+       The container allows its agents to send messages to specific topics
+       (via :meth:`send_message()`).
+    """
 
     def __init__(
-        self, *, addr, name: str, codec, loop, clock: Clock, copy_internal_messages=False
+        self,
+        *,
+        client_id: str,
+        addr: Optional[str],
+        loop: asyncio.AbstractEventLoop,
+        clock: Clock,
+        mqtt_client: paho.Client,
+        codec: Codec,
+        **kwargs,
     ):
-        self.name: str = name
-        self.addr = addr
-        self.clock = clock
-        self._copy_internal_messages = copy_internal_messages
-
-        self.codec: Codec = codec
-        self.loop: asyncio.AbstractEventLoop = loop
-
-        # dict of agents. aid: agent instance
-        self._agents: Dict = {}
-        self._aid_counter: int = 0  # counter for aids
-
-        self.running: bool = True  # True until self.shutdown() is called
-        self._no_agents_running: asyncio.Future = asyncio.Future()
-        self._no_agents_running.set_result(
-            True
-        )  # signals that currently no agent lives in this container
-
-        # inbox for all incoming messages
-        self.inbox: asyncio.Queue = asyncio.Queue()
-
-        # task that processes the inbox.
-        self._check_inbox_task: asyncio.Task = asyncio.create_task(self._check_inbox())
-
-    def is_aid_available(self, aid):
-        """
-        Check if the aid is available and allowed.
-        It is not possible to register aids matching the regular pattern "agentX".
-        :param aid: the aid you want to check
-        :return True if the aid is available, False if it is not
-        """
-        return aid not in self._agents and not self.__check_agent_aid_pattern_match(aid)
-
-    def __check_agent_aid_pattern_match(self, aid):
-        return (
-            aid.startswith(AGENT_PATTERN_NAME_PRE)
-            and aid[len(AGENT_PATTERN_NAME_PRE) :].isnumeric()
+        """
+        Initializes a container. Do not directly call this method but use
+        the factory method instead
+        :param client_id: The ID that the container should use when connecting
+        to the broker
+        :param addr: A string of the unique inbox topic to use.
+        No wildcards are allowed. If None, no inbox topic will be set
+        :param mqtt_client: The paho.Client object that is used for the
+        communication with the broker
+        :param codec: The codec to use. Currently only 'json' or 'protobuf' are
+         allowed
+        """
+        super().__init__(
+            codec=codec, addr=addr, loop=loop, clock=clock, name=client_id, **kwargs
         )
 
-    def register_agent(self, agent, suggested_aid: str = None):
-        """
-        Register *agent* and return the agent id
-        :param agent: The agent instance
-        :param suggested_aid: (Optional) suggested aid, if the aid is already taken, a generated aid is used.
-                              Using the generated aid-style ("agentX") is not allowed.
-        :return The agent ID
+        self.client_id: str = client_id
+        # the configured and connected paho client
+        self.mqtt_client: paho.Client = mqtt_client
+        self.inbox_topic: Optional[str] = addr
+        # dict mapping additionally subscribed topics to a set of aids
+        self.additional_subscriptions: Dict[str, Set[str]] = {}
+        # Future for pending sub requests
+        self.pending_sub_request: Optional[asyncio.Future] = None
+
+        # set the callbacks
+        self._set_mqtt_callbacks()
+
+        # start the mqtt client
+        self.mqtt_client.loop_start()
+
+    def _set_mqtt_callbacks(self):
+        """
+        Sets the callbacks for the mqtt paho client
+        """
+
+        def on_con(client, userdata, flags, rc):
+            if rc != 0:
+                logger.info("Connection attempt to broker failed")
+            else:
+                logger.debug("Successfully reconnected to broker.")
+
+        self.mqtt_client.on_connect = on_con
+
+        def on_discon(client, userdata, rc):
+            if rc != 0:
+                logger.warning("Unexpected disconnect from broker. Trying to reconnect")
+            else:
+                logger.debug("Successfully disconnected from broker.")
+
+        self.mqtt_client.on_disconnect = on_discon
+
+        def on_sub(client, userdata, mid, granted_qos):
+            self.loop.call_soon_threadsafe(self.pending_sub_request.set_result, 0)
+
+        self.mqtt_client.on_subscribe = on_sub
+
+        def on_message(client, userdata, message):
+            # extract the meta information first
+            meta = {
+                "network_protocol": "mqtt",
+                "topic": message.topic,
+                "qos": message.qos,
+                "retain": message.retain,
+            }
+            # decode message and extract content and meta
+            content, message_meta = self.decode_mqtt_message(
+                payload=message.payload, topic=message.topic
+            )
+            # update meta dict
+            meta.update(message_meta)
+            # put information to inbox
+            self.loop.call_soon_threadsafe(self.inbox.put_nowait, (0, content, meta))
+
+        self.mqtt_client.on_message = on_message
+        self.mqtt_client.enable_logger(logger)
+
+    def decode_mqtt_message(self, *, topic, payload):
+        """
+        deserializes a mqtt message.
+        Checks if for the topic a special class is defined, otherwise assumes
+        an ACLMessage
+        :param topic: the topic on which the message arrived
+        :param payload: the serialized message
+        :return: content and meta
         """
-        if not self._no_agents_running or self._no_agents_running.done():
-            self._no_agents_running = asyncio.Future()
-        if (
-            suggested_aid is None
-            or suggested_aid in self._agents
-            or self.__check_agent_aid_pattern_match(suggested_aid)
-        ):
-            aid = f"{AGENT_PATTERN_NAME_PRE}{self._aid_counter}"
-            self._aid_counter += 1
+        meta = {}
+        content = None
+
+        decoded = self.codec.decode(payload)
+        if isinstance(decoded, ACLMessage):
+            content, meta = decoded.split_content_and_meta()
         else:
-            aid = suggested_aid
-        self._agents[aid] = agent
-        logger.info("Successfully registered agent;%s", aid)
-        return aid
+            content = decoded
 
-    def deregister_agent(self, aid):
-        """
-        Deregister an agent
-        :param aid:
-        :return:
+        return content, meta
 
+    async def _handle_message(self, *, priority: int, content, meta: Dict[str, Any]):
+        """
+        This is called as a separate task for every message that is read
+        :param priority: priority of the message
+        :param content: Deserialized content of the message
+        :param meta: Dict with additional information (e.g. topic)
         """
-        del self._agents[aid]
-        if len(self._agents) == 0:
-            self._no_agents_running.set_result(True)
+        topic = meta["topic"]
+        logger.debug(
+            f"Received message with content and meta;{str(content)};{str(meta)}"
+        )
+        if topic == self.inbox_topic:
+            # General inbox topic, so no receiver is specified by the topic
+            # try to find the receiver from meta
+            receiver_id = meta.get("receiver_id", None)
+            if receiver_id and receiver_id in self._agents.keys():
+                receiver = self._agents[receiver_id]
+                await receiver.inbox.put((priority, content, meta))
+            else:
+                logger.warning("Receiver ID is unknown;%s", receiver_id)
+        else:
+            # no inbox topic. Check who has subscribed the topic.
+            receivers = set()
+            for sub, rec in self.additional_subscriptions.items():
+                if paho.topic_matches_sub(sub, topic):
+                    receivers.update(rec)
+            if not receivers:
+                logger.warning(
+                    f"Received a message at a topic which no agent subscribed;{topic}"
+                )
+            else:
+                for receiver_id in receivers:
+                    receiver = self._agents[receiver_id]
+                    await receiver.inbox.put((priority, content, meta))
 
-    @abstractmethod
     async def send_message(
         self,
         content,
         receiver_addr: Union[str, Tuple[str, int]],
         *,
         receiver_id: Optional[str] = None,
         **kwargs,
-    ) -> bool:
+    ):
         """
-        The Container sends a message to an agent according the container protocol.
+        The container sends the message of one of its own agents to a specific topic.
 
         :param content: The content of the message
-        :param receiver_addr: In case of TCP this is a tuple of host, port
-            In case of MQTT this is the topic to publish to.
+        :param receiver_addr: The topic to publish to.
         :param receiver_id: The agent id of the receiver
         :param kwargs: Additional parameters to provide protocol specific settings
+            Possible fields:
+            qos: The quality of service to use for publishing
+            retain: Indicates, weather the retain flag should be set
+            Ignored if connection_type != 'mqtt'
+
         """
-        raise NotImplementedError
+        # the message is already complete
+        message = content
+
+        # internal message first (if retain Flag is set, it has to be sent to
+        # the broker
+        actual_mqtt_kwargs = {} if kwargs is None else kwargs
+        if (
+            self.addr
+            and receiver_addr == self.addr
+            and not actual_mqtt_kwargs.get("retain", False)
+        ):
+            meta = {
+                "topic": self.addr,
+                "qos": actual_mqtt_kwargs.get("qos", 0),
+                "retain": False,
+                "network_protocol": "mqtt",
+            }
+            return self._send_internal_message(
+                message, receiver_id, default_meta=meta, inbox=self.inbox
+            )
 
-    async def send_acl_message(
-        self,
-        content,
-        receiver_addr: Union[str, Tuple[str, int]],
-        *,
-        receiver_id: Optional[str] = None,
-        acl_metadata: Optional[Dict[str, Any]] = None,
-        is_anonymous_acl=False,
-        **kwargs,
-    ) -> bool:
+        else:
+            self._send_external_message(topic=receiver_addr, message=message)
+            return True
+
+    def _send_external_message(self, *, topic: str, message):
         """
-        The Container sends a message, wrapped in an ACL message, to an agent according the container protocol.
 
-        :param content: The content of the message
-        :param receiver_addr: In case of TCP this is a tuple of host, port
-        In case of MQTT this is the topic to publish to.
-        :param receiver_id: The agent id of the receiver
-        :param acl_metadata: metadata for the acl_header.
-        :param is_anonymous_acl: If set to True, the sender information won't be written in the ACL header
-        :param kwargs: Additional parameters to provide protocol specific settings
+        :param topic: MQTT topic
+        :param message: The ACL message
+        :return:
         """
-        return await self.send_message(
-            self._create_acl(
-                content,
-                receiver_addr=receiver_addr,
-                receiver_id=receiver_id,
-                acl_metadata=acl_metadata,
-                is_anonymous_acl=is_anonymous_acl,
-            ),
-            receiver_addr=receiver_addr,
-            receiver_id=receiver_id,
-            **kwargs,
-        )
+        encoded_message = self.codec.encode(message)
+        logger.debug("Sending message;%s;%s", message, topic)
+        self.mqtt_client.publish(topic, encoded_message)
 
-    def _create_acl(
-        self,
-        content,
-        receiver_addr: Union[str, Tuple[str, int]],
-        receiver_id: Optional[str] = None,
-        acl_metadata: Optional[Dict[str, Any]] = None,
-        is_anonymous_acl=False,
-    ):
+    async def subscribe_for_agent(self, *, aid: str, topic: str, qos: int = 0) -> bool:
         """
-        :param content:
-        :param receiver_addr:
-        :param receiver_id:
-        :param acl_metadata:
-        :return:
+
+        :param aid: aid of the corresponding agent
+        :param topic: topic to subscribe (wildcards are allowed)
+        :param qos: The quality of service for the subscription
+        :return: A boolean signaling if subscription was true or not
         """
-        acl_metadata = {} if acl_metadata is None else acl_metadata.copy()
-        # analyse and complete acl_metadata
-        if "receiver_addr" not in acl_metadata.keys():
-            acl_metadata["receiver_addr"] = receiver_addr
-        elif acl_metadata["receiver_addr"] != receiver_addr:
-            warnings.warn(
-                f"The argument receiver_addr ({receiver_addr}) is not equal to "
-                f"acl_metadata['receiver_addr'] ({acl_metadata['receiver_addr']}). \
-                            For consistency, the value in acl_metadata['receiver_addr'] "
-                f"was overwritten with receiver_addr.",
-                UserWarning,
-            )
-            acl_metadata["receiver_addr"] = receiver_addr
-        if receiver_id:
-            if "receiver_id" not in acl_metadata.keys():
-                acl_metadata["receiver_id"] = receiver_id
-            elif acl_metadata["receiver_id"] != receiver_id:
-                warnings.warn(
-                    f"The argument receiver_id ({receiver_id}) is not equal to "
-                    f"acl_metadata['receiver_id'] ({acl_metadata['receiver_id']}). \
-                               For consistency, the value in acl_metadata['receiver_id'] "
-                    f"was overwritten with receiver_id.",
-                    UserWarning,
-                )
-                acl_metadata["receiver_id"] = receiver_id
-        # add sender_addr if not defined and not anonymous
-        if not is_anonymous_acl:
-            if "sender_addr" not in acl_metadata.keys() and self.addr is not None:
-                acl_metadata["sender_addr"] = self.addr
-
-        message = ACLMessage()
-        message.content = content
-
-        for key, value in acl_metadata.items():
-            setattr(message, key, value)
-        return message
-
-    def _send_internal_message(
-        self, message, priority=0, default_meta=None, target_inbox_overwrite=None
-    ) -> bool:
-        meta = {}
+        if aid not in self._agents.keys():
+            raise ValueError("Given aid is not known")
 
-        message_to_send = (
-            copy.deepcopy(message) if self._copy_internal_messages else message
-        )
-        target_inbox = (
-            self.inbox if target_inbox_overwrite is None else target_inbox_overwrite
-        )
+        if topic in self.additional_subscriptions.keys():
+            self.additional_subscriptions[topic].add(aid)
+            return True
 
-        if hasattr(message_to_send, "split_content_and_meta"):
-            content, meta = message_to_send.split_content_and_meta()
-        else:
-            content = message_to_send
-        meta.update(default_meta)
+        self.additional_subscriptions[topic] = {aid}
+        self.pending_sub_request = asyncio.Future()
+        result, _ = self.mqtt_client.subscribe(topic, qos=qos)
 
-        target_inbox.put_nowait((priority, content, meta))
+        if result != paho.MQTT_ERR_SUCCESS:
+            self.pending_sub_request.set_result(False)
+            return False
+
+        await self.pending_sub_request
         return True
 
-    async def _check_inbox(self):
-        """
-        Task that checks, if there is a message in inbox and then creates a
-        task to handle message
+    def deregister_agent(self, aid):
         """
 
-        def raise_exceptions(result):
-            """
-            Inline function used as a callback to tasks to raise exceptions
-            :param result: result object of the task
-            """
-            exception = result.exception()
-            if exception is not None:
-                logger.warning("Exception in _check_inbox_task.")
-                raise exception
-
-        while True:
-            data = await self.inbox.get()
-            priority, content, meta = data
-            task = asyncio.create_task(
-                self._handle_message(priority=priority, content=content, meta=meta)
-            )
-            task.add_done_callback(raise_exceptions)
-            self.inbox.task_done()  # signals that the queue object is
-            # processed
-
-    async def _handle_message(self, *, priority: int, content, meta: Dict[str, Any]):
-        """
-        This is called as a separate task for every message that is read
-        :param priority: priority of the message
-        :param content: Deserialized content of the message
-        :param meta: Dict with additional information (e.g. topic)
+        :param aid:
+        :return:
         """
+        super().deregister_agent(aid)
+        empty_subscriptions = []
+        for subscription, aid_set in self.additional_subscriptions.items():
+            if aid in aid_set:
+                aid_set.remove(aid)
+            if len(aid_set) == 0:
+                empty_subscriptions.append(subscription)
+
+        for subscription in empty_subscriptions:
+            self.additional_subscriptions.pop(subscription)
+            self.mqtt_client.unsubscribe(topic=subscription)
 
-        logger.debug(
-            f"Received message with content and meta;{str(content)};{str(meta)}"
+    def as_agent_process(
+        self,
+        agent_creator,
+        mirror_container_creator,
+    ):
+        return super().as_agent_process(
+            agent_creator=agent_creator,
+            mirror_container_creator=mirror_container_creator,
         )
-        receiver_id = meta.get("receiver_id", None)
-        if receiver_id and receiver_id in self._agents.keys():
-            receiver = self._agents[receiver_id]
-            await receiver.inbox.put((priority, content, meta))
-        else:
-            logger.warning("Received a message for an unknown receiver;%s", receiver_id)
 
     async def shutdown(self):
-        """Shutdown all agents in the container and the container itself"""
-        self.running = False
-        futs = []
-        for agent in self._agents.values():
-            # shutdown all running agents
-            futs.append(agent.shutdown())
-        await asyncio.gather(*futs)
-
-        # cancel check inbox task
-        if self._check_inbox_task is not None:
-            logger.debug("check inbox task will be cancelled")
-            self._check_inbox_task.cancel()
-            try:
-                await self._check_inbox_task
-            except asyncio.CancelledError:
-                pass
-            finally:
-                logger.info("Successfully shutdown")
+        """
+        Shutdown container, disconnect from broker and stop mqtt thread
+        """
+        await super().shutdown()
+        # disconnect to broker
+        self.mqtt_client.disconnect()
+        self.mqtt_client.loop_stop()
```

### Comparing `mango-agents-1.0.1/mango/container/factory.py` & `mango-agents-1.1.0/mango/container/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 
 async def create(
     *,
     connection_type: str = "tcp",
     codec: Codec = None,
     clock: Clock = None,
     addr: Optional[Union[str, Tuple[str, int]]] = None,
-    copy_internal_messages=True,
+    copy_internal_messages: bool = False,
     mqtt_kwargs: Dict[str, Any] = None,
+    **kwargs: Dict[str, Any],
 ) -> Container:
     """
     This method is called to instantiate a container instance, either
     a TCPContainer or a MQTTContainer, depending on the parameter
     connection_type.
     :param connection_type: Defines the connection type. So far only 'tcp'
     or 'mqtt' are allowed
@@ -65,23 +66,17 @@
         # initialize TCPContainer
         container = TCPContainer(
             addr=addr,
             codec=codec,
             loop=loop,
             clock=clock,
             copy_internal_messages=copy_internal_messages,
+            **kwargs,
         )
-
-        # create a TCP server bound to host and port that uses the
-        # specified protocol
-        container.server = await loop.create_server(
-            lambda: ContainerProtocol(container=container, loop=loop, codec=codec),
-            addr[0],
-            addr[1],
-        )
+        await container.setup()
         return container
 
     if connection_type == MOSAIK_CONNECTION:
         return MosaikContainer(addr=addr, loop=loop, codec=codec)
 
     if connection_type == MQTT_CONNECTION:
         # get and check relevant kwargs from mqtt_kwargs
@@ -136,26 +131,26 @@
             loop.call_soon_threadsafe(connected.set_result, returncode)
 
         mqtt_messenger.on_connect = on_con
 
         # check broker_addr input and connect
         if isinstance(broker_addr, tuple):
             if not 0 < len(broker_addr) < 4:
-                raise ValueError(f"Invalid broker address")
+                raise ValueError(f"Invalid broker address argument count")
             if len(broker_addr) > 0 and not isinstance(broker_addr[0], str):
-                raise ValueError("Invalid broker address")
+                raise ValueError("Invalid broker address - host must be str")
             if len(broker_addr) > 1 and not isinstance(broker_addr[1], int):
-                raise ValueError("Invalid broker address")
+                raise ValueError("Invalid broker address - port must be int")
             if len(broker_addr) > 2 and not isinstance(broker_addr[2], int):
-                raise ValueError("Invalid broker address")
+                raise ValueError("Invalid broker address - keepalive must be int")
             mqtt_messenger.connect(*broker_addr, **mqtt_kwargs)
 
         elif isinstance(broker_addr, dict):
             if "hostname" not in broker_addr.keys():
-                raise ValueError("Invalid broker address")
+                raise ValueError("Invalid broker address - host not given")
             mqtt_messenger.connect(**broker_addr, **mqtt_kwargs)
 
         else:
             if not isinstance(broker_addr, str):
                 raise ValueError("Invalid broker address")
             mqtt_messenger.connect(broker_addr, **mqtt_kwargs)
 
@@ -230,8 +225,9 @@
             client_id=client_id,
             addr=addr,
             loop=loop,
             clock=clock,
             mqtt_client=mqtt_messenger,
             codec=codec,
             copy_internal_messages=copy_internal_messages,
+            **kwargs,
         )
```

### Comparing `mango-agents-1.0.1/mango/container/mosaik.py` & `mango-agents-1.1.0/mango/container/mosaik.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from mango.container.core import Container
 
 from ..messages.codecs import Codec
 from ..util.clock import ExternalClock
+from ..util.termination_detection import tasks_complete_or_sleeping
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class MosaikAgentMessage:
     message: bytes
@@ -78,28 +79,19 @@
         :param kwargs: Additional parameters to provide protocol specific settings
         """
         message = content
 
         if receiver_addr == self.addr:
             if not receiver_id:
                 receiver_id = message.receiver_id
-            # internal message
-            receiver = self._agents.get(receiver_id, None)
-            if receiver is None:
-                logger.warning(
-                    f"Sending internal message not successful, receiver id unknown;{receiver_id}"
-                )
-                return False
-            self._new_internal_message = True
             default_meta = {"network_protocol": "mosaik"}
             success = self._send_internal_message(
-                message=message,
-                default_meta=default_meta,
-                target_inbox_overwrite=receiver.inbox,
+                message=message, receiver_id=receiver_id, default_meta=default_meta
             )
+            self._new_internal_message = True
         else:
             success = await self._send_external_message(receiver_addr, message)
 
         return success
 
     async def _send_external_message(self, addr, message) -> bool:
         """
@@ -118,15 +110,14 @@
             )
         )
         return True
 
     async def step(
         self, simulation_time: float, incoming_messages: List[bytes]
     ) -> MosaikContainerOutput:
-
         if self.message_buffer:
             logger.warning(
                 "There are messages in teh message buffer to be sent, at the start when step was called."
             )
 
         self.current_start_time_of_step = time.time()
 
@@ -145,22 +136,20 @@
         await self.inbox.join()
 
         # now wait for all agents to terminate
         # we need to loop here, because we might need to join the agents inbox another times in case we send internal
         # messages
         while True:
             self._new_internal_message = False
-            for agent in self._agents.values():
-                await agent.inbox.join()  # make sure inbox of agent is empty and all messages are processed
-                # TODO In the following we should also be able to recognize manual sleeps (maybe)
-                await agent._scheduler.tasks_complete_or_sleeping()  # wait until agent is done with all tasks
+            await tasks_complete_or_sleeping(self)
+            # wait until all agents are done with their tasks
             if not self._new_internal_message:
                 # if there have
                 break
-        # now all agents should be done
+        # now all agents in this container should be done
         end_time = time.time()
 
         messages_this_step, self.message_buffer = self.message_buffer, []
 
         return MosaikContainerOutput(
             duration=end_time - self.current_start_time_of_step,
             messages=messages_this_step,
```

### Comparing `mango-agents-1.0.1/mango/container/protocol.py` & `mango-agents-1.1.0/mango/container/protocol.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,133 +9,114 @@
 # The header stores the number of bytes in the payload
 HEADER = struct.Struct("!L")
 
 logger = logging.getLogger(__name__)
 
 
 class ContainerProtocol(asyncio.Protocol):
-    """ """
+    """Protocol for implementing the TCP Container connection. Internally reads the asyncio transport object
+    into a buffer and moves the read messages async to the container inbox."""
 
     def __init__(self, *, container, loop, codec):
         """
 
         :param container:
         :param loop:
         """
         super().__init__()
+
         self.codec = codec
         self.transport = None
         self.container = container
         self._loop = loop
         self._buffer = bytearray()
-        self._required_read_size = None
-
-        self._out_msgs = asyncio.Queue()
-        self._task_process_out_msg = None
 
     def connection_made(self, transport):
         """
 
         :param transport:
 
         """
         self.transport = transport  # store transport object
 
-        # start task for writing outgoing messages
-        self._task_process_out_msg = self._loop.create_task(self._process_out_msgs())
-
     def connection_lost(self, exc):
         """
 
         :param exc:
         :return:
         """
-        # TODO
-        self._task_process_out_msg.cancel()
-        self.transport.close()
+        super().connection_lost(exc)
 
     def data_received(self, data):
         """
 
         :param data:
         :return:
         """
-
+        required_read_size = None
         self._buffer.extend(data)
         while True:
             # We may have more then one message in the buffer,
             # so we loop over the buffer until we got all complete messages.
 
-            if self._required_read_size is None and len(self._buffer) >= HEADER.size:
+            if required_read_size is None and len(self._buffer) >= HEADER.size:
                 # Received the complete header of a new message
                 logger.debug("Received complete header of a message")
 
-                self._required_read_size = HEADER.unpack_from(self._buffer)[0]
+                required_read_size = HEADER.unpack_from(self._buffer)[0]
                 # Unpack from buffer, according to the format of the struct.
                 # The result is a tuple even if it contains exactly one item.
-                # The self._buffer object reamins unchanged
+                # The buffer object reamins unchanged
                 # The header is also in the buffer
-                self._required_read_size += HEADER.size
+                required_read_size += HEADER.size
 
             if (
-                self._required_read_size is not None
-                and len(self._buffer) >= self._required_read_size
+                required_read_size is not None
+                and len(self._buffer) >= required_read_size
             ):
                 logger.debug("Received complete message")
                 # At least one complete message is in the buffer
                 # read the payload of the message
-                data = self._buffer[HEADER.size : self._required_read_size]
-                self._buffer = self._buffer[self._required_read_size :]
-                self._required_read_size = None
+                data = self._buffer[HEADER.size : required_read_size]
+                self._buffer = self._buffer[required_read_size:]
+                required_read_size = None
 
                 message = self.codec.decode(data)
 
-                content, acl_meta = message.split_content_and_meta()
-                acl_meta["network_protocol"] = "tcp"
+                if hasattr(message, "split_content_and_meta"):
+                    content, acl_meta = message.split_content_and_meta()
+                    acl_meta["network_protocol"] = "tcp"
+                else:
+                    content, acl_meta = message, message
 
                 # TODO priority is now always 0,
                 #  but should be encoded in the message
                 self.container.inbox.put_nowait((0, content, acl_meta))
 
             else:
                 # No complete message in the buffer, nothing more to do.
                 break
 
     def write(self, msg_payload):
         """
+        Write the message (as bytes) to the connection.
 
         :param msg_payload:  message payload
         :return:
         """
 
         # get length of the payload and store the number of bytes as byte
         # object defined in Header
+
         header = HEADER.pack(len(msg_payload))
 
         message = header + msg_payload  # message is header and payload
 
-        self._out_msgs.put_nowait(message)
-
-    async def _process_out_msgs(self):
-        try:
-            while True:
-                content = await self._out_msgs.get()
-                self.transport.write(content)
-                self._out_msgs.task_done()
-                # done.set_result(True)
-        except asyncio.CancelledError:
-            # TODO
-            pass
-            # assert self._connection_lost is not None
+        self.transport.write(message)
 
     async def shutdown(self):
         """
         Will close the transport and stop the writing task
         :return:
         """
-        await self._out_msgs.join()  # wait until all outbox messages are sent
         self.transport.close()  # this will cause the
         # self._task_process_out_msg to be cancelled
-        try:
-            await self._task_process_out_msg
-        except asyncio.CancelledError:
-            pass
```

### Comparing `mango-agents-1.0.1/mango/messages/codecs.py` & `mango-agents-1.1.0/mango/messages/codecs.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 Most of this code is taken and adapted from Stefan Scherfkes aiomas:
 https://gitlab.com/sscherfke/aiomas/
 """
 
 import inspect
 import json
+import msgspec
 
 from mango.messages.message import ACLMessage, Performatives, enum_serializer
 
 from ..messages.acl_message_pb2 import ACLMessage as ACLProto
 from ..messages.other_proto_msgs_pb2 import GenericMsg as GenericProtoMsg
 
 
@@ -171,14 +172,32 @@
     def encode(self, data):
         return json.dumps(data, default=self.serialize_obj).encode()
 
     def decode(self, data):
         return json.loads(data.decode(), object_hook=self.deserialize_obj)
 
 
+class FastJSON(Codec):
+    def __init__(self):
+        super().__init__()
+        self.add_serializer(*ACLMessage.__json_serializer__())
+        self.add_serializer(*enum_serializer(Performatives))
+
+        self.encoder = msgspec.json.Encoder(enc_hook=self.serialize_obj)
+        self.decoder = msgspec.json.Decoder(
+            dec_hook=lambda _, b: self.deserialize_obj(b), type=ACLMessage
+        )
+
+    def encode(self, data):
+        return self.encoder.encode(data)
+
+    def decode(self, data):
+        return self.decoder.decode(data)
+
+
 class PROTOBUF(Codec):
     def __init__(self):
         super().__init__()
         # expected serializers: (obj, to_proto, from_proto)
         # output of to_proto is the already serialized(!) proto object
         # input of from_proto is the string representation of the proto object
         # the codec merely handles the mapping of object types to these methods
@@ -194,15 +213,15 @@
         proto_msg.type_id = typeid
         proto_msg.content = content.SerializeToString()
         return proto_msg.SerializeToString()
 
     def decode(self, data):
         proto_msg = GenericProtoMsg()
         try:
-            proto_msg.ParseFromString(data)
+            proto_msg.ParseFromString(bytes(data))
         except Exception as e:
             raise DecodeError(f"Could not parse data: {data}") from e
 
         obj_repr = {"__type__": (proto_msg.type_id, proto_msg.content)}
         return self.deserialize_obj(obj_repr)
 
     def serialize_obj(self, obj):
```

### Comparing `mango-agents-1.0.1/mango/messages/message.py` & `mango-agents-1.1.0/mango/messages/message.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.1/mango/modules/base_module.py` & `mango-agents-1.1.0/mango/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.1/mango/modules/mqtt_module.py` & `mango-agents-1.1.0/mango/modules/mqtt_module.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.1/mango/modules/rabbit_module.py` & `mango-agents-1.1.0/mango/modules/rabbit_module.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.1/mango/modules/zero_module.py` & `mango-agents-1.1.0/mango/modules/zero_module.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.1/mango/util/clock.py` & `mango-agents-1.1.0/mango/util/clock.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.1/mango/util/distributed_clock.py` & `mango-agents-1.1.0/mango/util/distributed_clock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import asyncio
 import logging
 
 from mango import Agent
-
+from .termination_detection import tasks_complete_or_sleeping
 logger = logging.getLogger(__name__)
 
 
 class ClockAgent(Agent):
     async def wait_all_done(self):
-        await self._context._container.inbox.join()
-        for ag in self._context._container._agents.values():  # type: Agent
-            await ag.inbox.join()  # make sure inbox of agent is empty and all messages are processed
-            await ag._scheduler.tasks_complete_or_sleeping()  # wait until agent is done with all tasks
+        await tasks_complete_or_sleeping(self._context._container)
 
 
 class DistributedClockManager(ClockAgent):
     def __init__(self, container, receiver_clock_addresses: list):
         super().__init__(container, "clock")
         self.receiver_clock_addresses = receiver_clock_addresses
         self.schedules = []
```

### Comparing `mango-agents-1.0.1/mango/util/scheduling.py` & `mango-agents-1.1.0/mango/util/scheduling.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,16 +134,18 @@
 
 
 class TimestampScheduledTask(ScheduledTask):
     """
     Timestamp based one-shot task. This task will get executed when a given unix timestamp is reached.
     """
 
-    def __init__(self, coroutine, timestamp: float, clock=None, on_stop=None):
-        super().__init__(clock, on_stop=on_stop)
+    def __init__(
+        self, coroutine, timestamp: float, clock=None, on_stop=None, observable=True
+    ):
+        super().__init__(clock, on_stop=on_stop, observable=observable)
         self._timestamp = timestamp
         self._coro = coroutine
 
     async def _wait(self, timestamp: float):
         sleep_future: asyncio.Future = self.clock.sleep(timestamp - self.clock.time)
         self.notify_sleeping()
         await sleep_future
@@ -156,16 +158,18 @@
 
 class AwaitingTask(ScheduledTask):
     """
     Awaiting task. This task will execute a given coroutine after another given coroutine has been awaited.
     Can be useful if you want to execute something after a Future has finished.
     """
 
-    def __init__(self, coroutine, awaited_coroutine, clock=None, on_stop=None):
-        super().__init__(clock, on_stop=on_stop)
+    def __init__(
+        self, coroutine, awaited_coroutine, clock=None, on_stop=None, observable=True
+    ):
+        super().__init__(clock, on_stop=on_stop, observable=observable)
         self._coroutine = coroutine
         self._awaited_coroutine = awaited_coroutine
 
     async def run(self):
         self.notify_sleeping()
         await self._awaited_coroutine
         self.notify_running()
@@ -173,28 +177,32 @@
 
 
 class InstantScheduledTask(TimestampScheduledTask):
     """
     One-shot task, which will get executed instantly.
     """
 
-    def __init__(self, coroutine, clock: Clock = None, on_stop=None):
+    def __init__(self, coroutine, clock: Clock = None, on_stop=None, observable=True):
         if clock is None:
             clock = AsyncioClock()
-        super().__init__(coroutine, clock.time, clock=clock, on_stop=on_stop)
+        super().__init__(
+            coroutine, clock.time, clock=clock, on_stop=on_stop, observable=observable
+        )
 
 
 class PeriodicScheduledTask(ScheduledTask):
     """
     Class for periodic scheduled tasks. It enables to create a task for an agent
     which will get executed periodically with a specified delay.
     """
 
-    def __init__(self, coroutine_func, delay, clock: Clock = None, on_stop=None):
-        super().__init__(clock, on_stop=on_stop)
+    def __init__(
+        self, coroutine_func, delay, clock: Clock = None, on_stop=None, observable=True
+    ):
+        super().__init__(clock, on_stop=on_stop, observable=observable)
 
         self._stopped = False
         self._coroutine_func = coroutine_func
         self._delay = delay
 
     async def run(self):
         while not self._stopped:
@@ -208,59 +216,68 @@
 class RecurrentScheduledTask(ScheduledTask):
     """
     Class for periodic scheduled tasks. It enables to create a task for an agent
     which will get executed periodically with a specified delay.
     """
 
     def __init__(
-        self, coroutine_func, recurrency: rrule, clock: Clock = None, on_stop=None
+        self,
+        coroutine_func,
+        recurrency: rrule,
+        clock: Clock = None,
+        on_stop=None,
+        observable=True,
     ):
-        super().__init__(clock, on_stop=on_stop)
+        super().__init__(clock, on_stop=on_stop, observable=observable)
         self._recurrency_rule = recurrency
         self._stopped = False
         self._coroutine_func = coroutine_func
 
     async def run(self):
         while not self._stopped:
             await self._coroutine_func()
             current_time = datetime.datetime.fromtimestamp(self.clock.time)
             after = self._recurrency_rule.after(current_time)
             # after can be None, if until or count was set on the rrule
             if after is None:
                 self._stopped = True
             else:
                 delay = (after - current_time).total_seconds()
-                await self.clock.sleep(delay)
+                sleep_future: asyncio.Future = self.clock.sleep(delay)
+                self.notify_sleeping()
+                await sleep_future
+                self.notify_running()
 
 
 class ConditionalTask(ScheduledTask):
     """Task which will get executed as soon as the given condition is fulfilled."""
 
     def __init__(
         self,
         coroutine,
         condition_func,
         lookup_delay=0.1,
         clock: Clock = None,
         on_stop=None,
+        observable=True,
     ):
-        super().__init__(clock=clock, on_stop=on_stop)
-
+        super().__init__(clock=clock, on_stop=on_stop, observable=observable)
+        assert coroutine is not None
         self._condition = condition_func
         self._coro = coroutine
         self._delay = lookup_delay
 
     async def run(self):
         while not self._condition():
             sleep_future: asyncio.Future = self.clock.sleep(self._delay)
             self.notify_sleeping()
             await sleep_future
             self.notify_running()
         return await self._coro
-    
+
 
 # process tasks
 
 
 class ScheduledProcessTask(ScheduledTask):
     # Mark class as task for an external process
 
@@ -269,27 +286,29 @@
     This is necessary due to the fact that not everything can be transferred to other processes i.e. coroutines are
     bound to the current event-loop resp the current thread, so they won't work in other processes.
     Furthermore, when using a ProcessTask you have to ensure, that the coroutine functions should not be bound to
     complex objects, meaning they should be static or bound to simple objects, which are transferable
     via pythons IPC implementation.
     """
 
-    def __init__(self, clock: Clock, on_stop=None):
+    def __init__(self, clock: Clock, on_stop=None, observable=False):
         if isinstance(clock, ExternalClock):
             raise ValueError("Process Tasks do currently not work with external clocks")
-        super().__init__(clock=clock, observable=False, on_stop=on_stop)
+        super().__init__(clock=clock, observable=observable, on_stop=on_stop)
 
 
 class TimestampScheduledProcessTask(TimestampScheduledTask, ScheduledProcessTask):
     """
     Timestamp based one-shot task.
     """
 
     def __init__(self, coroutine_creator, timestamp: float, clock=None, on_stop=None):
-        super().__init__(coroutine_creator, timestamp, clock, on_stop=on_stop)
+        super().__init__(
+            coroutine_creator, timestamp, clock, on_stop=on_stop, observable=False
+        )
 
     async def run(self):
         await self._wait(self._timestamp)
         return await self._coro()
 
 
 class AwaitingProcessTask(AwaitingTask, ScheduledProcessTask):
@@ -297,43 +316,52 @@
     Await a coroutine, then execute another.
     """
 
     def __init__(
         self, coroutine_creator, awaited_coroutine_creator, clock=None, on_stop=None
     ):
         super().__init__(
-            coroutine_creator, awaited_coroutine_creator, clock, on_stop=on_stop
+            coroutine_creator,
+            awaited_coroutine_creator,
+            clock,
+            on_stop=on_stop,
+            observable=False,
         )
 
     async def run(self):
         await self._awaited_coroutine()
         return await self._coroutine()
 
 
 class InstantScheduledProcessTask(TimestampScheduledProcessTask):
     """One-shot task, which will get executed instantly."""
 
     def __init__(self, coroutine_creator, clock: Clock = None, on_stop=None):
         if clock is None:
             clock = AsyncioClock()
         super().__init__(
-            coroutine_creator, timestamp=clock.time, clock=clock, on_stop=on_stop
+            coroutine_creator,
+            timestamp=clock.time,
+            clock=clock,
+            on_stop=on_stop,
         )
 
 
 class PeriodicScheduledProcessTask(PeriodicScheduledTask, ScheduledProcessTask):
     def __init__(self, coroutine_func, delay, clock: Clock = None, on_stop=None):
         super().__init__(coroutine_func, delay, clock, on_stop=on_stop)
 
 
 class RecurrentScheduledProcessTask(RecurrentScheduledTask, ScheduledProcessTask):
     def __init__(
         self, coroutine_func, recurrency: rrule, clock: Clock = None, on_stop=None
     ):
-        super().__init__(coroutine_func, recurrency, clock, on_stop=on_stop)
+        super().__init__(
+            coroutine_func, recurrency, clock, on_stop=on_stop, observable=False
+        )
 
 
 class ConditionalProcessTask(ConditionalTask, ScheduledProcessTask):
     """
     Task which will get executed as soon as the given condition is fulfilled.
     """
 
@@ -342,15 +370,20 @@
         coro_func,
         condition_func,
         lookup_delay=0.1,
         clock: Clock = None,
         on_stop=None,
     ):
         super().__init__(
-            coro_func, condition_func, lookup_delay, clock=clock, on_stop=on_stop
+            coro_func,
+            condition_func,
+            lookup_delay,
+            clock=clock,
+            on_stop=on_stop,
+            observable=False,
         )
 
     async def run(self):
         while not self._condition():
             await self.clock.sleep(self._delay)
         return await self._coro()
 
@@ -358,24 +391,32 @@
 def _create_asyncio_context():
     asyncio.set_event_loop(asyncio.new_event_loop())
 
 
 class Scheduler:
     """Scheduler for executing tasks."""
 
-    def __init__(self, clock: Clock = None, num_process_parallel=16):
+    def __init__(
+        self,
+        clock: Clock = None,
+        num_process_parallel=16,
+        suspendable=True,
+        observable=True,
+    ):
         # List of Tuples with asyncio.Future, ScheduledTask, Suspendable coro, Source
         self._scheduled_tasks: List[
             Tuple[ScheduledTask, asyncio.Future, Suspendable, Any]
         ] = []
         self.clock = clock if clock is not None else AsyncioClock()
         self._scheduled_process_tasks = []
         self._process_pool_exec = concurrent.futures.ProcessPoolExecutor(
             max_workers=num_process_parallel, initializer=_create_asyncio_context
         )
+        self._suspendable = suspendable
+        self._observable = observable
 
     @staticmethod
     def _run_task_in_p_context(task, suspend_event):
         try:
             coro = Suspendable(task.run(), ext_contr_event=suspend_event)
 
             return asyncio.get_event_loop().run_until_complete(coro)
@@ -396,19 +437,24 @@
         For scheduling options see the subclasses of ScheduledTask.
 
         :param task: task to be scheduled
         :type task: ScheduledTask
         :param src: creator of the task
         :type: Object
         """
-        susp_coro = Suspendable(task.run())
-        l_task = asyncio.ensure_future(susp_coro)
+        l_task = None
+        if self._suspendable:
+            coro = Suspendable(task.run())
+            l_task = asyncio.ensure_future(coro)
+        else:
+            coro = task.run()
+            l_task = asyncio.create_task(coro)
         l_task.add_done_callback(task.on_stop)
         l_task.add_done_callback(self._remove_task)
-        self._scheduled_tasks.append((task, l_task, susp_coro, src))
+        self._scheduled_tasks.append((task, l_task, coro, src))
         return l_task
 
     def schedule_timestamp_task(
         self, coroutine, timestamp: float, on_stop=None, src=None
     ):
         """Schedule a task at specified unix timestamp.
 
@@ -421,29 +467,33 @@
         """
         return self.schedule_task(
             TimestampScheduledTask(
                 coroutine=coroutine,
                 timestamp=timestamp,
                 clock=self.clock,
                 on_stop=on_stop,
+                observable=self._observable,
             ),
             src=src,
         )
 
     def schedule_instant_task(self, coroutine, on_stop=None, src=None):
         """Schedule an instantly executed task.
 
         :param coroutine: coroutine to be scheduled
         :type coroutine:
         :param src: creator of the task
         :type src: Object
         """
         return self.schedule_task(
             InstantScheduledTask(
-                coroutine=coroutine, clock=self.clock, on_stop=on_stop
+                coroutine=coroutine,
+                clock=self.clock,
+                on_stop=on_stop,
+                observable=self._observable,
             ),
             src=src,
         )
 
     def schedule_periodic_task(self, coroutine_func, delay, on_stop=None, src=None):
         """
         Schedule an open end periodically executed task.
@@ -456,14 +506,15 @@
         """
         return self.schedule_task(
             PeriodicScheduledTask(
                 coroutine_func=coroutine_func,
                 delay=delay,
                 clock=self.clock,
                 on_stop=on_stop,
+                observable=self._observable,
             ),
             src=src,
         )
 
     def schedule_recurrent_task(
         self, coroutine_func, recurrency, on_stop=None, src=None
     ):
@@ -478,14 +529,15 @@
         """
         return self.schedule_task(
             RecurrentScheduledTask(
                 coroutine_func=coroutine_func,
                 recurrency=recurrency,
                 clock=self.clock,
                 on_stop=on_stop,
+                observable=self._observable,
             ),
             src=src,
         )
 
     def schedule_conditional_task(
         self,
         coroutine,
@@ -508,14 +560,15 @@
         return self.schedule_task(
             ConditionalTask(
                 coroutine=coroutine,
                 condition_func=condition_func,
                 clock=self.clock,
                 lookup_delay=lookup_delay,
                 on_stop=on_stop,
+                observable=self._observable,
             ),
             src=src,
         )
 
     def schedule_awaiting_task(
         self, coroutine, awaited_coroutine, on_stop=None, src=None
     ):
@@ -530,14 +583,15 @@
         """
         return self.schedule_task(
             AwaitingTask(
                 coroutine=coroutine,
                 awaited_coroutine=awaited_coroutine,
                 clock=self.clock,
                 on_stop=on_stop,
+                observable=self._observable,
             ),
             src=src,
         )
 
     # conv. methods for process tasks
 
     def schedule_process_task(self, task: ScheduledProcessTask, src=None):
@@ -594,15 +648,18 @@
         Schedule an instantly executed task dispatched to another process.
         :param coroutine_creator: coroutine_creator to be scheduled
         :type coroutine_creator:
         :param src: creator of the task
         :type src: Object
         """
         return self.schedule_process_task(
-            InstantScheduledProcessTask(coroutine_creator=coroutine_creator), src=src
+            InstantScheduledProcessTask(
+                coroutine_creator=coroutine_creator, on_stop=on_stop
+            ),
+            src=src,
         )
 
     def schedule_periodic_process_task(
         self, coroutine_creator, delay, on_stop=None, src=None
     ):
         """Schedule an open end periodically executed task dispatched to another process.
 
@@ -679,27 +736,33 @@
 
     def suspend(self, given_src):
         """Suspend a set of tasks triggered by the given src object.
 
         :param given_src: the src object
         :type given_src: object
         """
+        if not self._suspendable:
+            raise Exception("The scheduler is configured as non-suspendable!")
+
         for _, _, coro, src in self._scheduled_tasks:
             if src == given_src and coro is not None:
                 coro.suspend()
         for _, _, event, src in self._scheduled_process_tasks:
             if src == given_src and event is not None:
                 event.clear()
 
     def resume(self, given_src):
         """Resume a set of tasks triggered by the given src object.
 
         :param given_src: the src object
         :type given_src: object
         """
+        if not self._suspendable:
+            raise Exception("The scheduler is configured as non-suspendable!")
+
         for _, _, coro, src in self._scheduled_tasks:
             if src == given_src and coro is not None:
                 coro.resume()
         for _, _, event, src in self._scheduled_process_tasks:
             if src == given_src and event is not None:
                 event.set()
```

### Comparing `mango-agents-1.0.1/mango_agents.egg-info/PKG-INFO` & `mango-agents-1.1.0/mango_agents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-agents
-Version: 1.0.1
+Version: 1.1.0
 Summary: Modular Python Agent Framework
 Author: mango Team
 Author-email: mango@offis.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mango-agents-1.0.1/mango_agents.egg-info/SOURCES.txt` & `mango-agents-1.1.0/mango_agents.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -20,13 +20,15 @@
 mango/modules/base_module.py
 mango/modules/mqtt_module.py
 mango/modules/rabbit_module.py
 mango/modules/zero_module.py
 mango/util/__init__.py
 mango/util/clock.py
 mango/util/distributed_clock.py
+mango/util/multiprocessing.py
 mango/util/scheduling.py
+mango/util/termination_detection.py
 mango_agents.egg-info/PKG-INFO
 mango_agents.egg-info/SOURCES.txt
 mango_agents.egg-info/dependency_links.txt
 mango_agents.egg-info/requires.txt
 mango_agents.egg-info/top_level.txt
```

### Comparing `mango-agents-1.0.1/setup.py` & `mango-agents-1.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,25 +8,29 @@
 import os
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
-NAME = 'mango-agents'
-DESCRIPTION = 'Modular Python Agent Framework'
-URL = 'https://gitlab.com/mango-agents/mango'
-EMAIL = 'mango@offis.de'
-AUTHOR = 'mango Team'
-REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.0.1'
+NAME = "mango-agents"
+DESCRIPTION = "Modular Python Agent Framework"
+URL = "https://gitlab.com/mango-agents/mango"
+EMAIL = "mango@offis.de"
+AUTHOR = "mango Team"
+REQUIRES_PYTHON = ">=3.7.0"
+VERSION = "1.1.0"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'paho-mqtt==1.5.1', 'protobuf==3.19.1', 'python-dateutil==2.8.2'
+    "paho-mqtt==1.5.1",
+    "python-dateutil>=2.8.2",
+    "dill>=0.3.6",
+    "msgspec>=0.14.2",
+    "protobuf>=3.20.3",
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
@@ -36,102 +40,99 @@
 # If you do change the License, remember to change the Trove Classifier for that!
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
-    with io.open(os.path.join(here, 'readme.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
+    with io.open(os.path.join(here, "readme.md"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 # Load the package's __version__.py module as a dictionary.
 about = {}
 if not VERSION:
     project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+    with open(os.path.join(here, project_slug, "__version__.py")) as f:
         exec(f.read(), about)
 else:
-    about['__version__'] = VERSION
+    about["__version__"] = VERSION
 
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
-    description = 'Build and publish the package.'
+    description = "Build and publish the package."
     user_options = []
 
     @staticmethod
     def status(s):
         """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
+        print("\033[1m{0}\033[0m".format(s))
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
+            self.status("Removing previous builds…")
+            rmtree(os.path.join(here, "dist"))
         except OSError:
             pass
 
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(
-            sys.executable))
-
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
+        self.status("Building Source and Wheel (universal) distribution…")
+        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
+
+        self.status("Uploading the package to PyPI via Twine…")
+        os.system("twine upload dist/*")
+
+        self.status("Pushing git tags…")
+        os.system("git tag v{0}".format(about["__version__"]))
+        os.system("git push --tags")
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version=about['__version__'],
+    version=about["__version__"],
     description=DESCRIPTION,
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     # url=URL,
-    packages=find_packages(
-        exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
-
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
-    license='MIT',
+    license="MIT",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy'
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
     ],
     # $ setup.py publish support.
     cmdclass={
-        'upload': UploadCommand,
+        "upload": UploadCommand,
     },
 )
```

