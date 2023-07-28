# Comparing `tmp/bus_station-7.1.0.tar.gz` & `tmp/bus_station-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_station-7.1.0.tar", max compression
+gzip compressed data, was "bus_station-7.2.0.tar", max compression
```

## Comparing `bus_station-7.1.0.tar` & `bus_station-7.2.0.tar`

### file list

```diff
@@ -1,151 +1,151 @@
--rw-r--r--   0        0        0       48 2023-07-28 09:14:48.927372 bus_station-7.1.0/README.md
--rw-r--r--   0        0        0      954 2023-07-28 09:16:26.693163 bus_station-7.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/bus_stop/__init__.py
--rw-r--r--   0        0        0      937 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/bus_stop/bus_stop.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/bus_stop/registration/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/bus_stop/registration/address/__init__.py
--rw-r--r--   0        0        0      214 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/bus_stop/registration/address/address_not_found_for_passenger.py
--rw-r--r--   0        0        0      653 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/bus_stop/registration/address/bus_stop_address_registry.py
--rw-r--r--   0        0        0     1299 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py
--rw-r--r--   0        0        0     1597 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/bus_stop/registration/bus_stop_registry.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus/asynchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus/asynchronous/distributed/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py
--rw-r--r--   0        0        0      889 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py
--rw-r--r--   0        0        0     1237 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py
--rw-r--r--   0        0        0      258 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus/command_bus.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus/synchronous/distributed/__init__.py
--rw-r--r--   0        0        0     1880 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py
--rw-r--r--   0        0        0     1753 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py
--rw-r--r--   0        0        0     1128 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     1185 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py
--rw-r--r--   0        0        0     2606 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py
--rw-r--r--   0        0        0     1715 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py
--rw-r--r--   0        0        0     1125 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py
--rw-r--r--   0        0        0      253 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/command.py
--rw-r--r--   0        0        0      292 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/command_execution_failed.py
--rw-r--r--   0        0        0      564 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/command_handler.py
--rw-r--r--   0        0        0      227 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/command_handler_not_found.py
--rw-r--r--   0        0        0      973 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/command_handler_registry.py
--rw-r--r--   0        0        0      233 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/handler_not_found_for_command.py
--rw-r--r--   0        0        0      725 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/json_rpc_command_server.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.927372 bus_station-7.1.0/src/bus_station/command_terminal/middleware/__init__.py
--rw-r--r--   0        0        0      607 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/command_terminal/middleware/command_middleware.py
--rw-r--r--   0        0        0     1078 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/command_terminal/middleware/command_middleware_receiver.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/command_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1070 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py
--rw-r--r--   0        0        0     1039 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py
--rw-r--r--   0        0        0      890 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py
--rw-r--r--   0        0        0      712 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/command_terminal/rpyc_command_server.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/bus/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/bus/asynchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/bus/asynchronous/distributed/__init__.py
--rw-r--r--   0        0        0     1247 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py
--rw-r--r--   0        0        0     1212 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py
--rw-r--r--   0        0        0      984 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py
--rw-r--r--   0        0        0      246 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/bus/event_bus.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0      872 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     3056 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py
--rw-r--r--   0        0        0     1625 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py
--rw-r--r--   0        0        0      249 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/event.py
--rw-r--r--   0        0        0      552 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/event_consumer.py
--rw-r--r--   0        0        0      221 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/event_consumer_not_found.py
--rw-r--r--   0        0        0      742 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/event_consumer_registry.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/middleware/__init__.py
--rw-r--r--   0        0        0      590 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/middleware/event_middleware.py
--rw-r--r--   0        0        0     1049 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/middleware/event_middleware_receiver.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1038 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py
--rw-r--r--   0        0        0     1012 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py
--rw-r--r--   0        0        0      864 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/__init__.py
--rw-r--r--   0        0        0     1440 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/memory_queue_passenger_worker.py
--rw-r--r--   0        0        0     2319 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/passenger.py
--rw-r--r--   0        0        0     2042 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/passenger_kombu_consumer.py
--rw-r--r--   0        0        0     2166 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/passenger_mapper.py
--rw-r--r--   0        0        0       76 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/passenger_middleware.py
--rw-r--r--   0        0        0      645 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/passenger_registry.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/reception/__init__.py
--rw-r--r--   0        0        0     1386 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/reception/passenger_middleware_receiver.py
--rw-r--r--   0        0        0      792 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/reception/passenger_receiver.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/serialization/__init__.py
--rw-r--r--   0        0        0      347 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/serialization/passenger_deserialization_error.py
--rw-r--r--   0        0        0      321 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/serialization/passenger_deserializer.py
--rw-r--r--   0        0        0     1016 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/serialization/passenger_json_deserializer.py
--rw-r--r--   0        0        0      822 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/serialization/passenger_json_serializer.py
--rw-r--r--   0        0        0      241 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/passengers/serialization/passenger_serializer.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/bus/__init__.py
--rw-r--r--   0        0        0      323 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/bus/query_bus.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/bus/synchronous/distributed/__init__.py
--rw-r--r--   0        0        0     2256 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py
--rw-r--r--   0        0        0     2165 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py
--rw-r--r--   0        0        0     1127 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     1103 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py
--rw-r--r--   0        0        0     1079 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py
--rw-r--r--   0        0        0      219 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/handler_not_found_for_query.py
--rw-r--r--   0        0        0     1483 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/json_rpc_query_server.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/middleware/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1261 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py
--rw-r--r--   0        0        0     1178 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py
--rw-r--r--   0        0        0     1227 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py
--rw-r--r--   0        0        0      726 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/middleware/query_middleware.py
--rw-r--r--   0        0        0     1286 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/middleware/query_middleware_receiver.py
--rw-r--r--   0        0        0      249 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/query.py
--rw-r--r--   0        0        0      273 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/query_execution_failed.py
--rw-r--r--   0        0        0      625 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/query_handler.py
--rw-r--r--   0        0        0      215 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/query_handler_not_found.py
--rw-r--r--   0        0        0      926 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/query_handler_registry.py
--rw-r--r--   0        0        0      138 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/query_response.py
--rw-r--r--   0        0        0     1442 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/rpyc_query_server.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/serialization/__init__.py
--rw-r--r--   0        0        0      282 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/serialization/query_response_deserializer.py
--rw-r--r--   0        0        0      465 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/serialization/query_response_json_deserializer.py
--rw-r--r--   0        0        0      390 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/serialization/query_response_json_serializer.py
--rw-r--r--   0        0        0      267 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/query_terminal/serialization/query_response_serializer.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/broker_connection/__init__.py
--rw-r--r--   0        0        0      352 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/broker_connection/broker_connection_type.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/__init__.py
--rw-r--r--   0        0        0      176 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/connection_parameters.py
--rw-r--r--   0        0        0     1249 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py
--rw-r--r--   0        0        0      587 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/bus.py
--rw-r--r--   0        0        0      438 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/context.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/engine/__init__.py
--rw-r--r--   0        0        0      181 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/engine/engine.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/engine/runner/__init__.py
--rw-r--r--   0        0        0      436 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/engine/runner/engine_runner.py
--rw-r--r--   0        0        0      805 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py
--rw-r--r--   0        0        0      241 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/engine/runner/self_process_engine_runner.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/factories/__init__.py
--rw-r--r--   0        0        0      381 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/factories/kombu_connection_factory.py
--rw-r--r--   0        0        0      545 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/factories/memory_queue_factory.py
--rw-r--r--   0        0        0     2493 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/json_rpc_server.py
--rw-r--r--   0        0        0      956 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/kafka_topic_creator.py
--rw-r--r--   0        0        0     2037 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/shared_terminal/rpyc_server.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/builders/__init__.py
--rw-r--r--   0        0        0     2570 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/builders/kafka_passenger_tracker_builder.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/models/__init__.py
--rw-r--r--   0        0        0      185 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/models/command_tracking.py
--rw-r--r--   0        0        0      183 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/models/event_tracking.py
--rw-r--r--   0        0        0      950 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py
--rw-r--r--   0        0        0      347 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/models/passenger_tracking.py
--rw-r--r--   0        0        0      744 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py
--rw-r--r--   0        0        0      297 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/models/passenger_tracking_serializer.py
--rw-r--r--   0        0        0      281 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/models/query_tracking.py
--rw-r--r--   0        0        0        0 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/trackers/__init__.py
--rw-r--r--   0        0        0     1400 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py
--rw-r--r--   0        0        0     2483 2023-07-28 09:14:48.931372 bus_station-7.1.0/src/bus_station/tracking_terminal/trackers/passenger_tracker.py
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 bus_station-7.1.0/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-07-28 10:31:51.082624 bus_station-7.2.0/README.md
+-rw-r--r--   0        0        0     1038 2023-07-28 10:33:47.062455 bus_station-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/bus_stop/__init__.py
+-rw-r--r--   0        0        0      937 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/bus_stop/bus_stop.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/bus_stop/registration/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/bus_stop/registration/address/__init__.py
+-rw-r--r--   0        0        0      214 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/bus_stop/registration/address/address_not_found_for_passenger.py
+-rw-r--r--   0        0        0      653 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/bus_stop/registration/address/bus_stop_address_registry.py
+-rw-r--r--   0        0        0     1299 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py
+-rw-r--r--   0        0        0     1597 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/bus_stop/registration/bus_stop_registry.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/command_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/command_terminal/bus/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/command_terminal/bus/asynchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/command_terminal/bus/asynchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py
+-rw-r--r--   0        0        0      889 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py
+-rw-r--r--   0        0        0     1237 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py
+-rw-r--r--   0        0        0      258 2023-07-28 10:31:51.082624 bus_station-7.2.0/src/bus_station/command_terminal/bus/command_bus.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/bus/synchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     1880 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py
+-rw-r--r--   0        0        0     1753 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py
+-rw-r--r--   0        0        0     1128 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     1185 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py
+-rw-r--r--   0        0        0     2606 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py
+-rw-r--r--   0        0        0     1715 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py
+-rw-r--r--   0        0        0     1125 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py
+-rw-r--r--   0        0        0      253 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/command.py
+-rw-r--r--   0        0        0      292 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/command_execution_failed.py
+-rw-r--r--   0        0        0      564 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/command_handler.py
+-rw-r--r--   0        0        0      227 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/command_handler_not_found.py
+-rw-r--r--   0        0        0      973 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/command_handler_registry.py
+-rw-r--r--   0        0        0      233 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/handler_not_found_for_command.py
+-rw-r--r--   0        0        0      725 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/json_rpc_command_server.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0      607 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/middleware/command_middleware.py
+-rw-r--r--   0        0        0     1078 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/middleware/command_middleware_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1070 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py
+-rw-r--r--   0        0        0     1039 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py
+-rw-r--r--   0        0        0      890 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py
+-rw-r--r--   0        0        0      712 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/command_terminal/rpyc_command_server.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/bus/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/bus/asynchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/bus/asynchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     1247 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py
+-rw-r--r--   0        0        0     1212 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py
+-rw-r--r--   0        0        0      984 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py
+-rw-r--r--   0        0        0      246 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/bus/event_bus.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0      872 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     3056 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py
+-rw-r--r--   0        0        0     1625 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py
+-rw-r--r--   0        0        0      249 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/event.py
+-rw-r--r--   0        0        0      552 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/event_consumer.py
+-rw-r--r--   0        0        0      221 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/event_consumer_not_found.py
+-rw-r--r--   0        0        0      742 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/event_consumer_registry.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/middleware/event_middleware.py
+-rw-r--r--   0        0        0     1049 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/middleware/event_middleware_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1038 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py
+-rw-r--r--   0        0        0     1012 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py
+-rw-r--r--   0        0        0      864 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/__init__.py
+-rw-r--r--   0        0        0     1440 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/memory_queue_passenger_worker.py
+-rw-r--r--   0        0        0     2319 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/passenger.py
+-rw-r--r--   0        0        0     2042 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/passenger_kombu_consumer.py
+-rw-r--r--   0        0        0     2166 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/passenger_mapper.py
+-rw-r--r--   0        0        0       76 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/passenger_middleware.py
+-rw-r--r--   0        0        0      645 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/passenger_registry.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/reception/__init__.py
+-rw-r--r--   0        0        0     1386 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/reception/passenger_middleware_receiver.py
+-rw-r--r--   0        0        0      792 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/reception/passenger_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/serialization/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/serialization/passenger_deserialization_error.py
+-rw-r--r--   0        0        0      321 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/serialization/passenger_deserializer.py
+-rw-r--r--   0        0        0     1016 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/serialization/passenger_json_deserializer.py
+-rw-r--r--   0        0        0      822 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/serialization/passenger_json_serializer.py
+-rw-r--r--   0        0        0      241 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/passengers/serialization/passenger_serializer.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/bus/__init__.py
+-rw-r--r--   0        0        0      323 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/bus/query_bus.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/bus/synchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     2256 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py
+-rw-r--r--   0        0        0     2165 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py
+-rw-r--r--   0        0        0     1127 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     1103 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py
+-rw-r--r--   0        0        0     1079 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py
+-rw-r--r--   0        0        0      219 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/handler_not_found_for_query.py
+-rw-r--r--   0        0        0     1483 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/json_rpc_query_server.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1261 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py
+-rw-r--r--   0        0        0     1178 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py
+-rw-r--r--   0        0        0     1227 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py
+-rw-r--r--   0        0        0      726 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/middleware/query_middleware.py
+-rw-r--r--   0        0        0     1286 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/middleware/query_middleware_receiver.py
+-rw-r--r--   0        0        0      249 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/query.py
+-rw-r--r--   0        0        0      273 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/query_execution_failed.py
+-rw-r--r--   0        0        0      625 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/query_handler.py
+-rw-r--r--   0        0        0      215 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/query_handler_not_found.py
+-rw-r--r--   0        0        0      926 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/query_handler_registry.py
+-rw-r--r--   0        0        0      138 2023-07-28 10:31:51.086624 bus_station-7.2.0/src/bus_station/query_terminal/query_response.py
+-rw-r--r--   0        0        0     1442 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/query_terminal/rpyc_query_server.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/query_terminal/serialization/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/query_terminal/serialization/query_response_deserializer.py
+-rw-r--r--   0        0        0      465 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/query_terminal/serialization/query_response_json_deserializer.py
+-rw-r--r--   0        0        0      390 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/query_terminal/serialization/query_response_json_serializer.py
+-rw-r--r--   0        0        0      267 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/query_terminal/serialization/query_response_serializer.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/broker_connection/__init__.py
+-rw-r--r--   0        0        0      352 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/broker_connection/broker_connection_type.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/__init__.py
+-rw-r--r--   0        0        0      176 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/connection_parameters.py
+-rw-r--r--   0        0        0     1249 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py
+-rw-r--r--   0        0        0      587 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/bus.py
+-rw-r--r--   0        0        0      438 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/context.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/engine/__init__.py
+-rw-r--r--   0        0        0      181 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/engine/engine.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/engine/runner/__init__.py
+-rw-r--r--   0        0        0      436 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/engine/runner/engine_runner.py
+-rw-r--r--   0        0        0      805 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py
+-rw-r--r--   0        0        0      241 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/engine/runner/self_process_engine_runner.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/factories/__init__.py
+-rw-r--r--   0        0        0      381 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/factories/kombu_connection_factory.py
+-rw-r--r--   0        0        0      545 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/factories/memory_queue_factory.py
+-rw-r--r--   0        0        0     2493 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/json_rpc_server.py
+-rw-r--r--   0        0        0      956 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/kafka_topic_creator.py
+-rw-r--r--   0        0        0     2037 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/shared_terminal/rpyc_server.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/builders/__init__.py
+-rw-r--r--   0        0        0     2570 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/builders/kafka_passenger_tracker_builder.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/models/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/models/command_tracking.py
+-rw-r--r--   0        0        0      183 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/models/event_tracking.py
+-rw-r--r--   0        0        0      950 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py
+-rw-r--r--   0        0        0      347 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/models/passenger_tracking.py
+-rw-r--r--   0        0        0      744 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py
+-rw-r--r--   0        0        0      297 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/models/passenger_tracking_serializer.py
+-rw-r--r--   0        0        0      281 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/models/query_tracking.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/trackers/__init__.py
+-rw-r--r--   0        0        0     1400 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py
+-rw-r--r--   0        0        0     2483 2023-07-28 10:31:51.090624 bus_station-7.2.0/src/bus_station/tracking_terminal/trackers/passenger_tracker.py
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 bus_station-7.2.0/PKG-INFO
```

### Comparing `bus_station-7.1.0/pyproject.toml` & `bus_station-7.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 [tool.poetry]
 name = "bus-station"
