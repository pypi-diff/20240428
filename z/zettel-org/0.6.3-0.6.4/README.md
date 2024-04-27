# Comparing `tmp/zettel_org-0.6.3.tar.gz` & `tmp/zettel_org-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zettel_org-0.6.3.tar", last modified: Fri Apr 19 15:39:39 2024, max compression
+gzip compressed data, was "zettel_org-0.6.4.tar", last modified: Sat Apr 27 22:41:38 2024, max compression
```

## Comparing `zettel_org-0.6.3.tar` & `zettel_org-0.6.4.tar`

### file list

```diff
@@ -1,171 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.958402 zettel_org-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.938402 zettel_org-0.6.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.938402 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/ci.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/misc.md
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/refactor.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/tests.md
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/labels.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.938402 zettel_org-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.hadolint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-19 15:39:31.000000 zettel_org-0.6.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-19 15:39:31.000000 zettel_org-0.6.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-19 15:39:31.000000 zettel_org-0.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-19 15:39:31.000000 zettel_org-0.6.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-19 15:39:31.000000 zettel_org-0.6.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-19 15:39:39.958402 zettel_org-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-19 15:39:31.000000 zettel_org-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.938402 zettel_org-0.6.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2662 2024-04-19 15:39:31.000000 zettel_org-0.6.3/bin/build_zorg_grammars
--rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-04-19 15:39:31.000000 zettel_org-0.6.3/bin/check_cc
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-19 15:39:31.000000 zettel_org-0.6.3/bin/publish_docs
--rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-19 15:39:31.000000 zettel_org-0.6.3/bin/quick-lints
--rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-04-19 15:39:31.000000 zettel_org-0.6.3/bin/render_all_cogs
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.938402 zettel_org-0.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.938402 zettel_org-0.6.3/docs/design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/design/design.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/design/design.template.md
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.942402 zettel_org-0.6.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.942402 zettel_org-0.6.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/_static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.942402 zettel_org-0.6.3/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/zorg.rst
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 15:39:31.000000 zettel_org-0.6.3/dpkg-dependencies.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.930402 zettel_org-0.6.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.942402 zettel_org-0.6.3/examples/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/20240323.zo
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/basic.zo
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/multiblocks.zo
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/priority.zo
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/property.zo
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/scrambled_prj_notes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/subnotes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/subsections.zo
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/tags_and_ids.zo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.942402 zettel_org-0.6.3/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-19 15:39:31.000000 zettel_org-0.6.3/lib/bugyi.sh
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-19 15:39:31.000000 zettel_org-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-19 15:39:31.000000 zettel_org-0.6.3/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-04-19 15:39:31.000000 zettel_org-0.6.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 15:39:31.000000 zettel_org-0.6.3/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-19 15:39:31.000000 zettel_org-0.6.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.942402 zettel_org-0.6.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 15:39:31.000000 zettel_org-0.6.3/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-19 15:39:39.958402 zettel_org-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-19 15:39:31.000000 zettel_org-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.930402 zettel_org-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.958402 zettel_org-0.6.3/src/zettel_org.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-19 15:39:39.000000 zettel_org-0.6.3/src/zettel_org.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-19 15:39:39.000000 zettel_org-0.6.3/src/zettel_org.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 15:39:39.000000 zettel_org-0.6.3/src/zettel_org.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 15:39:39.000000 zettel_org-0.6.3/src/zettel_org.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 15:39:36.000000 zettel_org-0.6.3/src/zettel_org.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-19 15:39:39.000000 zettel_org-0.6.3/src/zettel_org.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 15:39:39.000000 zettel_org-0.6.3/src/zettel_org.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.946402 zettel_org-0.6.3/src/zorg/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.946402 zettel_org-0.6.3/src/zorg/app/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.946402 zettel_org-0.6.3/src/zorg/app/runners/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/_run_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.946402 zettel_org-0.6.3/src/zorg/domain/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.946402 zettel_org-0.6.3/src/zorg/domain/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/domain/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/domain/messages/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/domain/messages/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/domain/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.950402 zettel_org-0.6.3/src/zorg/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.950402 zettel_org-0.6.3/src/zorg/grammar/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFile.g4
--rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFile.interp
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFile.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileListener.py
--rw-r--r--   0 runner    (1001) docker     (127)   118898 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.950402 zettel_org-0.6.3/src/zorg/service/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    17659 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/messagebus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/zid_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.950402 zettel_org-0.6.3/src/zorg/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.954402 zettel_org-0.6.3/src/zorg/storage/file/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/file/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/file/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.954402 zettel_org-0.6.3/src/zorg/storage/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/sql/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/sql/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/sql/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/sql/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-19 15:39:31.000000 zettel_org-0.6.3/targets.mk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.954402 zettel_org-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.954402 zettel_org-0.6.3/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    70292 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/__snapshots__/test_run_compile.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/__snapshots__/test_run_db.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/__snapshots__/test_run_edit.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/__snapshots__/test_run_template.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.958402 zettel_org-0.6.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/data/day_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/data/done_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/data/habit_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/data/hello.zot
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/data/links.zo
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_run_action_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.510029 zettel_org-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.490029 zettel_org-0.6.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.490029 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/misc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/refactor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/labels.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.490029 zettel_org-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.hadolint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-27 22:41:30.000000 zettel_org-0.6.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-27 22:41:30.000000 zettel_org-0.6.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-27 22:41:30.000000 zettel_org-0.6.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-27 22:41:30.000000 zettel_org-0.6.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-27 22:41:30.000000 zettel_org-0.6.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-27 22:41:38.510029 zettel_org-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-04-27 22:41:30.000000 zettel_org-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.490029 zettel_org-0.6.4/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2663 2024-04-27 22:41:30.000000 zettel_org-0.6.4/bin/build_zorg_grammars
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-04-27 22:41:30.000000 zettel_org-0.6.4/bin/check_cc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-27 22:41:30.000000 zettel_org-0.6.4/bin/publish_docs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-27 22:41:30.000000 zettel_org-0.6.4/bin/quick-lints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-04-27 22:41:30.000000 zettel_org-0.6.4/bin/render_all_cogs
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/docs/design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/design/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/design/design.template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/_static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/zorg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 22:41:30.000000 zettel_org-0.6.4/dpkg-dependencies.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.482029 zettel_org-0.6.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/examples/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/20240323.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/basic.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/multiblocks.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/priority.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/property.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/scrambled_prj_notes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/subnotes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/subsections.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/tags_and_ids.zo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/examples/zorg_query/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_query/all_contexts.zoq
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_query/open_projects.zoq
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-27 22:41:30.000000 zettel_org-0.6.4/lib/bugyi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-27 22:41:30.000000 zettel_org-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-27 22:41:30.000000 zettel_org-0.6.4/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-27 22:41:30.000000 zettel_org-0.6.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 22:41:30.000000 zettel_org-0.6.4/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-27 22:41:30.000000 zettel_org-0.6.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-27 22:41:30.000000 zettel_org-0.6.4/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-27 22:41:38.510029 zettel_org-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-27 22:41:30.000000 zettel_org-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.482029 zettel_org-0.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.510029 zettel_org-0.6.4/src/zettel_org.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-27 22:41:38.000000 zettel_org-0.6.4/src/zettel_org.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-27 22:41:38.000000 zettel_org-0.6.4/src/zettel_org.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:41:38.000000 zettel_org-0.6.4/src/zettel_org.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 22:41:38.000000 zettel_org-0.6.4/src/zettel_org.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:41:34.000000 zettel_org-0.6.4/src/zettel_org.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-27 22:41:38.000000 zettel_org-0.6.4/src/zettel_org.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-27 22:41:38.000000 zettel_org-0.6.4/src/zettel_org.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.498029 zettel_org-0.6.4/src/zorg/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.498029 zettel_org-0.6.4/src/zorg/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.498029 zettel_org-0.6.4/src/zorg/app/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_run_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_run_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.498029 zettel_org-0.6.4/src/zorg/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.498029 zettel_org-0.6.4/src/zorg/domain/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/messages/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/messages/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.502029 zettel_org-0.6.4/src/zorg/domain/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/models/_zorg_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/models/_zorg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.502029 zettel_org-0.6.4/src/zorg/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.502029 zettel_org-0.6.4/src/zorg/grammar/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFile.g4
+-rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFile.interp
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFile.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119519 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.502029 zettel_org-0.6.4/src/zorg/grammar/zorg_query/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQuery.g4
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQuery.interp
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQuery.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18225 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.506029 zettel_org-0.6.4/src/zorg/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.506029 zettel_org-0.6.4/src/zorg/service/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/compiler/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16902 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/compiler/_file_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/compiler/_query_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/messagebus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/zid_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.506029 zettel_org-0.6.4/src/zorg/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.506029 zettel_org-0.6.4/src/zorg/storage/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/file/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/file/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.506029 zettel_org-0.6.4/src/zorg/storage/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/sql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/sql/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/sql/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/sql/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-27 22:41:30.000000 zettel_org-0.6.4/targets.mk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.506029 zettel_org-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.510029 zettel_org-0.6.4/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    70292 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/__snapshots__/test_run_compile.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/__snapshots__/test_run_db.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/__snapshots__/test_run_edit.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/__snapshots__/test_run_template.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.510029 zettel_org-0.6.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/data/day_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/data/done_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/data/habit_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/data/hello.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/data/links.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_run_action_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tox.ini
```

### Comparing `zettel_org-0.6.3/.cruft.json` & `zettel_org-0.6.4/.cruft.json`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/.github/labels.yml` & `zettel_org-0.6.4/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/.github/workflows/ci.yml` & `zettel_org-0.6.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/.gitignore` & `zettel_org-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/.pylintrc` & `zettel_org-0.6.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/.readthedocs.yml` & `zettel_org-0.6.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/CHANGELOG.md` & `zettel_org-0.6.4/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,33 @@
 The format is based on [Keep a Changelog], and this project adheres to
 [Semantic Versioning].
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/
 
 
-## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.6.3...HEAD)
+## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.6.4...HEAD)
 
 No notable changes have been made.
 
 
+## [0.6.4](https://github.com/bbugyi200/zorg/compare/0.6.3...0.6.4) - 2024-04-27
+
+### Changed
+
+* Add `zorg query` command that does nothing ATM.
+* Stop generating ZIDs which use any of the following characters based on
+  similarity to digits OR because the lowercase letter hangs over an underline: `SQgipqy`
+
+### Fixed
+
+* Allow ZIDs and priorities in note body.
+* Strip zettel dir from sql.ZorgFile.path.
+
+
 ## [0.6.3](https://github.com/bbugyi200/zorg/compare/0.6.2...0.6.3) - 2024-04-19
 
 ### Fixed
 
 * Fix bug where absolute filename was used to key file hash. This was causing
   the file hash map to not be portable across different machines.
```

### Comparing `zettel_org-0.6.3/CONTRIBUTING.md` & `zettel_org-0.6.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/Dockerfile` & `zettel_org-0.6.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/Makefile` & `zettel_org-0.6.4/Makefile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/PKG-INFO` & `zettel_org-0.6.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.6.3
+Version: 0.6.4
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -87,24 +87,36 @@
 <!-- [[[[[kooky.cog
 import subprocess
 
 popen = subprocess.Popen(["zorg", "--help"], stdout=subprocess.PIPE)
 stdout, _ = popen.communicate()
 print("```", stdout.decode().strip(), "```", sep="\n")
 
-for cmd in ['action', 'action open', 'compile', 'db', 'db create', 'db reindex', 'edit', 'template', 'template init', 'template render']:
+for cmd in [
+    "action",
+    "action open",
+    "compile",
+    "db",
+    "db create",
+    "db reindex",
+    "edit",
+    "query",
+    "template",
+    "template init",
+    "template render",
+]:
     popen = subprocess.Popen(["zorg"] + cmd.split() + ["--help"], stdout=subprocess.PIPE)
     stdout, _ = popen.communicate()
     print(f"\n### `zorg {cmd} --help`\n")
     print("```", stdout.decode().strip(), "```", sep="\n")
 ]]]]] -->
 ```
 usage: zorg [-h] [-c CONFIG_FILE] [-L [FILE[:LEVEL][@FORMAT]]] [-v]
             [--version] [-d ZETTEL_DIR]
-            {action,compile,db,edit,template} ...
+            {action,compile,db,edit,query,template} ...
 
 The zettel note manager of the future.
 
 options:
   -c CONFIG_FILE, --config CONFIG_FILE
                         Absolute or relative path to a YAML file that contains
                         this application's configuration.
@@ -126,21 +138,22 @@
                         'nocolor']). NOTE: This option can be specified
                         multiple times and has a default argument of '+'.
   -v, --verbose         How verbose should the output be? This option can be
                         specified multiple times (e.g. -v, -vv, -vvv, ...).
   --version             show program's version number and exit
 
 subcommands:
-  {action,compile,db,edit,template}
+  {action,compile,db,edit,query,template}
     action              Used to interface with vim via an action protocol.
     compile             Compiles zorg (*.zo) files into zorc (*.zoc) files.
     db                  Commands for managing Zorg's SQL database.
     edit                Generate new day logs from templates and open the main
                         day log in your system's editor. This is the default
                         subcommand.
+    query               Run a zorg query against your zettel directory.
     template            Commands for managing .zot templates.
 ```
 
 ### `zorg action --help`
 
 ```
 usage: zorg action [-h] {open} ...
@@ -237,14 +250,28 @@
 positional arguments:
   zo_paths    The .zo files we want to open in an editor.
 
 options:
   -h, --help  show this help message and exit
 ```
 
+### `zorg query --help`
+
+```
+usage: zorg query [-h] query
+
+Run a zorg query against your zettel directory.
+
+positional arguments:
+  query       The zorg query we will run.
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ### `zorg template --help`
 
 ```
 usage: zorg template [-h] {render,init} ...
 
 Commands for managing .zot templates.
```

### Comparing `zettel_org-0.6.3/README.md` & `zettel_org-0.6.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -57,24 +57,36 @@
 <!-- [[[[[kooky.cog
 import subprocess
 
 popen = subprocess.Popen(["zorg", "--help"], stdout=subprocess.PIPE)
 stdout, _ = popen.communicate()
 print("```", stdout.decode().strip(), "```", sep="\n")
 
-for cmd in ['action', 'action open', 'compile', 'db', 'db create', 'db reindex', 'edit', 'template', 'template init', 'template render']:
+for cmd in [
+    "action",
+    "action open",
+    "compile",
+    "db",
+    "db create",
+    "db reindex",
+    "edit",
+    "query",
+    "template",
+    "template init",
+    "template render",
+]:
     popen = subprocess.Popen(["zorg"] + cmd.split() + ["--help"], stdout=subprocess.PIPE)
     stdout, _ = popen.communicate()
     print(f"\n### `zorg {cmd} --help`\n")
     print("```", stdout.decode().strip(), "```", sep="\n")
 ]]]]] -->
 ```
 usage: zorg [-h] [-c CONFIG_FILE] [-L [FILE[:LEVEL][@FORMAT]]] [-v]
             [--version] [-d ZETTEL_DIR]
-            {action,compile,db,edit,template} ...
+            {action,compile,db,edit,query,template} ...
 
 The zettel note manager of the future.
 
 options:
   -c CONFIG_FILE, --config CONFIG_FILE
                         Absolute or relative path to a YAML file that contains
                         this application's configuration.
@@ -96,21 +108,22 @@
                         'nocolor']). NOTE: This option can be specified
                         multiple times and has a default argument of '+'.
   -v, --verbose         How verbose should the output be? This option can be
                         specified multiple times (e.g. -v, -vv, -vvv, ...).
   --version             show program's version number and exit
 
 subcommands:
-  {action,compile,db,edit,template}
+  {action,compile,db,edit,query,template}
     action              Used to interface with vim via an action protocol.
     compile             Compiles zorg (*.zo) files into zorc (*.zoc) files.
     db                  Commands for managing Zorg's SQL database.
     edit                Generate new day logs from templates and open the main
                         day log in your system's editor. This is the default
                         subcommand.
+    query               Run a zorg query against your zettel directory.
     template            Commands for managing .zot templates.
 ```
 
 ### `zorg action --help`
 
 ```
 usage: zorg action [-h] {open} ...
@@ -207,14 +220,28 @@
 positional arguments:
   zo_paths    The .zo files we want to open in an editor.
 
 options:
   -h, --help  show this help message and exit
 ```
 
+### `zorg query --help`
+
+```
+usage: zorg query [-h] query
+
+Run a zorg query against your zettel directory.
+
+positional arguments:
+  query       The zorg query we will run.
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ### `zorg template --help`
 
 ```
 usage: zorg template [-h] {render,init} ...
 
 Commands for managing .zot templates.
```

### Comparing `zettel_org-0.6.3/bin/build_zorg_grammars` & `zettel_org-0.6.4/bin/build_zorg_grammars`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     if [[ "${dir}" == "_"* ]]; then
       log::debug "Skipping the %s directory." "${dir}"
       continue
     fi
 
     log::info "Generating %s parser using antlr4." $dir
     antlr4 -Dlanguage=Python3 src/zorg/grammar/$dir/*.g4
-    for f in examples/$dir/*.zo; do
+    for f in examples/$dir/*.zo*; do
       if [[ "${f}" != *"${ZO_NAME}"* ]]; then
         continue
       fi
       log::info "Contructing syntax tree from %s example file." $f
       echo "##### $f" >> $TMP_ERROR_FILE
       antlr4-parse src/zorg/grammar/$dir/*.g4 prog "${parse_cmds[@]}" $f 3>&1 1>&2 2>&3 | tee /dev/stderr >> $TMP_ERROR_FILE
       echo >> $TMP_ERROR_FILE
```

### Comparing `zettel_org-0.6.3/bin/check_cc` & `zettel_org-0.6.4/bin/check_cc`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/bin/publish_docs` & `zettel_org-0.6.4/bin/publish_docs`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/bin/quick-lints` & `zettel_org-0.6.4/bin/quick-lints`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/bin/render_all_cogs` & `zettel_org-0.6.4/bin/render_all_cogs`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/docs/Makefile` & `zettel_org-0.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/docs/make.bat` & `zettel_org-0.6.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/docs/source/conf.py` & `zettel_org-0.6.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/examples/zorg_file/20240323.zo` & `zettel_org-0.6.4/examples/zorg_file/20240323.zo`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/examples/zorg_file/scrambled_prj_notes.zo` & `zettel_org-0.6.4/examples/zorg_file/scrambled_prj_notes.zo`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/lib/bugyi.sh` & `zettel_org-0.6.4/lib/bugyi.sh`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/requirements-dev.in` & `zettel_org-0.6.4/requirements-dev.in`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/requirements-dev.txt` & `zettel_org-0.6.4/requirements-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     # via cookiecutter
 astroid==3.1.0
     # via pylint
 babel==2.14.0
     # via sphinx
 binaryornot==0.4.4
     # via cookiecutter
-black==24.4.0
+black==24.4.2
     # via -r requirements-dev.in
 bolton-clack==0.3.12
     # via
     #   -r requirements.in
     #   zettel-org
 bolton-eris==0.2.3
     # via
@@ -74,15 +74,15 @@
     #   cruft
     #   pip-tools
     #   typer
 cogapp==3.4.1
     # via -r requirements-dev.in
 cookiecutter==2.6.0
     # via cruft
-coverage[toml]==7.4.4
+coverage[toml]==7.5.0
     # via pytest-cov
 cruft[pyproject]==2.15.0
     # via -r requirements-dev.in
 dill==0.3.8
     # via pylint
 distlib==0.3.8
     # via virtualenv
@@ -95,15 +95,15 @@
     # via pytest
 filelock==3.13.4
     # via
     #   tox
     #   virtualenv
 flake8==7.0.0
     # via -r requirements-dev.in
-freezegun==1.4.0
+freezegun==1.5.0
     # via -r requirements-dev.in
 gitdb==4.0.11
     # via gitpython
 gitpython==3.1.43
     # via cruft
 greenlet==3.0.3
     # via sqlalchemy
@@ -135,15 +135,15 @@
     # via
     #   flake8
     #   pylint
 mdurl==0.1.2
     # via markdown-it-py
 mistune==0.8.4
     # via m2r2
-mypy==1.9.0
+mypy==1.10.0
     # via -r requirements-dev.in
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 packaging==24.0
     # via
@@ -153,37 +153,37 @@
     #   setuptools-scm
     #   sphinx
     #   tox
 pathspec==0.12.1
     # via black
 pip-tools==7.4.1
     # via -r requirements-dev.in
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   black
     #   pylint
     #   virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via
     #   pytest
     #   tox
 potoroo==0.6.0
     # via
     #   -r requirements.in
     #   zettel-org
 py==1.11.0
     # via tox
 pycodestyle==2.11.1
     # via flake8
-pydantic==2.7.0
+pydantic==2.7.1
     # via
     #   bolton-clack
     #   pydantic-settings
     #   sqlmodel
-pydantic-core==2.18.1
+pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
     # via bolton-clack
 pydocstyle[toml]==6.3.0
     # via -r requirements-dev.in
 pyflakes==3.2.0
     # via flake8
@@ -323,15 +323,15 @@
     #   typer
 urllib3==2.2.1
     # via requests
 vimala==0.2.0
     # via
     #   -r requirements.in
     #   zettel-org
-virtualenv==20.25.3
+virtualenv==20.26.0
     # via tox
 wheel==0.43.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==24.0
     # via pip-tools
