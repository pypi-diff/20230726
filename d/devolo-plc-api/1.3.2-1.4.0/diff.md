# Comparing `tmp/devolo_plc_api-1.3.2.tar.gz` & `tmp/devolo_plc_api-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devolo_plc_api-1.3.2.tar", last modified: Thu Jul 13 19:54:47 2023, max compression
+gzip compressed data, was "devolo_plc_api-1.4.0.tar", last modified: Wed Jul 26 07:00:15 2023, max compression
```

## Comparing `devolo_plc_api-1.3.2.tar` & `devolo_plc_api-1.4.0.tar`

### file list

```diff
@@ -1,95 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.509129 devolo_plc_api-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.481129 devolo_plc_api-1.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.481129 devolo_plc_api-1.3.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.481129 devolo_plc_api-1.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/workflows/convert_todos_to_issues.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-07-13 19:54:47.509129 devolo_plc_api-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.485128 devolo_plc_api-1.3.2/devolo_plc_api/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.489129 devolo_plc_api-1.3.2/devolo_plc_api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/clients/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.497129 devolo_plc_api-1.3.2/devolo_plc_api/device_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/deviceapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/deviceapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/factoryreset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/factoryreset_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/ledsettings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/ledsettings_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/multiap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/multiap_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/restart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/restart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/support_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/support_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/updatefirmware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/updatefirmware_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/wifinetwork_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/wifinetwork_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.497129 devolo_plc_api-1.3.2/devolo_plc_api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/exceptions/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/exceptions/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.497129 devolo_plc_api-1.3.2/devolo_plc_api/network/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.501129 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/identifydevice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/pairdevice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/plcnetapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/plcnetapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.501129 devolo_plc_api-1.3.2/devolo_plc_api/zeroconf/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/zeroconf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.489129 devolo_plc_api-1.3.2/devolo_plc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-07-13 19:54:47.000000 devolo_plc_api-1.3.2/devolo_plc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-13 19:54:47.000000 devolo_plc_api-1.3.2/devolo_plc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:54:47.000000 devolo_plc_api-1.3.2/devolo_plc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-13 19:54:47.000000 devolo_plc_api-1.3.2/devolo_plc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 19:54:47.000000 devolo_plc_api-1.3.2/devolo_plc_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.501129 devolo_plc_api-1.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/example_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/example_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.505129 devolo_plc_api-1.3.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4419 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/scripts/stubgen.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:54:47.509129 devolo_plc_api-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.505129 devolo_plc_api-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.509129 devolo_plc_api-1.3.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/fixtures/device_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/fixtures/plcnet_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.509129 devolo_plc_api-1.3.2/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/mocks/zeroconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.509129 devolo_plc_api-1.3.2/tests/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/snapshots/test_device.ambr
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/test_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/test_deviceapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/test_plcnetapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.182988 devolo_plc_api-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.170988 devolo_plc_api-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.170988 devolo_plc_api-1.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.170988 devolo_plc_api-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/.github/workflows/convert_todos_to_issues.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    45002 2023-07-26 07:00:15.178988 devolo_plc_api-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.170988 devolo_plc_api-1.4.0/devolo_plc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.174988 devolo_plc_api-1.4.0/devolo_plc_api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/clients/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11682 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.174988 devolo_plc_api-1.4.0/devolo_plc_api/device_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/deviceapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/deviceapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/factoryreset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/factoryreset_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/ledsettings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/ledsettings_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/multiap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/multiap_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/restart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/restart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/support_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/support_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/updatefirmware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/updatefirmware_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/wifinetwork_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/device_api/wifinetwork_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.174988 devolo_plc_api-1.4.0/devolo_plc_api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/exceptions/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/exceptions/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.174988 devolo_plc_api-1.4.0/devolo_plc_api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.174988 devolo_plc_api-1.4.0/devolo_plc_api/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.178988 devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/identifydevice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/pairdevice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/plcnetapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/plcnetapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.178988 devolo_plc_api-1.4.0/devolo_plc_api/zeroconf/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/devolo_plc_api/zeroconf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.174988 devolo_plc_api-1.4.0/devolo_plc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45002 2023-07-26 07:00:15.000000 devolo_plc_api-1.4.0/devolo_plc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-26 07:00:15.000000 devolo_plc_api-1.4.0/devolo_plc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 07:00:15.000000 devolo_plc_api-1.4.0/devolo_plc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-26 07:00:15.000000 devolo_plc_api-1.4.0/devolo_plc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-26 07:00:15.000000 devolo_plc_api-1.4.0/devolo_plc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.178988 devolo_plc_api-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/example_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/example_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.178988 devolo_plc_api-1.4.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4419 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/scripts/stubgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 07:00:15.182988 devolo_plc_api-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.178988 devolo_plc_api-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.178988 devolo_plc_api-1.4.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/fixtures/device_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/fixtures/plcnet_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.178988 devolo_plc_api-1.4.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/mocks/zeroconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:00:15.178988 devolo_plc_api-1.4.0/tests/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/snapshots/test_device.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/snapshots/test_helpers.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/test_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/test_deviceapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-07-26 06:59:58.000000 devolo_plc_api-1.4.0/tests/test_plcnetapi.py
```

### Comparing `devolo_plc_api-1.3.2/.github/ISSUE_TEMPLATE/bug_report.md` & `devolo_plc_api-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/.github/ISSUE_TEMPLATE/feature_request.md` & `devolo_plc_api-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/.github/workflows/pythonpackage.yml` & `devolo_plc_api-1.4.0/.github/workflows/pythonpackage.yml`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   format:
     name: Check formatting
     runs-on: ubuntu-latest
     steps:
     - name: Checkout sources
       uses: actions/checkout@v3.5.3
     - name: Set up Python
-      uses: actions/setup-python@v4.6.1
+      uses: actions/setup-python@v4.7.0
       with:
         python-version: "3.8"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install --no-binary=mypy mypy
     - name: Check formatting
@@ -24,15 +24,15 @@
   lint:
     name: Lint
     runs-on: ubuntu-latest
     steps:
     - name: Checkout sources
       uses: actions/checkout@v3.5.3
     - name: Set up Python
-      uses: actions/setup-python@v4.6.1
+      uses: actions/setup-python@v4.7.0
       with:
         python-version: "3.8"
     - name: Lint with ruff
       run: |
         python -m pip install --upgrade pip
         python -m pip install ruff
         ruff check --format=github devolo_plc_api scripts
@@ -49,15 +49,15 @@
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
     - name: Checkout sources
       uses: actions/checkout@v3.5.3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4.6.1
+      uses: actions/setup-python@v4.7.0
       with:
         python-version: ${{ matrix.python-version }}
         check-latest: true
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install -e .[test]
@@ -74,15 +74,15 @@
     name: Upload coverage
     runs-on: ubuntu-latest
     needs: test
     steps:
     - name: Checkout sources
       uses: actions/checkout@v3.5.3
     - name: Set up Python
-      uses: actions/setup-python@v4.6.1
+      uses: actions/setup-python@v4.7.0
       with:
         python-version: "3.8"
     - name: Download coverage
       uses: actions/download-artifact@v3.0.2
       with:
         name: coverage
     - name: Coveralls
```

