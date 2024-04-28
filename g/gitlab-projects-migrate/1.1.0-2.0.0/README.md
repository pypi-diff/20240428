# Comparing `tmp/gitlab_projects_migrate-1.1.0.tar.gz` & `tmp/gitlab_projects_migrate-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_migrate-1.1.0.tar", last modified: Mon Apr 22 00:53:17 2024, max compression
+gzip compressed data, was "gitlab_projects_migrate-2.0.0.tar", last modified: Sun Apr 28 16:08:49 2024, max compression
```

## Comparing `gitlab_projects_migrate-1.1.0.tar` & `gitlab_projects_migrate-2.0.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.116985 gitlab_projects_migrate-1.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.109985 gitlab_projects_migrate-1.1.0/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      702 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     6085 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.110985 gitlab_projects_migrate-1.1.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)      469 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5092 2024-04-22 00:53:17.115985 gitlab_projects_migrate-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.110985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.112985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4603 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.112985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3163 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/features/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     5472 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/features/migration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.113985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.114985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/prints/colors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.114985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/system/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.115985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5092 2024-04-22 00:53:17.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1178 2024-04-22 00:53:17.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 00:53:17.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2024-04-22 00:53:17.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-22 00:53:17.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-22 00:53:17.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.115985 gitlab_projects_migrate-1.1.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 00:53:17.116985 gitlab_projects_migrate-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2684 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:08:49.777668 gitlab_projects_migrate-2.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:08:49.769668 gitlab_projects_migrate-2.0.0/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      702 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     7153 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:08:49.770668 gitlab_projects_migrate-2.0.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     2079 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-04-28 16:08:49.776668 gitlab_projects_migrate-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3984 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:08:49.776668 gitlab_projects_migrate-2.0.0/gitlab_projects_migrate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-04-28 16:08:49.000000 gitlab_projects_migrate-2.0.0/gitlab_projects_migrate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      894 2024-04-28 16:08:49.000000 gitlab_projects_migrate-2.0.0/gitlab_projects_migrate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 16:08:49.000000 gitlab_projects_migrate-2.0.0/gitlab_projects_migrate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-28 16:08:49.000000 gitlab_projects_migrate-2.0.0/gitlab_projects_migrate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-28 16:08:49.000000 gitlab_projects_migrate-2.0.0/gitlab_projects_migrate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-28 16:08:49.000000 gitlab_projects_migrate-2.0.0/gitlab_projects_migrate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:08:49.772668 gitlab_projects_migrate-2.0.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 16:08:49.777668 gitlab_projects_migrate-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2875 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:08:49.773668 gitlab_projects_migrate-2.0.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:08:49.773668 gitlab_projects_migrate-2.0.0/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18654 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     5991 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:08:49.774668 gitlab_projects_migrate-2.0.0/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10277 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:08:49.775668 gitlab_projects_migrate-2.0.0/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:08:49.775668 gitlab_projects_migrate-2.0.0/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/prints/colors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:08:49.776668 gitlab_projects_migrate-2.0.0/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-28 16:08:42.000000 gitlab_projects_migrate-2.0.0/src/system/platform.py
```

### Comparing `gitlab_projects_migrate-1.1.0/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_migrate-2.0.0/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.1.0/.chglog/changelog.sh` & `gitlab_projects_migrate-2.0.0/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.1.0/.chglog/config.yml` & `gitlab_projects_migrate-2.0.0/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.1.0/.gitlab-ci.yml` & `gitlab_projects_migrate-2.0.0/.gitlab-ci.yml`

 * *Files 20% similar despite different names*

```diff
@@ -49,78 +49,116 @@
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
-    - yapf -i ./gitlab_projects_migrate/*.py ./gitlab_projects_migrate/*/*.py ./setup.py
-    - unify -i --quote "'" ./gitlab_projects_migrate/*.py ./gitlab_projects_migrate/*/*.py ./setup.py
+    - yapf -i ./src/*.py ./src/*/*.py ./setup.py
+    - unify -i --quote "'" ./src/*.py ./src/*/*.py ./setup.py
     - echo '' && git diff --name-status
     - git diff --quiet
   rules:
     - if: $CI_COMMIT_REF_NAME == "develop"
       changes:
         - 'CHANGELOG.md'