```

### Comparing `zettel_org-0.6.3/requirements.txt` & `zettel_org-0.6.4/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,20 +38,20 @@
     # via sqlalchemy
 jinja2==3.1.3
     # via -r requirements.in
 markupsafe==2.1.5
     # via jinja2
 potoroo==0.6.0
     # via -r requirements.in
-pydantic==2.7.0
+pydantic==2.7.1
     # via
     #   bolton-clack
     #   pydantic-settings
     #   sqlmodel
-pydantic-core==2.18.1
+pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
     # via bolton-clack
 python-dotenv==1.0.1
     # via pydantic-settings
 pyyaml==6.0.1
     # via bolton-clack
```

### Comparing `zettel_org-0.6.3/setup.cfg` & `zettel_org-0.6.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 show_error_context = True
 warn_redundant_casts = True
 warn_return_any = True
 warn_unreachable = True
 warn_unused_configs = True
 warn_unused_ignores = True
 
-[mypy-zorg.service.compiler]
+[mypy-zorg.service.compiler._file_compiler]
 disallow_untyped_calls = False
 
 [mypy-zorg.grammar.*]
 follow_imports = silent
 
 [mypy-antlr4.*,pluggy.*,setuptools.*]
 ignore_missing_imports = True
```

### Comparing `zettel_org-0.6.3/setup.py` & `zettel_org-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 DESCRIPTION = "The zettel note manager of the future."
 SUPPORTED_PYTHON_VERSIONS = [
     (3, 9),
     (3, 10),
     (3, 11),
     (3, 12),
 ]
-USE_SCM_VERSION = {"fallback_version": "0.6.3"}
+USE_SCM_VERSION = {"fallback_version": "0.6.4"}
 
 
 ###############################################################################
 # Helper functions.
 ###############################################################################
 def long_description() -> str:
     """Returns the body of this project's page on PyPI."""
```

### Comparing `zettel_org-0.6.3/src/zettel_org.egg-info/PKG-INFO` & `zettel_org-0.6.4/src/zettel_org.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.6.3
+Version: 0.6.4
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -87,24 +87,36 @@
 <!-- [[[[[kooky.cog
 import subprocess
 
 popen = subprocess.Popen(["zorg", "--help"], stdout=subprocess.PIPE)
 stdout, _ = popen.communicate()
 print("```", stdout.decode().strip(), "```", sep="\n")
 
-for cmd in ['action', 'action open', 'compile', 'db', 'db create', 'db reindex', 'edit', 'template', 'template init', 'template render']:
+for cmd in [
+    "action",
+    "action open",
+    "compile",
+    "db",
+    "db create",
+    "db reindex",
+    "edit",
+    "query",
+    "template",
+    "template init",
+    "template render",
+]:
     popen = subprocess.Popen(["zorg"] + cmd.split() + ["--help"], stdout=subprocess.PIPE)
     stdout, _ = popen.communicate()
     print(f"\n### `zorg {cmd} --help`\n")
     print("```", stdout.decode().strip(), "```", sep="\n")
 ]]]]] -->
 ```
 usage: zorg [-h] [-c CONFIG_FILE] [-L [FILE[:LEVEL][@FORMAT]]] [-v]
             [--version] [-d ZETTEL_DIR]
-            {action,compile,db,edit,template} ...
+            {action,compile,db,edit,query,template} ...
 
 The zettel note manager of the future.
 
 options:
   -c CONFIG_FILE, --config CONFIG_FILE
                         Absolute or relative path to a YAML file that contains
                         this application's configuration.
@@ -126,21 +138,22 @@
                         'nocolor']). NOTE: This option can be specified
                         multiple times and has a default argument of '+'.
   -v, --verbose         How verbose should the output be? This option can be
                         specified multiple times (e.g. -v, -vv, -vvv, ...).
   --version             show program's version number and exit
 
 subcommands:
-  {action,compile,db,edit,template}
+  {action,compile,db,edit,query,template}
     action              Used to interface with vim via an action protocol.
     compile             Compiles zorg (*.zo) files into zorc (*.zoc) files.
     db                  Commands for managing Zorg's SQL database.
     edit                Generate new day logs from templates and open the main
                         day log in your system's editor. This is the default
                         subcommand.
+    query               Run a zorg query against your zettel directory.
     template            Commands for managing .zot templates.
 ```
 
 ### `zorg action --help`
 
 ```
 usage: zorg action [-h] {open} ...
@@ -237,14 +250,28 @@
 positional arguments:
   zo_paths    The .zo files we want to open in an editor.
 
 options:
   -h, --help  show this help message and exit
 ```
 
+### `zorg query --help`
+
+```
+usage: zorg query [-h] query
+
+Run a zorg query against your zettel directory.
+
+positional arguments:
+  query       The zorg query we will run.
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ### `zorg template --help`
 
 ```
 usage: zorg template [-h] {render,init} ...
 
 Commands for managing .zot templates.
```

### Comparing `zettel_org-0.6.3/src/zettel_org.egg-info/SOURCES.txt` & `zettel_org-0.6.4/src/zettel_org.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 examples/zorg_file/multiblocks.zo
 examples/zorg_file/priority.zo
 examples/zorg_file/property.zo
 examples/zorg_file/scrambled_prj_notes.zo
 examples/zorg_file/subnotes.zo
 examples/zorg_file/subsections.zo
 examples/zorg_file/tags_and_ids.zo
+examples/zorg_query/all_contexts.zoq
+examples/zorg_query/open_projects.zoq
 lib/bugyi.sh
 scripts/README.md
 src/zettel_org.egg-info/PKG-INFO
 src/zettel_org.egg-info/SOURCES.txt
 src/zettel_org.egg-info/dependency_links.txt
 src/zettel_org.egg-info/entry_points.txt
 src/zettel_org.egg-info/not-zip-safe
@@ -79,40 +81,55 @@
 src/zorg/app/__main__.py
 src/zorg/app/config.py
 src/zorg/app/runners/__init__.py
 src/zorg/app/runners/_run_action.py
 src/zorg/app/runners/_run_compile.py
 src/zorg/app/runners/_run_db.py
 src/zorg/app/runners/_run_edit.py
+src/zorg/app/runners/_run_query.py
 src/zorg/app/runners/_run_template.py
 src/zorg/app/runners/_runners.py
 src/zorg/domain/__init__.py
-src/zorg/domain/models.py
 src/zorg/domain/types.py
 src/zorg/domain/messages/__init__.py
 src/zorg/domain/messages/commands.py
 src/zorg/domain/messages/events.py
+src/zorg/domain/models/__init__.py
+src/zorg/domain/models/_zorg_file.py
+src/zorg/domain/models/_zorg_query.py
 src/zorg/grammar/__init__.py
 src/zorg/grammar/zorg_file/ZorgFile.g4
 src/zorg/grammar/zorg_file/ZorgFile.interp
 src/zorg/grammar/zorg_file/ZorgFile.tokens
 src/zorg/grammar/zorg_file/ZorgFileLexer.interp
 src/zorg/grammar/zorg_file/ZorgFileLexer.py
 src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
 src/zorg/grammar/zorg_file/ZorgFileListener.py
 src/zorg/grammar/zorg_file/ZorgFileParser.py
 src/zorg/grammar/zorg_file/__init__.py
+src/zorg/grammar/zorg_query/ZorgQuery.g4
+src/zorg/grammar/zorg_query/ZorgQuery.interp
+src/zorg/grammar/zorg_query/ZorgQuery.tokens
+src/zorg/grammar/zorg_query/ZorgQueryLexer.interp
+src/zorg/grammar/zorg_query/ZorgQueryLexer.py
+src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens
+src/zorg/grammar/zorg_query/ZorgQueryListener.py
+src/zorg/grammar/zorg_query/ZorgQueryParser.py
+src/zorg/grammar/zorg_query/__init__.py
 src/zorg/service/__init__.py
 src/zorg/service/common.py
-src/zorg/service/compiler.py
 src/zorg/service/file_groups.py
 src/zorg/service/handlers.py
 src/zorg/service/messagebus.py
 src/zorg/service/templates.py
 src/zorg/service/zid_manager.py
+src/zorg/service/compiler/__init__.py
+src/zorg/service/compiler/_api.py
+src/zorg/service/compiler/_file_compiler.py
+src/zorg/service/compiler/_query_compiler.py
 src/zorg/storage/__init__.py
 src/zorg/storage/file/__init__.py
 src/zorg/storage/file/repo.py
 src/zorg/storage/file/session.py
 src/zorg/storage/sql/__init__.py
 src/zorg/storage/sql/converters.py
 src/zorg/storage/sql/engine.py
```

### Comparing `zettel_org-0.6.3/src/zorg/app/config.py` & `zettel_org-0.6.4/src/zorg/app/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .. import APP_NAME
 from ..domain.types import FileGroupMapType, TemplatePatternMapType, VarMapType
 from ..service import common
 
 
 Command = Literal[
-    "compile", "create", "edit", "init", "open", "reindex", "render"
+    "compile", "create", "edit", "init", "open", "query", "reindex", "render"
 ]
 
 _logger = Logger(__name__)
 
 _DEFAULT_ZETTEL_DIR: Final[Path] = Path.home() / "org"
 
 
@@ -64,15 +64,15 @@
 
 
 class DbReindexConfig(Config):
     """Clack config for the 'db reindex' command."""
 
     command: Literal["reindex"]
 
-    # ----- Arguments
+    # ----- ARGUMENTS
     paths: list[Path] = []
 
 
 class EditConfig(Config):
     """Clack config for the 'edit' command."""
 
     command: Literal["edit"]
@@ -82,14 +82,23 @@
 
     # ----- CONFIG
     file_group_map: FileGroupMapType = {}
     keep_alive_file: Path = Path("/tmp/zorg_keep_alive")
     vim_commands: list[str] = []
 
 
+class QueryConfig(Config):
+    """Clack config for the 'query' command."""
+
+    command: Literal["query"]
+
+    # ----- ARGUMENTS
+    query: str
+
+
 class TemplateRenderConfig(Config):
     """Clack config for the 'template' command."""
 
     command: Literal["render"]
 
     # ----- ARGUMENTS
     template: Path
@@ -207,14 +216,20 @@
     edit_parser.add_argument(
         "zo_paths",
         type=Path,
         nargs="*",
         help="The .zo files we want to open in an editor.",
     )
 