### Comparing `devolo_plc_api-1.3.2/.github/workflows/pythonpublish.yml` & `devolo_plc_api-1.4.0/.github/workflows/pythonpublish.yml`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3.5.3
     - name: Set up Python
-      uses: actions/setup-python@v4.6.1
+      uses: actions/setup-python@v4.7.0
       with:
         python-version: "3.8"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install --upgrade build twine
     - name: Build and publish
```

### Comparing `devolo_plc_api-1.3.2/.gitignore` & `devolo_plc_api-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/.pre-commit-config.yaml` & `devolo_plc_api-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/LICENSE` & `devolo_plc_api-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/PKG-INFO` & `devolo_plc_api-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devolo_plc_api
-Version: 1.3.2
+Version: 1.4.0
 Summary: devolo PLC devices in Python
 Author-email: Markus Bong <m.bong@famabo.de>, Guido Schmitz <guido.schmitz@fedaix.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,15 +703,16 @@
 Defining the system requirements with exact versions typically is difficult. But there is a tested environment:
 
 * Linux
 * Python 3.8.12
 * pip 20.2.4
 * httpx 0.21.0
 * protobuf 3.17.3
-* zeroconf 0.36.8
+* segno 1.5.2
+* zeroconf 0.70.0
 
 Other versions and even other operating systems might work. Feel free to tell us about your experience. If you want to run our unit tests, you also need:
 
 * pytest 6.2.5
 * pytest-asyncio 0.15.1
 * pytest-httpx 0.18
