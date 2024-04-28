# Comparing `tmp/types-tensorflow-2.16.0.20240424.tar.gz` & `tmp/types-tensorflow-2.16.0.20240428.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tensorflow-2.16.0.20240424.tar", last modified: Wed Apr 24 02:17:57 2024, max compression
+gzip compressed data, was "types-tensorflow-2.16.0.20240428.tar", last modified: Sun Apr 28 02:22:24 2024, max compression
```

## Comparing `types-tensorflow-2.16.0.20240424.tar` & `types-tensorflow-2.16.0.20240428.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.866320 types-tensorflow-2.16.0.20240424/
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-24 02:17:57.000000 types-tensorflow-2.16.0.20240424/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 02:17:57.000000 types-tensorflow-2.16.0.20240424/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-24 02:17:57.866320 types-tensorflow-2.16.0.20240424/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:17:57.866320 types-tensorflow-2.16.0.20240424/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-24 02:17:57.000000 types-tensorflow-2.16.0.20240424/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.842320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 02:17:57.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    16662 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/_aliases.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/audio.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/autodiff.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.842320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/autograph/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/autograph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/autograph/experimental.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/bitwise.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.838320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.842320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.846320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/service/
--rw-r--r--   0 runner    (1001) docker     (127)    80163 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/service/hlo_profile_printer_data_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/service/test_compilation_environment_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/service/xla_compile_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    95569 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   126501 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/xla_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.846320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/config/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/config/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.838320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.846320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/example/
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/example/example_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/example/feature_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.850320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/api_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/attr_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/cpp_shape_inference_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/dataset_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/full_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/graph_debug_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/log_memory_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/node_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/op_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/reader_base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/step_stats_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/summary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/variable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.854320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    77429 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/debug_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29456 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/rpc_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26715 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/saver_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20084 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.854320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tpu/
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    51846 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.858320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/util/
--rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/util/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/util/test_log_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.858320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/data/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.858320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/distribute/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/distribute/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/distribute/coordinator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.858320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/distribute/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/distribute/experimental/coordinator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.858320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/experimental/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/experimental/dtensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.858320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/feature_column/
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.858320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/io/
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/io/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/io/gfile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.858320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/activations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/callbacks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.858320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    16491 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/layers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/losses.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/metrics.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/models.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.858320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/optimizers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.858320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/optimizers/schedules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/regularizers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/linalg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/math.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/nn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 02:17:57.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.862320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.862320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/distribute/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/distribute/distribute_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.862320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/feature_column/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.862320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/framework/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.862320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/keras/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/keras/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.862320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/keras/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.862320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/trackable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/trackable/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/trackable/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/trackable/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/trackable/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/trackable/ressource.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.838320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/training/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.862320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/training/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/training/tracking/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/random.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/raw_ops.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.862320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/saved_model/
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/saved_model/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/saved_model/experimental.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/sparse.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/strings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/summary.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.862320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/train/
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/train/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/train/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.838320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.866320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    25411 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21347 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.866320 types-tensorflow-2.16.0.20240424/tensorflow-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-24 02:17:29.000000 types-tensorflow-2.16.0.20240424/tensorflow-stubs/types/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:57.866320 types-tensorflow-2.16.0.20240424/types_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-24 02:17:57.000000 types-tensorflow-2.16.0.20240424/types_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-24 02:17:57.000000 types-tensorflow-2.16.0.20240424/types_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:17:57.000000 types-tensorflow-2.16.0.20240424/types_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 02:17:57.000000 types-tensorflow-2.16.0.20240424/types_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 02:17:57.000000 types-tensorflow-2.16.0.20240424/types_tensorflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.923978 types-tensorflow-2.16.0.20240428/
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-04-28 02:22:24.000000 types-tensorflow-2.16.0.20240428/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-28 02:22:24.000000 types-tensorflow-2.16.0.20240428/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-28 02:22:24.923978 types-tensorflow-2.16.0.20240428/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 02:22:24.923978 types-tensorflow-2.16.0.20240428/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-28 02:22:24.000000 types-tensorflow-2.16.0.20240428/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.903978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-28 02:22:24.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    16662 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/_aliases.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/audio.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/autodiff.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.903978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/autograph/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/autograph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/autograph/experimental.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/bitwise.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.895978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.903978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.903978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    80163 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/service/hlo_profile_printer_data_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/service/test_compilation_environment_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/service/xla_compile_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    95569 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   126501 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/xla_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.903978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/config/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.895978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.903978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/example/example_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/example/feature_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.907978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/api_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/attr_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/cpp_shape_inference_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/dataset_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/full_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/graph_debug_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/log_memory_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/node_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/op_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/reader_base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/step_stats_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/summary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/variable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.915978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    77429 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/debug_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29456 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/rpc_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26715 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/saver_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20084 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.915978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    51846 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.915978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/util/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/util/test_log_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.915978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/data/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.915978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/distribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/distribute/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/distribute/coordinator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.915978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/distribute/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/distribute/experimental/coordinator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.915978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/experimental/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/experimental/dtensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.915978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.915978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/io/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/io/gfile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/activations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/callbacks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    16491 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/layers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/losses.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/metrics.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/models.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/optimizers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/optimizers/schedules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/regularizers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/linalg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/math.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/nn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 02:22:24.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/distribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/distribute/distribute_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/framework/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/keras/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/keras/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/trackable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/trackable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/trackable/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/trackable/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/trackable/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/trackable/ressource.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.899978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/training/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/training/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/training/tracking/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/random.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/raw_ops.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.919978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/saved_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/saved_model/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/saved_model/experimental.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/sparse.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/strings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/summary.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.923978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/train/
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/train/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/train/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.899978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.923978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25411 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21347 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.923978 types-tensorflow-2.16.0.20240428/tensorflow-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-28 02:22:01.000000 types-tensorflow-2.16.0.20240428/tensorflow-stubs/types/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:22:24.923978 types-tensorflow-2.16.0.20240428/types_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-28 02:22:24.000000 types-tensorflow-2.16.0.20240428/types_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-28 02:22:24.000000 types-tensorflow-2.16.0.20240428/types_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 02:22:24.000000 types-tensorflow-2.16.0.20240428/types_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-28 02:22:24.000000 types-tensorflow-2.16.0.20240428/types_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 02:22:24.000000 types-tensorflow-2.16.0.20240428/types_tensorflow.egg-info/top_level.txt
```

### Comparing `types-tensorflow-2.16.0.20240424/CHANGELOG.md` & `types-tensorflow-2.16.0.20240428/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.16.0.20240428 (2024-04-28)
+
+Fix stubtest for TensorFlow with latest keras release (#11838)
+
 ## 2.16.0.20240424 (2024-04-24)
 
 Fix stubtest errors in tensorflow with `keras>=3.3.2` (#11817)
 
 ## 2.16.0.20240423 (2024-04-23)
 
 Bump tensorflow to 2.16.* (#11696)
```

### Comparing `types-tensorflow-2.16.0.20240424/PKG-INFO` & `types-tensorflow-2.16.0.20240428/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.16.0.20240424
+Version: 2.16.0.20240428
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -34,10 +34,10 @@
 Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.16.1 .
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7ed91bc2e77ec18d28307dc6086a778ecc9c7bb3` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `bdf75023dfe3930deac1c6b4e269770427b106c4` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
```

### Comparing `types-tensorflow-2.16.0.20240424/setup.py` & `types-tensorflow-2.16.0.20240428/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.16.1 .
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7ed91bc2e77ec18d28307dc6086a778ecc9c7bb3` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `bdf75023dfe3930deac1c6b4e269770427b106c4` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.16.0.20240424",
+      version="2.16.0.20240428",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md",
```

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/METADATA.toml` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/METADATA.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 # requires a version of numpy with a `py.typed` file
 requires = ["numpy>=1.20", "types-protobuf", "types-requests"]
 extra_description = "Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.16.1 ."
 partial_stub = true
 
 [tool.stubtest]
 ignore_missing_stub = true
-stubtest_requirements = ["keras>=3.3.2"]
+stubtest_requirements = ["keras>=3.3.3"]
```

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/__init__.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/_aliases.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/_aliases.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/autodiff.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/autodiff.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/autograph/__init__.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/autograph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/autograph/experimental.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/autograph/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/bitwise.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/bitwise.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/service/hlo_profile_printer_data_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/service/hlo_profile_printer_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/service/test_compilation_environment_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/service/test_compilation_environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/service/xla_compile_result_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/service/xla_compile_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/compiler/xla/xla_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/compiler/xla/xla_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/config/__init__.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/config/experimental.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/config/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/example/example_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/example/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/example/feature_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/example/feature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/allocation_description_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/allocation_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/api_def_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/api_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/attr_value_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/attr_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/cost_graph_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/cost_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/cpp_shape_inference_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/cpp_shape_inference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/dataset_options_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/dataset_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/dataset_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/device_attributes_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/device_attributes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/full_type_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/full_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/function_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/graph_debug_info_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/graph_debug_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/graph_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/kernel_def_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/kernel_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/log_memory_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/log_memory_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/model_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/node_def_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/node_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/op_def_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/op_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/reader_base_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/reader_base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/resource_handle_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/resource_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/step_stats_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/step_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/summary_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/summary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/tensor_description_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/tensor_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/tensor_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/types_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/variable_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/variable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/framework/versions_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/framework/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/cluster_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/config_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/data_service_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/data_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/debug_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/debug_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/saver_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/saver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/service_config_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/service_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/struct_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/struct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/util/event_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/util/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/core/util/test_log_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/core/util/test_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/data/__init__.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/data/experimental.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/data/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/dtypes.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/experimental/dtensor.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/experimental/dtensor.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/feature_column/__init__.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/feature_column/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/io/__init__.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/io/gfile.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/io/gfile.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/activations.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/activations.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/callbacks.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/callbacks.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/constraints.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/constraints.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/initializers.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/initializers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/layers/__init__.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/layers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/losses.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/losses.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,14 @@
     @classmethod
     def validate(cls, key: object) -> TypeGuard[_ReductionValues]: ...
 
 _ReductionValues: TypeAlias = Literal["auto", "none", "sum", "sum_over_batch_size"]
 
 def categorical_hinge(y_true: TensorCompatible, y_pred: TensorCompatible) -> Tensor: ...
 def huber(y_true: TensorCompatible, y_pred: TensorCompatible, delta: float = 1.0) -> Tensor: ...
-def log_cosh(y_true: TensorCompatible, y_pred: TensorCompatible) -> Tensor: ...
 def deserialize(name: str | dict[str, Any], custom_objects: dict[str, Any] | None = None) -> Loss: ...
 def serialize(loss: KerasSerializable) -> dict[str, Any]: ...
 
 _FuncT = TypeVar("_FuncT", bound=Callable[..., Any])
 
 @overload
 def get(identifier: None) -> None: ...
```

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/metrics.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/metrics.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/models.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/models.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/optimizers/schedules.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/optimizers/schedules.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/keras/regularizers.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/keras/regularizers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/linalg.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/linalg.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/math.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/math.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/nn.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/nn.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/feature_column/feature_column_v2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/feature_column/feature_column_v2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/random.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/random.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/raw_ops.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/raw_ops.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/saved_model/__init__.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/saved_model/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/saved_model/experimental.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/saved_model/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/sparse.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/sparse.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/strings.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/strings.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/summary.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/summary.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/train/__init__.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/train/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/status_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/tensorflow-stubs/types/experimental.pyi` & `types-tensorflow-2.16.0.20240428/tensorflow-stubs/types/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.16.0.20240424/types_tensorflow.egg-info/PKG-INFO` & `types-tensorflow-2.16.0.20240428/types_tensorflow.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.16.0.20240424
+Version: 2.16.0.20240428
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -34,10 +34,10 @@
 Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.16.1 .
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7ed91bc2e77ec18d28307dc6086a778ecc9c7bb3` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `bdf75023dfe3930deac1c6b4e269770427b106c4` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
```

### Comparing `types-tensorflow-2.16.0.20240424/types_tensorflow.egg-info/SOURCES.txt` & `types-tensorflow-2.16.0.20240428/types_tensorflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

