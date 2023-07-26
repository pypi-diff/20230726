# Comparing `tmp/port_ocean-0.1.1.tar.gz` & `tmp/port_ocean-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.1.tar", max compression
+gzip compressed data, was "port_ocean-0.1.2rc1.tar", max compression
```

## Comparing `port_ocean-0.1.1.tar` & `port_ocean-0.1.2rc1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0    11357 2023-07-26 07:38:34.234947 port_ocean-0.1.1/LICENSE
--rw-r--r--   0        0        0     4639 2023-07-26 07:38:34.234947 port_ocean-0.1.1/README.md
--rw-r--r--   0        0        0      270 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/__init__.py
--rw-r--r--   0        0        0      328 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cli.py
--rw-r--r--   0        0        0      278 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/__init__.py
--rw-r--r--   0        0        0     1134 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/list_integrations.py
--rw-r--r--   0        0        0     1057 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/main.py
--rw-r--r--   0        0        0     1710 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/new.py
--rw-r--r--   0        0        0     2306 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/pull.py
--rw-r--r--   0        0        0     1537 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/sail.py
--rw-r--r--   0        0        0      536 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/version.py
--rw-r--r--   0        0        0      429 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       42 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0       12 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
--rw-r--r--   0        0        0      388 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
--rw-r--r--   0        0        0      292 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      449 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1680 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      655 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       12 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
--rw-r--r--   0        0        0      898 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
--rw-r--r--   0        0        0       65 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1920 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0       54 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2563 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2309 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     2928 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/clients/port/mixins/blueprints.py
--rw-r--r--   0        0        0     5623 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3909 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      781 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2277 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/config/base.py
--rw-r--r--   0        0        0     1218 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/config/dynamic.py
--rw-r--r--   0        0        0     1107 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     4147 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/context/event.py
--rw-r--r--   0        0        0     4286 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/base.py
--rw-r--r--   0        0        0      607 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/__init__.py
--rw-r--r--   0        0        0      560 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/base.py
--rw-r--r--   0        0        0     2555 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/factory.py
--rw-r--r--   0        0        0     1197 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/http/event_listener.py
--rw-r--r--   0        0        0     3347 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/kafka/event_listener.py
--rw-r--r--   0        0        0     1867 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/polling/event_listener.py
--rw-r--r--   0        0        0     2799 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/polling/utils.py
--rw-r--r--   0        0        0      716 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/__init__.py
--rw-r--r--   0        0        0      869 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/base.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/__init__.py
--rw-r--r--   0        0        0     7977 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/applier.py
--rw-r--r--   0        0        0     1339 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
--rw-r--r--   0        0        0      988 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     1392 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entity_processor/__init__.py
--rw-r--r--   0        0        0      955 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entity_processor/base.py
--rw-r--r--   0        0        0     2685 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      396 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1810 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     1912 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      698 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2569 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0    11831 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0     1683 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/mixins/utils.py
--rw-r--r--   0        0        0     1368 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/models.py
--rw-r--r--   0        0        0      781 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/ocean_types.py
--rw-r--r--   0        0        0     1957 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      532 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      407 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/port_defaults.py
--rw-r--r--   0        0        0      554 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2475 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/middlewares.py
--rw-r--r--   0        0        0     2266 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/ocean.py
--rw-r--r--   0        0        0     7164 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/port_defaults.py
--rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/py.typed
--rw-r--r--   0        0        0     2837 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/run.py
--rw-r--r--   0        0        0     1007 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/utils.py
--rw-r--r--   0        0        0     3439 2023-07-26 07:38:34.246947 port_ocean-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 port_ocean-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 15:20:48.100603 port_ocean-0.1.2rc1/LICENSE
+-rw-r--r--   0        0        0     4639 2023-07-26 15:20:48.100603 port_ocean-0.1.2rc1/README.md
+-rw-r--r--   0        0        0      270 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/__init__.py
+-rw-r--r--   0        0        0      328 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0      278 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1134 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/list_integrations.py
+-rw-r--r--   0        0        0     1057 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/main.py
+-rw-r--r--   0        0        0     1710 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/new.py
+-rw-r--r--   0        0        0     2306 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/pull.py
+-rw-r--r--   0        0        0     1808 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/sail.py
+-rw-r--r--   0        0        0      536 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/version.py
+-rw-r--r--   0        0        0      429 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0       12 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
+-rw-r--r--   0        0        0      388 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      292 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      449 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1680 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      655 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
+-rw-r--r--   0        0        0      898 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       65 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1920 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2563 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2309 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     2928 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/blueprints.py
+-rw-r--r--   0        0        0     5623 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3909 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      781 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2571 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1218 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0     1313 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     4147 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4286 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/base.py
+-rw-r--r--   0        0        0      607 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0      560 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     2555 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0     1197 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/http/event_listener.py
+-rw-r--r--   0        0        0     3347 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/kafka/event_listener.py
+-rw-r--r--   0        0        0     1867 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/polling/event_listener.py
+-rw-r--r--   0        0        0     2799 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/polling/utils.py
+-rw-r--r--   0        0        0      716 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0      869 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7977 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1339 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0      988 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0      955 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     2685 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1810 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     1912 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      698 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2569 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0    11831 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0     1683 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/utils.py
+-rw-r--r--   0        0        0     1368 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/models.py
+-rw-r--r--   0        0        0      781 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/ocean_types.py
+-rw-r--r--   0        0        0     1957 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      532 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      407 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/exceptions/port_defaults.py
+-rw-r--r--   0        0        0      554 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     2315 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/ocean.py
+-rw-r--r--   0        0        0     7164 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/port_defaults.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/py.typed
+-rw-r--r--   0        0        0     3059 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/run.py
+-rw-r--r--   0        0        0     1007 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/utils.py
+-rw-r--r--   0        0        0     3442 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     6319 1970-01-01 00:00:00.000000 port_ocean-0.1.2rc1/PKG-INFO
```

### Comparing `port_ocean-0.1.1/LICENSE` & `port_ocean-0.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/README.md` & `port_ocean-0.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/cli/commands/list_integrations.py` & `port_ocean-0.1.2rc1/port_ocean/cli/commands/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/cli/commands/main.py` & `port_ocean-0.1.2rc1/port_ocean/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/cli/commands/new.py` & `port_ocean-0.1.2rc1/port_ocean/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/cli/commands/pull.py` & `port_ocean-0.1.2rc1/port_ocean/cli/commands/pull.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/cli/commands/sail.py` & `port_ocean-0.1.2rc1/port_ocean/cli/commands/sail.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,24 +32,34 @@
     "-i",
     "--initialize-port-resources",
     "initialize_port_resources",
     type=bool,
     help="""Set to true to create default resources on installation.
             If not specified, the default value is false.""",
 )