```

### Comparing `devolo_plc_api-1.3.2/README.md` & `devolo_plc_api-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 Defining the system requirements with exact versions typically is difficult. But there is a tested environment:
 
 * Linux
 * Python 3.8.12
 * pip 20.2.4
 * httpx 0.21.0
 * protobuf 3.17.3
-* zeroconf 0.36.8
+* segno 1.5.2
+* zeroconf 0.70.0
 
 Other versions and even other operating systems might work. Feel free to tell us about your experience. If you want to run our unit tests, you also need:
 
 * pytest 6.2.5
 * pytest-asyncio 0.15.1
 * pytest-httpx 0.18
```

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/clients/protobuf.py` & `devolo_plc_api-1.4.0/devolo_plc_api/clients/protobuf.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device.py` & `devolo_plc_api-1.4.0/devolo_plc_api/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,21 +238,23 @@
         task = asyncio.create_task(self._get_service_info(zeroconf, service_type, name))
         self._background_tasks.add(task)
         task.add_done_callback(self._background_tasks.remove)
 
     async def _get_service_info(self, zeroconf: Zeroconf, service_type: str, name: str) -> None:
         """Get service information, if IP matches."""
         service_info = AsyncServiceInfo(service_type, name)
-        question_type = DNSQuestionType.QM if self._multicast else DNSQuestionType.QU
         update = {
             DEVICEAPI: self._get_device_info,
             PLCNETAPI: self._get_plcnet_info,
         }
         with suppress(RuntimeError):
-            await service_info.async_request(zeroconf, timeout=1000, question_type=question_type)
+            if not self._multicast:
+                await service_info.async_request(zeroconf, timeout=1000, question_type=DNSQuestionType.QU, addr=self.ip)
+            else:
+                await service_info.async_request(zeroconf, timeout=1000, question_type=DNSQuestionType.QM)
 
         if not service_info.addresses or self.ip not in service_info.parsed_addresses():
             return  # No need to continue, if there are no relevant service information
 
         self._logger.debug("Updating service info of %s for %s", service_type, service_info.server_key)
         if info := self.info_from_service(service_info):
             self._info[service_type] = info
```

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/__init__.py` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/deviceapi.py` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/deviceapi.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/deviceapi.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/deviceapi.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/factoryreset_pb2.py` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/factoryreset_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/factoryreset_pb2.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/factoryreset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/ledsettings_pb2.py` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/ledsettings_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/ledsettings_pb2.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/ledsettings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/multiap_pb2.py` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/multiap_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/multiap_pb2.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/multiap_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/restart_pb2.py` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/restart_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/restart_pb2.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/restart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/support_pb2.py` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/support_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/support_pb2.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/support_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/updatefirmware_pb2.py` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/updatefirmware_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/updatefirmware_pb2.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/updatefirmware_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/wifinetwork_pb2.py` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/wifinetwork_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/device_api/wifinetwork_pb2.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/device_api/wifinetwork_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/exceptions/device.py` & `devolo_plc_api-1.4.0/devolo_plc_api/exceptions/device.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/network/__init__.py` & `devolo_plc_api-1.4.0/devolo_plc_api/network/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/__init__.py` & `devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py` & `devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/identifydevice_pb2.py` & `devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/identifydevice_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/pairdevice_pb2.py` & `devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/pairdevice_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/plcnetapi.py` & `devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/plcnetapi.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/plcnetapi.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/plcnetapi.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py` & `devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi` & `devolo_plc_api-1.4.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api.egg-info/PKG-INFO` & `devolo_plc_api-1.4.0/devolo_plc_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devolo-plc-api
-Version: 1.3.2
+Version: 1.4.0
 Summary: devolo PLC devices in Python
 Author-email: Markus Bong <m.bong@famabo.de>, Guido Schmitz <guido.schmitz@fedaix.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,15 +703,16 @@
 Defining the system requirements with exact versions typically is difficult. But there is a tested environment:
 
 * Linux
 * Python 3.8.12
 * pip 20.2.4
 * httpx 0.21.0
 * protobuf 3.17.3
-* zeroconf 0.36.8
+* segno 1.5.2
+* zeroconf 0.70.0
 
 Other versions and even other operating systems might work. Feel free to tell us about your experience. If you want to run our unit tests, you also need:
 
 * pytest 6.2.5
 * pytest-asyncio 0.15.1
 * pytest-httpx 0.18
```