-        - 'gitlab_projects_migrate/**/*'
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
-    - pylint --errors-only ./gitlab_projects_migrate/ ./setup.py
-    - pylint --disable=missing-docstring --load-plugins=pylint.extensions.no_self_use ./gitlab_projects_migrate/ ./setup.py
+    - pylint --errors-only ./src/ ./setup.py
+    - pylint --disable=missing-docstring --load-plugins=pylint.extensions.no_self_use ./src/ ./setup.py
   rules:
     - if: $CI_COMMIT_REF_NAME == "develop"
       changes:
         - 'CHANGELOG.md'
-        - 'gitlab_projects_migrate/**/*'
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
+    MYPY_CACHE_DIR: /dev/null
     MYPY_FORCE_COLOR: 1
     TERM: ansi
   script:
     - set +x
     - |
       if [ $(git rev-list --count HEAD) -gt 1 ]; then
-        mypy --follow-imports silent --pretty $(git diff --name-only $(git diff --exit-code >/dev/null && echo 'HEAD^' || echo 'HEAD') ./gitlab_projects_migrate/ ./setup.py) 2>/dev/null || true
+        mypy --follow-imports silent --pretty $(git diff --name-only $(git diff --exit-code >/dev/null && echo 'HEAD^' || echo 'HEAD') ./src/ ./setup.py) 2>/dev/null || true
       fi
     - sleep 1
-    - mypy --follow-imports silent --pretty ./gitlab_projects_migrate/ ./setup.py
+    - mypy --follow-imports silent --pretty ./src/ ./setup.py
   rules:
     - if: $CI_COMMIT_REF_NAME == "develop"
       changes:
         - 'CHANGELOG.md'
-        - 'gitlab_projects_migrate/**/*'
         - 'requirements/**/*'
         - 'setup.py'
+        - 'src/**/*'
     - if: $CI_COMMIT_TAG || $CI_PIPELINE_SOURCE == "trigger" || $CI_PIPELINE_SOURCE == "web" || $CI_COMMIT_REF_NAME != "develop"
       when: on_success
   allow_failure: true
 
 # =============================================================================
 # Stage: build
 
@@ -133,16 +171,16 @@
     - python3 -m build
   after_script:
     - rm -rf ./build ./*.egg-info ./.eggs
   rules:
     - if: $CI_COMMIT_REF_NAME == "develop"
       changes:
         - 'CHANGELOG.md'
-        - 'gitlab_projects_migrate/**/*'
         - 'requirements/**/*'
+        - 'src/**/*'
     - if: $CI_COMMIT_TAG || $CI_PIPELINE_SOURCE == "trigger" || $CI_PIPELINE_SOURCE == "web" || $CI_COMMIT_REF_NAME != "develop"
       when: on_success
   artifacts:
     paths:
       - dist/
 
 install:
