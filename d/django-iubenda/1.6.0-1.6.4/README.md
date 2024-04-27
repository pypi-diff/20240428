# Comparing `tmp/django_iubenda-1.6.0.tar.gz` & `tmp/django_iubenda-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_iubenda-1.6.0.tar", last modified: Sun Apr 14 16:39:54 2024, max compression
+gzip compressed data, was "django_iubenda-1.6.4.tar", last modified: Sat Apr 27 22:31:52 2024, max compression
```

## Comparing `django_iubenda-1.6.0.tar` & `django_iubenda-1.6.4.tar`

### file list

```diff
@@ -1,85 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.875819 django_iubenda-1.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)    33664 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py310-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py311-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py38-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py39-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/runtests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.867819 django_iubenda-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/src/django_iubenda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-14 16:39:54.000000 django_iubenda-1.6.0/src/django_iubenda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-14 16:39:54.000000 django_iubenda-1.6.0/src/django_iubenda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:39:54.000000 django_iubenda-1.6.0/src/django_iubenda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:39:54.000000 django_iubenda-1.6.0/src/django_iubenda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 16:39:54.000000 django_iubenda-1.6.0/src/django_iubenda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 16:39:54.000000 django_iubenda-1.6.0/src/django_iubenda.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.879819 django_iubenda-1.6.0/src/iubenda/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.879819 django_iubenda-1.6.0/src/iubenda/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/fixtures/data.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.867819 django_iubenda-1.6.0/src/iubenda/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.867819 django_iubenda-1.6.0/src/iubenda/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.879819 django_iubenda-1.6.0/src/iubenda/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.879819 django_iubenda-1.6.0/src/iubenda/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/sitemaps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.867819 django_iubenda-1.6.0/src/iubenda/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.871819 django_iubenda-1.6.0/src/iubenda/static/iubenda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.879819 django_iubenda-1.6.0/src/iubenda/static/iubenda/css/
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/static/iubenda/css/iubenda_badge.css
--rw-r--r--   0 runner    (1001) docker     (127)    42615 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/static/iubenda/css/iubenda_policy.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.871819 django_iubenda-1.6.0/src/iubenda/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.879819 django_iubenda-1.6.0/src/iubenda/templates/iubenda/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/templates/iubenda/cookie-compress.html
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/templates/iubenda/cookie.html
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/templates/iubenda/include-content.html
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/templates/iubenda/privacy-compress.html
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/templates/iubenda/privacy.html
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/translation.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/fixtures/data.json
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/test_iubenda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/test_iubenda_custom_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/test_iubenda_default_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/test_iubenda_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/test_iubenda_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/test_iubenda_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.331055 django_iubenda-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-27 22:31:52.331055 django_iubenda-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.323055 django_iubenda-1.6.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-27 22:31:52.331055 django_iubenda-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.319055 django_iubenda-1.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.331055 django_iubenda-1.6.4/src/django_iubenda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-27 22:31:52.000000 django_iubenda-1.6.4/src/django_iubenda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-27 22:31:52.000000 django_iubenda-1.6.4/src/django_iubenda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:31:52.000000 django_iubenda-1.6.4/src/django_iubenda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-27 22:31:52.000000 django_iubenda-1.6.4/src/django_iubenda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 22:31:52.000000 django_iubenda-1.6.4/src/django_iubenda.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.327055 django_iubenda-1.6.4/src/iubenda/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.327055 django_iubenda-1.6.4/src/iubenda/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/fixtures/data.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.319055 django_iubenda-1.6.4/src/iubenda/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.319055 django_iubenda-1.6.4/src/iubenda/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.327055 django_iubenda-1.6.4/src/iubenda/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.327055 django_iubenda-1.6.4/src/iubenda/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/sitemaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.319055 django_iubenda-1.6.4/src/iubenda/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.319055 django_iubenda-1.6.4/src/iubenda/static/iubenda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.327055 django_iubenda-1.6.4/src/iubenda/static/iubenda/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/static/iubenda/css/iubenda_badge.css
+-rw-r--r--   0 runner    (1001) docker     (127)    42615 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/static/iubenda/css/iubenda_policy.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.319055 django_iubenda-1.6.4/src/iubenda/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.327055 django_iubenda-1.6.4/src/iubenda/templates/iubenda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/templates/iubenda/cookie-compress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/templates/iubenda/cookie.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/templates/iubenda/include-content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/templates/iubenda/privacy-compress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/templates/iubenda/privacy.html
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/src/iubenda/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.331055 django_iubenda-1.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.331055 django_iubenda-1.6.4/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tests/fixtures/data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:31:52.331055 django_iubenda-1.6.4/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tests/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tests/test_iubenda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tests/test_iubenda_custom_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tests/test_iubenda_default_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tests/test_iubenda_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tests/test_iubenda_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tests/test_iubenda_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-27 22:31:43.000000 django_iubenda-1.6.4/tox.ini
```

### Comparing `django_iubenda-1.6.0/.pre-commit-config.yaml` & `django_iubenda-1.6.4/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   - id: trailing-whitespace
 - repo: https://github.com/asottile/pyupgrade
   rev: v3.15.2
   hooks:
   - id: pyupgrade
     args: [--py36-plus]
 - repo: https://github.com/psf/black