### Comparing `devolo_plc_api-1.3.2/devolo_plc_api.egg-info/SOURCES.txt` & `devolo_plc_api-1.4.0/devolo_plc_api.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 devolo_plc_api/device_api/updatefirmware_pb2.py
 devolo_plc_api/device_api/updatefirmware_pb2.pyi
 devolo_plc_api/device_api/wifinetwork_pb2.py
 devolo_plc_api/device_api/wifinetwork_pb2.pyi
 devolo_plc_api/exceptions/__init__.py
 devolo_plc_api/exceptions/device.py
 devolo_plc_api/exceptions/feature.py
+devolo_plc_api/helpers/__init__.py
 devolo_plc_api/network/__init__.py
 devolo_plc_api/plcnet_api/__init__.py
 devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py
 devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi
 devolo_plc_api/plcnet_api/identifydevice_pb2.py
 devolo_plc_api/plcnet_api/identifydevice_pb2.pyi
 devolo_plc_api/plcnet_api/pairdevice_pb2.py
@@ -61,15 +62,17 @@
 docs/CONTRIBUTING.md
 scripts/stubgen.py
 tests/__init__.py
 tests/conftest.py
 tests/test_data.json
 tests/test_device.py
 tests/test_deviceapi.py
+tests/test_helpers.py
 tests/test_network.py
 tests/test_plcnetapi.py
 tests/fixtures/__init__.py
 tests/fixtures/device_api.py
 tests/fixtures/plcnet_api.py
 tests/mocks/__init__.py
 tests/mocks/zeroconf.py
-tests/snapshots/test_device.ambr
+tests/snapshots/test_device.ambr
+tests/snapshots/test_helpers.ambr
```

### Comparing `devolo_plc_api-1.3.2/docs/CHANGELOG.md` & `devolo_plc_api-1.4.0/docs/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [v1.4.0] - 2023/07/26
+
+### Added
+
+- Generate QR codes from wifi guest settings
+- Make use of zeroconf unicast requests to be able to respond across subnets
+
 ## [v1.3.2] - 2023/07/13
 
 ### Fixed
 
 - Frequently connecting to an offline device lead to a memory leak
 
 ## [v1.3.1] - 2023/05/12
```

### Comparing `devolo_plc_api-1.3.2/docs/CODE_OF_CONDUCT.md` & `devolo_plc_api-1.4.0/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/docs/CONTRIBUTING.md` & `devolo_plc_api-1.4.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/example_async.py` & `devolo_plc_api-1.4.0/example_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 
-from devolo_plc_api import Device
+from devolo_plc_api import Device, wifi_qr_code
 
 # IP of the device to query
 IP = "192.168.0.10"
 
 # Password, if the device has one. It is the same as the Web-UI has. It no password is set, you can remove the password
 # parameter or set it to None.
 PASSWORD = "super_secret"
@@ -62,14 +62,19 @@
         # duration.
         guest_wifi = await dpa.device.async_get_wifi_guest_access()
         print(guest_wifi.ssid)  # "devolo-guest-930"
         print(guest_wifi.key)  # "HMANPGBA"
         print(guest_wifi.enabled)  # False
         print(guest_wifi.remaining_duration)  # 0
 
