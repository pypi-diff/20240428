# Comparing `tmp/fractal_repositories-0.0.8.tar.gz` & `tmp/fractal_repositories-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_repositories-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fractal_repositories-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fractal_repositories-0.0.8.tar` & `fractal_repositories-0.0.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      187 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/.coveragerc
--rw-r--r--   0        0        0      100 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/.flake8
--rw-r--r--   0        0        0      945 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/.gitignore
--rw-r--r--   0        0        0      161 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/.isort.cfg
--rw-r--r--   0        0        0       43 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/.mypy.ini
--rw-r--r--   0        0        0     1691 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/LICENSE
--rw-r--r--   0        0        0     1557 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/Makefile
--rw-r--r--   0        0        0     2276 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/README.md
--rw-r--r--   0        0        0      780 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/align_version.py
--rw-r--r--   0        0        0      182 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/contrib/django/__init__.py
--rw-r--r--   0        0        0     3291 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/contrib/django/mixins.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/contrib/elastic/__init__.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0     5338 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/contrib/gcp/firestore/mixins.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     3273 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/contrib/mongo/mixins.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    11960 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/contrib/sqlalchemy/mixins.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/core/__init__.py
--rw-r--r--   0        0        0     1681 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/core/entity.py
--rw-r--r--   0        0        0     2434 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/core/repositories.py
--rw-r--r--   0        0        0      343 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/exceptions.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/mixins/__init__.py
--rw-r--r--   0        0        0     1219 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0     2909 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/mixins/file_repository_mixin.py
--rw-r--r--   0        0        0      967 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/mixins/filter_repository_mixin.py
--rw-r--r--   0        0        0     3088 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/mixins/inmemory_repository_mixin.py
--rw-r--r--   0        0        0       77 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/py.typed
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.349300 fractal_repositories-0.0.8/fractal_repositories/utils/__init__.py
--rw-r--r--   0        0        0     2299 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/fractal_repositories/utils/cached_repository.py
--rw-r--r--   0        0        0     2381 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/fractal_repositories/utils/distributed_read_repository.py
--rw-r--r--   0        0        0      636 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/fractal_repositories/utils/json_encoder.py
--rw-r--r--   0        0        0      235 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/poetry.lock
--rw-r--r--   0        0        0     1667 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       69 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/setup.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/contrib/__init__.py
--rw-r--r--   0        0        0     4177 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/contrib/test_django.py
--rw-r--r--   0        0        0     4438 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/contrib/test_firestore.py
--rw-r--r--   0        0        0     4100 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/contrib/test_mongo.py
--rw-r--r--   0        0        0    12220 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/contrib/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/core/__init__.py
--rw-r--r--   0        0        0     3208 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/core/test_models.py
--rw-r--r--   0        0        0     1046 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/core/test_repositories.py
--rw-r--r--   0        0        0      232 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2164 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/fixtures/django/__init__.py
--rw-r--r--   0        0        0      643 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/fixtures/django/models.py
--rw-r--r--   0        0        0     1144 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/fixtures/firestore.py
--rw-r--r--   0        0        0      898 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/fixtures/mongo.py
--rw-r--r--   0        0        0     6786 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/fixtures/repositories.py
--rw-r--r--   0        0        0     7674 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/fixtures/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/mixins/__init__.py
--rw-r--r--   0        0        0     1154 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/mixins/test_external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0      601 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/mixins/test_file_file_repository_mixin.py
--rw-r--r--   0        0        0     3745 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/mixins/test_file_repository_mixin.py
--rw-r--r--   0        0        0     3542 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/mixins/test_filter_repository_mixin.py
--rw-r--r--   0        0        0      827 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/mixins/test_inmemory_file_repository_mixin.py
--rw-r--r--   0        0        0     3478 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/mixins/test_inmemory_repository_mixin.py
--rw-r--r--   0        0        0        0 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/utils/__init__.py
--rw-r--r--   0        0        0     4025 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/utils/test_cached_repository.py
--rw-r--r--   0        0        0     2381 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/utils/test_distributed_read_repository.py
--rw-r--r--   0        0        0      996 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tests/utils/test_json_encoder.py
--rw-r--r--   0        0        0      826 2023-10-18 08:32:56.353299 fractal_repositories-0.0.8/tox.ini
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 fractal_repositories-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/.coveragerc
+-rw-r--r--   0        0        0      100 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/.flake8
+-rw-r--r--   0        0        0      945 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/.gitignore
+-rw-r--r--   0        0        0      161 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/.isort.cfg
+-rw-r--r--   0        0        0       43 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/.mypy.ini
+-rw-r--r--   0        0        0     1691 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1560 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/Makefile
+-rw-r--r--   0        0        0     2276 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/README.md
+-rw-r--r--   0        0        0      780 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/align_version.py
+-rw-r--r--   0        0        0      182 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/fractal_repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/fractal_repositories/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.454481 fractal_repositories-0.0.9/fractal_repositories/contrib/django/__init__.py
+-rw-r--r--   0        0        0     3291 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/contrib/django/mixins.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/contrib/elastic/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0     5338 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/contrib/gcp/firestore/mixins.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     3273 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/contrib/mongo/mixins.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11960 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/contrib/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/core/__init__.py
+-rw-r--r--   0        0        0     1681 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/core/entity.py
+-rw-r--r--   0        0        0     2434 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/core/repositories.py
+-rw-r--r--   0        0        0      343 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/exceptions.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/mixins/__init__.py
+-rw-r--r--   0        0        0     1219 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0     2909 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/mixins/file_repository_mixin.py
+-rw-r--r--   0        0        0      967 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/mixins/filter_repository_mixin.py
+-rw-r--r--   0        0        0     3088 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/mixins/inmemory_repository_mixin.py
+-rw-r--r--   0        0        0       77 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/py.typed
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/utils/__init__.py
+-rw-r--r--   0        0        0     2299 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/utils/cached_repository.py
+-rw-r--r--   0        0        0     2381 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/utils/distributed_read_repository.py
+-rw-r--r--   0        0        0      636 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/fractal_repositories/utils/json_encoder.py
+-rw-r--r--   0        0        0      235 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/poetry.lock
+-rw-r--r--   0        0        0     1667 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/setup.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/tests/contrib/__init__.py
+-rw-r--r--   0        0        0     4177 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/tests/contrib/test_django.py
+-rw-r--r--   0        0        0     4438 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/tests/contrib/test_firestore.py
+-rw-r--r--   0        0        0     4100 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/tests/contrib/test_mongo.py
+-rw-r--r--   0        0        0    12220 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/tests/contrib/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/tests/core/__init__.py
+-rw-r--r--   0        0        0     3376 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/tests/core/test_models.py
+-rw-r--r--   0        0        0     1046 2023-10-18 08:53:20.458481 fractal_repositories-0.0.9/tests/core/test_repositories.py
+-rw-r--r--   0        0        0      232 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2164 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/fixtures/django/__init__.py
+-rw-r--r--   0        0        0      643 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/fixtures/django/models.py
+-rw-r--r--   0        0        0     1144 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/fixtures/firestore.py
+-rw-r--r--   0        0        0      898 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/fixtures/mongo.py
+-rw-r--r--   0        0        0     6786 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/fixtures/repositories.py
+-rw-r--r--   0        0        0     7674 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/fixtures/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/mixins/__init__.py
+-rw-r--r--   0        0        0     1154 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/mixins/test_external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0      601 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/mixins/test_file_file_repository_mixin.py
+-rw-r--r--   0        0        0     3745 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/mixins/test_file_repository_mixin.py
+-rw-r--r--   0        0        0     3542 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/mixins/test_filter_repository_mixin.py
+-rw-r--r--   0        0        0      827 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/mixins/test_inmemory_file_repository_mixin.py
+-rw-r--r--   0        0        0     3478 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/mixins/test_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0        0 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/utils/__init__.py
+-rw-r--r--   0        0        0     4025 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/utils/test_cached_repository.py
+-rw-r--r--   0        0        0     2381 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/utils/test_distributed_read_repository.py
+-rw-r--r--   0        0        0      996 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tests/utils/test_json_encoder.py
+-rw-r--r--   0        0        0      826 2023-10-18 08:53:20.462481 fractal_repositories-0.0.9/tox.ini
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 fractal_repositories-0.0.9/PKG-INFO
```

### Comparing `fractal_repositories-0.0.8/.github/workflows/build.yml` & `fractal_repositories-0.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/.github/workflows/publish.yml` & `fractal_repositories-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/.gitignore` & `fractal_repositories-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/.pre-commit-config.yaml` & `fractal_repositories-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/LICENSE` & `fractal_repositories-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/Makefile` & `fractal_repositories-0.0.9/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 coverage:  ## Run tests with coverage
 	rm .coverage ||:
 	rm coverage.xml ||:
 	pytest --cov fractal_repositories --cov-report=xml
 
 deps:  ## Install dependencies
 	python -m pip install --upgrade pip
