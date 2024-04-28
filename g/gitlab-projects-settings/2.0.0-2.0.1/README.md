# Comparing `tmp/gitlab_projects_settings-2.0.0.tar.gz` & `tmp/gitlab_projects_settings-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_settings-2.0.0.tar", last modified: Sat Apr 27 20:17:30 2024, max compression
+gzip compressed data, was "gitlab_projects_settings-2.0.1.tar", last modified: Sat Apr 27 22:18:04 2024, max compression
```

## Comparing `gitlab_projects_settings-2.0.0.tar` & `gitlab_projects_settings-2.0.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.804652 gitlab_projects_settings-2.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.797652 gitlab_projects_settings-2.0.0/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      703 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     7123 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.798652 gitlab_projects_settings-2.0.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4934 2024-04-27 20:17:30.804652 gitlab_projects_settings-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3325 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.803652 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4934 2024-04-27 20:17:30.000000 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-27 20:17:30.000000 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 20:17:30.000000 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-27 20:17:30.000000 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-27 20:17:30.000000 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-27 20:17:30.000000 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.800652 gitlab_projects_settings-2.0.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 20:17:30.804652 gitlab_projects_settings-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.800652 gitlab_projects_settings-2.0.0/src/
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.801652 gitlab_projects_settings-2.0.0/src/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8271 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/cli/entrypoint.py
--rwxrwxrwx   0 root         (0) root         (0)     5352 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.801652 gitlab_projects_settings-2.0.0/src/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11456 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/features/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.802652 gitlab_projects_settings-2.0.0/src/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.803652 gitlab_projects_settings-2.0.0/src/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/prints/colors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.803652 gitlab_projects_settings-2.0.0/src/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.340480 gitlab_projects_settings-2.0.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.334480 gitlab_projects_settings-2.0.1/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      703 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     7123 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.334480 gitlab_projects_settings-2.0.1/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     1785 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4934 2024-04-27 22:18:04.340480 gitlab_projects_settings-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3325 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.340480 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4934 2024-04-27 22:18:04.000000 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-27 22:18:04.000000 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 22:18:04.000000 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-27 22:18:04.000000 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-27 22:18:04.000000 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-27 22:18:04.000000 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.337480 gitlab_projects_settings-2.0.1/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 22:18:04.340480 gitlab_projects_settings-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.337480 gitlab_projects_settings-2.0.1/src/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.338480 gitlab_projects_settings-2.0.1/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9137 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     5352 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.338480 gitlab_projects_settings-2.0.1/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11891 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.339480 gitlab_projects_settings-2.0.1/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.339480 gitlab_projects_settings-2.0.1/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/prints/colors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.340480 gitlab_projects_settings-2.0.1/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/system/platform.py
```

### Comparing `gitlab_projects_settings-2.0.0/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_settings-2.0.1/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/.chglog/changelog.sh` & `gitlab_projects_settings-2.0.1/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/.chglog/config.yml` & `gitlab_projects_settings-2.0.1/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/.gitlab-ci.yml` & `gitlab_projects_settings-2.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/.style.yapf` & `gitlab_projects_settings-2.0.1/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/.vscode/extensions.json` & `gitlab_projects_settings-2.0.1/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/.vscode/settings.json` & `gitlab_projects_settings-2.0.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/CHANGELOG.md` & `gitlab_projects_settings-2.0.1/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,16 @@
 
+<a name="2.0.1"></a>
+## [2.0.1](https://gitlab.com/AdrianDC/gitlab-projects-settings/compare/2.0.0...2.0.1) (2024-04-28)
+
+### Bug Fixes
+
+* **entrypoint:** fix description updates faulty descriptions
+
+
 <a name="2.0.0"></a>
 ## [2.0.0](https://gitlab.com/AdrianDC/gitlab-projects-settings/compare/1.1.0...2.0.0) (2024-04-27)
 
 ### Bug Fixes
 
 * **gitlab:** enforce '--dry-run' usage and improve Python codestyle
 * **settings:** apply 'subgroup' feature to subgroup groups
```

### Comparing `gitlab_projects_settings-2.0.0/LICENSE` & `gitlab_projects_settings-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/PKG-INFO` & `gitlab_projects_settings-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 2.0.0
+Version: 2.0.1
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
```

### Comparing `gitlab_projects_settings-2.0.0/README.md` & `gitlab_projects_settings-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/PKG-INFO` & `gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 2.0.0
+Version: 2.0.1
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
```

### Comparing `gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/SOURCES.txt` & `gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/setup.py` & `gitlab_projects_settings-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/src/cli/entrypoint.py` & `gitlab_projects_settings-2.0.1/src/cli/entrypoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -114,14 +114,26 @@
         criteria: str,
         subgroup: bool = False,
     ) -> None:
 
         # Acquire group
         group = gitlab.group(criteria)
 