-version = "7.1.0"
+version = "7.2.0"
 description = "A python bus station"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 
 [tool.poetry.dependencies]
 python = "~=3.10.0"
 kombu = "5.2.2"
 redis = "4.4.4"
 rpyc = "^5.3.1"
 jsonrpcserver = "^5.0.9"
 jsonrpcclient = "^4.0.3"
 requests = "^2.27.1"
-confluent-kafka = "^2.1.1"
+confluent-kafka = { version = "^2.1.1", optional = true }
 freezegun = "^1.2.2"
 
 [tool.poetry.dev-dependencies]
 black = "22.1.0"
 coverage = "5.3"
 flake8 = "3.8.4"
 pyre-check = "0.9.18"
 tox = "3.20.1"
 psycopg2 = "2.9.3"
 isort = "5.10.1"
 commitizen = "3.3.0"
 
+[tool.poetry.extras]
+tracking = ["confluent-kafka"]
+
 [tool.black]
 line-length = 120
 target-version = ['py310']
 exclude = '''
 /(
   | \.git
   | \.tox
@@ -39,15 +42,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "7.1.0"
+version = "7.2.0"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `bus_station-7.1.0/src/bus_station/bus_stop/bus_stop.py` & `bus_station-7.2.0/src/bus_station/bus_stop/bus_stop.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/bus_stop/registration/address/bus_stop_address_registry.py` & `bus_station-7.2.0/src/bus_station/bus_stop/registration/address/bus_stop_address_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py` & `bus_station-7.2.0/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/bus_stop/registration/bus_stop_registry.py` & `bus_station-7.2.0/src/bus_station/bus_stop/registration/bus_stop_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py` & `bus_station-7.2.0/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py` & `bus_station-7.2.0/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py` & `bus_station-7.2.0/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py` & `bus_station-7.2.0/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py` & `bus_station-7.2.0/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py` & `bus_station-7.2.0/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py` & `bus_station-7.2.0/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py` & `bus_station-7.2.0/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py` & `bus_station-7.2.0/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py` & `bus_station-7.2.0/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/command_handler.py` & `bus_station-7.2.0/src/bus_station/command_terminal/command_handler.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/command_handler_registry.py` & `bus_station-7.2.0/src/bus_station/command_terminal/command_handler_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/json_rpc_command_server.py` & `bus_station-7.2.0/src/bus_station/command_terminal/json_rpc_command_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/middleware/command_middleware.py` & `bus_station-7.2.0/src/bus_station/command_terminal/middleware/command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/middleware/command_middleware_receiver.py` & `bus_station-7.2.0/src/bus_station/command_terminal/middleware/command_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py` & `bus_station-7.2.0/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py` & `bus_station-7.2.0/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py` & `bus_station-7.2.0/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/command_terminal/rpyc_command_server.py` & `bus_station-7.2.0/src/bus_station/command_terminal/rpyc_command_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py` & `bus_station-7.2.0/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py` & `bus_station-7.2.0/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py` & `bus_station-7.2.0/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py` & `bus_station-7.2.0/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py` & `bus_station-7.2.0/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py` & `bus_station-7.2.0/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/event_consumer.py` & `bus_station-7.2.0/src/bus_station/event_terminal/event_consumer.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/event_consumer_registry.py` & `bus_station-7.2.0/src/bus_station/event_terminal/event_consumer_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/middleware/event_middleware.py` & `bus_station-7.2.0/src/bus_station/event_terminal/middleware/event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/middleware/event_middleware_receiver.py` & `bus_station-7.2.0/src/bus_station/event_terminal/middleware/event_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py` & `bus_station-7.2.0/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py` & `bus_station-7.2.0/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py` & `bus_station-7.2.0/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/passengers/memory_queue_passenger_worker.py` & `bus_station-7.2.0/src/bus_station/passengers/memory_queue_passenger_worker.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/passengers/passenger.py` & `bus_station-7.2.0/src/bus_station/passengers/passenger.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/passengers/passenger_kombu_consumer.py` & `bus_station-7.2.0/src/bus_station/passengers/passenger_kombu_consumer.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/passengers/passenger_mapper.py` & `bus_station-7.2.0/src/bus_station/passengers/passenger_mapper.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/passengers/passenger_registry.py` & `bus_station-7.2.0/src/bus_station/passengers/passenger_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/passengers/reception/passenger_middleware_receiver.py` & `bus_station-7.2.0/src/bus_station/passengers/reception/passenger_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/passengers/reception/passenger_receiver.py` & `bus_station-7.2.0/src/bus_station/passengers/reception/passenger_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/passengers/serialization/passenger_json_deserializer.py` & `bus_station-7.2.0/src/bus_station/passengers/serialization/passenger_json_deserializer.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/passengers/serialization/passenger_json_serializer.py` & `bus_station-7.2.0/src/bus_station/passengers/serialization/passenger_json_serializer.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py` & `bus_station-7.2.0/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py` & `bus_station-7.2.0/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py` & `bus_station-7.2.0/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py` & `bus_station-7.2.0/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py` & `bus_station-7.2.0/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/json_rpc_query_server.py` & `bus_station-7.2.0/src/bus_station/query_terminal/json_rpc_query_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py` & `bus_station-7.2.0/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py` & `bus_station-7.2.0/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py` & `bus_station-7.2.0/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/middleware/query_middleware.py` & `bus_station-7.2.0/src/bus_station/query_terminal/middleware/query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/middleware/query_middleware_receiver.py` & `bus_station-7.2.0/src/bus_station/query_terminal/middleware/query_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/query_handler.py` & `bus_station-7.2.0/src/bus_station/query_terminal/query_handler.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/query_handler_registry.py` & `bus_station-7.2.0/src/bus_station/query_terminal/query_handler_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/query_terminal/rpyc_query_server.py` & `bus_station-7.2.0/src/bus_station/query_terminal/rpyc_query_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py` & `bus_station-7.2.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/shared_terminal/bus.py` & `bus_station-7.2.0/src/bus_station/shared_terminal/bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py` & `bus_station-7.2.0/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/shared_terminal/factories/memory_queue_factory.py` & `bus_station-7.2.0/src/bus_station/shared_terminal/factories/memory_queue_factory.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/shared_terminal/json_rpc_server.py` & `bus_station-7.2.0/src/bus_station/shared_terminal/json_rpc_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/shared_terminal/kafka_topic_creator.py` & `bus_station-7.2.0/src/bus_station/shared_terminal/kafka_topic_creator.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/shared_terminal/rpyc_server.py` & `bus_station-7.2.0/src/bus_station/shared_terminal/rpyc_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/tracking_terminal/builders/kafka_passenger_tracker_builder.py` & `bus_station-7.2.0/src/bus_station/tracking_terminal/builders/kafka_passenger_tracker_builder.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py` & `bus_station-7.2.0/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py` & `bus_station-7.2.0/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py` & `bus_station-7.2.0/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py`

 * *Files identical despite different names*

### Comparing `bus_station-7.1.0/src/bus_station/tracking_terminal/trackers/passenger_tracker.py` & `bus_station-7.2.0/src/bus_station/tracking_terminal/trackers/passenger_tracker.py`

 * *Files identical despite different names*