+    # --- 'query' command
+    query_parser = new_command(
+        "query", help="Run a zorg query against your zettel directory."
+    )
+    query_parser.add_argument("query", help="The zorg query we will run.")
+
     # --- 'template' command
     template_parser = new_command(
         "template", help="Commands for managing .zot templates."
     )
     new_template_command = clack.new_command_factory(template_parser)
     # --- 'template render' command
     template_render_parser = new_template_command(
```

### Comparing `zettel_org-0.6.3/src/zorg/app/runners/__init__.py` & `zettel_org-0.6.4/src/zorg/app/runners/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """Contains this project's clack runners.
 
 WARNING: This package should contain modules of the form _runners.py or
          _run_*.py ONLY. Do NOT be tempted to add other libraries to this
          package even if they are only used by runners.
 """
 
-from . import _run_action, _run_compile, _run_db, _run_edit, _run_template
+from . import (
+    _run_action,
+    _run_compile,
+    _run_db,
+    _run_edit,
+    _run_query,
+    _run_template,
+)
 from ._runners import RUNNERS
 
 
 # HACK: It is necessary that we import these runner modules so the '@runner'
 # decorator registers functions as runners.
-del _run_action, _run_compile, _run_db, _run_edit, _run_template
+del _run_action, _run_compile, _run_db, _run_edit, _run_query, _run_template
 
 __all__ = ["RUNNERS"]
```

### Comparing `zettel_org-0.6.3/src/zorg/app/runners/_run_action.py` & `zettel_org-0.6.4/src/zorg/app/runners/_run_action.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/app/runners/_run_compile.py` & `zettel_org-0.6.4/src/zorg/app/runners/_run_compile.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/app/runners/_run_db.py` & `zettel_org-0.6.4/src/zorg/app/runners/_run_db.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/app/runners/_run_edit.py` & `zettel_org-0.6.4/src/zorg/app/runners/_run_edit.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/app/runners/_run_template.py` & `zettel_org-0.6.4/src/zorg/app/runners/_run_template.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/domain/messages/commands.py` & `zettel_org-0.6.4/src/zorg/domain/messages/commands.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/domain/messages/events.py` & `zettel_org-0.6.4/src/zorg/domain/messages/events.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/domain/models.py` & `zettel_org-0.6.4/src/zorg/domain/models/_zorg_query.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,34 @@
-"""This file contains Zorg's domain model classes."""
+"""Contains the ZorgQuery Domain entity."""
 
 from dataclasses import dataclass, field
 import datetime as dt
-from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, Optional
+from typing import Iterable, Optional
 
-from .types import (
+from ..types import (
     DescOperator,
     PropertyOperator,
     PropertyValueType,
+    Select,
     TodoPriorityType,
-    TodoStatus,
 )
 
 
-if TYPE_CHECKING:
-    from .messages.events import Event
-
-
-@dataclass(frozen=True)
-class TodoPayload:
-    """Extra fields that are added to ZorgNotes that are todos."""
-
-    priority: TodoPriorityType = "C"
-    status: TodoStatus = TodoStatus.OPEN
-
-
-@dataclass
-class ZorgNote:
-    """A Zorg note."""
-
-    body: str
-
-    areas: list[str] = field(default_factory=lambda: [])
-    child_note_ids: list[int] = field(default_factory=lambda: [])
-    contexts: list[str] = field(default_factory=lambda: [])
-    create_date: dt.date = field(default_factory=dt.date.today)
-    line_no: Optional[int] = None
-    links: list[str] = field(default_factory=lambda: [])
-    next_note_id: Optional[int] = None
-    parent_note_id: Optional[int] = None
-    people: list[str] = field(default_factory=lambda: [])
-    prev_note_id: Optional[int] = None
-    projects: list[str] = field(default_factory=lambda: [])
-    properties: dict[str, str] = field(default_factory=lambda: {})
-    todo_payload: Optional[TodoPayload] = None
-    zid: Optional[str] = None
-
-
-@dataclass
-class ZorgFile:
-    """A Zorg (i.e. *.zo) file."""
-
-    path: Path
-    has_errors: bool = False
-    notes: list[ZorgNote] = field(default_factory=lambda: [])
-    events: list["Event"] = field(default_factory=lambda: [])
-
-
 @dataclass(frozen=True)
 class DescFilter:
     """Represents a description query filter (e.g. '"foo"' or '!"bar"')."""
 
     value: str
     case_sensitive: Optional[bool] = None
     op: DescOperator = DescOperator.CONTAINS
 
 
 @dataclass(frozen=True)
 class PropertyFilter:
-    """Represents a single property filter (e.g. 'due<=0d' or '!recur')."""
+    """Represents a single property filter (e.g. 'due:<=0d' or '!recur:*')."""
 
     key: str
     value: str = ""
     op: PropertyOperator = PropertyOperator.EXISTS
     value_type: PropertyValueType = PropertyValueType.STRING
 
 
@@ -82,26 +37,42 @@
     """Represents a range of dates."""
 
     start: dt.date
     end: Optional[dt.date] = None
 
 
 @dataclass
-class AndZorgQuery:
+class WhereAndFilter:
     """Tag used to filter ZorgNotes."""
 
     areas: list[str] = field(default_factory=list)
     contexts: list[str] = field(default_factory=list)
     create_date_ranges: list[DateRange] = field(default_factory=list)
     desc_filters: list[DescFilter] = field(default_factory=list)
     done: Optional[bool] = None
-    done_date_ranges: list[DateRange] = field(default_factory=list)
+    modify_date_ranges: list[DateRange] = field(default_factory=list)
+    or_filters: list["WhereOrFilter"] = field(default_factory=list)
+    people: list[str] = field(default_factory=list)
     property_filters: list[PropertyFilter] = field(default_factory=list)
     priorities: list[TodoPriorityType] = field(default_factory=list)
     projects: list[str] = field(default_factory=list)
 
 
 @dataclass(frozen=True)
-class OrZorgQuery:
-    """A collection of `AndZorgQuery`s that have been ORed together."""
+class WhereOrFilter:
+    """A collection of `WhereAndFilter`s that have been ORed together."""
+
+    and_queries: Iterable[WhereAndFilter]
+
+
+@dataclass(frozen=True)
+class ZorgQuery:
+    """A zorg query that uses SWOG syntax.
+
+    (S)ELECT
+    (W)HERE
+    (O)RDER BY
+    (G)ROUP BY
+    """
 
-    and_queries: Iterable[AndZorgQuery]
+    select: Select = field(default=Select.NOTES)
+    where: Optional[WhereOrFilter] = None
```

### Comparing `zettel_org-0.6.3/src/zorg/domain/types.py` & `zettel_org-0.6.4/src/zorg/domain/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,21 @@
 class DescOperator(enum.Enum):
     """Used to determine the type of description constraint specified."""
 
     CONTAINS = enum.auto()
     NOT_CONTAINS = enum.auto()
 
 
+class Select(enum.Enum):
+    """A zorg query (S)ELECT."""
+
+    NOTES = enum.auto()
+    PROJECTS = enum.auto()
+
+
 class PropertyOperator(enum.Enum):
     """Used to determine what kind of metatag constraint has been specified."""
 
     # exists / not exists
     EXISTS = enum.auto()
     NOT_EXISTS = enum.auto()
```

### Comparing `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFile.g4` & `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFile.g4`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 // Zorg YYMMDD#XX IDs
 zid : ZID ;
 
 // atoms
 space_atoms : space_atom+ ;
 space_atom  : SPACE (SQUOTE non_tag_symbol)? (non_tag_symbol | DQUOTE)* (atom | quoted)? (any_symbol (any_symbol | id)*)? ref? ;
-atom        : tag_symbol | tag | link | property | id_group | ref ;
+atom        : tag_symbol | tag | link | property | id_group | ref | zid | priority ;
 
 // property
 property    : ID COLON COLON id_group ;
 id_group    : id (id_symbol+ id)* ;
 id          : ID | NUM_ID | date | time | LOWER_O | LOWER_X ;
 date        : DATE ;
 time        : TIME ;
```

### Comparing `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFile.interp` & `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFile.interp`

 * *Files 2% similar despite different names*

```diff
@@ -121,8 +121,8 @@
 h2_header
 h3_header
 h4_header
 eol
 
 
 atn:
-[4, 1, 35, 468, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 2, 43, 7, 43, 2, 44, 7, 44, 2, 45, 7, 45, 2, 46, 7, 46, 1, 0, 1, 0, 4, 0, 97, 8, 0, 11, 0, 12, 0, 98, 1, 0, 5, 0, 102, 8, 0, 10, 0, 12, 0, 105, 9, 0, 1, 0, 5, 0, 108, 8, 0, 10, 0, 12, 0, 111, 9, 0, 1, 0, 5, 0, 114, 8, 0, 10, 0, 12, 0, 117, 9, 0, 3, 0, 119, 8, 0, 1, 0, 1, 0, 1, 1, 4, 1, 124, 8, 1, 11, 1, 12, 1, 125, 1, 2, 1, 2, 3, 2, 130, 8, 2, 1, 2, 1, 2, 1, 3, 4, 3, 135, 8, 3, 11, 3, 12, 3, 136, 1, 3, 5, 3, 140, 8, 3, 10, 3, 12, 3, 143, 9, 3, 1, 4, 1, 4, 1, 4, 1, 4, 3, 4, 149, 8, 4, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 6, 1, 6, 1, 6, 5, 6, 159, 8, 6, 10, 6, 12, 6, 162, 9, 6, 1, 7, 1, 7, 1, 7, 1, 8, 1, 8, 3, 8, 169, 8, 8, 1, 8, 1, 8, 1, 9, 1, 9, 1, 9, 4, 9, 176, 8, 9, 11, 9, 12, 9, 177, 1, 9, 5, 9, 181, 8, 9, 10, 9, 12, 9, 184, 9, 9, 1, 10, 1, 10, 1, 10, 5, 10, 189, 8, 10, 10, 10, 12, 10, 192, 9, 10, 1, 11, 1, 11, 1, 11, 1, 12, 1, 12, 5, 12, 199, 8, 12, 10, 12, 12, 12, 202, 9, 12, 1, 13, 1, 13, 1, 13, 3, 13, 207, 8, 13, 1, 13, 1, 13, 1, 13, 1, 14, 1, 14, 1, 14, 1, 14, 3, 14, 216, 8, 14, 1, 15, 1, 15, 1, 15, 3, 15, 221, 8, 15, 1, 16, 1, 16, 1, 16, 1, 16, 1, 16, 1, 17, 1, 17, 1, 18, 4, 18, 231, 8, 18, 11, 18, 12, 18, 232, 1, 19, 1, 19, 1, 19, 3, 19, 238, 8, 19, 1, 19, 1, 19, 5, 19, 242, 8, 19, 10, 19, 12, 19, 245, 9, 19, 1, 19, 1, 19, 3, 19, 249, 8, 19, 1, 19, 1, 19, 1, 19, 5, 19, 254, 8, 19, 10, 19, 12, 19, 257, 9, 19, 3, 19, 259, 8, 19, 1, 19, 3, 19, 262, 8, 19, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 3, 20, 270, 8, 20, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 22, 1, 22, 4, 22, 279, 8, 22, 11, 22, 12, 22, 280, 1, 22, 1, 22, 5, 22, 285, 8, 22, 10, 22, 12, 22, 288, 9, 22, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 3, 23, 296, 8, 23, 1, 24, 1, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 26, 1, 26, 1, 26, 3, 26, 307, 8, 26, 1, 27, 1, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 30, 1, 30, 3, 30, 319, 8, 30, 1, 31, 1, 31, 1, 31, 1, 32, 1, 32, 1, 32, 1, 33, 1, 33, 1, 33, 1, 34, 1, 34, 1, 34, 1, 35, 1, 35, 1, 35, 1, 35, 1, 35, 4, 35, 338, 8, 35, 11, 35, 12, 35, 339, 1, 35, 1, 35, 1, 35, 4, 35, 345, 8, 35, 11, 35, 12, 35, 346, 1, 35, 1, 35, 3, 35, 351, 8, 35, 1, 36, 1, 36, 1, 36, 1, 36, 1, 37, 1, 37, 1, 37, 1, 37, 1, 38, 1, 38, 5, 38, 363, 8, 38, 10, 38, 12, 38, 366, 9, 38, 1, 38, 5, 38, 369, 8, 38, 10, 38, 12, 38, 372, 9, 38, 1, 38, 3, 38, 375, 8, 38, 1, 38, 5, 38, 378, 8, 38, 10, 38, 12, 38, 381, 9, 38, 1, 39, 1, 39, 5, 39, 385, 8, 39, 10, 39, 12, 39, 388, 9, 39, 1, 39, 5, 39, 391, 8, 39, 10, 39, 12, 39, 394, 9, 39, 1, 39, 3, 39, 397, 8, 39, 1, 39, 5, 39, 400, 8, 39, 10, 39, 12, 39, 403, 9, 39, 1, 40, 1, 40, 5, 40, 407, 8, 40, 10, 40, 12, 40, 410, 9, 40, 1, 40, 5, 40, 413, 8, 40, 10, 40, 12, 40, 416, 9, 40, 1, 40, 3, 40, 419, 8, 40, 1, 40, 5, 40, 422, 8, 40, 10, 40, 12, 40, 425, 9, 40, 1, 41, 1, 41, 5, 41, 429, 8, 41, 10, 41, 12, 41, 432, 9, 41, 1, 41, 5, 41, 435, 8, 41, 10, 41, 12, 41, 438, 9, 41, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 43, 1, 43, 1, 43, 1, 43, 1, 44, 1, 44, 1, 44, 1, 44, 1, 45, 1, 45, 1, 45, 1, 45, 1, 45, 1, 45, 1, 46, 1, 46, 1, 46, 0, 0, 47, 0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 0, 5, 2, 0, 9, 9, 32, 32, 4, 0, 17, 17, 21, 21, 24, 25, 32, 35, 2, 0, 18, 20, 22, 22, 1, 0, 26, 29, 1, 1, 7, 7, 492, 0, 94, 1, 0, 0, 0, 2, 123, 1, 0, 0, 0, 4, 127, 1, 0, 0, 0, 6, 134, 1, 0, 0, 0, 8, 148, 1, 0, 0, 0, 10, 150, 1, 0, 0, 0, 12, 155, 1, 0, 0, 0, 14, 163, 1, 0, 0, 0, 16, 168, 1, 0, 0, 0, 18, 172, 1, 0, 0, 0, 20, 185, 1, 0, 0, 0, 22, 193, 1, 0, 0, 0, 24, 196, 1, 0, 0, 0, 26, 203, 1, 0, 0, 0, 28, 215, 1, 0, 0, 0, 30, 217, 1, 0, 0, 0, 32, 222, 1, 0, 0, 0, 34, 227, 1, 0, 0, 0, 36, 230, 1, 0, 0, 0, 38, 234, 1, 0, 0, 0, 40, 269, 1, 0, 0, 0, 42, 271, 1, 0, 0, 0, 44, 276, 1, 0, 0, 0, 46, 295, 1, 0, 0, 0, 48, 297, 1, 0, 0, 0, 50, 299, 1, 0, 0, 0, 52, 306, 1, 0, 0, 0, 54, 308, 1, 0, 0, 0, 56, 310, 1, 0, 0, 0, 58, 312, 1, 0, 0, 0, 60, 318, 1, 0, 0, 0, 62, 320, 1, 0, 0, 0, 64, 323, 1, 0, 0, 0, 66, 326, 1, 0, 0, 0, 68, 329, 1, 0, 0, 0, 70, 350, 1, 0, 0, 0, 72, 352, 1, 0, 0, 0, 74, 356, 1, 0, 0, 0, 76, 360, 1, 0, 0, 0, 78, 382, 1, 0, 0, 0, 80, 404, 1, 0, 0, 0, 82, 426, 1, 0, 0, 0, 84, 439, 1, 0, 0, 0, 86, 451, 1, 0, 0, 0, 88, 455, 1, 0, 0, 0, 90, 459, 1, 0, 0, 0, 92, 465, 1, 0, 0, 0, 94, 118, 3, 2, 1, 0, 95, 97, 5, 7, 0, 0, 96, 95, 1, 0, 0, 0, 97, 98, 1, 0, 0, 0, 98, 96, 1, 0, 0, 0, 98, 99, 1, 0, 0, 0, 99, 103, 1, 0, 0, 0, 100, 102, 3, 6, 3, 0, 101, 100, 1, 0, 0, 0, 102, 105, 1, 0, 0, 0, 103, 101, 1, 0, 0, 0, 103, 104, 1, 0, 0, 0, 104, 109, 1, 0, 0, 0, 105, 103, 1, 0, 0, 0, 106, 108, 3, 78, 39, 0, 107, 106, 1, 0, 0, 0, 108, 111, 1, 0, 0, 0, 109, 107, 1, 0, 0, 0, 109, 110, 1, 0, 0, 0, 110, 115, 1, 0, 0, 0, 111, 109, 1, 0, 0, 0, 112, 114, 3, 76, 38, 0, 113, 112, 1, 0, 0, 0, 114, 117, 1, 0, 0, 0, 115, 113, 1, 0, 0, 0, 115, 116, 1, 0, 0, 0, 116, 119, 1, 0, 0, 0, 117, 115, 1, 0, 0, 0, 118, 96, 1, 0, 0, 0, 118, 119, 1, 0, 0, 0, 119, 120, 1, 0, 0, 0, 120, 121, 5, 0, 0, 1, 121, 1, 1, 0, 0, 0, 122, 124, 3, 4, 2, 0, 123, 122, 1, 0, 0, 0, 124, 125, 1, 0, 0, 0, 125, 123, 1, 0, 0, 0, 125, 126, 1, 0, 0, 0, 126, 3, 1, 0, 0, 0, 127, 129, 5, 26, 0, 0, 128, 130, 3, 36, 18, 0, 129, 128, 1, 0, 0, 0, 129, 130, 1, 0, 0, 0, 130, 131, 1, 0, 0, 0, 131, 132, 5, 7, 0, 0, 132, 5, 1, 0, 0, 0, 133, 135, 3, 8, 4, 0, 134, 133, 1, 0, 0, 0, 135, 136, 1, 0, 0, 0, 136, 134, 1, 0, 0, 0, 136, 137, 1, 0, 0, 0, 137, 141, 1, 0, 0, 0, 138, 140, 5, 7, 0, 0, 139, 138, 1, 0, 0, 0, 140, 143, 1, 0, 0, 0, 141, 139, 1, 0, 0, 0, 141, 142, 1, 0, 0, 0, 142, 7, 1, 0, 0, 0, 143, 141, 1, 0, 0, 0, 144, 149, 3, 24, 12, 0, 145, 149, 3, 12, 6, 0, 146, 149, 3, 10, 5, 0, 147, 149, 3, 4, 2, 0, 148, 144, 1, 0, 0, 0, 148, 145, 1, 0, 0, 0, 148, 146, 1, 0, 0, 0, 148, 147, 1, 0, 0, 0, 149, 9, 1, 0, 0, 0, 150, 151, 3, 74, 37, 0, 151, 152, 5, 22, 0, 0, 152, 153, 3, 36, 18, 0, 153, 154, 5, 7, 0, 0, 154, 11, 1, 0, 0, 0, 155, 156, 5, 18, 0, 0, 156, 160, 3, 14, 7, 0, 157, 159, 3, 20, 10, 0, 158, 157, 1, 0, 0, 0, 159, 162, 1, 0, 0, 0, 160, 158, 1, 0, 0, 0, 160, 161, 1, 0, 0, 0, 161, 13, 1, 0, 0, 0, 162, 160, 1, 0, 0, 0, 163, 164, 3, 16, 8, 0, 164, 165, 5, 7, 0, 0, 165, 15, 1, 0, 0, 0, 166, 167, 5, 23, 0, 0, 167, 169, 3, 34, 17, 0, 168, 166, 1, 0, 0, 0, 168, 169, 1, 0, 0, 0, 169, 170, 1, 0, 0, 0, 170, 171, 3, 18, 9, 0, 171, 17, 1, 0, 0, 0, 172, 182, 3, 36, 18, 0, 173, 175, 5, 7, 0, 0, 174, 176, 5, 23, 0, 0, 175, 174, 1, 0, 0, 0, 176, 177, 1, 0, 0, 0, 177, 175, 1, 0, 0, 0, 177, 178, 1, 0, 0, 0, 178, 179, 1, 0, 0, 0, 179, 181, 3, 36, 18, 0, 180, 173, 1, 0, 0, 0, 181, 184, 1, 0, 0, 0, 182, 180, 1, 0, 0, 0, 182, 183, 1, 0, 0, 0, 183, 19, 1, 0, 0, 0, 184, 182, 1, 0, 0, 0, 185, 186, 5, 15, 0, 0, 186, 190, 3, 14, 7, 0, 187, 189, 3, 22, 11, 0, 188, 187, 1, 0, 0, 0, 189, 192, 1, 0, 0, 0, 190, 188, 1, 0, 0, 0, 190, 191, 1, 0, 0, 0, 191, 21, 1, 0, 0, 0, 192, 190, 1, 0, 0, 0, 193, 194, 5, 16, 0, 0, 194, 195, 3, 14, 7, 0, 195, 23, 1, 0, 0, 0, 196, 200, 3, 26, 13, 0, 197, 199, 3, 20, 10, 0, 198, 197, 1, 0, 0, 0, 199, 202, 1, 0, 0, 0, 200, 198, 1, 0, 0, 0, 200, 201, 1, 0, 0, 0, 201, 25, 1, 0, 0, 0, 202, 200, 1, 0, 0, 0, 203, 206, 3, 28, 14, 0, 204, 205, 5, 23, 0, 0, 205, 207, 3, 32, 16, 0, 206, 204, 1, 0, 0, 0, 206, 207, 1, 0, 0, 0, 207, 208, 1, 0, 0, 0, 208, 209, 3, 16, 8, 0, 209, 210, 5, 7, 0, 0, 210, 27, 1, 0, 0, 0, 211, 216, 5, 8, 0, 0, 212, 216, 3, 30, 15, 0, 213, 216, 5, 34, 0, 0, 214, 216, 5, 35, 0, 0, 215, 211, 1, 0, 0, 0, 215, 212, 1, 0, 0, 0, 215, 213, 1, 0, 0, 0, 215, 214, 1, 0, 0, 0, 216, 29, 1, 0, 0, 0, 217, 220, 7, 0, 0, 0, 218, 219, 5, 22, 0, 0, 219, 221, 3, 50, 25, 0, 220, 218, 1, 0, 0, 0, 220, 221, 1, 0, 0, 0, 221, 31, 1, 0, 0, 0, 222, 223, 5, 1, 0, 0, 223, 224, 5, 26, 0, 0, 224, 225, 5, 10, 0, 0, 225, 226, 5, 2, 0, 0, 226, 33, 1, 0, 0, 0, 227, 228, 5, 13, 0, 0, 228, 35, 1, 0, 0, 0, 229, 231, 3, 38, 19, 0, 230, 229, 1, 0, 0, 0, 231, 232, 1, 0, 0, 0, 232, 230, 1, 0, 0, 0, 232, 233, 1, 0, 0, 0, 233, 37, 1, 0, 0, 0, 234, 237, 5, 23, 0, 0, 235, 236, 5, 30, 0, 0, 236, 238, 3, 54, 27, 0, 237, 235, 1, 0, 0, 0, 237, 238, 1, 0, 0, 0, 238, 243, 1, 0, 0, 0, 239, 242, 3, 54, 27, 0, 240, 242, 5, 31, 0, 0, 241, 239, 1, 0, 0, 0, 241, 240, 1, 0, 0, 0, 242, 245, 1, 0, 0, 0, 243, 241, 1, 0, 0, 0, 243, 244, 1, 0, 0, 0, 244, 248, 1, 0, 0, 0, 245, 243, 1, 0, 0, 0, 246, 249, 3, 40, 20, 0, 247, 249, 3, 70, 35, 0, 248, 246, 1, 0, 0, 0, 248, 247, 1, 0, 0, 0, 248, 249, 1, 0, 0, 0, 249, 258, 1, 0, 0, 0, 250, 255, 3, 52, 26, 0, 251, 254, 3, 52, 26, 0, 252, 254, 3, 46, 23, 0, 253, 251, 1, 0, 0, 0, 253, 252, 1, 0, 0, 0, 254, 257, 1, 0, 0, 0, 255, 253, 1, 0, 0, 0, 255, 256, 1, 0, 0, 0, 256, 259, 1, 0, 0, 0, 257, 255, 1, 0, 0, 0, 258, 250, 1, 0, 0, 0, 258, 259, 1, 0, 0, 0, 259, 261, 1, 0, 0, 0, 260, 262, 3, 74, 37, 0, 261, 260, 1, 0, 0, 0, 261, 262, 1, 0, 0, 0, 262, 39, 1, 0, 0, 0, 263, 270, 3, 58, 29, 0, 264, 270, 3, 60, 30, 0, 265, 270, 3, 72, 36, 0, 266, 270, 3, 42, 21, 0, 267, 270, 3, 44, 22, 0, 268, 270, 3, 74, 37, 0, 269, 263, 1, 0, 0, 0, 269, 264, 1, 0, 0, 0, 269, 265, 1, 0, 0, 0, 269, 266, 1, 0, 0, 0, 269, 267, 1, 0, 0, 0, 269, 268, 1, 0, 0, 0, 270, 41, 1, 0, 0, 0, 271, 272, 5, 10, 0, 0, 272, 273, 5, 22, 0, 0, 273, 274, 5, 22, 0, 0, 274, 275, 3, 44, 22, 0, 275, 43, 1, 0, 0, 0, 276, 286, 3, 46, 23, 0, 277, 279, 3, 56, 28, 0, 278, 277, 1, 0, 0, 0, 279, 280, 1, 0, 0, 0, 280, 278, 1, 0, 0, 0, 280, 281, 1, 0, 0, 0, 281, 282, 1, 0, 0, 0, 282, 283, 3, 46, 23, 0, 283, 285, 1, 0, 0, 0, 284, 278, 1, 0, 0, 0, 285, 288, 1, 0, 0, 0, 286, 284, 1, 0, 0, 0, 286, 287, 1, 0, 0, 0, 287, 45, 1, 0, 0, 0, 288, 286, 1, 0, 0, 0, 289, 296, 5, 10, 0, 0, 290, 296, 5, 14, 0, 0, 291, 296, 3, 48, 24, 0, 292, 296, 3, 50, 25, 0, 293, 296, 5, 8, 0, 0, 294, 296, 5, 9, 0, 0, 295, 289, 1, 0, 0, 0, 295, 290, 1, 0, 0, 0, 295, 291, 1, 0, 0, 0, 295, 292, 1, 0, 0, 0, 295, 293, 1, 0, 0, 0, 295, 294, 1, 0, 0, 0, 296, 47, 1, 0, 0, 0, 297, 298, 5, 11, 0, 0, 298, 49, 1, 0, 0, 0, 299, 300, 5, 12, 0, 0, 300, 51, 1, 0, 0, 0, 301, 307, 5, 30, 0, 0, 302, 307, 5, 31, 0, 0, 303, 307, 3, 54, 27, 0, 304, 307, 3, 58, 29, 0, 305, 307, 3, 56, 28, 0, 306, 301, 1, 0, 0, 0, 306, 302, 1, 0, 0, 0, 306, 303, 1, 0, 0, 0, 306, 304, 1, 0, 0, 0, 306, 305, 1, 0, 0, 0, 307, 53, 1, 0, 0, 0, 308, 309, 7, 1, 0, 0, 309, 55, 1, 0, 0, 0, 310, 311, 7, 2, 0, 0, 311, 57, 1, 0, 0, 0, 312, 313, 7, 3, 0, 0, 313, 59, 1, 0, 0, 0, 314, 319, 3, 62, 31, 0, 315, 319, 3, 64, 32, 0, 316, 319, 3, 66, 33, 0, 317, 319, 3, 68, 34, 0, 318, 314, 1, 0, 0, 0, 318, 315, 1, 0, 0, 0, 318, 316, 1, 0, 0, 0, 318, 317, 1, 0, 0, 0, 319, 61, 1, 0, 0, 0, 320, 321, 5, 26, 0, 0, 321, 322, 5, 10, 0, 0, 322, 63, 1, 0, 0, 0, 323, 324, 5, 27, 0, 0, 324, 325, 5, 10, 0, 0, 325, 65, 1, 0, 0, 0, 326, 327, 5, 29, 0, 0, 327, 328, 5, 10, 0, 0, 328, 67, 1, 0, 0, 0, 329, 330, 5, 28, 0, 0, 330, 331, 5, 10, 0, 0, 331, 69, 1, 0, 0, 0, 332, 337, 5, 30, 0, 0, 333, 338, 3, 40, 20, 0, 334, 338, 3, 32, 16, 0, 335, 338, 5, 3, 0, 0, 336, 338, 5, 4, 0, 0, 337, 333, 1, 0, 0, 0, 337, 334, 1, 0, 0, 0, 337, 335, 1, 0, 0, 0, 337, 336, 1, 0, 0, 0, 338, 339, 1, 0, 0, 0, 339, 337, 1, 0, 0, 0, 339, 340, 1, 0, 0, 0, 340, 341, 1, 0, 0, 0, 341, 351, 5, 30, 0, 0, 342, 344, 5, 31, 0, 0, 343, 345, 3, 40, 20, 0, 344, 343, 1, 0, 0, 0, 345, 346, 1, 0, 0, 0, 346, 344, 1, 0, 0, 0, 346, 347, 1, 0, 0, 0, 347, 348, 1, 0, 0, 0, 348, 349, 5, 31, 0, 0, 349, 351, 1, 0, 0, 0, 350, 332, 1, 0, 0, 0, 350, 342, 1, 0, 0, 0, 351, 71, 1, 0, 0, 0, 352, 353, 5, 3, 0, 0, 353, 354, 3, 44, 22, 0, 354, 355, 5, 4, 0, 0, 355, 73, 1, 0, 0, 0, 356, 357, 5, 1, 0, 0, 357, 358, 3, 44, 22, 0, 358, 359, 5, 2, 0, 0, 359, 75, 1, 0, 0, 0, 360, 364, 3, 84, 42, 0, 361, 363, 5, 7, 0, 0, 362, 361, 1, 0, 0, 0, 363, 366, 1, 0, 0, 0, 364, 362, 1, 0, 0, 0, 364, 365, 1, 0, 0, 0, 365, 370, 1, 0, 0, 0, 366, 364, 1, 0, 0, 0, 367, 369, 3, 6, 3, 0, 368, 367, 1, 0, 0, 0, 369, 372, 1, 0, 0, 0, 370, 368, 1, 0, 0, 0, 370, 371, 1, 0, 0, 0, 371, 379, 1, 0, 0, 0, 372, 370, 1, 0, 0, 0, 373, 375, 5, 7, 0, 0, 374, 373, 1, 0, 0, 0, 374, 375, 1, 0, 0, 0, 375, 376, 1, 0, 0, 0, 376, 378, 3, 78, 39, 0, 377, 374, 1, 0, 0, 0, 378, 381, 1, 0, 0, 0, 379, 377, 1, 0, 0, 0, 379, 380, 1, 0, 0, 0, 380, 77, 1, 0, 0, 0, 381, 379, 1, 0, 0, 0, 382, 386, 3, 86, 43, 0, 383, 385, 5, 7, 0, 0, 384, 383, 1, 0, 0, 0, 385, 388, 1, 0, 0, 0, 386, 384, 1, 0, 0, 0, 386, 387, 1, 0, 0, 0, 387, 392, 1, 0, 0, 0, 388, 386, 1, 0, 0, 0, 389, 391, 3, 6, 3, 0, 390, 389, 1, 0, 0, 0, 391, 394, 1, 0, 0, 0, 392, 390, 1, 0, 0, 0, 392, 393, 1, 0, 0, 0, 393, 401, 1, 0, 0, 0, 394, 392, 1, 0, 0, 0, 395, 397, 5, 7, 0, 0, 396, 395, 1, 0, 0, 0, 396, 397, 1, 0, 0, 0, 397, 398, 1, 0, 0, 0, 398, 400, 3, 80, 40, 0, 399, 396, 1, 0, 0, 0, 400, 403, 1, 0, 0, 0, 401, 399, 1, 0, 0, 0, 401, 402, 1, 0, 0, 0, 402, 79, 1, 0, 0, 0, 403, 401, 1, 0, 0, 0, 404, 408, 3, 88, 44, 0, 405, 407, 5, 7, 0, 0, 406, 405, 1, 0, 0, 0, 407, 410, 1, 0, 0, 0, 408, 406, 1, 0, 0, 0, 408, 409, 1, 0, 0, 0, 409, 414, 1, 0, 0, 0, 410, 408, 1, 0, 0, 0, 411, 413, 3, 6, 3, 0, 412, 411, 1, 0, 0, 0, 413, 416, 1, 0, 0, 0, 414, 412, 1, 0, 0, 0, 414, 415, 1, 0, 0, 0, 415, 423, 1, 0, 0, 0, 416, 414, 1, 0, 0, 0, 417, 419, 5, 7, 0, 0, 418, 417, 1, 0, 0, 0, 418, 419, 1, 0, 0, 0, 419, 420, 1, 0, 0, 0, 420, 422, 3, 82, 41, 0, 421, 418, 1, 0, 0, 0, 422, 425, 1, 0, 0, 0, 423, 421, 1, 0, 0, 0, 423, 424, 1, 0, 0, 0, 424, 81, 1, 0, 0, 0, 425, 423, 1, 0, 0, 0, 426, 430, 3, 90, 45, 0, 427, 429, 5, 7, 0, 0, 428, 427, 1, 0, 0, 0, 429, 432, 1, 0, 0, 0, 430, 428, 1, 0, 0, 0, 430, 431, 1, 0, 0, 0, 431, 436, 1, 0, 0, 0, 432, 430, 1, 0, 0, 0, 433, 435, 3, 6, 3, 0, 434, 433, 1, 0, 0, 0, 435, 438, 1, 0, 0, 0, 436, 434, 1, 0, 0, 0, 436, 437, 1, 0, 0, 0, 437, 83, 1, 0, 0, 0, 438, 436, 1, 0, 0, 0, 439, 440, 5, 26, 0, 0, 440, 441, 5, 26, 0, 0, 441, 442, 5, 26, 0, 0, 442, 443, 5, 26, 0, 0, 443, 444, 5, 26, 0, 0, 444, 445, 5, 26, 0, 0, 445, 446, 5, 26, 0, 0, 446, 447, 5, 26, 0, 0, 447, 448, 5, 26, 0, 0, 448, 449, 3, 36, 18, 0, 449, 450, 3, 92, 46, 0, 450, 85, 1, 0, 0, 0, 451, 452, 5, 5, 0, 0, 452, 453, 3, 36, 18, 0, 453, 454, 3, 92, 46, 0, 454, 87, 1, 0, 0, 0, 455, 456, 5, 6, 0, 0, 456, 457, 3, 36, 18, 0, 457, 458, 3, 92, 46, 0, 458, 89, 1, 0, 0, 0, 459, 460, 5, 18, 0, 0, 460, 461, 5, 18, 0, 0, 461, 462, 5, 18, 0, 0, 462, 463, 3, 36, 18, 0, 463, 464, 3, 92, 46, 0, 464, 91, 1, 0, 0, 0, 465, 466, 7, 4, 0, 0, 466, 93, 1, 0, 0, 0, 52, 98, 103, 109, 115, 118, 125, 129, 136, 141, 148, 160, 168, 177, 182, 190, 200, 206, 215, 220, 232, 237, 241, 243, 248, 253, 255, 258, 261, 269, 280, 286, 295, 306, 318, 337, 339, 346, 350, 364, 370, 374, 379, 386, 392, 396, 401, 408, 414, 418, 423, 430, 436]
+[4, 1, 35, 470, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 2, 43, 7, 43, 2, 44, 7, 44, 2, 45, 7, 45, 2, 46, 7, 46, 1, 0, 1, 0, 4, 0, 97, 8, 0, 11, 0, 12, 0, 98, 1, 0, 5, 0, 102, 8, 0, 10, 0, 12, 0, 105, 9, 0, 1, 0, 5, 0, 108, 8, 0, 10, 0, 12, 0, 111, 9, 0, 1, 0, 5, 0, 114, 8, 0, 10, 0, 12, 0, 117, 9, 0, 3, 0, 119, 8, 0, 1, 0, 1, 0, 1, 1, 4, 1, 124, 8, 1, 11, 1, 12, 1, 125, 1, 2, 1, 2, 3, 2, 130, 8, 2, 1, 2, 1, 2, 1, 3, 4, 3, 135, 8, 3, 11, 3, 12, 3, 136, 1, 3, 5, 3, 140, 8, 3, 10, 3, 12, 3, 143, 9, 3, 1, 4, 1, 4, 1, 4, 1, 4, 3, 4, 149, 8, 4, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 6, 1, 6, 1, 6, 5, 6, 159, 8, 6, 10, 6, 12, 6, 162, 9, 6, 1, 7, 1, 7, 1, 7, 1, 8, 1, 8, 3, 8, 169, 8, 8, 1, 8, 1, 8, 1, 9, 1, 9, 1, 9, 4, 9, 176, 8, 9, 11, 9, 12, 9, 177, 1, 9, 5, 9, 181, 8, 9, 10, 9, 12, 9, 184, 9, 9, 1, 10, 1, 10, 1, 10, 5, 10, 189, 8, 10, 10, 10, 12, 10, 192, 9, 10, 1, 11, 1, 11, 1, 11, 1, 12, 1, 12, 5, 12, 199, 8, 12, 10, 12, 12, 12, 202, 9, 12, 1, 13, 1, 13, 1, 13, 3, 13, 207, 8, 13, 1, 13, 1, 13, 1, 13, 1, 14, 1, 14, 1, 14, 1, 14, 3, 14, 216, 8, 14, 1, 15, 1, 15, 1, 15, 3, 15, 221, 8, 15, 1, 16, 1, 16, 1, 16, 1, 16, 1, 16, 1, 17, 1, 17, 1, 18, 4, 18, 231, 8, 18, 11, 18, 12, 18, 232, 1, 19, 1, 19, 1, 19, 3, 19, 238, 8, 19, 1, 19, 1, 19, 5, 19, 242, 8, 19, 10, 19, 12, 19, 245, 9, 19, 1, 19, 1, 19, 3, 19, 249, 8, 19, 1, 19, 1, 19, 1, 19, 5, 19, 254, 8, 19, 10, 19, 12, 19, 257, 9, 19, 3, 19, 259, 8, 19, 1, 19, 3, 19, 262, 8, 19, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 3, 20, 272, 8, 20, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 22, 1, 22, 4, 22, 281, 8, 22, 11, 22, 12, 22, 282, 1, 22, 1, 22, 5, 22, 287, 8, 22, 10, 22, 12, 22, 290, 9, 22, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 3, 23, 298, 8, 23, 1, 24, 1, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 26, 1, 26, 1, 26, 3, 26, 309, 8, 26, 1, 27, 1, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 30, 1, 30, 3, 30, 321, 8, 30, 1, 31, 1, 31, 1, 31, 1, 32, 1, 32, 1, 32, 1, 33, 1, 33, 1, 33, 1, 34, 1, 34, 1, 34, 1, 35, 1, 35, 1, 35, 1, 35, 1, 35, 4, 35, 340, 8, 35, 11, 35, 12, 35, 341, 1, 35, 1, 35, 1, 35, 4, 35, 347, 8, 35, 11, 35, 12, 35, 348, 1, 35, 1, 35, 3, 35, 353, 8, 35, 1, 36, 1, 36, 1, 36, 1, 36, 1, 37, 1, 37, 1, 37, 1, 37, 1, 38, 1, 38, 5, 38, 365, 8, 38, 10, 38, 12, 38, 368, 9, 38, 1, 38, 5, 38, 371, 8, 38, 10, 38, 12, 38, 374, 9, 38, 1, 38, 3, 38, 377, 8, 38, 1, 38, 5, 38, 380, 8, 38, 10, 38, 12, 38, 383, 9, 38, 1, 39, 1, 39, 5, 39, 387, 8, 39, 10, 39, 12, 39, 390, 9, 39, 1, 39, 5, 39, 393, 8, 39, 10, 39, 12, 39, 396, 9, 39, 1, 39, 3, 39, 399, 8, 39, 1, 39, 5, 39, 402, 8, 39, 10, 39, 12, 39, 405, 9, 39, 1, 40, 1, 40, 5, 40, 409, 8, 40, 10, 40, 12, 40, 412, 9, 40, 1, 40, 5, 40, 415, 8, 40, 10, 40, 12, 40, 418, 9, 40, 1, 40, 3, 40, 421, 8, 40, 1, 40, 5, 40, 424, 8, 40, 10, 40, 12, 40, 427, 9, 40, 1, 41, 1, 41, 5, 41, 431, 8, 41, 10, 41, 12, 41, 434, 9, 41, 1, 41, 5, 41, 437, 8, 41, 10, 41, 12, 41, 440, 9, 41, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 43, 1, 43, 1, 43, 1, 43, 1, 44, 1, 44, 1, 44, 1, 44, 1, 45, 1, 45, 1, 45, 1, 45, 1, 45, 1, 45, 1, 46, 1, 46, 1, 46, 0, 0, 47, 0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 0, 5, 2, 0, 9, 9, 32, 32, 4, 0, 17, 17, 21, 21, 24, 25, 32, 35, 2, 0, 18, 20, 22, 22, 1, 0, 26, 29, 1, 1, 7, 7, 496, 0, 94, 1, 0, 0, 0, 2, 123, 1, 0, 0, 0, 4, 127, 1, 0, 0, 0, 6, 134, 1, 0, 0, 0, 8, 148, 1, 0, 0, 0, 10, 150, 1, 0, 0, 0, 12, 155, 1, 0, 0, 0, 14, 163, 1, 0, 0, 0, 16, 168, 1, 0, 0, 0, 18, 172, 1, 0, 0, 0, 20, 185, 1, 0, 0, 0, 22, 193, 1, 0, 0, 0, 24, 196, 1, 0, 0, 0, 26, 203, 1, 0, 0, 0, 28, 215, 1, 0, 0, 0, 30, 217, 1, 0, 0, 0, 32, 222, 1, 0, 0, 0, 34, 227, 1, 0, 0, 0, 36, 230, 1, 0, 0, 0, 38, 234, 1, 0, 0, 0, 40, 271, 1, 0, 0, 0, 42, 273, 1, 0, 0, 0, 44, 278, 1, 0, 0, 0, 46, 297, 1, 0, 0, 0, 48, 299, 1, 0, 0, 0, 50, 301, 1, 0, 0, 0, 52, 308, 1, 0, 0, 0, 54, 310, 1, 0, 0, 0, 56, 312, 1, 0, 0, 0, 58, 314, 1, 0, 0, 0, 60, 320, 1, 0, 0, 0, 62, 322, 1, 0, 0, 0, 64, 325, 1, 0, 0, 0, 66, 328, 1, 0, 0, 0, 68, 331, 1, 0, 0, 0, 70, 352, 1, 0, 0, 0, 72, 354, 1, 0, 0, 0, 74, 358, 1, 0, 0, 0, 76, 362, 1, 0, 0, 0, 78, 384, 1, 0, 0, 0, 80, 406, 1, 0, 0, 0, 82, 428, 1, 0, 0, 0, 84, 441, 1, 0, 0, 0, 86, 453, 1, 0, 0, 0, 88, 457, 1, 0, 0, 0, 90, 461, 1, 0, 0, 0, 92, 467, 1, 0, 0, 0, 94, 118, 3, 2, 1, 0, 95, 97, 5, 7, 0, 0, 96, 95, 1, 0, 0, 0, 97, 98, 1, 0, 0, 0, 98, 96, 1, 0, 0, 0, 98, 99, 1, 0, 0, 0, 99, 103, 1, 0, 0, 0, 100, 102, 3, 6, 3, 0, 101, 100, 1, 0, 0, 0, 102, 105, 1, 0, 0, 0, 103, 101, 1, 0, 0, 0, 103, 104, 1, 0, 0, 0, 104, 109, 1, 0, 0, 0, 105, 103, 1, 0, 0, 0, 106, 108, 3, 78, 39, 0, 107, 106, 1, 0, 0, 0, 108, 111, 1, 0, 0, 0, 109, 107, 1, 0, 0, 0, 109, 110, 1, 0, 0, 0, 110, 115, 1, 0, 0, 0, 111, 109, 1, 0, 0, 0, 112, 114, 3, 76, 38, 0, 113, 112, 1, 0, 0, 0, 114, 117, 1, 0, 0, 0, 115, 113, 1, 0, 0, 0, 115, 116, 1, 0, 0, 0, 116, 119, 1, 0, 0, 0, 117, 115, 1, 0, 0, 0, 118, 96, 1, 0, 0, 0, 118, 119, 1, 0, 0, 0, 119, 120, 1, 0, 0, 0, 120, 121, 5, 0, 0, 1, 121, 1, 1, 0, 0, 0, 122, 124, 3, 4, 2, 0, 123, 122, 1, 0, 0, 0, 124, 125, 1, 0, 0, 0, 125, 123, 1, 0, 0, 0, 125, 126, 1, 0, 0, 0, 126, 3, 1, 0, 0, 0, 127, 129, 5, 26, 0, 0, 128, 130, 3, 36, 18, 0, 129, 128, 1, 0, 0, 0, 129, 130, 1, 0, 0, 0, 130, 131, 1, 0, 0, 0, 131, 132, 5, 7, 0, 0, 132, 5, 1, 0, 0, 0, 133, 135, 3, 8, 4, 0, 134, 133, 1, 0, 0, 0, 135, 136, 1, 0, 0, 0, 136, 134, 1, 0, 0, 0, 136, 137, 1, 0, 0, 0, 137, 141, 1, 0, 0, 0, 138, 140, 5, 7, 0, 0, 139, 138, 1, 0, 0, 0, 140, 143, 1, 0, 0, 0, 141, 139, 1, 0, 0, 0, 141, 142, 1, 0, 0, 0, 142, 7, 1, 0, 0, 0, 143, 141, 1, 0, 0, 0, 144, 149, 3, 24, 12, 0, 145, 149, 3, 12, 6, 0, 146, 149, 3, 10, 5, 0, 147, 149, 3, 4, 2, 0, 148, 144, 1, 0, 0, 0, 148, 145, 1, 0, 0, 0, 148, 146, 1, 0, 0, 0, 148, 147, 1, 0, 0, 0, 149, 9, 1, 0, 0, 0, 150, 151, 3, 74, 37, 0, 151, 152, 5, 22, 0, 0, 152, 153, 3, 36, 18, 0, 153, 154, 5, 7, 0, 0, 154, 11, 1, 0, 0, 0, 155, 156, 5, 18, 0, 0, 156, 160, 3, 14, 7, 0, 157, 159, 3, 20, 10, 0, 158, 157, 1, 0, 0, 0, 159, 162, 1, 0, 0, 0, 160, 158, 1, 0, 0, 0, 160, 161, 1, 0, 0, 0, 161, 13, 1, 0, 0, 0, 162, 160, 1, 0, 0, 0, 163, 164, 3, 16, 8, 0, 164, 165, 5, 7, 0, 0, 165, 15, 1, 0, 0, 0, 166, 167, 5, 23, 0, 0, 167, 169, 3, 34, 17, 0, 168, 166, 1, 0, 0, 0, 168, 169, 1, 0, 0, 0, 169, 170, 1, 0, 0, 0, 170, 171, 3, 18, 9, 0, 171, 17, 1, 0, 0, 0, 172, 182, 3, 36, 18, 0, 173, 175, 5, 7, 0, 0, 174, 176, 5, 23, 0, 0, 175, 174, 1, 0, 0, 0, 176, 177, 1, 0, 0, 0, 177, 175, 1, 0, 0, 0, 177, 178, 1, 0, 0, 0, 178, 179, 1, 0, 0, 0, 179, 181, 3, 36, 18, 0, 180, 173, 1, 0, 0, 0, 181, 184, 1, 0, 0, 0, 182, 180, 1, 0, 0, 0, 182, 183, 1, 0, 0, 0, 183, 19, 1, 0, 0, 0, 184, 182, 1, 0, 0, 0, 185, 186, 5, 15, 0, 0, 186, 190, 3, 14, 7, 0, 187, 189, 3, 22, 11, 0, 188, 187, 1, 0, 0, 0, 189, 192, 1, 0, 0, 0, 190, 188, 1, 0, 0, 0, 190, 191, 1, 0, 0, 0, 191, 21, 1, 0, 0, 0, 192, 190, 1, 0, 0, 0, 193, 194, 5, 16, 0, 0, 194, 195, 3, 14, 7, 0, 195, 23, 1, 0, 0, 0, 196, 200, 3, 26, 13, 0, 197, 199, 3, 20, 10, 0, 198, 197, 1, 0, 0, 0, 199, 202, 1, 0, 0, 0, 200, 198, 1, 0, 0, 0, 200, 201, 1, 0, 0, 0, 201, 25, 1, 0, 0, 0, 202, 200, 1, 0, 0, 0, 203, 206, 3, 28, 14, 0, 204, 205, 5, 23, 0, 0, 205, 207, 3, 32, 16, 0, 206, 204, 1, 0, 0, 0, 206, 207, 1, 0, 0, 0, 207, 208, 1, 0, 0, 0, 208, 209, 3, 16, 8, 0, 209, 210, 5, 7, 0, 0, 210, 27, 1, 0, 0, 0, 211, 216, 5, 8, 0, 0, 212, 216, 3, 30, 15, 0, 213, 216, 5, 34, 0, 0, 214, 216, 5, 35, 0, 0, 215, 211, 1, 0, 0, 0, 215, 212, 1, 0, 0, 0, 215, 213, 1, 0, 0, 0, 215, 214, 1, 0, 0, 0, 216, 29, 1, 0, 0, 0, 217, 220, 7, 0, 0, 0, 218, 219, 5, 22, 0, 0, 219, 221, 3, 50, 25, 0, 220, 218, 1, 0, 0, 0, 220, 221, 1, 0, 0, 0, 221, 31, 1, 0, 0, 0, 222, 223, 5, 1, 0, 0, 223, 224, 5, 26, 0, 0, 224, 225, 5, 10, 0, 0, 225, 226, 5, 2, 0, 0, 226, 33, 1, 0, 0, 0, 227, 228, 5, 13, 0, 0, 228, 35, 1, 0, 0, 0, 229, 231, 3, 38, 19, 0, 230, 229, 1, 0, 0, 0, 231, 232, 1, 0, 0, 0, 232, 230, 1, 0, 0, 0, 232, 233, 1, 0, 0, 0, 233, 37, 1, 0, 0, 0, 234, 237, 5, 23, 0, 0, 235, 236, 5, 30, 0, 0, 236, 238, 3, 54, 27, 0, 237, 235, 1, 0, 0, 0, 237, 238, 1, 0, 0, 0, 238, 243, 1, 0, 0, 0, 239, 242, 3, 54, 27, 0, 240, 242, 5, 31, 0, 0, 241, 239, 1, 0, 0, 0, 241, 240, 1, 0, 0, 0, 242, 245, 1, 0, 0, 0, 243, 241, 1, 0, 0, 0, 243, 244, 1, 0, 0, 0, 244, 248, 1, 0, 0, 0, 245, 243, 1, 0, 0, 0, 246, 249, 3, 40, 20, 0, 247, 249, 3, 70, 35, 0, 248, 246, 1, 0, 0, 0, 248, 247, 1, 0, 0, 0, 248, 249, 1, 0, 0, 0, 249, 258, 1, 0, 0, 0, 250, 255, 3, 52, 26, 0, 251, 254, 3, 52, 26, 0, 252, 254, 3, 46, 23, 0, 253, 251, 1, 0, 0, 0, 253, 252, 1, 0, 0, 0, 254, 257, 1, 0, 0, 0, 255, 253, 1, 0, 0, 0, 255, 256, 1, 0, 0, 0, 256, 259, 1, 0, 0, 0, 257, 255, 1, 0, 0, 0, 258, 250, 1, 0, 0, 0, 258, 259, 1, 0, 0, 0, 259, 261, 1, 0, 0, 0, 260, 262, 3, 74, 37, 0, 261, 260, 1, 0, 0, 0, 261, 262, 1, 0, 0, 0, 262, 39, 1, 0, 0, 0, 263, 272, 3, 58, 29, 0, 264, 272, 3, 60, 30, 0, 265, 272, 3, 72, 36, 0, 266, 272, 3, 42, 21, 0, 267, 272, 3, 44, 22, 0, 268, 272, 3, 74, 37, 0, 269, 272, 3, 34, 17, 0, 270, 272, 3, 32, 16, 0, 271, 263, 1, 0, 0, 0, 271, 264, 1, 0, 0, 0, 271, 265, 1, 0, 0, 0, 271, 266, 1, 0, 0, 0, 271, 267, 1, 0, 0, 0, 271, 268, 1, 0, 0, 0, 271, 269, 1, 0, 0, 0, 271, 270, 1, 0, 0, 0, 272, 41, 1, 0, 0, 0, 273, 274, 5, 10, 0, 0, 274, 275, 5, 22, 0, 0, 275, 276, 5, 22, 0, 0, 276, 277, 3, 44, 22, 0, 277, 43, 1, 0, 0, 0, 278, 288, 3, 46, 23, 0, 279, 281, 3, 56, 28, 0, 280, 279, 1, 0, 0, 0, 281, 282, 1, 0, 0, 0, 282, 280, 1, 0, 0, 0, 282, 283, 1, 0, 0, 0, 283, 284, 1, 0, 0, 0, 284, 285, 3, 46, 23, 0, 285, 287, 1, 0, 0, 0, 286, 280, 1, 0, 0, 0, 287, 290, 1, 0, 0, 0, 288, 286, 1, 0, 0, 0, 288, 289, 1, 0, 0, 0, 289, 45, 1, 0, 0, 0, 290, 288, 1, 0, 0, 0, 291, 298, 5, 10, 0, 0, 292, 298, 5, 14, 0, 0, 293, 298, 3, 48, 24, 0, 294, 298, 3, 50, 25, 0, 295, 298, 5, 8, 0, 0, 296, 298, 5, 9, 0, 0, 297, 291, 1, 0, 0, 0, 297, 292, 1, 0, 0, 0, 297, 293, 1, 0, 0, 0, 297, 294, 1, 0, 0, 0, 297, 295, 1, 0, 0, 0, 297, 296, 1, 0, 0, 0, 298, 47, 1, 0, 0, 0, 299, 300, 5, 11, 0, 0, 300, 49, 1, 0, 0, 0, 301, 302, 5, 12, 0, 0, 302, 51, 1, 0, 0, 0, 303, 309, 5, 30, 0, 0, 304, 309, 5, 31, 0, 0, 305, 309, 3, 54, 27, 0, 306, 309, 3, 58, 29, 0, 307, 309, 3, 56, 28, 0, 308, 303, 1, 0, 0, 0, 308, 304, 1, 0, 0, 0, 308, 305, 1, 0, 0, 0, 308, 306, 1, 0, 0, 0, 308, 307, 1, 0, 0, 0, 309, 53, 1, 0, 0, 0, 310, 311, 7, 1, 0, 0, 311, 55, 1, 0, 0, 0, 312, 313, 7, 2, 0, 0, 313, 57, 1, 0, 0, 0, 314, 315, 7, 3, 0, 0, 315, 59, 1, 0, 0, 0, 316, 321, 3, 62, 31, 0, 317, 321, 3, 64, 32, 0, 318, 321, 3, 66, 33, 0, 319, 321, 3, 68, 34, 0, 320, 316, 1, 0, 0, 0, 320, 317, 1, 0, 0, 0, 320, 318, 1, 0, 0, 0, 320, 319, 1, 0, 0, 0, 321, 61, 1, 0, 0, 0, 322, 323, 5, 26, 0, 0, 323, 324, 5, 10, 0, 0, 324, 63, 1, 0, 0, 0, 325, 326, 5, 27, 0, 0, 326, 327, 5, 10, 0, 0, 327, 65, 1, 0, 0, 0, 328, 329, 5, 29, 0, 0, 329, 330, 5, 10, 0, 0, 330, 67, 1, 0, 0, 0, 331, 332, 5, 28, 0, 0, 332, 333, 5, 10, 0, 0, 333, 69, 1, 0, 0, 0, 334, 339, 5, 30, 0, 0, 335, 340, 3, 40, 20, 0, 336, 340, 3, 32, 16, 0, 337, 340, 5, 3, 0, 0, 338, 340, 5, 4, 0, 0, 339, 335, 1, 0, 0, 0, 339, 336, 1, 0, 0, 0, 339, 337, 1, 0, 0, 0, 339, 338, 1, 0, 0, 0, 340, 341, 1, 0, 0, 0, 341, 339, 1, 0, 0, 0, 341, 342, 1, 0, 0, 0, 342, 343, 1, 0, 0, 0, 343, 353, 5, 30, 0, 0, 344, 346, 5, 31, 0, 0, 345, 347, 3, 40, 20, 0, 346, 345, 1, 0, 0, 0, 347, 348, 1, 0, 0, 0, 348, 346, 1, 0, 0, 0, 348, 349, 1, 0, 0, 0, 349, 350, 1, 0, 0, 0, 350, 351, 5, 31, 0, 0, 351, 353, 1, 0, 0, 0, 352, 334, 1, 0, 0, 0, 352, 344, 1, 0, 0, 0, 353, 71, 1, 0, 0, 0, 354, 355, 5, 3, 0, 0, 355, 356, 3, 44, 22, 0, 356, 357, 5, 4, 0, 0, 357, 73, 1, 0, 0, 0, 358, 359, 5, 1, 0, 0, 359, 360, 3, 44, 22, 0, 360, 361, 5, 2, 0, 0, 361, 75, 1, 0, 0, 0, 362, 366, 3, 84, 42, 0, 363, 365, 5, 7, 0, 0, 364, 363, 1, 0, 0, 0, 365, 368, 1, 0, 0, 0, 366, 364, 1, 0, 0, 0, 366, 367, 1, 0, 0, 0, 367, 372, 1, 0, 0, 0, 368, 366, 1, 0, 0, 0, 369, 371, 3, 6, 3, 0, 370, 369, 1, 0, 0, 0, 371, 374, 1, 0, 0, 0, 372, 370, 1, 0, 0, 0, 372, 373, 1, 0, 0, 0, 373, 381, 1, 0, 0, 0, 374, 372, 1, 0, 0, 0, 375, 377, 5, 7, 0, 0, 376, 375, 1, 0, 0, 0, 376, 377, 1, 0, 0, 0, 377, 378, 1, 0, 0, 0, 378, 380, 3, 78, 39, 0, 379, 376, 1, 0, 0, 0, 380, 383, 1, 0, 0, 0, 381, 379, 1, 0, 0, 0, 381, 382, 1, 0, 0, 0, 382, 77, 1, 0, 0, 0, 383, 381, 1, 0, 0, 0, 384, 388, 3, 86, 43, 0, 385, 387, 5, 7, 0, 0, 386, 385, 1, 0, 0, 0, 387, 390, 1, 0, 0, 0, 388, 386, 1, 0, 0, 0, 388, 389, 1, 0, 0, 0, 389, 394, 1, 0, 0, 0, 390, 388, 1, 0, 0, 0, 391, 393, 3, 6, 3, 0, 392, 391, 1, 0, 0, 0, 393, 396, 1, 0, 0, 0, 394, 392, 1, 0, 0, 0, 394, 395, 1, 0, 0, 0, 395, 403, 1, 0, 0, 0, 396, 394, 1, 0, 0, 0, 397, 399, 5, 7, 0, 0, 398, 397, 1, 0, 0, 0, 398, 399, 1, 0, 0, 0, 399, 400, 1, 0, 0, 0, 400, 402, 3, 80, 40, 0, 401, 398, 1, 0, 0, 0, 402, 405, 1, 0, 0, 0, 403, 401, 1, 0, 0, 0, 403, 404, 1, 0, 0, 0, 404, 79, 1, 0, 0, 0, 405, 403, 1, 0, 0, 0, 406, 410, 3, 88, 44, 0, 407, 409, 5, 7, 0, 0, 408, 407, 1, 0, 0, 0, 409, 412, 1, 0, 0, 0, 410, 408, 1, 0, 0, 0, 410, 411, 1, 0, 0, 0, 411, 416, 1, 0, 0, 0, 412, 410, 1, 0, 0, 0, 413, 415, 3, 6, 3, 0, 414, 413, 1, 0, 0, 0, 415, 418, 1, 0, 0, 0, 416, 414, 1, 0, 0, 0, 416, 417, 1, 0, 0, 0, 417, 425, 1, 0, 0, 0, 418, 416, 1, 0, 0, 0, 419, 421, 5, 7, 0, 0, 420, 419, 1, 0, 0, 0, 420, 421, 1, 0, 0, 0, 421, 422, 1, 0, 0, 0, 422, 424, 3, 82, 41, 0, 423, 420, 1, 0, 0, 0, 424, 427, 1, 0, 0, 0, 425, 423, 1, 0, 0, 0, 425, 426, 1, 0, 0, 0, 426, 81, 1, 0, 0, 0, 427, 425, 1, 0, 0, 0, 428, 432, 3, 90, 45, 0, 429, 431, 5, 7, 0, 0, 430, 429, 1, 0, 0, 0, 431, 434, 1, 0, 0, 0, 432, 430, 1, 0, 0, 0, 432, 433, 1, 0, 0, 0, 433, 438, 1, 0, 0, 0, 434, 432, 1, 0, 0, 0, 435, 437, 3, 6, 3, 0, 436, 435, 1, 0, 0, 0, 437, 440, 1, 0, 0, 0, 438, 436, 1, 0, 0, 0, 438, 439, 1, 0, 0, 0, 439, 83, 1, 0, 0, 0, 440, 438, 1, 0, 0, 0, 441, 442, 5, 26, 0, 0, 442, 443, 5, 26, 0, 0, 443, 444, 5, 26, 0, 0, 444, 445, 5, 26, 0, 0, 445, 446, 5, 26, 0, 0, 446, 447, 5, 26, 0, 0, 447, 448, 5, 26, 0, 0, 448, 449, 5, 26, 0, 0, 449, 450, 5, 26, 0, 0, 450, 451, 3, 36, 18, 0, 451, 452, 3, 92, 46, 0, 452, 85, 1, 0, 0, 0, 453, 454, 5, 5, 0, 0, 454, 455, 3, 36, 18, 0, 455, 456, 3, 92, 46, 0, 456, 87, 1, 0, 0, 0, 457, 458, 5, 6, 0, 0, 458, 459, 3, 36, 18, 0, 459, 460, 3, 92, 46, 0, 460, 89, 1, 0, 0, 0, 461, 462, 5, 18, 0, 0, 462, 463, 5, 18, 0, 0, 463, 464, 5, 18, 0, 0, 464, 465, 3, 36, 18, 0, 465, 466, 3, 92, 46, 0, 466, 91, 1, 0, 0, 0, 467, 468, 7, 4, 0, 0, 468, 93, 1, 0, 0, 0, 52, 98, 103, 109, 115, 118, 125, 129, 136, 141, 148, 160, 168, 177, 182, 190, 200, 206, 215, 220, 232, 237, 241, 243, 248, 253, 255, 258, 261, 271, 282, 288, 297, 308, 320, 339, 341, 348, 352, 366, 372, 376, 381, 388, 394, 398, 403, 410, 416, 420, 425, 432, 438]
```

### Comparing `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFile.tokens` & `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFile.tokens`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileLexer.interp` & `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileLexer.interp`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileLexer.py` & `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileLexer.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens` & `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileListener.py` & `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileListener.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileParser.py` & `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
 	from typing.io import TextIO
 
 def serializedATN():
     return [
-        4,1,35,468,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
+        4,1,35,470,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
         6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,13,7,13,
         2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,19,2,20,
         7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,26,7,26,
         2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,32,2,33,
         7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,39,7,39,
         2,40,7,40,2,41,7,41,2,42,7,42,2,43,7,43,2,44,7,44,2,45,7,45,2,46,
         7,46,1,0,1,0,4,0,97,8,0,11,0,12,0,98,1,0,5,0,102,8,0,10,0,12,0,105,
@@ -28,162 +28,164 @@
         10,12,10,192,9,10,1,11,1,11,1,11,1,12,1,12,5,12,199,8,12,10,12,12,
         12,202,9,12,1,13,1,13,1,13,3,13,207,8,13,1,13,1,13,1,13,1,14,1,14,
         1,14,1,14,3,14,216,8,14,1,15,1,15,1,15,3,15,221,8,15,1,16,1,16,1,
         16,1,16,1,16,1,17,1,17,1,18,4,18,231,8,18,11,18,12,18,232,1,19,1,
         19,1,19,3,19,238,8,19,1,19,1,19,5,19,242,8,19,10,19,12,19,245,9,
         19,1,19,1,19,3,19,249,8,19,1,19,1,19,1,19,5,19,254,8,19,10,19,12,
         19,257,9,19,3,19,259,8,19,1,19,3,19,262,8,19,1,20,1,20,1,20,1,20,
-        1,20,1,20,3,20,270,8,20,1,21,1,21,1,21,1,21,1,21,1,22,1,22,4,22,
-        279,8,22,11,22,12,22,280,1,22,1,22,5,22,285,8,22,10,22,12,22,288,
-        9,22,1,23,1,23,1,23,1,23,1,23,1,23,3,23,296,8,23,1,24,1,24,1,25,
-        1,25,1,26,1,26,1,26,1,26,1,26,3,26,307,8,26,1,27,1,27,1,28,1,28,
-        1,29,1,29,1,30,1,30,1,30,1,30,3,30,319,8,30,1,31,1,31,1,31,1,32,
-        1,32,1,32,1,33,1,33,1,33,1,34,1,34,1,34,1,35,1,35,1,35,1,35,1,35,
-        4,35,338,8,35,11,35,12,35,339,1,35,1,35,1,35,4,35,345,8,35,11,35,
-        12,35,346,1,35,1,35,3,35,351,8,35,1,36,1,36,1,36,1,36,1,37,1,37,
-        1,37,1,37,1,38,1,38,5,38,363,8,38,10,38,12,38,366,9,38,1,38,5,38,
-        369,8,38,10,38,12,38,372,9,38,1,38,3,38,375,8,38,1,38,5,38,378,8,
-        38,10,38,12,38,381,9,38,1,39,1,39,5,39,385,8,39,10,39,12,39,388,
-        9,39,1,39,5,39,391,8,39,10,39,12,39,394,9,39,1,39,3,39,397,8,39,
-        1,39,5,39,400,8,39,10,39,12,39,403,9,39,1,40,1,40,5,40,407,8,40,
-        10,40,12,40,410,9,40,1,40,5,40,413,8,40,10,40,12,40,416,9,40,1,40,
-        3,40,419,8,40,1,40,5,40,422,8,40,10,40,12,40,425,9,40,1,41,1,41,
-        5,41,429,8,41,10,41,12,41,432,9,41,1,41,5,41,435,8,41,10,41,12,41,
-        438,9,41,1,42,1,42,1,42,1,42,1,42,1,42,1,42,1,42,1,42,1,42,1,42,
-        1,42,1,43,1,43,1,43,1,43,1,44,1,44,1,44,1,44,1,45,1,45,1,45,1,45,
-        1,45,1,45,1,46,1,46,1,46,0,0,47,0,2,4,6,8,10,12,14,16,18,20,22,24,
-        26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,58,60,62,64,66,68,
-        70,72,74,76,78,80,82,84,86,88,90,92,0,5,2,0,9,9,32,32,4,0,17,17,
-        21,21,24,25,32,35,2,0,18,20,22,22,1,0,26,29,1,1,7,7,492,0,94,1,0,
-        0,0,2,123,1,0,0,0,4,127,1,0,0,0,6,134,1,0,0,0,8,148,1,0,0,0,10,150,
-        1,0,0,0,12,155,1,0,0,0,14,163,1,0,0,0,16,168,1,0,0,0,18,172,1,0,
-        0,0,20,185,1,0,0,0,22,193,1,0,0,0,24,196,1,0,0,0,26,203,1,0,0,0,
-        28,215,1,0,0,0,30,217,1,0,0,0,32,222,1,0,0,0,34,227,1,0,0,0,36,230,
-        1,0,0,0,38,234,1,0,0,0,40,269,1,0,0,0,42,271,1,0,0,0,44,276,1,0,
-        0,0,46,295,1,0,0,0,48,297,1,0,0,0,50,299,1,0,0,0,52,306,1,0,0,0,
-        54,308,1,0,0,0,56,310,1,0,0,0,58,312,1,0,0,0,60,318,1,0,0,0,62,320,
-        1,0,0,0,64,323,1,0,0,0,66,326,1,0,0,0,68,329,1,0,0,0,70,350,1,0,
-        0,0,72,352,1,0,0,0,74,356,1,0,0,0,76,360,1,0,0,0,78,382,1,0,0,0,
-        80,404,1,0,0,0,82,426,1,0,0,0,84,439,1,0,0,0,86,451,1,0,0,0,88,455,
-        1,0,0,0,90,459,1,0,0,0,92,465,1,0,0,0,94,118,3,2,1,0,95,97,5,7,0,
-        0,96,95,1,0,0,0,97,98,1,0,0,0,98,96,1,0,0,0,98,99,1,0,0,0,99,103,
-        1,0,0,0,100,102,3,6,3,0,101,100,1,0,0,0,102,105,1,0,0,0,103,101,
-        1,0,0,0,103,104,1,0,0,0,104,109,1,0,0,0,105,103,1,0,0,0,106,108,
-        3,78,39,0,107,106,1,0,0,0,108,111,1,0,0,0,109,107,1,0,0,0,109,110,
-        1,0,0,0,110,115,1,0,0,0,111,109,1,0,0,0,112,114,3,76,38,0,113,112,
-        1,0,0,0,114,117,1,0,0,0,115,113,1,0,0,0,115,116,1,0,0,0,116,119,
-        1,0,0,0,117,115,1,0,0,0,118,96,1,0,0,0,118,119,1,0,0,0,119,120,1,
-        0,0,0,120,121,5,0,0,1,121,1,1,0,0,0,122,124,3,4,2,0,123,122,1,0,
-        0,0,124,125,1,0,0,0,125,123,1,0,0,0,125,126,1,0,0,0,126,3,1,0,0,
-        0,127,129,5,26,0,0,128,130,3,36,18,0,129,128,1,0,0,0,129,130,1,0,
-        0,0,130,131,1,0,0,0,131,132,5,7,0,0,132,5,1,0,0,0,133,135,3,8,4,
-        0,134,133,1,0,0,0,135,136,1,0,0,0,136,134,1,0,0,0,136,137,1,0,0,
-        0,137,141,1,0,0,0,138,140,5,7,0,0,139,138,1,0,0,0,140,143,1,0,0,
-        0,141,139,1,0,0,0,141,142,1,0,0,0,142,7,1,0,0,0,143,141,1,0,0,0,
-        144,149,3,24,12,0,145,149,3,12,6,0,146,149,3,10,5,0,147,149,3,4,
-        2,0,148,144,1,0,0,0,148,145,1,0,0,0,148,146,1,0,0,0,148,147,1,0,
-        0,0,149,9,1,0,0,0,150,151,3,74,37,0,151,152,5,22,0,0,152,153,3,36,
-        18,0,153,154,5,7,0,0,154,11,1,0,0,0,155,156,5,18,0,0,156,160,3,14,
-        7,0,157,159,3,20,10,0,158,157,1,0,0,0,159,162,1,0,0,0,160,158,1,
-        0,0,0,160,161,1,0,0,0,161,13,1,0,0,0,162,160,1,0,0,0,163,164,3,16,
-        8,0,164,165,5,7,0,0,165,15,1,0,0,0,166,167,5,23,0,0,167,169,3,34,
-        17,0,168,166,1,0,0,0,168,169,1,0,0,0,169,170,1,0,0,0,170,171,3,18,
-        9,0,171,17,1,0,0,0,172,182,3,36,18,0,173,175,5,7,0,0,174,176,5,23,
-        0,0,175,174,1,0,0,0,176,177,1,0,0,0,177,175,1,0,0,0,177,178,1,0,
-        0,0,178,179,1,0,0,0,179,181,3,36,18,0,180,173,1,0,0,0,181,184,1,
-        0,0,0,182,180,1,0,0,0,182,183,1,0,0,0,183,19,1,0,0,0,184,182,1,0,
-        0,0,185,186,5,15,0,0,186,190,3,14,7,0,187,189,3,22,11,0,188,187,
-        1,0,0,0,189,192,1,0,0,0,190,188,1,0,0,0,190,191,1,0,0,0,191,21,1,
-        0,0,0,192,190,1,0,0,0,193,194,5,16,0,0,194,195,3,14,7,0,195,23,1,
-        0,0,0,196,200,3,26,13,0,197,199,3,20,10,0,198,197,1,0,0,0,199,202,
-        1,0,0,0,200,198,1,0,0,0,200,201,1,0,0,0,201,25,1,0,0,0,202,200,1,
-        0,0,0,203,206,3,28,14,0,204,205,5,23,0,0,205,207,3,32,16,0,206,204,
-        1,0,0,0,206,207,1,0,0,0,207,208,1,0,0,0,208,209,3,16,8,0,209,210,
-        5,7,0,0,210,27,1,0,0,0,211,216,5,8,0,0,212,216,3,30,15,0,213,216,
-        5,34,0,0,214,216,5,35,0,0,215,211,1,0,0,0,215,212,1,0,0,0,215,213,
-        1,0,0,0,215,214,1,0,0,0,216,29,1,0,0,0,217,220,7,0,0,0,218,219,5,
-        22,0,0,219,221,3,50,25,0,220,218,1,0,0,0,220,221,1,0,0,0,221,31,
-        1,0,0,0,222,223,5,1,0,0,223,224,5,26,0,0,224,225,5,10,0,0,225,226,
-        5,2,0,0,226,33,1,0,0,0,227,228,5,13,0,0,228,35,1,0,0,0,229,231,3,
-        38,19,0,230,229,1,0,0,0,231,232,1,0,0,0,232,230,1,0,0,0,232,233,
-        1,0,0,0,233,37,1,0,0,0,234,237,5,23,0,0,235,236,5,30,0,0,236,238,
-        3,54,27,0,237,235,1,0,0,0,237,238,1,0,0,0,238,243,1,0,0,0,239,242,
-        3,54,27,0,240,242,5,31,0,0,241,239,1,0,0,0,241,240,1,0,0,0,242,245,
-        1,0,0,0,243,241,1,0,0,0,243,244,1,0,0,0,244,248,1,0,0,0,245,243,
-        1,0,0,0,246,249,3,40,20,0,247,249,3,70,35,0,248,246,1,0,0,0,248,
-        247,1,0,0,0,248,249,1,0,0,0,249,258,1,0,0,0,250,255,3,52,26,0,251,
-        254,3,52,26,0,252,254,3,46,23,0,253,251,1,0,0,0,253,252,1,0,0,0,
-        254,257,1,0,0,0,255,253,1,0,0,0,255,256,1,0,0,0,256,259,1,0,0,0,
-        257,255,1,0,0,0,258,250,1,0,0,0,258,259,1,0,0,0,259,261,1,0,0,0,
-        260,262,3,74,37,0,261,260,1,0,0,0,261,262,1,0,0,0,262,39,1,0,0,0,
-        263,270,3,58,29,0,264,270,3,60,30,0,265,270,3,72,36,0,266,270,3,
-        42,21,0,267,270,3,44,22,0,268,270,3,74,37,0,269,263,1,0,0,0,269,
-        264,1,0,0,0,269,265,1,0,0,0,269,266,1,0,0,0,269,267,1,0,0,0,269,
-        268,1,0,0,0,270,41,1,0,0,0,271,272,5,10,0,0,272,273,5,22,0,0,273,
-        274,5,22,0,0,274,275,3,44,22,0,275,43,1,0,0,0,276,286,3,46,23,0,
-        277,279,3,56,28,0,278,277,1,0,0,0,279,280,1,0,0,0,280,278,1,0,0,
-        0,280,281,1,0,0,0,281,282,1,0,0,0,282,283,3,46,23,0,283,285,1,0,
-        0,0,284,278,1,0,0,0,285,288,1,0,0,0,286,284,1,0,0,0,286,287,1,0,
-        0,0,287,45,1,0,0,0,288,286,1,0,0,0,289,296,5,10,0,0,290,296,5,14,
-        0,0,291,296,3,48,24,0,292,296,3,50,25,0,293,296,5,8,0,0,294,296,
-        5,9,0,0,295,289,1,0,0,0,295,290,1,0,0,0,295,291,1,0,0,0,295,292,
-        1,0,0,0,295,293,1,0,0,0,295,294,1,0,0,0,296,47,1,0,0,0,297,298,5,
-        11,0,0,298,49,1,0,0,0,299,300,5,12,0,0,300,51,1,0,0,0,301,307,5,
-        30,0,0,302,307,5,31,0,0,303,307,3,54,27,0,304,307,3,58,29,0,305,
-        307,3,56,28,0,306,301,1,0,0,0,306,302,1,0,0,0,306,303,1,0,0,0,306,
-        304,1,0,0,0,306,305,1,0,0,0,307,53,1,0,0,0,308,309,7,1,0,0,309,55,
-        1,0,0,0,310,311,7,2,0,0,311,57,1,0,0,0,312,313,7,3,0,0,313,59,1,
-        0,0,0,314,319,3,62,31,0,315,319,3,64,32,0,316,319,3,66,33,0,317,
-        319,3,68,34,0,318,314,1,0,0,0,318,315,1,0,0,0,318,316,1,0,0,0,318,
-        317,1,0,0,0,319,61,1,0,0,0,320,321,5,26,0,0,321,322,5,10,0,0,322,
-        63,1,0,0,0,323,324,5,27,0,0,324,325,5,10,0,0,325,65,1,0,0,0,326,
-        327,5,29,0,0,327,328,5,10,0,0,328,67,1,0,0,0,329,330,5,28,0,0,330,
-        331,5,10,0,0,331,69,1,0,0,0,332,337,5,30,0,0,333,338,3,40,20,0,334,
-        338,3,32,16,0,335,338,5,3,0,0,336,338,5,4,0,0,337,333,1,0,0,0,337,
-        334,1,0,0,0,337,335,1,0,0,0,337,336,1,0,0,0,338,339,1,0,0,0,339,
-        337,1,0,0,0,339,340,1,0,0,0,340,341,1,0,0,0,341,351,5,30,0,0,342,
-        344,5,31,0,0,343,345,3,40,20,0,344,343,1,0,0,0,345,346,1,0,0,0,346,
-        344,1,0,0,0,346,347,1,0,0,0,347,348,1,0,0,0,348,349,5,31,0,0,349,
-        351,1,0,0,0,350,332,1,0,0,0,350,342,1,0,0,0,351,71,1,0,0,0,352,353,
-        5,3,0,0,353,354,3,44,22,0,354,355,5,4,0,0,355,73,1,0,0,0,356,357,
-        5,1,0,0,357,358,3,44,22,0,358,359,5,2,0,0,359,75,1,0,0,0,360,364,
-        3,84,42,0,361,363,5,7,0,0,362,361,1,0,0,0,363,366,1,0,0,0,364,362,
-        1,0,0,0,364,365,1,0,0,0,365,370,1,0,0,0,366,364,1,0,0,0,367,369,
-        3,6,3,0,368,367,1,0,0,0,369,372,1,0,0,0,370,368,1,0,0,0,370,371,
-        1,0,0,0,371,379,1,0,0,0,372,370,1,0,0,0,373,375,5,7,0,0,374,373,
-        1,0,0,0,374,375,1,0,0,0,375,376,1,0,0,0,376,378,3,78,39,0,377,374,
-        1,0,0,0,378,381,1,0,0,0,379,377,1,0,0,0,379,380,1,0,0,0,380,77,1,
-        0,0,0,381,379,1,0,0,0,382,386,3,86,43,0,383,385,5,7,0,0,384,383,
-        1,0,0,0,385,388,1,0,0,0,386,384,1,0,0,0,386,387,1,0,0,0,387,392,
-        1,0,0,0,388,386,1,0,0,0,389,391,3,6,3,0,390,389,1,0,0,0,391,394,
-        1,0,0,0,392,390,1,0,0,0,392,393,1,0,0,0,393,401,1,0,0,0,394,392,
-        1,0,0,0,395,397,5,7,0,0,396,395,1,0,0,0,396,397,1,0,0,0,397,398,
-        1,0,0,0,398,400,3,80,40,0,399,396,1,0,0,0,400,403,1,0,0,0,401,399,
-        1,0,0,0,401,402,1,0,0,0,402,79,1,0,0,0,403,401,1,0,0,0,404,408,3,
-        88,44,0,405,407,5,7,0,0,406,405,1,0,0,0,407,410,1,0,0,0,408,406,
-        1,0,0,0,408,409,1,0,0,0,409,414,1,0,0,0,410,408,1,0,0,0,411,413,
-        3,6,3,0,412,411,1,0,0,0,413,416,1,0,0,0,414,412,1,0,0,0,414,415,
-        1,0,0,0,415,423,1,0,0,0,416,414,1,0,0,0,417,419,5,7,0,0,418,417,
-        1,0,0,0,418,419,1,0,0,0,419,420,1,0,0,0,420,422,3,82,41,0,421,418,
-        1,0,0,0,422,425,1,0,0,0,423,421,1,0,0,0,423,424,1,0,0,0,424,81,1,
-        0,0,0,425,423,1,0,0,0,426,430,3,90,45,0,427,429,5,7,0,0,428,427,
-        1,0,0,0,429,432,1,0,0,0,430,428,1,0,0,0,430,431,1,0,0,0,431,436,
-        1,0,0,0,432,430,1,0,0,0,433,435,3,6,3,0,434,433,1,0,0,0,435,438,
-        1,0,0,0,436,434,1,0,0,0,436,437,1,0,0,0,437,83,1,0,0,0,438,436,1,
-        0,0,0,439,440,5,26,0,0,440,441,5,26,0,0,441,442,5,26,0,0,442,443,
+        1,20,1,20,1,20,1,20,3,20,272,8,20,1,21,1,21,1,21,1,21,1,21,1,22,
+        1,22,4,22,281,8,22,11,22,12,22,282,1,22,1,22,5,22,287,8,22,10,22,
+        12,22,290,9,22,1,23,1,23,1,23,1,23,1,23,1,23,3,23,298,8,23,1,24,
+        1,24,1,25,1,25,1,26,1,26,1,26,1,26,1,26,3,26,309,8,26,1,27,1,27,
+        1,28,1,28,1,29,1,29,1,30,1,30,1,30,1,30,3,30,321,8,30,1,31,1,31,
+        1,31,1,32,1,32,1,32,1,33,1,33,1,33,1,34,1,34,1,34,1,35,1,35,1,35,
+        1,35,1,35,4,35,340,8,35,11,35,12,35,341,1,35,1,35,1,35,4,35,347,
+        8,35,11,35,12,35,348,1,35,1,35,3,35,353,8,35,1,36,1,36,1,36,1,36,
+        1,37,1,37,1,37,1,37,1,38,1,38,5,38,365,8,38,10,38,12,38,368,9,38,
+        1,38,5,38,371,8,38,10,38,12,38,374,9,38,1,38,3,38,377,8,38,1,38,
+        5,38,380,8,38,10,38,12,38,383,9,38,1,39,1,39,5,39,387,8,39,10,39,
+        12,39,390,9,39,1,39,5,39,393,8,39,10,39,12,39,396,9,39,1,39,3,39,
+        399,8,39,1,39,5,39,402,8,39,10,39,12,39,405,9,39,1,40,1,40,5,40,
+        409,8,40,10,40,12,40,412,9,40,1,40,5,40,415,8,40,10,40,12,40,418,
+        9,40,1,40,3,40,421,8,40,1,40,5,40,424,8,40,10,40,12,40,427,9,40,
+        1,41,1,41,5,41,431,8,41,10,41,12,41,434,9,41,1,41,5,41,437,8,41,
+        10,41,12,41,440,9,41,1,42,1,42,1,42,1,42,1,42,1,42,1,42,1,42,1,42,
+        1,42,1,42,1,42,1,43,1,43,1,43,1,43,1,44,1,44,1,44,1,44,1,45,1,45,
+        1,45,1,45,1,45,1,45,1,46,1,46,1,46,0,0,47,0,2,4,6,8,10,12,14,16,
+        18,20,22,24,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,58,60,
+        62,64,66,68,70,72,74,76,78,80,82,84,86,88,90,92,0,5,2,0,9,9,32,32,
+        4,0,17,17,21,21,24,25,32,35,2,0,18,20,22,22,1,0,26,29,1,1,7,7,496,
+        0,94,1,0,0,0,2,123,1,0,0,0,4,127,1,0,0,0,6,134,1,0,0,0,8,148,1,0,
+        0,0,10,150,1,0,0,0,12,155,1,0,0,0,14,163,1,0,0,0,16,168,1,0,0,0,
+        18,172,1,0,0,0,20,185,1,0,0,0,22,193,1,0,0,0,24,196,1,0,0,0,26,203,
+        1,0,0,0,28,215,1,0,0,0,30,217,1,0,0,0,32,222,1,0,0,0,34,227,1,0,
+        0,0,36,230,1,0,0,0,38,234,1,0,0,0,40,271,1,0,0,0,42,273,1,0,0,0,
+        44,278,1,0,0,0,46,297,1,0,0,0,48,299,1,0,0,0,50,301,1,0,0,0,52,308,
+        1,0,0,0,54,310,1,0,0,0,56,312,1,0,0,0,58,314,1,0,0,0,60,320,1,0,
+        0,0,62,322,1,0,0,0,64,325,1,0,0,0,66,328,1,0,0,0,68,331,1,0,0,0,
+        70,352,1,0,0,0,72,354,1,0,0,0,74,358,1,0,0,0,76,362,1,0,0,0,78,384,
+        1,0,0,0,80,406,1,0,0,0,82,428,1,0,0,0,84,441,1,0,0,0,86,453,1,0,
+        0,0,88,457,1,0,0,0,90,461,1,0,0,0,92,467,1,0,0,0,94,118,3,2,1,0,
+        95,97,5,7,0,0,96,95,1,0,0,0,97,98,1,0,0,0,98,96,1,0,0,0,98,99,1,
+        0,0,0,99,103,1,0,0,0,100,102,3,6,3,0,101,100,1,0,0,0,102,105,1,0,
+        0,0,103,101,1,0,0,0,103,104,1,0,0,0,104,109,1,0,0,0,105,103,1,0,
+        0,0,106,108,3,78,39,0,107,106,1,0,0,0,108,111,1,0,0,0,109,107,1,
+        0,0,0,109,110,1,0,0,0,110,115,1,0,0,0,111,109,1,0,0,0,112,114,3,
+        76,38,0,113,112,1,0,0,0,114,117,1,0,0,0,115,113,1,0,0,0,115,116,
+        1,0,0,0,116,119,1,0,0,0,117,115,1,0,0,0,118,96,1,0,0,0,118,119,1,
+        0,0,0,119,120,1,0,0,0,120,121,5,0,0,1,121,1,1,0,0,0,122,124,3,4,
+        2,0,123,122,1,0,0,0,124,125,1,0,0,0,125,123,1,0,0,0,125,126,1,0,
+        0,0,126,3,1,0,0,0,127,129,5,26,0,0,128,130,3,36,18,0,129,128,1,0,
+        0,0,129,130,1,0,0,0,130,131,1,0,0,0,131,132,5,7,0,0,132,5,1,0,0,
+        0,133,135,3,8,4,0,134,133,1,0,0,0,135,136,1,0,0,0,136,134,1,0,0,
+        0,136,137,1,0,0,0,137,141,1,0,0,0,138,140,5,7,0,0,139,138,1,0,0,
+        0,140,143,1,0,0,0,141,139,1,0,0,0,141,142,1,0,0,0,142,7,1,0,0,0,
+        143,141,1,0,0,0,144,149,3,24,12,0,145,149,3,12,6,0,146,149,3,10,
+        5,0,147,149,3,4,2,0,148,144,1,0,0,0,148,145,1,0,0,0,148,146,1,0,
+        0,0,148,147,1,0,0,0,149,9,1,0,0,0,150,151,3,74,37,0,151,152,5,22,
+        0,0,152,153,3,36,18,0,153,154,5,7,0,0,154,11,1,0,0,0,155,156,5,18,
+        0,0,156,160,3,14,7,0,157,159,3,20,10,0,158,157,1,0,0,0,159,162,1,
+        0,0,0,160,158,1,0,0,0,160,161,1,0,0,0,161,13,1,0,0,0,162,160,1,0,
+        0,0,163,164,3,16,8,0,164,165,5,7,0,0,165,15,1,0,0,0,166,167,5,23,
+        0,0,167,169,3,34,17,0,168,166,1,0,0,0,168,169,1,0,0,0,169,170,1,
+        0,0,0,170,171,3,18,9,0,171,17,1,0,0,0,172,182,3,36,18,0,173,175,
+        5,7,0,0,174,176,5,23,0,0,175,174,1,0,0,0,176,177,1,0,0,0,177,175,
+        1,0,0,0,177,178,1,0,0,0,178,179,1,0,0,0,179,181,3,36,18,0,180,173,
+        1,0,0,0,181,184,1,0,0,0,182,180,1,0,0,0,182,183,1,0,0,0,183,19,1,
+        0,0,0,184,182,1,0,0,0,185,186,5,15,0,0,186,190,3,14,7,0,187,189,
+        3,22,11,0,188,187,1,0,0,0,189,192,1,0,0,0,190,188,1,0,0,0,190,191,
+        1,0,0,0,191,21,1,0,0,0,192,190,1,0,0,0,193,194,5,16,0,0,194,195,
+        3,14,7,0,195,23,1,0,0,0,196,200,3,26,13,0,197,199,3,20,10,0,198,
+        197,1,0,0,0,199,202,1,0,0,0,200,198,1,0,0,0,200,201,1,0,0,0,201,
+        25,1,0,0,0,202,200,1,0,0,0,203,206,3,28,14,0,204,205,5,23,0,0,205,
+        207,3,32,16,0,206,204,1,0,0,0,206,207,1,0,0,0,207,208,1,0,0,0,208,
+        209,3,16,8,0,209,210,5,7,0,0,210,27,1,0,0,0,211,216,5,8,0,0,212,
+        216,3,30,15,0,213,216,5,34,0,0,214,216,5,35,0,0,215,211,1,0,0,0,
+        215,212,1,0,0,0,215,213,1,0,0,0,215,214,1,0,0,0,216,29,1,0,0,0,217,
+        220,7,0,0,0,218,219,5,22,0,0,219,221,3,50,25,0,220,218,1,0,0,0,220,
+        221,1,0,0,0,221,31,1,0,0,0,222,223,5,1,0,0,223,224,5,26,0,0,224,
+        225,5,10,0,0,225,226,5,2,0,0,226,33,1,0,0,0,227,228,5,13,0,0,228,
+        35,1,0,0,0,229,231,3,38,19,0,230,229,1,0,0,0,231,232,1,0,0,0,232,
+        230,1,0,0,0,232,233,1,0,0,0,233,37,1,0,0,0,234,237,5,23,0,0,235,
+        236,5,30,0,0,236,238,3,54,27,0,237,235,1,0,0,0,237,238,1,0,0,0,238,
+        243,1,0,0,0,239,242,3,54,27,0,240,242,5,31,0,0,241,239,1,0,0,0,241,
+        240,1,0,0,0,242,245,1,0,0,0,243,241,1,0,0,0,243,244,1,0,0,0,244,
+        248,1,0,0,0,245,243,1,0,0,0,246,249,3,40,20,0,247,249,3,70,35,0,
+        248,246,1,0,0,0,248,247,1,0,0,0,248,249,1,0,0,0,249,258,1,0,0,0,
+        250,255,3,52,26,0,251,254,3,52,26,0,252,254,3,46,23,0,253,251,1,
+        0,0,0,253,252,1,0,0,0,254,257,1,0,0,0,255,253,1,0,0,0,255,256,1,
+        0,0,0,256,259,1,0,0,0,257,255,1,0,0,0,258,250,1,0,0,0,258,259,1,
+        0,0,0,259,261,1,0,0,0,260,262,3,74,37,0,261,260,1,0,0,0,261,262,
+        1,0,0,0,262,39,1,0,0,0,263,272,3,58,29,0,264,272,3,60,30,0,265,272,
+        3,72,36,0,266,272,3,42,21,0,267,272,3,44,22,0,268,272,3,74,37,0,
+        269,272,3,34,17,0,270,272,3,32,16,0,271,263,1,0,0,0,271,264,1,0,
+        0,0,271,265,1,0,0,0,271,266,1,0,0,0,271,267,1,0,0,0,271,268,1,0,
+        0,0,271,269,1,0,0,0,271,270,1,0,0,0,272,41,1,0,0,0,273,274,5,10,
+        0,0,274,275,5,22,0,0,275,276,5,22,0,0,276,277,3,44,22,0,277,43,1,
+        0,0,0,278,288,3,46,23,0,279,281,3,56,28,0,280,279,1,0,0,0,281,282,
+        1,0,0,0,282,280,1,0,0,0,282,283,1,0,0,0,283,284,1,0,0,0,284,285,
+        3,46,23,0,285,287,1,0,0,0,286,280,1,0,0,0,287,290,1,0,0,0,288,286,
+        1,0,0,0,288,289,1,0,0,0,289,45,1,0,0,0,290,288,1,0,0,0,291,298,5,
+        10,0,0,292,298,5,14,0,0,293,298,3,48,24,0,294,298,3,50,25,0,295,
+        298,5,8,0,0,296,298,5,9,0,0,297,291,1,0,0,0,297,292,1,0,0,0,297,
+        293,1,0,0,0,297,294,1,0,0,0,297,295,1,0,0,0,297,296,1,0,0,0,298,
+        47,1,0,0,0,299,300,5,11,0,0,300,49,1,0,0,0,301,302,5,12,0,0,302,
+        51,1,0,0,0,303,309,5,30,0,0,304,309,5,31,0,0,305,309,3,54,27,0,306,
+        309,3,58,29,0,307,309,3,56,28,0,308,303,1,0,0,0,308,304,1,0,0,0,
+        308,305,1,0,0,0,308,306,1,0,0,0,308,307,1,0,0,0,309,53,1,0,0,0,310,
+        311,7,1,0,0,311,55,1,0,0,0,312,313,7,2,0,0,313,57,1,0,0,0,314,315,
+        7,3,0,0,315,59,1,0,0,0,316,321,3,62,31,0,317,321,3,64,32,0,318,321,
+        3,66,33,0,319,321,3,68,34,0,320,316,1,0,0,0,320,317,1,0,0,0,320,
+        318,1,0,0,0,320,319,1,0,0,0,321,61,1,0,0,0,322,323,5,26,0,0,323,
+        324,5,10,0,0,324,63,1,0,0,0,325,326,5,27,0,0,326,327,5,10,0,0,327,
+        65,1,0,0,0,328,329,5,29,0,0,329,330,5,10,0,0,330,67,1,0,0,0,331,
+        332,5,28,0,0,332,333,5,10,0,0,333,69,1,0,0,0,334,339,5,30,0,0,335,
+        340,3,40,20,0,336,340,3,32,16,0,337,340,5,3,0,0,338,340,5,4,0,0,
+        339,335,1,0,0,0,339,336,1,0,0,0,339,337,1,0,0,0,339,338,1,0,0,0,
+        340,341,1,0,0,0,341,339,1,0,0,0,341,342,1,0,0,0,342,343,1,0,0,0,
+        343,353,5,30,0,0,344,346,5,31,0,0,345,347,3,40,20,0,346,345,1,0,
+        0,0,347,348,1,0,0,0,348,346,1,0,0,0,348,349,1,0,0,0,349,350,1,0,
+        0,0,350,351,5,31,0,0,351,353,1,0,0,0,352,334,1,0,0,0,352,344,1,0,
+        0,0,353,71,1,0,0,0,354,355,5,3,0,0,355,356,3,44,22,0,356,357,5,4,
+        0,0,357,73,1,0,0,0,358,359,5,1,0,0,359,360,3,44,22,0,360,361,5,2,
+        0,0,361,75,1,0,0,0,362,366,3,84,42,0,363,365,5,7,0,0,364,363,1,0,
+        0,0,365,368,1,0,0,0,366,364,1,0,0,0,366,367,1,0,0,0,367,372,1,0,
+        0,0,368,366,1,0,0,0,369,371,3,6,3,0,370,369,1,0,0,0,371,374,1,0,
+        0,0,372,370,1,0,0,0,372,373,1,0,0,0,373,381,1,0,0,0,374,372,1,0,
+        0,0,375,377,5,7,0,0,376,375,1,0,0,0,376,377,1,0,0,0,377,378,1,0,
+        0,0,378,380,3,78,39,0,379,376,1,0,0,0,380,383,1,0,0,0,381,379,1,
+        0,0,0,381,382,1,0,0,0,382,77,1,0,0,0,383,381,1,0,0,0,384,388,3,86,
+        43,0,385,387,5,7,0,0,386,385,1,0,0,0,387,390,1,0,0,0,388,386,1,0,
+        0,0,388,389,1,0,0,0,389,394,1,0,0,0,390,388,1,0,0,0,391,393,3,6,
+        3,0,392,391,1,0,0,0,393,396,1,0,0,0,394,392,1,0,0,0,394,395,1,0,
+        0,0,395,403,1,0,0,0,396,394,1,0,0,0,397,399,5,7,0,0,398,397,1,0,
+        0,0,398,399,1,0,0,0,399,400,1,0,0,0,400,402,3,80,40,0,401,398,1,
+        0,0,0,402,405,1,0,0,0,403,401,1,0,0,0,403,404,1,0,0,0,404,79,1,0,
+        0,0,405,403,1,0,0,0,406,410,3,88,44,0,407,409,5,7,0,0,408,407,1,
+        0,0,0,409,412,1,0,0,0,410,408,1,0,0,0,410,411,1,0,0,0,411,416,1,
+        0,0,0,412,410,1,0,0,0,413,415,3,6,3,0,414,413,1,0,0,0,415,418,1,
+        0,0,0,416,414,1,0,0,0,416,417,1,0,0,0,417,425,1,0,0,0,418,416,1,
+        0,0,0,419,421,5,7,0,0,420,419,1,0,0,0,420,421,1,0,0,0,421,422,1,
+        0,0,0,422,424,3,82,41,0,423,420,1,0,0,0,424,427,1,0,0,0,425,423,
+        1,0,0,0,425,426,1,0,0,0,426,81,1,0,0,0,427,425,1,0,0,0,428,432,3,
+        90,45,0,429,431,5,7,0,0,430,429,1,0,0,0,431,434,1,0,0,0,432,430,
+        1,0,0,0,432,433,1,0,0,0,433,438,1,0,0,0,434,432,1,0,0,0,435,437,
+        3,6,3,0,436,435,1,0,0,0,437,440,1,0,0,0,438,436,1,0,0,0,438,439,
+        1,0,0,0,439,83,1,0,0,0,440,438,1,0,0,0,441,442,5,26,0,0,442,443,
         5,26,0,0,443,444,5,26,0,0,444,445,5,26,0,0,445,446,5,26,0,0,446,
-        447,5,26,0,0,447,448,5,26,0,0,448,449,3,36,18,0,449,450,3,92,46,
-        0,450,85,1,0,0,0,451,452,5,5,0,0,452,453,3,36,18,0,453,454,3,92,
-        46,0,454,87,1,0,0,0,455,456,5,6,0,0,456,457,3,36,18,0,457,458,3,
-        92,46,0,458,89,1,0,0,0,459,460,5,18,0,0,460,461,5,18,0,0,461,462,
-        5,18,0,0,462,463,3,36,18,0,463,464,3,92,46,0,464,91,1,0,0,0,465,
-        466,7,4,0,0,466,93,1,0,0,0,52,98,103,109,115,118,125,129,136,141,
-        148,160,168,177,182,190,200,206,215,220,232,237,241,243,248,253,
-        255,258,261,269,280,286,295,306,318,337,339,346,350,364,370,374,
-        379,386,392,396,401,408,414,418,423,430,436
+        447,5,26,0,0,447,448,5,26,0,0,448,449,5,26,0,0,449,450,5,26,0,0,
+        450,451,3,36,18,0,451,452,3,92,46,0,452,85,1,0,0,0,453,454,5,5,0,
+        0,454,455,3,36,18,0,455,456,3,92,46,0,456,87,1,0,0,0,457,458,5,6,
+        0,0,458,459,3,36,18,0,459,460,3,92,46,0,460,89,1,0,0,0,461,462,5,
+        18,0,0,462,463,5,18,0,0,463,464,5,18,0,0,464,465,3,36,18,0,465,466,
+        3,92,46,0,466,91,1,0,0,0,467,468,7,4,0,0,468,93,1,0,0,0,52,98,103,
+        109,115,118,125,129,136,141,148,160,168,177,182,190,200,206,215,
+        220,232,237,241,243,248,253,255,258,261,271,282,288,297,308,320,
+        339,341,348,352,366,372,376,381,388,394,398,403,410,416,420,425,
+        432,438
     ]
 
 class ZorgFileParser ( Parser ):
 
     grammarFileName = "ZorgFile.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
@@ -1735,14 +1737,22 @@
             return self.getTypedRuleContext(ZorgFileParser.Id_groupContext,0)
 
 
         def ref(self):
             return self.getTypedRuleContext(ZorgFileParser.RefContext,0)
 
 
+        def zid(self):
+            return self.getTypedRuleContext(ZorgFileParser.ZidContext,0)
+
+
+        def priority(self):
+            return self.getTypedRuleContext(ZorgFileParser.PriorityContext,0)
+
+
         def getRuleIndex(self):
             return ZorgFileParser.RULE_atom
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterAtom" ):
                 listener.enterAtom(self)
 
@@ -1754,15 +1764,15 @@
 
 
     def atom(self):
 
         localctx = ZorgFileParser.AtomContext(self, self._ctx, self.state)
         self.enterRule(localctx, 40, self.RULE_atom)
         try:
-            self.state = 269
+            self.state = 271
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,28,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
                 self.state = 263
                 self.tag_symbol()
                 pass
@@ -1793,14 +1803,26 @@
 
             elif la_ == 6:
                 self.enterOuterAlt(localctx, 6)
                 self.state = 268
                 self.ref()
                 pass
 
+            elif la_ == 7:
+                self.enterOuterAlt(localctx, 7)
+                self.state = 269
+                self.zid()
+                pass
+
+            elif la_ == 8:
+                self.enterOuterAlt(localctx, 8)
+                self.state = 270
+                self.priority()
+                pass
+
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1843,21 +1865,21 @@
 
     def property_(self):
 
         localctx = ZorgFileParser.PropertyContext(self, self._ctx, self.state)
         self.enterRule(localctx, 42, self.RULE_property)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 271
+            self.state = 273
             self.match(ZorgFileParser.ID)
-            self.state = 272
+            self.state = 274
             self.match(ZorgFileParser.COLON)
-            self.state = 273
+            self.state = 275
             self.match(ZorgFileParser.COLON)
-            self.state = 274
+            self.state = 276
             self.id_group()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1902,36 +1924,36 @@
     def id_group(self):
 
         localctx = ZorgFileParser.Id_groupContext(self, self._ctx, self.state)
         self.enterRule(localctx, 44, self.RULE_id_group)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 276
+            self.state = 278
             self.id_()
-            self.state = 286
+            self.state = 288
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,30,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 278 
+                    self.state = 280 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     while True:
-                        self.state = 277
+                        self.state = 279
                         self.id_symbol()
-                        self.state = 280 
+                        self.state = 282 
                         self._errHandler.sync(self)
                         _la = self._input.LA(1)
                         if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 6029312) != 0)):
                             break
 