-	python -m pip install black coverage django firebase-admin flake8 flit fractal-specifications google-cloud-firestore isort mccabe mock-firestore mongomock mypy pylint pymongo pytest pytest-cov pytest-asyncio pytest-lazy-fixture pytest-mock 'sqlalchemy<2.0' tox tox-gh-actions pre-commit autoflake
+	python -m pip install -U black coverage django firebase-admin flake8 flit fractal-specifications google-cloud-firestore isort mccabe mock-firestore mongomock mypy pylint pymongo pytest pytest-cov pytest-asyncio pytest-lazy-fixture pytest-mock 'sqlalchemy<2.0' tox tox-gh-actions pre-commit autoflake
 	pre-commit install
 
 lint:  ## Lint and static-check
 	pre-commit run --all-files
 
 publish:  ## Publish to PyPi
 	python -m flit publish
```

### Comparing `fractal_repositories-0.0.8/README.md` & `fractal_repositories-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/align_version.py` & `fractal_repositories-0.0.9/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/fractal_repositories/contrib/django/mixins.py` & `fractal_repositories-0.0.9/fractal_repositories/contrib/django/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/fractal_repositories/contrib/gcp/firestore/mixins.py` & `fractal_repositories-0.0.9/fractal_repositories/contrib/gcp/firestore/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import date
-from typing import Iterable, Iterator, Union, Optional
+from typing import Iterable, Iterator, Optional, Union
 
 from fractal_specifications.contrib.google_firestore.specifications import (
     FirestoreSpecificationBuilder,
 )
 from fractal_specifications.generic.specification import Specification
 from google.cloud.firestore_v1 import Client, DocumentSnapshot, Query
 from google.cloud.firestore_v1.base_collection import BaseCollectionReference
