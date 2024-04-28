# Comparing `tmp/gitlab_projects_settings-2.0.1.tar.gz` & `tmp/gitlab_projects_settings-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_settings-2.0.1.tar", last modified: Sat Apr 27 22:18:04 2024, max compression
+gzip compressed data, was "gitlab_projects_settings-2.0.2.tar", last modified: Sun Apr 28 16:16:46 2024, max compression
```

## Comparing `gitlab_projects_settings-2.0.1.tar` & `gitlab_projects_settings-2.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.340480 gitlab_projects_settings-2.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.334480 gitlab_projects_settings-2.0.1/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      703 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     7123 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.334480 gitlab_projects_settings-2.0.1/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     1785 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4934 2024-04-27 22:18:04.340480 gitlab_projects_settings-2.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3325 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.340480 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4934 2024-04-27 22:18:04.000000 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-27 22:18:04.000000 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 22:18:04.000000 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-27 22:18:04.000000 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-27 22:18:04.000000 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-27 22:18:04.000000 gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.337480 gitlab_projects_settings-2.0.1/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 22:18:04.340480 gitlab_projects_settings-2.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.337480 gitlab_projects_settings-2.0.1/src/
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.338480 gitlab_projects_settings-2.0.1/src/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9137 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/cli/entrypoint.py
--rwxrwxrwx   0 root         (0) root         (0)     5352 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.338480 gitlab_projects_settings-2.0.1/src/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11891 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/features/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.339480 gitlab_projects_settings-2.0.1/src/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.339480 gitlab_projects_settings-2.0.1/src/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/prints/colors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:18:04.340480 gitlab_projects_settings-2.0.1/src/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-27 22:17:57.000000 gitlab_projects_settings-2.0.1/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:16:46.924551 gitlab_projects_settings-2.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:16:46.918551 gitlab_projects_settings-2.0.2/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      703 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     7153 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:16:46.918551 gitlab_projects_settings-2.0.2/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     2145 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5092 2024-04-28 16:16:46.924551 gitlab_projects_settings-2.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3483 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:16:46.924551 gitlab_projects_settings-2.0.2/gitlab_projects_settings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5092 2024-04-28 16:16:46.000000 gitlab_projects_settings-2.0.2/gitlab_projects_settings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-28 16:16:46.000000 gitlab_projects_settings-2.0.2/gitlab_projects_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 16:16:46.000000 gitlab_projects_settings-2.0.2/gitlab_projects_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-28 16:16:46.000000 gitlab_projects_settings-2.0.2/gitlab_projects_settings.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-28 16:16:46.000000 gitlab_projects_settings-2.0.2/gitlab_projects_settings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-28 16:16:46.000000 gitlab_projects_settings-2.0.2/gitlab_projects_settings.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:16:46.920551 gitlab_projects_settings-2.0.2/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 16:16:46.924551 gitlab_projects_settings-2.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:16:46.921551 gitlab_projects_settings-2.0.2/src/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:16:46.922551 gitlab_projects_settings-2.0.2/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9137 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     5497 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:16:46.922551 gitlab_projects_settings-2.0.2/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11891 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:16:46.923551 gitlab_projects_settings-2.0.2/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:16:46.923551 gitlab_projects_settings-2.0.2/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/prints/colors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:16:46.924551 gitlab_projects_settings-2.0.2/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-28 16:16:40.000000 gitlab_projects_settings-2.0.2/src/system/platform.py
```

### Comparing `gitlab_projects_settings-2.0.1/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_settings-2.0.2/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/.chglog/changelog.sh` & `gitlab_projects_settings-2.0.2/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/.chglog/config.yml` & `gitlab_projects_settings-2.0.2/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/.gitlab-ci.yml` & `gitlab_projects_settings-2.0.2/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,15 @@
       when: on_success
   allow_failure: true
 
 typings:
   stage: prepare
   image: registry.gitlab.com/adriandc/gitlabci-local/gitlabci-local:codestyle
   variables:
+    MYPY_CACHE_DIR: /dev/null
     MYPY_FORCE_COLOR: 1
     TERM: ansi
   script:
     - set +x
     - |
       if [ $(git rev-list --count HEAD) -gt 1 ]; then
         mypy --follow-imports silent --pretty $(git diff --name-only $(git diff --exit-code >/dev/null && echo 'HEAD^' || echo 'HEAD') ./src/ ./setup.py) 2>/dev/null || true