-  rev: 24.3.0
+  rev: 24.4.0
   hooks:
   - id: black
 - repo: https://github.com/asottile/blacken-docs
   rev: 1.16.0
   hooks:
   - id: blacken-docs
     additional_dependencies:
```

### Comparing `django_iubenda-1.6.0/LICENSE` & `django_iubenda-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/PKG-INFO` & `django_iubenda-1.6.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,68 @@
 Metadata-Version: 2.1
 Name: django-iubenda
-Version: 1.6.0
+Version: 1.6.4
 Summary: Django''s application for handling privacy and cookie policies configured with Iubenda.
 Home-page: https://github.com/DLRSP/django-iubenda
-Author: DLRSP
-Author-email: dlrsp.dev@gmail.com
+Author-email: DLRSP <dlrsp.dev@gmail.com>
 License: MIT License
+        
+        Copyright (c) 2010-present DLRSP (https://dlrsp.org) and other contributors.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Keywords: django,iubenda,privacy,cookie
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=3.2
-Provides-Extra: testing
-Requires-Dist: coverage; extra == "testing"
-Requires-Dist: codecov; extra == "testing"
-Provides-Extra: linting
-Requires-Dist: flake8; extra == "linting"
-Requires-Dist: pylint; extra == "linting"
+Requires-Dist: django
+Requires-Dist: django-modeltranslation
+Requires-Dist: requests
+Requires-Dist: django_compressor
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: codecov; extra == "test"
+Provides-Extra: lint
+Requires-Dist: black; extra == "lint"
+Requires-Dist: flake8; extra == "lint"
 
 # django-iubenda [![PyPi license](https://img.shields.io/pypi/l/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 
 [![PyPi status](https://img.shields.io/pypi/status/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi version](https://img.shields.io/pypi/v/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi python version](https://img.shields.io/pypi/pyversions/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi downloads](https://img.shields.io/pypi/dm/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
```

### Comparing `django_iubenda-1.6.0/README.md` & `django_iubenda-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/mkdocs.yml` & `django_iubenda-1.6.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/requirements/py310-django32.txt` & `django_iubenda-1.6.4/requirements/py310-django32.txt`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/requirements/py310-django42.txt` & `django_iubenda-1.6.4/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/requirements/py311-django32.txt` & `django_iubenda-1.6.4/requirements/py311-django32.txt`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/requirements/py311-django42.txt` & `django_iubenda-1.6.4/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/requirements/py38-django32.txt` & `django_iubenda-1.6.4/requirements/py38-django32.txt`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/requirements/py38-django42.txt` & `django_iubenda-1.6.4/requirements/py38-django42.txt`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/requirements/py39-django32.txt` & `django_iubenda-1.6.4/requirements/py39-django32.txt`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/requirements/py39-django42.txt` & `django_iubenda-1.6.4/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/runtests.py` & `django_iubenda-1.6.4/runtests.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/setup.py` & `django_iubenda-1.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/django_iubenda.egg-info/PKG-INFO` & `django_iubenda-1.6.4/src/django_iubenda.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,68 @@
 Metadata-Version: 2.1
 Name: django-iubenda
-Version: 1.6.0
+Version: 1.6.4
 Summary: Django''s application for handling privacy and cookie policies configured with Iubenda.
 Home-page: https://github.com/DLRSP/django-iubenda
-Author: DLRSP
-Author-email: dlrsp.dev@gmail.com
+Author-email: DLRSP <dlrsp.dev@gmail.com>
 License: MIT License
+        
+        Copyright (c) 2010-present DLRSP (https://dlrsp.org) and other contributors.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Keywords: django,iubenda,privacy,cookie
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=3.2
-Provides-Extra: testing
-Requires-Dist: coverage; extra == "testing"
-Requires-Dist: codecov; extra == "testing"
-Provides-Extra: linting
-Requires-Dist: flake8; extra == "linting"
-Requires-Dist: pylint; extra == "linting"
+Requires-Dist: django
+Requires-Dist: django-modeltranslation
+Requires-Dist: requests
+Requires-Dist: django_compressor
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: codecov; extra == "test"
+Provides-Extra: lint
+Requires-Dist: black; extra == "lint"
+Requires-Dist: flake8; extra == "lint"
 
 # django-iubenda [![PyPi license](https://img.shields.io/pypi/l/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 
 [![PyPi status](https://img.shields.io/pypi/status/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi version](https://img.shields.io/pypi/v/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi python version](https://img.shields.io/pypi/pyversions/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi downloads](https://img.shields.io/pypi/dm/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
```

### Comparing `django_iubenda-1.6.0/src/django_iubenda.egg-info/SOURCES.txt` & `django_iubenda-1.6.4/src/django_iubenda.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -6,34 +6,26 @@
 README.md
 mkdocs.yml
 pyproject.toml
 runtests.py
 setup.cfg
 setup.py
 tox.ini
-requirements/dev.in
-requirements/docs.in
-requirements/docs.txt
-requirements/py310-dev.txt
 requirements/py310-django32.txt
 requirements/py310-django42.txt
-requirements/py311-dev.txt
 requirements/py311-django32.txt
 requirements/py311-django42.txt
-requirements/py38-dev.txt
 requirements/py38-django32.txt
 requirements/py38-django42.txt
-requirements/py39-dev.txt
 requirements/py39-django32.txt
 requirements/py39-django42.txt
 requirements/requirements.in
 src/django_iubenda.egg-info/PKG-INFO
 src/django_iubenda.egg-info/SOURCES.txt
 src/django_iubenda.egg-info/dependency_links.txt
-src/django_iubenda.egg-info/not-zip-safe
 src/django_iubenda.egg-info/requires.txt
 src/django_iubenda.egg-info/top_level.txt
 src/iubenda/__init__.py
 src/iubenda/admin.py
 src/iubenda/apps.py
 src/iubenda/context_processors.py
 src/iubenda/models.py
```

### Comparing `django_iubenda-1.6.0/src/iubenda/context_processors.py` & `django_iubenda-1.6.4/src/iubenda/context_processors.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/iubenda/locale/it/LC_MESSAGES/django.po` & `django_iubenda-1.6.4/src/iubenda/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/iubenda/migrations/0001_initial.py` & `django_iubenda-1.6.4/src/iubenda/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/iubenda/models.py` & `django_iubenda-1.6.4/src/iubenda/models.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/iubenda/static/iubenda/css/iubenda_badge.css` & `django_iubenda-1.6.4/src/iubenda/static/iubenda/css/iubenda_badge.css`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/iubenda/static/iubenda/css/iubenda_policy.css` & `django_iubenda-1.6.4/src/iubenda/static/iubenda/css/iubenda_policy.css`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/iubenda/templates/iubenda/cookie-compress.html` & `django_iubenda-1.6.4/src/iubenda/templates/iubenda/cookie-compress.html`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/iubenda/templates/iubenda/cookie.html` & `django_iubenda-1.6.4/src/iubenda/templates/iubenda/cookie.html`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/iubenda/templates/iubenda/include-content.html` & `django_iubenda-1.6.4/src/iubenda/templates/iubenda/include-content.html`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/iubenda/templates/iubenda/privacy-compress.html` & `django_iubenda-1.6.4/src/iubenda/templates/iubenda/privacy-compress.html`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/iubenda/templates/iubenda/privacy.html` & `django_iubenda-1.6.4/src/iubenda/templates/iubenda/privacy.html`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/iubenda/urls.py` & `django_iubenda-1.6.4/src/iubenda/urls.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/src/iubenda/views.py` & `django_iubenda-1.6.4/src/iubenda/views.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/tests/settings.py` & `django_iubenda-1.6.4/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/tests/test_iubenda_custom_options.py` & `django_iubenda-1.6.4/tests/test_iubenda_custom_options.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/tests/test_iubenda_default_options.py` & `django_iubenda-1.6.4/tests/test_iubenda_default_options.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/tests/test_iubenda_settings.py` & `django_iubenda-1.6.4/tests/test_iubenda_settings.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/tests/test_iubenda_template.py` & `django_iubenda-1.6.4/tests/test_iubenda_template.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/tests/test_iubenda_urls.py` & `django_iubenda-1.6.4/tests/test_iubenda_urls.py`

 * *Files identical despite different names*

### Comparing `django_iubenda-1.6.0/tests/urls.py` & `django_iubenda-1.6.4/tests/urls.py`

 * *Files identical despite different names*