@@ -114,26 +114,26 @@
         *,
         offset: int = 0,
         limit: int = 0,
         order_by: str = "",
     ) -> Iterator[EntityType]:
         _filter = FirestoreSpecificationBuilder.build(specification)
         direction = Query.ASCENDING
+        order_by = order_by or self.order_by
         if order_by.startswith("-"):
             order_by = order_by[1:]
             direction = Query.DESCENDING
         collection: Union[BaseCollectionReference, BaseQuery] = self.collection
         if _filter:
             if isinstance(_filter, list):
                 for f in _filter:
                     collection = collection.where(*f)
             else:
                 collection = collection.where(*_filter)
 
-        order_by = order_by or self.order_by
         if order_by:
             collection = collection.order_by(order_by, direction=direction)
 
         if limit:
             if offset and (last := list(collection.limit(offset).stream())[-1]):
                 collection = collection.start_after(
                     {order_by: (last.to_dict() or {}).get(order_by)}
```

### Comparing `fractal_repositories-0.0.8/fractal_repositories/contrib/mongo/mixins.py` & `fractal_repositories-0.0.9/fractal_repositories/contrib/mongo/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Iterator, Tuple, Optional
+from typing import Dict, Iterator, Optional, Tuple
 
 from fractal_specifications.contrib.mongo.specifications import (
     MongoSpecificationBuilder,
 )
 from fractal_specifications.generic.specification import Specification
 from pymongo import MongoClient
 from pymongo.database import Database
@@ -70,24 +70,24 @@
         self,
         specification: Optional[Specification] = None,
         *,
         offset: int = 0,
         limit: int = 0,
         order_by: str = "",
     ) -> Iterator[EntityType]:
+        order_by = order_by or self.order_by
         direction = 1
         if order_by.startswith("-"):
             order_by = order_by[1:]
             direction = -1
 
         collection = self.collection.find(
             MongoSpecificationBuilder.build(specification)
         )
 
-        order_by = order_by or self.order_by
         if order_by:
             collection = collection.sort({order_by: direction})
 
         if limit:
             collection = collection.skip(offset).limit(limit)
 
         for obj in collection.sort(order_by, direction):
