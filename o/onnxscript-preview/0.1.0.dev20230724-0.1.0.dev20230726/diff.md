# Comparing `tmp/onnxscript-preview-0.1.0.dev20230724.tar.gz` & `tmp/onnxscript-preview-0.1.0.dev20230726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-preview-0.1.0.dev20230724.tar", last modified: Mon Jul 24 00:09:06 2023, max compression
+gzip compressed data, was "onnxscript-preview-0.1.0.dev20230726.tar", last modified: Wed Jul 26 00:09:23 2023, max compression
```

## Comparing `onnxscript-preview-0.1.0.dev20230724.tar` & `onnxscript-preview-0.1.0.dev20230726.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.129945 onnxscript-preview-0.1.0.dev20230724/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-24 00:09:06.129945 onnxscript-preview-0.1.0.dev20230724/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.093945 onnxscript-preview-0.1.0.dev20230724/onnxscript/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.093945 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/feature_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/param_manipulation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/analysis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/autocast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.097945 onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    59491 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    23291 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/converter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.089945 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.097945 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.109945 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/evaluator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.089945 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.089945 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.109945 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.109945 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/graph_building.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/graph_building_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.109945 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   225758 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)    75574 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/tensor_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/irbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.113945 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.117945 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)   152497 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 runner    (1001) docker     (123)    53435 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 runner    (1001) docker     (123)   156522 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 runner    (1001) docker     (123)    42746 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 runner    (1001) docker     (123)   139640 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 runner    (1001) docker     (123)    50619 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 runner    (1001) docker     (123)    69354 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 runner    (1001) docker     (123)    74270 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 runner    (1001) docker     (123)    33248 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 runner    (1001) docker     (123)    49053 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 runner    (1001) docker     (123)    58408 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/sourceinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tensor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.117945 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.117945 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/common/onnx_script_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/eager_mode_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/eager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/external_tensor_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.089945 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.121945 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/
--rw-r--r--   0 runner    (1001) docker     (123)    26593 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/ops_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    71562 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.121945 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/attr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/gemmgelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/gemmgelu_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/if_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/onnxfns1A_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/onnxfns2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/onnxfns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/ort_custom_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/if_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/loop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.125945 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/attrref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/cast_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/different_opset.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/eager_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/eg1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/graph_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/if_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/loops_break.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/loops_while.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/m1.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/onnxfns1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/onnxfns1A.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/onnxfns2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/opt_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/opt_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/renaming.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/signal_dft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/subfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/type_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/onnx_types_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/operator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/type_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/type_annotation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24387 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript/values_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:09:06.125945 onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-24 00:09:06.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-24 00:09:06.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:09:06.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 00:09:06.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 00:09:06.000000 onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-24 00:08:56.000000 onnxscript-preview-0.1.0.dev20230724/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 00:09:06.129945 onnxscript-preview-0.1.0.dev20230724/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-24 00:08:48.000000 onnxscript-preview-0.1.0.dev20230724/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.186549 onnxscript-preview-0.1.0.dev20230726/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-26 00:09:23.186549 onnxscript-preview-0.1.0.dev20230726/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.166549 onnxscript-preview-0.1.0.dev20230726/onnxscript/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.166549 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/feature_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/param_manipulation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/analysis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/autocast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.166549 onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59491 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23291 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/converter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.158549 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.166549 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.174548 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/evaluator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.158549 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.158549 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.174548 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.174548 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/graph_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/graph_building_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.174548 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   226462 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75574 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/tensor_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/irbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.174548 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.178549 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)   152497 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53435 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156522 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42746 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139640 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50619 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69354 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74270 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33248 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49053 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58408 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/sourceinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tensor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.178549 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.178549 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/common/onnx_script_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/eager_mode_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/eager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/external_tensor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.162549 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.182549 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    26593 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72345 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.182549 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/attr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/gemmgelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/gemmgelu_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/if_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/onnxfns1A_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/onnxfns2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/onnxfns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/ort_custom_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/if_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/loop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.186549 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/attrref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/cast_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/different_opset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/eager_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/eg1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/graph_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/if_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/loops_break.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/loops_while.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/m1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/onnxfns1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/onnxfns1A.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/onnxfns2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/opt_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/opt_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/renaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/signal_dft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/subfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/type_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/onnx_types_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/operator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/type_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/type_annotation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24387 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript/values_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:09:23.186549 onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-26 00:09:23.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-26 00:09:23.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:09:23.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 00:09:23.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 00:09:23.000000 onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-26 00:09:16.000000 onnxscript-preview-0.1.0.dev20230726/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 00:09:23.186549 onnxscript-preview-0.1.0.dev20230726/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 00:09:12.000000 onnxscript-preview-0.1.0.dev20230726/setup.py
```

### Comparing `onnxscript-preview-0.1.0.dev20230724/LICENSE` & `onnxscript-preview-0.1.0.dev20230726/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/PKG-INFO` & `onnxscript-preview-0.1.0.dev20230726/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript-preview
-Version: 0.1.0.dev20230724
+Version: 0.1.0.dev20230726
 Summary: Authoring ONNX functions in Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-preview-0.1.0.dev20230724/README.md` & `onnxscript-preview-0.1.0.dev20230726/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/__init__.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/ast_utils.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/param_manipulation.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/param_manipulation_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/param_manipulation_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/runtime_typing.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/_internal/version_utils.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/analysis.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/analysis_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/analysis_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/autocast.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_backend.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_backend_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_backend_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_export.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/backend/onnx_export_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/backend/onnx_export_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/converter.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/converter_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/converter_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/context.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/diagnostics/infra/utils.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/evaluator.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/evaluator_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/evaluator_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/graph_building.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/graph_building.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/graph_building_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/graph_building_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 @torch_op("aten::acosh")
 def aten_acosh(self: TFloat) -> TFloat:
     """acosh(Tensor self) -> Tensor"""
 
     return op.Acosh(self)
 
 
