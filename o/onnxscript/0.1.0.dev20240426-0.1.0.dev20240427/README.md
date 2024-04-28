# Comparing `tmp/onnxscript-0.1.0.dev20240426.tar.gz` & `tmp/onnxscript-0.1.0.dev20240427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240426.tar", last modified: Fri Apr 26 00:01:07 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240427.tar", last modified: Sat Apr 27 00:02:12 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240426.tar` & `onnxscript-0.1.0.dev20240427.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.025172 onnxscript-0.1.0.dev20240426/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.025172 onnxscript-0.1.0.dev20240426/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.029172 onnxscript-0.1.0.dev20240426/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.029172 onnxscript-0.1.0.dev20240426/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.029172 onnxscript-0.1.0.dev20240426/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.021172 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.029172 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.041172 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.021172 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.021172 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.045172 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.045172 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.045172 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.049172 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.049172 onnxscript-0.1.0.dev20240426/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.049172 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.057172 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.057172 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4316 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6603 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35227 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5522 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24160 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    37876 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-26 00:01:07.000000 onnxscript-0.1.0.dev20240426/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-04-26 00:01:07.000000 onnxscript-0.1.0.dev20240426/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-26 00:01:07.000000 onnxscript-0.1.0.dev20240426/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-26 00:01:07.000000 onnxscript-0.1.0.dev20240426/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-26 00:01:07.000000 onnxscript-0.1.0.dev20240426/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-26 00:01:07.061172 onnxscript-0.1.0.dev20240426/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-04-26 00:00:49.000000 onnxscript-0.1.0.dev20240426/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.032933 onnxscript-0.1.0.dev20240427/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:11.996933 onnxscript-0.1.0.dev20240427/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.000933 onnxscript-0.1.0.dev20240427/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.000933 onnxscript-0.1.0.dev20240427/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.000933 onnxscript-0.1.0.dev20240427/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.000933 onnxscript-0.1.0.dev20240427/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:11.992933 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.004933 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.012933 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:11.992933 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:11.992933 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.012933 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.012933 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.012933 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.016933 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.016933 onnxscript-0.1.0.dev20240427/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.020933 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.024933 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.024933 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4597 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6603 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35227 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5522 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24160 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36123 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-27 00:02:11.000000 onnxscript-0.1.0.dev20240427/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-04-27 00:02:11.000000 onnxscript-0.1.0.dev20240427/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-27 00:02:11.000000 onnxscript-0.1.0.dev20240427/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-27 00:02:11.000000 onnxscript-0.1.0.dev20240427/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-27 00:02:11.000000 onnxscript-0.1.0.dev20240427/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-27 00:02:12.032933 onnxscript-0.1.0.dev20240427/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240426/LICENSE` & `onnxscript-0.1.0.dev20240427/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/PKG-INFO` & `onnxscript-0.1.0.dev20240427/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240426
+Version: 0.1.0.dev20240427
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240426/README.md` & `onnxscript-0.1.0.dev20240427/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240427/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240427/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240427/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240427/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240427/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240427/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240427/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240427/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240427/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240427/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240427/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240427/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240427/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240427/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240427/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240427/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240427/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240427/onnxscript/ir/_convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240427/onnxscript/ir/_core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240427/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240427/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240427/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240427/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240427/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240427/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240427/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240427/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240427/onnxscript/ir/serde.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240427/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/main.py` & `onnxscript-0.1.0.dev20240427/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240427/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,16 +54,20 @@
             "To achieve the same behavior as 'function_aware_folding=True' before, set 'onnx_shape_inference=False'. "
             "This would turn off incremental onnx shape inference and rely on model carried shapes and types. "
             "See 'onnx_shape_inference' for more details."
         )
     for _ in range(num_iterations):
         if onnx_shape_inference:
             if model.ByteSize() < 1024 * 1024 * 1024 * 2:
+                # NOTE: strict mode is disabled because it crashes on the models
+                # that have different shapes inferred from the model carried shapes.
+                # The case can be found in:
+                # https://github.com/microsoft/onnxscript/issues/1443
                 model = onnx.shape_inference.infer_shapes(
-                    model, check_type=True, strict_mode=True, data_prop=True
+                    model, check_type=True, strict_mode=False, data_prop=True
                 )
             else:
                 logger.warning(
                     "The model size is too large for full model shape inference. "
                     "Skipping this step."
                 )