-                    self.state = 282
+                    self.state = 284
                     self.id_() 
-                self.state = 288
+                self.state = 290
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,30,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1982,45 +2004,45 @@
 
 
     def id_(self):
 
         localctx = ZorgFileParser.IdContext(self, self._ctx, self.state)
         self.enterRule(localctx, 46, self.RULE_id)
         try:
-            self.state = 295
+            self.state = 297
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [10]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 289
+                self.state = 291
                 self.match(ZorgFileParser.ID)
                 pass
             elif token in [14]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 290
+                self.state = 292
                 self.match(ZorgFileParser.NUM_ID)
                 pass
             elif token in [11]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 291
+                self.state = 293
                 self.date()
                 pass
             elif token in [12]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 292
+                self.state = 294
                 self.time()
                 pass
             elif token in [8]:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 293
+                self.state = 295
                 self.match(ZorgFileParser.LOWER_O)
                 pass
             elif token in [9]:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 294
+                self.state = 296
                 self.match(ZorgFileParser.LOWER_X)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2057,15 +2079,15 @@
 
     def date(self):
 
         localctx = ZorgFileParser.DateContext(self, self._ctx, self.state)
         self.enterRule(localctx, 48, self.RULE_date)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 297
+            self.state = 299
             self.match(ZorgFileParser.DATE)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2098,15 +2120,15 @@
 
     def time(self):
 
         localctx = ZorgFileParser.TimeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 50, self.RULE_time)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 299
