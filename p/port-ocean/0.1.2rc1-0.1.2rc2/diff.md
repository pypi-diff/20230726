# Comparing `tmp/port_ocean-0.1.2rc1.tar.gz` & `tmp/port_ocean-0.1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.2rc1.tar", max compression
+gzip compressed data, was "port_ocean-0.1.2rc2.tar", max compression
```

## Comparing `port_ocean-0.1.2rc1.tar` & `port_ocean-0.1.2rc2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0    11357 2023-07-26 15:20:48.100603 port_ocean-0.1.2rc1/LICENSE
--rw-r--r--   0        0        0     4639 2023-07-26 15:20:48.100603 port_ocean-0.1.2rc1/README.md
--rw-r--r--   0        0        0      270 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/__init__.py
--rw-r--r--   0        0        0      328 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cli.py
--rw-r--r--   0        0        0      278 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/__init__.py
--rw-r--r--   0        0        0     1134 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/list_integrations.py
--rw-r--r--   0        0        0     1057 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/main.py
--rw-r--r--   0        0        0     1710 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/new.py
--rw-r--r--   0        0        0     2306 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/pull.py
--rw-r--r--   0        0        0     1808 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/sail.py
--rw-r--r--   0        0        0      536 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/commands/version.py
--rw-r--r--   0        0        0      429 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       42 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0       12 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
--rw-r--r--   0        0        0      388 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
--rw-r--r--   0        0        0      292 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      449 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1680 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      655 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       12 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
--rw-r--r--   0        0        0      898 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
--rw-r--r--   0        0        0       65 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1920 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0       54 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/cli/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2563 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2309 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     2928 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/blueprints.py
--rw-r--r--   0        0        0     5623 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3909 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      781 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2571 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/config/base.py
--rw-r--r--   0        0        0     1218 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/config/dynamic.py
--rw-r--r--   0        0        0     1313 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     4147 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/context/event.py
--rw-r--r--   0        0        0     4286 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/base.py
--rw-r--r--   0        0        0      607 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/__init__.py
--rw-r--r--   0        0        0      560 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/base.py
--rw-r--r--   0        0        0     2555 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/factory.py
--rw-r--r--   0        0        0     1197 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/http/event_listener.py
--rw-r--r--   0        0        0     3347 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/kafka/event_listener.py
--rw-r--r--   0        0        0     1867 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/polling/event_listener.py
--rw-r--r--   0        0        0     2799 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/event_listener/polling/utils.py
--rw-r--r--   0        0        0      716 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/__init__.py
--rw-r--r--   0        0        0      869 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/base.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/__init__.py
--rw-r--r--   0        0        0     7977 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/applier.py
--rw-r--r--   0        0        0     1339 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
--rw-r--r--   0        0        0      988 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     1392 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entity_processor/__init__.py
--rw-r--r--   0        0        0      955 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entity_processor/base.py
--rw-r--r--   0        0        0     2685 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      396 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1810 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     1912 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      698 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2569 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0    11831 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0     1683 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/utils.py
--rw-r--r--   0        0        0     1368 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/models.py
--rw-r--r--   0        0        0      781 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/ocean_types.py
--rw-r--r--   0        0        0     1957 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-26 15:20:48.112604 port_ocean-0.1.2rc1/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      532 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      407 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/exceptions/port_defaults.py
--rw-r--r--   0        0        0      554 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2475 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/middlewares.py
--rw-r--r--   0        0        0     2315 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/ocean.py
--rw-r--r--   0        0        0     7164 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/port_defaults.py
--rw-r--r--   0        0        0        0 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/py.typed
--rw-r--r--   0        0        0     3059 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/run.py
--rw-r--r--   0        0        0     1007 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/port_ocean/utils.py
--rw-r--r--   0        0        0     3442 2023-07-26 15:20:48.116604 port_ocean-0.1.2rc1/pyproject.toml
--rw-r--r--   0        0        0     6319 1970-01-01 00:00:00.000000 port_ocean-0.1.2rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 19:07:52.321389 port_ocean-0.1.2rc2/LICENSE
+-rw-r--r--   0        0        0     4639 2023-07-26 19:07:52.321389 port_ocean-0.1.2rc2/README.md
+-rw-r--r--   0        0        0      270 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/__init__.py
+-rw-r--r--   0        0        0      328 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0      278 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1134 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/list_integrations.py
+-rw-r--r--   0        0        0     1057 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/main.py
+-rw-r--r--   0        0        0     1710 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/new.py
+-rw-r--r--   0        0        0     2306 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/pull.py
+-rw-r--r--   0        0        0     1537 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/sail.py
+-rw-r--r--   0        0        0      536 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/commands/version.py
+-rw-r--r--   0        0        0      429 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0       12 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
+-rw-r--r--   0        0        0      388 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      292 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      449 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1680 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      655 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
+-rw-r--r--   0        0        0      898 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       65 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1920 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/cli/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2563 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2309 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     2928 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/blueprints.py
+-rw-r--r--   0        0        0     5623 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3909 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      781 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2701 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1259 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0     1133 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     4147 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4286 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/base.py
+-rw-r--r--   0        0        0      607 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0      554 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     2555 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0     1165 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/http/event_listener.py
+-rw-r--r--   0        0        0     3128 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/kafka/event_listener.py
+-rw-r--r--   0        0        0     1867 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/polling/event_listener.py
+-rw-r--r--   0        0        0     2799 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/event_listener/polling/utils.py
+-rw-r--r--   0        0        0      716 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0      869 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7977 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1339 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0      988 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0      955 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     2685 2023-07-26 19:07:52.337389 port_ocean-0.1.2rc2/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1810 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     1912 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      698 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2569 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0    11843 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0     1683 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/utils.py
+-rw-r--r--   0        0        0     1368 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/models.py
+-rw-r--r--   0        0        0      781 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/ocean_types.py
+-rw-r--r--   0        0        0     1957 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      532 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      407 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/exceptions/port_defaults.py
+-rw-r--r--   0        0        0      554 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     2266 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/ocean.py
+-rw-r--r--   0        0        0     7164 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/port_defaults.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/py.typed
+-rw-r--r--   0        0        0     2837 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/run.py
+-rw-r--r--   0        0        0     1007 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/port_ocean/utils.py
+-rw-r--r--   0        0        0     3461 2023-07-26 19:07:52.341389 port_ocean-0.1.2rc2/pyproject.toml
+-rw-r--r--   0        0        0     6359 1970-01-01 00:00:00.000000 port_ocean-0.1.2rc2/PKG-INFO
```

### Comparing `port_ocean-0.1.2rc1/LICENSE` & `port_ocean-0.1.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/README.md` & `port_ocean-0.1.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/cli/commands/list_integrations.py` & `port_ocean-0.1.2rc2/port_ocean/cli/commands/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/cli/commands/main.py` & `port_ocean-0.1.2rc2/port_ocean/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/cli/commands/new.py` & `port_ocean-0.1.2rc2/port_ocean/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/cli/commands/pull.py` & `port_ocean-0.1.2rc2/port_ocean/cli/commands/pull.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/cli/commands/sail.py` & `port_ocean-0.1.2rc2/port_ocean/cli/commands/sail.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,34 +32,24 @@
     "-i",
     "--initialize-port-resources",
     "initialize_port_resources",
     type=bool,
     help="""Set to true to create default resources on installation.
             If not specified, the default value is false.""",
 )
