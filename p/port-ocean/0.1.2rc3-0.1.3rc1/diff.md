# Comparing `tmp/port_ocean-0.1.2rc3.tar.gz` & `tmp/port_ocean-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.2rc3.tar", max compression
+gzip compressed data, was "port_ocean-0.1.3rc1.tar", max compression
```

## Comparing `port_ocean-0.1.2rc3.tar` & `port_ocean-0.1.3rc1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0    11357 2023-07-26 19:43:37.416559 port_ocean-0.1.2rc3/LICENSE
--rw-r--r--   0        0        0     4639 2023-07-26 19:43:37.416559 port_ocean-0.1.2rc3/README.md
--rw-r--r--   0        0        0      270 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/__init__.py
--rw-r--r--   0        0        0      328 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cli.py
--rw-r--r--   0        0        0      278 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/__init__.py
--rw-r--r--   0        0        0     1134 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/list_integrations.py
--rw-r--r--   0        0        0     1057 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/main.py
--rw-r--r--   0        0        0     1710 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/new.py
--rw-r--r--   0        0        0     2306 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/pull.py
--rw-r--r--   0        0        0     1537 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/sail.py
--rw-r--r--   0        0        0      536 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/commands/version.py
--rw-r--r--   0        0        0      429 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       42 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0       12 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
--rw-r--r--   0        0        0      388 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
--rw-r--r--   0        0        0      292 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      449 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1680 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      655 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       12 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
--rw-r--r--   0        0        0      898 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
--rw-r--r--   0        0        0       65 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1920 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0       54 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/cli/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2563 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2309 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     2928 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/blueprints.py
--rw-r--r--   0        0        0     5623 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3909 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      781 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2701 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/config/base.py
--rw-r--r--   0        0        0     1259 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/config/dynamic.py
--rw-r--r--   0        0        0     1197 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     4147 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/context/event.py
--rw-r--r--   0        0        0     4286 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/base.py
--rw-r--r--   0        0        0      607 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/__init__.py
--rw-r--r--   0        0        0      580 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/base.py
--rw-r--r--   0        0        0     2555 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/factory.py
--rw-r--r--   0        0        0     1165 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/http/event_listener.py
--rw-r--r--   0        0        0     3128 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/kafka/event_listener.py
--rw-r--r--   0        0        0     1867 2023-07-26 19:43:37.428559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/polling/event_listener.py
--rw-r--r--   0        0        0     2799 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/event_listener/polling/utils.py
--rw-r--r--   0        0        0      716 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/__init__.py
--rw-r--r--   0        0        0      869 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/base.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/__init__.py
--rw-r--r--   0        0        0     7977 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/applier.py
--rw-r--r--   0        0        0     1339 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
--rw-r--r--   0        0        0      988 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     1392 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entity_processor/__init__.py
--rw-r--r--   0        0        0      955 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entity_processor/base.py
--rw-r--r--   0        0        0     2685 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      396 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1810 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     1912 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      698 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2569 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0    11843 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0     1683 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/utils.py
--rw-r--r--   0        0        0     1368 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/models.py
--rw-r--r--   0        0        0      781 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/ocean_types.py
--rw-r--r--   0        0        0     1957 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      532 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      407 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/exceptions/port_defaults.py
--rw-r--r--   0        0        0      554 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2475 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/middlewares.py
--rw-r--r--   0        0        0     2266 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/ocean.py
--rw-r--r--   0        0        0     7164 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/port_defaults.py
--rw-r--r--   0        0        0        0 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/py.typed
--rw-r--r--   0        0        0     2837 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/run.py
--rw-r--r--   0        0        0     1007 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/port_ocean/utils.py
--rw-r--r--   0        0        0     3461 2023-07-26 19:43:37.432559 port_ocean-0.1.2rc3/pyproject.toml
--rw-r--r--   0        0        0     6359 1970-01-01 00:00:00.000000 port_ocean-0.1.2rc3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-28 12:56:59.106535 port_ocean-0.1.3rc1/LICENSE
+-rw-r--r--   0        0        0     4639 2023-07-28 12:56:59.106535 port_ocean-0.1.3rc1/README.md
+-rw-r--r--   0        0        0      270 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/__init__.py
+-rw-r--r--   0        0        0      328 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0      278 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1134 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/commands/list_integrations.py
+-rw-r--r--   0        0        0     1057 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/commands/main.py
+-rw-r--r--   0        0        0     1710 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/commands/new.py
+-rw-r--r--   0        0        0     2306 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/commands/pull.py
+-rw-r--r--   0        0        0     1534 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/commands/sail.py
+-rw-r--r--   0        0        0      536 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/commands/version.py
+-rw-r--r--   0        0        0      429 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0       12 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
+-rw-r--r--   0        0        0      388 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      292 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      449 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1680 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      655 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
+-rw-r--r--   0        0        0      898 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       65 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1920 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/cli/utils.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2563 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2309 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     2928 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/clients/port/mixins/blueprints.py
+-rw-r--r--   0        0        0     5623 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3909 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      781 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     3541 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1259 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0     1231 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/config/settings.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     4147 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4283 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/base.py
+-rw-r--r--   0        0        0      607 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0      580 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     2555 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0     1165 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/event_listener/http/event_listener.py
+-rw-r--r--   0        0        0     3349 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/event_listener/kafka/event_listener.py
+-rw-r--r--   0        0        0     1867 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/event_listener/polling/event_listener.py
+-rw-r--r--   0        0        0     2799 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/event_listener/polling/utils.py
+-rw-r--r--   0        0        0      716 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0      869 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7977 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1339 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0      988 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0      955 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     2685 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1810 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     1912 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      698 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2569 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0    11843 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0     1683 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/integrations/mixins/utils.py
+-rw-r--r--   0        0        0     1368 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/models.py
+-rw-r--r--   0        0        0      781 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/ocean_types.py
+-rw-r--r--   0        0        0     1957 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      532 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      407 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/exceptions/port_defaults.py
+-rw-r--r--   0        0        0      551 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     2263 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/ocean.py
+-rw-r--r--   0        0        0     7161 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/port_defaults.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/py.typed
+-rw-r--r--   0        0        0     2834 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/run.py
+-rw-r--r--   0        0        0     1007 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/port_ocean/utils.py
+-rw-r--r--   0        0        0     3461 2023-07-28 12:56:59.118535 port_ocean-0.1.3rc1/pyproject.toml
+-rw-r--r--   0        0        0     6359 1970-01-01 00:00:00.000000 port_ocean-0.1.3rc1/PKG-INFO
```

### Comparing `port_ocean-0.1.2rc3/LICENSE` & `port_ocean-0.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/README.md` & `port_ocean-0.1.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/cli/commands/list_integrations.py` & `port_ocean-0.1.3rc1/port_ocean/cli/commands/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/cli/commands/main.py` & `port_ocean-0.1.3rc1/port_ocean/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/cli/commands/new.py` & `port_ocean-0.1.3rc1/port_ocean/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/cli/commands/pull.py` & `port_ocean-0.1.3rc1/port_ocean/cli/commands/pull.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/cli/commands/sail.py` & `port_ocean-0.1.3rc1/port_ocean/cli/commands/sail.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import click
 
 from port_ocean.cli.commands.main import cli_start, print_logo, console