```

### Comparing `gitlab_projects_migrate-1.1.0/.style.yapf` & `gitlab_projects_migrate-2.0.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.1.0/.vscode/extensions.json` & `gitlab_projects_migrate-2.0.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.1.0/.vscode/settings.json` & `gitlab_projects_migrate-2.0.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.1.0/LICENSE` & `gitlab_projects_migrate-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.1.0/PKG-INFO` & `gitlab_projects_migrate-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-migrate
-Version: 1.1.0
+Version: 2.0.0
 Summary: Migrate GitLab projects from a GitLab group to another GitLab's group
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-migrate
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-migrate/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-migrate/blob/main/CHANGELOG.md
@@ -73,41 +73,52 @@
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
+<!-- readme-help-start -->
 
 ```yaml
-usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--keep-members] [--overwrite]
+usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--dry-run] [--exclude-group]
+                               [--exclude-subgroups] [--exclude-projects] [--keep-members] [--overwrite]
                                [--set-avatar FILE] [--update-description]
-                               [input_gitlab] [input_group] [output_gitlab] [output_group]
+                               [input_gitlab] [input_path] [output_gitlab] [output_group]
 
-gitlab-projects-migrate: Synchronize projects from a GitLab group to another GitLab group
+gitlab-projects-migrate: Migrate GitLab projects from a GitLab group to another GitLab's group
 
 internal arguments:
   -h, --help            # Show this help message
   --version             # Show the current version
 
+credentials arguments:
+  -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
+  -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
+
 migration arguments:
-  -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN environment)
-  -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN environment or input_token)
+  --dry-run             # Enable dry run mode to check without saving
+  --exclude-group       # Exclude parent group migration
+  --exclude-subgroups   # Exclude children subgroups migration
+  --exclude-projects    # Exclude children projects migration
   --keep-members        # Keep input members after importing on output GitLab
   --overwrite           # Overwrite existing projects on output GitLab
-  --set-avatar FILE     # Set imported projects' avatar to a specific image file
-  --update-description  # Update project description automatically inside output group
+
+general settings arguments:
+  --set-avatar FILE     # Set avatar of GitLab output projects and groups
+  --update-description  # Update description of GitLab output projects and groups automatically
 
 positional arguments:
   input_gitlab          # Input GitLab URL (default: https://gitlab.com)
-  input_group           # Input GitLab group
+  input_path            # Input GitLab group or project path
   output_gitlab         # Output GitLab URL (default: https://gitlab.com)
-  output_group          # Output GitLab group (default: input_group)
+  output_group          # Output GitLab group
 ```
 
