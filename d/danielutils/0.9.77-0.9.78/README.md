# Comparing `tmp/danielutils-0.9.77.tar.gz` & `tmp/danielutils-0.9.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.9.77.tar", last modified: Sat Apr 27 19:11:29 2024, max compression
+gzip compressed data, was "danielutils-0.9.78.tar", last modified: Sat Apr 27 19:12:25 2024, max compression
```

## Comparing `danielutils-0.9.77.tar` & `danielutils-0.9.78.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.469435 danielutils-0.9.77/
--rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.77/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-27 19:11:28.000000 danielutils-0.9.77/MANIFEST.in
--rw-rw-rw-   0        0        0     4593 2024-04-27 19:11:29.469435 danielutils-0.9.77/PKG-INFO
--rw-rw-rw-   0        0        0     2650 2024-04-27 19:11:15.000000 danielutils-0.9.77/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.356810 danielutils-0.9.77/danielutils/
--rw-rw-rw-   0        0        0     1364 2024-04-21 19:46:04.000000 danielutils-0.9.77/danielutils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.362027 danielutils-0.9.77/danielutils/abstractions/
--rw-rw-rw-   0        0        0       77 2024-04-21 19:46:54.000000 danielutils-0.9.77/danielutils/abstractions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.364377 danielutils-0.9.77/danielutils/abstractions/database/
--rw-rw-rw-   0        0        0       57 2024-04-21 18:12:14.000000 danielutils-0.9.77/danielutils/abstractions/database/__init__.py
--rw-rw-rw-   0        0        0     2772 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/abstractions/database/cached_database.py
--rw-rw-rw-   0        0        0     2616 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/abstractions/database/database.py
--rw-rw-rw-   0        0        0     1048 2024-04-25 20:10:37.000000 danielutils-0.9.77/danielutils/abstractions/database/redis_database.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.366375 danielutils-0.9.77/danielutils/abstractions/multiprogramming/
--rw-rw-rw-   0        0        0       74 2024-04-21 19:21:56.000000 danielutils-0.9.77/danielutils/abstractions/multiprogramming/__init__.py
--rw-rw-rw-   0        0        0      374 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/abstractions/multiprogramming/multi_id.py
--rw-rw-rw-   0        0        0     2398 2024-04-21 19:22:23.000000 danielutils-0.9.77/danielutils/abstractions/multiprogramming/worker.py
--rw-rw-rw-   0        0        0     2426 2024-04-21 19:22:35.000000 danielutils-0.9.77/danielutils/abstractions/multiprogramming/worker_pool.py
--rw-rw-rw-   0        0        0     3162 2024-04-21 18:24:30.000000 danielutils-0.9.77/danielutils/abstractions/repl.py
--rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/aliases.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.368377 danielutils-0.9.77/danielutils/better_builtins/
--rw-rw-rw-   0        0        0       78 2024-04-21 18:23:39.000000 danielutils-0.9.77/danielutils/better_builtins/__init__.py
--rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/better_builtins/counter.py
--rw-rw-rw-   0        0        0     7174 2024-04-21 18:12:40.000000 danielutils-0.9.77/danielutils/better_builtins/frange.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.372391 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/
--rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/__init__.py
--rw-rw-rw-   0        0        0     4730 2024-04-09 22:20:09.000000 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/factory.py
--rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/tdict.py
--rw-rw-rw-   0        0        0     7214 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/tlist.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/tset.py
--rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/better_builtins/typed_builtins/ttuple.py
--rw-rw-rw-   0        0        0     5457 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/colors.py
--rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/convenience.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.373793 danielutils-0.9.77/danielutils/conversions/
--rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/conversions/__init__.py
--rw-rw-rw-   0        0        0     2227 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/conversions/main_conversions.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.375797 danielutils-0.9.77/danielutils/conversions/specialized_conversions/
--rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/conversions/specialized_conversions/__init__.py
--rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.77/danielutils/conversions/specialized_conversions/to_hex.py
--rw-rw-rw-   0        0        0      549 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/conversions/specialized_conversions/to_int.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.378797 danielutils-0.9.77/danielutils/data_structures/
--rw-rw-rw-   0        0        0      163 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/comparer.py
--rw-rw-rw-   0        0        0      273 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/default_dict.py
--rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.77/danielutils/data_structures/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.383273 danielutils-0.9.77/danielutils/data_structures/graph/
--rw-rw-rw-   0        0        0       97 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/graph/__init__.py
--rw-rw-rw-   0        0        0     2066 2024-04-18 18:33:41.000000 danielutils-0.9.77/danielutils/data_structures/graph/binary_node.py
--rw-rw-rw-   0        0        0     6917 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/graph/graph.py
--rw-rw-rw-   0        0        0     3149 2024-04-18 18:55:16.000000 danielutils-0.9.77/danielutils/data_structures/graph/multinode.py
--rw-rw-rw-   0        0        0     1647 2024-03-28 19:42:06.000000 danielutils-0.9.77/danielutils/data_structures/graph/node.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.386278 danielutils-0.9.77/danielutils/data_structures/heap/
--rw-rw-rw-   0        0        0       71 2024-03-28 19:45:24.000000 danielutils-0.9.77/danielutils/data_structures/heap/__init__.py
--rw-rw-rw-   0        0        0     3092 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/heap/heap.py
--rw-rw-rw-   0        0        0      292 2024-03-28 19:45:24.000000 danielutils-0.9.77/danielutils/data_structures/heap/max_heap.py
--rw-rw-rw-   0        0        0      300 2024-03-28 19:45:24.000000 danielutils-0.9.77/danielutils/data_structures/heap/min_heap.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.389278 danielutils-0.9.77/danielutils/data_structures/queue/
--rw-rw-rw-   0        0        0       82 2024-03-28 19:35:07.000000 danielutils-0.9.77/danielutils/data_structures/queue/__init__.py
--rw-rw-rw-   0        0        0      260 2024-03-28 19:35:13.000000 danielutils-0.9.77/danielutils/data_structures/queue/atomic_queue.py
--rw-rw-rw-   0        0        0     3661 2024-03-28 19:35:07.000000 danielutils-0.9.77/danielutils/data_structures/queue/priority_queue.py
--rw-rw-rw-   0        0        0     1621 2024-03-29 00:18:38.000000 danielutils-0.9.77/danielutils/data_structures/queue/queue.py
--rw-rw-rw-   0        0        0     2143 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/stack.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.391782 danielutils-0.9.77/danielutils/data_structures/trees/
--rw-rw-rw-   0        0        0       63 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/data_structures/trees/__init__.py
--rw-rw-rw-   0        0        0     2644 2024-04-25 21:14:44.000000 danielutils-0.9.77/danielutils/data_structures/trees/binary_syntax_tree.py
--rw-rw-rw-   0        0        0     1618 2024-04-18 18:33:41.000000 danielutils-0.9.77/danielutils/data_structures/trees/binary_tree.py
--rw-rw-rw-   0        0        0      631 2023-09-25 13:20:33.000000 danielutils-0.9.77/danielutils/date.py
--rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.77/danielutils/date_time.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.404279 danielutils-0.9.77/danielutils/decorators/
--rw-rw-rw-   0        0        0      466 2024-04-25 20:44:13.000000 danielutils-0.9.77/danielutils/decorators/__init__.py
--rw-rw-rw-   0        0        0      741 2024-04-27 18:47:34.000000 danielutils-0.9.77/danielutils/decorators/atomic.py
--rw-rw-rw-   0        0        0     1370 2024-04-27 18:47:49.000000 danielutils-0.9.77/danielutils/decorators/attach.py
--rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/decorators/chain_decorators.py
--rw-rw-rw-   0        0        0     1074 2024-04-10 11:18:47.000000 danielutils-0.9.77/danielutils/decorators/decorate_conditionally.py
--rw-rw-rw-   0        0        0     1008 2024-04-27 18:49:37.000000 danielutils-0.9.77/danielutils/decorators/delay_call.py
--rw-rw-rw-   0        0        0     1290 2024-04-27 18:48:35.000000 danielutils-0.9.77/danielutils/decorators/deprecate.py
--rw-rw-rw-   0        0        0     1023 2024-04-25 20:44:13.000000 danielutils-0.9.77/danielutils/decorators/final.py
--rw-rw-rw-   0        0        0     1681 2024-04-27 18:48:02.000000 danielutils-0.9.77/danielutils/decorators/limit_recursion.py
--rw-rw-rw-   0        0        0      811 2024-04-27 18:48:25.000000 danielutils-0.9.77/danielutils/decorators/memo.py
--rw-rw-rw-   0        0        0     7571 2024-04-27 18:48:52.000000 danielutils-0.9.77/danielutils/decorators/overload.py
--rw-rw-rw-   0        0        0      822 2024-04-27 18:49:05.000000 danielutils-0.9.77/danielutils/decorators/partially_implemented.py
--rw-rw-rw-   0        0        0     1716 2024-04-21 19:46:04.000000 danielutils-0.9.77/danielutils/decorators/processify.py
--rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/decorators/property.py
--rw-rw-rw-   0        0        0      776 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/decorators/singleton.py
--rw-rw-rw-   0        0        0      729 2024-04-27 18:49:28.000000 danielutils-0.9.77/danielutils/decorators/threadify.py
--rw-rw-rw-   0        0        0     1983 2024-04-27 18:49:18.000000 danielutils-0.9.77/danielutils/decorators/timeout.py
--rw-rw-rw-   0        0        0     3741 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/decorators/total_ordering.py
--rw-rw-rw-   0        0        0     9541 2024-04-27 18:40:42.000000 danielutils-0.9.77/danielutils/decorators/validate.py
--rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.411203 danielutils-0.9.77/danielutils/functions/
--rw-rw-rw-   0        0        0      235 2024-04-21 19:19:56.000000 danielutils-0.9.77/danielutils/functions/__init__.py
--rw-rw-rw-   0        0        0     1097 2024-03-27 18:52:27.000000 danielutils-0.9.77/danielutils/functions/areoneof.py
--rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/functions/check_foreach.py
--rw-rw-rw-   0        0        0      791 2024-04-21 19:19:56.000000 danielutils-0.9.77/danielutils/functions/flatten.py
--rw-rw-rw-   0        0        0    10081 2024-04-27 18:52:54.000000 danielutils-0.9.77/danielutils/functions/isoftype.py
--rw-rw-rw-   0        0        0     1598 2024-03-27 18:52:27.000000 danielutils-0.9.77/danielutils/functions/isoneof.py
--rw-rw-rw-   0        0        0     1286 2024-04-21 19:19:56.000000 danielutils-0.9.77/danielutils/functions/multiloop.py
--rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/functions/powerset.py
--rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/functions/subseteq.py
--rw-rw-rw-   0        0        0     1016 2024-03-27 18:52:27.000000 danielutils-0.9.77/danielutils/functions/types_subseteq.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.414716 danielutils-0.9.77/danielutils/generators/
--rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/generators/__init__.py
--rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/generators/conditional_generator.py
--rw-rw-rw-   0        0        0      463 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/generators/generator_from_stream.py
--rw-rw-rw-   0        0        0     2869 2024-04-21 18:13:57.000000 danielutils-0.9.77/danielutils/generators/join_generators.py
--rw-rw-rw-   0        0        0     2051 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/internet.py
--rw-rw-rw-   0        0        0    12002 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/io_.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.417096 danielutils-0.9.77/danielutils/math_/
--rw-rw-rw-   0        0        0       79 2024-04-21 18:05:24.000000 danielutils-0.9.77/danielutils/math_/__init__.py
--rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/math_/constants.py
--rw-rw-rw-   0        0        0      627 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/math_/functions.py
--rw-rw-rw-   0        0        0     1063 2024-04-21 18:05:24.000000 danielutils-0.9.77/danielutils/math_/math_print.py
--rw-rw-rw-   0        0        0     4052 2024-04-21 18:05:24.000000 danielutils-0.9.77/danielutils/math_/math_symbols.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.419094 danielutils-0.9.77/danielutils/math_/polynomial/
--rw-rw-rw-   0        0        0       25 2024-04-21 18:05:24.000000 danielutils-0.9.77/danielutils/math_/polynomial/__init__.py
--rw-rw-rw-   0        0        0      849 2024-04-25 21:17:25.000000 danielutils-0.9.77/danielutils/math_/polynomial/polinomial.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.424070 danielutils-0.9.77/danielutils/metaclasses/
--rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.77/danielutils/metaclasses/__init__.py
--rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/metaclasses/atomic_class_meta.py
--rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/metaclasses/implicit_data_deleter_meta.py
--rw-rw-rw-   0        0        0     1495 2024-04-21 18:13:57.000000 danielutils-0.9.77/danielutils/metaclasses/instance_cache_meta.py
--rw-rw-rw-   0        0        0    10952 2024-04-21 18:13:57.000000 danielutils-0.9.77/danielutils/metaclasses/interface.py
--rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/metaclasses/overload_meta.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.426500 danielutils-0.9.77/danielutils/mock_/
--rw-rw-rw-   0        0        0       58 2024-04-21 18:12:14.000000 danielutils-0.9.77/danielutils/mock_/__init__.py
--rw-rw-rw-   0        0        0     2017 2024-04-21 19:46:04.000000 danielutils-0.9.77/danielutils/mock_/mock_database.py
--rw-rw-rw-   0        0        0      419 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/mock_/mock_module.py
--rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/path.py
--rw-rw-rw-   0        0        0     2801 2024-04-21 18:05:24.000000 danielutils-0.9.77/danielutils/print_.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.428878 danielutils-0.9.77/danielutils/protocols/
--rw-rw-rw-   0        0        0       49 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/protocols/__init__.py
--rw-rw-rw-   0        0        0      454 2024-04-25 21:16:46.000000 danielutils-0.9.77/danielutils/protocols/dictable.py
--rw-rw-rw-   0        0        0      203 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/protocols/evaluable.py
--rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.77/danielutils/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.428878 danielutils-0.9.77/danielutils/reflection/
--rw-rw-rw-   0        0        0     1516 2024-04-21 18:21:37.000000 danielutils-0.9.77/danielutils/reflection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.429885 danielutils-0.9.77/danielutils/reflection/class_/
--rw-rw-rw-   0        0        0       31 2024-04-21 18:21:37.000000 danielutils-0.9.77/danielutils/reflection/class_/__init__.py
--rw-rw-rw-   0        0        0     5529 2024-04-27 18:35:37.000000 danielutils-0.9.77/danielutils/reflection/class_/class_reflection.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.431391 danielutils-0.9.77/danielutils/reflection/file/
--rw-rw-rw-   0        0        0       30 2024-04-21 18:21:37.000000 danielutils-0.9.77/danielutils/reflection/file/__init__.py
--rw-rw-rw-   0        0        0     1657 2024-04-27 18:35:37.000000 danielutils-0.9.77/danielutils/reflection/file/file_reflection.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.433265 danielutils-0.9.77/danielutils/reflection/function/
--rw-rw-rw-   0        0        0       35 2024-04-21 18:21:37.000000 danielutils-0.9.77/danielutils/reflection/function/__init__.py
--rw-rw-rw-   0        0        0     4459 2024-04-21 18:24:01.000000 danielutils-0.9.77/danielutils/reflection/function/function_reflections.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.438928 danielutils-0.9.77/danielutils/reflection/interpreter/
--rw-rw-rw-   0        0        0      179 2024-04-21 19:19:56.000000 danielutils-0.9.77/danielutils/reflection/interpreter/__init__.py
--rw-rw-rw-   0        0        0     1074 2024-04-25 20:37:30.000000 danielutils-0.9.77/danielutils/reflection/interpreter/callstack.py
--rw-rw-rw-   0        0        0      447 2024-04-21 18:22:32.000000 danielutils-0.9.77/danielutils/reflection/interpreter/get_traceback.py
--rw-rw-rw-   0        0        0      622 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/reflection/interpreter/os_.py
--rw-rw-rw-   0        0        0     1023 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/reflection/interpreter/packages.py
--rw-rw-rw-   0        0        0      627 2024-03-29 21:49:46.000000 danielutils-0.9.77/danielutils/reflection/interpreter/python_version.py
--rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/reflection/interpreter/signals.py
--rw-rw-rw-   0        0        0     5745 2024-04-25 21:09:28.000000 danielutils-0.9.77/danielutils/reflection/interpreter/tracer.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.439926 danielutils-0.9.77/danielutils/reflection/module/
--rw-rw-rw-   0        0        0       68 2024-04-21 18:27:13.000000 danielutils-0.9.77/danielutils/reflection/module/__init__.py
--rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/reflection/module/module_reflections.py
--rw-rw-rw-   0        0        0     4742 2024-04-21 18:27:13.000000 danielutils-0.9.77/danielutils/reflection/module/package_reflection.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.441942 danielutils-0.9.77/danielutils/snippets/
--rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/snippets/__init__.py
--rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/snippets/try_get.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.443949 danielutils-0.9.77/danielutils/system/
--rw-rw-rw-   0        0        0       52 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/system/__init__.py
--rw-rw-rw-   0        0        0     6844 2024-03-27 18:52:27.000000 danielutils-0.9.77/danielutils/system/independent.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.445946 danielutils-0.9.77/danielutils/system/windows/
--rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/system/windows/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.447416 danielutils-0.9.77/danielutils/system/windows/utils/
--rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/system/windows/utils/__init__.py
--rw-rw-rw-   0        0        0      499 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/system/windows/utils/filetime.py
--rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/system/windows/win32_ctime.py
--rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/system/windows/windows.py
--rw-rw-rw-   0        0        0     4093 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/text.py
--rw-rw-rw-   0        0        0     1225 2024-04-27 18:53:17.000000 danielutils-0.9.77/danielutils/time.py
--rw-rw-rw-   0        0        0     1731 2024-04-25 20:10:37.000000 danielutils-0.9.77/danielutils/tqdm_.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.448884 danielutils-0.9.77/danielutils/university/
--rw-rw-rw-   0        0        0       74 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.449890 danielutils-0.9.77/danielutils/university/databases/
--rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/university/databases/__init__.py
--rw-rw-rw-   0        0        0    24942 2024-03-21 20:59:13.000000 danielutils-0.9.77/danielutils/university/databases/all.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.451394 danielutils-0.9.77/danielutils/university/oop/
--rw-rw-rw-   0        0        0       25 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/oop/__init__.py
--rw-rw-rw-   0        0        0      802 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/oop/observer.py
--rw-rw-rw-   0        0        0       87 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/oop/strategy.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.456002 danielutils-0.9.77/danielutils/university/probability/
--rw-rw-rw-   0        0        0      189 2024-04-21 22:41:40.000000 danielutils-0.9.77/danielutils/university/probability/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.457730 danielutils-0.9.77/danielutils/university/probability/conditional_variable/
--rw-rw-rw-   0        0        0       89 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/__init__.py
--rw-rw-rw-   0        0        0     4004 2024-04-25 21:21:07.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/conditional_variable.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.457730 danielutils-0.9.77/danielutils/university/probability/conditional_variable/continuous/
--rw-rw-rw-   0        0        0        0 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/continuous/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.463436 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/
--rw-rw-rw-   0        0        0      209 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/__init__.py
--rw-rw-rw-   0        0        0     1149 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/bernoulli.py
--rw-rw-rw-   0        0        0     1257 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/binomial.py
--rw-rw-rw-   0        0        0     1108 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py
--rw-rw-rw-   0        0        0     1370 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/discrete.py
--rw-rw-rw-   0        0        0     1658 2024-04-25 21:22:17.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/geometric.py
--rw-rw-rw-   0        0        0      992 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/poisson.py
--rw-rw-rw-   0        0        0     1040 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/uniform.py
--rw-rw-rw-   0        0        0      904 2024-04-21 22:41:40.000000 danielutils-0.9.77/danielutils/university/probability/distributions.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.465435 danielutils-0.9.77/danielutils/university/probability/expressions/
--rw-rw-rw-   0        0        0       79 2024-04-17 22:49:00.000000 danielutils-0.9.77/danielutils/university/probability/expressions/__init__.py
--rw-rw-rw-   0        0        0     7439 2024-04-25 21:20:42.000000 danielutils-0.9.77/danielutils/university/probability/expressions/accumulation_expression.py
--rw-rw-rw-   0        0        0     4391 2024-04-25 21:20:53.000000 danielutils-0.9.77/danielutils/university/probability/expressions/probability_expression.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.468436 danielutils-0.9.77/danielutils/university/probability/funcs/
--rw-rw-rw-   0        0        0      120 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/probability/funcs/__init__.py
--rw-rw-rw-   0        0        0      338 2024-04-21 22:41:40.000000 danielutils-0.9.77/danielutils/university/probability/funcs/covariance.py
--rw-rw-rw-   0        0        0     1173 2024-04-21 22:41:40.000000 danielutils-0.9.77/danielutils/university/probability/funcs/expected_value.py
--rw-rw-rw-   0        0        0      306 2024-04-17 20:37:10.000000 danielutils-0.9.77/danielutils/university/probability/funcs/probability_function.py
--rw-rw-rw-   0        0        0      437 2024-04-21 22:41:40.000000 danielutils-0.9.77/danielutils/university/probability/funcs/variance.py
--rw-rw-rw-   0        0        0     2005 2024-04-25 21:18:16.000000 danielutils-0.9.77/danielutils/university/probability/operator.py
--rw-rw-rw-   0        0        0      641 2024-04-18 18:33:41.000000 danielutils-0.9.77/danielutils/university/probability/protocols.py
--rw-rw-rw-   0        0        0     2055 2024-04-21 22:51:43.000000 danielutils-0.9.77/danielutils/university/probability/supp.py
--rw-rw-rw-   0        0        0     1182 2024-04-25 20:08:45.000000 danielutils-0.9.77/danielutils/university/probability/transformation.py
--rw-rw-rw-   0        0        0      605 2024-04-27 18:47:16.000000 danielutils-0.9.77/danielutils/versioned_imports.py
-drwxrwxrwx   0        0        0        0 2024-04-27 19:11:29.360487 danielutils-0.9.77/danielutils.egg-info/
--rw-rw-rw-   0        0        0     4593 2024-04-27 19:11:29.000000 danielutils-0.9.77/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7689 2024-04-27 19:11:29.000000 danielutils-0.9.77/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 19:11:29.000000 danielutils-0.9.77/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-27 19:11:29.000000 danielutils-0.9.77/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      977 2024-04-27 19:11:28.000000 danielutils-0.9.77/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 19:11:29.469435 danielutils-0.9.77/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-27 19:11:28.000000 danielutils-0.9.77/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.750002 danielutils-0.9.78/
+-rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.78/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-27 19:12:25.000000 danielutils-0.9.78/MANIFEST.in
+-rw-rw-rw-   0        0        0     4593 2024-04-27 19:12:25.750002 danielutils-0.9.78/PKG-INFO
+-rw-rw-rw-   0        0        0     2650 2024-04-27 19:12:24.000000 danielutils-0.9.78/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.654482 danielutils-0.9.78/danielutils/
+-rw-rw-rw-   0        0        0     1364 2024-04-21 19:46:04.000000 danielutils-0.9.78/danielutils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.658163 danielutils-0.9.78/danielutils/abstractions/
+-rw-rw-rw-   0        0        0       77 2024-04-21 19:46:54.000000 danielutils-0.9.78/danielutils/abstractions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.660163 danielutils-0.9.78/danielutils/abstractions/database/
+-rw-rw-rw-   0        0        0       57 2024-04-21 18:12:14.000000 danielutils-0.9.78/danielutils/abstractions/database/__init__.py
+-rw-rw-rw-   0        0        0     2772 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/abstractions/database/cached_database.py
+-rw-rw-rw-   0        0        0     2616 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/abstractions/database/database.py
+-rw-rw-rw-   0        0        0     1048 2024-04-25 20:10:37.000000 danielutils-0.9.78/danielutils/abstractions/database/redis_database.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.662163 danielutils-0.9.78/danielutils/abstractions/multiprogramming/
+-rw-rw-rw-   0        0        0       74 2024-04-21 19:21:56.000000 danielutils-0.9.78/danielutils/abstractions/multiprogramming/__init__.py
+-rw-rw-rw-   0        0        0      374 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/abstractions/multiprogramming/multi_id.py
+-rw-rw-rw-   0        0        0     2398 2024-04-21 19:22:23.000000 danielutils-0.9.78/danielutils/abstractions/multiprogramming/worker.py
+-rw-rw-rw-   0        0        0     2426 2024-04-21 19:22:35.000000 danielutils-0.9.78/danielutils/abstractions/multiprogramming/worker_pool.py
+-rw-rw-rw-   0        0        0     3162 2024-04-21 18:24:30.000000 danielutils-0.9.78/danielutils/abstractions/repl.py
+-rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/aliases.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.664163 danielutils-0.9.78/danielutils/better_builtins/
+-rw-rw-rw-   0        0        0       78 2024-04-21 18:23:39.000000 danielutils-0.9.78/danielutils/better_builtins/__init__.py
+-rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/better_builtins/counter.py
+-rw-rw-rw-   0        0        0     7174 2024-04-21 18:12:40.000000 danielutils-0.9.78/danielutils/better_builtins/frange.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.668434 danielutils-0.9.78/danielutils/better_builtins/typed_builtins/
+-rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/better_builtins/typed_builtins/__init__.py
+-rw-rw-rw-   0        0        0     4730 2024-04-09 22:20:09.000000 danielutils-0.9.78/danielutils/better_builtins/typed_builtins/factory.py
+-rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/better_builtins/typed_builtins/tdict.py
+-rw-rw-rw-   0        0        0     7214 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/better_builtins/typed_builtins/tlist.py
+-rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/better_builtins/typed_builtins/tset.py
+-rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/better_builtins/typed_builtins/ttuple.py
+-rw-rw-rw-   0        0        0     5457 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/colors.py
+-rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/convenience.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.669440 danielutils-0.9.78/danielutils/conversions/
+-rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/conversions/__init__.py
+-rw-rw-rw-   0        0        0     2227 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/conversions/main_conversions.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.670441 danielutils-0.9.78/danielutils/conversions/specialized_conversions/
+-rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/conversions/specialized_conversions/__init__.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.78/danielutils/conversions/specialized_conversions/to_hex.py
+-rw-rw-rw-   0        0        0      549 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/conversions/specialized_conversions/to_int.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.674160 danielutils-0.9.78/danielutils/data_structures/
+-rw-rw-rw-   0        0        0      163 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/data_structures/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/data_structures/comparer.py
+-rw-rw-rw-   0        0        0      273 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/data_structures/default_dict.py
+-rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.78/danielutils/data_structures/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.676545 danielutils-0.9.78/danielutils/data_structures/graph/
+-rw-rw-rw-   0        0        0       97 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/data_structures/graph/__init__.py
+-rw-rw-rw-   0        0        0     2066 2024-04-18 18:33:41.000000 danielutils-0.9.78/danielutils/data_structures/graph/binary_node.py
+-rw-rw-rw-   0        0        0     6917 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/data_structures/graph/graph.py
+-rw-rw-rw-   0        0        0     3149 2024-04-18 18:55:16.000000 danielutils-0.9.78/danielutils/data_structures/graph/multinode.py
+-rw-rw-rw-   0        0        0     1647 2024-03-28 19:42:06.000000 danielutils-0.9.78/danielutils/data_structures/graph/node.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.678581 danielutils-0.9.78/danielutils/data_structures/heap/
+-rw-rw-rw-   0        0        0       71 2024-03-28 19:45:24.000000 danielutils-0.9.78/danielutils/data_structures/heap/__init__.py
+-rw-rw-rw-   0        0        0     3092 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/data_structures/heap/heap.py
+-rw-rw-rw-   0        0        0      292 2024-03-28 19:45:24.000000 danielutils-0.9.78/danielutils/data_structures/heap/max_heap.py
+-rw-rw-rw-   0        0        0      300 2024-03-28 19:45:24.000000 danielutils-0.9.78/danielutils/data_structures/heap/min_heap.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.680580 danielutils-0.9.78/danielutils/data_structures/queue/
+-rw-rw-rw-   0        0        0       82 2024-03-28 19:35:07.000000 danielutils-0.9.78/danielutils/data_structures/queue/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-03-28 19:35:13.000000 danielutils-0.9.78/danielutils/data_structures/queue/atomic_queue.py
+-rw-rw-rw-   0        0        0     3661 2024-03-28 19:35:07.000000 danielutils-0.9.78/danielutils/data_structures/queue/priority_queue.py
+-rw-rw-rw-   0        0        0     1621 2024-03-29 00:18:38.000000 danielutils-0.9.78/danielutils/data_structures/queue/queue.py
+-rw-rw-rw-   0        0        0     2143 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/data_structures/stack.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.683131 danielutils-0.9.78/danielutils/data_structures/trees/
+-rw-rw-rw-   0        0        0       63 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/data_structures/trees/__init__.py
+-rw-rw-rw-   0        0        0     2644 2024-04-25 21:14:44.000000 danielutils-0.9.78/danielutils/data_structures/trees/binary_syntax_tree.py
+-rw-rw-rw-   0        0        0     1618 2024-04-18 18:33:41.000000 danielutils-0.9.78/danielutils/data_structures/trees/binary_tree.py
+-rw-rw-rw-   0        0        0      631 2023-09-25 13:20:33.000000 danielutils-0.9.78/danielutils/date.py
+-rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.78/danielutils/date_time.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.694275 danielutils-0.9.78/danielutils/decorators/
+-rw-rw-rw-   0        0        0      466 2024-04-25 20:44:13.000000 danielutils-0.9.78/danielutils/decorators/__init__.py
+-rw-rw-rw-   0        0        0      741 2024-04-27 18:47:34.000000 danielutils-0.9.78/danielutils/decorators/atomic.py
+-rw-rw-rw-   0        0        0     1370 2024-04-27 18:47:49.000000 danielutils-0.9.78/danielutils/decorators/attach.py
+-rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/decorators/chain_decorators.py
+-rw-rw-rw-   0        0        0     1074 2024-04-10 11:18:47.000000 danielutils-0.9.78/danielutils/decorators/decorate_conditionally.py
+-rw-rw-rw-   0        0        0     1008 2024-04-27 18:49:37.000000 danielutils-0.9.78/danielutils/decorators/delay_call.py
+-rw-rw-rw-   0        0        0     1290 2024-04-27 18:48:35.000000 danielutils-0.9.78/danielutils/decorators/deprecate.py
+-rw-rw-rw-   0        0        0     1023 2024-04-25 20:44:13.000000 danielutils-0.9.78/danielutils/decorators/final.py
+-rw-rw-rw-   0        0        0     1681 2024-04-27 18:48:02.000000 danielutils-0.9.78/danielutils/decorators/limit_recursion.py
+-rw-rw-rw-   0        0        0      811 2024-04-27 18:48:25.000000 danielutils-0.9.78/danielutils/decorators/memo.py
+-rw-rw-rw-   0        0        0     7571 2024-04-27 18:48:52.000000 danielutils-0.9.78/danielutils/decorators/overload.py
+-rw-rw-rw-   0        0        0      822 2024-04-27 18:49:05.000000 danielutils-0.9.78/danielutils/decorators/partially_implemented.py
+-rw-rw-rw-   0        0        0     1716 2024-04-21 19:46:04.000000 danielutils-0.9.78/danielutils/decorators/processify.py
+-rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/decorators/property.py
+-rw-rw-rw-   0        0        0      776 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/decorators/singleton.py
+-rw-rw-rw-   0        0        0      729 2024-04-27 18:49:28.000000 danielutils-0.9.78/danielutils/decorators/threadify.py
+-rw-rw-rw-   0        0        0     1983 2024-04-27 18:49:18.000000 danielutils-0.9.78/danielutils/decorators/timeout.py
+-rw-rw-rw-   0        0        0     3741 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/decorators/total_ordering.py
+-rw-rw-rw-   0        0        0     9541 2024-04-27 18:40:42.000000 danielutils-0.9.78/danielutils/decorators/validate.py
+-rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.699780 danielutils-0.9.78/danielutils/functions/
+-rw-rw-rw-   0        0        0      235 2024-04-21 19:19:56.000000 danielutils-0.9.78/danielutils/functions/__init__.py
+-rw-rw-rw-   0        0        0     1097 2024-03-27 18:52:27.000000 danielutils-0.9.78/danielutils/functions/areoneof.py
+-rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/functions/check_foreach.py
+-rw-rw-rw-   0        0        0      791 2024-04-21 19:19:56.000000 danielutils-0.9.78/danielutils/functions/flatten.py
+-rw-rw-rw-   0        0        0    10081 2024-04-27 18:52:54.000000 danielutils-0.9.78/danielutils/functions/isoftype.py
+-rw-rw-rw-   0        0        0     1598 2024-03-27 18:52:27.000000 danielutils-0.9.78/danielutils/functions/isoneof.py
+-rw-rw-rw-   0        0        0     1286 2024-04-21 19:19:56.000000 danielutils-0.9.78/danielutils/functions/multiloop.py
+-rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/functions/powerset.py
+-rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/functions/subseteq.py
+-rw-rw-rw-   0        0        0     1016 2024-03-27 18:52:27.000000 danielutils-0.9.78/danielutils/functions/types_subseteq.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.702290 danielutils-0.9.78/danielutils/generators/
+-rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/generators/__init__.py
+-rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/generators/conditional_generator.py
+-rw-rw-rw-   0        0        0      463 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/generators/generator_from_stream.py
+-rw-rw-rw-   0        0        0     2869 2024-04-21 18:13:57.000000 danielutils-0.9.78/danielutils/generators/join_generators.py
+-rw-rw-rw-   0        0        0     2051 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/internet.py
+-rw-rw-rw-   0        0        0    12002 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/io_.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.705185 danielutils-0.9.78/danielutils/math_/
+-rw-rw-rw-   0        0        0       79 2024-04-21 18:05:24.000000 danielutils-0.9.78/danielutils/math_/__init__.py
+-rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/math_/constants.py
+-rw-rw-rw-   0        0        0      627 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/math_/functions.py
+-rw-rw-rw-   0        0        0     1063 2024-04-21 18:05:24.000000 danielutils-0.9.78/danielutils/math_/math_print.py
+-rw-rw-rw-   0        0        0     4052 2024-04-21 18:05:24.000000 danielutils-0.9.78/danielutils/math_/math_symbols.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.706222 danielutils-0.9.78/danielutils/math_/polynomial/
+-rw-rw-rw-   0        0        0       25 2024-04-21 18:05:24.000000 danielutils-0.9.78/danielutils/math_/polynomial/__init__.py
+-rw-rw-rw-   0        0        0      849 2024-04-25 21:17:25.000000 danielutils-0.9.78/danielutils/math_/polynomial/polinomial.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.709864 danielutils-0.9.78/danielutils/metaclasses/
+-rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.78/danielutils/metaclasses/__init__.py
+-rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/metaclasses/atomic_class_meta.py
+-rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/metaclasses/implicit_data_deleter_meta.py
+-rw-rw-rw-   0        0        0     1495 2024-04-21 18:13:57.000000 danielutils-0.9.78/danielutils/metaclasses/instance_cache_meta.py
+-rw-rw-rw-   0        0        0    10952 2024-04-21 18:13:57.000000 danielutils-0.9.78/danielutils/metaclasses/interface.py
+-rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/metaclasses/overload_meta.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.710863 danielutils-0.9.78/danielutils/mock_/
+-rw-rw-rw-   0        0        0       58 2024-04-21 18:12:14.000000 danielutils-0.9.78/danielutils/mock_/__init__.py
+-rw-rw-rw-   0        0        0     2017 2024-04-21 19:46:04.000000 danielutils-0.9.78/danielutils/mock_/mock_database.py
+-rw-rw-rw-   0        0        0      419 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/mock_/mock_module.py
+-rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/path.py
+-rw-rw-rw-   0        0        0     2801 2024-04-21 18:05:24.000000 danielutils-0.9.78/danielutils/print_.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.713405 danielutils-0.9.78/danielutils/protocols/
+-rw-rw-rw-   0        0        0       49 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/protocols/__init__.py
+-rw-rw-rw-   0        0        0      454 2024-04-25 21:16:46.000000 danielutils-0.9.78/danielutils/protocols/dictable.py
+-rw-rw-rw-   0        0        0      203 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/protocols/evaluable.py
+-rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.78/danielutils/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.714286 danielutils-0.9.78/danielutils/reflection/
+-rw-rw-rw-   0        0        0     1516 2024-04-21 18:21:37.000000 danielutils-0.9.78/danielutils/reflection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.715317 danielutils-0.9.78/danielutils/reflection/class_/
+-rw-rw-rw-   0        0        0       31 2024-04-21 18:21:37.000000 danielutils-0.9.78/danielutils/reflection/class_/__init__.py
+-rw-rw-rw-   0        0        0     5529 2024-04-27 18:35:37.000000 danielutils-0.9.78/danielutils/reflection/class_/class_reflection.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.716315 danielutils-0.9.78/danielutils/reflection/file/
+-rw-rw-rw-   0        0        0       30 2024-04-21 18:21:37.000000 danielutils-0.9.78/danielutils/reflection/file/__init__.py
+-rw-rw-rw-   0        0        0     1657 2024-04-27 18:35:37.000000 danielutils-0.9.78/danielutils/reflection/file/file_reflection.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.717358 danielutils-0.9.78/danielutils/reflection/function/
+-rw-rw-rw-   0        0        0       35 2024-04-21 18:21:37.000000 danielutils-0.9.78/danielutils/reflection/function/__init__.py
+-rw-rw-rw-   0        0        0     4459 2024-04-21 18:24:01.000000 danielutils-0.9.78/danielutils/reflection/function/function_reflections.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.722380 danielutils-0.9.78/danielutils/reflection/interpreter/
+-rw-rw-rw-   0        0        0      179 2024-04-21 19:19:56.000000 danielutils-0.9.78/danielutils/reflection/interpreter/__init__.py
+-rw-rw-rw-   0        0        0     1074 2024-04-25 20:37:30.000000 danielutils-0.9.78/danielutils/reflection/interpreter/callstack.py
+-rw-rw-rw-   0        0        0      447 2024-04-21 18:22:32.000000 danielutils-0.9.78/danielutils/reflection/interpreter/get_traceback.py
+-rw-rw-rw-   0        0        0      622 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/reflection/interpreter/os_.py
+-rw-rw-rw-   0        0        0     1023 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/reflection/interpreter/packages.py
+-rw-rw-rw-   0        0        0      627 2024-03-29 21:49:46.000000 danielutils-0.9.78/danielutils/reflection/interpreter/python_version.py
+-rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/reflection/interpreter/signals.py
+-rw-rw-rw-   0        0        0     5745 2024-04-25 21:09:28.000000 danielutils-0.9.78/danielutils/reflection/interpreter/tracer.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.723442 danielutils-0.9.78/danielutils/reflection/module/
+-rw-rw-rw-   0        0        0       68 2024-04-21 18:27:13.000000 danielutils-0.9.78/danielutils/reflection/module/__init__.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/reflection/module/module_reflections.py
+-rw-rw-rw-   0        0        0     4742 2024-04-21 18:27:13.000000 danielutils-0.9.78/danielutils/reflection/module/package_reflection.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.725641 danielutils-0.9.78/danielutils/snippets/
+-rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/snippets/__init__.py
+-rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/snippets/try_get.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.726642 danielutils-0.9.78/danielutils/system/
+-rw-rw-rw-   0        0        0       52 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/system/__init__.py
+-rw-rw-rw-   0        0        0     6844 2024-03-27 18:52:27.000000 danielutils-0.9.78/danielutils/system/independent.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.728686 danielutils-0.9.78/danielutils/system/windows/
+-rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/system/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.729685 danielutils-0.9.78/danielutils/system/windows/utils/
+-rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/system/windows/utils/__init__.py
+-rw-rw-rw-   0        0        0      499 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/system/windows/utils/filetime.py
+-rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/system/windows/win32_ctime.py
+-rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/system/windows/windows.py
+-rw-rw-rw-   0        0        0     4093 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/text.py
+-rw-rw-rw-   0        0        0     1225 2024-04-27 18:53:17.000000 danielutils-0.9.78/danielutils/time.py
+-rw-rw-rw-   0        0        0     1731 2024-04-25 20:10:37.000000 danielutils-0.9.78/danielutils/tqdm_.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.730494 danielutils-0.9.78/danielutils/university/
+-rw-rw-rw-   0        0        0       74 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/university/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.731500 danielutils-0.9.78/danielutils/university/databases/
+-rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/university/databases/__init__.py
+-rw-rw-rw-   0        0        0    24942 2024-03-21 20:59:13.000000 danielutils-0.9.78/danielutils/university/databases/all.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.732500 danielutils-0.9.78/danielutils/university/oop/
+-rw-rw-rw-   0        0        0       25 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/university/oop/__init__.py
+-rw-rw-rw-   0        0        0      802 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/university/oop/observer.py
+-rw-rw-rw-   0        0        0       87 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/university/oop/strategy.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.737070 danielutils-0.9.78/danielutils/university/probability/
+-rw-rw-rw-   0        0        0      189 2024-04-21 22:41:40.000000 danielutils-0.9.78/danielutils/university/probability/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.738070 danielutils-0.9.78/danielutils/university/probability/conditional_variable/
+-rw-rw-rw-   0        0        0       89 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/university/probability/conditional_variable/__init__.py
+-rw-rw-rw-   0        0        0     4004 2024-04-25 21:21:07.000000 danielutils-0.9.78/danielutils/university/probability/conditional_variable/conditional_variable.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.739117 danielutils-0.9.78/danielutils/university/probability/conditional_variable/continuous/
+-rw-rw-rw-   0        0        0        0 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/university/probability/conditional_variable/continuous/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.744020 danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/
+-rw-rw-rw-   0        0        0      209 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/__init__.py
+-rw-rw-rw-   0        0        0     1149 2024-04-21 22:51:43.000000 danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/bernoulli.py
+-rw-rw-rw-   0        0        0     1257 2024-04-21 22:51:43.000000 danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/binomial.py
+-rw-rw-rw-   0        0        0     1108 2024-04-21 22:51:43.000000 danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py
+-rw-rw-rw-   0        0        0     1370 2024-04-21 22:51:43.000000 danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/discrete.py
+-rw-rw-rw-   0        0        0     1658 2024-04-25 21:22:17.000000 danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/geometric.py
+-rw-rw-rw-   0        0        0      992 2024-04-21 22:51:43.000000 danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/poisson.py
+-rw-rw-rw-   0        0        0     1040 2024-04-21 22:51:43.000000 danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/uniform.py
+-rw-rw-rw-   0        0        0      904 2024-04-21 22:41:40.000000 danielutils-0.9.78/danielutils/university/probability/distributions.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.746417 danielutils-0.9.78/danielutils/university/probability/expressions/
+-rw-rw-rw-   0        0        0       79 2024-04-17 22:49:00.000000 danielutils-0.9.78/danielutils/university/probability/expressions/__init__.py
+-rw-rw-rw-   0        0        0     7439 2024-04-25 21:20:42.000000 danielutils-0.9.78/danielutils/university/probability/expressions/accumulation_expression.py
+-rw-rw-rw-   0        0        0     4391 2024-04-25 21:20:53.000000 danielutils-0.9.78/danielutils/university/probability/expressions/probability_expression.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.748995 danielutils-0.9.78/danielutils/university/probability/funcs/
+-rw-rw-rw-   0        0        0      120 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/university/probability/funcs/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-04-21 22:41:40.000000 danielutils-0.9.78/danielutils/university/probability/funcs/covariance.py
+-rw-rw-rw-   0        0        0     1173 2024-04-21 22:41:40.000000 danielutils-0.9.78/danielutils/university/probability/funcs/expected_value.py
+-rw-rw-rw-   0        0        0      306 2024-04-17 20:37:10.000000 danielutils-0.9.78/danielutils/university/probability/funcs/probability_function.py
+-rw-rw-rw-   0        0        0      437 2024-04-21 22:41:40.000000 danielutils-0.9.78/danielutils/university/probability/funcs/variance.py
+-rw-rw-rw-   0        0        0     2005 2024-04-25 21:18:16.000000 danielutils-0.9.78/danielutils/university/probability/operator.py
+-rw-rw-rw-   0        0        0      641 2024-04-18 18:33:41.000000 danielutils-0.9.78/danielutils/university/probability/protocols.py
+-rw-rw-rw-   0        0        0     2055 2024-04-21 22:51:43.000000 danielutils-0.9.78/danielutils/university/probability/supp.py
+-rw-rw-rw-   0        0        0     1182 2024-04-25 20:08:45.000000 danielutils-0.9.78/danielutils/university/probability/transformation.py
+-rw-rw-rw-   0        0        0      605 2024-04-27 18:47:16.000000 danielutils-0.9.78/danielutils/versioned_imports.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:12:25.657157 danielutils-0.9.78/danielutils.egg-info/
+-rw-rw-rw-   0        0        0     4593 2024-04-27 19:12:25.000000 danielutils-0.9.78/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7689 2024-04-27 19:12:25.000000 danielutils-0.9.78/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 19:12:25.000000 danielutils-0.9.78/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-27 19:12:25.000000 danielutils-0.9.78/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      977 2024-04-27 19:12:25.000000 danielutils-0.9.78/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 19:12:25.751002 danielutils-0.9.78/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-27 19:12:25.000000 danielutils-0.9.78/setup.py
```

### Comparing `danielutils-0.9.77/LICENSE` & `danielutils-0.9.78/LICENSE`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/PKG-INFO` & `danielutils-0.9.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.77
+Version: 0.9.78
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,15 +37,15 @@
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.75
+# danielutils v=0.9.78
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 **Tested python versions**: `3.8.0`*, `3.9.0`, `3.10.13`
```