-@click.option(
-    "-c",
-    "--config-path",
-    "config_path",
-    type=str,
-    default="./config.yml",
-    help="""Set the path to the configuration file.
-            If not specified, the default path is ./config.yml.""",
-)
 def sail(
     path: str,
     log_level: LogLevelType,
     port: int,
     initialize_port_resources: bool | None,
-    config_path: str | None,
 ) -> None:
     """
     Runs the integration in the given PATH. if no PATH is provided, the current directory will be used.
 
     PATH: Path to the integration.
     """
     from port_ocean import run
 
     print_logo()
 
     console.print("Setting sail... ⛵️⚓️⛵️⚓️ All hands on deck! ⚓️")
-    run(path, log_level, port, initialize_port_resources, config_path)
+    run(path, log_level, port, initialize_port_resources)
```

### Comparing `port_ocean-0.1.2rc1/port_ocean/cli/commands/version.py` & `port_ocean-0.1.2rc2/port_ocean/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md` & `port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml` & `port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.2rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.2rc2/port_ocean/clients/port/authentication.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/clients/port/client.py` & `port_ocean-0.1.2rc2/port_ocean/clients/port/client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/blueprints.py` & `port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/blueprints.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.2rc2/port_ocean/clients/port/mixins/integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/clients/port/types.py` & `port_ocean-0.1.2rc2/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/clients/port/utils.py` & `port_ocean-0.1.2rc2/port_ocean/clients/port/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/config/base.py` & `port_ocean-0.1.2rc2/port_ocean/config/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 import os
 import re
 from pathlib import Path
 from typing import Any