+<!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Dependencies
 
 - [colored](https://pypi.org/project/colored/): Terminal colors and styles
```

### Comparing `gitlab_projects_migrate-1.1.0/README.md` & `gitlab_projects_migrate-2.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -39,41 +39,52 @@
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
+<!-- readme-help-start -->
 
 ```yaml
-usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--keep-members] [--overwrite]
+usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--dry-run] [--exclude-group]
+                               [--exclude-subgroups] [--exclude-projects] [--keep-members] [--overwrite]
                                [--set-avatar FILE] [--update-description]
-                               [input_gitlab] [input_group] [output_gitlab] [output_group]
+                               [input_gitlab] [input_path] [output_gitlab] [output_group]
 
-gitlab-projects-migrate: Synchronize projects from a GitLab group to another GitLab group
+gitlab-projects-migrate: Migrate GitLab projects from a GitLab group to another GitLab's group
 
 internal arguments:
   -h, --help            # Show this help message
   --version             # Show the current version
 
+credentials arguments:
+  -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
+  -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
+
 migration arguments:
-  -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN environment)
-  -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN environment or input_token)
+  --dry-run             # Enable dry run mode to check without saving
+  --exclude-group       # Exclude parent group migration
+  --exclude-subgroups   # Exclude children subgroups migration
+  --exclude-projects    # Exclude children projects migration
   --keep-members        # Keep input members after importing on output GitLab
   --overwrite           # Overwrite existing projects on output GitLab
-  --set-avatar FILE     # Set imported projects' avatar to a specific image file
-  --update-description  # Update project description automatically inside output group
+
+general settings arguments:
+  --set-avatar FILE     # Set avatar of GitLab output projects and groups
+  --update-description  # Update description of GitLab output projects and groups automatically
 
 positional arguments:
   input_gitlab          # Input GitLab URL (default: https://gitlab.com)
-  input_group           # Input GitLab group
+  input_path            # Input GitLab group or project path
   output_gitlab         # Output GitLab URL (default: https://gitlab.com)
-  output_group          # Output GitLab group (default: input_group)
+  output_group          # Output GitLab group
 ```
 
+<!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Dependencies
 
 - [colored](https://pypi.org/project/colored/): Terminal colors and styles
```

### Comparing `gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/cli/main.py` & `gitlab_projects_migrate-2.0.0/src/cli/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 #!/usr/bin/env python3
 
 # Standard libraries
 from argparse import (_ArgumentGroup, ArgumentParser, Namespace, RawTextHelpFormatter)
 from os import environ
+from shutil import get_terminal_size
 from sys import exit as sys_exit
 
 # Components
-from ..features.migration import MigrationFeature
 from ..package.bundle import Bundle
 from ..package.version import Version
 from ..prints.colors import Colors
 from ..system.platform import Platform
+from .entrypoint import Entrypoint
 
-# Main
+# Main, pylint: disable=too-many-statements
 def main() -> None:
 
     # Variables
     group: _ArgumentGroup
     result: bool = False
 
     # Arguments creation
     parser: ArgumentParser = ArgumentParser(
         prog=Bundle.NAME,
-        description=f'{Bundle.NAME}: Synchronize issues from a GitLab project to another',
-        add_help=False, formatter_class=RawTextHelpFormatter)
+        description=f'{Bundle.NAME}: {Bundle.DESCRIPTION}',
+        add_help=False,
+        formatter_class=lambda prog: RawTextHelpFormatter(
+            prog,
+            max_help_position=30,
+            width=min(
+                120,
+                get_terminal_size().columns - 2,
+            ),
+        ),
+    )
 
     # Arguments internal definitions
     group = parser.add_argument_group('internal arguments')
     group.add_argument(
         '-h',
         '--help',
         dest='help',
@@ -37,84 +47,128 @@
     group.add_argument(
         '--version',
         dest='version',
         action='store_true',
         help='Show the current version',
     )
 
-    # Arguments migration definitions
-    group = parser.add_argument_group('migration arguments')
+    # Arguments credentials definitions
+    group = parser.add_argument_group('credentials arguments')
     group.add_argument(
         '-I',
         dest='input_token',
-        default=environ.get(Bundle.ENV_GITLAB_INPUT_TOKEN, ''), #
-        help=
-        f'Input GitLab API token (default: {Bundle.ENV_GITLAB_INPUT_TOKEN} environment)')
+        default=environ.get(
+            Bundle.ENV_GITLAB_INPUT_TOKEN,
+            environ.get(
+                Bundle.ENV_GITLAB_TOKEN,
+                '',
+            ),
+        ),
+        help=f'Input GitLab API token (default: {Bundle.ENV_GITLAB_INPUT_TOKEN}'
+        f' or {Bundle.ENV_GITLAB_TOKEN} environments)',
+    )
     group.add_argument(
         '-O',
         dest='output_token',
         action='store',
-        default=environ.get(Bundle.ENV_GITLAB_OUTPUT_TOKEN, ''), #
-        help=
-        f'Output GitLab API token (default: {Bundle.ENV_GITLAB_OUTPUT_TOKEN} environment'
-        ' or input_token)')
+        default=environ.get(
+            Bundle.ENV_GITLAB_OUTPUT_TOKEN,
+            environ.get(
+                Bundle.ENV_GITLAB_TOKEN,
+                '',
+            ),
+        ), #
+        help=f'Output GitLab API token (default: {Bundle.ENV_GITLAB_OUTPUT_TOKEN}'
+        f', {Bundle.ENV_GITLAB_TOKEN} environments,'
+        ' or INPUT_TOKEN argument)',
+    )
+
+    # Arguments migration definitions
+    group = parser.add_argument_group('migration arguments')
+    group.add_argument(
+        '--dry-run',
+        dest='dry_run',
+        action='store_true',
+        help='Enable dry run mode to check without saving',
+    )
+    group.add_argument(
+        '--exclude-group',
+        dest='exclude_group',
+        action='store_true',
+        help='Exclude parent group migration',
+    )
+    group.add_argument(
+        '--exclude-subgroups',
+        dest='exclude_subgroups',
+        action='store_true',
+        help='Exclude children subgroups migration',
+    )
+    group.add_argument(
+        '--exclude-projects',
+        dest='exclude_projects',
+        action='store_true',
+        help='Exclude children projects migration',
+    )
     group.add_argument(
         '--keep-members',
         dest='keep_members',
         action='store_true',
         help='Keep input members after importing on output GitLab',
     )
     group.add_argument(
         '--overwrite',
         dest='overwrite',
         action='store_true',
         help='Overwrite existing projects on output GitLab',
     )