-@torch_op("aten::add")
+@torch_op(("aten::add", "aten::add.Tensor"))
 def aten_add(self: TReal, other: TReal, alpha: float = 1.0) -> TReal:
     """add.Tensor(Tensor self, Tensor other, *, Scalar alpha=1) -> Tensor"""
     # TODO(microsoft/onnxruntime#15977): Improve fp16 precision
     alpha = op.CastLike(alpha, other)
     other = op.Mul(other, alpha)
     return op.Add(self, other)
 
@@ -1231,15 +1231,15 @@
     if remainder > 0:  # type: ignore[operator]
         # Append the remainder to the [n, n, n, n, ..., r]
         list_split = op.Concat(list_split, op.Reshape(remainder, neg_1), axis=0)
 
     return op.SplitToSequence(self, list_split, axis=dim)
 
 
-@torch_op("aten::clamp", trace_only=True)
+@torch_op(("aten::clamp", "aten::clamp.Tensor"), trace_only=True)
 def aten_clamp(self: TReal, min: Optional[TReal] = None, max: Optional[TReal] = None) -> TReal:
     """clamp(Tensor self, Tensor? min=None, Tensor? max=None) -> Tensor"""
     clamped = self
 
     if min is None and max is None:
         return clamped
 
@@ -2180,15 +2180,15 @@
 
 def aten_dist(self: TensorType, other: TensorType, p: float = 2.0) -> TensorType:
     """dist(Tensor self, Tensor other, Scalar p=2) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::div")
+@torch_op(("aten::div", "aten::div.Tensor"))
 def aten_div(self: TFloat, other: TFloat) -> TFloat:
     """div.Tensor(Tensor self, Tensor other) -> Tensor"""
 
     # Int inputs will be promoted to float by PyTorch
     return op.Div(self, other)
 
 
@@ -2295,15 +2295,15 @@
     scale_grad_by_freq: bool,
 ) -> TensorType:
     """embedding_sparse_backward(Tensor grad, Tensor indices, int num_weights, int padding_idx, bool scale_grad_by_freq) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::empty")
+@torch_op(("aten::empty", "aten::empty.memory_format"))
 def aten_empty(size: IntType, dtype: int = FLOAT.dtype) -> TTensor:  # type: ignore[type-var]
     # empty(SymInt[] size, *, ScalarType? dtype=None, Layout? layout=None, Device? device=None, bool? pin_memory=None, MemoryFormat? memory_format=None) -> Tensor
 
     # using Zeros to simulate np.empty()
     size = op.Cast(size, to=INT64.dtype)
     zero = op.Constant(value_float=0.0)
     zero = op.Cast(zero, to=dtype)