```

### Comparing `gitlab_projects_settings-2.0.1/.style.yapf` & `gitlab_projects_settings-2.0.2/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/.vscode/extensions.json` & `gitlab_projects_settings-2.0.2/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/.vscode/settings.json` & `gitlab_projects_settings-2.0.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/CHANGELOG.md` & `gitlab_projects_settings-2.0.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,24 @@
 
+<a name="2.0.2"></a>
+## [2.0.2](https://gitlab.com/AdrianDC/gitlab-projects-settings/compare/2.0.1...2.0.2) (2024-04-28)
+
+### Ci
+
+* **gitlab-ci:** disable 'typing' mypy caching with 'MYPY_CACHE_DIR'
+
+### Documentation
+
+* **readme:** document GitLab tokens' creation instructions
+
+### Features
+
+* **main:** limit '--help' width to terminal width or 120 chars
+
+
 <a name="2.0.1"></a>
 ## [2.0.1](https://gitlab.com/AdrianDC/gitlab-projects-settings/compare/2.0.0...2.0.1) (2024-04-28)
 
 ### Bug Fixes
 
 * **entrypoint:** fix description updates faulty descriptions
```

### Comparing `gitlab_projects_settings-2.0.1/LICENSE` & `gitlab_projects_settings-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/PKG-INFO` & `gitlab_projects_settings-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 2.0.1
+Version: 2.0.2
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -46,14 +46,18 @@
 
 This tool can automatically configure and update the GitLab settings  
 of groups, subgroups and projects, using multiple available options.
 
 Repetitive tasks can be performed accross multiple projects at once,  
 for example protecting tags and branches, or setting a new avatar recursively.
 
+The following step is required before using the tool:
+
+- The GitLab user tokens must be created with an `api` scope (a short expiration date is recommended)
+
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
```

### Comparing `gitlab_projects_settings-2.0.1/README.md` & `gitlab_projects_settings-2.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 
 This tool can automatically configure and update the GitLab settings  
 of groups, subgroups and projects, using multiple available options.
 
 Repetitive tasks can be performed accross multiple projects at once,  
 for example protecting tags and branches, or setting a new avatar recursively.
 
+The following step is required before using the tool:
+
+- The GitLab user tokens must be created with an `api` scope (a short expiration date is recommended)
+
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
```

### Comparing `gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/PKG-INFO` & `gitlab_projects_settings-2.0.2/gitlab_projects_settings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 2.0.1
+Version: 2.0.2
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -46,14 +46,18 @@
 
 This tool can automatically configure and update the GitLab settings  
 of groups, subgroups and projects, using multiple available options.
 
 Repetitive tasks can be performed accross multiple projects at once,  
 for example protecting tags and branches, or setting a new avatar recursively.
 
+The following step is required before using the tool:
+
+- The GitLab user tokens must be created with an `api` scope (a short expiration date is recommended)
+
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
```

### Comparing `gitlab_projects_settings-2.0.1/gitlab_projects_settings.egg-info/SOURCES.txt` & `gitlab_projects_settings-2.0.2/gitlab_projects_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/setup.py` & `gitlab_projects_settings-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/src/cli/entrypoint.py` & `gitlab_projects_settings-2.0.2/src/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/src/cli/main.py` & `gitlab_projects_settings-2.0.2/src/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 # Standard libraries
 from argparse import (_ArgumentGroup, ArgumentParser, Namespace, RawTextHelpFormatter)
 from os import environ
+from shutil import get_terminal_size
 from sys import exit as sys_exit
 
 # Components
 from ..package.bundle import Bundle
 from ..package.version import Version
 from ..prints.colors import Colors
 from ..system.platform import Platform
@@ -23,14 +24,18 @@
     parser: ArgumentParser = ArgumentParser(
         prog=Bundle.NAME,
         description=f'{Bundle.NAME}: {Bundle.DESCRIPTION}',
         add_help=False,
         formatter_class=lambda prog: RawTextHelpFormatter(
             prog,
             max_help_position=30,
+            width=min(
+                120,
+                get_terminal_size().columns - 2,
+            ),
         ),
     )
 
     # Arguments internal definitions
     group = parser.add_argument_group('internal arguments')
     group.add_argument(
         '-h',
```

### Comparing `gitlab_projects_settings-2.0.1/src/features/gitlab.py` & `gitlab_projects_settings-2.0.2/src/features/gitlab.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/src/package/version.py` & `gitlab_projects_settings-2.0.2/src/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/src/prints/colors.py` & `gitlab_projects_settings-2.0.2/src/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.0.1/src/system/platform.py` & `gitlab_projects_settings-2.0.2/src/system/platform.py`

 * *Files identical despite different names*