+            self.state = 301
             self.match(ZorgFileParser.TIME)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2153,40 +2175,40 @@
 
 
     def any_symbol(self):
 
         localctx = ZorgFileParser.Any_symbolContext(self, self._ctx, self.state)
         self.enterRule(localctx, 52, self.RULE_any_symbol)
         try:
-            self.state = 306
+            self.state = 308
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [30]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 301
+                self.state = 303
                 self.match(ZorgFileParser.SQUOTE)
                 pass
             elif token in [31]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 302
+                self.state = 304
                 self.match(ZorgFileParser.DQUOTE)
                 pass
             elif token in [17, 21, 24, 25, 32, 33, 34, 35]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 303
+                self.state = 305
                 self.non_tag_symbol()
                 pass
             elif token in [26, 27, 28, 29]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 304
+                self.state = 306
                 self.tag_symbol()
                 pass
             elif token in [18, 19, 20, 22]:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 305
+                self.state = 307
                 self.id_symbol()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2245,15 +2267,15 @@
     def non_tag_symbol(self):
 
         localctx = ZorgFileParser.Non_tag_symbolContext(self, self._ctx, self.state)
         self.enterRule(localctx, 54, self.RULE_non_tag_symbol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 308
+            self.state = 310
             _la = self._input.LA(1)
             if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 64477069312) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