+        # Acquire parent group
+        parent_group: Group = None
+        if group.parent_id:
+            parent_group = gitlab.group(group.parent_id)
+
+        # Get parent description
+        parent_description: str = ''
+        parent_name: str = ''
+        if parent_group:
+            parent_description = parent_group.description
+            parent_name = parent_group.name
+
         # Show group details
         group_type = 'subgroup' if subgroup else 'group'
         print(f'{Colors.BOLD} - GitLab {group_type}: '
               f'{Colors.YELLOW_LIGHT}{group.full_path} '
               f'{Colors.CYAN}({group.description})'
               f'{Colors.RESET}')
 
@@ -130,16 +142,22 @@
             gitlab.group_set_description(criteria, options.set_description)
             print(f'{Colors.BOLD}   - Set description: '
                   f'{Colors.CYAN}{options.set_description}'
                   f'{Colors.RESET}')
 
         # Update group description
         elif options.update_description:
-            description = f'{group.name[:1].capitalize()}{group.name[1:]}' \
-                          f' - description'
+            parent_description_text: str = ''
+            if parent_name:
+                parent_description_text = ' - ' + GitLabFeature.Helper.describe(
+                    parent_description,
+                    parent_name,
+                )
+            description = f'{GitLabFeature.Helper.capitalize(group.name)}' \
+                          f'{parent_description_text}'
             gitlab.group_set_description(criteria, description)
             print(f'{Colors.BOLD}   - Updated description: '
                   f'{Colors.CYAN}{description}'
                   f'{Colors.RESET}')
 
         # Reset group members
         if options.reset_members:
@@ -166,14 +184,17 @@
         gitlab: GitLabFeature,
         criteria: str,
     ) -> None:
 
         # Acquire project
         project = gitlab.project(criteria)
 
+        # Acquire group
+        group = gitlab.group(project.namespace['id'])
+
         # Show project details
         print(f'{Colors.BOLD} - GitLab project: '
               f'{Colors.YELLOW_LIGHT}{project.path_with_namespace} '
               f'{Colors.CYAN}({project.description})'
               f'{Colors.RESET}')
 
         # Set project description
@@ -181,19 +202,23 @@
             gitlab.project_set_description(criteria, options.set_description)
             print(f'{Colors.BOLD}   - Set description: '
                   f'{Colors.CYAN}{options.set_description}'
                   f'{Colors.RESET}')
 
         # Update project description
         elif options.update_description:
-            description = f'{project.name[:1].capitalize()}{project.name[1:]}' \
-                            f' - description'
+            group_description = GitLabFeature.Helper.describe(
+                group.description,
+                group.name,
+            )
+            description = f'{GitLabFeature.Helper.capitalize(project.name)}' \
+                          f' - {group_description}'
             gitlab.project_set_description(criteria, description)
             print(f'{Colors.BOLD}   - Updated description: '
-                  f'{Colors.CYAN}{description}'
+                  f'{Colors.CYAN}{group_description}'
                   f'{Colors.RESET}')
 
         # Reset project features
         if options.reset_features:
             features = ', '.join(gitlab.project_reset_features(criteria))
             if features:
                 print(f'{Colors.BOLD}   - Reset features: '
```

### Comparing `gitlab_projects_settings-2.0.0/src/cli/main.py` & `gitlab_projects_settings-2.0.1/src/cli/main.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/src/features/gitlab.py` & `gitlab_projects_settings-2.0.1/src/features/gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,7 +313,25 @@
             # Save project
             project.save()
 
     # URL
     @property
     def url(self) -> str:
         return str(self.__gitlab.api_url)
+
+    # Helper class
+    class Helper:
+
+        # Capitalize
+        @staticmethod
+        def capitalize(text: str) -> str:
+            return f'{text[:1].capitalize()}{text[1:]}'
+
+        # Describe
+        @staticmethod
+        def describe(
+            description: str,
+            name: str,
+        ) -> str:
+            if description:
+                return description
+            return GitLabFeature.Helper.capitalize(name)
```

### Comparing `gitlab_projects_settings-2.0.0/src/package/version.py` & `gitlab_projects_settings-2.0.1/src/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/src/prints/colors.py` & `gitlab_projects_settings-2.0.1/src/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.0/src/system/platform.py` & `gitlab_projects_settings-2.0.1/src/system/platform.py`

 * *Files identical despite different names*

