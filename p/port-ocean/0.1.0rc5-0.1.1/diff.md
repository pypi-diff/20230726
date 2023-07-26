# Comparing `tmp/port_ocean-0.1.0rc5.tar.gz` & `tmp/port_ocean-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.0rc5.tar", max compression
+gzip compressed data, was "port_ocean-0.1.1.tar", max compression
```

## Comparing `port_ocean-0.1.0rc5.tar` & `port_ocean-0.1.1.tar`

### file list

```diff
@@ -1,97 +1,99 @@
--rw-r--r--   0        0        0    11357 2023-07-20 12:14:21.346149 port_ocean-0.1.0rc5/LICENSE
--rw-r--r--   0        0        0     4585 2023-07-20 12:14:21.346149 port_ocean-0.1.0rc5/README.md
--rw-r--r--   0        0        0      255 2023-07-20 12:14:21.370149 port_ocean-0.1.0rc5/port_ocean/__init__.py
--rw-r--r--   0        0        0      321 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cli.py
--rw-r--r--   0        0        0     5561 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/commands.py
--rw-r--r--   0        0        0      429 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       42 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0       12 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/defaults/.gitignore
--rw-r--r--   0        0        0       12 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
--rw-r--r--   0        0        0      388 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
--rw-r--r--   0        0        0      598 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1680 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      653 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       12 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog_fragments/.gitignore
--rw-r--r--   0        0        0      778 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
--rw-r--r--   0        0        0       65 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1302 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1755 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/download_git_folder.py
--rw-r--r--   0        0        0      722 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/list_integrations.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2519 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2398 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     3049 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/blueprints.py
--rw-r--r--   0        0        0     5730 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3866 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      142 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2277 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/config/base.py
--rw-r--r--   0        0        0     1218 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/config/dynamic.py
--rw-r--r--   0        0        0     1107 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     4147 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/context/event.py
--rw-r--r--   0        0        0     4286 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/base.py
--rw-r--r--   0        0        0      593 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/__init__.py
--rw-r--r--   0        0        0      560 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/base.py
--rw-r--r--   0        0        0     3083 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/factory.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/http/__init__.py
--rw-r--r--   0        0        0     1197 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/http/event_listener.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/kafka/__init__.py
--rw-r--r--   0        0        0     3147 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/kafka/event_listener.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/sample/__init__.py
--rw-r--r--   0        0        0     1852 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/sample/event_listener.py
--rw-r--r--   0        0        0     2799 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/sample/utils.py
--rw-r--r--   0        0        0      716 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/__init__.py
--rw-r--r--   0        0        0      869 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/base.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/__init__.py
--rw-r--r--   0        0        0     7949 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/applier.py
--rw-r--r--   0        0        0     1339 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
--rw-r--r--   0        0        0      988 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     1392 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entity_processor/__init__.py
--rw-r--r--   0        0        0      955 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entity_processor/base.py
--rw-r--r--   0        0        0     2685 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      396 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1810 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     1912 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      698 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2569 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0    11831 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0     1683 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/utils.py
--rw-r--r--   0        0        0     1368 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/models.py
--rw-r--r--   0        0        0      781 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/ocean_types.py
--rw-r--r--   0        0        0     1957 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      532 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      407 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/port_defaults.py
--rw-r--r--   0        0        0      554 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2475 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/middlewares.py
--rw-r--r--   0        0        0     2266 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/ocean.py
--rw-r--r--   0        0        0     7361 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/port_defaults.py
--rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/py.typed
--rw-r--r--   0        0        0     2837 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/run.py
--rw-r--r--   0        0        0     1007 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/utils.py
--rw-r--r--   0        0        0     2736 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/pyproject.toml
--rw-r--r--   0        0        0     6204 1970-01-01 00:00:00.000000 port_ocean-0.1.0rc5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 07:38:34.234947 port_ocean-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4639 2023-07-26 07:38:34.234947 port_ocean-0.1.1/README.md
+-rw-r--r--   0        0        0      270 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/__init__.py
+-rw-r--r--   0        0        0      328 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0      278 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1134 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/list_integrations.py
+-rw-r--r--   0        0        0     1057 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/main.py
+-rw-r--r--   0        0        0     1710 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/new.py
+-rw-r--r--   0        0        0     2306 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/pull.py
+-rw-r--r--   0        0        0     1537 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/sail.py
+-rw-r--r--   0        0        0      536 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/commands/version.py
+-rw-r--r--   0        0        0      429 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0       12 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
+-rw-r--r--   0        0        0      388 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      292 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      449 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1680 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      655 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
+-rw-r--r--   0        0        0      898 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       65 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1920 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/cli/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2563 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2309 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     2928 2023-07-26 07:38:34.242947 port_ocean-0.1.1/port_ocean/clients/port/mixins/blueprints.py
+-rw-r--r--   0        0        0     5623 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3909 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      781 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2277 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1218 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0     1107 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     4147 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4286 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/base.py
+-rw-r--r--   0        0        0      607 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0      560 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     2555 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0     1197 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/http/event_listener.py
+-rw-r--r--   0        0        0     3347 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/kafka/event_listener.py
+-rw-r--r--   0        0        0     1867 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/polling/event_listener.py
+-rw-r--r--   0        0        0     2799 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/event_listener/polling/utils.py
+-rw-r--r--   0        0        0      716 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0      869 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7977 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1339 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0      988 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0      955 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     2685 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1810 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     1912 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      698 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2569 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0    11831 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0     1683 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/integrations/mixins/utils.py
+-rw-r--r--   0        0        0     1368 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/models.py
+-rw-r--r--   0        0        0      781 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/ocean_types.py
+-rw-r--r--   0        0        0     1957 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      532 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      407 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/exceptions/port_defaults.py
+-rw-r--r--   0        0        0      554 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     2266 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/ocean.py
+-rw-r--r--   0        0        0     7164 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/port_defaults.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/py.typed
+-rw-r--r--   0        0        0     2837 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/run.py
+-rw-r--r--   0        0        0     1007 2023-07-26 07:38:34.246947 port_ocean-0.1.1/port_ocean/utils.py
+-rw-r--r--   0        0        0     3439 2023-07-26 07:38:34.246947 port_ocean-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 port_ocean-0.1.1/PKG-INFO
```

### Comparing `port_ocean-0.1.0rc5/LICENSE` & `port_ocean-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/README.md` & `port_ocean-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+<img src="./assets/Thumbnail.jpg" alt="Ocean">
+
+
 # Ocean <img src="./assets/OceanSymbol.svg" alt="Ocean" width="100" height="100" align="right">
 
 [![Lint](https://github.com/port-labs/Port-Ocean/actions/workflows/lint.yml/badge.svg)](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml)
 
 Ocean is an innovative solution developed by Port to seamlessly integrate various third-party systems with our developer portal product,
 empowering engineers to effortlessly prioritize key features and streamline the integration process.
 
@@ -31,24 +34,30 @@
    ```sh
    . .venv/bin/activate
    ```
 
 2. Run
 
    ```sh
-   ocean sail ./path/to/integration
+   ocean sail ./path/to/
+   integration
    ```
 
 # Export Architecture
 
 ![image](./assets/ExportArchitecture.svg)
 
 ## Real-Time updates Architecture
 ![image](./assets/RealTimeUpdatesArchitecture.svg)
 
+## Integration Lifecycle
+
+![image](./assets/LifecycleOfIntegration.svg)
+
+
 ## Folder Structure
 The Ocean Integration Framework follows a specific folder structure within this mono repository. This structure ensures proper organization and easy identification of integration modules. The suggested folder structure is as follows:
 
 ```
 port-ocean/
 ├── port_ocean (framework)/
 │ ├── ocean.py
@@ -64,18 +73,14 @@
 ```
 
 - The `framework` folder contains the core logic for managing the integration lifecycle.
 - Each integration is represented by a separate folder inside the `integrations` directory.
 - Inside each integration folder, you'll find a `main.py` file that implements the core functionality of the integration for the specific third-party system.
 - The `pyproject.toml` file inside each integration folder lists the required dependencies for that integration.
 
-## Integration Lifecycle
-
-![image](./assets/LifecycleOfIntegration.svg)
-
 ## Configuration
 The Integration Framework utilizes a `config.yaml` file for its configuration. This file defines both the framework configuration and the integration configuration within it. Each integration is identified by its type and unique identifier, which are utilized during initialization to appropriately update Port.
 
 Example `config.yaml`:
 ```yaml
 # This is an example configuration file for the integration service.
 # Please copy this file to config.yaml file in the integration folder and edit it to your needs.
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md` & `port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -37,11 +37,11 @@
 
 
 ## Folder Structure
 The {{cookiecutter.integration_name}} integration suggested folder structure is as follows:
 
 ```
 {{cookiecutter.integration_name}}/
-????? main.py
-????? pyproject.toml
-????? Dockerfile
-```
+├─ main.py
+├─ pyproject.toml
+└─ Dockerfile
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml` & `port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# This is an example configuration file for the integration service.
-# Please copy this file to config.yaml file in the integration folder and edit it to your needs.
+{{ "# This is an example configuration file for the integration service." }}
+{{ "# Please copy this file to config.yaml file in the integration folder and edit it to your needs." }}
 
 port:
-  clientId: {{ from env PORT_CLIENT_ID }} # Can be loaded via environment variable: PORT_CLIENT_ID
-  clientSecret: {{ from env PORT_CLIENT_SECRET }} # Can be loaded via environment variable: PORT_CLIENT_SECRET
-# The event listener to use for the integration service.
+  clientId: {{ "{{" }} from env PORT_CLIENT_ID {{ "}}" }} {{ "# Can be loaded via environment variable: PORT_CLIENT_ID" }}
+  clientSecret: {{ "{{" }} from env PORT_CLIENT_SECRET {{ "}}" }} {{ "# Can be loaded via environment variable: PORT_CLIENT_SECRET" }}
+{{ "# The event listener to use for the integration service." }}
 eventListener:
   type: KAFKA
 integration:
-  # The identifier of this integration instance.
-  identifier: {{ from env INTEGRATION_IDENTIFIER }}
-  # The type of the integration.
+  {{ "# The identifier of this integration instance." }}
+  identifier: {{ "{{" }} from env INTEGRATION_IDENTIFIER {{ "}}" }}
+  {{ "# The type of the integration." }}
   type: "My Integration type (Gitlab, Jira, etc.)"
   config:
-    myGitToken: {{ from env MY_GIT_TOKEN }}
+    myGitToken: {{ "{{" }} from env MY_GIT_TOKEN {{ "}}" }}
     someApplicationUrl: "https://I-Am-Not-A-Real-Url.com"
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.1.1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/cli/download_git_folder.py` & `port_ocean-0.1.1/port_ocean/cli/commands/list_integrations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,35 @@
-import os
-import shutil
-from io import BytesIO
-
+# -*- coding: utf-8 -*-
 import httpx
-from rich.console import Console
 
-console = Console()
+from port_ocean.cli.commands.main import cli_start, console
 
 
-def download_github_folder(
-    owner: str, repo_name: str, folder_path: str, destination_path: str
-) -> None:
+def list_git_folders(owner: str, repo_name: str, path: str) -> list[str]:
     # Construct the API URL to get the contents of the folder
-    api_url = f"https://api.github.com/repos/{owner}/{repo_name}/contents/{folder_path}"
+    api_url = f"https://api.github.com/repos/{owner}/{repo_name}/contents/{path}"
 
     # Send a GET request to the API
     response = httpx.get(api_url)
 
     # Check if the request was successful
     if response.is_error:
         console.print(
-            f"[bold red]Failed to download the folder `{folder_path}`.[/bold red] Status Code: {response.status_code}, Error: {response.text}"
+            f"[bold red]Failed to list folders.[/bold red] Status Code: {response.status_code}, Error: {response.text}"
         )
         exit(1)
 
-    # Create the destination folder if it doesn't exist
-    if not os.path.exists(destination_path):
-        os.makedirs(destination_path)
-
-    # Iterate over the files and download them
-    repo_contents = response.json()
-    for content in repo_contents:
-        if content["type"] == "file":
-            file_url = content["download_url"]
-            file_name = os.path.join(destination_path, content["name"])
-
-            # Download the file
-            with httpx.stream("GET", file_url) as file_response:
-                if file_response.status_code == 200:
-                    with open(file_name, "wb") as file:
-                        shutil.copyfileobj(BytesIO(file_response.content), file)
-                else:
-                    console.print(
-                        f"[bold red]Failed to download file `{content['name']}`.[/bold red] Status code: {file_response.status_code}, Error: {file_response.text}"
-                    )
-                    exit(1)
+    contents = response.json()
+    folders = [item["name"] for item in contents if item["type"] == "dir"]
+    return folders
+
+
+@cli_start.command(name="list")
+def list_integrations() -> None:
+    """
+    List all available public integrations.
+    """
+    console.print("🌊 Here are the integrations available to you:", style="bold")
+    options = list_git_folders("port-labs", "port-ocean", "integrations")
 
-    console.print(f"Folder `{folder_path}` downloaded successfully!")
+    for option in options:
+        console.print(f"⚓️ [bold][blue]{option}[/blue][/bold]")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.1/port_ocean/clients/port/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any
 
 import httpx
 from loguru import logger
 from pydantic import BaseModel, Field, PrivateAttr
 
 from port_ocean.clients.port.types import UserAgentType
+from port_ocean.clients.port.utils import handle_status_code
 from port_ocean.utils import get_time
 
 
 class TokenResponse(BaseModel):
     access_token: str = Field(alias="accessToken")
     expires_in: int = Field(alias="expiresIn")
     token_type: str = Field(alias="tokenType")
@@ -41,19 +42,19 @@
         self.integration_type = integration_type
         self._last_token_object: TokenResponse | None = None
 
     async def _get_token(self, client_id: str, client_secret: str) -> TokenResponse:
         logger.info(f"Fetching access token for clientId: {client_id}")
 
         credentials = {"clientId": client_id, "clientSecret": client_secret}
-        token_response = await self.client.post(
+        response = await self.client.post(
             f"{self.api_url}/auth/access_token", json=credentials
         )
-        token_response.raise_for_status()
-        return TokenResponse(**token_response.json())
+        handle_status_code(response)
+        return TokenResponse(**response.json())
 
     def user_agent(self, user_agent_type: UserAgentType | None = None) -> str:
         user_agent = f"port-ocean/{self.integration_type}/{self.integration_identifier}"
         if user_agent_type:
             user_agent += f"/{user_agent_type.value or UserAgentType.exporter.value}"
 
         return user_agent
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/clients/port/client.py` & `port_ocean-0.1.1/port_ocean/clients/port/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,53 @@
-import httpx as httpx
 from loguru import logger
 
 from port_ocean.clients.port.authentication import PortAuthentication
 from port_ocean.clients.port.mixins.blueprints import BlueprintClientMixin
 from port_ocean.clients.port.mixins.entities import EntityClientMixin
 from port_ocean.clients.port.mixins.integrations import IntegrationClientMixin
 from port_ocean.clients.port.types import (
     KafkaCreds,
 )
-from port_ocean.clients.port.utils import handle_status_code
+from port_ocean.clients.port.utils import handle_status_code, http
 from port_ocean.exceptions.clients import KafkaCredentialsNotFound
 
 
 class PortClient(EntityClientMixin, IntegrationClientMixin, BlueprintClientMixin):
     def __init__(
         self,
         base_url: str,
         client_id: str,
         client_secret: str,
         integration_identifier: str,
         integration_type: str,
     ):
         self.api_url = f"{base_url}/v1"
-        self.client = httpx.AsyncClient()
+        self.client = http
         self.auth = PortAuthentication(
             self.client,
             client_id,
             client_secret,
             self.api_url,
             integration_identifier,
             integration_type,
         )
         EntityClientMixin.__init__(self, self.auth, self.client)
         IntegrationClientMixin.__init__(
             self, integration_identifier, self.auth, self.client
         )
         BlueprintClientMixin.__init__(self, self.auth, self.client)
 
-    async def get_kafka_creds(self, silent: bool = False) -> KafkaCreds:
+    async def get_kafka_creds(self) -> KafkaCreds:
         logger.info("Fetching organization kafka credentials")
         response = await self.client.get(
             f"{self.api_url}/kafka-credentials", headers=await self.auth.headers()
         )
         if response.is_error:
-            logger.error(f"Error getting kafka credentials, error: {response.text}")
-        handle_status_code(silent, response)
+            logger.error("Error getting kafka credentials")
+        handle_status_code(response)
 
         credentials = response.json().get("credentials")
 
         if credentials is None:
             raise KafkaCredentialsNotFound("No kafka credentials found")
 
         return credentials
@@ -57,10 +56,10 @@
         logger.info("Fetching organization id")
 
         response = await self.client.get(
             f"{self.api_url}/organization", headers=await self.auth.headers()
         )
         if response.is_error:
             logger.error(f"Error getting organization id, error: {response.text}")
-            response.raise_for_status()
+        handle_status_code(response)
 
         return response.json()["organization"]["id"]
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/blueprints.py` & `port_ocean-0.1.1/port_ocean/clients/port/mixins/blueprints.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,72 +9,74 @@
 
 
 class BlueprintClientMixin:
     def __init__(self, auth: PortAuthentication, client: httpx.AsyncClient):
         self.auth = auth
         self.client = client
 
-    async def get_blueprint(self, identifier: str, silent: bool = False) -> Blueprint:
+    async def get_blueprint(self, identifier: str) -> Blueprint:
         logger.info(f"Fetching blueprint with id: {identifier}")
         response = await self.client.get(
             f"{self.auth.api_url}/blueprints/{identifier}",
             headers=await self.auth.headers(),
         )
-        handle_status_code(silent, response)
+        handle_status_code(response)
         return Blueprint.parse_obj(response.json()["blueprint"])
 
-    async def create_blueprint(
-        self, raw_blueprint: dict[str, Any], silent: bool = False
-    ) -> None:
+    async def create_blueprint(self, raw_blueprint: dict[str, Any]) -> None:
         logger.info(f"Creating blueprint with id: {raw_blueprint.get('identifier')}")
         headers = await self.auth.headers()
         response = await self.client.post(
             f"{self.auth.api_url}/blueprints", headers=headers, json=raw_blueprint
         )
-        handle_status_code(silent, response)
+        handle_status_code(response)
         if response.is_success:
             return response.json()["blueprint"]
 
     async def patch_blueprint(
-        self, identifier: str, raw_blueprint: dict[str, Any], silent: bool = False
+        self, identifier: str, raw_blueprint: dict[str, Any]
     ) -> None:
         logger.info(f"Patching blueprint with id: {identifier}")
         headers = await self.auth.headers()
         response = await self.client.patch(
             f"{self.auth.api_url}/blueprints/{identifier}",
             headers=headers,
             json=raw_blueprint,
         )
-        handle_status_code(silent, response)
+        handle_status_code(response)
 
-    async def delete_blueprint(self, identifier: str, silent: bool = False) -> None:
+    async def delete_blueprint(
+        self, identifier: str, should_raise: bool = False
+    ) -> None:
         logger.info(f"Deleting blueprint with id: {identifier}")
         headers = await self.auth.headers()
         response = await self.client.delete(
             f"{self.auth.api_url}/blueprints/{identifier}",
             headers=headers,
         )
-        handle_status_code(silent, response)
+        handle_status_code(response, should_raise)
 
     async def create_action(
-        self, blueprint_identifier: str, action: dict[str, Any], silent: bool = False
+        self, blueprint_identifier: str, action: dict[str, Any]
     ) -> None:
         logger.info(f"Creating action: {action}")
         response = await self.client.post(
             f"{self.auth.api_url}/blueprints/{blueprint_identifier}/actions",
             json=action,
             headers=await self.auth.headers(),
         )
 
-        handle_status_code(silent, response)
+        handle_status_code(response)
 
     async def create_scorecard(
-        self, blueprint_identifier: str, scorecard: dict[str, Any], silent: bool = False
+        self,
+        blueprint_identifier: str,
+        scorecard: dict[str, Any],
     ) -> None:
         logger.info(f"Creating scorecard: {scorecard}")
         response = await self.client.post(
             f"{self.auth.api_url}/blueprints/{blueprint_identifier}/scorecards",
             json=scorecard,
             headers=await self.auth.headers(),
         )
 
-        handle_status_code(silent, response)
+        handle_status_code(response)
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.1/port_ocean/clients/port/mixins/entities.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.client = client
 
     async def upsert_entity(
         self,
         entity: Entity,
         request_options: RequestOptions,
         user_agent_type: UserAgentType | None = None,
-        silent: bool = False,
+        should_raise: bool = True,
     ) -> None:
         validation_only = request_options.get("validation_only", False)
         logger.info(
             f"{'Validating' if validation_only else 'Upserting'} entity: {entity.identifier} of blueprint: {entity.blueprint}"
         )
         headers = await self.auth.headers(user_agent_type)
 
@@ -41,25 +41,24 @@
             },
         )
 
         if response.is_error:
             logger.error(
                 f"Error {'Validating' if validation_only else 'Upserting'} "
                 f"entity: {entity.identifier} of "
-                f"blueprint: {entity.blueprint}, "
-                f"error: {response.text}"
+                f"blueprint: {entity.blueprint}"
             )
-        handle_status_code(silent, response)
+        handle_status_code(response, should_raise)
 
     async def delete_entity(
         self,
         entity: Entity,
         request_options: RequestOptions,
         user_agent_type: UserAgentType | None = None,
-        silent: bool = False,
+        should_raise: bool = True,
     ) -> None:
         logger.info(
             f"Delete entity: {entity.identifier} of blueprint: {entity.blueprint}"
         )
         response = await self.client.delete(
             f"{self.auth.api_url}/blueprints/{entity.blueprint}/entities/{quote_plus(entity.identifier)}",
             headers=await self.auth.headers(user_agent_type),
@@ -70,35 +69,33 @@
             },
         )
 
         if response.is_error:
             logger.error(
                 f"Error deleting "
                 f"entity: {entity.identifier} of "
-                f"blueprint: {entity.blueprint}, "
-                f"error: {response.text}"
+                f"blueprint: {entity.blueprint}"
             )
 
-        handle_status_code(silent, response)
+        handle_status_code(response, should_raise)
 
     async def validate_entity_exist(self, identifier: str, blueprint: str) -> None:
         logger.info(f"Validating entity {identifier} of blueprint {blueprint} exists")
 
         response = await self.client.get(
             f"{self.auth.api_url}/blueprints/{blueprint}/entities/{identifier}",
             headers=await self.auth.headers(),
         )
         if response.is_error:
             logger.error(
                 f"Error validating "
                 f"entity: {identifier} of "
-                f"blueprint: {blueprint}, "
-                f"error: {response.text}"
+                f"blueprint: {blueprint}"
             )
-        response.raise_for_status()
+        handle_status_code(response)
 
     async def search_entities(self, user_agent_type: UserAgentType) -> list[Entity]:
         query = {
             "combinator": "and",
             "rules": [
                 {
                     "property": "$datasource",
@@ -114,15 +111,15 @@
             json=query,
             headers=await self.auth.headers(user_agent_type),
             params={
                 "exclude_calculated_properties": "true",
                 "include": ["blueprint", "identifier"],
             },
         )
-        response.raise_for_status()
+        handle_status_code(response)
         return [Entity.parse_obj(result) for result in response.json()["entities"]]
 
     async def search_dependent_entities(self, entity: Entity) -> list[Entity]:
         body = {
             "combinator": "and",
             "rules": [
                 {
@@ -136,15 +133,15 @@
 
         logger.info(f"Searching dependent entity with body {body}")
         response = await self.client.post(
             f"{self.auth.api_url}/entities/search",
             headers=await self.auth.headers(),
             json=body,
         )
-        response.raise_for_status()
+        handle_status_code(response)
 
         return [Entity.parse_obj(result) for result in response.json()["entities"]]
 
     async def validate_entity_payload(
         self, entity: Entity, options: RequestOptions
     ) -> None:
         logger.info(f"Validating entity {entity.identifier}")
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.1/port_ocean/clients/port/mixins/integrations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, TYPE_CHECKING, Optional
 
 import httpx
 from loguru import logger
 from starlette import status
 
 from port_ocean.clients.port.authentication import PortAuthentication
+from port_ocean.clients.port.utils import handle_status_code
 
 if TYPE_CHECKING:
     from port_ocean.core.handlers.port_app_config.models import PortAppConfig
 
 
 class IntegrationClientMixin:
     def __init__(
@@ -17,42 +18,47 @@
         auth: PortAuthentication,
         client: httpx.AsyncClient,
     ):
         self.integration_identifier = integration_identifier
         self.auth = auth
         self.client = client
 
-    async def get_current_integration(self) -> dict[str, Any]:
+    async def _get_current_integration(self) -> httpx.Response:
         logger.info(f"Fetching integration with id: {self.integration_identifier}")
         response = await self.client.get(
             f"{self.auth.api_url}/integration/{self.integration_identifier}",
             headers=await self.auth.headers(),
         )
-        response.raise_for_status()
+        return response
+
+    async def get_current_integration(self) -> dict[str, Any]:
+        response = await self._get_current_integration()
+        handle_status_code(response)
         return response.json()["integration"]
 
     async def create_integration(
         self,
         _type: str,
         changelog_destination: dict[str, Any],
         port_app_config: Optional["PortAppConfig"] = None,
     ) -> None:
         logger.info(f"Creating integration with id: {self.integration_identifier}")
         headers = await self.auth.headers()
         json = {
             "installationId": self.integration_identifier,
             "installationAppType": _type,
             "changelogDestination": changelog_destination,
+            "config": {},
         }
         if port_app_config:
             json["config"] = port_app_config.to_request()
         response = await self.client.post(
             f"{self.auth.api_url}/integration", headers=headers, json=json
         )
-        response.raise_for_status()
+        handle_status_code(response)
 
     async def patch_integration(
         self,
         _type: str | None = None,
         changelog_destination: dict[str, Any] | None = None,
         port_app_config: Optional["PortAppConfig"] = None,
     ) -> None:
@@ -67,42 +73,35 @@
             json["config"] = port_app_config.to_request()
 
         response = await self.client.patch(
             f"{self.auth.api_url}/integration/{self.integration_identifier}",
             headers=headers,
             json=json,
         )
-        response.raise_for_status()
+        handle_status_code(response)
 
     async def initialize_integration(
         self,
         _type: str,
         changelog_destination: dict[str, Any],
         port_app_config: Optional["PortAppConfig"] = None,
     ) -> None:
         logger.info(f"Initiating integration with id: {self.integration_identifier}")
-        try:
-            integration = await self.get_current_integration()
+        response = await self._get_current_integration()
+        if response.status_code == status.HTTP_404_NOT_FOUND:
+            await self.create_integration(_type, changelog_destination, port_app_config)
+        else:
+            handle_status_code(response)
 
+            integration = response.json()["integration"]
             logger.info("Checking for diff in integration configuration")
             if (
                 integration["changelogDestination"] != changelog_destination
                 or integration["installationAppType"] != _type
             ):
                 await self.patch_integration(
                     _type, changelog_destination, port_app_config
                 )
-        except httpx.HTTPStatusError as e:
-            if e.response.status_code == status.HTTP_404_NOT_FOUND:
-                await self.create_integration(
-                    _type, changelog_destination, port_app_config
-                )
-                return
-
-            logger.error(
-                f"Error initiating integration with id: {self.integration_identifier}, error: {e.response.text}"
-            )
-            raise
 
         logger.info(
             f"Integration with id: {self.integration_identifier} successfully registered"
         )
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/clients/port/types.py` & `port_ocean-0.1.1/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/config/base.py` & `port_ocean-0.1.1/port_ocean/config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/config/dynamic.py` & `port_ocean-0.1.1/port_ocean/config/dynamic.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/config/integration.py` & `port_ocean-0.1.1/port_ocean/config/integration.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.1/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/context/event.py` & `port_ocean-0.1.1/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/context/ocean.py` & `port_ocean-0.1.1/port_ocean/context/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/event_listener/base.py` & `port_ocean-0.1.1/port_ocean/core/event_listener/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/event_listener/factory.py` & `port_ocean-0.1.1/port_ocean/core/event_listener/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from typing import Callable, Any, Awaitable
-
 from loguru import logger
 
 from port_ocean.context.ocean import PortOceanContext
 from port_ocean.core.base import BaseWithContext
 from port_ocean.core.event_listener import (
     HttpEventListener,
     KafkaEventListener,
-    SampleEventListener,
+    PollingEventListener,
 )
 from port_ocean.core.event_listener import (
     HttpEventListenerSettings,
     KafkaEventListenerSettings,
-    SampleEventListenerSettings,
+    PollingEventListenerSettings,
 )
 from port_ocean.core.event_listener.base import (
     BaseEventListener,
     EventListenerEvents,
 )
 from port_ocean.exceptions.core import UnsupportedEventListenerTypeException
 
@@ -28,31 +26,16 @@
         installation_id: str,
         events: EventListenerEvents,
     ):
         super().__init__(context)
         self.installation_id = installation_id
         self.events = events
 
-    def on_event(
-        self, callback: Callable[[dict[Any, Any]], Awaitable[None]]
-    ) -> Callable[[dict[Any, Any]], Awaitable[None]]:
-        async def wrapper(event: dict[Any, Any]) -> None:
-            integration_identifier = (
-                event.get("diff", {}).get("after", {}).get("identifier")
-            )
-
-            if integration_identifier == self.installation_id:
-                await callback(event)
-
-        return wrapper
-
     async def create_event_listener(self) -> BaseEventListener:
-        wrapped_events: EventListenerEvents = {
-            "on_resync": self.on_event(self.events["on_resync"])
-        }
+        wrapped_events: EventListenerEvents = {"on_resync": self.events["on_resync"]}
         event_listener: BaseEventListener
         config = self.context.config.event_listener
         _type = config.type.lower()
         assert_message = "Invalid event listener config, expected KafkaEventListenerSettings and got {0}"
         logger.info(f"Found event listener type: {_type}")
 
         match _type:
@@ -71,19 +54,19 @@
 
             case "webhook":
                 assert isinstance(
                     config, HttpEventListenerSettings
                 ), assert_message.format(type(config))
                 event_listener = HttpEventListener(wrapped_events, config)
 
-            case "sample":
+            case "polling":
                 assert isinstance(
-                    config, SampleEventListenerSettings
+                    config, PollingEventListenerSettings
                 ), assert_message.format(type(config))
-                event_listener = SampleEventListener(wrapped_events, config)
+                event_listener = PollingEventListener(wrapped_events, config)
 
             case _:
                 raise UnsupportedEventListenerTypeException(
                     f"Event listener {_type} not supported"
                 )
 
         return event_listener
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/event_listener/http/event_listener.py` & `port_ocean-0.1.1/port_ocean/core/event_listener/http/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/event_listener/kafka/event_listener.py` & `port_ocean-0.1.1/port_ocean/core/event_listener/kafka/event_listener.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,15 +52,20 @@
                 password=creds.get("password"),
                 group_name=f"{self.integration_type}.{self.integration_identifier}",
             )
 
         return KafkaConsumerConfig.parse_obj(self.event_listener_config.dict())
 
     def should_be_processed(self, msg_value: dict[Any, Any], topic: str) -> bool:
-        if "change.log" in topic:
+        integration_identifier = (
+            msg_value.get("diff", {}).get("after", {}).get("identifier")
+        )
+        if integration_identifier == self.integration_identifier and (
+            "change.log" in topic
+        ):
             return msg_value.get("changelogDestination", {}).get("type", "") == "KAFKA"
 
         return False
 
     async def _handle_message(self, message: dict[Any, Any], topic: str) -> None:
         if not self.should_be_processed(message, topic):
             return
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/event_listener/sample/event_listener.py` & `port_ocean-0.1.1/port_ocean/core/event_listener/polling/event_listener.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,54 +4,54 @@
 
 from port_ocean.context.ocean import ocean
 from port_ocean.core.event_listener.base import (
     BaseEventListener,
     EventListenerEvents,
     EventListenerSettings,
 )
-from port_ocean.core.event_listener.sample.utils import repeat_every
+from port_ocean.core.event_listener.polling.utils import repeat_every
 
 
-class SampleEventListenerSettings(EventListenerSettings):
-    type: Literal["SAMPLE"]
+class PollingEventListenerSettings(EventListenerSettings):
+    type: Literal["POLLING"]
     resync_on_start: bool = True
     interval: int = 60
 
     def to_request(self) -> dict[str, Any]:
         return {}
 
 
-class SampleEventListener(BaseEventListener):
+class PollingEventListener(BaseEventListener):
     def __init__(
         self,
         events: EventListenerEvents,
-        event_listener_config: SampleEventListenerSettings,
+        event_listener_config: PollingEventListenerSettings,
     ):
         super().__init__(events)
         self.event_listener_config = event_listener_config
         self._last_updated_at = None
 
     async def start(self) -> None:
         logger.info(
-            f"Setting up Sample event listener with interval: {self.event_listener_config.interval}"
+            f"Setting up Polling event listener with interval: {self.event_listener_config.interval}"
         )
 
         @repeat_every(seconds=self.event_listener_config.interval)
         async def resync() -> None:
             logger.info(
-                f"Sample event listener iteration after {self.event_listener_config.interval}. Checking for changes"
+                f"Polling event listener iteration after {self.event_listener_config.interval}. Checking for changes"
             )
             integration = await ocean.app.port_client.get_current_integration()
             last_updated_at = integration["updatedAt"]
 
             should_resync = (
                 self._last_updated_at is not None
                 or self.event_listener_config.resync_on_start
             ) and self._last_updated_at != last_updated_at
 
             if should_resync:
                 logger.info("Detected change in integration, resyncing")
                 self._last_updated_at = last_updated_at
-                await ocean.sync_raw_all()
+                await self.events["on_resync"]({})
 
         # Execute resync repeatedly task
         await resync()
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/event_listener/sample/utils.py` & `port_ocean-0.1.1/port_ocean/core/event_listener/polling/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/handlers/__init__.py` & `port_ocean-0.1.1/port_ocean/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/base.py` & `port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/applier.py` & `port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         if event.port_app_config.create_missing_related_entities:
             await asyncio.gather(
                 *(
                     self.context.port_client.upsert_entity(
                         entity,
                         event.port_app_config.get_port_request_options(),
                         user_agent_type,
-                        silent=True,
+                        should_raise=False,
                     )
                     for entity in entities
                 ),
                 return_exceptions=True,
             )
         else:
             ordered_created_entities = reversed(
@@ -171,36 +171,36 @@
             )
 
             for entity in ordered_created_entities:
                 await self.context.port_client.upsert_entity(
                     entity,
                     event.port_app_config.get_port_request_options(),
                     user_agent_type,
-                    silent=True,
+                    should_raise=False,
                 )
 
     async def delete(
         self, entities: list[Entity], user_agent_type: UserAgentType
     ) -> None:
         logger.info(f"Deleting {len(entities)} entities")
         if event.port_app_config.delete_dependent_entities:
             await asyncio.gather(
                 *(
                     self.context.port_client.delete_entity(
                         entity,
                         event.port_app_config.get_port_request_options(),
                         user_agent_type,
-                        silent=True,
+                        should_raise=False,
                     )
                     for entity in entities
                 )
             )
         else:
             ordered_deleted_entities = order_by_entities_dependencies(entities)
 
             for entity in ordered_deleted_entities:
                 await self.context.port_client.delete_entity(
                     entity,
                     event.port_app_config.get_port_request_options(),
                     user_agent_type,
-                    silent=True,
+                    should_raise=False,
                 )
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py` & `port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py` & `port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py` & `port_ocean-0.1.1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/handlers/entity_processor/base.py` & `port_ocean-0.1.1/port_ocean/core/handlers/entity_processor/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/handlers/entity_processor/jq_entity_processor.py` & `port_ocean-0.1.1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.1/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.1/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/integrations/base.py` & `port_ocean-0.1.1/port_ocean/core/integrations/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.1/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.1/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.1/port_ocean/core/integrations/mixins/sync.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/utils.py` & `port_ocean-0.1.1/port_ocean/core/integrations/mixins/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/models.py` & `port_ocean-0.1.1/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/ocean_types.py` & `port_ocean-0.1.1/port_ocean/core/ocean_types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/core/utils.py` & `port_ocean-0.1.1/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/exceptions/core.py` & `port_ocean-0.1.1/port_ocean/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/logger_setup.py` & `port_ocean-0.1.1/port_ocean/logger_setup.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/middlewares.py` & `port_ocean-0.1.1/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/ocean.py` & `port_ocean-0.1.1/port_ocean/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/port_defaults.py` & `port_ocean-0.1.1/port_ocean/port_defaults.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import asyncio
 import json
+from pathlib import Path
 from typing import Type, Any, TypedDict, Optional
 
 import httpx
 import yaml
 from loguru import logger
-from pathlib import Path
 from pydantic import BaseModel, Field
 from starlette import status
 
 from port_ocean.clients.port.client import PortClient
 from port_ocean.config.integration import IntegrationConfiguration
+from port_ocean.context.ocean import ocean
 from port_ocean.core.handlers.port_app_config.models import PortAppConfig
 from port_ocean.exceptions.port_defaults import (
     AbortDefaultCreationError,
     UnsupportedDefaultFileType,
 )
 
 YAML_EXTENSIONS = [".yaml", ".yml"]
@@ -146,21 +147,15 @@
         )
         raise AbortDefaultCreationError(created_blueprints, [e])
 
 
 async def _initialize_defaults(
     config_class: Type[PortAppConfig], integration_config: IntegrationConfiguration
 ) -> None:
-    port_client = PortClient(
-        base_url=integration_config.port.base_url,
-        client_id=integration_config.port.client_id,
-        client_secret=integration_config.port.client_secret,
-        integration_identifier=integration_config.integration.identifier,
-        integration_type=integration_config.integration.type,
-    )
+    port_client = ocean.port_client
     is_exists = await _is_integration_exists(port_client)
     if is_exists:
         return None
     defaults = get_port_integration_defaults(config_class)
     if not defaults:
         return None
 
@@ -168,15 +163,17 @@
         await _create_resources(port_client, defaults, integration_config)
     except AbortDefaultCreationError as e:
         logger.warning(
             f"Failed to create resources. Rolling back blueprints : {e.blueprints_to_rollback}"
         )
         await asyncio.gather(
             *(
-                port_client.delete_blueprint(blueprint["identifier"], silent=True)
+                port_client.delete_blueprint(
+                    blueprint["identifier"], should_raise=False
+                )
                 for blueprint in defaults.blueprints
             )
         )
 
         raise ExceptionGroup(str(e), e.errors)
 
 
@@ -204,20 +201,20 @@
         )
 
     default_jsons = {}
     allowed_file_names = [
         field_model.alias for _, field_model in Defaults.__fields__.items()
     ]
     for path in defaults_dir.iterdir():
-        if not path.is_file() or path.suffix not in ALLOWED_FILE_TYPES:
-            raise UnsupportedDefaultFileType(
-                f"Defaults directory should contain only one of the next types: {ALLOWED_FILE_TYPES}. Found: {path}"
-            )
-
         if path.stem in allowed_file_names:
+            if not path.is_file() or path.suffix not in ALLOWED_FILE_TYPES:
+                raise UnsupportedDefaultFileType(
+                    f"Defaults directory should contain only one of the next types: {ALLOWED_FILE_TYPES}. Found: {path}"
+                )
+
             if path.suffix in YAML_EXTENSIONS:
                 default_jsons[path.stem] = yaml.safe_load(path.read_text())
             else:
                 default_jsons[path.stem] = json.loads(path.read_text())
 
     return Defaults(
         blueprints=default_jsons.get("blueprints", []),
```

### Comparing `port_ocean-0.1.0rc5/port_ocean/run.py` & `port_ocean-0.1.1/port_ocean/run.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/port_ocean/utils.py` & `port_ocean-0.1.1/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc5/pyproject.toml` & `port_ocean-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.0.rc5"
+version = "0.1.1"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 homepage = "https://app.getport.io"
 repository = "https://github.com/port-labs/Port-Ocean"
 
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
@@ -48,39 +48,72 @@
 urllib3 = "^1.26.16"
 six = "^1.16.0"
 
 # CLI
 click = { version = "^8.1.3", optional = true }
 rich = { version = "^13.4.1", optional = true }
 cookiecutter = { version = "^2.1.1", optional = true }
+jinja2-time = { version = "^0.2.0", optional = true }
 
 [tool.poetry.extras]
-cli = ["click", "rich", "cookiecutter"]
+cli = ["click", "rich", "cookiecutter", "jinja2-time"]
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
 black = "^23.3.0"
 mypy = "^1.3.0"
 pylint = "^2.17.4"
 types-pyyaml = "^6.0.12.10"
 ruff = "^0.0.278"
 types-toml = "^0.10.8.6"
 towncrier = "^23.6.0"
 
 [tool.towncrier]
-directory = "changelog_fragments"
+directory = "changelog"
 filename = "CHANGELOG.md"
+title_format = "{version} ({project_date})"
+package_dir = "."
 package = "port_ocean"
 
+  [[tool.towncrier.type]]
+  directory = "breaking"
+  name = "Breaking Changes"
+  showcontent = true
+
+  [[tool.towncrier.type]]
+  directory = "deprecation"
+  name = "Deprecations"
+  showcontent = true
+
+  [[tool.towncrier.type]]
+  directory = "feature"
+  name = "Features"
+  showcontent = true
+
+  [[tool.towncrier.type]]
+  directory = "improvement"
+  name = "Improvements"
+  showcontent = true
+
+  [[tool.towncrier.type]]
+  directory = "bugfix"
+  name = "Bug Fixes"
+  showcontent = true
+
+  [[tool.towncrier.type]]
+  directory = "doc"
+  name = "Improved Documentation"
+  showcontent = true
+
 [tool.mypy]
 exclude = [
     'port_ocean/cli/cookiecutter',
     'venv',
-    '\.venv',
+    '.venv',
     'integrations'
 ]
 plugins = [
     "pydantic.mypy"
 ]
 
 follow_imports = "silent"
```

### Comparing `port_ocean-0.1.0rc5/PKG-INFO` & `port_ocean-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.0rc5
+Version: 0.1.1
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Home-page: https://app.getport.io
 Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: FastAPI
@@ -21,26 +21,30 @@
 Classifier: Topic :: Utilities
 Provides-Extra: cli
 Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "cli"
 Requires-Dist: confluent-kafka (>=2.1.1,<3.0.0)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0) ; extra == "cli"
 Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: jinja2-time (>=0.2.0,<0.3.0) ; extra == "cli"
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pyjq (>=2.6.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0) ; extra == "cli"
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: werkzeug (>=2.3.4,<3.0.0)
 Project-URL: Repository, https://github.com/port-labs/Port-Ocean
 Description-Content-Type: text/markdown
 
+<img src="./assets/Thumbnail.jpg" alt="Ocean">
+
+
 # Ocean <img src="./assets/OceanSymbol.svg" alt="Ocean" width="100" height="100" align="right">
 
 [![Lint](https://github.com/port-labs/Port-Ocean/actions/workflows/lint.yml/badge.svg)](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml)
 
 Ocean is an innovative solution developed by Port to seamlessly integrate various third-party systems with our developer portal product,
 empowering engineers to effortlessly prioritize key features and streamline the integration process.
 
@@ -70,24 +74,30 @@
    ```sh
    . .venv/bin/activate
    ```
 
 2. Run
 
    ```sh
-   ocean sail ./path/to/integration
+   ocean sail ./path/to/
+   integration
    ```
 
 # Export Architecture
 
 ![image](./assets/ExportArchitecture.svg)
 
 ## Real-Time updates Architecture
 ![image](./assets/RealTimeUpdatesArchitecture.svg)
 
+## Integration Lifecycle
+
+![image](./assets/LifecycleOfIntegration.svg)
+
+
 ## Folder Structure
 The Ocean Integration Framework follows a specific folder structure within this mono repository. This structure ensures proper organization and easy identification of integration modules. The suggested folder structure is as follows:
 
 ```
 port-ocean/
 ├── port_ocean (framework)/
 │ ├── ocean.py
@@ -103,18 +113,14 @@
 ```
 
 - The `framework` folder contains the core logic for managing the integration lifecycle.
 - Each integration is represented by a separate folder inside the `integrations` directory.
 - Inside each integration folder, you'll find a `main.py` file that implements the core functionality of the integration for the specific third-party system.
 - The `pyproject.toml` file inside each integration folder lists the required dependencies for that integration.
 
-## Integration Lifecycle
-
-![image](./assets/LifecycleOfIntegration.svg)
-
 ## Configuration
 The Integration Framework utilizes a `config.yaml` file for its configuration. This file defines both the framework configuration and the integration configuration within it. Each integration is identified by its type and unique identifier, which are utilized during initialization to appropriately update Port.
 
 Example `config.yaml`:
 ```yaml
 # This is an example configuration file for the integration service.
 # Please copy this file to config.yaml file in the integration folder and edit it to your needs.
```

