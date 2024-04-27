# Comparing `tmp/gitlab_projects_settings-1.1.0.tar.gz` & `tmp/gitlab_projects_settings-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_settings-1.1.0.tar", last modified: Thu Apr 25 08:04:34 2024, max compression
+gzip compressed data, was "gitlab_projects_settings-2.0.0.tar", last modified: Sat Apr 27 20:17:30 2024, max compression
```

## Comparing `gitlab_projects_settings-1.1.0.tar` & `gitlab_projects_settings-2.0.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.038734 gitlab_projects_settings-1.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.030734 gitlab_projects_settings-1.1.0/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      703 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     6097 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.030734 gitlab_projects_settings-1.1.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)      603 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4906 2024-04-25 08:04:34.037734 gitlab_projects_settings-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3297 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.031734 gitlab_projects_settings-1.1.0/gitlab_projects_settings/
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.033734 gitlab_projects_settings-1.1.0/gitlab_projects_settings/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5319 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.034734 gitlab_projects_settings-1.1.0/gitlab_projects_settings/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11344 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/features/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     7838 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/features/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.034734 gitlab_projects_settings-1.1.0/gitlab_projects_settings/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.035734 gitlab_projects_settings-1.1.0/gitlab_projects_settings/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/prints/colors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.035734 gitlab_projects_settings-1.1.0/gitlab_projects_settings/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings/system/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.037734 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4906 2024-04-25 08:04:34.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-25 08:04:34.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 08:04:34.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-25 08:04:34.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-25 08:04:34.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-25 08:04:34.000000 gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 08:04:34.037734 gitlab_projects_settings-1.1.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 08:04:34.038734 gitlab_projects_settings-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2677 2024-04-25 08:04:27.000000 gitlab_projects_settings-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.804652 gitlab_projects_settings-2.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.797652 gitlab_projects_settings-2.0.0/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      703 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     7123 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.798652 gitlab_projects_settings-2.0.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4934 2024-04-27 20:17:30.804652 gitlab_projects_settings-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3325 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.803652 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4934 2024-04-27 20:17:30.000000 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-27 20:17:30.000000 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 20:17:30.000000 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-27 20:17:30.000000 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-27 20:17:30.000000 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-27 20:17:30.000000 gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.800652 gitlab_projects_settings-2.0.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 20:17:30.804652 gitlab_projects_settings-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.800652 gitlab_projects_settings-2.0.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.801652 gitlab_projects_settings-2.0.0/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8271 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     5352 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.801652 gitlab_projects_settings-2.0.0/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11456 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.802652 gitlab_projects_settings-2.0.0/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.803652 gitlab_projects_settings-2.0.0/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/prints/colors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:17:30.803652 gitlab_projects_settings-2.0.0/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-27 20:17:23.000000 gitlab_projects_settings-2.0.0/src/system/platform.py
```

### Comparing `gitlab_projects_settings-1.1.0/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_settings-2.0.0/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.1.0/.chglog/changelog.sh` & `gitlab_projects_settings-2.0.0/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.1.0/.chglog/config.yml` & `gitlab_projects_settings-2.0.0/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.1.0/.gitlab-ci.yml` & `gitlab_projects_settings-2.0.0/.gitlab-ci.yml`

 * *Files 22% similar despite different names*

```diff
@@ -49,78 +49,115 @@
     - sh ./.chglog/changelog.sh --clean
     - git add -v ./CHANGELOG.md
     - git commit --amend --no-edit
     - git tag -f -m '' "${tag}"
   rules:
     - if: $CI_LOCAL
 
