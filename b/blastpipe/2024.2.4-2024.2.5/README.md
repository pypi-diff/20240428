# Comparing `tmp/blastpipe-2024.2.4.tar.gz` & `tmp/blastpipe-2024.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2024.2.4.tar", last modified: Sun Apr 28 01:48:17 2024, max compression
+gzip compressed data, was "blastpipe-2024.2.5.tar", last modified: Sun Apr 28 02:15:32 2024, max compression
```

## Comparing `blastpipe-2024.2.4.tar` & `blastpipe-2024.2.5.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:48:17.302104 blastpipe-2024.2.4/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5868 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/.github/workflows/scorecards.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/.pre-commit-config.yaml
--rw-rw-r--   0 runner    (1001) docker     (127)    85133 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-28 01:48:17.302104 blastpipe-2024.2.4/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/mixin.pyi
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/.gitignore.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/CHANGELOG.md.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      342 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/LICENSE.txt.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      112 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/PKG-INFO.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      618 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/README.rst.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1867 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/bandit.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/bandit.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/black.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      228 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/black.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      627 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/coverage.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      220 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/doc8.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      124 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/doc8.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     2798 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/filter.py
--rw-rw-r--   0 runner    (1001) docker     (127)      385 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/flake8.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      432 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/flake8.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     1648 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/ozi.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      757 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/publish.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1375 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/release.yml.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/gitlab_workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)      335 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/gitlab_workflows/ozi.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/isort.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/isort.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      355 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    20141 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      847 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/mit.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/wtfpl.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/zlib.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/
--rw-rw-r--   0 runner    (1001) docker     (127)    11067 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/
--rw-rw-r--   0 runner    (1001) docker     (127)    10315 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/
--rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/
--rw-rw-r--   0 runner    (1001) docker     (127)    19765 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    20209 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    19902 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    21198 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      431 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      469 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)    22960 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)    14199 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)    13154 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      370 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/
--rw-rw-r--   0 runner    (1001) docker     (127)    13831 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      370 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      379 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      403 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      378 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      403 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      378 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      409 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      379 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/mit.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      367 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       88 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/mpl-2.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      475 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     9269 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10302 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1639 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      435 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/zlib.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/Public_Domain/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/Public_Domain/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/Public_Domain/licenseref-public-domain.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/Public_Domain/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1213 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)    34525 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/agpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11359 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     8896 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1544 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11587 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    22965 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/gfdl-1.3.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    18094 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/gpl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    35151 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/gpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      788 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    25381 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/lgpl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    26528 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/lgpl-2.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7654 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/lgpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1204 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1114 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/mit.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/license/zlib.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1856 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      418 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      883 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/meson.options.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      168 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/mypy.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/mypy.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1151 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/new_child.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      353 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/ozi.wrap.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     2503 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     1138 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.array.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.feature.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      544 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.integer.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     3602 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.name/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.name/__init__.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      289 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.name/__init__.pyi.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      452 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.name/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      755 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.name/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.name/new_module.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      129 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.name/py.typed.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      129 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/project.ozi.wrap.j2
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/pydocstyle.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/pylint.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      600 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/pyproject.toml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      231 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/pyright.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      245 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/pyright.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/pytest.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      422 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/pytest.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      150 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/requirements.in.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      229 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/restructuredtext-lint.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/root.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1126 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/ruff.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1124 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/semantic_release.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      341 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/setuptools_scm.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/tests/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/tests/new_test.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1427 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/ozi_templates/tox.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     8358 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)       33 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      121 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/tests/test_filter.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-28 01:42:24.000000 blastpipe-2024.2.4/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:15:32.603424 blastpipe-2024.2.5/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5868 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)    85363 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-28 02:15:32.603424 blastpipe-2024.2.5/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/mixin.pyi
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/.gitignore.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/CHANGELOG.md.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      342 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/LICENSE.txt.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      112 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/PKG-INFO.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      618 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/README.rst.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1867 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/bandit.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/bandit.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/black.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      228 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/black.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      627 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/coverage.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      220 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/doc8.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      124 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/doc8.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2799 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/filter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      385 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/flake8.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      432 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/flake8.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1648 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/ozi.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      757 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/publish.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1375 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/release.yml.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/gitlab_workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)      335 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/gitlab_workflows/ozi.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/isort.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/isort.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      355 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20141 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      847 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/mit.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/wtfpl.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/zlib.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11067 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10315 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)    19765 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20209 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    19902 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    21198 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      431 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      469 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    22960 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    14199 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13154 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      370 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13831 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      370 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      379 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      403 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      378 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      403 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      378 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      409 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      379 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/mit.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      367 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       88 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/mpl-2.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      475 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     9269 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10302 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1639 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      435 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/zlib.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/Public_Domain/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/Public_Domain/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/Public_Domain/licenseref-public-domain.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/Public_Domain/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1213 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    34525 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/agpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11359 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     8896 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1544 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11587 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    22965 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/gfdl-1.3.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    18094 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/gpl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    35151 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/gpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      788 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    25381 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/lgpl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    26528 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/lgpl-2.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7654 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/lgpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1204 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1114 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/mit.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/license/zlib.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1856 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      418 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      883 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/meson.options.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      168 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/mypy.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/mypy.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1151 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/new_child.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      353 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/ozi.wrap.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     2503 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     1138 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.array.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.feature.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      544 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.integer.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     3602 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.name/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.name/__init__.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      289 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.name/__init__.pyi.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      452 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.name/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      755 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.name/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.name/new_module.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      129 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.name/py.typed.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      129 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/project.ozi.wrap.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/pydocstyle.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/pylint.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      600 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/pyproject.toml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      231 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/pyright.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      245 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/pyright.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/pytest.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      422 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/pytest.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      150 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/requirements.in.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      229 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/restructuredtext-lint.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/root.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1126 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/ruff.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1124 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/semantic_release.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      341 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/setuptools_scm.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/tests/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/tests/new_test.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1427 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/ozi_templates/tox.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8358 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)       33 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      121 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/tests/test_filter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-28 02:09:19.000000 blastpipe-2024.2.5/tests/test_tailcall.py
```

### Comparing `blastpipe-2024.2.4/.github/workflows/codeql.yml` & `blastpipe-2024.2.5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/.github/workflows/dependency-review.yml` & `blastpipe-2024.2.5/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/.github/workflows/ozi.yml` & `blastpipe-2024.2.5/.github/workflows/ozi.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/.github/workflows/scorecards.yml` & `blastpipe-2024.2.5/.github/workflows/scorecards.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/.gitignore` & `blastpipe-2024.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/CHANGELOG.md` & `blastpipe-2024.2.5/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # CHANGELOG
 
 
 