-from port_ocean.config.integration import LogLevelType
+from port_ocean.config.settings import LogLevelType
 
 
 @cli_start.command()
 @click.argument("path", default=".", type=click.Path(exists=True))
 @click.option(
     "-l",
     "--log-level",
```

### Comparing `port_ocean-0.1.2rc3/port_ocean/cli/commands/version.py` & `port_ocean-0.1.3rc1/port_ocean/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md` & `port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml` & `port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.3rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.3rc1/port_ocean/clients/port/authentication.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/clients/port/client.py` & `port_ocean-0.1.3rc1/port_ocean/clients/port/client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/blueprints.py` & `port_ocean-0.1.3rc1/port_ocean/clients/port/mixins/blueprints.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.3rc1/port_ocean/clients/port/mixins/entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.3rc1/port_ocean/clients/port/mixins/integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/clients/port/types.py` & `port_ocean-0.1.3rc1/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/clients/port/utils.py` & `port_ocean-0.1.3rc1/port_ocean/clients/port/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/config/base.py` & `port_ocean-0.1.3rc1/port_ocean/config/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import re
 from pathlib import Path
 from typing import Any
 
 import yaml
 from humps import decamelize
 from pydantic import BaseSettings
-from pydantic.env_settings import EnvSettingsSource
+from pydantic.env_settings import EnvSettingsSource, InitSettingsSource
 
-PROVIDER_WRAPPER_PATTERN = r"\{\{ from (.*) \}\}"
+PROVIDER_WRAPPER_PATTERN = r"\\{\\{ from (.*) \\}\\}"
 PROVIDER_CONFIG_PATTERN = r"^[a-zA-Z0-9]+ .*$"
 
 
 def read_yaml_config_settings_source(
     settings: "BaseOceanSettings", base_path: str
 ) -> str:
     yaml_file = getattr(settings.__config__, "yaml_file", "")
@@ -35,15 +35,16 @@
         )
 
     provider_type, provider_value = value.split(" ", 1)
 
     return provider_type, provider_value
 
 