+readme:
+  stage: development
+  image: local:silent
+  script:
+    - |
+      export COLUMNS=120
+      mkdir -p ./.tmp/
+      PACKAGE_NAME=$(grep '^PROJECT_NAME =' ./setup.py | cut -d"'" -f2)
+      {
+        echo ''
+        echo '```yaml'
+        alignments='[ ]\{2,\}'
+        argument='[[:alnum:]][[:alnum:]_-]\{0,\}'
+        letter='[[:alnum:]_]\{1\}'
+        parameter='[-]\{1,2\}[[:alnum:]][[:alnum:]_-]\{0,\}'
+        word='[[:alnum:]_-]\{1,\}'
+        "${PACKAGE_NAME}" --help \
+          | sed '1d; $d' \
+          | sed "s/^\(  ${parameter} ${word}${alignments}\)/\1# /g" \
+          | sed "s/^\(  ${parameter}${alignments}\)/\1# /g" \
+          | sed "s/^\(  ${parameter}, ${parameter}${alignments}\)/\1# /g" \
+          | sed "s/^\(  ${argument}${alignments}\)/\1# /g"
+        echo '```'
+        echo ''
+      } >./.tmp/README.help.tmp
+    - |
+      lead='^<!-- readme-help-start -->$'
+      tail='^<!-- readme-help-stop -->$'
+      sed -i "/${lead}/,/${tail}/{ /${lead}/{ p; r ./.tmp/README.help.tmp
+        }; /${tail}/p; d }"  ./README.md | head -n 100
+    - rm -f ./.tmp/README.help.tmp
+    - |
+      git -c color.diff=always --no-pager diff ./README.md | grep --color=never '.' && echo ''
+      echo  ' > README: Updated successfully'
+  rules:
+    - if: $CI_LOCAL
+
 # =============================================================================
 # Stage: prepare
 
 codestyle:
   stage: prepare
   image: registry.gitlab.com/adriandc/gitlabci-local/gitlabci-local:codestyle
   script:
-    - yapf -i ./gitlab_projects_settings/*.py ./gitlab_projects_settings/*/*.py ./setup.py
-    - unify -i --quote "'" ./gitlab_projects_settings/*.py ./gitlab_projects_settings/*/*.py ./setup.py
+    - yapf -i ./src/*.py ./src/*/*.py ./setup.py
+    - unify -i --quote "'" ./src/*.py ./src/*/*.py ./setup.py
     - echo '' && git diff --name-status
     - git diff --quiet
   rules:
     - if: $CI_COMMIT_REF_NAME == "develop"
       changes:
         - 'CHANGELOG.md'
-        - 'gitlab_projects_settings/**/*'
         - 'requirements/**/*'
         - 'setup.py'
+        - 'src/**/*'
     - if: $CI_COMMIT_TAG || $CI_PIPELINE_SOURCE == "trigger" || $CI_PIPELINE_SOURCE == "web" || $CI_COMMIT_REF_NAME != "develop"
       when: on_success
   allow_failure: true
 
 lint:
   stage: prepare
   image: registry.gitlab.com/adriandc/gitlabci-local/gitlabci-local:codestyle
   variables:
     PIP_DISABLE_PIP_VERSION_CHECK: 1
   before_script:
     - pip3 install -q -r ./requirements/runtime.txt --upgrade
   script:
-    - pylint --errors-only ./gitlab_projects_settings/ ./setup.py
-    - pylint --disable=missing-docstring --load-plugins=pylint.extensions.no_self_use ./gitlab_projects_settings/ ./setup.py
+    - pylint --errors-only ./src/ ./setup.py
+    - pylint --disable=missing-docstring --load-plugins=pylint.extensions.no_self_use ./src/ ./setup.py
   rules:
     - if: $CI_COMMIT_REF_NAME == "develop"
       changes:
         - 'CHANGELOG.md'
-        - 'gitlab_projects_settings/**/*'
         - 'requirements/**/*'
         - 'setup.py'