```

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/copy_propagation.py` & `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/copy_propagation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import dataclasses
 import inspect
 import itertools
 import math
-from typing import Any, Callable, List, Optional, Sequence, Tuple
+from typing import Any, Callable, List, MutableSequence, Optional, Sequence, Tuple
 
 import numpy as np
 import onnx
 import onnx.numpy_helper
 import onnx.printer
 
 from onnxscript import ir
@@ -316,77 +316,71 @@
     raise TypeError(f"Cannot convert {type(x)} to ValuePattern")
 
 
 class MatchResult:
     """Represents the result of a match operation.
 
     A match can either succeed or fail.
-    If it succeeds, it returns a list of IR values that matched the pattern
+    If it succeeds, it returns a list of nodes that matched the pattern
     and a set of bindings for the variables in the pattern.
 
     Example:
     ::
         def pattern(x, shape1, shape2):
             t1 = op.Reshape(x, shape1)
             t2 = op.Reshape(t1, shape2)
             return t2
     The above pattern matches a sequence of two Reshape ops.
-    The matched_values will contain the values representing the (output of)
-    the two Reshape ops, and the bindings will contain the values that
-    are bound to the variables `x`, `shape1`, and `shape2`.
+    The matched_nodes will contain the two Reshape ops, and the bindings will
+    contain the values that are bound to the variables `x`, `shape1`, and `shape2`.
     """
 
-    def __init__(
-        self, matched_values=None, bindings: dict[str, ir.Value | Any] | None = None
-    ) -> None:
-        assert matched_values is None or isinstance(matched_values, list)
-        self.success: bool = matched_values is not None
-        # For a successful match, matched_values is a list of values that matched the pattern.
+    def __init__(self, success: bool) -> None:
+        self.success: bool = success
+        # For a successful match, matched_nodes is a list of values that matched the pattern.
         # These include the internal nodes of the pattern that were matched, but not
         # the leaves (sub-trees) that match against the variables in the pattern.
         # These represent the values that will be replaced by the replacement pattern.
-        self.matched_values: Sequence[Any] | None = matched_values
+        self.matched_nodes: MutableSequence[ir.Node] = []
         # For a successful match, bindings is a dictionary of mapping pattern-variable-names
         # to values.
-        self.bindings: dict[str, Any] = bindings if bindings is not None else {}
+        self.bindings: dict[str, Any] = {}
 
     def __bool__(self):
         return self.success
 
     @classmethod
     def FAIL(cls):
-        return cls(None)
+        return cls(False)
 
     @property
-    def values(self) -> Sequence[Any] | None:
-        return self.matched_values
+    def nodes(self) -> MutableSequence[ir.Node]:
+        return self.matched_nodes
 
-    def fail(self):
-        self.success = False
-        self.matched_values = None
-        self.bindings = {}
+    def bind(self, var: str, value: Any):
+        self.bindings[var] = value
 
     def extend(self, other: MatchResult | bool):
         if not self.success:
             return
         if not other:
-            self.fail()
+            self.success = False
             return
         if isinstance(other, bool):
             return
         for var, val in other.bindings.items():
             if var in self.bindings:
                 # TODO: handle attribute var bindings
                 if self.bindings[var] != val:
-                    self.fail()
+                    self.success = False
                     return
             else:
                 self.bindings[var] = val
-        assert self.matched_values is not None, "matched_values should not be None."
-        self.matched_values.extend(other.matched_values)  # type: ignore[attr-defined]
+        assert self.matched_nodes is not None, "matched_nodes should not be None."
+        self.matched_nodes.extend(other.matched_nodes)  # type: ignore[attr-defined]
 
 
 class ValuePattern:
     """Base class for all patterns that match against IR values.
 
     This is used primarily to provide operator overloadings for arithmetic
     operations, so that we can write patterns like `x + 1` and `1 + x`.
@@ -395,17 +389,18 @@
     def __init__(self, name: str | None) -> None:
         self.name = name
 
     def __repr__(self) -> str:
         return f"ValuePattern({self.name!r})"
 
     def matches(self, value: ir.Value, model: ir.Model):
-        if self.name is None:
-            return MatchResult([], {})
-        return MatchResult([], {self.name: value})
+        result = MatchResult(success=True)
+        if self.name is not None:
+            result.bind(self.name, value)
+        return result
 
     def commute(self) -> Sequence[ValuePattern]:
         """Return a list of commuted patterns.
 
         This is used to handle commutative operations like addition and multiplication.
         A single pattern is converted into a list of equivalent patterns by swapping
         the parameters of commutative operations.
@@ -463,15 +458,15 @@
 
     def matches_node(self, node: ir.Node, model: ir.Model) -> MatchResult:
         """Examine if the IR node matches the self pattern."""
         if not self.domain.matches(node.domain):
             return MatchResult.FAIL()
         if not self.op.matches(node.op_type):
             return MatchResult.FAIL()
-        match = MatchResult([])
+        match = MatchResult(success=True)
         # TODO: We should add filtered logging starting from here to emit why
         # matching failed. This should cut a lot of noises compared to logging everything,
         # because at least the starting node op_type is already matched.
         for arg_value, previous_node_output_pattern in zip(node.inputs, self.inputs):
             # previous_node_output_pattern could be a Var, if it's the original arg.
             if arg_value is None and previous_node_output_pattern is None:
                 continue
@@ -487,19 +482,19 @@
             if attr_value is None:
                 return MatchResult.FAIL()
             sub_match = attr_pattern.matches(attr_value, model)  # type: ignore[arg-type]
             if not sub_match:
                 return MatchResult.FAIL()
             match.extend(sub_match)
         for name in node.attributes:
-            # TODO: Support matching default values for attributes.
+            # TODO: Support matching default nodes for attributes.
             if name not in self.attributes:
                 return MatchResult.FAIL()
-        assert match.values is not None, "Matched values should not be None."
-        match.values.append(node)  #  type: ignore[attr-defined]
+        assert match.nodes is not None, "Matched nodes should not be None."
+        match.nodes.append(node)
         return match
 
     def commute(self) -> Sequence[NodePattern]:
         list_of_lists = [
             [None] if pattern is None else pattern.commute() for pattern in self.inputs
         ]  # type: ignore[attr-defined]
 
@@ -559,36 +554,35 @@
         self, value: int | float, rel_tol: float = 1e-5, abs_tol: float = 1e-8
     ) -> None:
         super().__init__(None)
         self.value = value
         self.rel_tol = rel_tol
         self.abs_tol = abs_tol
 
-    def match_scalar(self, scalar_value, return_value: Sequence[ir.Node]):
-        if math.isclose(scalar_value, self.value, rel_tol=self.rel_tol, abs_tol=self.abs_tol):
-            return MatchResult(return_value)
-        return MatchResult.FAIL()
+    def match_scalar(self, scalar_value):
+        status = math.isclose(
+            scalar_value, self.value, rel_tol=self.rel_tol, abs_tol=self.abs_tol
+        )
+        # Note: If the value is produced by a Constant node, we could include
+        # the Constant node in the return_value list. However, we don't do that.
+        # Instead, we will rely on DCE to remove the constant node if it is not
+        # used elsewhere.
+        return MatchResult(success=status)
 
     def matches(self, value: ir.Value, model: ir.Model):
         value = _ir_utils.propagate_const_value(value)
         constant_value = _ir_utils.get_numpy_from_ir_value(value)
         if constant_value is None:
             return MatchResult.FAIL()
 
         # TODO (rama): allow users to specify shape requirement, if desired.
         if constant_value.size != 1:
             return MatchResult.FAIL()
 
-        return_value: list[ir.Node] = []
-        # Note: If the value is produced by a Constant node, we could include
-        # the Constant node in the return_value list. However, we don't do that.
-        # Instead, we will rely on DCE to remove the constant node if it is not
-        # used elsewhere.
-
-        return self.match_scalar(constant_value.item(), return_value)
+        return self.match_scalar(constant_value.item())
 
     def commute(self) -> list[ValuePattern]:
         return [self]
 
 
 def _handle_pattern_return_value(
     node_output_pattern: NodeOutputPattern | list[NodeOutputPattern],
@@ -631,15 +625,15 @@
                     "Use other APIs to handle multi-output patterns."
                 )
     else:
         raise TypeError(f"Invalid type {type(node_output_pattern)} for pattern")
     return node_pattern, num_outputs
 
 
-def _valid_to_replace(matched_nodes: Sequence[Any]) -> bool:
+def _valid_to_replace(matched_nodes: Sequence[ir.Node]) -> bool:
     """Check that values computed by the matched_nodes, except for the last one, are used only by the matched_nodes."""
     # * Must check that all values matched by pattern are used only by pattern,
     # except for the value that is replaced.
     # * Must ensure that replacement subgraph does not use any of the deleted
     # (intermediate) values. (Not necessary for now. Guaranteed.)
     deleted_nodes = matched_nodes[:-1]
     for n in deleted_nodes:
@@ -717,38 +711,38 @@
         return self._used_opsets
 
 
 @dataclasses.dataclass
 class ReplacementSubgraph:
     """A subgraph that will replace the matched pattern."""
 
-    new_values: Sequence[ir.Value]
+    match: MatchResult
+    new_outputs: Sequence[ir.Value]
     new_nodes: Sequence[ir.Node]
     used_opsets: UsedOpsets
 
 
 class ReplacementPatternFunction:
     """The replacement pattern that will replace the targeted pattern.
 
     Attributes:
         function (Callable): The replacement function that will be used to replace the matched pattern.
     """
 
     def __init__(self, function) -> None:
         self._function = function
 
-    def get_replacement(
-        self,
-        match_bindings: dict[str, ir.Value | Any] | None = None,
-    ) -> ReplacementSubgraph:
+    def get_replacement(self, match: MatchResult) -> ReplacementSubgraph | None:
         context = RewriterContext()
-        new_values = self._function(context, **match_bindings)
-        if not isinstance(new_values, Sequence):
-            new_values = [new_values]
-        return ReplacementSubgraph(new_values, context.nodes, context.used_opsets)
+        new_outputs = self._function(context, **match.bindings)
+        if new_outputs is None:
+            return None  # Failed to create replacement subgraph
+        if not isinstance(new_outputs, Sequence):
+            new_outputs = [new_outputs]
+        return ReplacementSubgraph(match, new_outputs, context.nodes, context.used_opsets)
 
 
 def _update_opset_imports(
     graph_or_function: ir.Graph | ir.Function, delta: ReplacementSubgraph
 ):
     imports = graph_or_function.opset_imports
     for domain, version in delta.used_opsets:
@@ -819,37 +813,34 @@
             and not self._condition_function(match.bindings)
         ):
             return MatchResult.FAIL()
         return match
 
     def try_rewrite(
         self, model: ir.Model, graph_or_function: ir.Graph | ir.Function, node: ir.Node
-    ):  # TODO(rama) -> ReplacementSubgraph | None:
+    ) -> ReplacementSubgraph | None:
         """If the node matches the pattern, then replace the node with the replacement pattern."""
         match = self.matches(node, model)
         if match:
-            assert match.values is not None, "Matched values should not be None."
-            if _valid_to_replace(match.values):
-                # bindings will be consumed by the replacement function
-                delta = self._replacement_pattern.get_replacement(match.bindings)
-                if len(delta.new_values) != self._target_num_outputs:
+            assert match.nodes is not None, "Matched values should not be None."
+            if _valid_to_replace(match.nodes):
+                replacement_subgraph = self._replacement_pattern.get_replacement(match)
+                if replacement_subgraph is None:
+                    return None
+                if len(replacement_subgraph.new_outputs) != self._target_num_outputs:
                     raise ValueError(
                         f"Number of outputs from replacement function does not match the number of outputs from the target pattern. "
-                        f"Expected {self._target_num_outputs}, but got {len(delta.new_values)}."
+                        f"Expected {self._target_num_outputs}, but got {len(replacement_subgraph.new_outputs)}."
                     )
                 # TODO(rama): Check/update opset-imports
-                # (i) Integrate following with the multi-output matcher and code elsewhere:
+                # (i) Following is required by multi-output matcher too; move this.
                 # (ii) Remove the opset imports from deleted nodes?
-                # (iii) Code in the caller (below) checks if match overlaps previous match, which
-                # appears incorrect for single-pattern matcher. Best to alter iteration to apply
-                # each rewrite immediately, instead of accumulating them.
-                # (iv) return delta here
-                _update_opset_imports(graph_or_function, delta)
-                _update_opset_imports(model.graph, delta)
-                return match.values, delta.new_nodes
+                _update_opset_imports(graph_or_function, replacement_subgraph)
+                _update_opset_imports(model.graph, replacement_subgraph)
+                return replacement_subgraph
         return None
 
     def apply_to_model(self, model: ir.Model, *, commute: bool = False):
         # TODO(titaiwang): Why do we need RewriteRuleSet?
         return RewriteRuleSet([self], commute=commute).apply_to_model(model)
 
     def count_matches(self, model: ir.Model, *, commute: bool = False):
@@ -865,20 +856,21 @@
             rule._replacement_pattern = self._replacement_pattern
             rule._vars = self._vars
             return rule
 
         return [replace_pattern(p) for p in self._target_node_pattern.commute()]
 
 
-def _apply_deltas(
+def _apply_delta(
     graph_or_function: ir.Graph | ir.Function,
+    node: ir.Node,
     # TODO(jutinchuby): Use a more descriptive data structure to store deltas
-    deltas: Sequence[tuple[int, tuple[Sequence[ir.Node], Sequence[ir.Node]]]],
+    delta,
 ):
-    """Applies deltas.
+    """Applies delta.
 
     This code is valid is the considered pattern has only one output.
     In case of multi output replacements, there is not need to rename
     the outputs.
 
     In case of multi-output design, the nodes may not be necessary inserted
     all at the same position. To be convinced, you can take a pattern
@@ -887,116 +879,86 @@
     the right place to inserted all of the node.
 
     The current implementation insert all the nodes at the same position
     but checks there is not inconsistency. In that case, it fails.
     We could reorder (long) or do more clever changes.
     The reordering would probably happen not very often.
     """
-    existing_ids = {id(n): (i, n) for i, n in enumerate(graph_or_function)}
-    to_delete: set[ir.Node] = set()
-    to_insert: list[tuple[ir.Node, list[ir.Node]]] = []
-
-    for i, delta in reversed(deltas):
-        if len(delta) == 3:
-            # multi-outut strategy
-            n_matches, deleted_nodes, inserted_nodes = delta
-            for d in deleted_nodes:
-                assert id(d) in existing_ids
-                to_delete.add(d)
-
-            # the position to insert must be chosen.
-            # we'll try position i
-            assert i not in to_insert  # conflicts should avoid that case
-            to_insert.append((graph_or_function[i], inserted_nodes))
-        else:
-            deleted_nodes, inserted_nodes = delta
-            # Replace deleted nodes with inserted nodes.
-            # TODO: simplify this
-            last_deleted = deleted_nodes[-1]
-            last_inserted = inserted_nodes[-1]
-
-            for old_value, new_value in zip(last_deleted.outputs, last_inserted.outputs):
-                # Propagate relevant info from old value to new value
-                # TODO(Rama): Perhaps we should merge old and new types. As of now, new
-                # values don't have type information. Note that this could be a problem
-                # for semantics-altering rewrite-rules: we should allow users to override
-                # this for such rules.
-                new_value.type = old_value.type
-                new_value.shape = old_value.shape
-                new_value.const_value = old_value.const_value
-                new_value.name = old_value.name
-
-            # Reconnect the users of the deleted node to use the new outputs
-            _convenience.replace_all_uses_with(last_deleted.outputs, last_inserted.outputs)
-            # Update graph/function outputs if the node generates output
-            replacement_mapping = dict(zip(last_deleted.outputs, last_inserted.outputs))
-            for idx, graph_or_function_output in enumerate(graph_or_function.outputs):
-                if graph_or_function_output in replacement_mapping:
-                    graph_or_function.outputs[idx] = replacement_mapping[
-                        graph_or_function_output
-                    ]
-
-            # insert new nodes after the index node
-            graph_or_function.insert_after(last_deleted, inserted_nodes)
-            graph_or_function.remove(deleted_nodes, safe=True)
 
-    for replaced_node, inserted_nodes in to_insert:
-        graph_or_function.insert_after(replaced_node, inserted_nodes)
+    if isinstance(delta, tuple):
+        # multi-output strategy
+        n_matches, matched_nodes, inserted_nodes = delta
+
+        # TODO(rama): Was "assert i not in to_insert"; seems wrong.
+        # What is this trying to check? Best effort correction below.
+        assert node not in inserted_nodes  # conflicts should avoid that case
+
+        graph_or_function.insert_after(node, inserted_nodes)
         # TODO: improve this
         # This is updating the graph/function outputs to use the new outputs
         for inserted_node in inserted_nodes:
             for new_output in inserted_node.outputs:
                 if (index := new_output.meta.get(_ir_utils.GRAPH_OUTPUT_META_KEY)) is not None:  # type: ignore[assignment]
                     graph_or_function.outputs[index] = new_output
 
-    graph_or_function.remove(to_delete, safe=True)
+        for d in matched_nodes:
+            assert d in graph_or_function
+        graph_or_function.remove(matched_nodes, safe=True)
+    else:
+        assert isinstance(delta, ReplacementSubgraph)
+        # Replace matched nodes with new nodes.
+        last_inserted = delta.new_nodes[-1]
+
+        for old_value, new_value in zip(node.outputs, last_inserted.outputs):
+            # Propagate relevant info from old value to new value
+            # TODO(Rama): Perhaps we should merge old and new types. As of now, new
+            # values don't have type information. Note that this could be a problem
+            # for semantics-altering rewrite-rules: we should allow users to override
+            # this for such rules.
+            new_value.type = old_value.type
+            new_value.shape = old_value.shape
+            new_value.const_value = old_value.const_value
+            new_value.name = old_value.name
+
+        # Reconnect the users of the deleted node to use the new outputs
+        _convenience.replace_all_uses_with(node.outputs, last_inserted.outputs)
+        # Update graph/function outputs if the node generates output
+        replacement_mapping = dict(zip(node.outputs, last_inserted.outputs))
+        for idx, graph_or_function_output in enumerate(graph_or_function.outputs):
+            if graph_or_function_output in replacement_mapping:
+                graph_or_function.outputs[idx] = replacement_mapping[graph_or_function_output]
+
+        # insert new nodes after the index node
+        graph_or_function.insert_after(node, delta.new_nodes)
+        graph_or_function.remove(delta.match.nodes, safe=True)
 
 
 class RewriteRuleSet:
     def __init__(self, rules: Sequence[RewriteRule], *, commute: bool = False) -> None:
         if commute:
             rules = list(itertools.chain.from_iterable([rule.commute() for rule in rules]))
         self.rules = rules
 
     def _apply_to_graph_or_function(
         self,
         model: ir.Model,
         graph_or_function: ir.Graph | ir.Function,
     ) -> int:
         count = 0
-        marked = set()
+
         # NOTE: Rules should be prioritized in the order they are added to the RewriteRuleSet.
         # And the graph is applied in order.
         for rule in self.rules:
-            deltas = []
-            for i, node in enumerate(graph_or_function):
+            for node in graph_or_function:
                 delta = rule.try_rewrite(model, graph_or_function, node)
-
                 if delta is None:
                     continue
-
-                matched_nodes, _ = delta[-2:]
-
-                conflict = False
-                for n in matched_nodes:
-                    if id(n) in marked:
-                        # The same node cannot be matched twice with different patterns.
-                        conflict = True
-                        break
-
-                if conflict:
-                    # Some nodes are already marked as rewritten.
-                    continue
-
-                marked |= set(map(id, matched_nodes))
-
-                deltas.append((i, delta))
+                _apply_delta(graph_or_function, node, delta)
                 count += 1
 
-            _apply_deltas(graph_or_function, deltas)
         return count
 
     def apply_to_model(self, model: ir.Model) -> int:
         assert isinstance(model, ir.Model)
         count = self._apply_to_graph_or_function(model, model.graph)
         for function in model.functions.values():
             count += self._apply_to_graph_or_function(model, function)
```

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240427/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240427/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240427/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240427/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240427/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240427/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240427/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript/values.py` & `onnxscript-0.1.0.dev20240427/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240427/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240426
+Version: 0.1.0.dev20240427
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240426/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240427/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/pyproject.toml` & `onnxscript-0.1.0.dev20240427/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240426/setup.py` & `onnxscript-0.1.0.dev20240427/setup.py`

 * *Files identical despite different names*