@@ -2349,15 +2349,15 @@
     # using Zeros to simulate empty()
     size = op.Cast(size, to=INT64.dtype)
     zero = op.Constant(value_float=0.0)
 
     return op.Expand(zero, size)
 
 
-@torch_op("aten::eq")
+@torch_op(("aten::eq", "aten::eq.Tensor", "aten::eq.Scalar"))
 def aten_eq(self: TTensor, other: TTensor) -> BOOL:
     """eq.Tensor(Tensor self, Tensor other) -> Tensor"""
 
     return op.Equal(self, other)
 
 
 @torch_op("aten::equal")
@@ -2559,15 +2559,15 @@
 
 def aten_feature_dropout(input: TensorType, p: float, train: bool) -> TensorType:
     """feature_dropout(Tensor input, float p, bool train) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::fill")
+@torch_op(("aten::fill", "aten::fill.Tensor"))
 def aten_fill(self: TTensor, value: TTensor) -> TTensor:
     """fill.Tensor(Tensor self, Tensor value) -> Tensor"""
 
     # after fill, the self Tensor should keep origianl type
     shape = op.Shape(self)
     expanded = op.Expand(value, shape)
     result = op.CastLike(expanded, self)
@@ -2744,15 +2744,15 @@
 
 def aten_gcd(self: TensorType, other: TensorType) -> TensorType:
     """gcd(Tensor self, Tensor other) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::ge")
+@torch_op(("aten::ge", "aten::ge.Tensor", "aten::ge.Scalar"))
 def aten_ge(self: TReal, other: TReal) -> BOOL:
     """ge.Tensor(Tensor self, Tensor other) -> Tensor"""
 
     return op.GreaterOrEqual(self, other)
 
 
 def aten_geqrf(self: TensorType) -> tuple[TensorType, TensorType]:
@@ -2901,15 +2901,15 @@
     b_hh: Optional[TensorType] = None,
 ) -> TensorType:
     """gru_cell(Tensor input, Tensor hx, Tensor w_ih, Tensor w_hh, Tensor? b_ih=None, Tensor? b_hh=None) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::gt")
+@torch_op(("aten::gt", "aten::gt.Scalar"))
 def aten_gt(self: TReal, other: TReal) -> BOOL:
     """gt.Tensor(Tensor self, Tensor other) -> Tensor"""
 
     # TODO(justinchuby): Input spec: non bool tensor
     # Boolean inputs can be pre-casted by policy
     return op.Greater(self, other)
 
@@ -3591,15 +3591,15 @@
 
 def aten_ldexp(self: TensorType, other: TensorType) -> TensorType:
     """ldexp.Tensor(Tensor self, Tensor other) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::le")
+@torch_op(("aten::le", "aten::le.Tensor"))
 def aten_le(self: TReal, other: TReal) -> BOOL:
     """le.Tensor(Tensor self, Tensor other) -> Tensor"""
 
     return op.LessOrEqual(self, other)
 
 
 def aten_lerp(self: TensorType, end: TensorType, weight: TensorType) -> TensorType:
@@ -3880,15 +3880,15 @@
     batch_first: bool,
 ) -> tuple[TensorType, TensorType, TensorType]:
     """lstm_mps_backward(Tensor grad_y, Tensor? grad_hy, Tensor? grad_cy, Tensor z_state, Tensor cell_state_fwd, Tensor input, Tensor[] hx, Tensor[] params, bool has_biases, int num_layers, float dropout, bool train, bool bidirectional, bool batch_first) -> (Tensor, Tensor[], Tensor[])"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::lt")
+@torch_op(("aten::lt", "aten::lt.Scalar"))
 def aten_lt(self: TReal, other: TReal) -> BOOL:
     """lt.Tensor(Tensor self, Tensor other) -> Tensor"""
 
     # TODO(justinchuby): Input spec: non bool tensor
     # Boolean inputs can be pre-casted by policy
     return op.Less(self, other)
 
@@ -3953,15 +3953,15 @@
     reduction: int = 1,
 ) -> TensorType:
     """margin_ranking_loss(Tensor input1, Tensor input2, Tensor target, float margin=0.0, int reduction=Mean) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::masked_fill")