+@click.option(
+    "-c",
+    "--config-path",
+    "config_path",
+    type=str,
+    default="./config.yml",
+    help="""Set the path to the configuration file.
+            If not specified, the default path is ./config.yml.""",
+)
 def sail(
     path: str,
     log_level: LogLevelType,
     port: int,
     initialize_port_resources: bool | None,
+    config_path: str | None,
 ) -> None:
     """
     Runs the integration in the given PATH. if no PATH is provided, the current directory will be used.
 
     PATH: Path to the integration.
     """
     from port_ocean import run
 
     print_logo()
 
     console.print("Setting sail... ⛵️⚓️⛵️⚓️ All hands on deck! ⚓️")
-    run(path, log_level, port, initialize_port_resources)
+    run(path, log_level, port, initialize_port_resources, config_path)
```

### Comparing `port_ocean-0.1.1/port_ocean/cli/commands/version.py` & `port_ocean-0.1.2rc1/port_ocean/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md` & `port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml` & `port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.2rc1/port_ocean/clients/port/authentication.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/clients/port/client.py` & `port_ocean-0.1.2rc1/port_ocean/clients/port/client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/clients/port/mixins/blueprints.py` & `port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/blueprints.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/clients/port/types.py` & `port_ocean-0.1.2rc1/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/clients/port/utils.py` & `port_ocean-0.1.2rc1/port_ocean/clients/port/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/config/base.py` & `port_ocean-0.1.2rc1/port_ocean/config/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import os
 import re
 from pathlib import Path
 from typing import Any
+from urllib.parse import urlparse
 
+import httpx
 import yaml
 from pydantic import BaseSettings
 
 PROVIDER_WRAPPER_PATTERN = r"\{\{ from (.*) \}\}"
 PROVIDER_CONFIG_PATTERN = r"^[a-zA-Z0-9]+ .*$"
