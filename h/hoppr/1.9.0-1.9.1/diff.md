# Comparing `tmp/hoppr-1.9.0.tar.gz` & `tmp/hoppr-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr-1.9.0.tar", max compression
+gzip compressed data, was "hoppr-1.9.1.tar", max compression
```

## Comparing `hoppr-1.9.0.tar` & `hoppr-1.9.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1084 2023-07-12 18:05:34.000000 hoppr-1.9.0/LICENSE
--rw-r--r--   0        0        0     1215 2023-07-12 18:05:34.000000 hoppr-1.9.0/README.md
--rw-r--r--   0        0        0      994 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/__init__.py
--rw-r--r--   0        0        0      154 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/__main__.py
--rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/base_plugins/__init__.py
--rw-r--r--   0        0        0    11546 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/base_plugins/collector.py
--rw-r--r--   0        0        0    10563 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/base_plugins/hoppr.py
--rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/base_plugins/py.typed
--rw-r--r--   0        0        0     2843 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/cli/__init__.py
--rw-r--r--   0        0        0     2875 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/cli/bundle.py
--rw-r--r--   0        0        0     2252 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/cli/generate.py
--rw-r--r--   0        0        0     4025 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/cli/layout.py
--rw-r--r--   0        0        0     7383 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/cli/merge.py
--rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/cli/py.typed
--rw-r--r--   0        0        0      563 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/constants.py
--rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/__init__.py
--rw-r--r--   0        0        0     3046 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/bundle_tar.py
--rw-r--r--   0        0        0    12806 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_apt_plugin.py
--rw-r--r--   0        0        0     2330 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_cargo_plugin.py
--rw-r--r--   0        0        0    10738 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_dnf_plugin.py
--rw-r--r--   0        0        0     4327 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_docker_plugin.py
--rw-r--r--   0        0        0     4637 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_git_plugin.py
--rw-r--r--   0        0        0     2330 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_golang_plugin.py
--rw-r--r--   0        0        0     4109 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_helm_plugin.py
--rw-r--r--   0        0        0     6284 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_maven_plugin.py
--rw-r--r--   0        0        0     7946 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_nexus_search.py
--rw-r--r--   0        0        0     2390 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_npm_plugin.py
--rw-r--r--   0        0        0     2788 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_nuget_plugin.py
--rw-r--r--   0        0        0     4819 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_pypi_plugin.py
--rw-r--r--   0        0        0     3033 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_raw_plugin.py
--rw-r--r--   0        0        0     3608 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/collect_yum_plugin.py
--rw-r--r--   0        0        0     4278 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/composite_collector.py
--rw-r--r--   0        0        0     5511 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/delta_sbom.py
--rw-r--r--   0        0        0     6885 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/oras_bundle.py
--rw-r--r--   0        0        0     5248 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/oras_registry.py
--rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/py.typed
--rw-r--r--   0        0        0      202 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/__init__.py
--rw-r--r--   0        0        0   126749 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
--rw-r--r--   0        0        0     4635 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/report_generator.py
--rw-r--r--   0        0        0    60554 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
--rw-r--r--   0        0        0      518 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/scripts/custom.js
--rw-r--r--   0        0        0   220780 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
--rw-r--r--   0        0        0     3562 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/styles/custom.css
--rw-r--r--   0        0        0     5052 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/templates/component_card.jinja2
--rw-r--r--   0        0        0     1230 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
--rw-r--r--   0        0        0     7246 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/core_plugins/report_generator/templates/index.jinja2
--rw-r--r--   0        0        0      458 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/exceptions.py
--rw-r--r--   0        0        0     6782 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/in_toto.py
--rw-r--r--   0        0        0     3378 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/main.py
--rw-r--r--   0        0        0     4106 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/mem_logger.py
--rw-r--r--   0        0        0     1627 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/__init__.py
--rw-r--r--   0        0        0     1602 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/__main__.py
--rw-r--r--   0        0        0     1546 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/base.py
--rw-r--r--   0        0        0     4001 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/credentials.py
--rw-r--r--   0        0        0    12363 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/manifest.py
--rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/py.typed
--rw-r--r--   0        0        0    20656 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/sbom.py
--rw-r--r--   0        0        0     4556 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/transfer.py
--rw-r--r--   0        0        0     5667 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/models/types.py
--rw-r--r--   0        0        0     2335 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/net.py
--rw-r--r--   0        0        0     4251 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/oci_artifacts.py
--rw-r--r--   0        0        0     1332 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/plugin_utils.py
--rw-r--r--   0        0        0    27443 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/processor.py
--rw-r--r--   0        0        0        0 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/py.typed
--rw-r--r--   0        0        0    22579 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/resources/hoppr-hippo.ansi
--rw-r--r--   0        0        0    19725 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/resources/hoppr-hippo.ascii
--rw-r--r--   0        0        0     4036 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/result.py
--rw-r--r--   0        0        0     7785 2023-07-12 18:05:34.000000 hoppr-1.9.0/hoppr/utils.py
--rw-r--r--   0        0        0     5100 2023-07-12 18:05:34.000000 hoppr-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 hoppr-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-26 21:05:34.000000 hoppr-1.9.1/LICENSE
+-rw-r--r--   0        0        0     1215 2023-07-26 21:05:34.000000 hoppr-1.9.1/README.md
+-rw-r--r--   0        0        0      994 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/base_plugins/__init__.py
+-rw-r--r--   0        0        0    11546 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/base_plugins/collector.py
+-rw-r--r--   0        0        0    10563 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/base_plugins/hoppr.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/base_plugins/py.typed
+-rw-r--r--   0        0        0     2843 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/cli/__init__.py
+-rw-r--r--   0        0        0     2875 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/cli/bundle.py
+-rw-r--r--   0        0        0     2252 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/cli/generate.py
+-rw-r--r--   0        0        0     4025 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/cli/layout.py
+-rw-r--r--   0        0        0     7383 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/cli/merge.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/cli/py.typed
+-rw-r--r--   0        0        0      563 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/constants.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3046 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/bundle_tar.py
+-rw-r--r--   0        0        0    12806 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_apt_plugin.py
+-rw-r--r--   0        0        0     2330 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_cargo_plugin.py
+-rw-r--r--   0        0        0    10738 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_dnf_plugin.py
+-rw-r--r--   0        0        0     4327 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_docker_plugin.py
+-rw-r--r--   0        0        0     4647 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_git_plugin.py
+-rw-r--r--   0        0        0     2330 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_golang_plugin.py
+-rw-r--r--   0        0        0     4109 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_helm_plugin.py
+-rw-r--r--   0        0        0     6284 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_maven_plugin.py
+-rw-r--r--   0        0        0     7946 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_nexus_search.py
+-rw-r--r--   0        0        0     2390 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_npm_plugin.py
+-rw-r--r--   0        0        0     2788 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_nuget_plugin.py
+-rw-r--r--   0        0        0     6799 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_pypi_plugin.py
+-rw-r--r--   0        0        0     3033 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_raw_plugin.py
+-rw-r--r--   0        0        0     3608 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/collect_yum_plugin.py
+-rw-r--r--   0        0        0     4278 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/composite_collector.py
+-rw-r--r--   0        0        0     5506 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/delta_sbom.py
+-rw-r--r--   0        0        0     6885 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/oras_bundle.py
+-rw-r--r--   0        0        0     5252 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/oras_registry.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/py.typed
+-rw-r--r--   0        0        0      202 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/__init__.py
+-rw-r--r--   0        0        0   126749 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
+-rw-r--r--   0        0        0     4635 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/report_generator.py
+-rw-r--r--   0        0        0    60554 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
+-rw-r--r--   0        0        0      518 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/scripts/custom.js
+-rw-r--r--   0        0        0   220780 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
+-rw-r--r--   0        0        0     3562 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/styles/custom.css
+-rw-r--r--   0        0        0     5052 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/templates/component_card.jinja2
+-rw-r--r--   0        0        0     1230 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
+-rw-r--r--   0        0        0     7246 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/core_plugins/report_generator/templates/index.jinja2
+-rw-r--r--   0        0        0      458 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/exceptions.py
+-rw-r--r--   0        0        0     6827 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/in_toto.py
+-rw-r--r--   0        0        0     2908 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/main.py
+-rw-r--r--   0        0        0     4106 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/mem_logger.py
+-rw-r--r--   0        0        0     1627 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/__init__.py
+-rw-r--r--   0        0        0     1602 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/__main__.py
+-rw-r--r--   0        0        0     1546 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/base.py
+-rw-r--r--   0        0        0     4001 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/credentials.py
+-rw-r--r--   0        0        0    12711 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/manifest.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/py.typed
+-rw-r--r--   0        0        0    20814 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/sbom.py
+-rw-r--r--   0        0        0     4730 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/transfer.py
+-rw-r--r--   0        0        0     5677 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/models/types.py
+-rw-r--r--   0        0        0     2335 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/net.py
+-rw-r--r--   0        0        0     4251 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/oci_artifacts.py
+-rw-r--r--   0        0        0     1332 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/plugin_utils.py
+-rw-r--r--   0        0        0    28786 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/processor.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/py.typed
+-rw-r--r--   0        0        0    22579 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/resources/hoppr-hippo.ansi
+-rw-r--r--   0        0        0    19725 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/resources/hoppr-hippo.ascii
+-rw-r--r--   0        0        0     4036 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/result.py
+-rw-r--r--   0        0        0     7785 2023-07-26 21:05:34.000000 hoppr-1.9.1/hoppr/utils.py
+-rw-r--r--   0        0        0     5052 2023-07-26 21:05:34.000000 hoppr-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 hoppr-1.9.1/PKG-INFO
```

### Comparing `hoppr-1.9.0/LICENSE` & `hoppr-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/README.md` & `hoppr-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/__init__.py` & `hoppr-1.9.1/hoppr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     "Manifest",
     "PurlType",
     "Result",
     "Sbom",
     "Transfer",
 ]
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
```

### Comparing `hoppr-1.9.0/hoppr/base_plugins/collector.py` & `hoppr-1.9.1/hoppr/base_plugins/collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/base_plugins/hoppr.py` & `hoppr-1.9.1/hoppr/base_plugins/hoppr.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/cli/__init__.py` & `hoppr-1.9.1/hoppr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/cli/bundle.py` & `hoppr-1.9.1/hoppr/cli/bundle.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/cli/generate.py` & `hoppr-1.9.1/hoppr/cli/generate.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/cli/layout.py` & `hoppr-1.9.1/hoppr/cli/layout.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/cli/merge.py` & `hoppr-1.9.1/hoppr/cli/merge.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/constants.py` & `hoppr-1.9.1/hoppr/constants.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/bundle_tar.py` & `hoppr-1.9.1/hoppr/core_plugins/bundle_tar.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_apt_plugin.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_apt_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_cargo_plugin.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_cargo_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_dnf_plugin.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_dnf_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_docker_plugin.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_docker_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_git_plugin.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_git_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
         # Default depth
         depth = "1"
         if self.config is not None:
             # Allow for further depth default to 1
             depth = self.config.get("depth", depth)
 
         # Recognize the 'all' keyword as requesting all history