+
+    # Arguments general settings definitions
+    group = parser.add_argument_group('general settings arguments')
     group.add_argument(
         '--set-avatar',
         dest='set_avatar',
         action='store',
         metavar='FILE',
-        help='Set imported projects\' avatar to a specific image file',
+        help='Set avatar of GitLab output projects and groups',
     )
     group.add_argument(
         '--update-description',
         dest='update_description',
         action='store_true',
-        help='Update project description automatically inside output group',
+        help='Update description of GitLab output projects and groups automatically',
     )
 
     # Arguments positional definitions
     group = parser.add_argument_group('positional arguments')
     group.add_argument(
         dest='input_gitlab',
         action='store',
         nargs='?',
         default='https://gitlab.com',
         help='Input GitLab URL (default: https://gitlab.com)',
     )
     group.add_argument(
-        dest='input_group',
+        dest='input_path',
         action='store',
         nargs='?',
-        help='Input GitLab group',
+        help='Input GitLab group or project path',
     )
     group.add_argument(
         dest='output_gitlab',
         action='store',
         nargs='?',
         default='https://gitlab.com',
         help='Output GitLab URL (default: https://gitlab.com)',
     )
     group.add_argument(
         dest='output_group',
         action='store',
         nargs='?',
         default='',
-        help='Output GitLab group (default: input_group)',
+        help='Output GitLab group',
     )
 
     # Arguments parser
     options: Namespace = parser.parse_args()
 
     # Help informations
     if options.help:
@@ -132,33 +186,32 @@
         print(
             f'{Bundle.NAME} {Version.get()} from {Version.path()} (python {Version.python()})'
         )
         Platform.flush()
         sys_exit(0)
 
     # Arguments validation
-    if not options.input_gitlab or not options.input_group or not options.output_gitlab:
+    if not options.input_token or not options.input_gitlab or not options.input_path \
+            or not options.output_gitlab or not options.output_group:
         print(' ')
         parser.print_help()
         print(' ')
         Platform.flush()
         sys_exit(1)
 
     # Arguments adaptations
     if not options.output_token:
         options.output_token = options.input_token
-    if not options.output_group:
-        options.output_group = options.input_group
 
     # Header
     print(' ')
     Platform.flush()
 
-    # Migrate GitLab projects
-    result = MigrationFeature.gitlab_projects_migrate(options)
+    # CLI entrypoint
+    result = Entrypoint.cli(options)
 
     # Footer
     print(' ')
     Platform.flush()
 
     # Result
     if result:
```

### Comparing `gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/package/version.py` & `gitlab_projects_migrate-2.0.0/src/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/prints/colors.py` & `gitlab_projects_migrate-2.0.0/src/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/system/platform.py` & `gitlab_projects_migrate-2.0.0/src/system/platform.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/PKG-INFO` & `gitlab_projects_migrate-2.0.0/gitlab_projects_migrate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-migrate
-Version: 1.1.0
+Version: 2.0.0
 Summary: Migrate GitLab projects from a GitLab group to another GitLab's group
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-migrate
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-migrate/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-migrate/blob/main/CHANGELOG.md
@@ -73,41 +73,52 @@
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
+<!-- readme-help-start -->
 
 ```yaml
-usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--keep-members] [--overwrite]
+usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--dry-run] [--exclude-group]
+                               [--exclude-subgroups] [--exclude-projects] [--keep-members] [--overwrite]
                                [--set-avatar FILE] [--update-description]
-                               [input_gitlab] [input_group] [output_gitlab] [output_group]
+                               [input_gitlab] [input_path] [output_gitlab] [output_group]
 
-gitlab-projects-migrate: Synchronize projects from a GitLab group to another GitLab group
+gitlab-projects-migrate: Migrate GitLab projects from a GitLab group to another GitLab's group
 
 internal arguments:
   -h, --help            # Show this help message
   --version             # Show the current version
 
+credentials arguments:
+  -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
+  -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
+
 migration arguments:
-  -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN environment)
-  -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN environment or input_token)
+  --dry-run             # Enable dry run mode to check without saving
+  --exclude-group       # Exclude parent group migration
+  --exclude-subgroups   # Exclude children subgroups migration
+  --exclude-projects    # Exclude children projects migration
   --keep-members        # Keep input members after importing on output GitLab
   --overwrite           # Overwrite existing projects on output GitLab
-  --set-avatar FILE     # Set imported projects' avatar to a specific image file
-  --update-description  # Update project description automatically inside output group
+
+general settings arguments:
+  --set-avatar FILE     # Set avatar of GitLab output projects and groups
+  --update-description  # Update description of GitLab output projects and groups automatically
 
 positional arguments:
   input_gitlab          # Input GitLab URL (default: https://gitlab.com)
-  input_group           # Input GitLab group
+  input_path            # Input GitLab group or project path
   output_gitlab         # Output GitLab URL (default: https://gitlab.com)
-  output_group          # Output GitLab group (default: input_group)
+  output_group          # Output GitLab group
 ```
 