-from urllib.parse import urlparse
 
-import httpx
 import yaml
+from humps import decamelize
 from pydantic import BaseSettings
+from pydantic.env_settings import EnvSettingsSource
 
 PROVIDER_WRAPPER_PATTERN = r"\{\{ from (.*) \}\}"
 PROVIDER_CONFIG_PATTERN = r"^[a-zA-Z0-9]+ .*$"
-DEFAULT_CONFIG_PATH = "./config.yaml"
 
 
-def read_yaml_config_settings_source(config_path: str) -> str:
-    parsed_url = urlparse(config_path)
-    if parsed_url.scheme == "file" or not parsed_url.scheme:
-        path = Path(config_path)
-
-        if not path.exists():
-            raise FileNotFoundError(f"Could not open yaml settings file at: {path}")
-
-        return path.read_text("utf-8")
-    elif parsed_url.scheme in ["http", "https"]:
-        config_response = httpx.get(config_path)
-        config_response.raise_for_status()
-        return config_response.text
-    else:
-        raise ValueError(f"Invalid config path: {config_path}")
+def read_yaml_config_settings_source(
+    settings: "BaseOceanSettings", base_path: str
+) -> str:
+    yaml_file = getattr(settings.__config__, "yaml_file", "")
+
+    assert yaml_file, "Settings.yaml_file not properly configured"
+
+    path = Path(base_path, yaml_file)
+
+    if not path.exists():
+        raise FileNotFoundError(f"Could not open yaml settings file at: {path}")
+
+    return path.read_text("utf-8")
 
 
 def parse_config_provider(value: str) -> tuple[str, str]:
     match = re.match(PROVIDER_CONFIG_PATTERN, value)
     if not match:
         raise ValueError(
             f"Invalid pattern: {value}. Pattern should match: {PROVIDER_CONFIG_PATTERN}"
@@ -48,31 +45,41 @@
         if result is None:
             raise ValueError(f"Environment variable not found: {value}")
         return result
     else:
         raise ValueError(f"Invalid provider type: {provider_type}")
 
 
-def load_providers(config_path: str) -> dict[str, Any]:
-    yaml_content = read_yaml_config_settings_source(config_path)
+def decamelize_object(obj: Any) -> Any:
+    if isinstance(obj, dict):
+        return {decamelize(k): decamelize_object(v) for k, v in obj.items()}
+    elif isinstance(obj, list):
+        return [decamelize_object(v) for v in obj]
+    else:
+        return obj
+
+
+def load_providers(settings: "BaseOceanSettings", base_path: str) -> dict[str, Any]:
+    yaml_content = read_yaml_config_settings_source(settings, base_path)
     matches = re.finditer(PROVIDER_WRAPPER_PATTERN, yaml_content)
     for match in matches:
         provider_type, provider_value = parse_config_provider(match.group(1))
         data = load_from_config_provider(provider_type, provider_value)
         # Replace the provider wrapper with the actual value
         yaml_content = re.sub(re.escape(match.group()), data, yaml_content, count=1)
 
-    return yaml.safe_load(yaml_content)
+    return decamelize_object(yaml.safe_load(yaml_content))
 
 
 class BaseOceanSettings(BaseSettings):
-    config_path: str | None = DEFAULT_CONFIG_PATH
+    base_path: str
 
     class Config:
+        yaml_file = "./config.yaml"
+
         @classmethod
-        def customise_sources(cls, init_settings, *_, **__):  # type: ignore
+        def customise_sources(cls, init_settings, env_settings: EnvSettingsSource, *_, **__):  # type: ignore
             return (
+                env_settings,
                 init_settings,
-                lambda s: load_providers(
-                    init_settings.init_kwargs["config_path"] or DEFAULT_CONFIG_PATH
-                ),
+                lambda s: load_providers(s, init_settings.init_kwargs["base_path"]),
             )
```

### Comparing `port_ocean-0.1.2rc1/port_ocean/config/dynamic.py` & `port_ocean-0.1.2rc2/port_ocean/config/dynamic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Type, Any, Optional
 
+from humps import decamelize
 from pydantic import BaseModel, AnyUrl, create_model, Extra, parse_obj_as
 
 
 class Configuration(BaseModel, extra=Extra.allow):
     name: str
     type: str
     required: bool = False
@@ -30,13 +31,13 @@
                 field_type = bool
             case _:
                 raise ValueError(f"Unknown type: {config.type}")
 
         default = ... if config.required else None
         if config.default is not None:
             default = parse_obj_as(field_type, config.default)
-        fields[config.name] = (
+        fields[decamelize(config.name)] = (
             field_type,
             default,
         )
 
     return create_model("Config", **fields)  # type: ignore
```

### Comparing `port_ocean-0.1.2rc1/port_ocean/config/integration.py` & `port_ocean-0.1.2rc2/port_ocean/config/integration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from typing import Any, Literal
 
-from pydantic import Field, BaseSettings
+from pydantic import BaseSettings, BaseModel
 
 from port_ocean.config.base import BaseOceanSettings
 from port_ocean.core.event_listener import EventListenerSettingsType
 
 
-class PortSettings(BaseSettings):
-    client_id: str = Field(alias="clientId")
-    client_secret: str = Field(alias="clientSecret")
-    base_url: str = Field(alias="baseUrl", default="https://api.getport.io")
+class PortSettings(BaseModel):
+    client_id: str
+    client_secret: str
+    base_url: str = "https://api.getport.io"
 
 
-class IntegrationSettings(BaseSettings):
+class IntegrationSettings(BaseModel):
     identifier: str
     type: str
     config: dict[str, Any]
 
 
 class IntegrationConfiguration(BaseOceanSettings):
     port: PortSettings
-    event_listener: EventListenerSettingsType = Field(alias="eventListener")
-    batch_work_size: int = Field(alias="batchWorkSize", default=20)
-    initialize_port_resources: bool = Field(
-        alias="initializePortResources", default=False
-    )
+    event_listener: EventListenerSettingsType
+    batch_work_size: int = 20
+    initialize_port_resources: bool = False
     integration: IntegrationSettings
 
+    class Config:
+        env_prefix = "OCEAN__"
+        env_nested_delimiter = "__"
+
 
 LogLevelType = Literal["ERROR", "WARNING", "INFO", "DEBUG", "CRITICAL"]
 
 
 class ApplicationSettings(BaseSettings):
     log_level: LogLevelType = "DEBUG"
     port: int = 8000
-    config_path: str | None = "./config.yaml"
 
     class Config:
-        env_prefix = "APPLICATION_"
+        env_prefix = "APPLICATION__"
 
         @classmethod
         def customise_sources(cls, init_settings, env_settings, *_, **__):  # type: ignore
             return env_settings, init_settings
```

### Comparing `port_ocean-0.1.2rc1/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.2rc2/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/context/event.py` & `port_ocean-0.1.2rc2/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/context/ocean.py` & `port_ocean-0.1.2rc2/port_ocean/context/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/event_listener/__init__.py` & `port_ocean-0.1.2rc2/port_ocean/core/event_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/event_listener/base.py` & `port_ocean-0.1.2rc2/port_ocean/core/event_listener/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod
 from typing import TypedDict, Callable, Any, Awaitable
 
-from pydantic import BaseSettings
+from pydantic import BaseModel
 
 
 class EventListenerEvents(TypedDict):
     on_resync: Callable[[dict[Any, Any]], Awaitable[None]]
 
 
 class BaseEventListener:
@@ -16,12 +16,12 @@
         self.events = events
 
     @abstractmethod
     async def start(self) -> None:
         pass
 
 
-class EventListenerSettings(BaseSettings):
+class EventListenerSettings(BaseModel):
     type: str
 
     def to_request(self) -> dict[str, Any]:
         return {"type": self.type}
```

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/event_listener/factory.py` & `port_ocean-0.1.2rc2/port_ocean/core/event_listener/factory.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/event_listener/http/event_listener.py` & `port_ocean-0.1.2rc2/port_ocean/core/event_listener/http/event_listener.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Literal, Any
 
 from fastapi import APIRouter
 from loguru import logger
-from pydantic import AnyHttpUrl, Field
+from pydantic import AnyHttpUrl
 
 from port_ocean.context.ocean import ocean
 from port_ocean.core.event_listener.base import (
     BaseEventListener,
     EventListenerEvents,
     EventListenerSettings,
 )
 
 
 class HttpEventListenerSettings(EventListenerSettings):
     type: Literal["WEBHOOK"]
-    app_host: AnyHttpUrl = Field(alias="appHost")
+    app_host: AnyHttpUrl
 
     def to_request(self) -> dict[str, Any]:
         return {
             **super().to_request(),
             "url": self.app_host + "/resync",
         }
```

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/event_listener/kafka/event_listener.py` & `port_ocean-0.1.2rc2/port_ocean/core/event_listener/kafka/event_listener.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import threading
 from typing import Any, Callable, Literal
 
 from loguru import logger
-from pydantic import Field
 
 from port_ocean.consumers.kafka_consumer import KafkaConsumer, KafkaConsumerConfig
 from port_ocean.context.ocean import (
     PortOceanContext,
     initialize_port_ocean_context,
     ocean,
 )
@@ -16,20 +15,18 @@
     EventListenerSettings,
 )
 
 
 class KafkaEventListenerSettings(EventListenerSettings):
     type: Literal["KAFKA"]
     brokers: str = ""
-    security_protocol: str = Field(alias="securityProtocol", default="SASL_SSL")
-    authentication_mechanism: str = Field(
-        alias="authenticationMechanism", default="SCRAM-SHA-512"
-    )
-    kafka_security_enabled: bool = Field(alias="kafkaSecurityEnabled", default=True)
-    consumer_poll_timeout: int = Field(alias="consumerPollTimeout", default=1)
+    security_protocol: str = "SASL_SSL"
+    authentication_mechanism: str = "SCRAM-SHA-512"
+    kafka_security_enabled: bool = True
+    consumer_poll_timeout: int = 1
 
 
 class KafkaEventListener(BaseEventListener):
     def __init__(
         self,
         events: EventListenerEvents,
         event_listener_config: KafkaEventListenerSettings,
```

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/event_listener/polling/event_listener.py` & `port_ocean-0.1.2rc2/port_ocean/core/event_listener/polling/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/event_listener/polling/utils.py` & `port_ocean-0.1.2rc2/port_ocean/core/event_listener/polling/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/handlers/__init__.py` & `port_ocean-0.1.2rc2/port_ocean/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/base.py` & `port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/applier.py` & `port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py` & `port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py` & `port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py` & `port_ocean-0.1.2rc2/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/handlers/entity_processor/base.py` & `port_ocean-0.1.2rc2/port_ocean/core/handlers/entity_processor/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py` & `port_ocean-0.1.2rc2/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.2rc2/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.2rc2/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/integrations/base.py` & `port_ocean-0.1.2rc2/port_ocean/core/integrations/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
             creation_results: list[tuple[list[Entity], list[Exception]]] = []
             for resource in app_config.resources:
                 creation_results.append(
                     await self._register_in_batches(
                         resource, user_agent_type, ocean.config.batch_work_size
                     )
                 )
-            flat_created_entities, errors = zip_and_sum(creation_results)
+            flat_created_entities, errors = zip_and_sum(creation_results) or [[], []]
 
             if errors:
                 message = f"Resync failed with {len(errors)}. Skipping delete phase due to incomplete state"
                 error_group = ExceptionGroup(
                     f"Resync failed with {len(errors)}. Skipping delete phase due to incomplete state",
                     errors,
                 )
```

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/integrations/mixins/utils.py` & `port_ocean-0.1.2rc2/port_ocean/core/integrations/mixins/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/models.py` & `port_ocean-0.1.2rc2/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/ocean_types.py` & `port_ocean-0.1.2rc2/port_ocean/core/ocean_types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/core/utils.py` & `port_ocean-0.1.2rc2/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/exceptions/core.py` & `port_ocean-0.1.2rc2/port_ocean/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/logger_setup.py` & `port_ocean-0.1.2rc2/port_ocean/logger_setup.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/middlewares.py` & `port_ocean-0.1.2rc2/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/ocean.py` & `port_ocean-0.1.2rc2/port_ocean/ocean.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,21 +22,20 @@
 class Ocean:
     def __init__(
         self,
         app: FastAPI | None = None,
         integration_class: Callable[[PortOceanContext], BaseIntegration] | None = None,
         integration_router: APIRouter | None = None,
         config_factory: Callable[..., BaseModel] | None = None,
-        config_path: str | None = None,
     ):
         initialize_port_ocean_context(self)
         self.fast_api_app = app or FastAPI()
         self.fast_api_app.middleware("http")(request_handler)
 
-        self.config = IntegrationConfiguration(config_path=config_path)
+        self.config = IntegrationConfiguration(base_path="./")
         if config_factory:
             self.config.integration.config = config_factory(
                 **self.config.integration.config
             ).dict()
         self.integration_router = integration_router or APIRouter()
 
         self.port_client = PortClient(
```

### Comparing `port_ocean-0.1.2rc1/port_ocean/port_defaults.py` & `port_ocean-0.1.2rc2/port_ocean/port_defaults.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/port_ocean/run.py` & `port_ocean-0.1.2rc2/port_ocean/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,49 +37,40 @@
 
     module = module_from_spec(spec)
     spec.loader.exec_module(module)
 
     return module
 
 
-def _create_default_app(
-    path: str | None = None, config_path: str | None = None
-) -> Ocean:
+def _create_default_app(path: str | None = None) -> Ocean:
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
-    return Ocean(
-        integration_class=integration_class,
-        config_factory=config_factory,
-        config_path=config_path or "./config.yaml",
-    )
+    return Ocean(integration_class=integration_class, config_factory=config_factory)
 
 
 def run(
     path: str = ".",
     log_level: LogLevelType = "DEBUG",
     port: int = 8000,
     initialize_port_resources: bool | None = None,
-    config_path: str | None = None,
 ) -> None:
-    application_settings = ApplicationSettings(
-        log_level=log_level, port=port, config_path=config_path
-    )
+    application_settings = ApplicationSettings(log_level=log_level, port=port)
 
     setup_logger(application_settings.log_level)
-    default_app = _create_default_app(path, application_settings.config_path)
+    default_app = _create_default_app(path)
 
     main_path = f"{path}/main.py" if path else "main.py"
     app_module = _load_module(main_path)
     app: Ocean = {name: item for name, item in getmembers(app_module)}.get(
         "app", default_app
     )
```

### Comparing `port_ocean-0.1.2rc1/port_ocean/utils.py` & `port_ocean-0.1.2rc2/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.2rc1/pyproject.toml` & `port_ocean-0.1.2rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.2rc1"
+version = "0.1.2rc2"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 homepage = "https://app.getport.io"
 repository = "https://github.com/port-labs/Port-Ocean"
 
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
@@ -43,14 +43,15 @@
 fastapi = "^0.100.0"
 uvicorn = "^0.22.0"
 confluent-kafka = "^2.1.1"
 httpx = "^0.24.1"
 pyjq = "^2.6.0"
 urllib3 = "^1.26.16"
 six = "^1.16.0"
+pyhumps = "^3.8.0"
 
 # CLI
 click = { version = "^8.1.3", optional = true }
 rich = { version = "^13.4.1", optional = true }
 cookiecutter = { version = "^2.1.1", optional = true }
 jinja2-time = { version = "^0.2.0", optional = true }
```

### Comparing `port_ocean-0.1.2rc1/PKG-INFO` & `port_ocean-0.1.2rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.2rc1
+Version: 0.1.2rc2
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Home-page: https://app.getport.io
 Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: FastAPI
@@ -24,14 +24,15 @@
 Requires-Dist: confluent-kafka (>=2.1.1,<3.0.0)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0) ; extra == "cli"
 Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: jinja2-time (>=0.2.0,<0.3.0) ; extra == "cli"
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: pyjq (>=2.6.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0) ; extra == "cli"
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: werkzeug (>=2.3.4,<3.0.0)
```