@@ -2301,15 +2323,15 @@
     def id_symbol(self):
 
         localctx = ZorgFileParser.Id_symbolContext(self, self._ctx, self.state)
         self.enterRule(localctx, 56, self.RULE_id_symbol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 310
+            self.state = 312
             _la = self._input.LA(1)
             if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 6029312) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
@@ -2357,15 +2379,15 @@
     def tag_symbol(self):
 
         localctx = ZorgFileParser.Tag_symbolContext(self, self._ctx, self.state)
         self.enterRule(localctx, 58, self.RULE_tag_symbol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 312
+            self.state = 314
             _la = self._input.LA(1)
             if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006632960) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
@@ -2415,35 +2437,35 @@
 
 
     def tag(self):
 
         localctx = ZorgFileParser.TagContext(self, self._ctx, self.state)
         self.enterRule(localctx, 60, self.RULE_tag)
         try:
-            self.state = 318
+            self.state = 320
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [26]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 314
+                self.state = 316
                 self.area()
                 pass
             elif token in [27]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 315
+                self.state = 317
                 self.context()
                 pass
             elif token in [29]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 316
+                self.state = 318
                 self.person()
                 pass
             elif token in [28]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 317
+                self.state = 319
                 self.project()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2483,17 +2505,17 @@
 
     def area(self):
 
         localctx = ZorgFileParser.AreaContext(self, self._ctx, self.state)
         self.enterRule(localctx, 62, self.RULE_area)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 320
