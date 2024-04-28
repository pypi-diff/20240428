# Comparing `tmp/YaraForge-0.1.8b1.tar.gz` & `tmp/YaraForge-0.1.9b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YaraForge-0.1.8b1.tar", last modified: Sun Apr 28 13:23:43 2024, max compression
+gzip compressed data, was "YaraForge-0.1.9b1.tar", last modified: Sun Apr 28 13:33:35 2024, max compression
```

## Comparing `YaraForge-0.1.8b1.tar` & `YaraForge-0.1.9b1.tar`

### file list

```diff
@@ -1,269 +1,270 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.073327 YaraForge-0.1.8b1/
--rw-rw-rw-   0        0        0     1110 2024-04-26 02:46:31.000000 YaraForge-0.1.8b1/LICENSE
--rw-rw-rw-   0        0        0        0 2024-03-12 14:12:32.000000 YaraForge-0.1.8b1/MANIFEST.in
--rw-rw-rw-   0        0        0     4252 2024-04-28 13:23:43.073327 YaraForge-0.1.8b1/PKG-INFO
--rw-rw-rw-   0        0        0     3377 2024-04-26 02:54:36.000000 YaraForge-0.1.8b1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.894023 YaraForge-0.1.8b1/YaraForge.egg-info/
--rw-rw-rw-   0        0        0     4252 2024-04-28 13:23:42.000000 YaraForge-0.1.8b1/YaraForge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8288 2024-04-28 13:23:42.000000 YaraForge-0.1.8b1/YaraForge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 13:23:42.000000 YaraForge-0.1.8b1/YaraForge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-28 13:23:42.000000 YaraForge-0.1.8b1/YaraForge.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-28 13:23:42.000000 YaraForge-0.1.8b1/YaraForge.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.894023 YaraForge-0.1.8b1/python/
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.942488 YaraForge-0.1.8b1/python/3/
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.943484 YaraForge-0.1.8b1/python/3/PyQt5/
--rw-rw-rw-   0        0        0     1235 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.950296 YaraForge-0.1.8b1/python/3/PyQt5/uic/
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.956203 YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/
--rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/__init__.py
--rw-rw-rw-   0        0        0     4645 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/compiler.py
--rw-rw-rw-   0        0        0     2742 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/indenter.py
--rw-rw-rw-   0        0        0     2374 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/misc.py
--rw-rw-rw-   0        0        0     4324 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/proxy_metaclass.py
--rw-rw-rw-   0        0        0     5903 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/qobjectcreator.py
--rw-rw-rw-   0        0        0    16315 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/qtproxies.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.958150 YaraForge-0.1.8b1/python/3/PyQt5/uic/Loader/
--rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/Loader/__init__.py
--rw-rw-rw-   0        0        0     2858 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/Loader/loader.py
--rw-rw-rw-   0        0        0     5022 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/Loader/qobjectcreator.py
--rw-rw-rw-   0        0        0     9507 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/__init__.py
--rw-rw-rw-   0        0        0     4192 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/driver.py
--rw-rw-rw-   0        0        0     2279 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/exceptions.py
--rw-rw-rw-   0        0        0     4566 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/icon_cache.py
--rw-rw-rw-   0        0        0     5970 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/objcreator.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.963071 YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v2/
--rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v2/__init__.py
--rw-rw-rw-   0        0        0      979 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v2/as_string.py
--rw-rw-rw-   0        0        0      869 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v2/ascii_upper.py
--rw-rw-rw-   0        0        0      763 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v2/proxy_base.py
--rw-rw-rw-   0        0        0      674 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v2/string_io.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.966352 YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v3/
--rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v3/__init__.py
--rw-rw-rw-   0        0        0      956 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v3/as_string.py
--rw-rw-rw-   0        0        0      866 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v3/ascii_upper.py
--rw-rw-rw-   0        0        0      745 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v3/proxy_base.py
--rw-rw-rw-   0        0        0      604 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v3/string_io.py
--rw-rw-rw-   0        0        0    17761 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/properties.py
--rw-rw-rw-   0        0        0     3094 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/pyuic.py
--rw-rw-rw-   0        0        0    38150 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/uiparser.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.972230 YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/__init__.py
--rw-rw-rw-   0        0        0     1101 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qaxcontainer.py
--rw-rw-rw-   0        0        0     1097 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qscintilla.py
--rw-rw-rw-   0        0        0     1106 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qtcharts.py
--rw-rw-rw-   0        0        0     1132 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qtprintsupport.py
--rw-rw-rw-   0        0        0     1106 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qtquickwidgets.py
--rw-rw-rw-   0        0        0     1112 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qtwebenginewidgets.py
--rw-rw-rw-   0        0        0     2507 2023-06-08 15:50:59.000000 YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qtwebkit.py
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:22.000000 YaraForge-0.1.8b1/python/3/__init__.py
--rw-rw-rw-   0        0        0   832972 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_allins.py
--rw-rw-rw-   0        0        0    14032 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_auto.py
--rw-rw-rw-   0        0        0     8502 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_bitrange.py
--rw-rw-rw-   0        0        0   136649 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_bytes.py
--rw-rw-rw-   0        0        0   129129 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_dbg.py
--rw-rw-rw-   0        0        0    40649 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_dirtree.py
--rw-rw-rw-   0        0        0    16401 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_diskio.py
--rw-rw-rw-   0        0        0     5818 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_entry.py
--rw-rw-rw-   0        0        0    19054 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_enum.py
--rw-rw-rw-   0        0        0    38928 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_expr.py
--rw-rw-rw-   0        0        0    18628 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_fixup.py
--rw-rw-rw-   0        0        0     8436 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_fpro.py
--rw-rw-rw-   0        0        0    34902 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_frame.py
--rw-rw-rw-   0        0        0    59731 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_funcs.py
--rw-rw-rw-   0        0        0    24940 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_gdl.py
--rw-rw-rw-   0        0        0   106310 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_graph.py
--rw-rw-rw-   0        0        0   788487 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_hexrays.py
--rw-rw-rw-   0        0        0   100897 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_ida.py
--rw-rw-rw-   0        0        0    40739 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_idaapi.py
--rw-rw-rw-   0        0        0     2719 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_idc.py
--rw-rw-rw-   0        0        0   134230 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_idd.py
--rw-rw-rw-   0        0        0   264974 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_idp.py
--rw-rw-rw-   0        0        0    16171 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_ieee.py
--rw-rw-rw-   0        0        0   379220 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_kernwin.py
--rw-rw-rw-   0        0        0    23145 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_lines.py
--rw-rw-rw-   0        0        0    37073 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_loader.py
--rw-rw-rw-   0        0        0    28642 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_moves.py
--rw-rw-rw-   0        0        0    91052 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_nalt.py
--rw-rw-rw-   0        0        0    39716 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_name.py
--rw-rw-rw-   0        0        0    43940 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_netnode.py
--rw-rw-rw-   0        0        0    11454 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_offset.py
--rw-rw-rw-   0        0        0    83307 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_pro.py
--rw-rw-rw-   0        0        0     6353 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_problems.py
--rw-rw-rw-   0        0        0    28927 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_range.py
--rw-rw-rw-   0        0        0     9907 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_registry.py
--rw-rw-rw-   0        0        0     7877 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_search.py
--rw-rw-rw-   0        0        0    51938 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_segment.py
--rw-rw-rw-   0        0        0     9757 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_segregs.py
--rw-rw-rw-   0        0        0     5334 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_srclang.py
--rw-rw-rw-   0        0        0     6429 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_strlist.py
--rw-rw-rw-   0        0        0    36082 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_struct.py
--rw-rw-rw-   0        0        0    22949 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_tryblks.py
--rw-rw-rw-   0        0        0   289055 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_typeinf.py
--rw-rw-rw-   0        0        0    69494 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_ua.py
--rw-rw-rw-   0        0        0    27691 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/ida_xref.py
--rw-rw-rw-   0        0        0     2993 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/idaapi.py
--rw-rw-rw-   0        0        0    19673 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/idadex.py
--rw-rw-rw-   0        0        0    23522 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/idautils.py
--rw-rw-rw-   0        0        0   195546 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/idc.py
--rw-rw-rw-   0        0        0     6547 2023-06-08 15:50:57.000000 YaraForge-0.1.8b1/python/3/init.py
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:22.000000 YaraForge-0.1.8b1/python/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.973233 YaraForge-0.1.8b1/python/examples/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.974374 YaraForge-0.1.8b1/python/examples/analysis/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/analysis/__init__.py
--rw-rw-rw-   0        0        0     3401 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/analysis/dump_func_info.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:42.998881 YaraForge-0.1.8b1/python/examples/core/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/core/__init__.py
--rw-rw-rw-   0        0        0     8158 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/actions.py
--rw-rw-rw-   0        0        0      996 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/add_hotkey.py
--rw-rw-rw-   0        0        0      736 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/add_idc_hotkey.py
--rw-rw-rw-   0        0        0     3758 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/auto_instantiate_widget_plugin.py
--rw-rw-rw-   0        0        0     3349 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/bin_search.py
--rw-rw-rw-   0        0        0      790 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/colorize_disassembly.py
--rw-rw-rw-   0        0        0     4898 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/colorize_disassembly_on_the_fly.py
--rw-rw-rw-   0        0        0     2373 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/create_structure_programmatically.py
--rw-rw-rw-   0        0        0     2623 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/custom_cli.py
--rw-rw-rw-   0        0        0     8878 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/custom_data_types_and_formats.py
--rw-rw-rw-   0        0        0     2683 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/dump_extra_comments.py
--rw-rw-rw-   0        0        0     1932 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/dump_flowchart.py
--rw-rw-rw-   0        0        0     2574 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/dump_selection.py
--rw-rw-rw-   0        0        0      741 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/extend_idc.py
--rw-rw-rw-   0        0        0      827 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/idapythonrc.py
--rw-rw-rw-   0        0        0     1266 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/install_user_defined_prefix.py
--rw-rw-rw-   0        0        0     1337 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/list_bookmarks.py
--rw-rw-rw-   0        0        0     3285 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/list_function_items.py
--rw-rw-rw-   0        0        0      804 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/list_imports.py
--rw-rw-rw-   0        0        0     1183 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/list_patched_bytes.py
--rw-rw-rw-   0        0        0     1021 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/list_problems.py
--rw-rw-rw-   0        0        0     1350 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/list_segment_functions.py
--rw-rw-rw-   0        0        0     1318 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/list_segment_functions_using_idautils.py
--rw-rw-rw-   0        0        0     2373 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/list_stkvar_xrefs.py
--rw-rw-rw-   0        0        0      670 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/list_strings.py
--rw-rw-rw-   0        0        0      933 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/produce_c_file.py
--rw-rw-rw-   0        0        0     1067 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/produce_lst_file.py
--rw-rw-rw-   0        0        0     1223 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/register_timer.py
--rw-rw-rw-   0        0        0     2820 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/core/trigger_actions_programmatically.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.000828 YaraForge-0.1.8b1/python/examples/cvt64/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/cvt64/__init__.py
--rw-rw-rw-   0        0        0     2815 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/cvt64/py_cvt64_sample.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.002334 YaraForge-0.1.8b1/python/examples/debugging/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/debugging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.005281 YaraForge-0.1.8b1/python/examples/debugging/appcall/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/debugging/appcall/__init__.py
--rw-rw-rw-   0        0        0     1577 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/debugging/appcall/simple_appcall_common.py
--rw-rw-rw-   0        0        0      895 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/debugging/appcall/simple_appcall_linux.py
--rw-rw-rw-   0        0        0     1284 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/debugging/appcall/simple_appcall_win.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.007228 YaraForge-0.1.8b1/python/examples/debugging/dbghooks/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/debugging/dbghooks/__init__.py
--rw-rw-rw-   0        0        0     3770 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/debugging/dbghooks/automatic_steps.py
--rw-rw-rw-   0        0        0     3813 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/debugging/dbghooks/dbg_trace.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.011122 YaraForge-0.1.8b1/python/examples/debugging/misc/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/debugging/misc/__init__.py
--rw-rw-rw-   0        0        0     2127 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/debugging/misc/print_call_stack.py
--rw-rw-rw-   0        0        0     1753 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/debugging/misc/print_registers.py
--rw-rw-rw-   0        0        0     1899 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/debugging/misc/registers_context_menu.py
--rw-rw-rw-   0        0        0      661 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/debugging/show_debug_names.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.027335 YaraForge-0.1.8b1/python/examples/hexrays/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/hexrays/__init__.py
--rw-rw-rw-   0        0        0     3512 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/colorize_pseudocode_lines.py
--rw-rw-rw-   0        0        0     3638 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/curpos_details.py
--rw-rw-rw-   0        0        0     2453 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/decompile_entry_points.py
--rw-rw-rw-   0        0        0      732 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds1.py
--rw-rw-rw-   0        0        0     2518 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds10.py
--rw-rw-rw-   0        0        0     2875 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds11.py
--rw-rw-rw-   0        0        0     5949 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds12.py
--rw-rw-rw-   0        0        0     1162 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds13.py
--rw-rw-rw-   0        0        0    10835 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds17.py
--rw-rw-rw-   0        0        0     2325 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds19.py
--rw-rw-rw-   0        0        0     3913 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds21.py
--rw-rw-rw-   0        0        0     7264 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds3.py
--rw-rw-rw-   0        0        0     3569 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds4.py
--rw-rw-rw-   0        0        0    12037 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds5.py
--rw-rw-rw-   0        0        0     3037 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds6.py
--rw-rw-rw-   0        0        0     1147 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds7.py
--rw-rw-rw-   0        0        0     3037 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds8.py
--rw-rw-rw-   0        0        0     1128 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds_create_hint.py
--rw-rw-rw-   0        0        0     4700 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds_hooks.py
--rw-rw-rw-   0        0        0     1860 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds_modify_user_lvars.py
--rw-rw-rw-   0        0        0     9292 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/hexrays/vds_xrefs.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.030249 YaraForge-0.1.8b1/python/examples/idbhooks/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/idbhooks/__init__.py
--rw-rw-rw-   0        0        0     9228 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/idbhooks/log_idb_events.py
--rw-rw-rw-   0        0        0     2882 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/idbhooks/operand_changed.py
--rw-rw-rw-   0        0        0     3116 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/idbhooks/replay_prototypes_changes.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.032230 YaraForge-0.1.8b1/python/examples/idphooks/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/idphooks/__init__.py
--rw-rw-rw-   0        0        0     1573 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/idphooks/ana_emu_out.py
--rw-rw-rw-   0        0        0     1329 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/idphooks/assemble.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.036151 YaraForge-0.1.8b1/python/examples/pyqt/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/pyqt/__init__.py
--rw-rw-rw-   0        0        0     3335 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/pyqt/inject_command.py
--rw-rw-rw-   0        0        0     5627 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/pyqt/paint_over_graph.py
--rw-rw-rw-   0        0        0     2599 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/pyqt/paint_over_navbar.py
--rw-rw-rw-   0        0        0     1130 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/pyqt/populate_pluginform_with_pyqt_widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.040043 YaraForge-0.1.8b1/python/examples/uihooks/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/uihooks/__init__.py
--rw-rw-rw-   0        0        0      972 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/uihooks/func_chooser_coloring.py
--rw-rw-rw-   0        0        0     4757 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/uihooks/lines_rendering.py
--rw-rw-rw-   0        0        0     5181 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/uihooks/log_misc_events.py
--rw-rw-rw-   0        0        0      644 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/uihooks/prevent_jump.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.040043 YaraForge-0.1.8b1/python/examples/widgets/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.041016 YaraForge-0.1.8b1/python/examples/widgets/forms/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/widgets/forms/__init__.py
--rw-rw-rw-   0        0        0    11536 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/forms/askusingform.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.043857 YaraForge-0.1.8b1/python/examples/widgets/graphs/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/widgets/graphs/__init__.py
--rw-rw-rw-   0        0        0     5336 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/graphs/custom_graph_with_actions.py
--rw-rw-rw-   0        0        0     3115 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/graphs/sync_two_graphs.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.045806 YaraForge-0.1.8b1/python/examples/widgets/idaview/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/widgets/idaview/__init__.py
--rw-rw-rw-   0        0        0     4003 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/idaview/wrap_idaview.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.048728 YaraForge-0.1.8b1/python/examples/widgets/listings/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/widgets/listings/__init__.py
--rw-rw-rw-   0        0        0     6720 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/listings/custom_viewer.py
--rw-rw-rw-   0        0        0     3956 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/listings/jump_next_comment.py
--rw-rw-rw-   0        0        0     3160 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/listings/save_and_restore_listing_pos.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.050673 YaraForge-0.1.8b1/python/examples/widgets/misc/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/widgets/misc/__init__.py
--rw-rw-rw-   0        0        0     1829 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/misc/add_menus.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.050673 YaraForge-0.1.8b1/python/examples/widgets/tabular_views/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/widgets/tabular_views/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.056144 YaraForge-0.1.8b1/python/examples/widgets/tabular_views/custom/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/widgets/tabular_views/custom/__init__.py
--rw-rw-rw-   0        0        0     5338 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/tabular_views/custom/choose.py
--rw-rw-rw-   0        0        0     1634 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/tabular_views/custom/choose_multi.py
--rw-rw-rw-   0        0        0    10380 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/tabular_views/custom/chooser_with_folders.py
--rw-rw-rw-   0        0        0     1579 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/tabular_views/custom/func_chooser.py
--rw-rw-rw-   0        0        0     3142 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/tabular_views/custom/lazy_loaded_chooser.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.058090 YaraForge-0.1.8b1/python/examples/widgets/tabular_views/string_window/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/widgets/tabular_views/string_window/__init__.py
--rw-rw-rw-   0        0        0     3204 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/tabular_views/string_window/show_selected_strings.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.059063 YaraForge-0.1.8b1/python/examples/widgets/waitbox/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.8b1/python/examples/widgets/waitbox/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-06-08 15:50:58.000000 YaraForge-0.1.8b1/python/examples/widgets/waitbox/show_and_hide_waitbox.py
--rw-rw-rw-   0        0        0       42 2024-04-28 13:23:43.075278 YaraForge-0.1.8b1/setup.cfg
--rw-rw-rw-   0        0        0     1321 2024-04-26 03:09:58.000000 YaraForge-0.1.8b1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.061010 YaraForge-0.1.8b1/yaraforge/
--rw-rw-rw-   0        0        0        0 2024-03-09 20:13:15.000000 YaraForge-0.1.8b1/yaraforge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.064491 YaraForge-0.1.8b1/yaraforge/maker/
--rw-rw-rw-   0        0        0        0 2024-03-11 07:42:22.000000 YaraForge-0.1.8b1/yaraforge/maker/__init__.py
--rw-rw-rw-   0        0        0     1614 2024-04-12 20:13:05.000000 YaraForge-0.1.8b1/yaraforge/maker/dump_maker.py
--rw-rw-rw-   0        0        0     2622 2024-04-12 20:13:05.000000 YaraForge-0.1.8b1/yaraforge/maker/instruction_maker.py
--rw-rw-rw-   0        0        0     5311 2024-04-27 19:07:29.000000 YaraForge-0.1.8b1/yaraforge/maker/yara_maker.py
--rw-rw-rw-   0        0        0     1322 2024-04-12 20:13:05.000000 YaraForge-0.1.8b1/yaraforge/metadata.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.066437 YaraForge-0.1.8b1/yaraforge/plugin/
--rw-rw-rw-   0        0        0     2387 2024-04-28 12:38:34.000000 YaraForge-0.1.8b1/yaraforge/plugin/__init__.py
--rw-rw-rw-   0        0        0      294 2024-04-12 20:13:05.000000 YaraForge-0.1.8b1/yaraforge/plugin/yaraforge.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.066437 YaraForge-0.1.8b1/yaraforge/tests/
--rw-rw-rw-   0        0        0        0 2024-03-12 14:12:08.000000 YaraForge-0.1.8b1/yaraforge/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.068388 YaraForge-0.1.8b1/yaraforge/updater/
--rw-rw-rw-   0        0        0        0 2024-04-28 07:57:02.000000 YaraForge-0.1.8b1/yaraforge/updater/__init__.py
--rw-rw-rw-   0        0        0     2509 2024-04-28 13:22:28.000000 YaraForge-0.1.8b1/yaraforge/updater/update.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:23:43.072318 YaraForge-0.1.8b1/yaraforge/utils/
--rw-rw-rw-   0        0        0        0 2024-03-11 07:42:44.000000 YaraForge-0.1.8b1/yaraforge/utils/__init__.py
--rw-rw-rw-   0        0        0     1413 2024-04-12 20:13:05.000000 YaraForge-0.1.8b1/yaraforge/utils/cache_dumper.py
--rw-rw-rw-   0        0        0     4659 2024-04-12 20:13:05.000000 YaraForge-0.1.8b1/yaraforge/utils/common.py
--rw-rw-rw-   0        0        0     2413 2024-04-12 20:13:05.000000 YaraForge-0.1.8b1/yaraforge/utils/logger.py
--rw-rw-rw-   0        0        0     1280 2024-04-12 20:13:05.000000 YaraForge-0.1.8b1/yaraforge/utils/opcode_processor.py
--rw-rw-rw-   0        0        0      342 2024-04-28 13:23:06.000000 YaraForge-0.1.8b1/yaraforge/version.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.891209 YaraForge-0.1.9b1/
+-rw-rw-rw-   0        0        0     1110 2024-04-26 02:46:31.000000 YaraForge-0.1.9b1/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-03-12 14:12:32.000000 YaraForge-0.1.9b1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4252 2024-04-28 13:33:35.891209 YaraForge-0.1.9b1/PKG-INFO
+-rw-rw-rw-   0        0        0     3377 2024-04-26 02:54:36.000000 YaraForge-0.1.9b1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.695109 YaraForge-0.1.9b1/YaraForge.egg-info/
+-rw-rw-rw-   0        0        0     4252 2024-04-28 13:33:35.000000 YaraForge-0.1.9b1/YaraForge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8318 2024-04-28 13:33:35.000000 YaraForge-0.1.9b1/YaraForge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 13:33:35.000000 YaraForge-0.1.9b1/YaraForge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-28 13:33:35.000000 YaraForge-0.1.9b1/YaraForge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-28 13:33:35.000000 YaraForge-0.1.9b1/YaraForge.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.696078 YaraForge-0.1.9b1/python/
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.739006 YaraForge-0.1.9b1/python/3/
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.739006 YaraForge-0.1.9b1/python/3/PyQt5/
+-rw-rw-rw-   0        0        0     1235 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.745820 YaraForge-0.1.9b1/python/3/PyQt5/uic/
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.750759 YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/
+-rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/__init__.py
+-rw-rw-rw-   0        0        0     4645 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/compiler.py
+-rw-rw-rw-   0        0        0     2742 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/indenter.py
+-rw-rw-rw-   0        0        0     2374 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/misc.py
+-rw-rw-rw-   0        0        0     4324 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/proxy_metaclass.py
+-rw-rw-rw-   0        0        0     5903 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/qobjectcreator.py
+-rw-rw-rw-   0        0        0    16315 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/qtproxies.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.753680 YaraForge-0.1.9b1/python/3/PyQt5/uic/Loader/
+-rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/Loader/__init__.py
+-rw-rw-rw-   0        0        0     2858 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/Loader/loader.py
+-rw-rw-rw-   0        0        0     5022 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/Loader/qobjectcreator.py
+-rw-rw-rw-   0        0        0     9507 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/__init__.py
+-rw-rw-rw-   0        0        0     4192 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/driver.py
+-rw-rw-rw-   0        0        0     2279 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/exceptions.py
+-rw-rw-rw-   0        0        0     4566 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/icon_cache.py
+-rw-rw-rw-   0        0        0     5970 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/objcreator.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.757135 YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v2/
+-rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v2/__init__.py
+-rw-rw-rw-   0        0        0      979 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v2/as_string.py
+-rw-rw-rw-   0        0        0      869 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v2/ascii_upper.py
+-rw-rw-rw-   0        0        0      763 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v2/proxy_base.py
+-rw-rw-rw-   0        0        0      674 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v2/string_io.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.761069 YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v3/
+-rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v3/__init__.py
+-rw-rw-rw-   0        0        0      956 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v3/as_string.py
+-rw-rw-rw-   0        0        0      866 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v3/ascii_upper.py
+-rw-rw-rw-   0        0        0      745 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v3/proxy_base.py
+-rw-rw-rw-   0        0        0      604 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v3/string_io.py
+-rw-rw-rw-   0        0        0    17761 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/properties.py
+-rw-rw-rw-   0        0        0     3094 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/pyuic.py
+-rw-rw-rw-   0        0        0    38150 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/uiparser.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.767966 YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/__init__.py
+-rw-rw-rw-   0        0        0     1101 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qaxcontainer.py
+-rw-rw-rw-   0        0        0     1097 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qscintilla.py
+-rw-rw-rw-   0        0        0     1106 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qtcharts.py
+-rw-rw-rw-   0        0        0     1132 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qtprintsupport.py
+-rw-rw-rw-   0        0        0     1106 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qtquickwidgets.py
+-rw-rw-rw-   0        0        0     1112 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qtwebenginewidgets.py
+-rw-rw-rw-   0        0        0     2507 2023-06-08 15:50:59.000000 YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qtwebkit.py
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:22.000000 YaraForge-0.1.9b1/python/3/__init__.py
+-rw-rw-rw-   0        0        0   832972 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_allins.py
+-rw-rw-rw-   0        0        0    14032 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_auto.py
+-rw-rw-rw-   0        0        0     8502 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_bitrange.py
+-rw-rw-rw-   0        0        0   136649 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_bytes.py
+-rw-rw-rw-   0        0        0   129129 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_dbg.py
+-rw-rw-rw-   0        0        0    40649 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_dirtree.py
+-rw-rw-rw-   0        0        0    16401 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_diskio.py
+-rw-rw-rw-   0        0        0     5818 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_entry.py
+-rw-rw-rw-   0        0        0    19054 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_enum.py
+-rw-rw-rw-   0        0        0    38928 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_expr.py
+-rw-rw-rw-   0        0        0    18628 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_fixup.py
+-rw-rw-rw-   0        0        0     8436 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_fpro.py
+-rw-rw-rw-   0        0        0    34902 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_frame.py
+-rw-rw-rw-   0        0        0    59731 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_funcs.py
+-rw-rw-rw-   0        0        0    24940 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_gdl.py
+-rw-rw-rw-   0        0        0   106310 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_graph.py
+-rw-rw-rw-   0        0        0   788487 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_hexrays.py
+-rw-rw-rw-   0        0        0   100897 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_ida.py
+-rw-rw-rw-   0        0        0    40739 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_idaapi.py
+-rw-rw-rw-   0        0        0     2719 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_idc.py
+-rw-rw-rw-   0        0        0   134230 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_idd.py
+-rw-rw-rw-   0        0        0   264974 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_idp.py
+-rw-rw-rw-   0        0        0    16171 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_ieee.py
+-rw-rw-rw-   0        0        0   379220 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_kernwin.py
+-rw-rw-rw-   0        0        0    23145 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_lines.py
+-rw-rw-rw-   0        0        0    37073 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_loader.py
+-rw-rw-rw-   0        0        0    28642 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_moves.py
+-rw-rw-rw-   0        0        0    91052 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_nalt.py
+-rw-rw-rw-   0        0        0    39716 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_name.py
+-rw-rw-rw-   0        0        0    43940 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_netnode.py
+-rw-rw-rw-   0        0        0    11454 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_offset.py
+-rw-rw-rw-   0        0        0    83307 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_pro.py
+-rw-rw-rw-   0        0        0     6353 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_problems.py
+-rw-rw-rw-   0        0        0    28927 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_range.py
+-rw-rw-rw-   0        0        0     9907 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_registry.py
+-rw-rw-rw-   0        0        0     7877 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_search.py
+-rw-rw-rw-   0        0        0    51938 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_segment.py
+-rw-rw-rw-   0        0        0     9757 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_segregs.py
+-rw-rw-rw-   0        0        0     5334 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_srclang.py
+-rw-rw-rw-   0        0        0     6429 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_strlist.py
+-rw-rw-rw-   0        0        0    36082 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_struct.py
+-rw-rw-rw-   0        0        0    22949 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_tryblks.py
+-rw-rw-rw-   0        0        0   289055 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_typeinf.py
+-rw-rw-rw-   0        0        0    69494 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_ua.py
+-rw-rw-rw-   0        0        0    27691 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/ida_xref.py
+-rw-rw-rw-   0        0        0     2993 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/idaapi.py
+-rw-rw-rw-   0        0        0    19673 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/idadex.py
+-rw-rw-rw-   0        0        0    23522 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/idautils.py
+-rw-rw-rw-   0        0        0   195546 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/idc.py
+-rw-rw-rw-   0        0        0     6547 2023-06-08 15:50:57.000000 YaraForge-0.1.9b1/python/3/init.py
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:22.000000 YaraForge-0.1.9b1/python/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.769002 YaraForge-0.1.9b1/python/examples/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.769983 YaraForge-0.1.9b1/python/examples/analysis/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/analysis/__init__.py
+-rw-rw-rw-   0        0        0     3401 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/analysis/dump_func_info.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.792036 YaraForge-0.1.9b1/python/examples/core/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/core/__init__.py
+-rw-rw-rw-   0        0        0     8158 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/actions.py
+-rw-rw-rw-   0        0        0      996 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/add_hotkey.py
+-rw-rw-rw-   0        0        0      736 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/add_idc_hotkey.py
+-rw-rw-rw-   0        0        0     3758 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/auto_instantiate_widget_plugin.py
+-rw-rw-rw-   0        0        0     3349 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/bin_search.py
+-rw-rw-rw-   0        0        0      790 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/colorize_disassembly.py
+-rw-rw-rw-   0        0        0     4898 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/colorize_disassembly_on_the_fly.py
+-rw-rw-rw-   0        0        0     2373 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/create_structure_programmatically.py
+-rw-rw-rw-   0        0        0     2623 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/custom_cli.py
+-rw-rw-rw-   0        0        0     8878 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/custom_data_types_and_formats.py
+-rw-rw-rw-   0        0        0     2683 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/dump_extra_comments.py
+-rw-rw-rw-   0        0        0     1932 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/dump_flowchart.py
+-rw-rw-rw-   0        0        0     2574 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/dump_selection.py
+-rw-rw-rw-   0        0        0      741 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/extend_idc.py
+-rw-rw-rw-   0        0        0      827 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/idapythonrc.py
+-rw-rw-rw-   0        0        0     1266 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/install_user_defined_prefix.py
+-rw-rw-rw-   0        0        0     1337 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/list_bookmarks.py
+-rw-rw-rw-   0        0        0     3285 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/list_function_items.py
+-rw-rw-rw-   0        0        0      804 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/list_imports.py
+-rw-rw-rw-   0        0        0     1183 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/list_patched_bytes.py
+-rw-rw-rw-   0        0        0     1021 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/list_problems.py
+-rw-rw-rw-   0        0        0     1350 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/list_segment_functions.py
+-rw-rw-rw-   0        0        0     1318 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/list_segment_functions_using_idautils.py
+-rw-rw-rw-   0        0        0     2373 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/list_stkvar_xrefs.py
+-rw-rw-rw-   0        0        0      670 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/list_strings.py
+-rw-rw-rw-   0        0        0      933 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/produce_c_file.py
+-rw-rw-rw-   0        0        0     1067 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/produce_lst_file.py
+-rw-rw-rw-   0        0        0     1223 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/register_timer.py
+-rw-rw-rw-   0        0        0     2820 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/core/trigger_actions_programmatically.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.793010 YaraForge-0.1.9b1/python/examples/cvt64/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/cvt64/__init__.py
+-rw-rw-rw-   0        0        0     2815 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/cvt64/py_cvt64_sample.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.794952 YaraForge-0.1.9b1/python/examples/debugging/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/debugging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.797927 YaraForge-0.1.9b1/python/examples/debugging/appcall/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/debugging/appcall/__init__.py
+-rw-rw-rw-   0        0        0     1577 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/debugging/appcall/simple_appcall_common.py
+-rw-rw-rw-   0        0        0      895 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/debugging/appcall/simple_appcall_linux.py
+-rw-rw-rw-   0        0        0     1284 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/debugging/appcall/simple_appcall_win.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.800136 YaraForge-0.1.9b1/python/examples/debugging/dbghooks/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/debugging/dbghooks/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/debugging/dbghooks/automatic_steps.py
+-rw-rw-rw-   0        0        0     3813 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/debugging/dbghooks/dbg_trace.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.803056 YaraForge-0.1.9b1/python/examples/debugging/misc/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/debugging/misc/__init__.py
+-rw-rw-rw-   0        0        0     2127 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/debugging/misc/print_call_stack.py
+-rw-rw-rw-   0        0        0     1753 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/debugging/misc/print_registers.py
+-rw-rw-rw-   0        0        0     1899 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/debugging/misc/registers_context_menu.py
+-rw-rw-rw-   0        0        0      661 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/debugging/show_debug_names.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.819008 YaraForge-0.1.9b1/python/examples/hexrays/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/hexrays/__init__.py
+-rw-rw-rw-   0        0        0     3512 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/colorize_pseudocode_lines.py
+-rw-rw-rw-   0        0        0     3638 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/curpos_details.py
+-rw-rw-rw-   0        0        0     2453 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/decompile_entry_points.py
+-rw-rw-rw-   0        0        0      732 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds1.py
+-rw-rw-rw-   0        0        0     2518 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds10.py
+-rw-rw-rw-   0        0        0     2875 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds11.py
+-rw-rw-rw-   0        0        0     5949 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds12.py
+-rw-rw-rw-   0        0        0     1162 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds13.py
+-rw-rw-rw-   0        0        0    10835 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds17.py
+-rw-rw-rw-   0        0        0     2325 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds19.py
+-rw-rw-rw-   0        0        0     3913 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds21.py
+-rw-rw-rw-   0        0        0     7264 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds3.py
+-rw-rw-rw-   0        0        0     3569 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds4.py
+-rw-rw-rw-   0        0        0    12037 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds5.py
+-rw-rw-rw-   0        0        0     3037 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds6.py
+-rw-rw-rw-   0        0        0     1147 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds7.py
+-rw-rw-rw-   0        0        0     3037 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds8.py
+-rw-rw-rw-   0        0        0     1128 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds_create_hint.py
+-rw-rw-rw-   0        0        0     4700 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds_hooks.py
+-rw-rw-rw-   0        0        0     1860 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds_modify_user_lvars.py
+-rw-rw-rw-   0        0        0     9292 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/hexrays/vds_xrefs.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.821929 YaraForge-0.1.9b1/python/examples/idbhooks/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/idbhooks/__init__.py
+-rw-rw-rw-   0        0        0     9228 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/idbhooks/log_idb_events.py
+-rw-rw-rw-   0        0        0     2882 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/idbhooks/operand_changed.py
+-rw-rw-rw-   0        0        0     3116 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/idbhooks/replay_prototypes_changes.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.823875 YaraForge-0.1.9b1/python/examples/idphooks/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/idphooks/__init__.py
+-rw-rw-rw-   0        0        0     1573 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/idphooks/ana_emu_out.py
+-rw-rw-rw-   0        0        0     1329 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/idphooks/assemble.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.827824 YaraForge-0.1.9b1/python/examples/pyqt/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/pyqt/__init__.py
+-rw-rw-rw-   0        0        0     3335 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/pyqt/inject_command.py
+-rw-rw-rw-   0        0        0     5627 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/pyqt/paint_over_graph.py
+-rw-rw-rw-   0        0        0     2599 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/pyqt/paint_over_navbar.py
+-rw-rw-rw-   0        0        0     1130 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/pyqt/populate_pluginform_with_pyqt_widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.831725 YaraForge-0.1.9b1/python/examples/uihooks/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/uihooks/__init__.py
+-rw-rw-rw-   0        0        0      972 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/uihooks/func_chooser_coloring.py
+-rw-rw-rw-   0        0        0     4757 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/uihooks/lines_rendering.py
+-rw-rw-rw-   0        0        0     5181 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/uihooks/log_misc_events.py
+-rw-rw-rw-   0        0        0      644 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/uihooks/prevent_jump.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.832695 YaraForge-0.1.9b1/python/examples/widgets/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.833667 YaraForge-0.1.9b1/python/examples/widgets/forms/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/widgets/forms/__init__.py
+-rw-rw-rw-   0        0        0    11536 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/forms/askusingform.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.835613 YaraForge-0.1.9b1/python/examples/widgets/graphs/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/widgets/graphs/__init__.py
+-rw-rw-rw-   0        0        0     5336 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/graphs/custom_graph_with_actions.py
+-rw-rw-rw-   0        0        0     3115 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/graphs/sync_two_graphs.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.837119 YaraForge-0.1.9b1/python/examples/widgets/idaview/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/widgets/idaview/__init__.py
+-rw-rw-rw-   0        0        0     4003 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/idaview/wrap_idaview.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.840082 YaraForge-0.1.9b1/python/examples/widgets/listings/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/widgets/listings/__init__.py
+-rw-rw-rw-   0        0        0     6720 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/listings/custom_viewer.py
+-rw-rw-rw-   0        0        0     3956 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/listings/jump_next_comment.py
+-rw-rw-rw-   0        0        0     3160 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/listings/save_and_restore_listing_pos.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.842029 YaraForge-0.1.9b1/python/examples/widgets/misc/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/widgets/misc/__init__.py
+-rw-rw-rw-   0        0        0     1829 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/misc/add_menus.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.843002 YaraForge-0.1.9b1/python/examples/widgets/tabular_views/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/widgets/tabular_views/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.847921 YaraForge-0.1.9b1/python/examples/widgets/tabular_views/custom/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/widgets/tabular_views/custom/__init__.py
+-rw-rw-rw-   0        0        0     5338 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/tabular_views/custom/choose.py
+-rw-rw-rw-   0        0        0     1634 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/tabular_views/custom/choose_multi.py
+-rw-rw-rw-   0        0        0    10380 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/tabular_views/custom/chooser_with_folders.py
+-rw-rw-rw-   0        0        0     1579 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/tabular_views/custom/func_chooser.py
+-rw-rw-rw-   0        0        0     3142 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/tabular_views/custom/lazy_loaded_chooser.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.849108 YaraForge-0.1.9b1/python/examples/widgets/tabular_views/string_window/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/widgets/tabular_views/string_window/__init__.py
+-rw-rw-rw-   0        0        0     3204 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/tabular_views/string_window/show_selected_strings.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.850080 YaraForge-0.1.9b1/python/examples/widgets/waitbox/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.9b1/python/examples/widgets/waitbox/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-06-08 15:50:58.000000 YaraForge-0.1.9b1/python/examples/widgets/waitbox/show_and_hide_waitbox.py
+-rw-rw-rw-   0        0        0       42 2024-04-28 13:33:35.893157 YaraForge-0.1.9b1/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2024-04-26 03:09:58.000000 YaraForge-0.1.9b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.853001 YaraForge-0.1.9b1/yaraforge/
+-rw-rw-rw-   0        0        0        0 2024-03-09 20:13:15.000000 YaraForge-0.1.9b1/yaraforge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.854947 YaraForge-0.1.9b1/yaraforge/maker/
+-rw-rw-rw-   0        0        0        0 2024-03-11 07:42:22.000000 YaraForge-0.1.9b1/yaraforge/maker/__init__.py
+-rw-rw-rw-   0        0        0     1614 2024-04-12 20:13:05.000000 YaraForge-0.1.9b1/yaraforge/maker/dump_maker.py
+-rw-rw-rw-   0        0        0     2622 2024-04-12 20:13:05.000000 YaraForge-0.1.9b1/yaraforge/maker/instruction_maker.py
+-rw-rw-rw-   0        0        0     5311 2024-04-27 19:07:29.000000 YaraForge-0.1.9b1/yaraforge/maker/yara_maker.py
+-rw-rw-rw-   0        0        0     1322 2024-04-12 20:13:05.000000 YaraForge-0.1.9b1/yaraforge/metadata.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.879932 YaraForge-0.1.9b1/yaraforge/plugin/
+-rw-rw-rw-   0        0        0     2387 2024-04-28 12:38:34.000000 YaraForge-0.1.9b1/yaraforge/plugin/__init__.py
+-rw-rw-rw-   0        0        0      294 2024-04-12 20:13:05.000000 YaraForge-0.1.9b1/yaraforge/plugin/yaraforge.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.881879 YaraForge-0.1.9b1/yaraforge/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-12 14:12:08.000000 YaraForge-0.1.9b1/yaraforge/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-28 13:32:56.000000 YaraForge-0.1.9b1/yaraforge/tests/test_empty.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.882852 YaraForge-0.1.9b1/yaraforge/updater/
+-rw-rw-rw-   0        0        0        0 2024-04-28 07:57:02.000000 YaraForge-0.1.9b1/yaraforge/updater/__init__.py
+-rw-rw-rw-   0        0        0     2509 2024-04-28 13:22:28.000000 YaraForge-0.1.9b1/yaraforge/updater/update.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:33:35.890236 YaraForge-0.1.9b1/yaraforge/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-11 07:42:44.000000 YaraForge-0.1.9b1/yaraforge/utils/__init__.py
+-rw-rw-rw-   0        0        0     1413 2024-04-12 20:13:05.000000 YaraForge-0.1.9b1/yaraforge/utils/cache_dumper.py
+-rw-rw-rw-   0        0        0     4659 2024-04-12 20:13:05.000000 YaraForge-0.1.9b1/yaraforge/utils/common.py
+-rw-rw-rw-   0        0        0     2413 2024-04-12 20:13:05.000000 YaraForge-0.1.9b1/yaraforge/utils/logger.py
+-rw-rw-rw-   0        0        0     1280 2024-04-12 20:13:05.000000 YaraForge-0.1.9b1/yaraforge/utils/opcode_processor.py
+-rw-rw-rw-   0        0        0      342 2024-04-28 13:33:29.000000 YaraForge-0.1.9b1/yaraforge/version.py
```

### Comparing `YaraForge-0.1.8b1/LICENSE` & `YaraForge-0.1.9b1/LICENSE`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/PKG-INFO` & `YaraForge-0.1.9b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YaraForge
-Version: 0.1.8b1
+Version: 0.1.9b1
 Summary: A plugin for IDA Pro to generate Yara rules from binary files.
 Home-page: https://github.com/zhaoxinnZ/YaraForge
 Author: Zhao Xinn, Tsai YA-HSUAN, Ting0525
 Author-email: zhaoxinzhang0429@gmail.com, aooood456@gmail.com, zg45154551@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `YaraForge-0.1.8b1/README.md` & `YaraForge-0.1.9b1/README.md`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/YaraForge.egg-info/PKG-INFO` & `YaraForge-0.1.9b1/YaraForge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YaraForge
-Version: 0.1.8b1
+Version: 0.1.9b1
 Summary: A plugin for IDA Pro to generate Yara rules from binary files.
 Home-page: https://github.com/zhaoxinnZ/YaraForge
 Author: Zhao Xinn, Tsai YA-HSUAN, Ting0525
 Author-email: zhaoxinzhang0429@gmail.com, aooood456@gmail.com, zg45154551@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `YaraForge-0.1.8b1/YaraForge.egg-info/SOURCES.txt` & `YaraForge-0.1.9b1/YaraForge.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,15 @@
 yaraforge/maker/__init__.py
 yaraforge/maker/dump_maker.py
 yaraforge/maker/instruction_maker.py
 yaraforge/maker/yara_maker.py
 yaraforge/plugin/__init__.py
 yaraforge/plugin/yaraforge.py
 yaraforge/tests/__init__.py