+        # Get a QR code of the guest wifi settings as byte stream in SVG format
+        qr = wifi_qr_code(guest_wifi)
+        with open("qr.svg", "wb") as binary_file:
+            binary_file.write(qr)
+
         # Enable or disable the wifi guest access. Set enable to True to it turn on, to False to turn it off. Optionally
         # specify a duration in minutes. Changing SSID or the wifi key is currently not supported. If the state was changed
         # successfully, True is returned, otherwise False.
         print("success" if await dpa.device.async_set_wifi_guest_access(enable=True, duration=5) else "failed")
 
         # Get details about other access points in your neighborhood: MAC address, SSID, wifi band, used channel, signal
         # strength in DB and a value from 1 to 5, if you would want to map the signal strength to a signal bars.
```

### Comparing `devolo_plc_api-1.3.2/example_sync.py` & `devolo_plc_api-1.4.0/example_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from devolo_plc_api import Device
+from devolo_plc_api import Device, wifi_qr_code
 
 # IP of the device to query
 IP = "192.168.0.10"
 
 # Password, if the device has one. It is the same as the Web-UI has. It no password is set, you can remove the password
 # parameter or set it to None.
 PASSWORD = "super_secret"
@@ -60,14 +60,19 @@
         # duration.
         guest_wifi = dpa.device.get_wifi_guest_access()
         print(guest_wifi.ssid)  # "devolo-guest-930"
         print(guest_wifi.key)  # "HMANPGBA"
         print(guest_wifi.enabled)  # False
         print(guest_wifi.remaining_duration)  # 0
 
+        # Get a QR code of the guest wifi settings as byte stream in SVG format
+        qr = wifi_qr_code(guest_wifi)
+        with open("qr.svg", "wb") as binary_file:
+            binary_file.write(qr)
+
         # Enable or disable the wifi guest access. Set enable to True to it turn on, to False to turn it off. Optionally
         # specify a duration in minutes. Changing SSID or the wifi key is currently not supported. If the state was changed
         # successfully, True is returned, otherwise False.
         print("success" if dpa.device.set_wifi_guest_access(enable=True, duration=5) else "failed")
 
         # Get details about other access points in your neighborhood: MAC address, SSID, wifi band, used channel, signal
         # strength in DB and a value from 1 to 5, if you would want to map the signal strength to a signal bars.
```

### Comparing `devolo_plc_api-1.3.2/pyproject.toml` & `devolo_plc_api-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     "Operating System :: OS Independent",
 ]
 description = "devolo PLC devices in Python"
 dependencies = [
     "ifaddr>=0.1.7",
     "httpx>=0.21.0",
     "protobuf>=4.22.0",
-    "zeroconf>=0.32.0",
+    "segno>=1.5.2",
+    "zeroconf>=0.70.0",
 ]
 dynamic = [
     "version",
 ]
 license = { file = "LICENSE" }
 name = "devolo_plc_api"
 readme = "README.md"
```

### Comparing `devolo_plc_api-1.3.2/scripts/stubgen.py` & `devolo_plc_api-1.4.0/scripts/stubgen.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/tests/__init__.py` & `devolo_plc_api-1.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/tests/conftest.py` & `devolo_plc_api-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/tests/fixtures/device_api.py` & `devolo_plc_api-1.4.0/tests/fixtures/device_api.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/tests/fixtures/plcnet_api.py` & `devolo_plc_api-1.4.0/tests/fixtures/plcnet_api.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/tests/mocks/zeroconf.py` & `devolo_plc_api-1.4.0/tests/mocks/zeroconf.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/tests/snapshots/test_device.ambr` & `devolo_plc_api-1.4.0/tests/snapshots/test_device.ambr`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/tests/test_data.json` & `devolo_plc_api-1.4.0/tests/test_data.json`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/tests/test_device.py` & `devolo_plc_api-1.4.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/tests/test_deviceapi.py` & `devolo_plc_api-1.4.0/tests/test_deviceapi.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/tests/test_network.py` & `devolo_plc_api-1.4.0/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.2/tests/test_plcnetapi.py` & `devolo_plc_api-1.4.0/tests/test_plcnetapi.py`

 * *Files identical despite different names*