```

### Comparing `fractal_repositories-0.0.8/fractal_repositories/contrib/sqlalchemy/mixins.py` & `fractal_repositories-0.0.9/fractal_repositories/contrib/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/fractal_repositories/core/entity.py` & `fractal_repositories-0.0.9/fractal_repositories/core/entity.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/fractal_repositories/core/repositories.py` & `fractal_repositories-0.0.9/fractal_repositories/core/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py` & `fractal_repositories-0.0.9/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/fractal_repositories/mixins/file_repository_mixin.py` & `fractal_repositories-0.0.9/fractal_repositories/mixins/file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/fractal_repositories/mixins/filter_repository_mixin.py` & `fractal_repositories-0.0.9/fractal_repositories/mixins/filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/fractal_repositories/mixins/inmemory_repository_mixin.py` & `fractal_repositories-0.0.9/fractal_repositories/mixins/inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/fractal_repositories/utils/cached_repository.py` & `fractal_repositories-0.0.9/fractal_repositories/utils/cached_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/fractal_repositories/utils/distributed_read_repository.py` & `fractal_repositories-0.0.9/fractal_repositories/utils/distributed_read_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/fractal_repositories/utils/json_encoder.py` & `fractal_repositories-0.0.9/fractal_repositories/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/pyproject.toml` & `fractal_repositories-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-repositories"
-version = "0.0.8"
+version = "0.0.9"
 description = "Fractal Repositories is an implementation of the repository pattern for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `fractal_repositories-0.0.8/tests/contrib/test_django.py` & `fractal_repositories-0.0.9/tests/contrib/test_django.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/contrib/test_firestore.py` & `fractal_repositories-0.0.9/tests/contrib/test_firestore.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/contrib/test_mongo.py` & `fractal_repositories-0.0.9/tests/contrib/test_mongo.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/contrib/test_sqlalchemy.py` & `fractal_repositories-0.0.9/tests/contrib/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/core/test_models.py` & `fractal_repositories-0.0.9/tests/core/test_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -74,15 +74,21 @@
         **some_new_values,
         "now": now.isoformat(),
         "decimal_number": f"{decimal:.2f}",
     }
 
 
 def test_model_skip_types(model_instance, now, decimal):
-    assert model_instance.asdict(skip_types=(list, date, Decimal,)) == {
+    assert model_instance.asdict(
+        skip_types=(
+            list,
+            date,
+            Decimal,
+        )
+    ) == {
         "id": "1",
         "string": "name",
         "number": 1,
         "string_list": ["a", "b"],
         "now": now,
         "decimal_number": decimal,
     }
@@ -101,23 +107,34 @@
                 "decimal_number": f"{decimal:.2f}",
             }
         ],
     }
 
 
 def test_model_nested_skip_types(nested_model_instance, model_instance, now, decimal):
-    m = nested_model_instance.asdict(skip_types=(list, date, Decimal,))[
+    m = nested_model_instance.asdict(
+        skip_types=(
+            list,
+            date,
+            Decimal,
+        )
+    )[
         "nested_list"
     ][0]
     assert type(m) == type(model_instance)
     assert m.now == now
 
 
 def test_model_nested_skip_types_no_list(nested_model_instance, now, decimal):
-    assert nested_model_instance.asdict(skip_types=(date, Decimal,)) == {
+    assert nested_model_instance.asdict(
+        skip_types=(
+            date,
+            Decimal,
+        )
+    ) == {
         "id": "1",
         "nested_list": [
             {
                 "id": "1",
                 "string": "name",
                 "number": 1,
                 "string_list": ["a", "b"],
```

### Comparing `fractal_repositories-0.0.8/tests/core/test_repositories.py` & `fractal_repositories-0.0.9/tests/core/test_repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/fixtures/django/__init__.py` & `fractal_repositories-0.0.9/tests/fixtures/django/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/fixtures/django/models.py` & `fractal_repositories-0.0.9/tests/fixtures/django/models.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/fixtures/firestore.py` & `fractal_repositories-0.0.9/tests/fixtures/firestore.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/fixtures/mongo.py` & `fractal_repositories-0.0.9/tests/fixtures/mongo.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/fixtures/repositories.py` & `fractal_repositories-0.0.9/tests/fixtures/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/fixtures/sqlalchemy.py` & `fractal_repositories-0.0.9/tests/fixtures/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/mixins/test_external_data_inmemory_repository_mixin.py` & `fractal_repositories-0.0.9/tests/mixins/test_external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/mixins/test_file_file_repository_mixin.py` & `fractal_repositories-0.0.9/tests/mixins/test_file_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/mixins/test_file_repository_mixin.py` & `fractal_repositories-0.0.9/tests/mixins/test_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/mixins/test_filter_repository_mixin.py` & `fractal_repositories-0.0.9/tests/mixins/test_filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/mixins/test_inmemory_file_repository_mixin.py` & `fractal_repositories-0.0.9/tests/mixins/test_inmemory_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/mixins/test_inmemory_repository_mixin.py` & `fractal_repositories-0.0.9/tests/mixins/test_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/utils/test_cached_repository.py` & `fractal_repositories-0.0.9/tests/utils/test_cached_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/utils/test_distributed_read_repository.py` & `fractal_repositories-0.0.9/tests/utils/test_distributed_read_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tests/utils/test_json_encoder.py` & `fractal_repositories-0.0.9/tests/utils/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/tox.ini` & `fractal_repositories-0.0.9/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.8/PKG-INFO` & `fractal_repositories-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-repositories
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fractal Repositories is an implementation of the repository pattern of Domain Driven Design (DDD) for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-repositories
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