+@torch_op(("aten::masked_fill", "aten::masked_fill.Scalar", "aten::masked_fill.Tensor"))
 def aten_masked_fill(self: TTensor, mask: BOOL, value: TTensor) -> TTensor:
     """masked_fill.Tensor(Tensor self, Tensor mask, Tensor value) -> Tensor"""
     # NOTE: Do not attempt to cast `mask` to BOOL because mask should not take any other types.
     # `mask` coming in as other types is often an error and should fail the model.
     value_cast = op.CastLike(value, self)
     return op.Where(mask, value_cast, self)
 
@@ -4458,23 +4458,23 @@
 
 def aten_msort(self: TensorType) -> TensorType:
     """msort(Tensor self) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::mul")
+@torch_op(("aten::mul", "aten::mul.Tensor"))
 def aten_mul(self: TReal, other: TReal) -> TReal:
     """mul.Tensor(Tensor self, Tensor other) -> Tensor"""
     # FIXME(titaiwang): get rid of this when we have type_promotion
     other = op.CastLike(other, self)
     return op.Mul(self, other)
 
 
-@torch_op("aten::mul")
+@torch_op(("aten::mul", "aten::mul.Tensor"))
 def aten_mul_bool(self: BOOL, other: BOOL) -> BOOL:
     """ONNX Mul doesn't support Boolean, so use And as an equivalent operator."""
 
     # TODO(justinchuby): Handle cases where type reconcilation is not enough,
     # since different ONNX operators are used based on different data types.
 
     return op.And(self, other)
@@ -4879,15 +4879,15 @@
 
 def aten_native_norm(self: TensorType, p: float = 2.0) -> TensorType:
     """native_norm(Tensor self, Scalar p=2) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::ne")
+@torch_op(("aten::ne", "aten::ne.Scalar", "aten::ne.Tensor"))
 def aten_ne(self: TReal, other: TReal) -> BOOL:
     """ne.Tensor(Tensor self, Tensor other) -> Tensor"""
 
     return op.Not(op.Equal(self, other))
 
 
 @torch_op("aten::neg")
@@ -5219,15 +5219,15 @@
 
 def aten_positive(self: TensorType) -> TensorType:
     """positive(Tensor(a) self) -> Tensor(a)"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::pow")
+@torch_op(("aten::pow", "aten::pow.Tensor_Tensor", "aten::pow.Tensor_Scalar"))
 def aten_pow(self: TReal, exponent: TTensor) -> TReal:
     """pow(Tensor self, Tensor exponent) -> Tensor"""
 
     return op.Pow(self, exponent)
 
 
 def aten_prelu(self: TensorType, weight: TensorType) -> TensorType:
@@ -5752,15 +5752,15 @@
 @torch_op("aten::rsqrt")
 def aten_rsqrt(self: TFloatOrBFloat16) -> TFloatOrBFloat16:
     """rsqrt(Tensor self) -> Tensor"""
 
     return op.Reciprocal(op.Sqrt(self))
 
 
-@torch_op("aten::rsub")
+@torch_op(("aten::rsub", "aten::rsub.Scalar"))
 def aten_rsub(self: TReal, other: TReal, alpha: float = 1.0) -> TReal:
     """rsub.Tensor(Tensor self, Tensor other, *, Scalar alpha=1) -> Tensor"""
     # FIXME(titaiwang): get rid of this when we have type_promotion
     other = op.CastLike(other, self)
     alpha = op.CastLike(alpha, self)
     return op.Sub(other, op.Mul(self, alpha))
 
@@ -5781,15 +5781,15 @@
 ) -> TReal:
     """scatter_add(Tensor self, int dim, Tensor index, Tensor src) -> Tensor"""
 
     # if rank(self) == 0 will lead ORT failed, skipped
     return op.ScatterElements(self, index, src, axis=dim, reduction="add")
 
 