+            self.state = 322
             self.match(ZorgFileParser.HASH)
-            self.state = 321
+            self.state = 323
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2529,17 +2551,17 @@
 
     def context(self):
 
         localctx = ZorgFileParser.ContextContext(self, self._ctx, self.state)
         self.enterRule(localctx, 64, self.RULE_context)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 323
+            self.state = 325
             self.match(ZorgFileParser.AT_SIGN)
-            self.state = 324
+            self.state = 326
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2575,17 +2597,17 @@
 
     def person(self):
 
         localctx = ZorgFileParser.PersonContext(self, self._ctx, self.state)
         self.enterRule(localctx, 66, self.RULE_person)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 326
+            self.state = 328
             self.match(ZorgFileParser.PERCENT)
-            self.state = 327
+            self.state = 329
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2621,17 +2643,17 @@
 
     def project(self):
 
         localctx = ZorgFileParser.ProjectContext(self, self._ctx, self.state)
         self.enterRule(localctx, 68, self.RULE_project)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 329
+            self.state = 331
             self.match(ZorgFileParser.PLUS)
-            self.state = 330
+            self.state = 332
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2688,73 +2710,73 @@
     def quoted(self):
 
         localctx = ZorgFileParser.QuotedContext(self, self._ctx, self.state)
         self.enterRule(localctx, 70, self.RULE_quoted)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 350
+            self.state = 352
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [30]:
-                self.state = 332
+                self.state = 334
                 self.match(ZorgFileParser.SQUOTE)
-                self.state = 337 
+                self.state = 339 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while True:
-                    self.state = 337
+                    self.state = 339
                     self._errHandler.sync(self)
                     la_ = self._interp.adaptivePredict(self._input,34,self._ctx)
                     if la_ == 1:
-                        self.state = 333
+                        self.state = 335
                         self.atom()
                         pass
 
                     elif la_ == 2:
-                        self.state = 334
+                        self.state = 336
                         self.priority()
                         pass
 
                     elif la_ == 3:
-                        self.state = 335
+                        self.state = 337
                         self.match(ZorgFileParser.T__2)
                         pass
 
                     elif la_ == 4:
-                        self.state = 336
+                        self.state = 338
                         self.match(ZorgFileParser.T__3)
                         pass
 
 
-                    self.state = 339 
+                    self.state = 341 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006657306) != 0)):
+                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006665498) != 0)):
                         break
 
-                self.state = 341
+                self.state = 343
                 self.match(ZorgFileParser.SQUOTE)
                 pass
             elif token in [31]:
-                self.state = 342
+                self.state = 344
                 self.match(ZorgFileParser.DQUOTE)
-                self.state = 344 
+                self.state = 346 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while True:
-                    self.state = 343
+                    self.state = 345
                     self.atom()
-                    self.state = 346 
+                    self.state = 348 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006657290) != 0)):
+                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006665482) != 0)):
                         break
 
-                self.state = 348
+                self.state = 350
                 self.match(ZorgFileParser.DQUOTE)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2792,19 +2814,19 @@
 
     def link(self):
 
         localctx = ZorgFileParser.LinkContext(self, self._ctx, self.state)
         self.enterRule(localctx, 72, self.RULE_link)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 352
+            self.state = 354
             self.match(ZorgFileParser.T__2)
-            self.state = 353
+            self.state = 355
             self.id_group()
-            self.state = 354
+            self.state = 356
             self.match(ZorgFileParser.T__3)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2838,19 +2860,19 @@
 
     def ref(self):
 
         localctx = ZorgFileParser.RefContext(self, self._ctx, self.state)
         self.enterRule(localctx, 74, self.RULE_ref)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 356
+            self.state = 358
             self.match(ZorgFileParser.T__0)
-            self.state = 357
+            self.state = 359
             self.id_group()
-            self.state = 358
+            self.state = 360
             self.match(ZorgFileParser.T__1)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2905,53 +2927,53 @@
     def h1_section(self):
 
         localctx = ZorgFileParser.H1_sectionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 76, self.RULE_h1_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 360
+            self.state = 362
             self.h1_header()
-            self.state = 364
+            self.state = 366
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 361
+                    self.state = 363
                     self.match(ZorgFileParser.NL) 
-                self.state = 366
+                self.state = 368
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
 
-            self.state = 370
+            self.state = 372
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,39,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 367
+                    self.state = 369
                     self.block() 
-                self.state = 372
+                self.state = 374
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,39,self._ctx)
 
-            self.state = 379
+            self.state = 381
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==5 or _la==7:
-                self.state = 374
+                self.state = 376
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la==7:
-                    self.state = 373
+                    self.state = 375
                     self.match(ZorgFileParser.NL)
 
 
-                self.state = 376
+                self.state = 378
                 self.h2_section()
-                self.state = 381
+                self.state = 383
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3008,54 +3030,54 @@
     def h2_section(self):
 
         localctx = ZorgFileParser.H2_sectionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 78, self.RULE_h2_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 382
+            self.state = 384
             self.h2_header()
-            self.state = 386
+            self.state = 388
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 383
+                    self.state = 385
                     self.match(ZorgFileParser.NL) 
-                self.state = 388
+                self.state = 390
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
 
-            self.state = 392
+            self.state = 394
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,43,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 389
+                    self.state = 391
                     self.block() 
-                self.state = 394
+                self.state = 396
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,43,self._ctx)
 
-            self.state = 401
+            self.state = 403
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 396
+                    self.state = 398
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la==7:
-                        self.state = 395
+                        self.state = 397
                         self.match(ZorgFileParser.NL)
 
 
-                    self.state = 398
+                    self.state = 400
                     self.h3_section() 
-                self.state = 403
+                self.state = 405
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3112,54 +3134,54 @@
     def h3_section(self):
 
         localctx = ZorgFileParser.H3_sectionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 80, self.RULE_h3_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 404
+            self.state = 406
             self.h3_header()
-            self.state = 408
+            self.state = 410
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 405
+                    self.state = 407
                     self.match(ZorgFileParser.NL) 
-                self.state = 410
+                self.state = 412
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
 
-            self.state = 414
+            self.state = 416
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,47,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 411
+                    self.state = 413
                     self.block() 
-                self.state = 416
+                self.state = 418
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,47,self._ctx)
 
-            self.state = 423
+            self.state = 425
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 418
+                    self.state = 420
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la==7:
-                        self.state = 417
+                        self.state = 419
                         self.match(ZorgFileParser.NL)
 
 
-                    self.state = 420
+                    self.state = 422
                     self.h4_section() 
-                self.state = 425
+                self.state = 427
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3208,35 +3230,35 @@
 
     def h4_section(self):
 
         localctx = ZorgFileParser.H4_sectionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 82, self.RULE_h4_section)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 426
+            self.state = 428
             self.h4_header()
-            self.state = 430
+            self.state = 432
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 427
+                    self.state = 429
                     self.match(ZorgFileParser.NL) 
-                self.state = 432
+                self.state = 434
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
 
-            self.state = 436
+            self.state = 438
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 433
+                    self.state = 435
                     self.block() 
-                self.state = 438
+                self.state = 440
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3282,18 +3304,14 @@
 
     def h1_header(self):
 
         localctx = ZorgFileParser.H1_headerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 84, self.RULE_h1_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 439
-            self.match(ZorgFileParser.HASH)
-            self.state = 440
-            self.match(ZorgFileParser.HASH)
             self.state = 441
             self.match(ZorgFileParser.HASH)
             self.state = 442
             self.match(ZorgFileParser.HASH)
             self.state = 443
             self.match(ZorgFileParser.HASH)
             self.state = 444
@@ -3301,16 +3319,20 @@
             self.state = 445
             self.match(ZorgFileParser.HASH)
             self.state = 446
             self.match(ZorgFileParser.HASH)
             self.state = 447
             self.match(ZorgFileParser.HASH)
             self.state = 448
-            self.space_atoms()
+            self.match(ZorgFileParser.HASH)
             self.state = 449
+            self.match(ZorgFileParser.HASH)
+            self.state = 450
+            self.space_atoms()
+            self.state = 451
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3348,19 +3370,19 @@
 
     def h2_header(self):
 
         localctx = ZorgFileParser.H2_headerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 86, self.RULE_h2_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 451
+            self.state = 453
             self.match(ZorgFileParser.T__4)
-            self.state = 452
+            self.state = 454
             self.space_atoms()
-            self.state = 453
+            self.state = 455
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3398,19 +3420,19 @@
 
     def h3_header(self):
 
         localctx = ZorgFileParser.H3_headerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 88, self.RULE_h3_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 455
+            self.state = 457
             self.match(ZorgFileParser.T__5)
-            self.state = 456
+            self.state = 458
             self.space_atoms()
-            self.state = 457
+            self.state = 459
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3454,23 +3476,23 @@
 
     def h4_header(self):
 
         localctx = ZorgFileParser.H4_headerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 90, self.RULE_h4_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 459
-            self.match(ZorgFileParser.DASH)
-            self.state = 460
-            self.match(ZorgFileParser.DASH)
             self.state = 461
             self.match(ZorgFileParser.DASH)
             self.state = 462