### Comparing `danielutils-0.9.77/README.md` & `danielutils-0.9.78/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.75
+# danielutils v=0.9.78
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 **Tested python versions**: `3.8.0`*, `3.9.0`, `3.10.13`
```

### Comparing `danielutils-0.9.77/danielutils/__init__.py` & `danielutils-0.9.78/danielutils/__init__.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/abstractions/database/cached_database.py` & `danielutils-0.9.78/danielutils/abstractions/database/cached_database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/abstractions/database/database.py` & `danielutils-0.9.78/danielutils/abstractions/database/database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/abstractions/database/redis_database.py` & `danielutils-0.9.78/danielutils/abstractions/database/redis_database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/abstractions/multiprogramming/worker.py` & `danielutils-0.9.78/danielutils/abstractions/multiprogramming/worker.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/abstractions/multiprogramming/worker_pool.py` & `danielutils-0.9.78/danielutils/abstractions/multiprogramming/worker_pool.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/abstractions/repl.py` & `danielutils-0.9.78/danielutils/abstractions/repl.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/aliases.py` & `danielutils-0.9.78/danielutils/aliases.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/better_builtins/counter.py` & `danielutils-0.9.78/danielutils/better_builtins/counter.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/better_builtins/frange.py` & `danielutils-0.9.78/danielutils/better_builtins/frange.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/better_builtins/typed_builtins/factory.py` & `danielutils-0.9.78/danielutils/better_builtins/typed_builtins/factory.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/better_builtins/typed_builtins/tdict.py` & `danielutils-0.9.78/danielutils/better_builtins/typed_builtins/tdict.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/better_builtins/typed_builtins/tlist.py` & `danielutils-0.9.78/danielutils/better_builtins/typed_builtins/tlist.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/better_builtins/typed_builtins/tset.py` & `danielutils-0.9.78/danielutils/better_builtins/typed_builtins/tset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/colors.py` & `danielutils-0.9.78/danielutils/colors.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/conversions/main_conversions.py` & `danielutils-0.9.78/danielutils/conversions/main_conversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/conversions/specialized_conversions/to_int.py` & `danielutils-0.9.78/danielutils/conversions/specialized_conversions/to_int.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/data_structures/comparer.py` & `danielutils-0.9.78/danielutils/data_structures/comparer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/data_structures/functions.py` & `danielutils-0.9.78/danielutils/data_structures/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/data_structures/graph/binary_node.py` & `danielutils-0.9.78/danielutils/data_structures/graph/binary_node.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/data_structures/graph/graph.py` & `danielutils-0.9.78/danielutils/data_structures/graph/graph.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/data_structures/graph/multinode.py` & `danielutils-0.9.78/danielutils/data_structures/graph/multinode.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/data_structures/graph/node.py` & `danielutils-0.9.78/danielutils/data_structures/graph/node.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/data_structures/heap/heap.py` & `danielutils-0.9.78/danielutils/data_structures/heap/heap.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/data_structures/queue/priority_queue.py` & `danielutils-0.9.78/danielutils/data_structures/queue/priority_queue.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/data_structures/queue/queue.py` & `danielutils-0.9.78/danielutils/data_structures/queue/queue.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/data_structures/stack.py` & `danielutils-0.9.78/danielutils/data_structures/stack.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/data_structures/trees/binary_syntax_tree.py` & `danielutils-0.9.78/danielutils/data_structures/trees/binary_syntax_tree.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/data_structures/trees/binary_tree.py` & `danielutils-0.9.78/danielutils/data_structures/trees/binary_tree.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/date.py` & `danielutils-0.9.78/danielutils/date.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/atomic.py` & `danielutils-0.9.78/danielutils/decorators/atomic.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/attach.py` & `danielutils-0.9.78/danielutils/decorators/attach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/chain_decorators.py` & `danielutils-0.9.78/danielutils/decorators/chain_decorators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/decorate_conditionally.py` & `danielutils-0.9.78/danielutils/decorators/decorate_conditionally.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/delay_call.py` & `danielutils-0.9.78/danielutils/decorators/delay_call.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/deprecate.py` & `danielutils-0.9.78/danielutils/decorators/deprecate.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/final.py` & `danielutils-0.9.78/danielutils/decorators/final.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/limit_recursion.py` & `danielutils-0.9.78/danielutils/decorators/limit_recursion.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/memo.py` & `danielutils-0.9.78/danielutils/decorators/memo.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/overload.py` & `danielutils-0.9.78/danielutils/decorators/overload.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/partially_implemented.py` & `danielutils-0.9.78/danielutils/decorators/partially_implemented.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/processify.py` & `danielutils-0.9.78/danielutils/decorators/processify.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/property.py` & `danielutils-0.9.78/danielutils/decorators/property.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/singleton.py` & `danielutils-0.9.78/danielutils/decorators/singleton.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/threadify.py` & `danielutils-0.9.78/danielutils/decorators/threadify.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/timeout.py` & `danielutils-0.9.78/danielutils/decorators/timeout.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/total_ordering.py` & `danielutils-0.9.78/danielutils/decorators/total_ordering.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/decorators/validate.py` & `danielutils-0.9.78/danielutils/decorators/validate.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/exceptions.py` & `danielutils-0.9.78/danielutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/functions/areoneof.py` & `danielutils-0.9.78/danielutils/functions/areoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/functions/check_foreach.py` & `danielutils-0.9.78/danielutils/functions/check_foreach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/functions/flatten.py` & `danielutils-0.9.78/danielutils/functions/flatten.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/functions/isoftype.py` & `danielutils-0.9.78/danielutils/functions/isoftype.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/functions/isoneof.py` & `danielutils-0.9.78/danielutils/functions/isoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/functions/multiloop.py` & `danielutils-0.9.78/danielutils/functions/multiloop.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/functions/powerset.py` & `danielutils-0.9.78/danielutils/functions/powerset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/functions/types_subseteq.py` & `danielutils-0.9.78/danielutils/functions/types_subseteq.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/generators/conditional_generator.py` & `danielutils-0.9.78/danielutils/generators/conditional_generator.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/generators/join_generators.py` & `danielutils-0.9.78/danielutils/generators/join_generators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/internet.py` & `danielutils-0.9.78/danielutils/internet.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/io_.py` & `danielutils-0.9.78/danielutils/io_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/math_/constants.py` & `danielutils-0.9.78/danielutils/math_/constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/math_/functions.py` & `danielutils-0.9.78/danielutils/math_/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/math_/math_print.py` & `danielutils-0.9.78/danielutils/math_/math_print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/math_/math_symbols.py` & `danielutils-0.9.78/danielutils/math_/math_symbols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/math_/polynomial/polinomial.py` & `danielutils-0.9.78/danielutils/math_/polynomial/polinomial.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/metaclasses/atomic_class_meta.py` & `danielutils-0.9.78/danielutils/metaclasses/atomic_class_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/metaclasses/implicit_data_deleter_meta.py` & `danielutils-0.9.78/danielutils/metaclasses/implicit_data_deleter_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/metaclasses/instance_cache_meta.py` & `danielutils-0.9.78/danielutils/metaclasses/instance_cache_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/metaclasses/interface.py` & `danielutils-0.9.78/danielutils/metaclasses/interface.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/metaclasses/overload_meta.py` & `danielutils-0.9.78/danielutils/metaclasses/overload_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/mock_/mock_database.py` & `danielutils-0.9.78/danielutils/mock_/mock_database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/path.py` & `danielutils-0.9.78/danielutils/path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/print_.py` & `danielutils-0.9.78/danielutils/print_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/reflection/__init__.py` & `danielutils-0.9.78/danielutils/reflection/__init__.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/reflection/class_/class_reflection.py` & `danielutils-0.9.78/danielutils/reflection/class_/class_reflection.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/reflection/file/file_reflection.py` & `danielutils-0.9.78/danielutils/reflection/file/file_reflection.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/reflection/function/function_reflections.py` & `danielutils-0.9.78/danielutils/reflection/function/function_reflections.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/reflection/interpreter/callstack.py` & `danielutils-0.9.78/danielutils/reflection/interpreter/callstack.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/reflection/interpreter/os_.py` & `danielutils-0.9.78/danielutils/reflection/interpreter/os_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/reflection/interpreter/packages.py` & `danielutils-0.9.78/danielutils/reflection/interpreter/packages.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/reflection/interpreter/python_version.py` & `danielutils-0.9.78/danielutils/reflection/interpreter/python_version.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/reflection/interpreter/tracer.py` & `danielutils-0.9.78/danielutils/reflection/interpreter/tracer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/reflection/module/package_reflection.py` & `danielutils-0.9.78/danielutils/reflection/module/package_reflection.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/system/independent.py` & `danielutils-0.9.78/danielutils/system/independent.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/system/windows/win32_ctime.py` & `danielutils-0.9.78/danielutils/system/windows/win32_ctime.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/system/windows/windows.py` & `danielutils-0.9.78/danielutils/system/windows/windows.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/text.py` & `danielutils-0.9.78/danielutils/text.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/time.py` & `danielutils-0.9.78/danielutils/time.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/tqdm_.py` & `danielutils-0.9.78/danielutils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/databases/all.py` & `danielutils-0.9.78/danielutils/university/databases/all.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/oop/observer.py` & `danielutils-0.9.78/danielutils/university/oop/observer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/conditional_variable/conditional_variable.py` & `danielutils-0.9.78/danielutils/university/probability/conditional_variable/conditional_variable.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/bernoulli.py` & `danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/bernoulli.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/binomial.py` & `danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/binomial.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py` & `danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/discrete.py` & `danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/discrete.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/geometric.py` & `danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/geometric.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/poisson.py` & `danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/poisson.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/conditional_variable/discrete/uniform.py` & `danielutils-0.9.78/danielutils/university/probability/conditional_variable/discrete/uniform.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/distributions.py` & `danielutils-0.9.78/danielutils/university/probability/distributions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/expressions/accumulation_expression.py` & `danielutils-0.9.78/danielutils/university/probability/expressions/accumulation_expression.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/expressions/probability_expression.py` & `danielutils-0.9.78/danielutils/university/probability/expressions/probability_expression.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/funcs/expected_value.py` & `danielutils-0.9.78/danielutils/university/probability/funcs/expected_value.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/operator.py` & `danielutils-0.9.78/danielutils/university/probability/operator.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/protocols.py` & `danielutils-0.9.78/danielutils/university/probability/protocols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/supp.py` & `danielutils-0.9.78/danielutils/university/probability/supp.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/university/probability/transformation.py` & `danielutils-0.9.78/danielutils/university/probability/transformation.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils/versioned_imports.py` & `danielutils-0.9.78/danielutils/versioned_imports.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/danielutils.egg-info/PKG-INFO` & `danielutils-0.9.78/danielutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.77
+Version: 0.9.78
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,15 +37,15 @@
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.75
+# danielutils v=0.9.78
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 **Tested python versions**: `3.8.0`*, `3.9.0`, `3.10.13`
```

### Comparing `danielutils-0.9.77/danielutils.egg-info/SOURCES.txt` & `danielutils-0.9.78/danielutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.77/pyproject.toml` & `danielutils-0.9.78/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "danielutils"
-version = "0.9.77"
+version = "0.9.78"
 authors = [
     { name = "danielnachumdev", email = "danielnachumdev@gmail.com" },
 ]
 dependencies = []
 keywords = ['functions', 'decorators', 'methods', 'better_builtins', 'metaclasses']
 license = { "file" = "./LICENSE" }
 description = "A python utils library for things I find useful"
```