+        - 'src/**/*'
     - if: $CI_COMMIT_TAG || $CI_PIPELINE_SOURCE == "trigger" || $CI_PIPELINE_SOURCE == "web" || $CI_COMMIT_REF_NAME != "develop"
       when: on_success
   allow_failure: true
 
 typings:
   stage: prepare
   image: registry.gitlab.com/adriandc/gitlabci-local/gitlabci-local:codestyle
   variables:
     MYPY_FORCE_COLOR: 1
     TERM: ansi
   script:
     - set +x
     - |
       if [ $(git rev-list --count HEAD) -gt 1 ]; then
-        mypy --follow-imports silent --pretty $(git diff --name-only $(git diff --exit-code >/dev/null && echo 'HEAD^' || echo 'HEAD') ./gitlab_projects_settings/ ./setup.py) 2>/dev/null || true
+        mypy --follow-imports silent --pretty $(git diff --name-only $(git diff --exit-code >/dev/null && echo 'HEAD^' || echo 'HEAD') ./src/ ./setup.py) 2>/dev/null || true
       fi
     - sleep 1
-    - mypy --follow-imports silent --pretty ./gitlab_projects_settings/ ./setup.py
+    - mypy --follow-imports silent --pretty ./src/ ./setup.py
   rules:
     - if: $CI_COMMIT_REF_NAME == "develop"
       changes:
         - 'CHANGELOG.md'
-        - 'gitlab_projects_settings/**/*'
         - 'requirements/**/*'
         - 'setup.py'
+        - 'src/**/*'
     - if: $CI_COMMIT_TAG || $CI_PIPELINE_SOURCE == "trigger" || $CI_PIPELINE_SOURCE == "web" || $CI_COMMIT_REF_NAME != "develop"
       when: on_success
   allow_failure: true
 
 # =============================================================================
 # Stage: build
 
@@ -133,16 +170,16 @@
     - python3 -m build
   after_script:
     - rm -rf ./build ./*.egg-info ./.eggs
   rules:
     - if: $CI_COMMIT_REF_NAME == "develop"
       changes:
         - 'CHANGELOG.md'
-        - 'gitlab_projects_settings/**/*'
         - 'requirements/**/*'
+        - 'src/**/*'
     - if: $CI_COMMIT_TAG || $CI_PIPELINE_SOURCE == "trigger" || $CI_PIPELINE_SOURCE == "web" || $CI_COMMIT_REF_NAME != "develop"
       when: on_success
   artifacts:
     paths:
       - dist/
 
 install:
```

### Comparing `gitlab_projects_settings-1.1.0/.style.yapf` & `gitlab_projects_settings-2.0.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.1.0/.vscode/extensions.json` & `gitlab_projects_settings-2.0.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.1.0/.vscode/settings.json` & `gitlab_projects_settings-2.0.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.1.0/LICENSE` & `gitlab_projects_settings-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.1.0/PKG-INFO` & `gitlab_projects_settings-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 1.1.0
+Version: 2.0.0
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -51,55 +51,55 @@
 for example protecting tags and branches, or setting a new avatar recursively.
 
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
+<!-- readme-help-start -->
 
 ```yaml
-usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group]
-                                [--exclude-subgroups] [--exclude-projects] [--reset-features]
-                                [--reset-members] [--set-avatar FILE] [--set-description TEXT]
-                                [--update-description] [--protect-branches]
+usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group] [--exclude-subgroups]
+                                [--exclude-projects] [--reset-features] [--reset-members] [--set-avatar FILE]
+                                [--set-description TEXT] [--update-description] [--protect-branches]
                                 [--protect-tags LEVEL]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
 internal arguments:
-  -h, --help            # Show this help message
-  --version             # Show the current version
+  -h, --help              # Show this help message
+  --version               # Show the current version
 
 credentials arguments:
-  -t TOKEN              # GitLab API token (default: GITLAB_TOKEN environment)
+  -t TOKEN                # GitLab API token (default: GITLAB_TOKEN environment)
 
 common settings arguments:
-  --dry-run             # Enable dry run mode to check without saving
-  --exclude-group       # Exclude parent group settings
-  --exclude-subgroups   # Exclude children subgroups settings
-  --exclude-projects    # Exclude children projects settings
+  --dry-run               # Enable dry run mode to check without saving
+  --exclude-group         # Exclude parent group settings
+  --exclude-subgroups     # Exclude children subgroups settings
+  --exclude-projects      # Exclude children projects settings
 
 general settings arguments:
-  --reset-features      # Reset features of GitLab projects based on usage
-  --reset-members       # Reset members of GitLab projects and groups
-  --set-avatar FILE     # Set avatar of GitLab projects and groups
-  --set-description TEXT
-                        # Set description of GitLab projects and groups
-  --update-description  # Update description of GitLab projects and groups automatically
+  --reset-features        # Reset features of GitLab projects based on usage
+  --reset-members         # Reset members of GitLab projects and groups
+  --set-avatar FILE       # Set avatar of GitLab projects and groups
+  --set-description TEXT  # Set description of GitLab projects and groups
+  --update-description    # Update description of GitLab projects and groups automatically
 
 repository settings arguments:
-  --protect-branches    # Protect branches with default master/main, develop and staging
-  --protect-tags LEVEL  # Protect tags at level [no-one,admins,maintainers,developers]
+  --protect-branches      # Protect branches with default master/main, develop and staging
+  --protect-tags LEVEL    # Protect tags at level [no-one,admins,maintainers,developers]
 
 positional arguments:
-  gitlab                # GitLab URL (default: https://gitlab.com)
-  path                  # GitLab group or project path
+  gitlab                  # GitLab URL (default: https://gitlab.com)
+  path                    # GitLab group or project path
 ```
 