-@torch_op("aten::scatter_reduce", trace_only=True)
+@torch_op(("aten::scatter_reduce", "aten::scatter_reduce.two"), trace_only=True)
 def aten_scatter_reduce(
     self: TReal,
     dim: int,  # we have to use int here because ScatterElements() will use this attribute
     index: TInt,
     src: TReal,
     reduce: str,
     include_self: bool = True,  # pylint: disable=unused-argument
@@ -5851,15 +5851,15 @@
     initial: Optional[float] = None,
 ) -> TensorType:
     """segment_reduce(Tensor data, str reduce, *, Tensor? lengths=None, Tensor? indices=None, Tensor? offsets=None, int axis=0, bool unsafe=False, Scalar? initial=None) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::select")
+@torch_op(("aten::select", "aten::select.int"))
 def aten_select(self: TTensor, dim: int, index: int) -> TTensor:
     """select(Tensor self, int dim, int index) -> Tensor"""
 
     return op.Gather(self, index, axis=dim)
 
 
 def aten_select_backward(
@@ -5931,15 +5931,15 @@
 @torch_op("aten::sinh")
 def aten_sinh(self: TFloat) -> TFloat:
     """sinh(Tensor self) -> Tensor"""
 
     return op.Sinh(self)
 
 
-@torch_op("aten::slice", trace_only=True)
+@torch_op(("aten::slice", "aten::slice.Tensor"), trace_only=True)
 def aten_slice(
     self: TTensor,
     dim: int = 0,
     start: Optional[INT64] = None,
     end: Optional[INT64] = None,
     step: Optional[INT64] = None,
 ) -> TTensor:
@@ -6077,15 +6077,15 @@
 
 def aten_sparse_mask(self: TensorType, mask: TensorType) -> TensorType:
     """sparse_mask(Tensor self, Tensor mask) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::split")
+@torch_op(("aten::split", "aten::split.Tensor"))
 def aten_split(self: TTensor, split_size: INT64, dim: int = 0) -> TTensor:
     """split.Tensor(Tensor(a -> *) self, SymInt split_size, int dim=0) -> Tensor(a)[]"""
 
     return op.SplitToSequence(self, split_size, axis=dim)
 
 
 def aten_split_copy(self: TensorType, split_size: INT64, dim: int = 0) -> TensorType:
@@ -6305,30 +6305,30 @@
     # Normalize, if needed
     if normalized:
         result = _normalize_fft_result(self, result, n_fft)
 
     return result
 
 
-@torch_op("aten::sub")
+@torch_op(("aten::sub", "aten::sub.Tensor"))
 def aten_sub(self: TReal, other: TReal, alpha: float = 1.0) -> TReal:
     """sub.Tensor(Tensor self, Tensor other, *, Scalar alpha=1) -> Tensor"""
     alpha = op.CastLike(alpha, other)
     other = op.Mul(other, alpha)
 
     return op.Sub(self, other)
 
 
 def aten_subtract(self: TensorType, other: TensorType, alpha: float = 1.0) -> TensorType:
     """subtract.Tensor(Tensor self, Tensor other, *, Scalar alpha=1) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::sum", trace_only=True)
+@torch_op(("aten::sum", "aten::sum.dim_IntList"), trace_only=True)
 def aten_sum_dim_IntList(
     self: TReal, dim: Optional[INT64] = None, keepdim: bool = False, dtype: int = -1
 ) -> TReal:
     """sum(Tensor self, SymInt dim, bool keepdim, *, ScalarType? dtype=None) -> Tensor"""
 
     # NOTE: trace_only because both if branches need to be the same type, but we have
     # a cast in the if branch.
@@ -6630,15 +6630,15 @@
 
 def aten_trace_backward(grad: TensorType, sizes: INT64) -> TensorType:
     """trace_backward(Tensor grad, SymInt[] sizes) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::transpose", trace_only=True)
+@torch_op(("aten::transpose", "aten::transpose.int"), trace_only=True)
 def aten_transpose(self, dim0: int, dim1: int):
     """transpose.int(Tensor(a) self, int dim0, int dim1) -> Tensor(a)"""
 
     # Use trace only to construct the prem attribute in Transpose
     self_rank = len(self.shape)  # type: ignore[attr-defined]
 
     if self_rank == 0:
@@ -6725,15 +6725,15 @@
 
 def aten_type_as(self: TensorType, other: TensorType) -> TensorType:
     """type_as(Tensor self, Tensor other) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::unbind")
+@torch_op(("aten::unbind", "aten::unbind.int"))
 def aten_unbind(self: TTensor, dim: int = 0) -> Sequence[TTensor]:
     """unbind.int(Tensor(a -> *) self, int dim=0) -> Tensor(a)[]"""
 
     split_sizes = op.Constant(value_int=1)
     return op.SplitToSequence(self, split_sizes, axis=dim, keepdims=0)
 
 
@@ -7078,15 +7078,15 @@
 def aten_vstack(tensors: Sequence[TTensor]) -> TTensor:
     """vstack(Tensor[] tensors) -> Tensor"""
 
     tensors = _aten_atleast_2d_onnx(tensors)
     return op.ConcatFromSequence(tensors, axis=0)
 
 
-@torch_op("aten::where")
+@torch_op(("aten::where", "aten::where.self"))
 def aten_where(condition: BOOL, self: TTensor, other: TTensor) -> TTensor:
     """where.self(Tensor condition, Tensor self, Tensor other) -> Tensor"""
 
     return op.Where(condition, self, other)
 
 
 def aten_xor(self: TensorType, other: TensorType) -> TensorType:
```

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/irbuilder.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/main.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/__init__.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/onnx_types.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/sourceinfo.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tensor.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tensor_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tensor_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/testing.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/testing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/common/onnx_script_test_case.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/common/onnx_script_test_case.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/eager_mode_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/eager_mode_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/eager_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/eager_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/external_tensor_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/external_tensor_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/ops_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/ops_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,23 +54,26 @@
 
 def dtypes_except(*dtypes: torch.dtype) -> Sequence[torch.dtype]:
     """Returns all dtypes except the ones specified."""
     return tuple(dtype for dtype in TESTED_DTYPES if dtype not in dtypes)
 
 
 def _should_skip_xfail_test_sample(
-    op_name: str, sample
+    op_name: str, sample, dtype: torch.dtype
 ) -> Tuple[Optional[str], Optional[str]]:
     """Returns a reason if a test sample should be skipped."""
     if op_name not in ops_test_data.OP_WITH_SKIPPED_XFAIL_SUBTESTS:
         return None, None
     for decorator_meta in ops_test_data.SKIP_XFAIL_SUBTESTS:
         # Linear search on ops_test_data.SKIP_XFAIL_SUBTESTS. That's fine because the list is small.
         if decorator_meta.op_name == op_name:
             assert decorator_meta.matcher is not None, "Matcher must be defined"
+            if decorator_meta.dtypes is not None and dtype not in decorator_meta.dtypes:
+                # Not applicable for this dtype
+                continue
             if decorator_meta.matcher(sample):
                 return decorator_meta.test_behavior, decorator_meta.reason
     return None, None
 
 
 class TestFunctionValidity(unittest.TestCase):
     def test_all_script_functions_are_onnx_functions(self):
@@ -180,15 +183,15 @@
                     if isinstance(inp, torch.Tensor)
                     else inp
                     for inp in inputs
                 ]
             ),
             kwargs=repr(cpu_sample.kwargs),
         ):
-            test_behavior, reason = _should_skip_xfail_test_sample(op.name, cpu_sample)
+            test_behavior, reason = _should_skip_xfail_test_sample(op.name, cpu_sample, dtype)
 
             with ops_test_common.normal_xfail_skip_test_behaviors(test_behavior, reason):
                 input_onnx = [ops_test_common.convert_tensor_to_numpy(x) for x in inputs]
                 kwargs_onnx = ops_test_common.convert_kwargs_for_onnx(cpu_sample.kwargs)
                 if input_wrangler:
                     input_onnx, kwargs_onnx = input_wrangler(input_onnx, kwargs_onnx)
                 torch_output = op(*inputs, **cpu_sample.kwargs)
```

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/ops_test_common.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/ops_test_common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/function_libs/torch_lib/ops_test_data.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/function_libs/torch_lib/ops_test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 import numpy as np
 import torch
 from torch.testing._internal import common_methods_invocations
 from torch.testing._internal.opinfo import definitions as opinfo_definitions
 from typing_extensions import Self
 
 from onnxscript.function_libs.torch_lib.ops import core as core_ops
+from onnxscript.function_libs.torch_lib.ops import linalg as linalg_ops
 from onnxscript.function_libs.torch_lib.ops import nn as nn_ops
 from onnxscript.function_libs.torch_lib.ops import special as special_ops
 from onnxscript.tests.function_libs.torch_lib import extra_opinfo, ops_test_common
 
 # Create a copy of the op_db to modify
 OPS_DB = copy.deepcopy(common_methods_invocations.op_db)
 
@@ -266,14 +267,23 @@
     args.append(inter_mode_options[kwargs["mode"]])
     args.append(padding_mode_options[kwargs["padding_mode"]])
     args.append(kwargs["align_corners"])
     kwargs.clear()
     return args, kwargs
 
 
+def _linalg_vector_norm_input_wrangler(
+    args: list[Any], kwargs: dict[str, Any]
+) -> tuple[list[Any], dict[str, Any]]:
+    # Make the dims as tensor
+    if "dim" in kwargs:
+        kwargs["dim"] = np.array(kwargs["dim"], dtype=np.int64)
+    return args, kwargs
+
+
 def _max_pool_input_wrangler(
     args: list[Any], kwargs: dict[str, Any]
 ) -> tuple[list[Any], dict[str, Any]]:
     # Remove return_indices argument because this op doesn't accept it
     if "return_indices" in kwargs:
         del kwargs["return_indices"]
     return args, kwargs
@@ -627,14 +637,25 @@
     TorchLibOpInfo("isclose", core_ops.aten_isclose),
     TorchLibOpInfo("isfinite", core_ops.aten_isfinite),
     TorchLibOpInfo("isinf", core_ops.aten_isinf),
     TorchLibOpInfo("isnan", core_ops.aten_isnan),
     TorchLibOpInfo("isneginf", core_ops.aten_isneginf),
     TorchLibOpInfo("isposinf", core_ops.aten_isposinf),
     TorchLibOpInfo(
+        "linalg.vector_norm",
+        linalg_ops.aten_linalg_vector_norm,
+        trace_only=True,
+        tolerance={torch.float16: (2e-3, 2e-3)},
+        input_wrangler=_linalg_vector_norm_input_wrangler,
+    ).skip(
+        matcher=lambda sample: sample.kwargs.get("ord") == 6,
+        dtypes=[torch.float16],
+        reason="ORT returns a more accurate value for float16 with ord=6 (expected=Inf, actual=9.48).",
+    ),
+    TorchLibOpInfo(
         "linspace",
         core_ops.aten_linspace,
         trace_only=True,
     )
     .xfail(
         dtypes=(torch.int64,),
         reason="fixme: Results do not match with PyTorch. https://github.com/microsoft/onnxscript/issues/854",
```

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/attr_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/attr_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/gemmgelu.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/gemmgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/gemmgelu_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/gemmgelu_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/if_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/if_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/onnxfns1A_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/onnxfns1A_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/onnxfns2_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/onnxfns2_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/onnxfns_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/onnxfns_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/functions/ort_custom_ops.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/functions/ort_custom_ops.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/if_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/if_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/loop_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/loop_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/attrref.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/attrref.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/cast_like.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/cast_like.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/different_opset.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/different_opset.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/dropout.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/dropout.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/eager_op.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/eager_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/eg1.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/eg1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/getitem.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/getitem.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/graph_attr.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/graph_attr.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/identity.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/identity.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/if_statement.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/if_statement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/loops_break.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/loops_break.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/loops_while.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/loops_while.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/onnxfns1.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/onnxfns1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/onnxfns1A.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/onnxfns1A.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/onnxfns2.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/onnxfns2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/opt_input.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/opt_input.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/opt_output.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/opt_output.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/renaming.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/renaming.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/sequences.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/sequences.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/signal_dft.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/signal_dft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/subfunction.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/subfunction.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/models/type_double.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/models/type_double.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/onnx_types_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/onnx_types_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/tests/operator_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/tests/operator_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/type_annotation.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/type_annotation_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/type_annotation_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/utils.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/values.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript/values_test.py` & `onnxscript-preview-0.1.0.dev20230726/onnxscript/values_test.py`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/PKG-INFO` & `onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript-preview
-Version: 0.1.0.dev20230724
+Version: 0.1.0.dev20230726
 Summary: Authoring ONNX functions in Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-preview-0.1.0.dev20230724/onnxscript_preview.egg-info/SOURCES.txt` & `onnxscript-preview-0.1.0.dev20230726/onnxscript_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/pyproject.toml` & `onnxscript-preview-0.1.0.dev20230726/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-preview-0.1.0.dev20230724/setup.py` & `onnxscript-preview-0.1.0.dev20230726/setup.py`

 * *Files identical despite different names*