+yaraforge/tests/test_empty.py
 yaraforge/updater/__init__.py
 yaraforge/updater/update.py
 yaraforge/utils/__init__.py
 yaraforge/utils/cache_dumper.py
 yaraforge/utils/common.py
 yaraforge/utils/logger.py
 yaraforge/utils/opcode_processor.py
```

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/__init__.py` & `YaraForge-0.1.9b1/python/3/PyQt5/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/__init__.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/compiler.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/indenter.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/indenter.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/misc.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/misc.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/proxy_metaclass.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/proxy_metaclass.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/qobjectcreator.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/qobjectcreator.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/Compiler/qtproxies.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/Compiler/qtproxies.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/Loader/__init__.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/Loader/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/Loader/loader.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/Loader/loader.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/Loader/qobjectcreator.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/Loader/qobjectcreator.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/__init__.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/driver.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/driver.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/exceptions.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/exceptions.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/icon_cache.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/icon_cache.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/objcreator.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/objcreator.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v2/__init__.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v2/as_string.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v2/as_string.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v2/ascii_upper.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v2/ascii_upper.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v2/proxy_base.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v2/proxy_base.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v2/string_io.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v2/string_io.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v3/__init__.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v3/as_string.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v3/as_string.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v3/ascii_upper.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v3/ascii_upper.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v3/proxy_base.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v3/proxy_base.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/port_v3/string_io.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/port_v3/string_io.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/properties.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/properties.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/pyuic.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/pyuic.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/uiparser.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/uiparser.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qaxcontainer.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qaxcontainer.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qscintilla.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qscintilla.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qtcharts.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qtcharts.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qtprintsupport.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qtprintsupport.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qtquickwidgets.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qtquickwidgets.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qtwebenginewidgets.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qtwebenginewidgets.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/PyQt5/uic/widget-plugins/qtwebkit.py` & `YaraForge-0.1.9b1/python/3/PyQt5/uic/widget-plugins/qtwebkit.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_allins.py` & `YaraForge-0.1.9b1/python/3/ida_allins.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_auto.py` & `YaraForge-0.1.9b1/python/3/ida_auto.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_bitrange.py` & `YaraForge-0.1.9b1/python/3/ida_bitrange.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_bytes.py` & `YaraForge-0.1.9b1/python/3/ida_bytes.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_dbg.py` & `YaraForge-0.1.9b1/python/3/ida_dbg.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_dirtree.py` & `YaraForge-0.1.9b1/python/3/ida_dirtree.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_diskio.py` & `YaraForge-0.1.9b1/python/3/ida_diskio.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_entry.py` & `YaraForge-0.1.9b1/python/3/ida_entry.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_enum.py` & `YaraForge-0.1.9b1/python/3/ida_enum.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_expr.py` & `YaraForge-0.1.9b1/python/3/ida_expr.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_fixup.py` & `YaraForge-0.1.9b1/python/3/ida_fixup.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_fpro.py` & `YaraForge-0.1.9b1/python/3/ida_fpro.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_frame.py` & `YaraForge-0.1.9b1/python/3/ida_frame.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_funcs.py` & `YaraForge-0.1.9b1/python/3/ida_funcs.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_gdl.py` & `YaraForge-0.1.9b1/python/3/ida_gdl.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_graph.py` & `YaraForge-0.1.9b1/python/3/ida_graph.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_hexrays.py` & `YaraForge-0.1.9b1/python/3/ida_hexrays.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_ida.py` & `YaraForge-0.1.9b1/python/3/ida_ida.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_idaapi.py` & `YaraForge-0.1.9b1/python/3/ida_idaapi.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_idc.py` & `YaraForge-0.1.9b1/python/3/ida_idc.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_idd.py` & `YaraForge-0.1.9b1/python/3/ida_idd.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_idp.py` & `YaraForge-0.1.9b1/python/3/ida_idp.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_ieee.py` & `YaraForge-0.1.9b1/python/3/ida_ieee.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_kernwin.py` & `YaraForge-0.1.9b1/python/3/ida_kernwin.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_lines.py` & `YaraForge-0.1.9b1/python/3/ida_lines.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_loader.py` & `YaraForge-0.1.9b1/python/3/ida_loader.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_moves.py` & `YaraForge-0.1.9b1/python/3/ida_moves.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_nalt.py` & `YaraForge-0.1.9b1/python/3/ida_nalt.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_name.py` & `YaraForge-0.1.9b1/python/3/ida_name.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_netnode.py` & `YaraForge-0.1.9b1/python/3/ida_netnode.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_offset.py` & `YaraForge-0.1.9b1/python/3/ida_offset.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_pro.py` & `YaraForge-0.1.9b1/python/3/ida_pro.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_problems.py` & `YaraForge-0.1.9b1/python/3/ida_problems.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_range.py` & `YaraForge-0.1.9b1/python/3/ida_range.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_registry.py` & `YaraForge-0.1.9b1/python/3/ida_registry.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_search.py` & `YaraForge-0.1.9b1/python/3/ida_search.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_segment.py` & `YaraForge-0.1.9b1/python/3/ida_segment.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_segregs.py` & `YaraForge-0.1.9b1/python/3/ida_segregs.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_srclang.py` & `YaraForge-0.1.9b1/python/3/ida_srclang.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_strlist.py` & `YaraForge-0.1.9b1/python/3/ida_strlist.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_struct.py` & `YaraForge-0.1.9b1/python/3/ida_struct.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_tryblks.py` & `YaraForge-0.1.9b1/python/3/ida_tryblks.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_typeinf.py` & `YaraForge-0.1.9b1/python/3/ida_typeinf.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_ua.py` & `YaraForge-0.1.9b1/python/3/ida_ua.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/ida_xref.py` & `YaraForge-0.1.9b1/python/3/ida_xref.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/idaapi.py` & `YaraForge-0.1.9b1/python/3/idaapi.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/idadex.py` & `YaraForge-0.1.9b1/python/3/idadex.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/idautils.py` & `YaraForge-0.1.9b1/python/3/idautils.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/idc.py` & `YaraForge-0.1.9b1/python/3/idc.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/3/init.py` & `YaraForge-0.1.9b1/python/3/init.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/analysis/dump_func_info.py` & `YaraForge-0.1.9b1/python/examples/analysis/dump_func_info.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/actions.py` & `YaraForge-0.1.9b1/python/examples/core/actions.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/add_hotkey.py` & `YaraForge-0.1.9b1/python/examples/core/add_hotkey.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/add_idc_hotkey.py` & `YaraForge-0.1.9b1/python/examples/core/add_idc_hotkey.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/auto_instantiate_widget_plugin.py` & `YaraForge-0.1.9b1/python/examples/core/auto_instantiate_widget_plugin.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/bin_search.py` & `YaraForge-0.1.9b1/python/examples/core/bin_search.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/colorize_disassembly.py` & `YaraForge-0.1.9b1/python/examples/core/colorize_disassembly.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/colorize_disassembly_on_the_fly.py` & `YaraForge-0.1.9b1/python/examples/core/colorize_disassembly_on_the_fly.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/create_structure_programmatically.py` & `YaraForge-0.1.9b1/python/examples/core/create_structure_programmatically.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/custom_cli.py` & `YaraForge-0.1.9b1/python/examples/core/custom_cli.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/custom_data_types_and_formats.py` & `YaraForge-0.1.9b1/python/examples/core/custom_data_types_and_formats.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/dump_extra_comments.py` & `YaraForge-0.1.9b1/python/examples/core/dump_extra_comments.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/dump_flowchart.py` & `YaraForge-0.1.9b1/python/examples/core/dump_flowchart.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/dump_selection.py` & `YaraForge-0.1.9b1/python/examples/core/dump_selection.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/extend_idc.py` & `YaraForge-0.1.9b1/python/examples/core/extend_idc.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/idapythonrc.py` & `YaraForge-0.1.9b1/python/examples/core/idapythonrc.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/install_user_defined_prefix.py` & `YaraForge-0.1.9b1/python/examples/core/install_user_defined_prefix.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/list_bookmarks.py` & `YaraForge-0.1.9b1/python/examples/core/list_bookmarks.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/list_function_items.py` & `YaraForge-0.1.9b1/python/examples/core/list_function_items.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/list_imports.py` & `YaraForge-0.1.9b1/python/examples/core/list_imports.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/list_patched_bytes.py` & `YaraForge-0.1.9b1/python/examples/core/list_patched_bytes.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/list_problems.py` & `YaraForge-0.1.9b1/python/examples/core/list_problems.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/list_segment_functions.py` & `YaraForge-0.1.9b1/python/examples/core/list_segment_functions.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/list_segment_functions_using_idautils.py` & `YaraForge-0.1.9b1/python/examples/core/list_segment_functions_using_idautils.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/list_stkvar_xrefs.py` & `YaraForge-0.1.9b1/python/examples/core/list_stkvar_xrefs.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/list_strings.py` & `YaraForge-0.1.9b1/python/examples/core/list_strings.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/produce_c_file.py` & `YaraForge-0.1.9b1/python/examples/core/produce_c_file.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/produce_lst_file.py` & `YaraForge-0.1.9b1/python/examples/core/produce_lst_file.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/register_timer.py` & `YaraForge-0.1.9b1/python/examples/core/register_timer.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/core/trigger_actions_programmatically.py` & `YaraForge-0.1.9b1/python/examples/core/trigger_actions_programmatically.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/cvt64/py_cvt64_sample.py` & `YaraForge-0.1.9b1/python/examples/cvt64/py_cvt64_sample.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/debugging/appcall/simple_appcall_common.py` & `YaraForge-0.1.9b1/python/examples/debugging/appcall/simple_appcall_common.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/debugging/appcall/simple_appcall_linux.py` & `YaraForge-0.1.9b1/python/examples/debugging/appcall/simple_appcall_linux.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/debugging/appcall/simple_appcall_win.py` & `YaraForge-0.1.9b1/python/examples/debugging/appcall/simple_appcall_win.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/debugging/dbghooks/automatic_steps.py` & `YaraForge-0.1.9b1/python/examples/debugging/dbghooks/automatic_steps.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/debugging/dbghooks/dbg_trace.py` & `YaraForge-0.1.9b1/python/examples/debugging/dbghooks/dbg_trace.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/debugging/misc/print_call_stack.py` & `YaraForge-0.1.9b1/python/examples/debugging/misc/print_call_stack.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/debugging/misc/print_registers.py` & `YaraForge-0.1.9b1/python/examples/debugging/misc/print_registers.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/debugging/misc/registers_context_menu.py` & `YaraForge-0.1.9b1/python/examples/debugging/misc/registers_context_menu.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/debugging/show_debug_names.py` & `YaraForge-0.1.9b1/python/examples/debugging/show_debug_names.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/colorize_pseudocode_lines.py` & `YaraForge-0.1.9b1/python/examples/hexrays/colorize_pseudocode_lines.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/curpos_details.py` & `YaraForge-0.1.9b1/python/examples/hexrays/curpos_details.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/decompile_entry_points.py` & `YaraForge-0.1.9b1/python/examples/hexrays/decompile_entry_points.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds1.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds1.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds10.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds10.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds11.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds11.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds12.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds12.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds13.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds13.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds17.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds17.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds19.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds19.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds21.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds21.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds3.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds3.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds4.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds4.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds5.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds5.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds6.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds6.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds7.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds7.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds8.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds8.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds_create_hint.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds_create_hint.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds_hooks.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds_hooks.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds_modify_user_lvars.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds_modify_user_lvars.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/hexrays/vds_xrefs.py` & `YaraForge-0.1.9b1/python/examples/hexrays/vds_xrefs.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/idbhooks/log_idb_events.py` & `YaraForge-0.1.9b1/python/examples/idbhooks/log_idb_events.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/idbhooks/operand_changed.py` & `YaraForge-0.1.9b1/python/examples/idbhooks/operand_changed.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/idbhooks/replay_prototypes_changes.py` & `YaraForge-0.1.9b1/python/examples/idbhooks/replay_prototypes_changes.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/idphooks/ana_emu_out.py` & `YaraForge-0.1.9b1/python/examples/idphooks/ana_emu_out.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/idphooks/assemble.py` & `YaraForge-0.1.9b1/python/examples/idphooks/assemble.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/pyqt/inject_command.py` & `YaraForge-0.1.9b1/python/examples/pyqt/inject_command.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/pyqt/paint_over_graph.py` & `YaraForge-0.1.9b1/python/examples/pyqt/paint_over_graph.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/pyqt/paint_over_navbar.py` & `YaraForge-0.1.9b1/python/examples/pyqt/paint_over_navbar.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/pyqt/populate_pluginform_with_pyqt_widgets.py` & `YaraForge-0.1.9b1/python/examples/pyqt/populate_pluginform_with_pyqt_widgets.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/uihooks/func_chooser_coloring.py` & `YaraForge-0.1.9b1/python/examples/uihooks/func_chooser_coloring.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/uihooks/lines_rendering.py` & `YaraForge-0.1.9b1/python/examples/uihooks/lines_rendering.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/uihooks/log_misc_events.py` & `YaraForge-0.1.9b1/python/examples/uihooks/log_misc_events.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/uihooks/prevent_jump.py` & `YaraForge-0.1.9b1/python/examples/uihooks/prevent_jump.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/forms/askusingform.py` & `YaraForge-0.1.9b1/python/examples/widgets/forms/askusingform.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/graphs/custom_graph_with_actions.py` & `YaraForge-0.1.9b1/python/examples/widgets/graphs/custom_graph_with_actions.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/graphs/sync_two_graphs.py` & `YaraForge-0.1.9b1/python/examples/widgets/graphs/sync_two_graphs.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/idaview/wrap_idaview.py` & `YaraForge-0.1.9b1/python/examples/widgets/idaview/wrap_idaview.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/listings/custom_viewer.py` & `YaraForge-0.1.9b1/python/examples/widgets/listings/custom_viewer.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/listings/jump_next_comment.py` & `YaraForge-0.1.9b1/python/examples/widgets/listings/jump_next_comment.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/listings/save_and_restore_listing_pos.py` & `YaraForge-0.1.9b1/python/examples/widgets/listings/save_and_restore_listing_pos.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/misc/add_menus.py` & `YaraForge-0.1.9b1/python/examples/widgets/misc/add_menus.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/tabular_views/custom/choose.py` & `YaraForge-0.1.9b1/python/examples/widgets/tabular_views/custom/choose.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/tabular_views/custom/choose_multi.py` & `YaraForge-0.1.9b1/python/examples/widgets/tabular_views/custom/choose_multi.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/tabular_views/custom/chooser_with_folders.py` & `YaraForge-0.1.9b1/python/examples/widgets/tabular_views/custom/chooser_with_folders.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/tabular_views/custom/func_chooser.py` & `YaraForge-0.1.9b1/python/examples/widgets/tabular_views/custom/func_chooser.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/tabular_views/custom/lazy_loaded_chooser.py` & `YaraForge-0.1.9b1/python/examples/widgets/tabular_views/custom/lazy_loaded_chooser.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/tabular_views/string_window/show_selected_strings.py` & `YaraForge-0.1.9b1/python/examples/widgets/tabular_views/string_window/show_selected_strings.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/python/examples/widgets/waitbox/show_and_hide_waitbox.py` & `YaraForge-0.1.9b1/python/examples/widgets/waitbox/show_and_hide_waitbox.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/setup.py` & `YaraForge-0.1.9b1/setup.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/yaraforge/maker/dump_maker.py` & `YaraForge-0.1.9b1/yaraforge/maker/dump_maker.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/yaraforge/maker/instruction_maker.py` & `YaraForge-0.1.9b1/yaraforge/maker/instruction_maker.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/yaraforge/maker/yara_maker.py` & `YaraForge-0.1.9b1/yaraforge/maker/yara_maker.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/yaraforge/metadata.py` & `YaraForge-0.1.9b1/yaraforge/metadata.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/yaraforge/plugin/__init__.py` & `YaraForge-0.1.9b1/yaraforge/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/yaraforge/updater/update.py` & `YaraForge-0.1.9b1/yaraforge/updater/update.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/yaraforge/utils/cache_dumper.py` & `YaraForge-0.1.9b1/yaraforge/utils/cache_dumper.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/yaraforge/utils/common.py` & `YaraForge-0.1.9b1/yaraforge/utils/common.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/yaraforge/utils/logger.py` & `YaraForge-0.1.9b1/yaraforge/utils/logger.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.8b1/yaraforge/utils/opcode_processor.py` & `YaraForge-0.1.9b1/yaraforge/utils/opcode_processor.py`

 * *Files identical despite different names*