+<!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Dependencies
 
 - [colored](https://pypi.org/project/colored/): Terminal colors and styles
```

### Comparing `gitlab_projects_settings-1.1.0/README.md` & `gitlab_projects_settings-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,55 +17,55 @@
 for example protecting tags and branches, or setting a new avatar recursively.
 
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
+<!-- readme-help-start -->
 
 ```yaml
-usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group]
-                                [--exclude-subgroups] [--exclude-projects] [--reset-features]
-                                [--reset-members] [--set-avatar FILE] [--set-description TEXT]
-                                [--update-description] [--protect-branches]
+usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group] [--exclude-subgroups]
+                                [--exclude-projects] [--reset-features] [--reset-members] [--set-avatar FILE]
+                                [--set-description TEXT] [--update-description] [--protect-branches]
                                 [--protect-tags LEVEL]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
 internal arguments:
-  -h, --help            # Show this help message
-  --version             # Show the current version
+  -h, --help              # Show this help message
+  --version               # Show the current version
 
 credentials arguments:
-  -t TOKEN              # GitLab API token (default: GITLAB_TOKEN environment)
+  -t TOKEN                # GitLab API token (default: GITLAB_TOKEN environment)
 
 common settings arguments:
-  --dry-run             # Enable dry run mode to check without saving
-  --exclude-group       # Exclude parent group settings
-  --exclude-subgroups   # Exclude children subgroups settings
-  --exclude-projects    # Exclude children projects settings
+  --dry-run               # Enable dry run mode to check without saving
+  --exclude-group         # Exclude parent group settings
+  --exclude-subgroups     # Exclude children subgroups settings
+  --exclude-projects      # Exclude children projects settings
 
 general settings arguments:
-  --reset-features      # Reset features of GitLab projects based on usage
-  --reset-members       # Reset members of GitLab projects and groups
-  --set-avatar FILE     # Set avatar of GitLab projects and groups
-  --set-description TEXT
-                        # Set description of GitLab projects and groups
-  --update-description  # Update description of GitLab projects and groups automatically
+  --reset-features        # Reset features of GitLab projects based on usage
+  --reset-members         # Reset members of GitLab projects and groups
+  --set-avatar FILE       # Set avatar of GitLab projects and groups
+  --set-description TEXT  # Set description of GitLab projects and groups
+  --update-description    # Update description of GitLab projects and groups automatically
 
 repository settings arguments:
-  --protect-branches    # Protect branches with default master/main, develop and staging
-  --protect-tags LEVEL  # Protect tags at level [no-one,admins,maintainers,developers]
+  --protect-branches      # Protect branches with default master/main, develop and staging
+  --protect-tags LEVEL    # Protect tags at level [no-one,admins,maintainers,developers]
 
 positional arguments:
-  gitlab                # GitLab URL (default: https://gitlab.com)
-  path                  # GitLab group or project path
+  gitlab                  # GitLab URL (default: https://gitlab.com)
+  path                    # GitLab group or project path
 ```
 
+<!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Dependencies
 
 - [colored](https://pypi.org/project/colored/): Terminal colors and styles
```

### Comparing `gitlab_projects_settings-1.1.0/gitlab_projects_settings/cli/main.py` & `gitlab_projects_settings-2.0.0/src/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,36 @@
 
 # Standard libraries
 from argparse import (_ArgumentGroup, ArgumentParser, Namespace, RawTextHelpFormatter)
 from os import environ
 from sys import exit as sys_exit
 
 # Components
-from ..features.settings import SettingsFeature
 from ..package.bundle import Bundle
 from ..package.version import Version
 from ..prints.colors import Colors
 from ..system.platform import Platform
+from .entrypoint import Entrypoint
 
 # Main, pylint: disable=too-many-statements
 def main() -> None:
 
     # Variables
     group: _ArgumentGroup
     result: bool = False
 
     # Arguments creation
     parser: ArgumentParser = ArgumentParser(
         prog=Bundle.NAME,
         description=f'{Bundle.NAME}: {Bundle.DESCRIPTION}',
         add_help=False,
-        formatter_class=RawTextHelpFormatter,
+        formatter_class=lambda prog: RawTextHelpFormatter(
+            prog,
+            max_help_position=30,
+        ),
     )
 
     # Arguments internal definitions
     group = parser.add_argument_group('internal arguments')
     group.add_argument(
         '-h',
         '--help',
@@ -100,15 +103,15 @@
         metavar='FILE',
         help='Set avatar of GitLab projects and groups',
     )
     group.add_argument(
         '--set-description',
         dest='set_description',
         action='store',
-        metavar='DESCRIPTION',
+        metavar='TEXT',
         help='Set description of GitLab projects and groups',
     )
     group.add_argument(
         '--update-description',
         dest='update_description',
         action='store_true',
         help='Update description of GitLab projects and groups automatically',
@@ -176,16 +179,16 @@
         Platform.flush()
         sys_exit(1)
 
     # Header
     print(' ')
     Platform.flush()
 
-    # Configure GitLab projects
-    result = SettingsFeature.entrypoint(options)
+    # CLI entrypoint
+    result = Entrypoint.cli(options)
 
     # Footer
     print(' ')
     Platform.flush()
 
     # Result
     if result:
```

### Comparing `gitlab_projects_settings-1.1.0/gitlab_projects_settings/features/gitlab.py` & `gitlab_projects_settings-2.0.0/src/features/gitlab.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,31 +38,31 @@
         if not self.__dry_run:
             group.save()
 
     # Group set avatar
     def group_set_avatar(self, criteria: str, file: str) -> None:
 
         # Set group avatar
-        group = self.group(criteria)
-        with open(file, 'rb') as avatar:
-            group.avatar = avatar
+        if not self.__dry_run:
+            group = self.group(criteria)
+            with open(file, 'rb') as avatar:
+                group.avatar = avatar
 
-            # Save group
-            if not self.__dry_run:
+                # Save group
                 group.save()
 
     # Group set description
     def group_set_description(self, criteria: str, description: str) -> None:
 
         # Set group description
-        group = self.group(criteria)
-        group.description = description
-
-        # Save group
         if not self.__dry_run:
+            group = self.group(criteria)
+            group.description = description
+
+            # Save group
             group.save()
 
     # Project
     def project(self, criteria: str) -> Project:
         return self.__gitlab.projects.get(criteria)
 
     # Project protect branches
@@ -278,37 +278,42 @@
         # Result
         return result
 
     # Project reset members
     def project_reset_members(self, criteria: str) -> None:
 
         # Remove project members
-        project = self.project(criteria)
-        for member in project.members.list():
-            if not self.__dry_run:
+        if not self.__dry_run:
+            project = self.project(criteria)
+            for member in project.members.list():
                 project.members.delete(member.id)
 
-        # Save project
-        if not self.__dry_run:
+            # Save project
             project.save()
 
     # Project set avatar
     def project_set_avatar(self, criteria: str, file: str) -> None:
 
         # Set project avatar
-        project = self.project(criteria)
-        with open(file, 'rb') as avatar:
-            project.avatar = avatar
-            if not self.__dry_run:
+        if not self.__dry_run:
+            project = self.project(criteria)
+            with open(file, 'rb') as avatar:
+                project.avatar = avatar
+
+                # Save project
                 project.save()
 
     # Project set description
     def project_set_description(self, criteria: str, description: str) -> None:
-        project = self.project(criteria)
-        project.description = description
+
+        # Set project description
         if not self.__dry_run:
+            project = self.project(criteria)
+            project.description = description
+
+            # Save project
             project.save()
 
     # URL
     @property
     def url(self) -> str:
         return str(self.__gitlab.api_url)
```

### Comparing `gitlab_projects_settings-1.1.0/gitlab_projects_settings/features/settings.py` & `gitlab_projects_settings-2.0.0/src/cli/entrypoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,81 +8,104 @@
 from gitlab.v4.objects import Group, Project
 
 # Components
 from ..features.gitlab import GitLabFeature
 from ..prints.colors import Colors
 from ..system.platform import Platform
 
-# SettingsFeature class, pylint: disable=too-few-public-methods
-class SettingsFeature:
+# Entrypoint class, pylint: disable=too-few-public-methods
+class Entrypoint:
 
-    # Entrypoint
+    # CLI
     @staticmethod
-    def entrypoint(options: Namespace) -> bool:
+    def cli(options: Namespace) -> bool:
 
         # Variables
         group: Group = None
         project: Project = None
 
         # Header
         print(' ')
 
         # GitLab client
-        gitlab = GitLabFeature(options.gitlab, options.token, options.dry_run)
+        gitlab = GitLabFeature(
+            options.gitlab,
+            options.token,
+            options.dry_run,
+        )
         print(f'{Colors.BOLD} - GitLab host: '
               f'{Colors.GREEN}{gitlab.url}'
               f'{Colors.RESET}')
         Platform.flush()
 
         # GitLab path
         try:
             group = gitlab.group(options.path)
             print(f'{Colors.BOLD} - GitLab group: '
-                  f'{Colors.GREEN}{group.full_path} ({group.description})'
+                  f'{Colors.GREEN}{group.full_path}'
+                  f'{Colors.CYAN} ({group.description})'
                   f'{Colors.RESET}')
             print(' ')
             Platform.flush()
         except GitlabGetError:
             project = gitlab.project(options.path)
             print(f'{Colors.BOLD} - GitLab project: '
-                  f'{Colors.GREEN}{project.path_with_namespace} ({project.description})'
+                  f'{Colors.GREEN}{project.path_with_namespace}'
+                  f'{Colors.CYAN} ({project.description})'
                   f'{Colors.RESET}')
             print(' ')
             Platform.flush()
 
         # Handle single project
         if project:
-            SettingsFeature.project(options, gitlab, project.id)
+            Entrypoint.project(
+                options,
+                gitlab,
+                project.id,
+            )
 
         # Handle group recursively
         elif group:
 
             # Handle group
             if not options.exclude_group:
-                SettingsFeature.group(options, gitlab, group.id)
+                Entrypoint.group(
+                    options,
+                    gitlab,
+                    group.id,
+                )
 
             # Iterate through subgroups
             if not options.exclude_subgroups:
                 for group_subgroup in group.descendant_groups.list(
                         get_all=True,
                         include_subgroups=True,
                         order_by='path',
                         sort='asc',
                 ):
-                    SettingsFeature.group(options, gitlab, group_subgroup.id)
+                    Entrypoint.group(
+                        options,
+                        gitlab,
+                        group_subgroup.id,
+                        True,
+                    )
 
             # Iterate through projects
             if not options.exclude_projects:
                 for group_project in group.projects.list(
                         get_all=True,
                         include_subgroups=not options.exclude_subgroups,
                         order_by='path',
                         sort='asc',
                 ):
-                    SettingsFeature.project(options, gitlab, group_project.id)
+                    Entrypoint.project(
+                        options,
+                        gitlab,
+                        group_project.id,
+                    )
 
         # Result
         return True
 
     # Group
     @staticmethod
     def group(
@@ -108,15 +131,15 @@
             print(f'{Colors.BOLD}   - Set description: '
                   f'{Colors.CYAN}{options.set_description}'
                   f'{Colors.RESET}')
 
         # Update group description
         elif options.update_description:
             description = f'{group.name[:1].capitalize()}{group.name[1:]}' \
-                            f' - description'
+                          f' - description'
             gitlab.group_set_description(criteria, description)
             print(f'{Colors.BOLD}   - Updated description: '
                   f'{Colors.CYAN}{description}'
                   f'{Colors.RESET}')
 
         # Reset group members
         if options.reset_members:
```

### Comparing `gitlab_projects_settings-1.1.0/gitlab_projects_settings/package/version.py` & `gitlab_projects_settings-2.0.0/src/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.1.0/gitlab_projects_settings/prints/colors.py` & `gitlab_projects_settings-2.0.0/src/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.1.0/gitlab_projects_settings/system/platform.py` & `gitlab_projects_settings-2.0.0/src/system/platform.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-1.1.0/gitlab_projects_settings.egg-info/PKG-INFO` & `gitlab_projects_settings-2.0.0/gitlab_projects_settings.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 1.1.0
+Version: 2.0.0
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -51,55 +51,55 @@
 for example protecting tags and branches, or setting a new avatar recursively.
 
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
+<!-- readme-help-start -->
 
 ```yaml
-usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group]
-                                [--exclude-subgroups] [--exclude-projects] [--reset-features]
-                                [--reset-members] [--set-avatar FILE] [--set-description TEXT]
-                                [--update-description] [--protect-branches]
+usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group] [--exclude-subgroups]
+                                [--exclude-projects] [--reset-features] [--reset-members] [--set-avatar FILE]
+                                [--set-description TEXT] [--update-description] [--protect-branches]
                                 [--protect-tags LEVEL]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
 internal arguments:
-  -h, --help            # Show this help message
-  --version             # Show the current version
+  -h, --help              # Show this help message
+  --version               # Show the current version
 
 credentials arguments:
-  -t TOKEN              # GitLab API token (default: GITLAB_TOKEN environment)
+  -t TOKEN                # GitLab API token (default: GITLAB_TOKEN environment)
 
 common settings arguments:
-  --dry-run             # Enable dry run mode to check without saving
-  --exclude-group       # Exclude parent group settings
-  --exclude-subgroups   # Exclude children subgroups settings
-  --exclude-projects    # Exclude children projects settings
+  --dry-run               # Enable dry run mode to check without saving
+  --exclude-group         # Exclude parent group settings
+  --exclude-subgroups     # Exclude children subgroups settings
+  --exclude-projects      # Exclude children projects settings
 
 general settings arguments:
-  --reset-features      # Reset features of GitLab projects based on usage
-  --reset-members       # Reset members of GitLab projects and groups
-  --set-avatar FILE     # Set avatar of GitLab projects and groups
-  --set-description TEXT
-                        # Set description of GitLab projects and groups
-  --update-description  # Update description of GitLab projects and groups automatically
+  --reset-features        # Reset features of GitLab projects based on usage
+  --reset-members         # Reset members of GitLab projects and groups
+  --set-avatar FILE       # Set avatar of GitLab projects and groups
+  --set-description TEXT  # Set description of GitLab projects and groups
+  --update-description    # Update description of GitLab projects and groups automatically
 
 repository settings arguments:
-  --protect-branches    # Protect branches with default master/main, develop and staging
-  --protect-tags LEVEL  # Protect tags at level [no-one,admins,maintainers,developers]
+  --protect-branches      # Protect branches with default master/main, develop and staging
+  --protect-tags LEVEL    # Protect tags at level [no-one,admins,maintainers,developers]
 
 positional arguments:
-  gitlab                # GitLab URL (default: https://gitlab.com)
-  path                  # GitLab group or project path
+  gitlab                  # GitLab URL (default: https://gitlab.com)
+  path                    # GitLab group or project path
 ```
 
+<!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Dependencies
 
 - [colored](https://pypi.org/project/colored/): Terminal colors and styles
```

### Comparing `gitlab_projects_settings-1.1.0/setup.py` & `gitlab_projects_settings-2.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,38 +19,48 @@
 # Project configurations
 PROJECT_AUTHOR = 'Adrian DC'
 PROJECT_DESCRIPTION = 'Configure GitLab groups and projects settings automatically'
 PROJECT_EMAIL = 'radian.dc@gmail.com'
 PROJECT_KEYWORDS = 'gitlab issues sync'
 PROJECT_NAME = 'gitlab-projects-settings'
 PROJECT_OWNER = 'AdrianDC'
-PROJECT_PACKAGE = 'gitlab-projects-settings'
+PROJECT_PACKAGE = 'gitlab_projects_settings'
 PROJECT_SCRIPTS = [
     'gitlab-projects-settings = gitlab_projects_settings.cli.main:main',
 ]
 
 # Setup configurations
 setup(
-    name=PROJECT_PACKAGE,
+    name=PROJECT_NAME,
     use_scm_version=True,
     author=PROJECT_AUTHOR,
     author_email=PROJECT_EMAIL,
     license='Apache License 2.0',
     description=PROJECT_DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url=f'https://gitlab.com/{PROJECT_OWNER}/{PROJECT_NAME}',
     project_urls={
         'Bug Reports': f'https://gitlab.com/{PROJECT_OWNER}/{PROJECT_NAME}/-/issues',
         'Changelog': f'https://gitlab.com/{PROJECT_OWNER}/{PROJECT_NAME}/blob/main/CHANGELOG.md',
-        'Documentation': f'https://gitlab.com/{PROJECT_OWNER}/{PROJECT_NAME}#{PROJECT_PACKAGE}',
+        'Documentation': f'https://gitlab.com/{PROJECT_OWNER}/{PROJECT_NAME}#{PROJECT_NAME}',
         'Source': f'https://gitlab.com/{PROJECT_OWNER}/{PROJECT_NAME}',
-        'Statistics': f'https://pypistats.org/packages/{PROJECT_PACKAGE}'
+        'Statistics': f'https://pypistats.org/packages/{PROJECT_NAME}'
+    },
+    packages=[
+        PROJECT_PACKAGE,
+    ] + [
+        f'{PROJECT_PACKAGE}.{module}' for module in find_packages(
+            where='src',
+            exclude=['tests'],
+        )
+    ],
+    package_dir={
+        PROJECT_PACKAGE: 'src',
     },
-    packages=find_packages(exclude=['tests']),
     setup_requires=['setuptools_scm'],
     install_requires=requirements,
     classifiers=[
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
```