+<!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Dependencies
 
 - [colored](https://pypi.org/project/colored/): Terminal colors and styles
```

### Comparing `gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/SOURCES.txt` & `gitlab_projects_migrate-2.0.0/gitlab_projects_migrate.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 mypy.ini
 setup.py
 .chglog/CHANGELOG.tpl.md
 .chglog/changelog.sh
 .chglog/config.yml
 .vscode/extensions.json
 .vscode/settings.json
-gitlab_projects_migrate/__init__.py
-gitlab_projects_migrate/__main__.py
 gitlab_projects_migrate.egg-info/PKG-INFO
 gitlab_projects_migrate.egg-info/SOURCES.txt
 gitlab_projects_migrate.egg-info/dependency_links.txt
 gitlab_projects_migrate.egg-info/entry_points.txt
 gitlab_projects_migrate.egg-info/requires.txt
 gitlab_projects_migrate.egg-info/top_level.txt
-gitlab_projects_migrate/cli/__init__.py
-gitlab_projects_migrate/cli/main.py
-gitlab_projects_migrate/features/__init__.py
-gitlab_projects_migrate/features/gitlab.py
-gitlab_projects_migrate/features/migration.py
-gitlab_projects_migrate/package/__init__.py
-gitlab_projects_migrate/package/bundle.py
-gitlab_projects_migrate/package/version.py
-gitlab_projects_migrate/prints/__init__.py
-gitlab_projects_migrate/prints/colors.py
-gitlab_projects_migrate/system/__init__.py
-gitlab_projects_migrate/system/platform.py
 requirements/build.txt
 requirements/deploy.txt
 requirements/quality.txt
-requirements/runtime.txt
+requirements/runtime.txt
+src/__init__.py
+src/__main__.py
+src/cli/__init__.py
+src/cli/entrypoint.py
+src/cli/main.py
+src/features/__init__.py
+src/features/gitlab.py
+src/package/__init__.py
+src/package/bundle.py
+src/package/version.py
+src/prints/__init__.py
+src/prints/colors.py
+src/system/__init__.py
+src/system/platform.py
```

### Comparing `gitlab_projects_migrate-1.1.0/setup.py` & `gitlab_projects_migrate-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,38 +19,48 @@
 # Project configurations
 PROJECT_AUTHOR = 'Adrian DC'
 PROJECT_DESCRIPTION = 'Migrate GitLab projects from a GitLab group to another GitLab\'s group'
 PROJECT_EMAIL = 'radian.dc@gmail.com'
 PROJECT_KEYWORDS = 'gitlab issues sync'
 PROJECT_NAME = 'gitlab-projects-migrate'
 PROJECT_OWNER = 'AdrianDC'
-PROJECT_PACKAGE = 'gitlab-projects-migrate'
+PROJECT_PACKAGE = 'gitlab_projects_migrate'
 PROJECT_SCRIPTS = [
     'gitlab-projects-migrate = gitlab_projects_migrate.cli.main:main',
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

