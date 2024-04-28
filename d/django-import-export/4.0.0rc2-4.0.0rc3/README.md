# Comparing `tmp/django-import-export-4.0.0rc2.tar.gz` & `tmp/django_import_export-4.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-import-export-4.0.0rc2.tar", last modified: Mon Apr  8 18:43:19 2024, max compression
+gzip compressed data, was "django_import_export-4.0.0rc3.tar", last modified: Sat Apr 13 13:35:48 2024, max compression
```

## Comparing `django-import-export-4.0.0rc2.tar` & `django_import_export-4.0.0rc3.tar`

### file list

```diff
@@ -1,333 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.729486 django-import-export-4.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.689487 django-import-export-4.0.0rc2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.689487 django-import-export-4.0.0rc2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.689487 django-import-export-4.0.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-08 18:43:19.729486 django-import-export-4.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.725486 django-import-export-4.0.0rc2/django_import_export.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-08 18:43:19.000000 django-import-export-4.0.0rc2/django_import_export.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-08 18:43:19.000000 django-import-export-4.0.0rc2/django_import_export.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:43:19.000000 django-import-export-4.0.0rc2/django_import_export.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-08 18:43:19.000000 django-import-export-4.0.0rc2/django_import_export.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 18:43:19.000000 django-import-export-4.0.0rc2/django_import_export.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.697486 django-import-export-4.0.0rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.697486 django-import-export-4.0.0rc2/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/change-form-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/custom-export-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/custom-import-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/date-widget-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/django-import-export-change.png
--rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/django-import-export-export-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/django-import-export-import-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/django-import-export-import.png
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/export-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    33286 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/export_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/import-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/import_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/non-field-specific-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/_static/images/select-for-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/admin_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    30548 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_admin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_fields.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_forms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_instance_loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_mixins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_tmp_storages.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/api_widgets.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/bulk_import.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/celery.rst
--rw-r--r--   0 runner    (1001) docker     (127)    30218 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/export_workflow.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    10047 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.697486 django-import-export-4.0.0rc2/docs/image_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/image_src/export_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/image_src/import_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/import_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-08 18:43:19.000000 django-import-export-4.0.0rc2/import_export/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    35251 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/formats/base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/instance_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.701486 django-import-export-4.0.0rc2/import_export/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/kz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/kz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/kz/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/kz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.681487 django-import-export-4.0.0rc2/import_export/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.705486 django-import-export-4.0.0rc2/import_export/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/import_export/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/import_export/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/import_export/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    48286 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/import_export/static/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/static/import_export/export.css
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/static/import_export/export_selectable_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/static/import_export/guess_format.js
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/static/import_export/import.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/import_export/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_list_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_list_export_item.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_list_import.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_list_import_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/change_list_import_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/export.html
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/import.html
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templates/admin/import_export/resource_fields_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/import_export/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/templatetags/import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21360 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/import_export/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.709486 django-import-export-4.0.0rc2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/runtests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/runtests.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:43:19.729486 django-import-export-4.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.713486 django-import-export-4.0.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/books-sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.713486 django-import-export-4.0.0rc2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.713486 django-import-export-4.0.0rc2/tests/core/exports/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/authors.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-ISO-8859-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-dos.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-empty-author-email.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-for-delete.csv
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-invalid-date.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-mac.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-mac.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-unicode.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books-unicode.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books.csv
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books.json
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books.xls
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/books.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/exports/child.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.717486 django-import-export-4.0.0rc2/tests/core/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/fixtures/author.json
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/fixtures/book.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/fixtures/category.json
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.717486 django-import-export-4.0.0rc2/tests/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0002_book_published_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0003_withfloatfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0004_bookwithchapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0005_addparentchild.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0006_auto_20171130_0147.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0007_auto_20180628_0411.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0008_auto_20190409_0846.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0009_auto_20211111_0807.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0010_uuidbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0012_delete_legacybook.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0013_alter_author_birthday.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/0014_bookwithchapternumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/tests/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.717486 django-import-export-4.0.0rc2/tests/core/templates/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.717486 django-import-export-4.0.0rc2/tests/core/templates/core/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/templates/core/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/templates/core/category_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.721486 django-import-export-4.0.0rc2/tests/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.721486 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    41866 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_instance_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_invalidrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.721486 django-import-export-4.0.0rc2/tests/core/tests/test_resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_bulk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_import_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.725486 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)    28373 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/tests/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.685487 django-import-export-4.0.0rc2/tests/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.725486 django-import-export-4.0.0rc2/tests/docker/db/
--rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/docker/db/init-mysql-db.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/docker/db/init-postgres-db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:19.725486 django-import-export-4.0.0rc2/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/scripts/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-08 18:43:10.000000 django-import-export-4.0.0rc2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.528308 django_import_export-4.0.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.488308 django_import_export-4.0.0rc3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.492308 django_import_export-4.0.0rc3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.492308 django_import_export-4.0.0rc3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-13 13:35:48.528308 django_import_export-4.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.524308 django_import_export-4.0.0rc3/django_import_export.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-13 13:35:48.000000 django_import_export-4.0.0rc3/django_import_export.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-13 13:35:48.000000 django_import_export-4.0.0rc3/django_import_export.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:35:48.000000 django_import_export-4.0.0rc3/django_import_export.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 13:35:48.000000 django_import_export-4.0.0rc3/django_import_export.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 13:35:48.000000 django_import_export-4.0.0rc3/django_import_export.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.496308 django_import_export-4.0.0rc3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.500308 django_import_export-4.0.0rc3/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/change-form-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/custom-export-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/custom-import-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/date-widget-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/django-import-export-change.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/django-import-export-export-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/django-import-export-import-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/django-import-export-import.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/export-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33286 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/export_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/import-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/import_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/non-field-specific-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/select-for-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/admin_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    30548 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_admin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_forms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_instance_loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_tmp_storages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_widgets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/bulk_import.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    30340 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/export_workflow.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10047 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.500308 django_import_export-4.0.0rc3/docs/image_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/image_src/export_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/image_src/import_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/import_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.500308 django_import_export-4.0.0rc3/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 13:35:48.000000 django_import_export-4.0.0rc3/import_export/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35262 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.500308 django_import_export-4.0.0rc3/import_export/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/formats/base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/instance_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.500308 django_import_export-4.0.0rc3/import_export/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.500308 django_import_export-4.0.0rc3/import_export/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/kz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/kz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/kz/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/kz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48286 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/static/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/static/import_export/export.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/static/import_export/export_selectable_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/static/import_export/guess_format.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/static/import_export/import.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_list_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_list_export_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_list_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_list_import_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_list_import_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/export.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/resource_fields_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.512308 django_import_export-4.0.0rc3/import_export/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templatetags/import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21360 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.512308 django_import_export-4.0.0rc3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/runtests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/runtests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:35:48.528308 django_import_export-4.0.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.512308 django_import_export-4.0.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/books-sample.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.512308 django_import_export-4.0.0rc3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.516308 django_import_export-4.0.0rc3/tests/core/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/authors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-ISO-8859-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-dos.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-empty-author-email.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-for-delete.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-invalid-date.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-mac.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-mac.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-unicode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-unicode.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/child.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.516308 django_import_export-4.0.0rc3/tests/core/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/fixtures/author.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/fixtures/book.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/fixtures/category.json
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.516308 django_import_export-4.0.0rc3/tests/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0002_book_published_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0003_withfloatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0004_bookwithchapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0005_addparentchild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0006_auto_20171130_0147.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0007_auto_20180628_0411.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0008_auto_20190409_0846.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0009_auto_20211111_0807.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0010_uuidbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0012_delete_legacybook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0013_alter_author_birthday.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0014_bookwithchapternumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.484308 django_import_export-4.0.0rc3/tests/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.516308 django_import_export-4.0.0rc3/tests/core/templates/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.516308 django_import_export-4.0.0rc3/tests/core/templates/core/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/templates/core/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/templates/core/category_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.520308 django_import_export-4.0.0rc3/tests/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.520308 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41866 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_instance_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_invalidrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.520308 django_import_export-4.0.0rc3/tests/core/tests/test_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_bulk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.524308 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28373 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.484308 django_import_export-4.0.0rc3/tests/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.524308 django_import_export-4.0.0rc3/tests/docker/db/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/docker/db/init-mysql-db.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/docker/db/init-postgres-db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.524308 django_import_export-4.0.0rc3/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/scripts/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tox.ini
```

### Comparing `django-import-export-4.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md` & `django_import_export-4.0.0rc3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/.github/ISSUE_TEMPLATE/question.md` & `django_import_export-4.0.0rc3/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/.github/stale.yml` & `django_import_export-4.0.0rc3/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/.github/workflows/release.yml` & `django_import_export-4.0.0rc3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/.github/workflows/test.yml` & `django_import_export-4.0.0rc3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/AUTHORS` & `django_import_export-4.0.0rc3/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/CODE_OF_CONDUCT.md` & `django_import_export-4.0.0rc3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/LICENSE` & `django_import_export-4.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/Makefile` & `django_import_export-4.0.0rc3/Makefile`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/PKG-INFO` & `django_import_export-4.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.0rc2
+Version: 4.0.0rc3
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `django-import-export-4.0.0rc2/README.rst` & `django_import_export-4.0.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/RELEASE.md` & `django_import_export-4.0.0rc3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/django_import_export.egg-info/PKG-INFO` & `django_import_export-4.0.0rc3/django_import_export.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.0rc2
+Version: 4.0.0rc3
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `django-import-export-4.0.0rc2/django_import_export.egg-info/SOURCES.txt` & `django_import_export-4.0.0rc3/django_import_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/Makefile` & `django_import_export-4.0.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/change-form-export.png` & `django_import_export-4.0.0rc3/docs/_static/images/change-form-export.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/custom-export-form.png` & `django_import_export-4.0.0rc3/docs/_static/images/custom-export-form.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/custom-import-form.png` & `django_import_export-4.0.0rc3/docs/_static/images/custom-import-form.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/date-widget-validation-error.png` & `django_import_export-4.0.0rc3/docs/_static/images/date-widget-validation-error.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/django-import-export-change.png` & `django_import_export-4.0.0rc3/docs/_static/images/django-import-export-change.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/django-import-export-export-confirm.png` & `django_import_export-4.0.0rc3/docs/_static/images/django-import-export-export-confirm.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/django-import-export-import-confirm.png` & `django_import_export-4.0.0rc3/docs/_static/images/django-import-export-import-confirm.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/django-import-export-import.png` & `django_import_export-4.0.0rc3/docs/_static/images/django-import-export-import.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/export-button.png` & `django_import_export-4.0.0rc3/docs/_static/images/export-button.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/export_workflow.svg` & `django_import_export-4.0.0rc3/docs/_static/images/export_workflow.svg`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/import-button.png` & `django_import_export-4.0.0rc3/docs/_static/images/import-button.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/import_workflow.svg` & `django_import_export-4.0.0rc3/docs/_static/images/import_workflow.svg`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/non-field-specific-validation-error.png` & `django_import_export-4.0.0rc3/docs/_static/images/non-field-specific-validation-error.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/_static/images/select-for-export.png` & `django_import_export-4.0.0rc3/docs/_static/images/select-for-export.png`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/admin_integration.rst` & `django_import_export-4.0.0rc3/docs/admin_integration.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/advanced_usage.rst` & `django_import_export-4.0.0rc3/docs/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/api_mixins.rst` & `django_import_export-4.0.0rc3/docs/api_mixins.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/api_widgets.rst` & `django_import_export-4.0.0rc3/docs/api_widgets.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/bulk_import.rst` & `django_import_export-4.0.0rc3/docs/bulk_import.rst`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,17 @@
   resource fields are declared appropriately with the correct widgets.  If an exception is raised by a bulk operation,
   then that batch will fail.  It's also possible that transactions can be left in a corrupted state.  Other batches may
   be successfully persisted, meaning that you may have a partially successful import.
 
 * In bulk mode, exceptions are not linked to a row.  Any exceptions raised by bulk operations are logged and returned
   as critical (non-validation) errors (and re-raised if ``raise_errors`` is true).
 
-* If you use :class:`~import_export.widgets.ForeignKeyWidget` then this can affect performance, because it reads from
-  the database for each row.  If this is an issue then create a subclass which caches ``get_queryset()`` results rather
-  than reading for each invocation.
+* If you use :class:`~import_export.widgets.ForeignKeyWidget` then this should not affect performance during lookups,
+  because the ``QuerySet`` cache should be used.  Some more information
+  `here <https://stackoverflow.com/a/78309357/39296>`_.
 
 * If there is the potential for concurrent writes to a table during a bulk operation, then you need to consider the
   potential impact of this.  Refer to :ref:`concurrent-writes` for more information.
 
 For more information, please read the Django documentation on
 `bulk_create() <https://docs.djangoproject.com/en/stable/ref/models/querysets/#bulk-create>`_ and
 `bulk_update() <https://docs.djangoproject.com/en/stable/ref/models/querysets/#bulk-update>`_.