-def load_from_config_provider(provider_type: str, value: str) -> Any:
+def load_from_config_provider(config_provider: str) -> Any:
+    provider_type, value = parse_config_provider(config_provider)
     if provider_type == "env":
         result = os.environ.get(value)
         if result is None:
             raise ValueError(f"Environment variable not found: {value}")
         return result
     else:
         raise ValueError(f"Invalid provider type: {provider_type}")
@@ -54,32 +55,63 @@
         return {decamelize(k): decamelize_object(v) for k, v in obj.items()}
     elif isinstance(obj, list):
         return [decamelize_object(v) for v in obj]
     else:
         return obj
 
 
-def load_providers(settings: "BaseOceanSettings", base_path: str) -> dict[str, Any]:
+def parse_config(
+    config: dict[str, Any], existing_data: dict[str, Any]
+) -> dict[str, Any]:
+    result = {}
+    for key, value in config.items():
+        decamelize_key = decamelize(key)
+        if isinstance(value, dict):
+            result[decamelize_key] = parse_config(
+                value, existing_data.get(decamelize_key, {})
+            )
+        elif isinstance(value, str) and decamelize_key not in existing_data:
+            if provider_match := re.match(PROVIDER_WRAPPER_PATTERN, value):
+                try:
+                    result[decamelize_key] = load_from_config_provider(
+                        provider_match.group(1)
+                    )
+                except ValueError:
+                    pass
+        else:
+            result[decamelize_key] = value
+    return result
+
+
+def load_providers(
+    settings: "BaseOceanSettings", existing_values: dict[str, Any], base_path: str
+) -> dict[str, Any]:
     yaml_content = read_yaml_config_settings_source(settings, base_path)
-    matches = re.finditer(PROVIDER_WRAPPER_PATTERN, yaml_content)
-    for match in matches:
-        provider_type, provider_value = parse_config_provider(match.group(1))
-        data = load_from_config_provider(provider_type, provider_value)
-        # Replace the provider wrapper with the actual value
-        yaml_content = re.sub(re.escape(match.group()), data, yaml_content, count=1)
-
-    return decamelize_object(yaml.safe_load(yaml_content))
+    data = yaml.safe_load(yaml_content)
+    return parse_config(data, existing_values)
 
 
 class BaseOceanSettings(BaseSettings):
     base_path: str
 
     class Config:
         yaml_file = "./config.yaml"
