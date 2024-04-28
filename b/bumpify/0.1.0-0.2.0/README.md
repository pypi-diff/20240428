# Comparing `tmp/bumpify-0.1.0.tar.gz` & `tmp/bumpify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumpify-0.1.0.tar", max compression
+gzip compressed data, was "bumpify-0.2.0.tar", max compression
```

## Comparing `bumpify-0.1.0.tar` & `bumpify-0.2.0.tar`

### file list

```diff
@@ -1,61 +1,71 @@
--rw-r--r--   0        0        0     1072 2024-04-22 16:27:42.181355 bumpify-0.1.0/LICENSE
--rw-r--r--   0        0        0     4152 2024-04-22 16:27:42.181355 bumpify-0.1.0/README.md
--rw-r--r--   0        0        0       22 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/__init__.py
--rw-r--r--   0        0        0      624 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/context.py
--rw-r--r--   0        0        0        0 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/api/__init__.py
--rw-r--r--   0        0        0     5090 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/api/commands.py
--rw-r--r--   0        0        0     2597 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/api/interface.py
--rw-r--r--   0        0        0     1744 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/api/presenters.py
--rw-r--r--   0        0        0     4078 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/api/providers.py
--rw-r--r--   0        0        0        0 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/config/__init__.py
--rw-r--r--   0        0        0     2538 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/config/exc.py
--rw-r--r--   0        0        0      513 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/config/helpers.py
--rw-r--r--   0        0        0     2450 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/config/implementation.py
--rw-r--r--   0        0        0     1506 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/config/interface.py
--rw-r--r--   0        0        0     4797 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/config/objects.py
--rw-r--r--   0        0        0        0 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/console/__init__.py
--rw-r--r--   0        0        0      746 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/console/_message_formatter.py
--rw-r--r--   0        0        0     2956 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/console/helpers.py
--rw-r--r--   0        0        0      660 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/console/input.py
--rw-r--r--   0        0        0     1793 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/console/interface.py
--rw-r--r--   0        0        0      702 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/console/objects.py
--rw-r--r--   0        0        0     1003 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/console/output.py
--rw-r--r--   0        0        0        0 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/filesystem/__init__.py
--rw-r--r--   0        0        0      668 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/filesystem/exc.py
--rw-r--r--   0        0        0     2388 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/filesystem/helpers.py
--rw-r--r--   0        0        0     4671 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/filesystem/implementation.py
--rw-r--r--   0        0        0     2805 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/filesystem/interface.py
--rw-r--r--   0        0        0        0 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/semver/__init__.py
--rw-r--r--   0        0        0     1473 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/semver/_changelog_formatters.py
--rw-r--r--   0        0        0      680 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/semver/_constants.py
--rw-r--r--   0        0        0     3821 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/semver/_parsing.py
--rw-r--r--   0        0        0     2735 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/semver/_version_file_updater.py
--rw-r--r--   0        0        0      964 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/semver/exc.py
--rw-r--r--   0        0        0     1600 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/semver/helpers.py
--rw-r--r--   0        0        0     4444 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/semver/implementation.py
--rw-r--r--   0        0        0     3107 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/semver/interface.py
--rw-r--r--   0        0        0    18959 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/semver/objects.py
--rw-r--r--   0        0        0        0 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/vcs/__init__.py
--rw-r--r--   0        0        0     1483 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/vcs/exc.py
--rw-r--r--   0        0        0     1610 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/vcs/helpers.py
--rw-r--r--   0        0        0        0 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/vcs/implementation/__init__.py
--rw-r--r--   0        0        0     7973 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/vcs/implementation/git.py
--rw-r--r--   0        0        0     2044 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/vcs/implementation/proxy.py
--rw-r--r--   0        0        0     4049 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/vcs/interface.py
--rw-r--r--   0        0        0     1226 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/core/vcs/objects.py
--rw-r--r--   0        0        0        0 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/delivery/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/delivery/cli/__init__.py
--rw-r--r--   0        0        0     3029 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/delivery/cli/__main__.py
--rw-r--r--   0        0        0      723 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/delivery/cli/decorators.py
--rw-r--r--   0        0        0      575 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/di/__init__.py
--rw-r--r--   0        0        0     1931 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/di/api.py
--rw-r--r--   0        0        0     1060 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/di/config.py
--rw-r--r--   0        0        0      485 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/di/console.py
--rw-r--r--   0        0        0     1079 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/di/filesystem.py
--rw-r--r--   0        0        0     1091 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/di/semver.py
--rw-r--r--   0        0        0     1212 2024-04-22 16:27:42.181355 bumpify-0.1.0/bumpify/di/vcs.py
--rw-r--r--   0        0        0     2921 2024-04-22 16:27:42.185355 bumpify-0.1.0/bumpify/exc.py
--rw-r--r--   0        0        0     5579 2024-04-22 16:27:42.185355 bumpify-0.1.0/bumpify/utils.py
--rw-r--r--   0        0        0      946 2024-04-22 16:27:42.185355 bumpify-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 bumpify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-28 17:53:41.902929 bumpify-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4327 2024-04-28 17:53:41.902929 bumpify-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/__init__.py
+-rw-r--r--   0        0        0      624 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/context.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/api/__init__.py
+-rw-r--r--   0        0        0     5090 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/api/commands.py
+-rw-r--r--   0        0        0     2597 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/api/interface.py
+-rw-r--r--   0        0        0     1744 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/api/presenters.py
+-rw-r--r--   0        0        0     4078 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/api/providers.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/config/__init__.py
+-rw-r--r--   0        0        0     2538 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/config/exc.py
+-rw-r--r--   0        0        0      513 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/config/helpers.py
+-rw-r--r--   0        0        0     2450 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/config/implementation.py
+-rw-r--r--   0        0        0     1506 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/config/interface.py
+-rw-r--r--   0        0        0     4797 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/config/objects.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/console/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/console/_message_formatter.py
+-rw-r--r--   0        0        0     2956 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/console/helpers.py
+-rw-r--r--   0        0        0      660 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/console/input.py
+-rw-r--r--   0        0        0     1793 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/console/interface.py
+-rw-r--r--   0        0        0      702 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/console/objects.py
+-rw-r--r--   0        0        0     1003 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/console/output.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/filesystem/__init__.py
+-rw-r--r--   0        0        0      668 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/filesystem/exc.py
+-rw-r--r--   0        0        0     2388 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/filesystem/helpers.py
+-rw-r--r--   0        0        0     4671 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/filesystem/implementation.py
+-rw-r--r--   0        0        0     2805 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/filesystem/interface.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/__init__.py
+-rw-r--r--   0        0        0      333 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/_utils.py
+-rw-r--r--   0        0        0      180 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/decorators.py
+-rw-r--r--   0        0        0      696 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/exc.py
+-rw-r--r--   0        0        0     3179 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/implementation.py
+-rw-r--r--   0        0        0     1885 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/interface.py
+-rw-r--r--   0        0        0      499 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/objects.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/__init__.py
+-rw-r--r--   0        0        0     1473 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/_changelog_formatters.py
+-rw-r--r--   0        0        0      680 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/_constants.py
+-rw-r--r--   0        0        0      744 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/_hook_invokers.py
+-rw-r--r--   0        0        0     3821 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/_parsing.py
+-rw-r--r--   0        0        0     2735 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/_version_file_updater.py
+-rw-r--r--   0        0        0      964 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/exc.py
+-rw-r--r--   0        0        0     1600 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/helpers.py
+-rw-r--r--   0        0        0      382 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/hooks.py
+-rw-r--r--   0        0        0     4626 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/implementation.py
+-rw-r--r--   0        0        0     3107 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/interface.py
+-rw-r--r--   0        0        0    18959 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/objects.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/__init__.py
+-rw-r--r--   0        0        0     1483 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/exc.py
+-rw-r--r--   0        0        0     1610 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/implementation/__init__.py
+-rw-r--r--   0        0        0     7973 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/implementation/git.py
+-rw-r--r--   0        0        0     2044 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/implementation/proxy.py
+-rw-r--r--   0        0        0     4049 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/interface.py
+-rw-r--r--   0        0        0     1226 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/objects.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/delivery/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/delivery/cli/__init__.py
+-rw-r--r--   0        0        0     3029 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/delivery/cli/__main__.py
+-rw-r--r--   0        0        0      723 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/delivery/cli/decorators.py
+-rw-r--r--   0        0        0      612 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/__init__.py
+-rw-r--r--   0        0        0     1931 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/api.py
+-rw-r--r--   0        0        0     1060 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/config.py
+-rw-r--r--   0        0        0      485 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/console.py
+-rw-r--r--   0        0        0     1079 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/filesystem.py
+-rw-r--r--   0        0        0      751 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/hook.py
+-rw-r--r--   0        0        0     1203 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/semver.py
+-rw-r--r--   0        0        0     1212 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/vcs.py
+-rw-r--r--   0        0        0     2921 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/exc.py
+-rw-r--r--   0        0        0     5704 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/utils.py
+-rw-r--r--   0        0        0      946 2024-04-28 17:53:41.906929 bumpify-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5490 1970-01-01 00:00:00.000000 bumpify-0.2.0/PKG-INFO
```

### Comparing `bumpify-0.1.0/LICENSE` & `bumpify-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/README.md` & `bumpify-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+![PyPI - Version](https://img.shields.io/pypi/v/bumpify)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/bumpify)
+![PyPI - License](https://img.shields.io/pypi/l/bumpify)
+
 # Bumpify
 
 Semantic versioning automation tool for software projects.
 
 ## About
 
 Bumpify is a CLI tool that analyzes VCS changelog of your project and generates
```

### Comparing `bumpify-0.1.0/bumpify/context.py` & `bumpify-0.2.0/bumpify/context.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/api/commands.py` & `bumpify-0.2.0/bumpify/core/api/commands.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/api/interface.py` & `bumpify-0.2.0/bumpify/core/api/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/api/presenters.py` & `bumpify-0.2.0/bumpify/core/api/presenters.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/api/providers.py` & `bumpify-0.2.0/bumpify/core/api/providers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/config/exc.py` & `bumpify-0.2.0/bumpify/core/config/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/config/helpers.py` & `bumpify-0.2.0/bumpify/core/config/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/config/implementation.py` & `bumpify-0.2.0/bumpify/core/config/implementation.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/config/interface.py` & `bumpify-0.2.0/bumpify/core/config/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/config/objects.py` & `bumpify-0.2.0/bumpify/core/config/objects.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/console/_message_formatter.py` & `bumpify-0.2.0/bumpify/core/console/_message_formatter.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/console/helpers.py` & `bumpify-0.2.0/bumpify/core/console/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/console/input.py` & `bumpify-0.2.0/bumpify/core/console/input.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/console/interface.py` & `bumpify-0.2.0/bumpify/core/console/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/console/objects.py` & `bumpify-0.2.0/bumpify/core/console/objects.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/console/output.py` & `bumpify-0.2.0/bumpify/core/console/output.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/filesystem/exc.py` & `bumpify-0.2.0/bumpify/core/filesystem/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/filesystem/helpers.py` & `bumpify-0.2.0/bumpify/core/filesystem/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/filesystem/implementation.py` & `bumpify-0.2.0/bumpify/core/filesystem/implementation.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/filesystem/interface.py` & `bumpify-0.2.0/bumpify/core/filesystem/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/semver/_changelog_formatters.py` & `bumpify-0.2.0/bumpify/core/semver/_changelog_formatters.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/semver/_constants.py` & `bumpify-0.2.0/bumpify/core/semver/_constants.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/semver/_parsing.py` & `bumpify-0.2.0/bumpify/core/semver/_parsing.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/semver/_version_file_updater.py` & `bumpify-0.2.0/bumpify/core/semver/_version_file_updater.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/semver/exc.py` & `bumpify-0.2.0/bumpify/core/semver/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/semver/helpers.py` & `bumpify-0.2.0/bumpify/core/semver/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/semver/implementation.py` & `bumpify-0.2.0/bumpify/core/semver/implementation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import io
 from typing import List, Optional
 
 from bumpify.core.config.objects import LoadedModuleConfig
 from bumpify.core.filesystem.interface import IFileSystemReaderWriter
+from bumpify.core.hook.interface import IHookApi
 from bumpify.core.semver.objects import (
     Changelog,
     ChangelogEntry,
     ChangelogEntryData,
     ConventionalCommit,
     Version,
     VersionTag,
 )
 from bumpify.core.vcs.interface import IVcsReaderWriter
 
-from . import _changelog_formatters, _version_file_updater
+from . import _changelog_formatters, _hook_invokers, _version_file_updater
 from .exc import UnsupportedChangelogFormat
 from .interface import ISemVerApi
 from .objects import SemVerConfig
 
 
 class SemVerApi(ISemVerApi):
     """Default implementation of the semantic versioning API."""
 
     def __init__(
         self,
         semver_config: LoadedModuleConfig[SemVerConfig],
         filesystem_reader_writer: IFileSystemReaderWriter,
         vcs_reader_writer: IVcsReaderWriter,
+        hook_api: IHookApi,
     ):
         self._semver_config = semver_config
         self._filesystem_reader_writer = filesystem_reader_writer
         self._vcs_reader_writer = vcs_reader_writer
+        self._hook_api = hook_api
 
     def list_version_tags(self) -> List[VersionTag]:
         result = []
         for tag in self._vcs_reader_writer.list_merged_tags():
             maybe_version_tag = VersionTag.from_tag(tag)
             if maybe_version_tag:
                 result.append(maybe_version_tag)
@@ -42,15 +45,17 @@
         return result
 
     def list_conventional_commits(
         self, start_rev: str = None, end_rev: str = None
     ) -> List[ConventionalCommit]:
         result = []
         for commit in self._vcs_reader_writer.list_commits(start_rev=start_rev, end_rev=end_rev):
-            maybe_conventional_commit = ConventionalCommit.from_commit(commit)
+            maybe_conventional_commit = _hook_invokers.invoke_parse_commit_hook(
+                self._hook_api, commit
+            )
             if maybe_conventional_commit:
                 result.append(maybe_conventional_commit)
         return result
 
     def fetch_unreleased_changes(self, version_tag: VersionTag) -> Optional[ChangelogEntryData]:
         conventional_commits = self.list_conventional_commits(start_rev=version_tag.tag.rev)
         if not conventional_commits:
```

### Comparing `bumpify-0.1.0/bumpify/core/semver/interface.py` & `bumpify-0.2.0/bumpify/core/semver/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/semver/objects.py` & `bumpify-0.2.0/bumpify/core/semver/objects.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/vcs/exc.py` & `bumpify-0.2.0/bumpify/core/vcs/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/vcs/helpers.py` & `bumpify-0.2.0/bumpify/core/vcs/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/vcs/implementation/git.py` & `bumpify-0.2.0/bumpify/core/vcs/implementation/git.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/vcs/implementation/proxy.py` & `bumpify-0.2.0/bumpify/core/vcs/implementation/proxy.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/vcs/interface.py` & `bumpify-0.2.0/bumpify/core/vcs/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/core/vcs/objects.py` & `bumpify-0.2.0/bumpify/core/vcs/objects.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/delivery/cli/__main__.py` & `bumpify-0.2.0/bumpify/delivery/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/delivery/cli/decorators.py` & `bumpify-0.2.0/bumpify/delivery/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/di/__init__.py` & `bumpify-0.2.0/bumpify/di/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from pydio.api import Provider
 
 from bumpify.context import Context
 
-from . import api, config, console, filesystem, semver, vcs
+from . import api, config, console, filesystem, hook, semver, vcs
 
 provider = Provider()
 provider.attach(api.provider)
 provider.attach(config.provider)
 provider.attach(semver.provider)
 provider.attach(filesystem.provider)
 provider.attach(vcs.provider)
 provider.attach(console.provider)
+provider.attach(hook.provider)
 
 
 @provider.provides(Context)
 def make_context():
     # NOTE: Context is created by injector to ensure that all providers will
     # use same instance of it. It must be initialized shortly after creation.
     return Context()
```

### Comparing `bumpify-0.1.0/bumpify/di/api.py` & `bumpify-0.2.0/bumpify/di/api.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/di/config.py` & `bumpify-0.2.0/bumpify/di/config.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/di/filesystem.py` & `bumpify-0.2.0/bumpify/di/filesystem.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/di/semver.py` & `bumpify-0.2.0/bumpify/di/semver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from pydio.api import Provider
 
 from bumpify import utils
 from bumpify.core.config.objects import LoadedConfig, LoadedModuleConfig
 from bumpify.core.filesystem.interface import IFileSystemReaderWriter
+from bumpify.core.hook.interface import IHookApi
 from bumpify.core.semver.implementation import SemVerApi
 from bumpify.core.semver.interface import ISemVerApi
 from bumpify.core.semver.objects import SemVerConfig
 from bumpify.core.vcs.interface import IVcsReaderWriter
 
 provider = Provider()
 
 
 @provider.provides(ISemVerApi)
 def make_semver_api(injector):
     semver_config = utils.inject_type(injector, LoadedModuleConfig[SemVerConfig])
     filesystem_reader_writer = utils.inject_type(injector, IFileSystemReaderWriter)
     vcs_reader_writer = utils.inject_type(injector, IVcsReaderWriter)
-    return SemVerApi(semver_config, filesystem_reader_writer, vcs_reader_writer)
+    hook_api = utils.inject_type(injector, IHookApi)
+    return SemVerApi(semver_config, filesystem_reader_writer, vcs_reader_writer, hook_api)
 
 
 @provider.provides(LoadedModuleConfig[SemVerConfig])
 def make_loaded_semver_config(injector):
     loaded_config = utils.inject_type(injector, LoadedConfig)
     loaded_semver_config = loaded_config.require_module_config(SemVerConfig)
     return loaded_semver_config
```

### Comparing `bumpify-0.1.0/bumpify/di/vcs.py` & `bumpify-0.2.0/bumpify/di/vcs.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/exc.py` & `bumpify-0.2.0/bumpify/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.1.0/bumpify/utils.py` & `bumpify-0.2.0/bumpify/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     args = tuple(x for x in args if x is not None)
     logger.debug("Running shell command: %r", args)
     p = subprocess.Popen(
         args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE, env=env
     )
     stdout, stderr = (x.strip() for x in p.communicate(input=input))
     if p.returncode != 0 or (fail_on_stderr and stderr):
+        logger.error("Shell command %r failed with returncode %d", args, p.returncode)
+        logger.error(stderr.decode())
         raise exc.ShellCommandError(args, p.returncode, stdout, stderr)
     return stdout
 
 
 @contextlib.contextmanager
 def cwd(path: str):
     """Temporarily change current working directory to *path*."""
```

### Comparing `bumpify-0.1.0/pyproject.toml` & `bumpify-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bumpify"
-version = "0.1.0"
+version = "0.2.0"
 description = "Semantic versioning automation tool for software projects"
 authors = ["Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mwiatrzyk/bumpify"
 keywords = ["semantic", "versioning", "cli", "tool"]
 classifiers = [
```

### Comparing `bumpify-0.1.0/PKG-INFO` & `bumpify-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpify
-Version: 0.1.0
+Version: 0.2.0
 Summary: Semantic versioning automation tool for software projects
 Home-page: https://github.com/mwiatrzyk/bumpify
 License: MIT
 Keywords: semantic,versioning,cli,tool
 Author: Maciej Wiatrzyk
 Author-email: maciej.wiatrzyk@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -24,14 +24,18 @@
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: pydantic (==2.6.3)
 Requires-Dist: pydio (>=0.4.1,<0.5.0)
 Requires-Dist: tomlkit (>=0.12.4,<0.13.0)
 Project-URL: Repository, https://github.com/mwiatrzyk/bumpify
 Description-Content-Type: text/markdown
 
+![PyPI - Version](https://img.shields.io/pypi/v/bumpify)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/bumpify)
+![PyPI - License](https://img.shields.io/pypi/l/bumpify)
+
 # Bumpify
 
 Semantic versioning automation tool for software projects.
 
 ## About
 
 Bumpify is a CLI tool that analyzes VCS changelog of your project and generates
```