+## v2024.2.5 (2024-04-28)
+
+### :bug:
+
+* :bug: fix next_minor filter typo.
+
+Signed-off-by: rjdbcm &lt;rjdbcm@outlook.com&gt; ([`404c645`](https://github.com/OZI-Project/blastpipe/commit/404c6454186915e20b2a2e4b4756f09e507cf30b))
+
+
 ## v2024.2.4 (2024-04-28)
 
 ### :bug:
 
 * :bug: Load jinja2 env from blastpipe package.
 
 Signed-off-by: rjdbcm &lt;rjdbcm@outlook.com&gt; ([`9e34d11`](https://github.com/OZI-Project/blastpipe/commit/9e34d11ab58b2509a8cc9fdf80bc746c62bc8cd1))
```

### Comparing `blastpipe-2024.2.4/LICENSE.txt` & `blastpipe-2024.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/NOTICE.md` & `blastpipe-2024.2.5/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/PKG-INFO` & `blastpipe-2024.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2024.2.4
+Version: 2024.2.5
 Summary: OZI integrated test library.
 Home-page: https://oziproject.dev
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
-Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.2.4.tar.gz
+Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.2.5.tar.gz
 Requires-Python: >=3.10, <3.13
 Keywords: ozi,meson
 Provides-Dist: ozi-templates
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `blastpipe-2024.2.4/README.rst` & `blastpipe-2024.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/__init__.py` & `blastpipe-2024.2.5/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/backports.py` & `blastpipe-2024.2.5/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/backports.pyi` & `blastpipe-2024.2.5/blastpipe/backports.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/buffer.py` & `blastpipe-2024.2.5/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/loop.py` & `blastpipe-2024.2.5/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/malloc.py` & `blastpipe-2024.2.5/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/meson.build` & `blastpipe-2024.2.5/blastpipe/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/mixin.py` & `blastpipe-2024.2.5/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/README.rst.j2` & `blastpipe-2024.2.5/blastpipe/ozi_templates/README.rst.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/__init__.py` & `blastpipe-2024.2.5/blastpipe/ozi_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/coverage.pyproject.toml` & `blastpipe-2024.2.5/blastpipe/ozi_templates/coverage.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/filter.py` & `blastpipe-2024.2.5/blastpipe/ozi_templates/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,9 +88,9 @@
     """Given a Python version, determine the next minor version.
 
     :param version: Python version string
     :type version: str
     :return: The next minor version
     :rtype: str
     """
-    major, _, minor = map(int, version.split('.'))
+    major, minor, *_ = map(int, version.split('.'))
     return f'{major}.{minor + 1}'
```

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2` & `blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2` & `blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/meson.build` & `blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/ozi.yml.j2` & `blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/ozi.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/publish.yml.j2` & `blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/publish.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/github_workflows/release.yml.j2` & `blastpipe-2024.2.5/blastpipe/ozi_templates/github_workflows/release.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/DFSG_approved/meson.build` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/DFSG_approved/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/OSI_Approved/meson.build` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/OSI_Approved/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/agpl-3.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/apache-2.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/artistic-2.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/bsd-3-clause.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/bsd-3-clause.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/cc0-1.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/cc0-1.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/epl-1.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/epl-1.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/gfdl-1.3.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/gfdl-1.3.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/gpl-2.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/gpl-3.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/isc.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/isc.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/lgpl-2.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/lgpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/lgpl-2.1.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/lgpl-2.1.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/lgpl-3.0.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/meson.build` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/mit.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/mit.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/license/zlib.txt` & `blastpipe-2024.2.5/blastpipe/ozi_templates/license/zlib.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/meson.build` & `blastpipe-2024.2.5/blastpipe/ozi_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/meson.options.j2` & `blastpipe-2024.2.5/blastpipe/ozi_templates/meson.options.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/new_child.j2` & `blastpipe-2024.2.5/blastpipe/ozi_templates/new_child.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/project.PKG-INFO` & `blastpipe-2024.2.5/blastpipe/ozi_templates/project.PKG-INFO`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/project.array.meson.options` & `blastpipe-2024.2.5/blastpipe/ozi_templates/project.array.meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/project.feature.meson.options` & `blastpipe-2024.2.5/blastpipe/ozi_templates/project.feature.meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/project.integer.meson.options` & `blastpipe-2024.2.5/blastpipe/ozi_templates/project.integer.meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/project.meson.build` & `blastpipe-2024.2.5/blastpipe/ozi_templates/project.meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/project.name/meson.build.j2` & `blastpipe-2024.2.5/blastpipe/ozi_templates/project.name/meson.build.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/pyproject.toml.j2` & `blastpipe-2024.2.5/blastpipe/ozi_templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/root.pyproject.toml` & `blastpipe-2024.2.5/blastpipe/ozi_templates/root.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/ruff.pyproject.toml` & `blastpipe-2024.2.5/blastpipe/ozi_templates/ruff.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/semantic_release.pyproject.toml` & `blastpipe-2024.2.5/blastpipe/ozi_templates/semantic_release.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/tests/meson.build.j2` & `blastpipe-2024.2.5/blastpipe/ozi_templates/tests/meson.build.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/ozi_templates/tox.pyproject.toml` & `blastpipe-2024.2.5/blastpipe/ozi_templates/tox.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/sequence.py` & `blastpipe-2024.2.5/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/blastpipe/tailcall.py` & `blastpipe-2024.2.5/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/meson.build` & `blastpipe-2024.2.5/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/meson.options` & `blastpipe-2024.2.5/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/pyproject.toml` & `blastpipe-2024.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/subprojects/docs/LICENSE.txt` & `blastpipe-2024.2.5/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.2.5/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.2.5/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/subprojects/docs/_static/meson.build` & `blastpipe-2024.2.5/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/subprojects/docs/_templates/layout.html` & `blastpipe-2024.2.5/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/subprojects/docs/_templates/meson.build` & `blastpipe-2024.2.5/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/subprojects/docs/conf.cfg` & `blastpipe-2024.2.5/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/subprojects/docs/index.rst` & `blastpipe-2024.2.5/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/subprojects/docs/meson.build` & `blastpipe-2024.2.5/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/subprojects/docs/meson.options` & `blastpipe-2024.2.5/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/tests/meson.build` & `blastpipe-2024.2.5/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/tests/test_backports.py` & `blastpipe-2024.2.5/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/tests/test_filter.py` & `blastpipe-2024.2.5/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/tests/test_fuzz.py` & `blastpipe-2024.2.5/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.2.4/tests/test_tailcall.py` & `blastpipe-2024.2.5/tests/test_tailcall.py`

 * *Files identical despite different names*