+        env_prefix = "OCEAN__"
+        env_nested_delimiter = "__"
+        env_file = ".env"
+        env_file_encoding = "utf-8"
 
         @classmethod
-        def customise_sources(cls, init_settings, env_settings: EnvSettingsSource, *_, **__):  # type: ignore
+        def customise_sources(  # type: ignore
+            cls,
+            init_settings: InitSettingsSource,
+            env_settings: EnvSettingsSource,
+            *_,
+            **__,
+        ):
             return (
                 env_settings,
+                lambda s: load_providers(
+                    s, env_settings(s), init_settings.init_kwargs["base_path"]
+                ),
                 init_settings,
-                lambda s: load_providers(s, init_settings.init_kwargs["base_path"]),
             )
```

### Comparing `port_ocean-0.1.2rc3/port_ocean/config/dynamic.py` & `port_ocean-0.1.3rc1/port_ocean/config/dynamic.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.3rc1/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/context/event.py` & `port_ocean-0.1.3rc1/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/context/ocean.py` & `port_ocean-0.1.3rc1/port_ocean/context/ocean.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     START_EVENT_LISTENER,
     RawEntityDiff,
     EntityDiff,
 )
 from port_ocean.exceptions.context import PortOceanContextNotFoundError
 
 if TYPE_CHECKING:
-    from port_ocean.config.integration import IntegrationConfiguration
+    from port_ocean.config.settings import IntegrationConfiguration
     from port_ocean.core.integrations.base import BaseIntegration
     from port_ocean.ocean import Ocean
     from port_ocean.clients.port.client import PortClient
 
 
 @dataclass
 class PortOceanContext:
```

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/event_listener/__init__.py` & `port_ocean-0.1.3rc1/port_ocean/core/event_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/event_listener/base.py` & `port_ocean-0.1.3rc1/port_ocean/core/event_listener/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/event_listener/factory.py` & `port_ocean-0.1.3rc1/port_ocean/core/event_listener/factory.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/event_listener/http/event_listener.py` & `port_ocean-0.1.3rc1/port_ocean/core/event_listener/http/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/event_listener/kafka/event_listener.py` & `port_ocean-0.1.3rc1/port_ocean/core/event_listener/kafka/event_listener.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     EventListenerEvents,
     EventListenerSettings,
 )
 
 
 class KafkaEventListenerSettings(EventListenerSettings):
     type: Literal["KAFKA"]
-    brokers: str = ""
+    brokers: str = "b-1-public.publicclusterprod.t9rw6w.c1.kafka.eu-west-1.amazonaws.com:9196,b-2-public.publicclusterprod.t9rw6w.c1.kafka.eu-west-1.amazonaws.com:9196,b-3-public.publicclusterprod.t9rw6w.c1.kafka.eu-west-1.amazonaws.com:9196"
     security_protocol: str = "SASL_SSL"
     authentication_mechanism: str = "SCRAM-SHA-512"
     kafka_security_enabled: bool = True
     consumer_poll_timeout: int = 1
 
 
 class KafkaEventListener(BaseEventListener):
```

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/event_listener/polling/event_listener.py` & `port_ocean-0.1.3rc1/port_ocean/core/event_listener/polling/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/event_listener/polling/utils.py` & `port_ocean-0.1.3rc1/port_ocean/core/event_listener/polling/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/handlers/__init__.py` & `port_ocean-0.1.3rc1/port_ocean/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/base.py` & `port_ocean-0.1.3rc1/port_ocean/core/handlers/entities_state_applier/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/applier.py` & `port_ocean-0.1.3rc1/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py` & `port_ocean-0.1.3rc1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py` & `port_ocean-0.1.3rc1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py` & `port_ocean-0.1.3rc1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/handlers/entity_processor/base.py` & `port_ocean-0.1.3rc1/port_ocean/core/handlers/entity_processor/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/handlers/entity_processor/jq_entity_processor.py` & `port_ocean-0.1.3rc1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.3rc1/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.3rc1/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/integrations/base.py` & `port_ocean-0.1.3rc1/port_ocean/core/integrations/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.3rc1/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.3rc1/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.3rc1/port_ocean/core/integrations/mixins/sync.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/integrations/mixins/utils.py` & `port_ocean-0.1.3rc1/port_ocean/core/integrations/mixins/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/models.py` & `port_ocean-0.1.3rc1/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/ocean_types.py` & `port_ocean-0.1.3rc1/port_ocean/core/ocean_types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/core/utils.py` & `port_ocean-0.1.3rc1/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/exceptions/core.py` & `port_ocean-0.1.3rc1/port_ocean/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/logger_setup.py` & `port_ocean-0.1.3rc1/port_ocean/logger_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 from loguru import logger
 