```

### Comparing `django-import-export-4.0.0rc2/docs/changelog.rst` & `django_import_export-4.0.0rc3/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Changelog
 =========
 
 .. warning::
 
     Version 4 introduces breaking changes.  Please refer to :doc:`release notes<release_notes>`.
 
+4.0.0-rc.3 (unreleased)
+-----------------------
+
+- fix form not being passed to ``get_import_resource_kwargs()`` (#1789)
+
 4.0.0-rc.2 (2024-04-08)
 -----------------------
 
 - Add form error if source file contains invalid header (#1780)
 - Fix for incorrect header order on 'confirm' page (#1786)
 - Remove unneeded format method overrides (#1785)
 - Support dynamic selection of Resource class based on request property (#1787)
```

### Comparing `django-import-export-4.0.0rc2/docs/conf.py` & `django_import_export-4.0.0rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/contributing.rst` & `django_import_export-4.0.0rc3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/export_workflow.rst` & `django_import_export-4.0.0rc3/docs/export_workflow.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/faq.rst` & `django_import_export-4.0.0rc3/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/getting_started.rst` & `django_import_export-4.0.0rc3/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/image_src/export_workflow.txt` & `django_import_export-4.0.0rc3/docs/image_src/export_workflow.txt`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/image_src/import_workflow.txt` & `django_import_export-4.0.0rc3/docs/image_src/import_workflow.txt`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/import_workflow.rst` & `django_import_export-4.0.0rc3/docs/import_workflow.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/index.rst` & `django_import_export-4.0.0rc3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/installation.rst` & `django_import_export-4.0.0rc3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/make.bat` & `django_import_export-4.0.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/release_notes.rst` & `django_import_export-4.0.0rc3/docs/release_notes.rst`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/docs/testing.rst` & `django_import_export-4.0.0rc3/docs/testing.rst`

 * *Files 12% similar despite different names*

```diff
@@ -60,8 +60,24 @@
 
   # run creates, updates, and deletes
   ./manage.py runscript bulk_import
 
   # pass 'create', 'update' or 'delete' to run the single test
   ./manage.py runscript bulk_import --script-args create
 
+Enable logging
+^^^^^^^^^^^^^^
+
+You can see console debug logging by updating the ``LOGGING`` block in `settings.py`::
+
+    LOGGING = {
+        "version": 1,
+        "handlers": {"console": {"class": "logging.StreamHandler"}},
+        "root": {
+            "handlers": ["console"],
+        },
+        "loggers": {
+            "django.db.backends": {"level": "DEBUG", "handlers": ["console"]},
+        }
+    }
+
```

### Comparing `django-import-export-4.0.0rc2/import_export/admin.py` & `django_import_export-4.0.0rc3/import_export/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     def process_dataset(
         self,
         dataset,
         form,
         request,
         **kwargs,
     ):
-        res_kwargs = self.get_import_resource_kwargs(request, **kwargs)
+        res_kwargs = self.get_import_resource_kwargs(request, form=form, **kwargs)
         resource = self.choose_import_resource_class(form, request)(**res_kwargs)
         imp_kwargs = self.get_import_data_kwargs(request=request, form=form, **kwargs)
         imp_kwargs["retain_instance_in_row_result"] = True
 
         return resource.import_data(
             dataset,
             dry_run=False,
```

### Comparing `django-import-export-4.0.0rc2/import_export/declarative.py` & `django_import_export-4.0.0rc3/import_export/declarative.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/exceptions.py` & `django_import_export-4.0.0rc3/import_export/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/fields.py` & `django_import_export-4.0.0rc3/import_export/fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/formats/base_formats.py` & `django_import_export-4.0.0rc3/import_export/formats/base_formats.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/forms.py` & `django_import_export-4.0.0rc3/import_export/forms.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/instance_loaders.py` & `django_import_export-4.0.0rc3/import_export/instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/ar/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/ar/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/bg/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/bg/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/ca/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/ca/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/cs/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/cs/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/de/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/de/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/es/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/es/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/es_AR/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/es_AR/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/fa/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/fa/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/fi/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/fi/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/fr/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/fr/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/it/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/it/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/ja/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/ja/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/ko/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/ko/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/kz/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/kz/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/kz/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/kz/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/nl/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/nl/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/pl/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/pl/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/pt_BR/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/pt_BR/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/ru/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/ru/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/sk/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/sk/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/tr/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/tr/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_import_export-4.0.0rc3/import_export/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/locale/zh_Hans/LC_MESSAGES/django.po` & `django_import_export-4.0.0rc3/import_export/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/mixins.py` & `django_import_export-4.0.0rc3/import_export/mixins.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/options.py` & `django_import_export-4.0.0rc3/import_export/options.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/resources.py` & `django_import_export-4.0.0rc3/import_export/resources.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/results.py` & `django_import_export-4.0.0rc3/import_export/results.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/static/import_export/export_selectable_fields.js` & `django_import_export-4.0.0rc3/import_export/static/import_export/export_selectable_fields.js`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/static/import_export/guess_format.js` & `django_import_export-4.0.0rc3/import_export/static/import_export/guess_format.js`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/static/import_export/import.css` & `django_import_export-4.0.0rc3/import_export/static/import_export/import.css`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/templates/admin/import_export/base.html` & `django_import_export-4.0.0rc3/import_export/templates/admin/import_export/base.html`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/templates/admin/import_export/export.html` & `django_import_export-4.0.0rc3/import_export/templates/admin/import_export/export.html`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/templates/admin/import_export/import.html` & `django_import_export-4.0.0rc3/import_export/templates/admin/import_export/import.html`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/templates/admin/import_export/resource_fields_list.html` & `django_import_export-4.0.0rc3/import_export/templates/admin/import_export/resource_fields_list.html`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/tmp_storages.py` & `django_import_export-4.0.0rc3/import_export/tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/utils.py` & `django_import_export-4.0.0rc3/import_export/utils.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/import_export/widgets.py` & `django_import_export-4.0.0rc3/import_export/widgets.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/pyproject.toml` & `django_import_export-4.0.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/runtests.py` & `django_import_export-4.0.0rc3/runtests.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/runtests.sh` & `django_import_export-4.0.0rc3/runtests.sh`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/admin.py` & `django_import_export-4.0.0rc3/tests/core/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,17 @@
             initial["author"] = import_form.cleaned_data["author"].id
         return initial
 
     def get_import_resource_kwargs(self, request, **kwargs):
         # update resource kwargs so that the Resource is passed the authenticated user
         # This is included as an example of how dynamic values
         # can be passed to resources
+        if "form" not in kwargs:
+            # test for #1789
+            raise ValueError("'form' param was expected in kwargs")
         kwargs = super().get_resource_kwargs(request, **kwargs)
         kwargs.update({"user": request.user})
         return kwargs
 
     def get_export_resource_kwargs(self, request, **kwargs):
         # this is overridden to demonstrate that custom form fields can be used
         # to override the export query.
```

### Comparing `django-import-export-4.0.0rc2/tests/core/exports/books-empty-author-email.xlsx` & `django_import_export-4.0.0rc3/tests/core/exports/books-empty-author-email.xlsx`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/exports/books.json` & `django_import_export-4.0.0rc3/tests/core/exports/books.json`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/exports/books.xls` & `django_import_export-4.0.0rc3/tests/core/exports/books.xls`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/exports/books.xlsx` & `django_import_export-4.0.0rc3/tests/core/exports/books.xlsx`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/fixtures/book.json` & `django_import_export-4.0.0rc3/tests/core/fixtures/book.json`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/forms.py` & `django_import_export-4.0.0rc3/tests/core/forms.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/migrations/0001_initial.py` & `django_import_export-4.0.0rc3/tests/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/migrations/0003_withfloatfield.py` & `django_import_export-4.0.0rc3/tests/core/migrations/0003_withfloatfield.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/migrations/0004_bookwithchapters.py` & `django_import_export-4.0.0rc3/tests/core/migrations/0004_bookwithchapters.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/migrations/0005_addparentchild.py` & `django_import_export-4.0.0rc3/tests/core/migrations/0005_addparentchild.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/migrations/0007_auto_20180628_0411.py` & `django_import_export-4.0.0rc3/tests/core/migrations/0007_auto_20180628_0411.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/migrations/0008_auto_20190409_0846.py` & `django_import_export-4.0.0rc3/tests/core/migrations/0008_auto_20190409_0846.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/migrations/0009_auto_20211111_0807.py` & `django_import_export-4.0.0rc3/tests/core/migrations/0009_auto_20211111_0807.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/migrations/0010_uuidbook.py` & `django_import_export-4.0.0rc3/tests/core/migrations/0010_uuidbook.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py` & `django_import_export-4.0.0rc3/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/migrations/0014_bookwithchapternumbers.py` & `django_import_export-4.0.0rc3/tests/core/migrations/0014_bookwithchapternumbers.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/models.py` & `django_import_export-4.0.0rc3/tests/core/models.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/admin_integration/mixins.py` & `django_import_export-4.0.0rc3/tests/core/tests/admin_integration/mixins.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_action.py` & `django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_action.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_export.py` & `django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_export.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_import.py` & `django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_import.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/admin_integration/test_views.py` & `django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_views.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/resources.py` & `django_import_export-4.0.0rc3/tests/core/tests/resources.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_base_formats.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_base_formats.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_declarative.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_declarative.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_fields.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_forms.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_instance_loaders.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_invalidrow.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_invalidrow.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_mixins.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_permissions.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_bulk_operations.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_bulk_operations.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_diffs.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_diffs.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_import_export.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_import_export.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_misc.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_misc.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_data_handling.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_data_handling.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_data_import.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_data_import.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_error_handling.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_export.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_export.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_fields.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_m2m.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_m2m.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_queryset.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_queryset.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_relationship.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_relationship.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_resources/test_relationships.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_relationships.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_results.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_tmp_storages.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/test_widgets.py` & `django_import_export-4.0.0rc3/tests/core/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/core/tests/utils.py` & `django_import_export-4.0.0rc3/tests/core/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/docker-compose.yml` & `django_import_export-4.0.0rc3/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/scripts/bulk_import.py` & `django_import_export-4.0.0rc3/tests/scripts/bulk_import.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tests/settings.py` & `django_import_export-4.0.0rc3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-import-export-4.0.0rc2/tox.ini` & `django_import_export-4.0.0rc3/tox.ini`

 * *Files identical despite different names*