-            self.space_atoms()
+            self.match(ZorgFileParser.DASH)
             self.state = 463
+            self.match(ZorgFileParser.DASH)
+            self.state = 464
+            self.space_atoms()
+            self.state = 465
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3507,15 +3529,15 @@
     def eol(self):
 
         localctx = ZorgFileParser.EolContext(self, self._ctx, self.state)
         self.enterRule(localctx, 92, self.RULE_eol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 465
+            self.state = 467
             _la = self._input.LA(1)
             if not(_la==-1 or _la==7):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
```

### Comparing `zettel_org-0.6.3/src/zorg/service/common.py` & `zettel_org-0.6.4/src/zorg/service/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,11 +31,16 @@
         path = Path(p)
         new_paths.append(
             path if zdir_path in path.parents else zdir_path / path
         )
     return new_paths
 
 
+def strip_zdir(zdir: PathLike, path: PathLike) -> str:
+    """Strips {zdir} from {path}."""
+    return str(path).replace(f"{zdir}/", "")
+
+
 def _var_map_value(value: str) -> Any:
     if re.match("^[0-9]{4}[01][0-9][0-3][0-9]$", value):
         return dt.datetime.strptime(value, "%Y%m%d")
     return value
```

### Comparing `zettel_org-0.6.3/src/zorg/service/compiler.py` & `zettel_org-0.6.4/src/zorg/service/compiler/_file_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 """Contains service logic used to compile zorg files."""
 
 from dataclasses import dataclass, field
 import datetime as dt
 from functools import partial
-from pathlib import Path
 from typing import Any, Literal, Optional
 
 import antlr4
 from antlr4.error.ErrorListener import ErrorListener
 from logrus import Logger
 from typist import assert_never
 
-from ..domain.models import TodoPayload, ZorgFile, ZorgNote
-from ..domain.types import TodoPriorityType, TodoStatus, TodoStatusPrefixChar
-from ..grammar.zorg_file.ZorgFileLexer import ZorgFileLexer
-from ..grammar.zorg_file.ZorgFileListener import ZorgFileListener
-from ..grammar.zorg_file.ZorgFileParser import ZorgFileParser
+from ...domain.models import TodoPayload, ZorgFile, ZorgNote
+from ...domain.types import TodoPriorityType, TodoStatus, TodoStatusPrefixChar
+from ...grammar.zorg_file.ZorgFileListener import ZorgFileListener
+from ...grammar.zorg_file.ZorgFileParser import ZorgFileParser
 
 
 TagName = Literal["areas", "contexts", "people", "projects"]
 
-logger = Logger(__name__)
+_LOGGER = Logger(__name__)
 
 
-class _ErrorManager(ErrorListener):
+class ErrorManager(ErrorListener):
     """Keeps track of zorg file syntax errors."""
 
     def __init__(self) -> None:
         super().__init__()
         self.errors: list[str] = []
 
     def syntaxError(
@@ -39,19 +37,23 @@
         msg: str,
         e: Any,
     ) -> None:  # noqa: D102
         del recognizer, offendingSymbol, e
         self.errors.append(f"Line {line}:{column} {msg}")
 
 
-class _ZorgFileCompiler(ZorgFileListener):
-    """Listener that compiles zorg files into zorc files."""
+class ZorgFileCompiler(ZorgFileListener):
+    """Listener that compiles zorg files.
+
+    This compiler takes as input a single *.zo file. When walked, it produces
+    as output the {zorg_file} instance attribute.
+    """
 
     def __init__(
-        self, zorg_file: ZorgFile, error_manager: _ErrorManager
+        self, zorg_file: ZorgFile, error_manager: ErrorManager
     ) -> None:
         self.zorg_file = zorg_file
         self.error_manager = error_manager
 
         self._s = _ZorgFileCompilerState()
 
     def enterArea(self, ctx: ZorgFileParser.AreaContext) -> None:  # noqa: D102
@@ -227,19 +229,19 @@
                 "todo_payload": TodoPayload(
                     priority=self._s.todo_priority, status=self._s.todo_status
                 ),
             },
         )
         id_note_body = ctx.id_note_body()
         if id_note_body is None:
-            logger.warning("Skipping todo with no note body")
+            _LOGGER.warning("Skipping todo with no note body")
         elif id_note_body.getText().strip() == "":
-            logger.warning("Skipping todo with empty note body")
+            _LOGGER.warning("Skipping todo with empty note body")
         elif self.error_manager.errors:
-            logger.warning(
+            _LOGGER.warning(
                 "Skipping note since zorg file has errors.",
                 file_path=str(self.zorg_file.path),
             )
             self.zorg_file.has_errors = True
         else:
             todo = ZorgNote(id_note_body.getText(), **kwargs)
             self.zorg_file.notes.append(todo)
@@ -320,22 +322,22 @@
         self._s.in_note = False
         extra_kwargs = {}
         if self._s.parent_id is not None:
             extra_kwargs["parent_note_id"] = self._s.parent_id
         kwargs = self._get_note_kwargs(ctx, extra_kwargs)
         body: str = ctx.id_note_body().getText().strip()
         if body == "":
-            logger.warning(
+            _LOGGER.warning(
                 "Skipping note with empty body",
                 file_path=str(self.zorg_file.path),
             )
             return
 
         if self.error_manager.errors:
-            logger.warning(
+            _LOGGER.warning(
                 "Skipping note since zorg file has errors.",
                 file_path=str(self.zorg_file.path),
             )
             self.zorg_file.has_errors = True
             return
 
         note = ZorgNote(body, **kwargs)
@@ -386,15 +388,15 @@
         self._s.note_date = None
 
     def _add_tags(
         self, ctx: antlr4.ParserRuleContext, tag_name: TagName
     ) -> None:
         text = ctx.children[1].getText()
         if all(ch.isdigit() for ch in text):
-            logger.debug(
+            _LOGGER.debug(
                 "Tag identifiers cannot contain only digits.",
                 tag_name=tag_name,
                 ID=text,
             )
             return
         if self._s.in_first_comment:
             self._s.file_tags[tag_name].append(text)
@@ -406,37 +408,14 @@
             self._s.h3_tags[tag_name].append(text)
         elif self._s.in_h4_header:
             self._s.h4_tags[tag_name].append(text)
         elif self._s.in_note:
             self._s.note_tags[tag_name].append(text)
 
 
-def walk_zorg_file(
-    zdir: Path, zo_path_part: Path, verbose: bool = False
-) -> ZorgFile:
-    """Create a new _ZorgFileCompiler and walk through notes in {zorg_file}."""
-    zo_path = (
-        zo_path_part if zo_path_part.is_absolute() else zdir / zo_path_part
-    )
-    zorg_file = ZorgFile(zo_path)
-    stream = antlr4.FileStream(zorg_file.path, errors="ignore")
-    lexer = ZorgFileLexer(stream)
-    tokens = antlr4.CommonTokenStream(lexer)
-    parser = ZorgFileParser(tokens)
-    if not verbose:
-        parser.removeErrorListeners()
-    error_manager = _ErrorManager()
-    parser.addErrorListener(error_manager)
-    tree = parser.prog()
-    compiler = _ZorgFileCompiler(zorg_file, error_manager)
-    walker = antlr4.ParseTreeWalker()
-    walker.walk(compiler, tree)
-    return zorg_file
-
-
 def _get_default_tags_map() -> dict[TagName, list[str]]:
     return {"areas": [], "projects": [], "contexts": [], "people": []}
 
 
 @dataclass
 class _ZorgFileCompilerState:
     """Serves as a data store while parsing zorg files."""
```

### Comparing `zettel_org-0.6.3/src/zorg/service/file_groups.py` & `zettel_org-0.6.4/src/zorg/service/file_groups.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/service/handlers.py` & `zettel_org-0.6.4/src/zorg/service/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import sys
 from typing import Iterable, Iterator
 
 from logrus import Logger
 from tqdm import tqdm
 import vimala
 
+from . import common
 from .. import APP_NAME
 from ..domain.messages import commands, events
 from ..storage.sql.session import SQLSession
-from .common import prepend_zdir
 from .compiler import walk_zorg_file
 from .zid_manager import ZIDManager
 
 
 logger = Logger(__name__)
 
 
@@ -44,15 +44,15 @@
     if event.edit_cmd.keep_alive_file.stat().st_size == 0:
         logger.debug(
             "Empty keep alive file found.",
             keep_alive_file=event.edit_cmd.keep_alive_file,
         )
         paths = event.edit_cmd.paths
     else:
-        new_paths = prepend_zdir(
+        new_paths = common.prepend_zdir(
             event.edit_cmd.zettel_dir,
             [
                 Path(p.strip())
                 for p in event.edit_cmd.keep_alive_file.read_text().split()
             ],
         )
         logger.debug(
@@ -117,17 +117,16 @@
 def reindex_database(
     cmd: commands.ReindexDBCommand, session: SQLSession
 ) -> None:
     """Reindex an existing zorg database."""
     paths = cmd.paths if cmd.paths else sorted(cmd.zettel_dir.rglob("*.zo"))
     file_to_hash: dict[str, str] = {}
     for path in paths:
-        file_to_hash[str(path).replace(f"{cmd.zettel_dir}/", "")] = _hash_file(
-            path
-        )
+        key = common.strip_zdir(cmd.zettel_dir, path)
+        file_to_hash[key] = _hash_file(path)
 
     zorg_data_dir = cmd.zettel_dir / f".{APP_NAME}"
     zorg_data_dir.mkdir(parents=True, exist_ok=True)
     file_hash_path = zorg_data_dir / "file_hash.json"
     old_file_to_hash: dict[str, str] = (
         json.loads(file_hash_path.read_bytes())
         if file_hash_path.exists()
@@ -242,18 +241,16 @@
         chunk_size: Size of chunks to read the file. Default is 8192 bytes.
 
     Returns:
         A SHA256 hash of the file's contents.
     """
     hasher = hashlib.sha256()  # Initialize the hasher
     with filepath.open("rb") as file:
-        chunk = file.read(chunk_size)
-        while chunk:
+        while chunk := file.read(chunk_size):
             hasher.update(chunk)
-            chunk = file.read(chunk_size)
     return hasher.hexdigest()
 
 
 def _process_vim_commands(
     zettel_dir: Path, vim_commands: Iterable[str]
 ) -> Iterator[str]:
     for vim_cmd in vim_commands:
```

### Comparing `zettel_org-0.6.3/src/zorg/service/messagebus.py` & `zettel_org-0.6.4/src/zorg/service/messagebus.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/service/templates.py` & `zettel_org-0.6.4/src/zorg/service/templates.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/service/zid_manager.py` & `zettel_org-0.6.4/src/zorg/service/zid_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 """Zorg ID generation and persistence logic lives here."""
 
 import datetime as dt
 import json
 from pathlib import Path
-from typing import Optional
+from typing import Final, Optional
 
 from .. import APP_NAME
 
 
+_UNSUPPORTED_ZID_CHARS: Final[tuple[str, ...]] = (
+    "I",
+    "O",
+    "Q",
+    "S",
+    "g",
+    "i",
+    "j",
+    "l",
+    "p",
+    "q",
+    "y",
+)
+
+
 class ZIDManager:
     """Responsible for knowing what the next zorg ID is based on the date."""
 
     _class_next_id_map: Optional[dict[str, str]] = None
 
     def __init__(self, zettel_dir: Path) -> None:
         zorg_data_dir = zettel_dir / f".{APP_NAME}"
@@ -49,29 +64,23 @@
 def _get_next_id(last_id: str) -> str:
     next_ch: Optional[str] = None
     idx = -1
     while next_ch is None and abs(idx) <= len(last_id):
         ch = last_id[idx]
         if ch == "9":
             next_ch = "A"
-        elif ch == "H":
-            next_ch = "J"
-        elif ch == "N":
-            next_ch = "P"
         elif ch == "Z":
             next_ch = "a"
-        elif ch == "i":
-            next_ch = "k"
-        elif ch == "k":
-            next_ch = "m"
         elif ch == "z":
             next_ch = None
             idx -= 1
         else:
             next_ch = chr(ord(ch) + 1)
+            while next_ch in _UNSUPPORTED_ZID_CHARS:
+                next_ch = chr(ord(next_ch) + 1)
 
     if next_ch is None and len(last_id) == 2:
         # Special case that allows for 3-digit ID part if necessary. This
         # allows for enough available IDs if you run 'db create' on a large
         # zettel org with a lot of notes that need ZIDs.
         return "000"
     elif next_ch is None:
```

### Comparing `zettel_org-0.6.3/src/zorg/storage/sql/converters.py` & `zettel_org-0.6.4/src/zorg/storage/sql/converters.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,40 +5,42 @@
 from typing import Any
 
 from sqlmodel import Session, select
 
 from . import models as sql
 from ...domain.models import ZorgFile, ZorgNote
 from ...domain.types import EntityConverter
+from ...service import common
 
 
 class ZorgFileConverter(EntityConverter[ZorgFile, sql.ZorgFile]):
     """Converts ZorgFile domain entities to/from ZorgFile sqlmodels."""
 
-    def __init__(self, session: Session) -> None:
+    def __init__(self, zdir: Path, session: Session) -> None:
+        self._zdir = zdir
         self._note_converter = ZorgNoteConverter(session)
         self._all_sql_notes: list[sql.ZorgNote] = []
 
     def from_entity(self, entity: ZorgFile) -> sql.ZorgFile:
         """Model-to-SQL-model converter for a ZorgFile."""
         sql_notes = []
         for note in entity.notes:
             sql_note = self._note_converter.from_entity(note)
             self._all_sql_notes.append(sql_note)
             sql_notes.append(sql_note)
         return sql.ZorgFile(
-            path=str(entity.path),
+            path=common.strip_zdir(self._zdir, entity.path),
             notes=sql_notes,
             has_errors=entity.has_errors,
         )
 
     def to_entity(self, sql_model: sql.ZorgFile) -> ZorgFile:
         """Model-to-SQL-model converter for a ZorgFile."""
         return ZorgFile(
-            Path(sql_model.path),
+            Path(common.strip_zdir(self._zdir, sql_model.path)),
             has_errors=sql_model.has_errors,
             notes=[
                 self._note_converter.to_entity(sql_note)
                 for sql_note in sql_model.notes
             ],
         )
```

### Comparing `zettel_org-0.6.3/src/zorg/storage/sql/engine.py` & `zettel_org-0.6.4/src/zorg/storage/sql/engine.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/storage/sql/models.py` & `zettel_org-0.6.4/src/zorg/storage/sql/models.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/src/zorg/storage/sql/repo.py` & `zettel_org-0.6.4/src/zorg/storage/sql/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,33 +8,33 @@
 from eris import ErisResult, Err, Ok
 from logrus import Logger
 from potoroo import QueryRepo
 from sqlmodel import Session, select
 
 from . import models as sql
 from ...domain.messages.events import NewZorgNotesEvent
-from ...domain.models import OrZorgQuery, ZorgFile
+from ...domain.models import ZorgFile, ZorgQuery
 from ...service.zid_manager import ZIDManager
 from .converters import ZorgFileConverter
 
 
 logger = Logger(__name__)
 
 
-class SQLRepo(QueryRepo[str, ZorgFile, OrZorgQuery]):
+class SQLRepo(QueryRepo[str, ZorgFile, ZorgQuery]):
     """Repo that stores zorg notes in sqlite database."""
 
     def __init__(
         self,
         zettel_dir: Path,
         session: Session,
     ) -> None:
         self._zettel_dir = zettel_dir
         self._session = session
-        self._converter = ZorgFileConverter(session)
+        self._converter = ZorgFileConverter(zettel_dir, session)
 
         self.seen: list[ZorgFile] = []
 
     def add(
         self, zorg_file: ZorgFile, /, *, key: str = None
     ) -> ErisResult[str]:
         """Adds a new file to the DB.
@@ -106,15 +106,15 @@
         if sql_zorg_file:
             zorg_file = self._converter.to_entity(sql_zorg_file)
             self._seen_zorg_file(zorg_file)
             return Ok(zorg_file)
         else:
             return Ok(None)
 
-    def get_by_query(self, query: OrZorgQuery) -> ErisResult[list[ZorgFile]]:
+    def get_by_query(self, query: ZorgQuery) -> ErisResult[list[ZorgFile]]:
         """Get file(s) from DB by using a query."""
         del query
         result: list[ZorgFile] = []
         for zorg_file in result:
             self._seen_zorg_file(zorg_file)
         return Ok(result)
```

### Comparing `zettel_org-0.6.3/src/zorg/storage/sql/session.py` & `zettel_org-0.6.4/src/zorg/storage/sql/session.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/targets.mk` & `zettel_org-0.6.4/targets.mk`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/__snapshots__/test_run_compile.ambr` & `zettel_org-0.6.4/tests/__snapshots__/test_run_compile.ambr`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/__snapshots__/test_run_db.ambr` & `zettel_org-0.6.4/tests/__snapshots__/test_run_db.ambr`

 * *Files 2% similar despite different names*

```diff
@@ -131,47 +131,40 @@
     '000103#0H',
     '000103#0J',
     '000103#0K',
     '000103#0L',
     '000103#0M',
     '000103#0N',
     '000103#0P',
-    '000103#0Q',
     '000103#0R',
-    '000103#0S',
     '000103#0T',
     '000103#0U',
     '000103#0V',
     '000103#0W',
     '000103#0X',
     '000103#0Y',
     '000103#0Z',
     '000103#0a',
     '000103#0b',
     '000103#0c',
     '000103#0d',
     '000103#0e',
     '000103#0f',
-    '000103#0g',
     '000103#0h',
-    '000103#0i',
     '000103#0k',
     '000103#0m',
     '000103#0n',
     '000103#0o',
-    '000103#0p',
-    '000103#0q',
     '000103#0r',
     '000103#0s',
     '000103#0t',
     '000103#0u',
     '000103#0v',
     '000103#0w',
     '000103#0x',
-    '000103#0y',
     '000103#0z',
     '000103#10',
     '000103#11',
     '000103#12',
     '000103#13',
     '000103#14',
     '000103#15',
@@ -189,41 +182,48 @@
     '000103#1H',
     '000103#1J',
     '000103#1K',
     '000103#1L',
     '000103#1M',
     '000103#1N',
     '000103#1P',
-    '000103#1Q',
     '000103#1R',
-    '000103#1S',
     '000103#1T',
     '000103#1U',
     '000103#1V',
     '000103#1W',
     '000103#1X',
     '000103#1Y',
     '000103#1Z',
     '000103#1a',
     '000103#1b',
     '000103#1c',
     '000103#1d',
     '000103#1e',
     '000103#1f',
-    '000103#1g',
     '000103#1h',
-    '000103#1i',
     '000103#1k',
     '000103#1m',
     '000103#1n',
     '000103#1o',
-    '000103#1p',
-    '000103#1q',
     '000103#1r',
     '000103#1s',
+    '000103#1t',
+    '000103#1u',
+    '000103#1v',
+    '000103#1w',
+    '000103#1x',
+    '000103#1z',
+    '000103#20',
+    '000103#21',
+    '000103#22',
+    '000103#23',
+    '000103#24',
+    '000103#25',
+    '000103#26',
     '240313#00',
     '240313#01',
     '240313#02',
     '240323#00',
     '240323#01',
     '240323#02',
     '240323#03',
```

### Comparing `zettel_org-0.6.3/tests/__snapshots__/test_run_edit.ambr` & `zettel_org-0.6.4/tests/__snapshots__/test_run_edit.ambr`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   # 2000-01-03.Mon
   #
   # ^ = [[2000/20000103]]
   # < = [[2000/20000102_day]]
   # > = [[2000/20000104_day]]
   # @ = [[day_log.zot]]
   
-  o 000103#1t #gtd pomodoro
+  o 000103#27 #gtd pomodoro
     * Google Calendar (bbugyi@google + bryanbugyi34@gmail)
     * Process yesterday's bujo log (e.g. close events, add missing pomodoros, rollover goals)
     * Copy any important gchat convos from yesterday into chat/*.txt
     * Check today's tickler file: [[tick_03]]
     * Fill out yesterday's habit tracker: [[2000/20000102_habit]]
     * go/g3co
     * Review Google Keep Inbox
```

### Comparing `zettel_org-0.6.3/tests/__snapshots__/test_run_template.ambr` & `zettel_org-0.6.4/tests/__snapshots__/test_run_template.ambr`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/common.py` & `zettel_org-0.6.4/tests/common.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/conftest.py` & `zettel_org-0.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/data/day_log.zot` & `zettel_org-0.6.4/tests/data/day_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/data/done_log.zot` & `zettel_org-0.6.4/tests/data/done_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/data/habit_log.zot` & `zettel_org-0.6.4/tests/data/habit_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/test_config.py` & `zettel_org-0.6.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/test_file_groups.py` & `zettel_org-0.6.4/tests/test_file_groups.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/test_run_action_open.py` & `zettel_org-0.6.4/tests/test_run_action_open.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/test_run_compile.py` & `zettel_org-0.6.4/tests/test_run_compile.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/test_run_db.py` & `zettel_org-0.6.4/tests/test_run_db.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/test_run_edit.py` & `zettel_org-0.6.4/tests/test_run_edit.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.3/tests/test_run_template.py` & `zettel_org-0.6.4/tests/test_run_template.py`

 * *Files identical despite different names*