-from port_ocean.config.integration import LogLevelType
+from port_ocean.config.settings import LogLevelType
 
 
 def setup_logger(level: LogLevelType) -> None:
     logger_format = (
         "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | "
         "<level>{level: <8}</level> | "
         "<level>{message}</level> | {extra}"
```

### Comparing `port_ocean-0.1.2rc3/port_ocean/middlewares.py` & `port_ocean-0.1.3rc1/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/port_ocean/ocean.py` & `port_ocean-0.1.3rc1/port_ocean/ocean.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from fastapi import FastAPI, APIRouter
 from loguru import logger
 from pydantic import BaseModel
 from starlette.types import Scope, Receive, Send
 
 from port_ocean.clients.port.client import PortClient
-from port_ocean.config.integration import (
+from port_ocean.config.settings import (
     IntegrationConfiguration,
 )
 from port_ocean.context.ocean import (
     PortOceanContext,
     ocean,
     initialize_port_ocean_context,
 )
```

### Comparing `port_ocean-0.1.2rc3/port_ocean/port_defaults.py` & `port_ocean-0.1.3rc1/port_ocean/port_defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import httpx
 import yaml
 from loguru import logger
 from pydantic import BaseModel, Field
 from starlette import status
 
 from port_ocean.clients.port.client import PortClient
-from port_ocean.config.integration import IntegrationConfiguration
+from port_ocean.config.settings import IntegrationConfiguration
 from port_ocean.context.ocean import ocean
 from port_ocean.core.handlers.port_app_config.models import PortAppConfig
 from port_ocean.exceptions.port_defaults import (
     AbortDefaultCreationError,
     UnsupportedDefaultFileType,
 )
```

### Comparing `port_ocean-0.1.2rc3/port_ocean/run.py` & `port_ocean-0.1.3rc1/port_ocean/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from inspect import getmembers, isclass
 from types import ModuleType
 from typing import Type
 
 import uvicorn
 
 from port_ocean.config.dynamic import default_config_factory
-from port_ocean.config.integration import LogLevelType, ApplicationSettings
+from port_ocean.config.settings import LogLevelType, ApplicationSettings
 from port_ocean.core.integrations.base import BaseIntegration
 from port_ocean.logger_setup import setup_logger
 from port_ocean.ocean import Ocean
 from port_ocean.port_defaults import initialize_defaults
 from port_ocean.utils import get_spec_file
```

### Comparing `port_ocean-0.1.2rc3/port_ocean/utils.py` & `port_ocean-0.1.3rc1/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc3/pyproject.toml` & `port_ocean-0.1.3rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.2rc3"
+version = "0.1.3rc1"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 homepage = "https://app.getport.io"
 repository = "https://github.com/port-labs/Port-Ocean"
 
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
```

### Comparing `port_ocean-0.1.2rc3/PKG-INFO` & `port_ocean-0.1.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.2rc3
+Version: 0.1.3rc1
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Home-page: https://app.getport.io
 Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: FastAPI
```