-        if depth.lower() != "all":
-            opts.extend(("--depth", depth))
+        if str(depth).lower() != "all":
+            opts.extend(("--depth", str(depth)))
 
         # Command
         command = [self.required_commands[0], "clone", *opts, git_src]
 
         # Only clone with a depth of one and reference the version specified.
         result = self.run_command(
             command,
```

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_golang_plugin.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_golang_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_helm_plugin.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_helm_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_maven_plugin.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_maven_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_nexus_search.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_nexus_search.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_npm_plugin.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_npm_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_nuget_plugin.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_nuget_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_raw_plugin.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_raw_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/collect_yum_plugin.py` & `hoppr-1.9.1/hoppr/core_plugins/collect_yum_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/composite_collector.py` & `hoppr-1.9.1/hoppr/core_plugins/composite_collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/delta_sbom.py` & `hoppr-1.9.1/hoppr/core_plugins/delta_sbom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Plugin to remove SBOM components that are specified by a "previous" SBOM
 """
 from __future__ import annotations
 
-import contextlib
 import io
 import tarfile
 
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import hoppr.utils
@@ -88,30 +87,32 @@
             f"Delivering updates for {len(delta_sbom.components)} of "
             f"{len(self.context.delivered_sbom.components)} components.",
             return_obj=delta_sbom,
         )
 
     @staticmethod
     def _get_previous_bom(source: str) -> Sbom:
-        with contextlib.suppress(TypeError, UnicodeDecodeError):
-            Sbom.loaded_sboms.clear()
-            return Manifest.load(Path(source)).consolidated_sbom
-
-        with tarfile.open(source) as tar:
-            buffer = tar.extractfile("./generic/_metadata_/_consolidated_bom.json")
-
-            if buffer is None:
-                raise HopprError("Unable to extract BOM file from tar")
-
-            with io.TextIOWrapper(buffer) as bom_file:
-                content: str = bom_file.read()
-                bom_dict = hoppr.utils.load_string(content)
-                if not isinstance(bom_dict, dict):
-                    raise HopprError("Invalid BOM file retrieved from tar")
-                return Sbom(**bom_dict)
+        if tarfile.is_tarfile(name=source):
+            with tarfile.open(source) as tar:
+                buffer = tar.extractfile("./generic/_metadata_/_consolidated_bom.json")
+
+                if buffer is None:
+                    raise HopprError("Unable to extract BOM file from tar")
+
+                with io.TextIOWrapper(buffer) as bom_file:
+                    content: str = bom_file.read()
+                    bom_dict = hoppr.utils.load_string(content)
+
+                    if not isinstance(bom_dict, dict):
+                        raise HopprError("Invalid BOM file retrieved from tar")
+
+                    return Sbom(**bom_dict)
+
+        Sbom.loaded_sboms.clear()
+        return Manifest.load(Path(source)).consolidated_sbom
 
     @staticmethod
     def _purl_match(new_purl: PackageURL, prev_purl: PackageURL) -> bool:
         if any(
             getattr(new_purl, attr) != getattr(prev_purl, attr)
             for attr in ["name", "type", "namespace", "version", "subpath"]
         ):
```

### Comparing `hoppr-1.9.0/hoppr/core_plugins/oras_bundle.py` & `hoppr-1.9.1/hoppr/core_plugins/oras_bundle.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/oras_registry.py` & `hoppr-1.9.1/hoppr/core_plugins/oras_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import os
 import platform
 
 from datetime import datetime
 from http import cookiejar
 
-import jsonschema  # type: ignore[import]
+import jsonschema
 import oras.defaults
 import oras.oci
 import oras.provider
 import oras.schemas
 import requests
 
 from oras.container import Container
@@ -140,12 +140,12 @@
     """
     Block all cookies
 
     Args:
         cookiejar (CookiePolicy): _description_
     """
 
-    return_ok = (
+    return_ok = (  # type: ignore[assignment]
         set_ok
     ) = domain_return_ok = path_return_ok = lambda self, *args, **kwargs: False  # pylint: disable=C3001
     netscape = True
     rfc2965 = hide_cookie2 = False
```

### Comparing `hoppr-1.9.0/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png` & `hoppr-1.9.1/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/report_generator/report_generator.py` & `hoppr-1.9.1/hoppr/core_plugins/report_generator/report_generator.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js` & `hoppr-1.9.1/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/report_generator/scripts/custom.js` & `hoppr-1.9.1/hoppr/core_plugins/report_generator/scripts/custom.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/report_generator/styles/bootstrap.min.css` & `hoppr-1.9.1/hoppr/core_plugins/report_generator/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/report_generator/styles/custom.css` & `hoppr-1.9.1/hoppr/core_plugins/report_generator/styles/custom.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/report_generator/templates/component_card.jinja2` & `hoppr-1.9.1/hoppr/core_plugins/report_generator/templates/component_card.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/report_generator/templates/general_summary.jinja2` & `hoppr-1.9.1/hoppr/core_plugins/report_generator/templates/general_summary.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/core_plugins/report_generator/templates/index.jinja2` & `hoppr-1.9.1/hoppr/core_plugins/report_generator/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/in_toto.py` & `hoppr-1.9.1/hoppr/in_toto.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         for plugin_ref in stage_ref.plugins:
             plugin_cls = plugin_class(plugin_ref.name)
             products[stage_ref.name] += plugin_cls.get_attestation_products(plugin_ref.config)
 
         products[stage_ref.name] += [
             "generic/_metadata_/_delivered_bom.json",
             f"generic/_metadata_/_intermediate_{stage_ref.name}_delivered_bom.json",
+            "generic/_metadata_/_run_data_",
         ]
 
     stages.append("_finalize")
     products["_finalize"] = ["generic/_metadata_/_delivered_bom.json"]
 
     return (products, stages)
```

### Comparing `hoppr-1.9.0/hoppr/main.py` & `hoppr-1.9.1/hoppr/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Framework for manipulating bundles for airgapped transfers.
 """
 import logging
 import sys
 
 from pathlib import Path
-from posixpath import sep
 from typing import List, Optional
 
 from typer import Exit, echo, prompt
 
 from hoppr import __version__
 from hoppr.in_toto import generate_in_toto_layout
 from hoppr.models.credentials import Credentials
@@ -31,24 +30,14 @@
     functionary_key_password: Optional[str] = None,
     previous_delivery: Optional[Path] = None,
 ):
     """
     Run the stages specified in the transfer config
     file on the content specified in the manifest
     """
-    echo(
-        f"Loading {str(manifest_file).rsplit(str(sep), maxsplit=1)[-1]} and "
-        f"{str(transfer_file).rsplit(str(sep), maxsplit=1)[-1]} files..."
-    )
-    metadata_files = [manifest_file, transfer_file]
-
-    if credentials_file is not None:
-        echo(f"Loading {str(credentials_file).rsplit(str(sep), maxsplit=1)[-1]} file...")
-        metadata_files.append(credentials_file)
-
     log_level = logging.DEBUG if verbose else logging.INFO
 
     if create_attestations and functionary_key_path is None:
         echo("To create attestations both the `--attest` option and a functionary private key need to be provided.")
         raise Exit(code=1)
 
     if functionary_key_prompt:
@@ -63,16 +52,14 @@
         functionary_key_password=functionary_key_password,
         log_level=log_level,
         log_file=log_file,
         strict_repos=strict_repos,
         previous_delivery=previous_delivery,
     )
 
-    processor.metadata_files = metadata_files
-
     result = processor.run()
 
     if result.is_fail():
         sys.exit(1)
 
 
 def generate_layout(
```

### Comparing `hoppr-1.9.0/hoppr/mem_logger.py` & `hoppr-1.9.1/hoppr/mem_logger.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/models/__init__.py` & `hoppr-1.9.1/hoppr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/models/__main__.py` & `hoppr-1.9.1/hoppr/models/__main__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/models/base.py` & `hoppr-1.9.1/hoppr/models/base.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/models/credentials.py` & `hoppr-1.9.1/hoppr/models/credentials.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/models/manifest.py` & `hoppr-1.9.1/hoppr/models/manifest.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,28 +96,30 @@
     sboms: list[SbomRef] = []
 
     @classmethod
     def parse_file(cls, path: str | Path, *args, **kwargs) -> ManifestFile:  # pylint: disable=unused-argument
         """
         Override to resolve local file paths relative to manifest file
         """
-        path = Path(path).resolve()
+        path = Path(path)
 
         data = hoppr.utils.load_file(path)
         if not isinstance(data, dict):
             raise TypeError("Local file content was not loaded as dictionary")
 
         # Resolve local file path references relative to manifest file path
         for sbom in data.get("sboms", []):
             if "local" in sbom:
-                sbom["local"] = str((path.parent / sbom["local"]).resolve())
+                local_ref = (path.parent / sbom["local"]).resolve().relative_to(Path.cwd())
+                sbom["local"] = str(local_ref)
 
         for include in data.get("includes", []):
             if "local" in include:
-                include["local"] = str((path.parent / include["local"]).resolve())
+                local_ref = (path.parent / include["local"]).resolve().relative_to(Path.cwd())
+                include["local"] = str(local_ref)
 
         return cls(**data)
 
     @classmethod
     def parse_obj(cls, obj: DictStrAny) -> ManifestFile:
         """
         Override to remove local file paths that can't be resolved
@@ -287,14 +289,15 @@
             location (str | Path): Path to included manifest
 
         Returns:
             ManifestFile | None: Manifest object if found, otherwise None
         """
         match ref_type:
             case "local":
+                location = Path(location).resolve().relative_to(Path.cwd())
                 return cls.loaded_manifests.get(LocalFile(local=Path(location)))
             case "url":
                 return cls.loaded_manifests.get(UrlFile(url=str(location)))
             case _:
                 return None
 
     @classmethod
@@ -302,18 +305,20 @@
         """
         Load manifest from local file, URL, or dict
         """
         match source:
             case dict():
                 data = source
             case Path():
-                path = Path(source).resolve()
-                manifest_file = cls.parse_file(path)
-                local_ref = LocalFile(local=path)
-                cls.loaded_manifests[local_ref] = manifest_file
+                # Convert source to relative path if in current working directory subpath
+                source = source.resolve()
+                source = source.relative_to(Path.cwd()) if source.is_relative_to(Path.cwd()) else source
+
+                manifest_file = cls.parse_file(source)
+                cls.loaded_manifests[LocalFile(local=source)] = manifest_file
                 data = manifest_file.dict(by_alias=True)
             case str():
                 try:
                     include_dict = hoppr.net.load_url(source)
                     if not isinstance(include_dict, dict):
                         raise TypeError("URL manifest include was not loaded as dictionary")
```

### Comparing `hoppr-1.9.0/hoppr/models/sbom.py` & `hoppr-1.9.1/hoppr/models/sbom.py`

 * *Files 4% similar despite different names*

```diff
@@ -546,18 +546,20 @@
         Load SBOM from local file, URL, or dict
         """
         # pylint: disable=duplicate-code
         match source:
             case dict():
                 sbom = cls(**source)
             case Path():
-                path = Path(source).resolve()
-                sbom = cls.parse_file(path)
-                local_ref = LocalFile(local=path)
-                cls.loaded_sboms[local_ref] = sbom
+                # Convert source to relative path if in current working directory subpath
+                source = source.resolve()
+                source = source.relative_to(Path.cwd()) if source.is_relative_to(Path.cwd()) else source
+
+                sbom = cls.parse_file(source)
+                cls.loaded_sboms[LocalFile(local=source)] = sbom
             case str():
                 try:
                     sbom_dict = hoppr.net.load_url(source)
                     if not isinstance(sbom_dict, dict):
                         raise TypeError("URL SBOM was not loaded as dictionary")
 
                     sbom = cls.parse_obj(sbom_dict)
```

### Comparing `hoppr-1.9.0/hoppr/models/transfer.py` & `hoppr-1.9.1/hoppr/models/transfer.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 """
 from __future__ import annotations
 
 import math
 import re
 
 from enum import Enum
+from importlib.metadata import entry_points
 from pathlib import Path
 from typing import TYPE_CHECKING, Annotated, Any, Literal, Pattern
 
-from importlib.metadata import entry_points
-from pydantic import ConstrainedStr, Field, validator, root_validator
+from pydantic import ConstrainedStr, Field, root_validator, validator
 
 from hoppr.models.base import HopprBaseModel, HopprBaseSchemaModel
 
 if TYPE_CHECKING:
     from pydantic.typing import DictStrAny
 else:
     DictStrAny = dict[str, Any]
@@ -37,24 +37,25 @@
     """
 
     name: str = Field(..., description="Name of plugin")
     config: DictStrAny | None = Field(None, description="Mapping of additional plugin configuration settings to values")
 
     @root_validator(pre=True)
     @classmethod
-    def validate_model(cls, values: DictStrAny):
+    def validate_plugin(cls, values: DictStrAny):
         """
         Validate Plugin model
         """
         name = values.get("name")
-        plugin_eps = entry_points(group='hoppr.plugin')
+        plugin_eps = entry_points(group="hoppr.plugin")
 
         for plugin in plugin_eps:
-            if str(name) in plugin.value:
-                values["name"] = plugin.value.split(":")[0]
+            # Check project entry points for plugin name, module, or class
+            if str(name) in {plugin.name, plugin.module, plugin.attr}:
+                values["name"] = plugin.module
                 break
 
         return values
 
 
 Plugin.update_forward_refs()
 
@@ -125,39 +126,27 @@
     @validator("stages", allow_reuse=True, pre=True)
     @classmethod
     def validate_stages(cls, stages: DictStrAny) -> list[StageRef]:
         """
         Transform Stages into list of StageRef objects
         """
         stage_refs: list[StageRef] = []
-
-        add_delta = True
+        plugin_names = set()
 
         for stage_name, stage in stages.items():
             stage["name"] = stage_name
             stage_refs.append(StageRef.parse_obj(stage))
 
-            for plugin in stage["plugins"]:
-                plugin = Plugin.validate_model(plugin)
-                if plugin["name"] == "hoppr.core_plugins.delta_sbom":
-                    add_delta = False
-
-        if add_delta:
-            stage_refs.insert(
-                0,
-                StageRef(
-                    name=StageName("_delta_sbom_"),
-                    plugins=[
-                        Plugin(
-                            name="hoppr.core_plugins.delta_sbom",
-                            config=None,
-                        )
-                    ],
-                ),
-            )
+            plugin_names.update({plugin["name"] for plugin in stage["plugins"]})
+
+        if not plugin_names.intersection({"DeltaSbom", "delta_sbom", "hoppr.core_plugins.delta_sbom"}):
+            stage_refs = [
+                StageRef(name=StageName("_delta_sbom_"), plugins=[Plugin(name="delta_sbom", config=None)]),
+                *stage_refs,
+            ]
 
         return stage_refs
 
     @classmethod
     def load(cls, source: str | Path | DictStrAny) -> Transfer:
         """
         Load transfer file from local path or dict
@@ -165,7 +154,16 @@
         match source:
             case dict():
                 return cls.parse_obj(source)
             case str() | Path():
                 return cls.parse_file(source)
             case _:
                 raise TypeError("'source' argument must be one of: 'str', 'Path', 'dict[str, Any]'")
+
+    def yaml(self, *args, **kwargs) -> str:
+        transfer_dict = self.dict(by_alias=True)
+        transfer_dict["stages"] = {}
+
+        for stage in self.stages:
+            transfer_dict["stages"][str(stage.name)] = {"plugins": stage.plugins}
+
+        return TransferFile.parse_obj(transfer_dict).yaml(*args, **kwargs)
```

### Comparing `hoppr-1.9.0/hoppr/models/types.py` & `hoppr-1.9.1/hoppr/models/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
     LocalFile data model
     """
 
     local: Path
 
     def __str__(self) -> str:
-        return self.local.as_uri()
+        return self.local.resolve().as_uri()
 
 
 class OciFile(HopprBaseModel):
     """
     OciFile data model
     """
```

### Comparing `hoppr-1.9.0/hoppr/net.py` & `hoppr-1.9.1/hoppr/net.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/oci_artifacts.py` & `hoppr-1.9.1/hoppr/oci_artifacts.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/plugin_utils.py` & `hoppr-1.9.1/hoppr/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/processor.py` & `hoppr-1.9.1/hoppr/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,20 @@
 class StageProcessor:  # pylint: disable=too-few-public-methods
     """
     Class to handle all processing within a single Hoppr stage
     """
 
     component_based_methods = [HopprPlugin.process_component.__name__]
 
-    def __init__(self, stage_ref: StageRef, context: HopprContext):
+    # pylint: disable=line-too-long
+    def __init__(self, stage_ref: StageRef, context: HopprContext, logger: MemoryLogger = None):  # type: ignore[assignment]
         self.stage_id = stage_ref.name
         self.context = context
         self.plugin_ref_list = stage_ref.plugins
+        self.logger = logger
 
         self.config_component_coverage = None
         if stage_ref.component_coverage is not None:
             self.config_component_coverage = ComponentCoverage[str(stage_ref.component_coverage)]
 
         self.required_coverage = ComponentCoverage.OPTIONAL
         self.results: dict[str, list[tuple[str, str | None, Result]]] = {}
@@ -367,22 +369,35 @@
         )
 
         used_purl_types.update(hoppr.utils.get_package_url(purl).type for purl in results)
 
         plugin_list: list[Plugin] = []
 
         # Loop over copy of transfer plugin references
-        for plugin_ref in set(self.plugin_ref_list):
-            plugin_cls = hoppr.utils.plugin_class(plugin_ref.name)
-
-            # Determine if plugin's `supported_purl_types` are in the set of PURL types defined in SBOM components
-            plugin_needed: bool = len(used_purl_types.intersection(plugin_cls.supported_purl_types)) > 0
-
-            if len(plugin_cls.supported_purl_types) == 0 or plugin_needed:
-                plugin_list.append(plugin_ref)
+        with (Path(self.context.collect_root_dir) / "generic" / "_metadata_" / "_run_data_").open(
+            mode="a", encoding="utf-8"
+        ) as rundata:
+            if self.logger:
+                self.logger.info(f"Plugins for stage {self.stage_id}:")
+            rundata.write(f"\nPlugins for stage {self.stage_id}:\n")
+            for plugin_ref in set(self.plugin_ref_list):
+                plugin_cls = hoppr.utils.plugin_class(plugin_ref.name)
+
+                # Determine if plugin's `supported_purl_types` are in the set of PURL types defined in SBOM components
+                plugin_needed: bool = len(used_purl_types.intersection(plugin_cls.supported_purl_types)) > 0
+
+                if len(plugin_cls.supported_purl_types) == 0 or plugin_needed:
+                    plugin_list.append(plugin_ref)
+                    instance = plugin_instance(plugin_ref.name, self.context, plugin_ref.config)
+                    if self.logger:
+                        self.logger.info(
+                            f"{plugin_cls.__name__} version {instance.get_version()} from {plugin_ref.name}",
+                            indent_level=1,
+                        )
+                    rundata.write(f"   {plugin_cls.__name__} version {instance.get_version()} from {plugin_ref.name}\n")
 
         return plugin_list
 
 
 class HopprProcessor:  # pylint: disable=too-many-instance-attributes
     """
     Run the Hoppr process
@@ -402,26 +417,30 @@
         previous_delivery: Path | None = None,
     ) -> None:
         self.context: HopprContext
         self.logger: MemoryLogger
         self.log_file: Path = Path(log_file or f"hoppr_{time.strftime('%Y%m%d-%H%M%S')}.log")
         self.log_level = log_level
         self.logfile_lock = multiprocessing.RLock()
-        self.metadata_files: list[Path] = []
+        self.metadata_files: list[Path] = [manifest_file, transfer_file]
+        self.previous_delivery = previous_delivery
         self.strict_repos: bool = strict_repos
 
+        echo(f"Loading {manifest_file.name} and {transfer_file.name} files...")
         self.manifest_file = ManifestFile.parse_file(manifest_file)
-
-        self.credentials = Credentials.load(credentials_file)
         self.manifest = Manifest.load(manifest_file)
         self.transfer = Transfer.load(transfer_file)
 
-        self.stage_processor_map: MutableMapping[StageRef, StageProcessor] = {}
+        self.credentials = None
+        if credentials_file is not None:
+            echo(f"Loading {credentials_file.name} file...")
+            self.credentials = Credentials.load(credentials_file)
+            self.metadata_files.append(credentials_file)
 
-        self.previous_delivery: Path | None = previous_delivery
+        self.stage_processor_map: MutableMapping[StageRef, StageProcessor] = {}
 
         self.in_toto_links = HopprInTotoLinks(
             create_attestations,
             self.transfer,
             functionary_key_path,
             functionary_key_password,
         )
@@ -440,30 +459,30 @@
     def _collect_manifest_metadata(self, manifest: ManifestFile, target_dir: str | PathLike[str]) -> None:
         echo(f"Loading {len(manifest.includes)} includes from manifest...")
         for include_ref in manifest.includes:
             include = Manifest.loaded_manifests[include_ref]
             include_dict = include_ref.dict()
 
             if "local" in include_dict:
-                url = str(include_dict["local"])
+                url = str(Path(include_dict["local"]).resolve())
             else:
                 url = str(include_dict["url"])
 
             target_file = Path(target_dir) / quote_plus(url)
 
             with target_file.open(mode="w+", encoding="utf-8") as output_file:
                 output_file.write(include.yaml(by_alias=True, exclude_unset=True, indent=True))
 
         echo(f"Loading {len(manifest.sboms)} sboms from manifest...")
         for sbom_ref in manifest.sboms:
             sbom = Sbom.loaded_sboms[sbom_ref]
             sbom_dict = sbom_ref.dict()
 
             if "local" in sbom_dict:
-                url = str(sbom_dict["local"])
+                url = str(Path(sbom_dict["local"]).resolve())
             elif "oci" in sbom_dict:
                 url = str(sbom_dict["oci"])
             else:
                 url = str(sbom_dict["url"])
 
             target_file = Path(target_dir) / quote_plus(url)
 
@@ -608,14 +627,15 @@
                 logfile_location=self.log_file,
                 logfile_lock=logfile_lock,
                 max_processes=self.transfer.max_processes or cpu_count(),
                 repositories=self.manifest.repositories,
                 sboms=list(Sbom.loaded_sboms.values()),
                 stages=self.transfer.stages,
                 strict_repos=self.strict_repos,
+                previous_delivery=self.previous_delivery,
             )
 
             self.logger = self.get_logger(
                 lock=logfile_lock,
                 log_name=f"HopprProcessor--{os.getpid()}",
                 log_file=self.log_file,
                 log_level=self.log_level,
@@ -645,15 +665,15 @@
             echo(message=msg)
 
             for stage_ref in self.transfer.stages:
                 msg = f" Beginning Stage {stage_ref.name} ".center(100, "=")
                 self.logger.info(msg)
                 echo(msg)
 
-                stage = StageProcessor(stage_ref, self.context)
+                stage = StageProcessor(stage_ref, self.context, self.logger)
                 self.in_toto_links.record_stage_start(stage_ref.name)
                 self.stage_processor_map[stage_ref] = stage
 
                 result = stage.run()
 
                 if result.is_fail() or result.is_retry():
                     msg = f"Stage {stage_ref.name} failed, processing terminated: {result.message}"
```

### Comparing `hoppr-1.9.0/hoppr/resources/hoppr-hippo.ansi` & `hoppr-1.9.1/hoppr/resources/hoppr-hippo.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/resources/hoppr-hippo.ascii` & `hoppr-1.9.1/hoppr/resources/hoppr-hippo.ascii`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/result.py` & `hoppr-1.9.1/hoppr/result.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/hoppr/utils.py` & `hoppr-1.9.1/hoppr/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.0/pyproject.toml` & `hoppr-1.9.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr"
-version = "1.9.0"
+version = "1.9.1"
 description = "A tool for defining, verifying, and transferring software dependencies between environments."
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev"
 repository = "https://gitlab.com/hoppr/hoppr"
 
@@ -17,56 +17,54 @@
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Information Technology",
   "Topic :: Communications :: File Sharing",
   "Topic :: Software Development :: Version Control",
   "Topic :: System :: Software Distribution"
-
 ]
 
 [[tool.poetry.packages]]
 include = "hoppr"
 
 [tool.poetry.scripts]
 hopctl = "hoppr.cli:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-hoppr-cyclonedx-models = "^0.4.7"
+hoppr-cyclonedx-models = "0.*"
 in-toto = "^1.3.1"
 jc = "^1.22.2"
 Jinja2 = "^3.1.2"
 jmespath = "^1.0.1"
-oras = "^0.1.17"
-packageurl-python = "~0"
-pydantic-yaml = "^0.10.0"
+oras = "0.*"
+packageurl-python = "0.*"
+pydantic-yaml = "0.*"
 PyYAML = "^6.0"
 rapidfuzz = "^3.1.1"
-securesystemslib = "0.26.0"
 types-PyYAML = "^6.0.5"
 
 [tool.poetry.dependencies.pydantic]
 extras = ["email"]
 version = "^1.9.0"
 
 [tool.poetry.dependencies.typer]
 extras = ["all"]
-version = "^0.9.0"
+version = "0.*"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
-dill = "^0.3.6"
+dill = "0.*"
 isort = "^5.10.1"
 pre-commit = "^3.0.0"
 setuptools = "^67.0.0"
 shfmt-py = "^3.4.3.1"
 
 [tool.poetry.group.test.dependencies]
-mypy = "^0.961"
+mypy = "0.*"
 pylint = "^2.12.2"
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-pretty = "^1.1.0"
 types-mock = "^5.0.0.2"
 types-requests = "^2.27.15"
```

### Comparing `hoppr-1.9.0/PKG-INFO` & `hoppr-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr
-Version: 1.9.0
+Version: 1.9.1
 Summary: A tool for defining, verifying, and transferring software dependencies between environments.
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
@@ -15,25 +15,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: System :: Software Distribution
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: hoppr-cyclonedx-models (>=0.4.7,<0.5.0)
+Requires-Dist: hoppr-cyclonedx-models (==0.*)
 Requires-Dist: in-toto (>=1.3.1,<2.0.0)
 Requires-Dist: jc (>=1.22.2,<2.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
-Requires-Dist: oras (>=0.1.17,<0.2.0)
-Requires-Dist: packageurl-python (>=0,<1)
-Requires-Dist: pydantic-yaml (>=0.10.0,<0.11.0)
+Requires-Dist: oras (==0.*)
+Requires-Dist: packageurl-python (==0.*)
+Requires-Dist: pydantic-yaml (==0.*)
 Requires-Dist: pydantic[email] (>=1.9.0,<2.0.0)
 Requires-Dist: rapidfuzz (>=3.1.1,<4.0.0)
-Requires-Dist: securesystemslib (==0.26.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: typer[all] (==0.*)
 Requires-Dist: types-PyYAML (>=6.0.5,<7.0.0)
 Project-URL: Repository, https://gitlab.com/hoppr/hoppr
 Description-Content-Type: text/markdown
 
 <img src="https://gitlab.com/hoppr/hoppr/-/raw/dev/media/hoppr-repo-banner.png" />
 <br />
 <br />
```