+DEFAULT_CONFIG_PATH = "./config.yaml"
 
 
-def read_yaml_config_settings_source(
-    settings: "BaseOceanSettings", base_path: str
-) -> str:
-    yaml_file = getattr(settings.__config__, "yaml_file", "")
-
-    assert yaml_file, "Settings.yaml_file not properly configured"
-
-    path = Path(base_path, yaml_file)
-
-    if not path.exists():
-        raise FileNotFoundError(f"Could not open yaml settings file at: {path}")
-
-    return path.read_text("utf-8")
+def read_yaml_config_settings_source(config_path: str) -> str:
+    parsed_url = urlparse(config_path)
+    if parsed_url.scheme == "file" or not parsed_url.scheme:
+        path = Path(config_path)
+
+        if not path.exists():
+            raise FileNotFoundError(f"Could not open yaml settings file at: {path}")
+
+        return path.read_text("utf-8")
+    elif parsed_url.scheme in ["http", "https"]:
+        config_response = httpx.get(config_path)
+        config_response.raise_for_status()
+        return config_response.text
+    else:
+        raise ValueError(f"Invalid config path: {config_path}")
 
 
 def parse_config_provider(value: str) -> tuple[str, str]:
     match = re.match(PROVIDER_CONFIG_PATTERN, value)
     if not match:
         raise ValueError(
             f"Invalid pattern: {value}. Pattern should match: {PROVIDER_CONFIG_PATTERN}"
@@ -43,31 +48,31 @@
         if result is None:
             raise ValueError(f"Environment variable not found: {value}")
         return result
     else:
         raise ValueError(f"Invalid provider type: {provider_type}")
 
 
-def load_providers(settings: "BaseOceanSettings", base_path: str) -> dict[str, Any]:
-    yaml_content = read_yaml_config_settings_source(settings, base_path)
+def load_providers(config_path: str) -> dict[str, Any]:
+    yaml_content = read_yaml_config_settings_source(config_path)
     matches = re.finditer(PROVIDER_WRAPPER_PATTERN, yaml_content)
     for match in matches:
         provider_type, provider_value = parse_config_provider(match.group(1))
         data = load_from_config_provider(provider_type, provider_value)
         # Replace the provider wrapper with the actual value
         yaml_content = re.sub(re.escape(match.group()), data, yaml_content, count=1)
 
     return yaml.safe_load(yaml_content)
 
 
 class BaseOceanSettings(BaseSettings):
-    base_path: str
+    config_path: str | None = DEFAULT_CONFIG_PATH
 
     class Config:
-        yaml_file = "./config.yaml"
-
         @classmethod
         def customise_sources(cls, init_settings, *_, **__):  # type: ignore
             return (
                 init_settings,
-                lambda s: load_providers(s, init_settings.init_kwargs["base_path"]),
+                lambda s: load_providers(
+                    init_settings.init_kwargs["config_path"] or DEFAULT_CONFIG_PATH
+                ),
             )
```

### Comparing `port_ocean-0.1.1/port_ocean/config/dynamic.py` & `port_ocean-0.1.2rc1/port_ocean/config/dynamic.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/config/integration.py` & `port_ocean-0.1.2rc1/port_ocean/config/integration.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,10 +30,15 @@
 
 LogLevelType = Literal["ERROR", "WARNING", "INFO", "DEBUG", "CRITICAL"]
 
 
 class ApplicationSettings(BaseSettings):
     log_level: LogLevelType = "DEBUG"
     port: int = 8000
+    config_path: str | None = "./config.yaml"
 
     class Config:
         env_prefix = "APPLICATION_"
+
+        @classmethod
+        def customise_sources(cls, init_settings, env_settings, *_, **__):  # type: ignore
+            return env_settings, init_settings
```

### Comparing `port_ocean-0.1.1/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.2rc1/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/context/event.py` & `port_ocean-0.1.2rc1/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/context/ocean.py` & `port_ocean-0.1.2rc1/port_ocean/context/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/event_listener/__init__.py` & `port_ocean-0.1.2rc1/port_ocean/core/event_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/event_listener/base.py` & `port_ocean-0.1.2rc1/port_ocean/core/event_listener/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/event_listener/factory.py` & `port_ocean-0.1.2rc1/port_ocean/core/event_listener/factory.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/event_listener/http/event_listener.py` & `port_ocean-0.1.2rc1/port_ocean/core/event_listener/http/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/event_listener/kafka/event_listener.py` & `port_ocean-0.1.2rc1/port_ocean/core/event_listener/kafka/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/event_listener/polling/event_listener.py` & `port_ocean-0.1.2rc1/port_ocean/core/event_listener/polling/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/event_listener/polling/utils.py` & `port_ocean-0.1.2rc1/port_ocean/core/event_listener/polling/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/handlers/__init__.py` & `port_ocean-0.1.2rc1/port_ocean/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/base.py` & `port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/applier.py` & `port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py` & `port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py` & `port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py` & `port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/handlers/entity_processor/base.py` & `port_ocean-0.1.2rc1/port_ocean/core/handlers/entity_processor/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py` & `port_ocean-0.1.2rc1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.2rc1/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.2rc1/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/integrations/base.py` & `port_ocean-0.1.2rc1/port_ocean/core/integrations/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/sync.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/integrations/mixins/utils.py` & `port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/models.py` & `port_ocean-0.1.2rc1/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/ocean_types.py` & `port_ocean-0.1.2rc1/port_ocean/core/ocean_types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/core/utils.py` & `port_ocean-0.1.2rc1/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/exceptions/core.py` & `port_ocean-0.1.2rc1/port_ocean/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/logger_setup.py` & `port_ocean-0.1.2rc1/port_ocean/logger_setup.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/middlewares.py` & `port_ocean-0.1.2rc1/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/ocean.py` & `port_ocean-0.1.2rc1/port_ocean/ocean.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,20 +22,21 @@
 class Ocean:
     def __init__(
         self,
         app: FastAPI | None = None,
         integration_class: Callable[[PortOceanContext], BaseIntegration] | None = None,
         integration_router: APIRouter | None = None,
         config_factory: Callable[..., BaseModel] | None = None,
+        config_path: str | None = None,
     ):
         initialize_port_ocean_context(self)
         self.fast_api_app = app or FastAPI()
         self.fast_api_app.middleware("http")(request_handler)
 
-        self.config = IntegrationConfiguration(base_path="./")
+        self.config = IntegrationConfiguration(config_path=config_path)
         if config_factory:
             self.config.integration.config = config_factory(
                 **self.config.integration.config
             ).dict()
         self.integration_router = integration_router or APIRouter()
 
         self.port_client = PortClient(
```

### Comparing `port_ocean-0.1.1/port_ocean/port_defaults.py` & `port_ocean-0.1.2rc1/port_ocean/port_defaults.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/port_ocean/run.py` & `port_ocean-0.1.2rc1/port_ocean/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,40 +37,49 @@
 
     module = module_from_spec(spec)
     spec.loader.exec_module(module)
 
     return module
 
 
-def _create_default_app(path: str | None = None) -> Ocean:
+def _create_default_app(
+    path: str | None = None, config_path: str | None = None
+) -> Ocean:
     sys.path.append(".")
     try:
         integration_path = f"{path}/integration.py" if path else "integration.py"
         module = _load_module(integration_path)
         integration_class = _get_base_integration_class_from_module(module)
     except Exception:
         integration_class = None
 
     spec = get_spec_file()
     config_factory = None
     if spec is not None:
         config_factory = default_config_factory(spec.get("configurations", []))
-    return Ocean(integration_class=integration_class, config_factory=config_factory)
+    return Ocean(
+        integration_class=integration_class,
+        config_factory=config_factory,
+        config_path=config_path or "./config.yaml",
+    )
 
 
 def run(
     path: str = ".",
     log_level: LogLevelType = "DEBUG",
     port: int = 8000,
     initialize_port_resources: bool | None = None,
+    config_path: str | None = None,
 ) -> None:
-    application_settings = ApplicationSettings(log_level=log_level, port=port)
+    application_settings = ApplicationSettings(
+        log_level=log_level, port=port, config_path=config_path
+    )
 
     setup_logger(application_settings.log_level)
-    default_app = _create_default_app(path)
+    default_app = _create_default_app(path, application_settings.config_path)
 
     main_path = f"{path}/main.py" if path else "main.py"
     app_module = _load_module(main_path)
     app: Ocean = {name: item for name, item in getmembers(app_module)}.get(
         "app", default_app
     )
```

### Comparing `port_ocean-0.1.1/port_ocean/utils.py` & `port_ocean-0.1.2rc1/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.1/pyproject.toml` & `port_ocean-0.1.2rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.1"
+version = "0.1.2rc1"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 homepage = "https://app.getport.io"
 repository = "https://github.com/port-labs/Port-Ocean"
 
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
```

### Comparing `port_ocean-0.1.1/PKG-INFO` & `port_ocean-0.1.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.1
+Version: 0.1.2rc1
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Home-page: https://app.getport.io
 Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: FastAPI
```

