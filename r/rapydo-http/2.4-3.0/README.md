# Comparing `tmp/rapydo_http-2.4.tar.gz` & `tmp/rapydo_http-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapydo_http-2.4.tar", last modified: Thu Dec  8 15:17:54 2022, max compression
+gzip compressed data, was "rapydo_http-3.0.tar", last modified: Sun Apr 28 07:09:35 2024, max compression
```

## Comparing `rapydo_http-2.4.tar` & `rapydo_http-3.0.tar`

### file list

```diff
@@ -1,175 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.777819 rapydo_http-2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2022-12-08 15:17:44.000000 rapydo_http-2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2022-12-08 15:17:54.777819 rapydo_http-2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-08 15:17:44.000000 rapydo_http-2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.753818 rapydo_http-2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2022-12-08 15:17:44.000000 rapydo_http-2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2022-12-08 15:17:44.000000 rapydo_http-2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.753818 rapydo_http-2.4/rapydo_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2022-12-08 15:17:54.000000 rapydo_http-2.4/rapydo_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2022-12-08 15:17:54.000000 rapydo_http-2.4/rapydo_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 15:17:54.000000 rapydo_http-2.4/rapydo_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-08 15:17:54.000000 rapydo_http-2.4/rapydo_http.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2022-12-08 15:17:54.000000 rapydo_http-2.4/rapydo_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-08 15:17:54.000000 rapydo_http-2.4/rapydo_http.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.757818 rapydo_http-2.4/restapi/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/__commands__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.757818 rapydo_http-2.4/restapi/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)    19071 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.757818 rapydo_http-2.4/restapi/connectors/celery/
--rw-r--r--   0 runner    (1001) docker     (123)    21956 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/celery/beat.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/celery/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.757818 rapydo_http-2.4/restapi/connectors/ftp/
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/ftp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.757818 rapydo_http-2.4/restapi/connectors/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)    18513 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/neo4j/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/neo4j/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/neo4j/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.757818 rapydo_http-2.4/restapi/connectors/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.757818 rapydo_http-2.4/restapi/connectors/redis/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.757818 rapydo_http-2.4/restapi/connectors/smtp/
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/mailmock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.761818 rapydo_http-2.4/restapi/connectors/smtp/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/templates/activate_account.html
--rw-r--r--   0 runner    (1001) docker     (123)      902 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/templates/blocked_credentials.html
--rw-r--r--   0 runner    (1001) docker     (123)      300 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/templates/celery_error_notification.html
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/templates/email_footer.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/templates/email_header.html
--rw-r--r--   0 runner    (1001) docker     (123)      357 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/templates/new_credentials.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/templates/new_user_registered.html
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/templates/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (123)      353 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/smtp/templates/update_credentials.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.761818 rapydo_http-2.4/restapi/connectors/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)    21923 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/connectors/sqlalchemy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/customizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.765818 rapydo_http-2.4/restapi/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/admin_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/admin_logins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/admin_server_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/admin_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/admin_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/group_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/login_unlock.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/profile_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/profile_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/reset_password.py
--rw-r--r--   0 runner    (1001) docker     (123)    15817 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/send_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9241 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/swagger_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_depends_on.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_gzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_parameters_injection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/test_vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/endpoints/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.765818 rapydo_http-2.4/restapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/models/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/models/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.765818 rapydo_http-2.4/restapi/rest/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/rest/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10266 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/rest/bearer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/rest/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14649 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/rest/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16058 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/rest/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.769818 rapydo_http-2.4/restapi/services/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45036 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/services/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/services/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/services/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/services/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.769818 rapydo_http-2.4/restapi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    26776 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/tests_initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.769818 rapydo_http-2.4/restapi/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/utilities/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/utilities/faker.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/utilities/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/utilities/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/utilities/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/utilities/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/utilities/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-08 15:17:44.000000 rapydo_http-2.4/restapi/utilities/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 15:17:54.777819 rapydo_http-2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.769818 rapydo_http-2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:54.773818 rapydo_http-2.4/tests/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_aaa_unused_credentials_step1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_connector_celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_connector_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10971 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_connector_neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_connector_rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_connector_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_connector_smtp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_connector_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_admin_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_admin_logins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_admin_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_admin_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    26339 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    17386 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_db_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_depends_on.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_group_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21691 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_login_ban.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_login_expiration.py
--rw-r--r--   0 runner    (1001) docker     (123)    25665 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_login_profile_logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_parameters_injection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_password_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15483 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_registration_and_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_send_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    12950 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_upload_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_users_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_endpoints_vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    26397 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_module_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    43105 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_module_miscellanous.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_xxx_unused_credentials_step2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_zzz1_destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/base/test_zzz2_re-init.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2022-12-08 15:17:44.000000 rapydo_http-2.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.249632 rapydo_http-3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-28 07:09:31.000000 rapydo_http-3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-28 07:09:35.249632 rapydo_http-3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-28 07:09:31.000000 rapydo_http-3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.225632 rapydo_http-3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-28 07:09:31.000000 rapydo_http-3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-28 07:09:31.000000 rapydo_http-3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.245632 rapydo_http-3.0/rapydo_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-28 07:09:35.000000 rapydo_http-3.0/rapydo_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-28 07:09:35.000000 rapydo_http-3.0/rapydo_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 07:09:35.000000 rapydo_http-3.0/rapydo_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-28 07:09:35.000000 rapydo_http-3.0/rapydo_http.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-28 07:09:35.000000 rapydo_http-3.0/rapydo_http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-28 07:09:35.000000 rapydo_http-3.0/rapydo_http.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 07:09:31.000000 rapydo_http-3.0/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-28 07:09:31.000000 rapydo_http-3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-28 07:09:31.000000 rapydo_http-3.0/requirements.types.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.225632 rapydo_http-3.0/restapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/__commands__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/alembic_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.225632 rapydo_http-3.0/restapi/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.229632 rapydo_http-3.0/restapi/connectors/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/celery/beat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/celery/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.229632 rapydo_http-3.0/restapi/connectors/ftp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/ftp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.229632 rapydo_http-3.0/restapi/connectors/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (127)    18734 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/neo4j/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/neo4j/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/neo4j/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.229632 rapydo_http-3.0/restapi/connectors/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)    13881 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.229632 rapydo_http-3.0/restapi/connectors/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.229632 rapydo_http-3.0/restapi/connectors/smtp/
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/mailmock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.229632 rapydo_http-3.0/restapi/connectors/smtp/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/templates/activate_account.html
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/templates/blocked_credentials.html
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/templates/celery_error_notification.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/templates/email_footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/templates/email_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/templates/new_credentials.html
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/templates/new_user_registered.html
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/templates/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/smtp/templates/update_credentials.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.229632 rapydo_http-3.0/restapi/connectors/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)    21202 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/connectors/sqlalchemy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/customizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17638 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.237632 rapydo_http-3.0/restapi/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/admin_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/admin_logins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/admin_server_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/admin_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/admin_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/login_unlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/profile_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/profile_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/reset_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15802 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/send_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/swagger_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_depends_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_gzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_parameters_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/endpoints/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.237632 rapydo_http-3.0/restapi/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/models/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/models/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.237632 rapydo_http-3.0/restapi/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/rest/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/rest/bearer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/rest/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14612 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/rest/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15913 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/rest/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.237632 rapydo_http-3.0/restapi/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45357 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/services/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/services/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/services/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/services/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.237632 rapydo_http-3.0/restapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    26987 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/tests_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.237632 rapydo_http-3.0/restapi/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/utilities/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/utilities/faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/utilities/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/utilities/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/utilities/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/utilities/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/utilities/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 07:09:31.000000 rapydo_http-3.0/restapi/utilities/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 07:09:35.249632 rapydo_http-3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.221632 rapydo_http-3.0/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.241632 rapydo_http-3.0/stubs/glom/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-28 07:09:31.000000 rapydo_http-3.0/stubs/glom/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.241632 rapydo_http-3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:35.245632 rapydo_http-3.0/tests/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_aaa_unused_credentials_step1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_connector_celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_connector_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12148 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_connector_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_connector_rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_connector_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_connector_smtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_connector_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_admin_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_admin_logins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_admin_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23393 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_admin_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11024 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26319 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_db_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_depends_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21683 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_login_ban.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_login_expiration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25664 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_login_profile_logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_parameters_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_password_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15482 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_registration_and_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_send_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_upload_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_endpoints_users_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26600 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_module_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43504 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_module_miscellanous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_xxx_unused_credentials_step2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_zzz1_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/base/test_zzz2_re-init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 07:09:31.000000 rapydo_http-3.0/tests/conftest.py
```

### Comparing `rapydo_http-2.4/LICENSE` & `rapydo_http-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rapydo_http-2.4/docs/conf.py` & `rapydo_http-3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
 sys.path.insert(0, os.path.abspath(".."))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "RAPyDo HTTP-APIs"
-copyright = "2022, RAPyDo"
+copyright = "RAPyDo"
 author = "RAPyDo"
 
 # The full version, including alpha/beta/rc tags
-release = "2.4"
+release = "3.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `rapydo_http-2.4/pyproject.toml` & `rapydo_http-3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "rapydo_http"
-version = "2.4"
+version = "3.0"
 description = "HTTP API server working on top of the RAPyDo framework"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 dynamic = ["dependencies", "optional-dependencies"]
 readme = "README.md"
 keywords = ["http", "api", "rest", "web", "backend", "rapydo"]
 classifiers=[
     "Programming Language :: Python",
     "Intended Audience :: Developers",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Framework :: Flask",
 ]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = {dev = {file = ["requirements.dev.txt"]}, types = {file = ["requirements.types.txt"]}}
 
@@ -39,15 +39,15 @@
 restapi = ["py.typed", "templates/*", "connectors/smtp/templates/*"]
 
 [tool.setuptools.packages.find]
 exclude = ["stubs"]
 
 [tool.black]
 line-length = 88
-target_version = ['py38', 'py39', 'py310']
+target_version = ['py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
   | \.hg
   | \.mypy_cache
   | \.tox
@@ -59,12 +59,12 @@
   # The following are specific to Black, you probably don't want those.
   | blib2to3
   | tests/data
 )/
 '''
 
 [tool.isort]
-py_version = 38
+py_version = 39
 line_length = 88
 multi_line_output = 3
 include_trailing_comma = true
 ensure_newline_before_comments = true
```

### Comparing `rapydo_http-2.4/rapydo_http.egg-info/SOURCES.txt` & `rapydo_http-3.0/rapydo_http.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
+requirements.dev.txt
+requirements.txt
+requirements.types.txt
 docs/conf.py
 rapydo_http.egg-info/PKG-INFO
 rapydo_http.egg-info/SOURCES.txt
 rapydo_http.egg-info/dependency_links.txt
 rapydo_http.egg-info/entry_points.txt
 rapydo_http.egg-info/requires.txt
 rapydo_http.egg-info/top_level.txt
 restapi/__commands__.py
 restapi/__init__.py
 restapi/__main__.py
+restapi/alembic_env.py
 restapi/config.py
 restapi/customizer.py
 restapi/decorators.py
 restapi/env.py
 restapi/exceptions.py
 restapi/mocks.py
 restapi/py.typed
@@ -75,15 +79,14 @@
 restapi/endpoints/test_gzip.py
 restapi/endpoints/test_inputs.py
 restapi/endpoints/test_neo4j.py
 restapi/endpoints/test_outputs.py
 restapi/endpoints/test_pagination.py
 restapi/endpoints/test_parameters_injection.py
 restapi/endpoints/test_upload.py
-restapi/endpoints/test_vulnerabilities.py
 restapi/endpoints/tokens.py
 restapi/models/__init__.py
 restapi/models/fields.py
 restapi/models/schema.py
 restapi/rest/__init__.py
 restapi/rest/annotations.py
 restapi/rest/bearer.py
@@ -101,14 +104,15 @@
 restapi/utilities/faker.py
 restapi/utilities/globals.py
 restapi/utilities/logs.py
 restapi/utilities/meta.py
 restapi/utilities/processes.py
 restapi/utilities/time.py
 restapi/utilities/uuid.py
+stubs/glom/__init__.pyi
 tests/__init__.py
 tests/conftest.py
 tests/base/__init__.py
 tests/base/test_aaa_unused_credentials_step1.py
 tests/base/test_cli.py
 tests/base/test_connector_celery.py
 tests/base/test_connector_ftp.py
@@ -140,13 +144,12 @@
 tests/base/test_endpoints_registration_and_activation.py
 tests/base/test_endpoints_send_mail.py
 tests/base/test_endpoints_specs.py
 tests/base/test_endpoints_status.py
 tests/base/test_endpoints_tokens.py
 tests/base/test_endpoints_upload_download.py
 tests/base/test_endpoints_users_custom_fields.py
-tests/base/test_endpoints_vulnerabilities.py
 tests/base/test_module_authentication.py
 tests/base/test_module_miscellanous.py
 tests/base/test_xxx_unused_credentials_step2.py
 tests/base/test_zzz1_destroy.py
 tests/base/test_zzz2_re-init.py
```

### Comparing `rapydo_http-2.4/rapydo_http.egg-info/requires.txt` & `rapydo_http-3.0/rapydo_http.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,63 @@
-Flask==2.1.3
+Flask==2.3.3
 flask-apispec==0.11.4
-Flask-Caching==2.0.1
-Flask-Cors==3.0.10
-Flask-SQLAlchemy==2.5.1
-Flask-Migrate==4.0.0
-Werkzeug==2.2.2
-PyJWT==2.6.0
-pyOpenSSL==22.1.0
-passlib[bcrypt]==1.7.4
-marshmallow==3.17.1
-webargs==8.2.0
-apispec==5.2.2
-neomodel==4.0.8
-psycopg2-binary==2.9.5
-PyMySQL==1.0.2
-redis==4.4.0
-pika==1.3.1
-celery[redis]==5.2.7
-flower==1.2.0
-celery-redbeat==2.0.0
-amqp==5.1.1
-pyotp==2.7.0
-segno==1.5.2
-PyYAML==6.0
-loguru==0.6.0
-glom==22.1.0
-requests==2.28.1
-psutil==5.9.4
-plumbum==1.8.0
-html2text==2020.1.16
-orjson==3.8.3
-sentry-sdk[flask]==1.10.1
+Flask-Caching==2.1.0
+Flask-Cors==4.0.0
+SQLAlchemy==2.0.29
+alembic==1.13.1
+Werkzeug==3.0.2
+PyJWT==2.8.0
+pyOpenSSL==24.1.0
+marshmallow==3.21.1
+webargs==8.4.0
+apispec==6.3.1
+neomodel==5.2.1
+neobolt==1.7.17
+psycopg2-binary==2.9.9
+PyMySQL==1.1.0
+redis==5.0.4
+pika==1.3.2
+celery[redis]==5.4.0
+flower==2.0.1
+celery-redbeat==2.2.0
+amqp==5.2.0
+pyotp==2.9.0
+segno==1.6.1
+PyYAML==6.0.1
+loguru==0.7.2
+glom==23.5.0
+requests==2.31.0
+psutil==5.9.8
+plumbum==1.8.2
+html2text==2024.2.26
+orjson==3.10.1
+sentry-sdk[flask]==2.0.1
+bcrypt==4.1.2
+async-timeout==4.0.3
 
 [dev]
-pytest==7.2.0
-pytest-flask==1.2.0
-pytest-cov==4.0.0
-pytest-timeout==2.1.0
-pytest-sugar==0.9.6
-Faker==15.3.4
+pytest==8.1.2
+pytest-flask==1.3.0
+pytest-cov==5.0.0
+pytest-timeout==2.3.1
+pytest-sugar==1.0.0
+Faker==24.14.0
 
 [types]
 rapydo_http[dev]
-mypy==0.991
-lxml==4.9.1
+mypy==1.10.0
+lxml==5.2.1
 html5lib==1.1
-types-pytz==2022.6.0.1
-types-urllib3==1.26.25.4
-types-python-dateutil==2.8.19.4
-types-requests==2.28.11.5
+celery-types==0.22.0
+pika-stubs==0.1.3
 types-certifi==2021.10.8.3
 types-click==7.1.8
-types-PyYAML==6.0.12.2
 types-orjson==3.6.2
-types-redis==4.3.21.6
-pika-stubs==0.1.3
-celery-types==0.14.0
-sqlalchemy-stubs==0.4
+types-python-dateutil==2.9.0.20240316
+types-pytz==2024.1.0.20240417
+types-PyYAML==6.0.12.20240311
+types-redis==4.6.0.20240425
+types-requests==2.31.0.20240406
+types-psycopg2==2.9.21.20240417
+types-urllib3==1.26.25.14
+pyyaml>=5.4
+sentry-sdk>=1.4.1
```

### Comparing `rapydo_http-2.4/restapi/__commands__.py` & `rapydo_http-3.0/restapi/__commands__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import os
 import sys
 import time
 from pathlib import Path
-from typing import Dict, Optional, Tuple
+from typing import Optional
 
 import click
 from flask.cli import FlaskGroup
 
 from restapi import __package__ as current_package
 from restapi.config import BACKEND_PACKAGE, CUSTOM_PACKAGE, PRODUCTION
 from restapi.connectors import Connector
 from restapi.env import Env
+from restapi.server import ServerModes
 from restapi.utilities import print_and_exit
+from restapi.utilities.globals import mem
 from restapi.utilities.logs import log
 from restapi.utilities.processes import find_process, wait_socket
 
 BIND_INTERFACE = "0.0.0.0"
 
 
 @click.group()
 def cli() -> None:  # pragma: no cover
     click.echo("*** RESTful HTTP API ***")
 
 
 def initializing() -> bool:
-
     return find_process(current_package, keywords=["init"], prefix="/usr/local/bin/")
 
 
 # Too dangerous to launch it during tests... skipping tests
 @cli.command()
 def launch() -> None:  # pragma: no cover
     """Launch the RAPyDo-based HTTP API server"""
@@ -48,30 +49,30 @@
         "run",
         "--host",
         BIND_INTERFACE,
         "--port",
         Env.get("FLASK_PORT", "8080"),
         "--reload",
         "--no-debugger",
-        "--eager-loading",
         "--with-threads",
     ]
 
     # Call to untyped function "FlaskGroup" in typed context
-    fg_cli = FlaskGroup()  # type: ignore
+    fg_cli = FlaskGroup()
     # Call to untyped function "main" in typed context
-    fg_cli.main(prog_name="restapi", args=args)  # type: ignore
+    fg_cli.main(prog_name="restapi", args=args)
     log.warning("Server shutdown")
 
 
 @cli.command()
 @click.option("--service", "-s")
 def verify(service: str) -> None:
     """Verify if a service is connected"""
 
+    mem.boot_completed = False
     if not Connector.check_availability(service):
         print_and_exit("Service {} not detected", service)
 
     log.info("Verifying service: {}", service)
     variables = Connector.services.get(service, {})
     host, port = get_service_address(variables, "host", "port", service)
     if host != "nohost":
@@ -125,17 +126,16 @@
 @cli.command()
 def wait() -> None:
     """Wait critical service(s) startup"""
     mywait()
 
 
 def get_service_address(
-    variables: Dict[str, str], host_var: str, port_var: str, service: str
-) -> Tuple[str, int]:
-
+    variables: dict[str, str], host_var: str, port_var: str, service: str
+) -> tuple[str, int]:
     host = variables.get(host_var)
     if host is None:
         print_and_exit("Cannot find any variable matching {} for {}", host_var, service)
 
     port = variables.get(port_var)
     if port is None:
         print_and_exit("Cannot find any variable matching {} for {}", port_var, service)
@@ -147,21 +147,19 @@
 
 def mywait() -> None:
     """
     Wait for a service on his host:port configuration
     This check is merely based on a socket connection
     """
     for name, variables in Connector.services.items():
-
         if name == "smtp" or name == "ftp":
             log.info("Service {} is enabled but not tested at startup time", name)
             continue
 
         if name == "celery":
-
             broker = variables.get("broker_service", "N/A")
 
             if broker == "RABBIT":
                 service_vars = Env.load_variables_group(prefix="rabbitmq")
             elif broker == "REDIS":
                 service_vars = Env.load_variables_group(prefix="redis")
             else:
@@ -200,28 +198,28 @@
 def clean() -> None:  # pragma: no cover
     """Destroy current services data"""
 
     from restapi.server import ServerModes, create_app
 
     log.info("Launching destruction app")
 
-    create_app(name="Removing data", mode=ServerModes.DESTROY)
+    create_app(name="Removing data", mode=ServerModes.DESTROY, options={})
 
     log.info("Destruction completed")
 
 
 @cli.command()
 def forced_clean() -> None:  # pragma: no cover
     """DANGEROUS: Destroy current data without asking yes/no"""
 
     from restapi.server import ServerModes, create_app
 
     log.info("Launching destruction app")
 
-    create_app(name="Removing data", mode=ServerModes.DESTROY)
+    create_app(name="Removing data", mode=ServerModes.DESTROY, options={})
 
     log.info("Destruction completed")
 
 
 @cli.command()
 @click.option("--wait/--no-wait", default=False, help="Wait for startup to finish")
 @click.option(
@@ -264,38 +262,35 @@
     if core:
         parameters.append(current_package)
     else:
         parameters.append(CUSTOM_PACKAGE)
 
     test_folder = Path("tests")
     if file is not None:
-
         filepath = Path(file)
         if test_folder not in filepath.parents:
             filepath = test_folder.joinpath(filepath)
 
         if not filepath.is_file():
             print_and_exit("File not found: {}", file)
         parameters.append(str(filepath.relative_to(test_folder)))
     elif folder is not None:
-
         folderpath = Path(folder)
         if test_folder not in folderpath.parents:
             folderpath = test_folder.joinpath(folderpath)
 
         if not folderpath.is_dir():
             print_and_exit("Folder not found: {}", folder)
         parameters.append(str(folderpath.relative_to(test_folder)))
 
     # In prod mode tests are execute with the server running.
     # Destroy test fails with alchemy due to db locks
     if destroy and not PRODUCTION:
         os.environ["TEST_DESTROY_MODE"] = "1"
     try:
-
         log.info("Running tests... this may take some time")
         log.debug("Executing: {}", parameters)
         from plumbum import local
 
         command = local["bash"]
         command(parameters, stdout=sys.stdout, stderr=sys.stderr)
         sys.exit(0)
@@ -306,12 +301,12 @@
 
 @cli.command()
 def clearcache() -> None:
     """Clear all data from the endpoints cache"""
     from restapi.server import create_app
     from restapi.services.cache import Cache
 
-    create_app(name="Cache clearing")
+    create_app(name="Cache clearing", mode=ServerModes.NORMAL, options={})
 
     Cache.clear()
 
     log.info("Cache cleared")
```

### Comparing `rapydo_http-2.4/restapi/config.py` & `rapydo_http-3.0/restapi/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Configuration variables set for the server instance
 """
+
 from functools import lru_cache
 from pathlib import Path
 
 from glom import glom
 
 from restapi.env import Env
 from restapi.utilities.globals import mem
@@ -28,15 +29,14 @@
 FLOWER_HOSTNAME = "flower"
 CELERYBEAT_HOSTNAME = "celery-beat"
 CELERY_HOSTNAME = "celery"
 DOCS = "docs-generation"
 
 
 def get_host_type(HOSTNAME: str) -> str:
-
     if HOSTNAME == DOCS:
         return DOCS
 
     if HOSTNAME == BACKEND_HOSTNAME:
         return BACKEND_HOSTNAME
 
     if HOSTNAME == FLOWER_HOSTNAME:
@@ -85,15 +85,14 @@
 @lru_cache
 def get_project_configuration(key: str, default: str) -> str:
     return glom(mem.configuration, key, default=default)
 
 
 @lru_cache
 def get_backend_url() -> str:
-
     BACKEND_URL = Env.get("BACKEND_URL", "")
 
     if BACKEND_URL:
         return BACKEND_URL
 
     BACKEND_PREFIX = Env.get("BACKEND_PREFIX", "").strip("/")
     if BACKEND_PREFIX:
@@ -104,15 +103,14 @@
 
     port = Env.get("FLASK_PORT", "8080")
     return f"http://{DOMAIN}{BACKEND_PREFIX}:{port}"
 
 
 @lru_cache
 def get_frontend_url() -> str:
-
     FRONTEND_URL = Env.get("FRONTEND_URL", "")
 
     if FRONTEND_URL:
         return FRONTEND_URL
 
     FRONTEND_PREFIX = Env.get("FRONTEND_PREFIX", "").strip("/")
     if FRONTEND_PREFIX:
```

### Comparing `rapydo_http-2.4/restapi/connectors/__init__.py` & `rapydo_http-3.0/restapi/connectors/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Set of modules for the connection and handling of external services
 """
+
 import abc
 import os
+import time
 from datetime import datetime, timedelta
 from pathlib import Path
 from types import ModuleType, TracebackType
-from typing import Any, Dict, Generic, List, Optional, Tuple, Type, TypeVar
+from typing import Any, Optional, TypeVar, cast
 
-# mypy: ignore-errors
 from flask import Flask
-from flask import _app_ctx_stack as stack
 
 from restapi.config import (
     ABS_RESTAPI_PATH,
     BACKEND_PACKAGE,
     CUSTOM_PACKAGE,
     EXTENDED_PACKAGE,
     EXTENDED_PROJECT_DISABLED,
@@ -30,45 +30,42 @@
 from restapi.utilities.meta import Meta
 
 # https://mypy.readthedocs.io/en/latest/generics.html#generic-methods-and-generic-self
 T = TypeVar("T", bound="Connector")
 
 CONNECTORS_FOLDER = "connectors"
 NO_AUTH = "NO_AUTHENTICATION"
+DEFAULT_DATETIME = datetime.fromtimestamp(0)
 
-# thread-id.ConnectorName.params-unique-key = instance
-InstancesCache = Dict[int, Dict[str, Dict[str, T]]]
 # service-name => dict of variables
-Services = Dict[str, Dict[str, str]]
+Services = dict[str, dict[str, str]]
 
-ExceptionsList = Optional[Tuple[Type[Exception]]]
+ExceptionsList = Optional[tuple[type[Exception]]]
 
 
 class Connector(metaclass=abc.ABCMeta):
-
     authentication_service: str = Env.get("AUTH_SERVICE", NO_AUTH)
     # Available services with associated env variables
     services: Services = {}
 
     # Assigned by init_app
-    app: Flask = None
+    app: Optional[Flask] = None
 
     # Used by get_authentication_module
     _authentication_module: Optional[ModuleType] = None
 
     # Returned by __getattr__ in neo4j and sqlalchemy connectors
-    _models: Dict[str, Type] = {}
+    _models: dict[str, type[Any]] = {}
 
     # Used by set_object and get_object
-    _instances: InstancesCache = {}
+    _instances: dict[str, T] = {}  # type: ignore
 
     def __init__(self) -> None:
-
         # This is the lower-cased class name (neomodel, celeryext)
-        self.name = self.__class__.__name__.lower()
+        # self.name = self.__class__.__name__.lower()
         # This is the folder name corresponding to the connector name (neo4j, celery, )
         # self.__class__.__module__ == restapi.connectors.sqlalchemy
         # .split(".") == ['restapi', 'connectors', 'sqlalchemy']
         # [-1] == 'sqlalchemy'
         self.name = self.__class__.__module__.split(".")[-1]
 
         # Will be modified by self.disconnect()
@@ -78,17 +75,20 @@
         if self.app is None:  # pragma: no cover
             # This should never happen because app is
             # assigned during init_services
             from flask import current_app
 
             self.app = current_app
 
+        self.connection_verification_time: Optional[datetime] = None
+        self.connection_expiration_time: Optional[datetime] = None
+        self.connection_time: datetime = DEFAULT_DATETIME
+
     @staticmethod
     def init() -> None:
-
         if Connector.authentication_service == NO_AUTH:
             log.info("No Authentication service configured")
         else:
             log.debug("Authentication service: {}", Connector.authentication_service)
 
         Connector.services = Connector.load_connectors(
             ABS_RESTAPI_PATH, BACKEND_PACKAGE, Connector.services
@@ -101,66 +101,62 @@
                 Connector.services,
             )
 
         Connector.services = Connector.load_connectors(
             Path(CUSTOM_PACKAGE), CUSTOM_PACKAGE, Connector.services
         )
 
-        Connector.load_models(Connector.services.keys())
-
     def __del__(self) -> None:
         if not self.disconnected:
             self.disconnect()
 
     def __enter__(self: T) -> T:
         return self
 
     def __exit__(
         self,
-        exctype: Optional[Type[Exception]],
+        exctype: Optional[type[Exception]],
         excinst: Optional[Exception],
         exctb: Optional[TracebackType],
     ) -> bool:
-
         if not self.disconnected:
             self.disconnect()
-        if excinst:
+        if excinst:  # pragma: no cover
             raise excinst
         return True
 
     @staticmethod
     @abc.abstractmethod
     def get_connection_exception() -> ExceptionsList:  # pragma: no cover
         return None
 
     @abc.abstractmethod
-    def connect(self: T, **kwargs: Any) -> Generic[T]:  # pragma: no cover
+    def connect(self: T, **kwargs: Any) -> T:  # pragma: no cover
         return self
 
     @abc.abstractmethod
     def disconnect(self) -> None:  # pragma: no cover
         return
 
     @abc.abstractmethod
-    def is_connected(instance: T) -> bool:  # pragma: no cover
+    def is_connected(self) -> bool:  # pragma: no cover
         return True
 
     def destroy(self) -> None:  # pragma: no cover
         print_and_exit("Missing destroy method in {}", self.__class__.__name__)
 
     def initialize(self) -> None:  # pragma: no cover
         print_and_exit("Missing initialize method in {}", self.__class__.__name__)
 
     @property
-    def variables(self) -> Dict[str, str]:
+    def variables(self) -> dict[str, str]:
         return self.services.get(self.name) or {}
 
     @classmethod
     def load_connectors(cls, path: Path, module: str, services: Services) -> Services:
-
         main_folder = path.joinpath(CONNECTORS_FOLDER)
         if not main_folder.is_dir():
             log.debug("Connectors folder not found: {}", main_folder)
             return services
 
         for connector in main_folder.iterdir():
             if not connector.is_dir():
@@ -198,113 +194,76 @@
 
             if not available:
                 continue
 
             connector_module = Connector.get_module(connector_name, module)
             connector_class = Connector.get_class(connector_module)
 
-            # Can't test connector misconfiguration...
+            # Can't test connector misconfigurations...
+            if not connector_module:  # pragma: no cover
+                log.error("No connector module found in {}", connector)
+                continue
             if not connector_class:  # pragma: no cover
                 log.error("No connector class found in {}", connector)
                 continue
 
             try:
                 # This is to test the Connector compliance,
                 # i.e. to verify instance and get_instance in the connector module
                 # and verify that the Connector can be instanced
                 connector_module.instance
                 connector_module.get_instance
                 connector_class()
             except AttributeError as e:  # pragma: no cover
-                print_and_exit(e)
+                print_and_exit(str(e))
 
             services[connector_name] = variables
 
             log.debug("Got class definition for {}", connector_class)
 
         return services
 
-    def load_models(connectors: List[str]) -> None:
-
-        for connector in connectors:
-            # Models are strictly core-dependent. If you need to enable models starting
-            # from a custom connector this function has to be refactored:
-            # 1) now is checked the existence of models.py in ABS_RESTAPI_PATH/connector
-            # 2) Core model is mandatory
-            # 3) Connector class, used to inject models is taken from BACKEND_PACKAGE
-
-            models_path = ABS_RESTAPI_PATH.joinpath(
-                CONNECTORS_FOLDER, connector, "models.py"
-            )
-
-            if not models_path.is_file():
-                log.debug("No model found for {}", connector)
-                continue
-
-            log.debug("Loading models from {}", connector)
-            base_models = Meta.import_models(connector, BACKEND_PACKAGE, mandatory=True)
-            if EXTENDED_PACKAGE == EXTENDED_PROJECT_DISABLED:
-                extended_models = {}
-            else:
-                extended_models = Meta.import_models(connector, EXTENDED_PACKAGE)
-            custom_models = Meta.import_models(connector, CUSTOM_PACKAGE)
-
-            log.debug(
-                "Models loaded from {}: core {}, extended {}, custom {}",
-                connector,
-                len(base_models),
-                len(extended_models),
-                len(custom_models),
-            )
-            connector_module = Connector.get_module(connector, BACKEND_PACKAGE)
-            connector_class = Connector.get_class(connector_module)
-            if connector_class:
-                connector_class.set_models(base_models, extended_models, custom_models)
-            else:  # pragma: no cover
-                log.error("Connector class not found for {}", connector)
-
     @staticmethod
     def get_module(connector: str, module: str) -> Optional[ModuleType]:
         return Meta.get_module_from_string(
             ".".join((module, CONNECTORS_FOLDER, connector))
         )
 
     @staticmethod
-    def get_class(connector_module: Optional[ModuleType]) -> Optional[Type]:
-
+    def get_class(connector_module: Optional[ModuleType]) -> Optional[type[Any]]:
         if not connector_module:  # pragma: no cover
-            return False
+            return None
 
         classes = Meta.get_new_classes_from_module(connector_module)
         for connector_class in classes.values():
             if issubclass(connector_class, Connector):
                 return connector_class
 
         return None  # pragma: no cover
 
     @staticmethod
     def get_authentication_instance() -> BaseAuthentication:
-
         if Connector.authentication_service == NO_AUTH:
             return NoAuthentication()
 
         if not Connector._authentication_module:
             Connector._authentication_module = Connector.get_module(
                 Connector.authentication_service, BACKEND_PACKAGE
             )
 
         if not Connector._authentication_module:  # pragma: no cover
             log.critical("{} not available", Connector.authentication_service)
             raise ServiceUnavailable("Authentication service not available")
 
-        return Connector._authentication_module.Authentication()
+        return cast(
+            BaseAuthentication, Connector._authentication_module.Authentication()
+        )
 
     @staticmethod
     def init_app(app: Flask, worker_mode: bool = False) -> None:
-
         Connector.app = app
 
         if Connector.authentication_service == NO_AUTH:
             return
 
         if (
             Connector.authentication_service not in Connector.services
@@ -313,29 +272,32 @@
                 "Auth service '{}' is not available", Connector.authentication_service
             )
 
         authentication_instance = Connector.get_authentication_instance()
         authentication_instance.module_initialization()
 
     @staticmethod
-    def project_init(options: Optional[Dict[str, bool]] = None) -> None:
-
+    def project_init(options: dict[str, bool]) -> None:
         if Connector.authentication_service != NO_AUTH:
             authentication_instance = Connector.get_authentication_instance()
 
             connector_module = Connector.get_module(
                 Connector.authentication_service, BACKEND_PACKAGE
             )
+            if not connector_module:  # pragma: no cover
+                return None
+
             connector = connector_module.get_instance()
 
             log.debug("Initializing {}", Connector.authentication_service)
             connector.initialize()
 
-            if options is None:
-                options: Dict[str, bool] = {}
+            if not Connector.app:  # pragma: no cover
+                log.error("Connector.app found uninitilizated at runtime")
+                return None
 
             with Connector.app.app_context():
                 authentication_instance.init_auth_db(options)
                 log.info("Initialized authentication module")
 
             initializer = mem.initializer()
             if initializer:
@@ -348,36 +310,53 @@
                 initialize_testing_environment(authentication_instance)
                 # Custom test initialization
                 initializer.initialize_testing_environment()
 
     @staticmethod
     def project_clean() -> None:
         if Connector.authentication_service != NO_AUTH:
-
             connector_module = Connector.get_module(
                 Connector.authentication_service, BACKEND_PACKAGE
             )
+            if not connector_module:  # pragma: no cover
+                return None
+
             connector = connector_module.get_instance()
 
             log.debug("Destroying {}", Connector.authentication_service)
             connector.destroy()
 
+    def load_models(self) -> None:
+        base_models = Meta.import_models(self.name, BACKEND_PACKAGE, mandatory=True)
+        if EXTENDED_PACKAGE == EXTENDED_PROJECT_DISABLED:
+            extended_models = {}
+        else:
+            extended_models = Meta.import_models(self.name, EXTENDED_PACKAGE)
+        custom_models = Meta.import_models(self.name, CUSTOM_PACKAGE)
+
+        log.debug(
+            "Models loaded from {}: core {}, extended {}, custom {}",
+            self.name,
+            len(base_models),
+            len(extended_models),
+            len(custom_models),
+        )
+        self.set_models(base_models, extended_models, custom_models)
+
     @classmethod
     def set_models(
         cls,
-        base_models: Dict[str, Type],
-        extended_models: Dict[str, Type],
-        custom_models: Dict[str, Type],
+        base_models: dict[str, type[Any]],
+        extended_models: dict[str, type[Any]],
+        custom_models: dict[str, type[Any]],
     ) -> None:
-
         # Join models as described by issue #16
         cls._models = base_models
         for m in [extended_models, custom_models]:
             for key, model in m.items():
-
                 # Verify if overriding => replace
                 if key in base_models.keys():
                     if issubclass(model, base_models[key]):  # pragma: no cover
                         log.debug("Overriding model {}", key)
                         cls._models[key] = model
                         continue
 
@@ -388,68 +367,61 @@
             log.debug("Models loaded")
 
     @staticmethod
     def is_external(host: str) -> bool:
         return not host.endswith(".dockerized.io")
 
     @classmethod
-    def set_object(cls, name: str, obj: T, key: str = "[]") -> None:
-        """set object into internal array"""
-
+    def get_instance_cache_key(cls, name: str, key: str) -> str:
         tid = os.getpid()
-        cls._instances.setdefault(tid, {})
-        cls._instances[tid].setdefault(name, {})
-        cls._instances[tid][name][key] = obj
+        return f"{tid}:{name}:{key}"
 
     @classmethod
-    def get_object(cls, name: str, key: str = "[]") -> Optional[T]:
-        """recover object if any"""
+    def set_object(cls, name: str, key: str, obj: T) -> None:
+        """set object into internal array"""
+        cache_key = cls.get_instance_cache_key(name, key)
+        cls._instances[cache_key] = obj
 
-        tid = os.getpid()
-        cls._instances.setdefault(tid, {})
-        cls._instances[tid].setdefault(name, {})
-        return cls._instances[tid][name].get(key, None)
+    @classmethod
+    def get_object(cls, name: str, key: str) -> Optional["Connector"]:
+        """recover object if any"""
+        cache_key = cls.get_instance_cache_key(name, key)
+        return cast(Optional["Connector"], cls._instances.get(cache_key))
 
     # From server.teardown... not executed during tests
     @classmethod
     def disconnect_all(cls) -> None:  # pragma: no cover
-        for connectors in cls._instances.values():
-            for instances in connectors.values():
-                for instance in instances.values():
-                    if not instance.disconnected:
-                        log.info(
-                            "Disconnecting {} {}", instance.name, hex(id(instance))
-                        )
-                        instance.disconnect()
+        for instance in cls._instances.values():
+            if not instance.disconnected:  # type: ignore
+                log.info(
+                    "Disconnecting {} {}",
+                    instance.name,  # type: ignore
+                    hex(id(instance)),
+                )
+                instance.disconnect()  # type: ignore
 
         cls._instances.clear()
 
         log.info("[{}] All connectors disconnected", os.getpid())
 
     def initialize_connection(
-        self, expiration: int, verification: int, **kwargs: str
+        self: T, expiration: int, verification: int, **kwargs: str
     ) -> T:
-
         # Create a new instance of itself
         obj = self.__class__()
 
         exceptions = obj.get_connection_exception()
         if exceptions is None:
             exceptions = (Exception,)
 
         try:
             obj = obj.connect(**kwargs)
         except exceptions as e:
             log.error("{} raised {}: {}", obj.name, e.__class__.__name__, e)
-            raise ServiceUnavailable(
-                {
-                    "Service Unavailable": "This service is temporarily unavailable, "
-                    "please retry in a few minutes"
-                }
-            )
+            raise ServiceUnavailable(f"Service {self.name} is not available") from e
 
         obj.connection_time = datetime.now()
 
         obj.connection_verification_time = None
         if verification > 0:
             ver = obj.connection_time + timedelta(seconds=verification)
             obj.connection_verification_time = ver
@@ -468,73 +440,87 @@
 
         return name in Connector.services
 
     def get_instance(
         self: T,
         verification: Optional[int] = None,
         expiration: Optional[int] = None,
+        retries: int = 1,
+        retry_wait: int = 0,
         **kwargs: str,
     ) -> T:
+        if retries < 1:
+            raise ServiceUnavailable(f"Invalid retry value: {retries}")
+
+        if retry_wait < 0:
+            raise ServiceUnavailable(f"Invalid retry wait value: {retry_wait}")
 
         if not Connector.check_availability(self.name):
             raise ServiceUnavailable(f"Service {self.name} is not available")
 
         if verification is None:
             # this should be the default value for this connector
             verification = Env.to_int(self.variables.get("verification_time"))
 
         if expiration is None:
             # this should be the default value for this connector
             expiration = Env.to_int(self.variables.get("expiration_time"))
 
-        # When context is empty this is a connection at loading time
-        # Do not save it
-        if stack.top is None:
+        # This is a connection at loading time, do not save it
+        if not mem.boot_completed:
             log.debug("First connection for {}", self.name)
             # can raise ServiceUnavailable exception
-            obj = self.initialize_connection(expiration, verification, **kwargs)
-            return obj
+            return self.initialize_connection(expiration, verification, **kwargs)
 
         unique_hash = str(sorted(kwargs.items()))
 
-        obj = self.get_object(name=self.name, key=unique_hash)
+        cached_obj = self.get_object(name=self.name, key=unique_hash)
 
         # if an expiration time is set, verify the instance age
-        if obj and obj.connection_expiration_time:
-
+        if cached_obj and cached_obj.connection_expiration_time:
             # the instance is invalidated if older than the expiration time
-            if datetime.now() >= obj.connection_expiration_time:
-
+            if datetime.now() >= cached_obj.connection_expiration_time:
                 log.info("{} connection is expired", self.name)
-                obj.disconnect()
-                obj = None
+                cached_obj.disconnect()
+                cached_obj = None
 
         # If a verification time is set, verify the instance age
-        if obj and obj.connection_verification_time:
+        if cached_obj and cached_obj.connection_verification_time:
             now = datetime.now()
 
             # the instance is verified if older than the verification time
-            if now >= obj.connection_verification_time:
+            if now >= cached_obj.connection_verification_time:
                 # if the connection is still valid, set a new verification time
-                if obj.is_connected():
+                if cached_obj.is_connected():
                     # Set the new verification time
                     ver = timedelta(seconds=verification)
-                    obj.connection_verification_time = now + ver
+                    cached_obj.connection_verification_time = now + ver
                 # if the connection is no longer valid, invalidate the instance
                 else:  # pragma: no cover
                     log.info(
                         "{} is no longer connected, connector invalidated", self.name
                     )
-                    obj.disconnected = True
+                    cached_obj.disconnected = True
 
         # return the instance only if still connected
         # (and not invalidated by the verification check)
-        if obj and not obj.disconnected:
-            return obj
+        if cached_obj and not cached_obj.disconnected:
+            return cast(T, cached_obj)
 
         # can raise ServiceUnavailable exception
-        obj = self.initialize_connection(expiration, verification, **kwargs)
-        self.set_object(name=self.name, obj=obj, key=unique_hash)
-        return obj
+        for retry in range(retries):
+            try:
+                instance = self.initialize_connection(
+                    expiration, verification, **kwargs
+                )
+                break
+            except ServiceUnavailable as e:
+                # This is the last iteration:
+                if retry == retries - 1:
+                    raise e
+                time.sleep(retry_wait)
+
+        self.set_object(name=self.name, key=unique_hash, obj=instance)
+        return instance
 
 
 Connector.init()
```

### Comparing `rapydo_http-2.4/restapi/connectors/celery/__init__.py` & `rapydo_http-3.0/restapi/connectors/celery/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,15 @@
 Celery connector with automatic integration in rapydo framework
 """
 
 import ssl
 import traceback
 from datetime import timedelta
 from functools import wraps
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    List,
-    NoReturn,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-    cast,
-)
+from typing import Any, Callable, NoReturn, Optional, TypeVar, Union, cast
 
 import certifi
 from celery import Celery, states
 from celery.app.task import Task
 from celery.exceptions import Ignore
 
 from restapi.config import CUSTOM_PACKAGE, DOCS, HOST_TYPE, SSL_CERTIFICATE, TESTING
@@ -91,15 +79,14 @@
         traceback=traceback.format_exc(),
     )
 
     raise Ignore(str(exception))
 
 
 def mark_task_as_failed_ignore(self: Any, name: str, exception: Exception) -> NoReturn:
-
     if TESTING:
         self.request.id = "fixed-id"
         self.request.task = name
 
     task_id = self.request.id
     task_name = self.request.task
     log.warning("Celery task {} ({}) failed: {}", task_id, task_name, exception)
@@ -134,15 +121,16 @@
     task_id = self.request.id
     task_name = self.request.task
     arguments = str(self.request.args)
     retry_num = 1 + self.request.retries
 
     # All retries attempts failed,
     # the error will be converted to permanent
-    if retry_num > MAX_RETRIES:
+    # TODO: it is not tested
+    if retry_num > MAX_RETRIES:  # pragma: no cover
         log.critical("MAX retries reached")
         mark_task_as_failed(self=self, name=name, exception=exception)
 
     # Removing username and password from urls in error stack
     clean_error_stack = ""
     for line in traceback.format_exc().split("\n"):
         clean_error_stack += f"{obfuscate_url(line)}\n"
@@ -179,15 +167,15 @@
     # Use with
     # @CeleryExt.task() [to automatically use function name]
     # or: CeleryExt.task(name="your_custom_name")
     @staticmethod
     def task(
         idempotent: bool,
         name: Optional[str] = None,
-        autoretry_for: Tuple[Type[Exception], ...] = tuple(),
+        autoretry_for: tuple[type[Exception], ...] = tuple(),
     ) -> Callable[[F], F]:
         """
         Wrapper of the celery task decorator for a smooth integration in RAPyDo.
 
         :param idempotent: A flag to specify if the task is idempotent or not.
             If idempotent (i.e. will not cause unintended effects even if called
             multiple times with the same arguments),
@@ -225,76 +213,71 @@
                 # This means the task may be executed multiple times if the worker
                 # crashes in the middle of execution.
                 # Make sure your tasks are idempotent
                 acks_late=idempotent,
             )
             @wraps(func)
             def wrapper(self: Any, *args: Any, **kwargs: Any) -> Any:
-
                 try:
-                    with CeleryExt.app.app_context():
+                    # app is officially Optional[Flask]... but can never be None at runtime
+                    with CeleryExt.app.app_context():  # type: ignore
                         return func(self, *args, **kwargs)
                 except Ignore as ex:
-
                     mark_task_as_failed_ignore(
                         self=self, name=name or func.__name__, exception=ex
                     )
 
                 except autoretry_for as ex:
-
                     mark_task_as_retriable(
                         self=self,
                         name=name or func.__name__,
                         exception=ex,
                         MAX_RETRIES=MAX_RETRIES,
                     )
                 except Exception as ex:
-
                     mark_task_as_failed(
                         self=self, name=name or func.__name__, exception=ex
                     )
 
             return cast(F, wrapper)
 
         return decorator
 
     @staticmethod
     def get_connection_exception() -> ExceptionsList:
         return None
 
     @staticmethod
-    def get_rabbit_url(variables: Dict[str, str], protocol: str) -> str:
+    def get_rabbit_url(variables: dict[str, str], protocol: str) -> str:
         host = variables.get("host")
         port = Env.to_int(variables.get("port"))
         vhost = variables.get("vhost", "")
         vhost = f"/{vhost}"
 
         user = variables.get("user", "")
         pwd = variables.get("password", "")
         creds = ""
         if user and pwd:
             creds = f"{user}:{pwd}@"
 
         return f"{protocol}://{creds}{host}:{port}{vhost}"
 
     @staticmethod
-    def get_redis_url(variables: Dict[str, str], protocol: str, db: int) -> str:
+    def get_redis_url(variables: dict[str, str], protocol: str, db: int) -> str:
         host = variables.get("host")
         port = Env.to_int(variables.get("port"))
         pwd = variables.get("password", "")
         creds = ""
         if pwd:
             creds = f":{pwd}@"
 
         return f"{protocol}://{creds}{host}:{port}/{db}"
 
     def connect(self, **kwargs: str) -> "CeleryExt":
-
-        variables = self.variables.copy()
-        variables.update(kwargs)
+        variables = self.variables | kwargs
         broker = variables.get("broker_service")
 
         if HOST_TYPE == DOCS:  # pragma: no cover
             broker = "RABBIT"
 
         if broker is None:  # pragma: no cover
             print_and_exit("Unable to start Celery, missing broker service")
@@ -444,20 +427,22 @@
         # tasks with late acknowledgement enabled.
         # These tasks cannot be acknowledged as the connection is gone,
         # and the tasks are automatically redelivered back to the queue.
         # In Celery 5.1 it is set to False by default.
         # The setting will be set to True by default in Celery 6.0.
         self.celery_app.conf.worker_cancel_long_running_tasks_on_connection_loss = True
 
-        if Env.get_bool("CELERYBEAT_ENABLED"):
+        # Automatically try to establish the connection to the AMQP broker on Celery startup
+        # if it is unavailable.
+        self.celery_app.conf.broker_connection_retry_on_startup = True
 
+        if Env.get_bool("CELERYBEAT_ENABLED"):
             CeleryExt.CELERYBEAT_SCHEDULER = backend
 
             if backend == "REDIS":
-
                 service_vars = Env.load_variables_group(prefix="redis")
                 url = self.get_redis_url(
                     service_vars, protocol="redis", db=RedisExt.CELERY_BEAT_DB
                 )
 
                 self.celery_app.conf["REDBEAT_REDIS_URL"] = url
                 self.celery_app.conf["REDBEAT_KEY_PREFIX"] = REDBEAT_KEY_PREFIX
@@ -484,21 +469,19 @@
 
         return self
 
     def disconnect(self) -> None:
         self.disconnected = True
 
     def is_connected(self) -> bool:
-
         log.warning("celery.is_connected method is not implemented")
         return not self.disconnected
 
     @classmethod
     def get_periodic_task(cls, name: str) -> Any:
-
         if cls.CELERYBEAT_SCHEDULER == "REDIS":
             from redbeat.schedulers import RedBeatSchedulerEntry
 
             try:
                 task_key = f"{REDBEAT_KEY_PREFIX}{name}"
                 return RedBeatSchedulerEntry.from_key(
                     task_key, app=CeleryExt.celery_app
@@ -521,16 +504,16 @@
     @classmethod
     def create_periodic_task(
         cls,
         name: str,
         task: str,
         every: Union[str, int, timedelta],
         period: AllowedTimedeltaPeriods = "seconds",
-        args: Optional[List[Any]] = None,
-        kwargs: Optional[Dict[str, Any]] = None,
+        args: Optional[list[Any]] = None,
+        kwargs: Optional[dict[str, Any]] = None,
     ) -> None:
         if args is None:
             args = []
         if kwargs is None:
             kwargs = {}
 
         if cls.CELERYBEAT_SCHEDULER == "REDIS":
@@ -565,18 +548,17 @@
         name: str,
         task: str,
         minute: str,
         hour: str,
         day_of_week: str = "*",
         day_of_month: str = "*",
         month_of_year: str = "*",
-        args: Optional[List[Any]] = None,
-        kwargs: Optional[Dict[str, Any]] = None,
+        args: Optional[list[Any]] = None,
+        kwargs: Optional[dict[str, Any]] = None,
     ) -> None:
-
         if args is None:
             args = []
         if kwargs is None:
             kwargs = {}
 
         if cls.CELERYBEAT_SCHEDULER == "REDIS":
             from celery.schedules import crontab
@@ -603,13 +585,18 @@
 
 instance = CeleryExt()
 
 
 def get_instance(
     verification: Optional[int] = None,
     expiration: Optional[int] = None,
+    retries: int = 1,
+    retry_wait: int = 0,
     **kwargs: str,
 ) -> "CeleryExt":
-
     return instance.get_instance(
-        verification=verification, expiration=expiration, **kwargs
+        verification=verification,
+        expiration=expiration,
+        retries=retries,
+        retry_wait=retry_wait,
+        **kwargs,
     )
```

### Comparing `rapydo_http-2.4/restapi/connectors/celery/beat.py` & `rapydo_http-3.0/restapi/connectors/celery/beat.py`

 * *Files identical despite different names*

### Comparing `rapydo_http-2.4/restapi/connectors/celery/worker.py` & `rapydo_http-3.0/restapi/connectors/celery/worker.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,10 +5,12 @@
 
 instance = celery.get_instance()
 # Used by Celery to run the instance (--app app)
 celery_app = instance.celery_app
 
 if HOST_TYPE != DOCS:
     # Reload Flask app code for the worker (needed to have the app context available)
-    celery.CeleryExt.app = create_app(mode=ServerModes.WORKER)
+    celery.CeleryExt.app = create_app(
+        name="Celery Worker", mode=ServerModes.WORKER, options={}
+    )
 
     log.debug("Celery worker is ready {}", celery_app)
```

### Comparing `rapydo_http-2.4/restapi/connectors/ftp/__init__.py` & `rapydo_http-3.0/restapi/connectors/ftp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,18 +53,15 @@
     # i.e. begin with a digit in the range 1–5.
 
     @staticmethod
     def get_connection_exception() -> ExceptionsList:
         return (socket.gaierror,)
 
     def connect(self, **kwargs: str) -> "FTPExt":
-
-        variables = self.variables.copy()
-
-        variables.update(kwargs)
+        variables = self.variables | kwargs
 
         if (host := variables.get("host")) is None:  # pragma: no cover
             raise ServiceUnavailable("Missing hostname")
 
         if (user := variables.get("user")) is None:  # pragma: no cover
             raise ServiceUnavailable("Missing credentials")
 
@@ -136,13 +133,18 @@
 
 instance = FTPExt()
 
 
 def get_instance(
     verification: Optional[int] = None,
     expiration: Optional[int] = None,
+    retries: int = 1,
+    retry_wait: int = 0,
     **kwargs: str,
 ) -> "FTPExt":
-
     return instance.get_instance(
-        verification=verification, expiration=expiration, **kwargs
+        verification=verification,
+        expiration=expiration,
+        retries=retries,
+        retry_wait=retry_wait,
+        **kwargs,
     )
```

### Comparing `rapydo_http-2.4/restapi/connectors/neo4j/__init__.py` & `rapydo_http-3.0/restapi/connectors/neo4j/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Neo4j connector with automatic integration in rapydo framework, based on neomodel
 """
 
 import re
 import socket
 from datetime import datetime, timedelta
 from functools import wraps
-from typing import Any, Callable, Dict, List, Optional, TypeVar, cast
+from typing import Any, Callable, Optional, TypeVar, cast
 
 import pytz
 from neo4j.exceptions import (
     AuthError,
     CypherSyntaxError,
     ServiceUnavailable,
     TransientError,
@@ -53,53 +53,50 @@
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 
 def catch_db_exceptions(func: F) -> F:
     @wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
-
         try:
             return func(*args, **kwargs)
         except DatabaseDuplicatedEntry as e:
             # already catched and parser, raise up
             raise (e)
         except DoesNotExist as e:
             raise (e)
         except CypherSyntaxError as e:
             raise (e)
         except UniqueProperty as e:
-
             t = "already exists with label"
             m = re.search(
                 rf"Node\([0-9]+\) {t} `(.+)` and property `(.+)` = '(.+)'", str(e)
             )
 
             if m:
                 node = m.group(1)
                 prop = m.group(2)
                 val = m.group(3)
                 error = f"A {node.title()} already exists with {prop}: {val}"
-                raise DatabaseDuplicatedEntry(error)
+                raise DatabaseDuplicatedEntry(error) from e
 
             # Can't be tested, should never happen except in case of new neo4j version
             log.error("Unrecognized error message: {}", e)  # pragma: no cover
-            raise DatabaseDuplicatedEntry("Duplicated entry")  # pragma: no cover
+            raise DatabaseDuplicatedEntry("Duplicated entry") from e  # pragma: no cover
         except RequiredProperty as e:
-
             # message = property 'xyz' on objects of class XYZ
 
             message = str(e)
             m = re.search(r"property '(.*)' on objects of class (.*)", str(e))
             if m:
                 missing_property = m.group(1)
                 model = m.group(2)
                 message = f"Missing property {missing_property} required by {model}"
 
-            raise DatabaseMissingRequiredProperty(message)
+            raise DatabaseMissingRequiredProperty(message) from e
         except DeflateError as e:
             log.warning(e)
             return None
 
         except ServiceUnavailable:  # pragma: no cover
             # refresh_connection()
             raise
@@ -112,41 +109,37 @@
             log.critical("Raised unknown exception: {}", type(e))
             raise e
 
     return cast(F, wrapper)
 
 
 class NeoModel(Connector):
-
     # This is used to return Models in a type-safe way
     # Return type becomes "Any" due to an unfollowed import
     def __getattr__(self, name: str) -> StructuredNode:  # type: ignore
         if name in self._models:
             return self._models[name]
         raise AttributeError(f"Model {name} not found")
 
     @staticmethod
     def get_connection_exception() -> ExceptionsList:
-
         return (
             neobolt_ServiceUnavailable,
             neobolt_AddressError,
             ServiceUnavailable,
             AuthError,
             socket.gaierror,
             # REALLY?? A ValueError!? :-(
             # Raised here:
             # https://github.com/neo4j/neo4j-python-driver/blob/d36334e80a66d57b32621d319032751d2204ef67/neo4j/addressing.py#L112
             ValueError,
         )  # type: ignore
 
     def connect(self, **kwargs: str) -> "NeoModel":
-
-        variables = self.variables.copy()
-        variables.update(kwargs)
+        variables = self.variables | kwargs
 
         USER = variables.get("user", "neo4j")
         PWD = variables.get("password")
         HOST = variables.get("host")
         PORT = variables.get("port")
         # Fixed... to be configured?
         DATABASE = "neo4j"
@@ -166,34 +159,33 @@
         db.set_connection(URI)
 
         db.driver.verify_connectivity()
 
         StructuredNode.save = catch_db_exceptions(StructuredNode.save)
         NodeSet.get = catch_db_exceptions(NodeSet.get)
 
+        self.load_models()
         self.db = db
         return self
 
     def disconnect(self) -> None:
         self.disconnected = True
 
     def is_connected(self) -> bool:
-
         if self.disconnected or not self.db or not self.db.driver:
             return False
 
         try:
             self.db.driver.verify_connectivity()
             return True
-        except (ServiceUnavailable, TransientError) as e:
+        except (ServiceUnavailable, TransientError) as e:  # pragma: no cover
             log.error(e)
             return False
 
     def initialize(self) -> None:
-
         if self.app:
             with self.app.app_context():
                 try:
                     remove_all_labels()
                 # With Neo4j 4.3 remove all labels on empty DB started to fail with:
                 # [...]
                 #   File "/usr/local/lib/python3.9/dist-packages/neomodel/core.py", ...
@@ -214,15 +206,14 @@
                 #     {message: An equivalent constraint already exists,
                 #         'Constraint( type='UNIQUENESS', schema=(:XYZ {uuid}), [...]
                 # This loop with install_labels prevent errors
                 for model in self._models.values():
                     install_labels(model, quiet=False)
 
     def destroy(self) -> None:
-
         graph = self.get_instance()
 
         if self.app:
             with self.app.app_context():
                 log.critical("Destroy current Neo4j data")
 
                 clear_neo4j_database(graph.db)
@@ -234,44 +225,42 @@
 
     #     log.info("Refreshing neo4j connection...")
     #     self.db.set_connection(self.db.url)
     #     return True
 
     @staticmethod
     # Argument 1 to "update_properties" becomes "Any" due to an unfollowed import
-    def update_properties(instance: StructuredNode, properties: Dict[str, Any]) -> None:  # type: ignore
-
+    def update_properties(instance: StructuredNode, properties: dict[str, Any]) -> None:  # type: ignore  # noqa
         for field, value in properties.items():
             instance.__dict__[field] = value
 
     @catch_db_exceptions
     def cypher(self, query: str, **parameters: str) -> Any:
         """Execute raw cypher queries"""
 
         try:
             # results, meta = db.cypher_query(query, parameters)
             results, _ = db.cypher_query(query, parameters)
         except CypherSyntaxError as e:
             log.warning(query)
             log.error(f"Failed to execute Cypher Query\n{e}")
-            raise CypherSyntaxError("Failed to execute Cypher Query")
+            raise CypherSyntaxError("Failed to execute Cypher Query") from e
         return results
 
     @staticmethod
     def sanitize_input(term: str) -> str:
         """
         Strip and clean up terms from special characters. To be used in fuzzy search
         """
         return term.strip().replace("*", "").replace("'", "\\'").replace("~", "")
 
     @staticmethod
     def fuzzy_tokenize(term: str) -> str:
         tokens = re.findall(r'[^"\s]\S*|".+?"', term)
         for index, t in enumerate(tokens):
-
             # Do not apply fuzzy search to quoted strings
             if '"' in t:
                 continue
 
             # Do not apply fuzzy search to special characters
             if t == "+" or t == "!":
                 continue
@@ -288,26 +277,25 @@
 class Authentication(BaseAuthentication):
     def __init__(self) -> None:
         self.db: NeoModel = get_instance()
 
     def get_user(
         self, username: Optional[str] = None, user_id: Optional[str] = None
     ) -> Optional[User]:
-
         if username:
             return self.db.User.nodes.get_or_none(email=username)
 
         if user_id:
             return self.db.User.nodes.get_or_none(uuid=user_id)
 
         # reached if both username and user_id are None
         return None
 
-    def get_users(self) -> List[User]:
-        return cast(List[User], self.db.User.nodes.all())
+    def get_users(self) -> list[User]:
+        return cast(list[User], self.db.User.nodes.all())
 
     def save_user(self, user: User) -> bool:
         if not user:
             return False
 
         user.save()
         return True
@@ -326,21 +314,21 @@
             return self.db.Group.nodes.get_or_none(uuid=group_id)
 
         if name:
             return self.db.Group.nodes.get_or_none(shortname=name)
 
         return None
 
-    def get_groups(self) -> List[Group]:
-        return cast(List[Group], self.db.Group.nodes.all())
+    def get_groups(self) -> list[Group]:
+        return cast(list[Group], self.db.Group.nodes.all())
 
     def get_user_group(self, user: User) -> Group:
         return user.belongs_to.single()
 
-    def get_group_members(self, group: Group) -> List[User]:
+    def get_group_members(self, group: Group) -> list[User]:
         return list(group.members)
 
     def save_group(self, group: Group) -> bool:
         if not group:
             return False
 
         group.save()
@@ -349,24 +337,23 @@
     def delete_group(self, group: Group) -> bool:
         if not group:
             return False
 
         group.delete()
         return True
 
-    def get_roles(self) -> List[RoleObj]:
+    def get_roles(self) -> list[RoleObj]:
         roles = []
         for role in self.db.Role.nodes.all():
             if role:
                 roles.append(role)
 
         return roles
 
-    def get_roles_from_user(self, user: Optional[User]) -> List[str]:
-
+    def get_roles_from_user(self, user: Optional[User]) -> list[str]:
         # No user for non authenticated endpoints -> return no role
         if user is None:
             return []
 
         return [role.name for role in user.roles.all()]
 
     def create_role(self, name: str, description: str) -> None:
@@ -376,68 +363,67 @@
     def save_role(self, role: RoleObj) -> bool:
         if role:
             role.save()
             return True
         return False
 
     # Also used by POST user
-    def create_user(self, userdata: Dict[str, Any], roles: List[str]) -> User:
-
+    def create_user(
+        self, userdata: dict[str, Any], roles: list[str], group: Group
+    ) -> User:
         userdata.setdefault("authmethod", "credentials")
 
         if "password" in userdata:
             userdata["password"] = self.get_password_hash(userdata["password"])
 
         userdata, extra_userdata = self.custom_user_properties_pre(userdata)
 
         user = self.db.User(**userdata)
         user.save()
 
+        self.add_user_to_group(user, group)
         self.link_roles(user, roles)
 
         self.custom_user_properties_post(user, userdata, extra_userdata, self.db)
 
         return user
 
     # Also used by PUT user
-    def link_roles(self, user: User, roles: List[str]) -> None:
-
+    def link_roles(self, user: User, roles: list[str]) -> None:
         if not roles:
             roles = [self.default_role]
 
         for p in user.roles.all():
             user.roles.disconnect(p)
 
         for role in roles:
             log.debug("Adding role {}", role)
             try:
                 role_obj = self.db.Role.nodes.get(name=role)
-            except self.db.Role.DoesNotExist:  # pragma: no cover
-                raise Exception(f"Graph role {role} does not exist")
+            except self.db.Role.DoesNotExist as e:  # pragma: no cover
+                raise Exception(f"Graph role {role} does not exist") from e
             user.roles.connect(role_obj)
 
-    def create_group(self, groupdata: Dict[str, Any]) -> Group:
+    def create_group(self, groupdata: dict[str, Any]) -> Group:
         group = self.db.Group(**groupdata).save()
 
         return group
 
     def add_user_to_group(self, user: User, group: Group) -> None:
-
         if user and group:
             prev_group = user.belongs_to.single()
 
             if prev_group is not None:
                 user.belongs_to.reconnect(prev_group, group)
             else:
                 user.belongs_to.connect(group)
 
     def save_token(
         self, user: User, token: str, payload: Payload, token_type: Optional[str] = None
     ) -> None:
-
         ip_address = self.get_remote_ip()
 
         if token_type is None:
             token_type = self.FULL_TOKEN
 
         now = datetime.now(pytz.utc)
         exp = payload.get("exp", now + timedelta(seconds=self.DEFAULT_TOKEN_TTL))
@@ -454,15 +440,14 @@
 
         token_node.save()
         # Save user updated in profile endpoint
         user.save()
         token_node.emitted_for.connect(user)
 
     def verify_token_validity(self, jti: str, user: User) -> bool:
-
         try:
             token_node = self.db.Token.nodes.get(jti=jti)
         except self.db.Token.DoesNotExist:
             return False
 
         if not token_node.emitted_for.is_connected(user):  # pragma: no cover
             return False
@@ -495,17 +480,16 @@
         return True
 
     def get_tokens(
         self,
         user: Optional[User] = None,
         token_jti: Optional[str] = None,
         get_all: bool = False,
-    ) -> List[Token]:
-
-        tokens_list: List[Token] = []
+    ) -> list[Token]:
+        tokens_list: list[Token] = []
         tokens = None
 
         if get_all:
             tokens = self.db.Token.nodes.all()
         elif user:
             tokens = user.tokens.all()
         elif token_jti:
@@ -540,15 +524,14 @@
             self.log_event(Events.delete, target=token_node)
         except self.db.Token.DoesNotExist:
             log.warning("Unable to invalidate, token not found: {}", token)
             return False
         return True
 
     def save_login(self, username: str, user: Optional[User], failed: bool) -> None:
-
         date = datetime.now(pytz.utc)
         ip_address = self.get_remote_ip()
 
         login = self.db.Login()
         login.date = date
         login.username = username
         login.IP = ip_address
@@ -560,37 +543,40 @@
 
         login.save()
         if user:
             login.user.connect(user)
 
     def get_logins(
         self, username: Optional[str] = None, only_unflushed: bool = False
-    ) -> List[Login]:
-
+    ) -> list[Login]:
         if not username:
             logins = self.db.Login.nodes.all()
         elif only_unflushed:
             logins = self.db.Login.nodes.filter(username=username, flushed=False)
         else:
             logins = self.db.Login.nodes.filter(username=username)
 
         return [x for x in logins]
 
     def flush_failed_logins(self, username: str) -> None:
-
         for login in self.db.Login.nodes.filter(username=username, flushed=False):
             login.flushed = True
             login.save()
 
 
 instance = NeoModel()
 
 
 def get_instance(
     verification: Optional[int] = None,
     expiration: Optional[int] = None,
+    retries: int = 1,
+    retry_wait: int = 0,
     **kwargs: str,
 ) -> "NeoModel":
-
     return instance.get_instance(
-        verification=verification, expiration=expiration, **kwargs
+        verification=verification,
+        expiration=expiration,
+        retries=retries,
+        retry_wait=retry_wait,
+        **kwargs,
     )
```

### Comparing `rapydo_http-2.4/restapi/connectors/neo4j/models.py` & `rapydo_http-3.0/restapi/connectors/neo4j/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-""" Models for graph database """
-from typing import Type
+""" Models for neo4j database """
 
 from neomodel import (
     AliasProperty,
     ArrayProperty,
     BooleanProperty,
     DateProperty,
     DateTimeProperty,
@@ -22,22 +21,35 @@
 )
 
 from restapi.config import TESTING
 from restapi.connectors.neo4j.types import IdentifiedNode, TimestampedNode
 from restapi.utilities.meta import Meta
 
 # mypy: ignore-errors
-UserCustomClass: Type[IdentifiedNode] = (
+UserCustomClass: type[IdentifiedNode] = (
     Meta.get_class("models.neo4j", "UserCustom") or IdentifiedNode
 )
 # mypy: ignore-errors
-GroupCustomClass: Type[IdentifiedNode] = (
+GroupCustomClass: type[IdentifiedNode] = (
     Meta.get_class("models.neo4j", "GroupCustom") or IdentifiedNode
 )
 
+GroupModelPath = "restapi.connectors.neo4j.models.Group"
+LoginModelPath = "restapi.connectors.neo4j.models.Login"
+RoleModelPath = "restapi.connectors.neo4j.models.Role"
+TokenModelPath = "restapi.connectors.neo4j.models.Token"
+UserModelPath = "restapi.connectors.neo4j.models.User"
+
+
+class Group(GroupCustomClass):
+    shortname = StringProperty(required=True, unique_index=True)
+    fullname = StringProperty(required=True, unique_index=False)
+
+    members = RelationshipFrom(UserModelPath, "BELONGS_TO", cardinality=ZeroOrMore)
+
 
 class User(UserCustomClass):
     email = EmailProperty(required=True, unique_index=True)
     name = StringProperty(required=True)
     surname = StringProperty(required=True)
     authmethod = StringProperty(required=True)
     password = StringProperty(required=True)
@@ -45,51 +57,44 @@
     first_login = DateTimeProperty()
     last_login = DateTimeProperty()
     last_password_change = DateTimeProperty()
     is_active = BooleanProperty(default=True)
     privacy_accepted = BooleanProperty(default=True)
     expiration = DateTimeProperty()
 
-    tokens = RelationshipTo("Token", "HAS_TOKEN", cardinality=ZeroOrMore)
-    roles = RelationshipTo("Role", "HAS_ROLE", cardinality=ZeroOrMore)
-    belongs_to = RelationshipTo("Group", "BELONGS_TO")
-    logins = RelationshipTo("Login", "HAS_LOGIN", cardinality=ZeroOrMore)
-
-
-class Group(GroupCustomClass):
-    shortname = StringProperty(required=True, unique_index=True)
-    fullname = StringProperty(required=True, unique_index=False)
-
-    members = RelationshipFrom("User", "BELONGS_TO", cardinality=ZeroOrMore)
+    tokens = RelationshipTo(TokenModelPath, "HAS_TOKEN", cardinality=ZeroOrMore)
+    roles = RelationshipTo(RoleModelPath, "HAS_ROLE", cardinality=ZeroOrMore)
+    belongs_to = RelationshipTo(GroupModelPath, "BELONGS_TO", cardinality=ZeroOrOne)
+    logins = RelationshipTo(LoginModelPath, "HAS_LOGIN", cardinality=ZeroOrMore)
 
 
 class Token(StructuredNode):
     jti = StringProperty(required=True, unique_index=True)
     token = StringProperty(required=True, unique_index=True)
     token_type = StringProperty(required=True)
     creation = DateTimeProperty(required=True)
     expiration = DateTimeProperty()
     last_access = DateTimeProperty()
     IP = StringProperty()
     location = StringProperty()
-    emitted_for = RelationshipFrom("User", "HAS_TOKEN", cardinality=ZeroOrOne)
+    emitted_for = RelationshipFrom(UserModelPath, "HAS_TOKEN", cardinality=ZeroOrOne)
 
 
 class Role(StructuredNode):
     name = StringProperty(required=True, unique_index=True)
     description = StringProperty(default="No description")
-    privileged = RelationshipFrom(User, "HAS_ROLE", cardinality=OneOrMore)
+    privileged = RelationshipFrom(UserModelPath, "HAS_ROLE", cardinality=OneOrMore)
 
 
 class Login(StructuredNode):
     date = DateTimeProperty(required=True)
     username = StringProperty()
     IP = StringProperty()
     location = StringProperty()
-    user = RelationshipFrom("User", "HAS_LOGIN", cardinality=ZeroOrOne)
+    user = RelationshipFrom(UserModelPath, "HAS_LOGIN", cardinality=ZeroOrOne)
     failed = BooleanProperty(default=False)
     flushed = BooleanProperty(default=False)
 
 
 if TESTING:
 
     class RelationTest(StructuredRel):
@@ -103,19 +108,19 @@
         p_float = FloatProperty()
         p_date = DateProperty()
         p_dt = DateTimeProperty()
         p_bool = BooleanProperty()
         p_alias = AliasProperty()
 
         test1 = RelationshipFrom(
-            "restapi.connectors.neo4j.models.User",
+            UserModelPath,
             "TEST",
             cardinality=ZeroOrMore,
             model=RelationTest,
         )
 
         test2 = RelationshipFrom(
-            "restapi.connectors.neo4j.models.User",
+            UserModelPath,
             "TEST2",
             cardinality=ZeroOrMore,
             model=RelationTest,
         )
```

### Comparing `rapydo_http-2.4/restapi/connectors/neo4j/parser.py` & `rapydo_http-3.0/restapi/connectors/neo4j/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import csv
-from typing import Any, Dict, List
+from typing import Any
 
 from restapi.config import IMPORT_PATH
 from restapi.connectors import neo4j
 from restapi.utilities.logs import log
 
 
 class DataDump:
-    def __init__(self, filename: str, fields: List[str]) -> None:
-
+    def __init__(self, filename: str, fields: list[str]) -> None:
         for f in fields:
             if ":" not in f:
                 raise ValueError(
                     f"Wrong field syntax, type is missing in {f}. Expected {f}:TYPE. "
                     "Supported types: string,int,float"
                 )
 
         # This will be used by the backend to write the file
         self.filepath = IMPORT_PATH.joinpath(filename)
         # This will be used by neo4j to read the file
         self.filename = filename
-        self.cache: Dict[str, bool] = {}
+        self.cache: dict[str, bool] = {}
         self.fields = fields
         self.counter = 0
 
         with open(self.filepath, "w+") as out_handle:
             tsv_node_writer = csv.writer(out_handle, delimiter="\t")
-            fields_without_types: List[str] = []
+            fields_without_types: list[str] = []
             for f in fields:
                 fields_without_types.append(f.split(":")[0])
             tsv_node_writer.writerow(fields_without_types)
 
         self.handle = open(self.filepath, "a+")
         self.writer = csv.writer(self.handle, delimiter="\t")
 
@@ -44,15 +43,14 @@
 
     def clean(self) -> None:
         self.flush_cache()
         self.close()
         self.filepath.unlink()
 
     def print_line(self, args: Any) -> None:
-
         for a in args:
             if a is None:
                 raise ValueError(f"Found NULL value in line: {args}")
 
         h = str(args)
         if h in self.cache:
             return
@@ -62,16 +60,16 @@
 
     @staticmethod
     def cypher_exec(cypher: str) -> Any:
         graph = neo4j.get_instance()
         return graph.cypher(cypher)
 
     @staticmethod
-    def get_properties(fields: List[str]) -> str:
-        properties: List[str] = []
+    def get_properties(fields: list[str]) -> str:
+        properties: list[str] = []
 
         for f in fields:
             tokens = f.split(":")
             if tokens[1] == "string":
                 properties.append(f"{tokens[0]}: line.{tokens[0]}")
             elif tokens[1] == "int":
                 properties.append(f"{tokens[0]}: toInteger(line.{tokens[0]})")
@@ -140,16 +138,15 @@
             self.handle.close()
 
     def __del__(self) -> None:
         self.close()
 
 
 class NodeDump(DataDump):
-    def __init__(self, label: str, fields: List[str]) -> None:
-
+    def __init__(self, label: str, fields: list[str]) -> None:
         filename = f"{label}.tsv".lower()
         super().__init__(filename, fields)
         self.label = label
 
     # def bulk_delete(self, limit: int = 10000) -> None:
     #     self.delete_nodes(self.label, limit=limit)
 
@@ -158,15 +155,14 @@
             raise ValueError(
                 f"Unexpected number of fields\nReceived {len(args)} ({args})\n"
                 f"Expected {len(self.fields)} ({self.fields})"
             )
         self.print_line(args)
 
     def store(self, chunk_size: int = 10000) -> None:
-
         self.close()
 
         log.info("Storing {} ({}) nodes", self.count, self.label)
 
         properties: str = self.get_properties(self.fields)
 
         cypher = f"""
@@ -180,27 +176,25 @@
 }} IN TRANSACTIONS OF {chunk_size} ROWS
 """
 
         self.cypher_exec(cypher)
 
 
 class RelationDump(DataDump):
-
     NODE1_LABEL = "node1"
     NODE2_LABEL = "node2"
 
     def __init__(
         self,
         label1: str,
         relation: str,
         label2: str,
-        fields: List[str],
+        fields: list[str],
         ignore_indexes: bool = False,
     ) -> None:
-
         filename = f"{label1}_{relation}_{label2}.tsv".lower()
         # This is to prevent duplicates in node keys
         self.key1 = fields[0]
         self.key2 = fields[1]
         fields[0] = f"{self.NODE1_LABEL}:string"
         fields[1] = f"{self.NODE2_LABEL}:string"
         super().__init__(filename, fields)
@@ -223,15 +217,14 @@
             raise ValueError(
                 f"Unexpected number of fields\nReceived {len(args)} ({args})\n"
                 f"Expected {len(self.fields)} ({self.fields})"
             )
         self.print_line(args)
 
     def store(self, chunk_size: int = 10000) -> None:
-
         self.close()
 
         log.info(
             "Storing {} ({})-[:{}]->({}) relationships",
             self.count,
             self.label1,
             self.relation,
```

### Comparing `rapydo_http-2.4/restapi/connectors/neo4j/types.py` & `rapydo_http-3.0/restapi/connectors/neo4j/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,30 +5,28 @@
 from neomodel import DateTimeProperty, StringProperty, StructuredNode
 
 from restapi.utilities.uuid import getUUID
 
 
 # Base type StructuredNode becomes "Any" due to an unfollowed import
 class IdentifiedNode(StructuredNode):  # type: ignore
-
     """
     A StructuredNode identified by an uuid
     """
 
     __abstract_node__ = True
 
     # UniqueIdProperty creates uuid in hex formata (without hyphes)
     # These are not compatible with marshmallow that serializes with UUID(value) so that
     # hex uuids are serialized with hyphes and this create divergences
     # uuid = UniqueIdProperty()
     uuid = StringProperty(default=getUUID, unique_index=True)
 
 
 class TimestampedNode(IdentifiedNode):
-
     """
     An IdentifiedNode with creation and modification dates
     """
 
     __abstract_node__ = True
 
     created = DateTimeProperty(default_now=True, show=True)
```

### Comparing `rapydo_http-2.4/restapi/connectors/rabbitmq/__init__.py` & `rapydo_http-3.0/restapi/connectors/rabbitmq/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 RabbitMQ connector with automatic integration in rapydo framework, based on pika
 """
 
 import socket
 import ssl
 import urllib.parse
-from typing import Any, Dict, List, Optional
+from typing import Any, Optional
 
 import certifi
 import orjson
 import pika
 import requests
 from pika.exceptions import (
     AMQPChannelError,
@@ -45,21 +45,18 @@
         return (
             AMQPConnectionError,
             # Includes failures in name resolution
             socket.gaierror,
         )  # type: ignore
 
     def connect(self, **kwargs: str) -> "RabbitExt":
-
-        variables = self.variables.copy()
         # Beware, if you specify a user different by the default,
-        # then the send method will fail to to PRECONDITION_FAILED because
-        # the user_id will not pass the verification
-        # Locally save self.variables + kwargs to be used in send()
-        variables.update(kwargs)
+        # then the send method will fail with PRECONDITION_FAILED
+        # because the user_id will not pass the verification
+        variables = self.variables | kwargs
 
         ssl_enabled = Env.to_bool(variables.get("ssl_enabled"))
 
         log.info("Connecting to the Rabbit (SSL = {})", ssl_enabled)
 
         if (host := variables.get("host")) is None:  # pragma: no cover
             raise ServiceUnavailable("Missing hostname")
@@ -70,15 +67,14 @@
         if (password := variables.get("password")) is None:  # pragma: no cover
             raise ServiceUnavailable("Missing credentials")
 
         port = int(variables.get("port", "0"))
         vhost = variables.get("vhost", "/")
 
         if ssl_enabled:
-
             # This started failing with python 3.10:
             # context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
             # -> Cannot create a client socket with a PROTOCOL_TLS_SERVER context
             context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
 
             context.load_default_certs()
 
@@ -106,15 +102,14 @@
                     ssl_options=pika.SSLOptions(
                         context=context, server_hostname=self.get_hostname(host)
                     ),
                 )
             )
 
         else:
-
             self.connection = pika.BlockingConnection(
                 pika.ConnectionParameters(
                     host=host,
                     port=port,
                     virtual_host=vhost,
                     credentials=pika.PlainCredentials(user, password),
                 )
@@ -170,51 +165,47 @@
             channel.exchange_declare(exchange=exchange, passive=True)
             return True
         except ChannelClosedByBroker as e:
             log.error(e)
             return False
 
     def create_exchange(self, exchange: str) -> None:
-
         channel = self.get_channel()
         channel.exchange_declare(
             exchange=exchange, exchange_type="direct", durable=True, auto_delete=False
         )
 
     def delete_exchange(self, exchange: str) -> None:
-
         channel = self.get_channel()
         channel.exchange_delete(exchange, if_unused=False)
 
     def queue_exists(self, queue: str) -> bool:
         channel = self.get_channel()
         try:
             channel.queue_declare(queue=queue, passive=True)
             return True
         except ChannelClosedByBroker as e:
             log.error(e)
             return False
 
     def create_queue(self, queue: str) -> None:
-
         channel = self.get_channel()
         channel.queue_declare(
             queue=queue, durable=True, exclusive=False, auto_delete=False
         )
 
     def delete_queue(self, queue: str) -> None:
-
         channel = self.get_channel()
         channel.queue_delete(
             queue,
             if_unused=False,
             if_empty=False,
         )
 
-    def get_bindings(self, exchange: str) -> Optional[List[Dict[str, str]]]:
+    def get_bindings(self, exchange: str) -> Optional[list[dict[str, str]]]:
         if not self.exchange_exists(exchange):
             log.error("Exchange {} does not exist", exchange)
             return None
 
         host = self.variables.get("host", "")
         schema = ""
         if not host.startswith("http"):
@@ -225,14 +216,18 @@
 
         port = self.variables.get("management_port")
         # url-encode unsafe characters by also including / (thanks to safe parameter)
         # / -> %2F
         vhost = urllib.parse.quote(self.variables.get("vhost", "/"), safe="")
         user = self.variables.get("user")
         password = self.variables.get("password")
+        if not user or not password:  # pragma: no cover
+            log.error("Invalid rabbitmq username or password, can't retrieve bindings")
+            return None
+
         # API Reference:
         # A list of all bindings in which a given exchange is the source.
         r = requests.get(
             f"{schema}{host}:{port}/api/exchanges/{vhost}/{exchange}/bindings/source",
             auth=HTTPBasicAuth(user, password),
             # this verify=False is needed because APIs are called on
             # the internal docker network where the TLS certificate is invalid
@@ -251,58 +246,56 @@
         for row in response:
             # row == {
             #   'source': exchange-name,
             #   'vhost': probably '/',
             #   'destination': queue-or-dest-exchange-name,
             #   'destination_type': 'queue' or 'exchange',
             #   'routing_key': routing_key,
-            #   'arguments': Dict,
+            #   'arguments': dict,
             #   'properties_key': ?? as routing_key?
             # }
 
             bindings.append(
                 {
                     "exchange": row["source"],
                     "routing_key": row["routing_key"],
                     "queue": row["destination"],
                 }
             )
 
         return bindings
 
     def queue_bind(self, queue: str, exchange: str, routing_key: str) -> None:
-
         channel = self.get_channel()
         channel.queue_bind(queue=queue, exchange=exchange, routing_key=routing_key)
 
     def queue_unbind(self, queue: str, exchange: str, routing_key: str) -> None:
-
         channel = self.get_channel()
         channel.queue_unbind(queue=queue, exchange=exchange, routing_key=routing_key)
 
     def send_json(
         self,
         message: Any,
         routing_key: str = "",
         exchange: str = "",
-        headers: Optional[Dict[str, Any]] = None,
+        headers: Optional[dict[str, Any]] = None,
     ) -> bool:
         return self.send(
             body=orjson.dumps(message),
             routing_key=routing_key,
             exchange=exchange,
             headers=headers,
         )
 
     def send(
         self,
         body: bytes,
         routing_key: str = "",
         exchange: str = "",
-        headers: Optional[Dict[str, Any]] = None,
+        headers: Optional[dict[str, Any]] = None,
     ) -> bool:
         """
         Send a message to the RabbitMQ queue
 
         :param body: the data to be send.
                         If this message should be json-encoded please use .send_json()
         :param exchange: RabbitMQ exchange where the message should be sent.
@@ -328,15 +321,14 @@
             #           "
             #     )
             # )
             user_id=self.variables.get("user"),
         )
 
         try:
-
             channel = self.get_channel()
             channel.basic_publish(
                 exchange=exchange,
                 routing_key=routing_key,
                 body=body,
                 properties=props,
                 mandatory=True,
@@ -384,13 +376,18 @@
 
 instance = RabbitExt()
 
 
 def get_instance(
     verification: Optional[int] = None,
     expiration: Optional[int] = None,
+    retries: int = 1,
+    retry_wait: int = 0,
     **kwargs: str,
 ) -> "RabbitExt":
-
     return instance.get_instance(
-        verification=verification, expiration=expiration, **kwargs
+        verification=verification,
+        expiration=expiration,
+        retries=retries,
+        retry_wait=retry_wait,
+        **kwargs,
     )
```

### Comparing `rapydo_http-2.4/restapi/connectors/smtp/__init__.py` & `rapydo_http-3.0/restapi/connectors/smtp/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,22 @@
 SMTP connector with automatic integration in rapydo framework
 """
 
 import socket
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.utils import formatdate
-from smtplib import SMTPAuthenticationError, SMTPException, SMTPServerDisconnected
+from smtplib import (
+    SMTPAuthenticationError,
+    SMTPConnectError,
+    SMTPException,
+    SMTPServerDisconnected,
+)
 from threading import Thread
-from typing import List, Optional, Union
+from typing import Optional, Union
 
 from restapi.config import TESTING
 from restapi.connectors import Connector, ExceptionsList
 from restapi.env import Env
 
 # mypy: ignore-errors
 if TESTING:
@@ -25,25 +30,26 @@
 MAX_NUM_RETRIES = 3
 
 
 class Mail(Connector):
     def __init__(self) -> None:
         self.smtp: Optional[SMTP] = None
         super().__init__()
-        # instance_variables is updated with custom variabiles in connect
-        # and the used in the send method.
-        # This way the send method will be able to use variabiles overridden in connect
+        # instance_variables is updated with custom variables in connect
+        # and then used in the send method.
+        # This way the send method will be able to use variables overridden in connect
         self.instance_variables = self.variables.copy()
 
     @staticmethod
     def get_connection_exception() -> ExceptionsList:
-        return (socket.gaierror, SMTPAuthenticationError)
+        return (socket.gaierror, SMTPAuthenticationError, SMTPConnectError)
 
     def connect(self, **kwargs: str) -> "Mail":
-        self.instance_variables.update(kwargs)
+        # Note: will be used later in send()
+        self.instance_variables = self.variables | kwargs
 
         port = Env.to_int(self.instance_variables.get("port")) or 25
 
         host = self.instance_variables.get("host")
 
         if port == 465:
             smtp = SMTP_SSL(host)
@@ -74,15 +80,14 @@
             self.smtp = None
         except SMTPServerDisconnected:  # pragma: no cover
             log.debug("SMTP is already disconnected")
 
         return None
 
     def is_connected(self) -> bool:
-
         if not self.smtp or self.disconnected:
             return False
 
         try:
             status = self.smtp.noop()[0]
             return status == 250
         except SMTPServerDisconnected:  # pragma: no cover
@@ -91,19 +96,18 @@
     @classmethod
     def send_async(
         cls,
         body: str,
         subject: str,
         to_address: Optional[str] = None,
         from_address: Optional[str] = None,
-        cc: Union[None, str, List[str]] = None,
-        bcc: Union[None, str, List[str]] = None,
+        cc: Union[None, str, list[str]] = None,
+        bcc: Union[None, str, list[str]] = None,
         plain_body: Optional[str] = None,
     ) -> None:
-
         thr = Thread(
             target=cls.send_async_thread,
             args=[body, subject, to_address, from_address, cc, bcc, plain_body],
         )
         thr.start()
 
         # in TESTING mode async mails are kept sync to simplify checks
@@ -118,20 +122,19 @@
     @classmethod
     def send_async_thread(
         cls,
         body: str,
         subject: str,
         to_address: Optional[str] = None,
         from_address: Optional[str] = None,
-        cc: Union[None, str, List[str]] = None,
-        bcc: Union[None, str, List[str]] = None,
+        cc: Union[None, str, list[str]] = None,
+        bcc: Union[None, str, list[str]] = None,
         plain_body: Optional[str] = None,
         retry: int = 1,
     ) -> bool:
-
         with get_instance() as client:
             sent = client.send(
                 body, subject, to_address, from_address, cc, bcc, plain_body
             )
 
         if sent or retry > MAX_NUM_RETRIES:
             return sent
@@ -150,19 +153,18 @@
 
     def send(
         self,
         body: str,
         subject: str,
         to_address: Optional[str] = None,
         from_address: Optional[str] = None,
-        cc: Union[None, str, List[str]] = None,
-        bcc: Union[None, str, List[str]] = None,
+        cc: Union[None, str, list[str]] = None,
+        bcc: Union[None, str, list[str]] = None,
         plain_body: Optional[str] = None,
     ) -> bool:
-
         if not to_address:
             to_address = self.instance_variables.get("admin")
         if not to_address:
             log.error("Skipping send email: destination address not configured")
             return False
 
         if not from_address:
@@ -170,46 +172,45 @@
         if not from_address:
             from_address = self.instance_variables.get("admin")
         if not from_address:
             log.error("Skipping send email: from address not configured")
             return False
 
         try:
-
             if plain_body is not None:
                 msg = MIMEMultipart("alternative")
             else:
                 msg = MIMEText(body)
 
             msg["Subject"] = subject
             msg["From"] = from_address
             msg["To"] = to_address
 
-            dest_addresses = [to_address]
+            dest_addresses: list[str] = [to_address]
 
             if cc is None:
                 pass
             elif isinstance(cc, str):
                 msg["Cc"] = cc
                 dest_addresses.append(cc.split(","))
             elif isinstance(cc, list):
                 msg["Cc"] = ",".join(cc)
-                dest_addresses.append(cc)
+                dest_addresses.extend(cc)
             else:
                 log.warning("Invalid CC value: {}", cc)
                 cc = None
 
             if bcc is None:
                 pass
             elif isinstance(bcc, str):
                 msg["Bcc"] = bcc
                 dest_addresses.append(bcc.split(","))
             elif isinstance(bcc, list):
                 msg["Bcc"] = ",".join(bcc)
-                dest_addresses.append(bcc)
+                dest_addresses.extend(bcc)
             else:
                 log.warning("Invalid BCC value: {}", bcc)
                 bcc = None
 
             msg["Date"] = formatdate()
 
             if plain_body is not None:
@@ -242,13 +243,18 @@
 
 instance = Mail()
 
 
 def get_instance(
     verification: Optional[int] = None,
     expiration: Optional[int] = None,
+    retries: int = 1,
+    retry_wait: int = 0,
     **kwargs: str,
 ) -> "Mail":
-
     return instance.get_instance(
-        verification=verification, expiration=expiration, **kwargs
+        verification=verification,
+        expiration=expiration,
+        retries=retries,
+        retry_wait=retry_wait,
+        **kwargs,
     )
```

### Comparing `rapydo_http-2.4/restapi/connectors/smtp/mailmock.py` & `rapydo_http-3.0/restapi/connectors/smtp/mailmock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import email
 from smtplib import SMTPException, SMTPServerDisconnected
 from types import TracebackType
-from typing import Optional, Tuple, Type, TypeVar
+from typing import Optional, TypeVar
 
 import orjson
 
 from restapi.utilities.logs import LOGS_FOLDER, log
 
 T = TypeVar("T", bound="SMTP")
 
@@ -20,15 +20,15 @@
         self.disconnected = False
 
     def __enter__(self: T) -> T:  # pragma: no cover
         return self
 
     def __exit__(
         self,
-        _type: Optional[Type[Exception]],
+        _type: Optional[type[Exception]],
         value: Optional[Exception],
         tb: Optional[TracebackType],
     ) -> bool:  # pragma: no cover
         # return False if the exception is not handled:
         # -> return True if the exception is None (nothing to be handled)
         # -> return False if the exception is not None (because it is not handled here)
         # always return False is not accepted by mypy...
@@ -52,15 +52,14 @@
 
     @staticmethod
     def ehlo() -> None:
         log.info("Mail mock sent ehlo message")
 
     @staticmethod
     def sendmail(from_address: str, dest_addresses: str, msg: str) -> None:
-
         if from_address == "invalid1":
             raise SMTPException("SMTP Error")
 
         if from_address == "invalid2":
             raise Exception("Generic Error")
 
         json_fpath = LOGS_FOLDER.joinpath("mock.mail.lastsent.json")
@@ -81,31 +80,31 @@
         log.info("Mail mock sent email from {} to {}", from_address, dest_addresses)
         log.info("Mail mock mail written in {}", json_fpath)
 
         log.info("Extracting body")
         b = email.message_from_string(msg)
         if b.is_multipart():
             # get the first payload (the non html version)
-            first_payload = b.get_payload()[0]
+            first_payload = b.get_payload()[0]  # type: ignore
             # This is enough when the message is not based64-encoded
-            payload = first_payload.get_payload()
+            # payload = first_payload.get_payload()
             # Otherwise this is needed:
-            payload = first_payload.get_payload(decode=True).decode("utf-8")
+            payload = first_payload.get_payload(decode=True).decode("utf-8")  # type: ignore
         else:
             # This is enough when the message is not based64-encoded
             # payload = b.get_payload()
             # Otherwise this is needed:
-            payload = b.get_payload(decode=True).decode("utf-8")
+            payload = b.get_payload(decode=True).decode("utf-8")  # type: ignore
 
         with open(body_fpath, "w+") as file:
             file.write(payload)
 
         log.info("Mail body written in {}", body_fpath)
 
-    def noop(self) -> Tuple[int]:
+    def noop(self) -> tuple[int]:
         if self.disconnected:
             raise SMTPServerDisconnected  # pragma: no cover
 
         return (250,)
 
 
 class SMTP_SSL(SMTP):
```

### Comparing `rapydo_http-2.4/restapi/connectors/smtp/notifications.py` & `rapydo_http-3.0/restapi/connectors/smtp/notifications.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Dict, Iterator, Optional, Tuple
+from collections.abc import Iterator
+from typing import Any, Optional
 
 import html2text
 import jinja2
 
 from restapi.config import (
     ABS_RESTAPI_PATH,
     CODE_DIR,
@@ -16,44 +17,42 @@
 from restapi.env import Env
 from restapi.services.authentication import Login, User
 from restapi.utilities.logs import log
 from restapi.utilities.time import seconds_to_human
 
 
 def get_html_template(
-    template_file: str, replaces: Dict[str, Any]
-) -> Tuple[Optional[str], Optional[str]]:
-
+    template_file: str, replaces: dict[str, Any]
+) -> tuple[Optional[str], Optional[str]]:
     html = _get_html_template(template_file, replaces)
     header_html = _get_html_template("email_header.html", replaces)
     footer_html = _get_html_template("email_footer.html", replaces)
 
     if html is None or header_html is None or footer_html is None:
         return None, None
 
     html_body = f"{header_html}{html}{footer_html}"
     plain_body = convert_html2text(html_body)
     return html_body, plain_body
 
 
 def convert_html2text(html_body: str) -> str:
-
     h2t = html2text.HTML2Text()
     h2t.unicode_snob = False
     h2t.ignore_emphasis = True
     h2t.single_line_break = True
     h2t.ignore_images = True
     # zero for no wrap of long lines [otherwise tokens in urls will be broken]
     # but since the maximum allowed line length on email is 998 octets
     # I set a very long wrap, that should not break any tokens
     h2t.body_width = 512
     return h2t.handle(html_body)
 
 
-def _get_html_template(template_file: str, replaces: Dict[str, Any]) -> Optional[str]:
+def _get_html_template(template_file: str, replaces: dict[str, Any]) -> Optional[str]:
     # Custom templates from project backend/models/email/
     template_path = CODE_DIR.joinpath(
         CUSTOM_PACKAGE, MODELS_DIR, "emails", template_file
     )
 
     if not template_path.exists():
         # Core templates from restapi/connectors/smtp/templates/
@@ -65,43 +64,50 @@
         )
 
     if not template_path.exists():
         log.info("Template not found: {}", template_path)
         return None
 
     try:
-
         templateLoader = jinja2.FileSystemLoader(searchpath=template_path.parent)
         templateEnv = jinja2.Environment(loader=templateLoader, autoescape=True)
         template = templateEnv.get_template(template_file)
 
         replaces.setdefault("host", get_frontend_url())
 
         return template.render(**replaces)
     except Exception as e:  # pragma: no cover
         log.error("Error loading template {}: {}", template_file, e)
         return None
 
 
+def get_reply_to() -> str:
+    if addr := Env.get("SMTP_REPLYTO", ""):
+        return addr
+    if addr := Env.get("SMTP_NOREPLY", ""):
+        return addr
+    return Env.get("SMTP_ADMIN", "")
+
+
 def send_notification(
     subject: str,
     template: str,
     # if None will be sent to the administrator
     to_address: Optional[str] = None,
-    data: Optional[Dict[str, Any]] = None,
+    data: Optional[dict[str, Any]] = None,
     user: Optional[User] = None,
     send_async: bool = False,
 ) -> bool:
-
     # Always enabled during tests
     if not Connector.check_availability("smtp"):  # pragma: no cover
         return False
 
     title = get_project_configuration("project.title", default="Unkown title")
-    reply_to = Env.get("SMTP_NOREPLY", Env.get("SMTP_ADMIN", ""))
+
+    reply_to = get_reply_to()
 
     if data is None:
         data = {}
 
     data.setdefault("project", title)
     data.setdefault("reply_to", reply_to)
 
@@ -133,93 +139,86 @@
         body=html_body,
         to_address=to_address,
         plain_body=plain_body,
     )
 
 
 def send_registration_notification(user: User) -> None:
-
     # no return value since it is a send_async
     send_notification(
         subject="New user registered",
         template="new_user_registered.html",
         to_address=None,
         data=None,
         user=user,
         send_async=True,
     )
 
 
 def send_activation_link(user: User, url: str) -> bool:
-
     return send_notification(
         subject=Env.get("EMAIL_ACTIVATION_SUBJECT", "Account activation"),
         template="activate_account.html",
         to_address=user.email,
         data={"url": url},
         user=user,
     )
 
 
 def send_password_reset_link(user: User, uri: str, reset_email: str) -> bool:
-
     return send_notification(
         subject="Password Reset",
         template="reset_password.html",
         to_address=reset_email,
         data={"url": uri},
         user=user,
     )
 
 
 def notify_login_block(
     user: User, events: Iterator[Login], duration: int, url: str
 ) -> None:
-
     # no return value since it is a send_async
     send_notification(
         subject="Your credentials have been blocked",
         template="blocked_credentials.html",
         to_address=user.email,
         data={"events": events, "duration": seconds_to_human(duration), "url": url},
         user=user,
         send_async=True,
     )
 
 
 def notify_new_credentials_to_user(user: User, unhashed_password: str) -> None:
-
     # no return value since it is a send_async
     send_notification(
         subject="New credentials",
         template="new_credentials.html",
         to_address=user.email,
         data={"password": unhashed_password},
         user=user,
         send_async=True,
     )
 
 
 def notify_update_credentials_to_user(user: User, unhashed_password: str) -> None:
-
     # no return value since it is a send_async
     send_notification(
         subject="Password changed",
         template="update_credentials.html",
         to_address=user.email,
         data={"password": unhashed_password},
         user=user,
         send_async=True,
     )
 
 
 def send_celery_error_notification(
     task_id: str, task_name: str, arguments: str, error_stack: Any, retry_num: int
 ) -> None:
-
     if retry_num > 0:
         subject = f"Task {task_name} failed (failure #{retry_num})"
     else:
         subject = f"Task {task_name} failed"
 
     # no return value since it is a send_async
     send_notification(
```

### Comparing `rapydo_http-2.4/restapi/connectors/smtp/templates/blocked_credentials.html` & `rapydo_http-3.0/restapi/connectors/smtp/templates/blocked_credentials.html`

 * *Files identical despite different names*

### Comparing `rapydo_http-2.4/restapi/connectors/smtp/templates/email_footer.html` & `rapydo_http-3.0/restapi/connectors/smtp/templates/email_footer.html`

 * *Files identical despite different names*

### Comparing `rapydo_http-2.4/restapi/connectors/sqlalchemy/__init__.py` & `rapydo_http-3.0/restapi/connectors/sqlalchemy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 """
-SQLalchemy connector based on Flask-SQLalchemy, with automatic integration in
-rapydo framework
+Connector based on SQLalchemy with automatic integration with RAPyDo framework
 """
 
 import re
 from datetime import datetime, timedelta
 from functools import wraps
-from typing import Any, Callable, Dict, List, Optional, TypeVar, cast
+from typing import Any, Callable, Optional, TypeVar, cast
 
 import pytz
-import sqlalchemy
-from flask_migrate import Migrate
-from flask_sqlalchemy import Model
-from flask_sqlalchemy import SQLAlchemy as OriginalAlchemy
 from psycopg2 import OperationalError as PsycopgOperationalError
-from sqlalchemy import create_engine, text
+from sqlalchemy import create_engine, inspect, select, text
 from sqlalchemy.engine.base import Connection
 from sqlalchemy.engine.url import URL
 from sqlalchemy.exc import (
+    DatabaseError,
     IntegrityError,
     InternalError,
+    InvalidRequestError,
     OperationalError,
     ProgrammingError,
+    StatementError,
 )
 from sqlalchemy.orm import Session, scoped_session, sessionmaker
 from sqlalchemy.orm.attributes import set_attribute
 from sqlalchemy.orm.session import close_all_sessions
 
 from restapi.connectors import Connector, ExceptionsList
 from restapi.env import Env
@@ -41,25 +39,22 @@
     Group,
     Login,
     Payload,
     RoleObj,
     Token,
     User,
 )
+from restapi.utilities.globals import mem
 from restapi.utilities.logs import Events, log
-from restapi.utilities.time import get_now
 from restapi.utilities.uuid import getUUID
 
-# all instances have to use the same alchemy object
-db = OriginalAlchemy()
-
 F = TypeVar("F", bound=Callable[..., Any])
 
 
-def parse_postgres_duplication_error(excpt: List[str]) -> Optional[str]:
+def parse_postgres_duplication_error(excpt: list[str]) -> Optional[str]:
     if m0 := re.search(
         r".*duplicate key value violates unique constraint \"(.*)\"", excpt[0]
     ):
         # duplicate key value violates unique constraint "user_email_key"
         # => m0.group(1) === user_email_key
         # => table = user
         table = m0.group(1).split("_")[0]
@@ -69,75 +64,60 @@
             prop = m.group(1)
             val = m.group(2)
             return f"A {table.title()} already exists with {prop}: {val}"
 
     return None
 
 
-def parse_missing_error(excpt: List[str]) -> Optional[str]:
-
+def parse_missing_error(excpt: list[str]) -> Optional[str]:
     if m := re.search(
         r"null value in column \"(.*)\" of relation \"(.*)\" "
         "violates not-null constraint",
         excpt[0],
     ):
         prop = m.group(1)
         table = m.group(2)
 
         return f"Missing property {prop} required by {table.title()}"
 
-    if m0 := re.search(r".*Column '(.*)' cannot be null.*", excpt[0]):
-
-        prop = m0.group(1)
-
-        # table name can be "tablename" or "`tablename`"
-        # => match all non-space and non-backticks characters optioanlly wrapped among `
-        m = re.search(r".*INSERT INTO `?([^\s`]+)`? \(.*", excpt[1])
-
-        if m:
-            table = m.group(1)
-            return f"Missing property {prop} required by {table.title()}"
-
     return None  # pragma: no cover
 
 
 def catch_db_exceptions(func: F) -> F:
     @wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
-
         try:
             return func(*args, **kwargs)
         except RestApiException:
             # already catched and parser, raise up
             raise
         except IntegrityError as e:
             message = str(e).split("\n")
 
             if error := parse_postgres_duplication_error(message):
-                raise DatabaseDuplicatedEntry(error)
+                raise DatabaseDuplicatedEntry(error) from e
 
             if error := parse_missing_error(message):
-                raise DatabaseMissingRequiredProperty(error)
+                raise DatabaseMissingRequiredProperty(error) from e
 
             # Should never happen except in case of a new alchemy version
             log.error("Unrecognized error message: {}", e)  # pragma: no cover
-            raise ServiceUnavailable("Duplicated entry")  # pragma: no cover
+            raise ServiceUnavailable("Duplicated entry") from e  # pragma: no cover
 
         except InternalError as e:  # pragma: no cover
-
             m = re.search(
                 r"Incorrect string value: '(.*)' for column `.*`.`.*`.`(.*)` at row .*",
                 str(e),
             )
 
             if m:
                 value = m.group(1)
                 column = m.group(2)
                 error = f"Invalid {column}: {value}"
-                raise BadRequest(error)
+                raise BadRequest(error) from e
 
             log.error("Unrecognized error message: {}", e)
             raise
 
         except ProgrammingError as e:
             # Ignore ProgrammingError (like Table doesn't exist) during initialization
             if not SQLAlchemy.DB_INITIALIZING:
@@ -154,318 +134,317 @@
 
     return cast(F, wrapper)
 
 
 class SQLAlchemy(Connector):
     # Used to suppress some errors raised during DB initialization
     DB_INITIALIZING = False
+    _session: Optional[scoped_session[Session]] = None
 
     def __init__(self) -> None:
         # Type of variable becomes "Any" due to an unfollowed import
-        self.db: OriginalAlchemy = None  # type: ignore
+        self.db: Any = None
+        # self.engine: Optional[Engine] = None
         super().__init__()
 
-    # This is used to return Models in a type-safe way
-    # Return type becomes "Any" due to an unfollowed import
-    def __getattr__(self, name: str) -> Model:  # type: ignore
+    def __getattr__(self, name: str) -> Any:
         if name in self._models:
             return self._models[name]
         raise AttributeError(f"Model {name} not found")
 
     @staticmethod
-    def is_mysql() -> bool:
-        # could be based on self.variables but this version Env based
-        # can be used as static method and be used before creating instances
-        return (
-            Env.get("AUTH_SERVICE", "NO_AUTHENTICATION") == "sqlalchemy"
-            and Env.get("ALCHEMY_DBTYPE", "postgresql") == "mysql+pymysql"
-        )
-        # return self.variables.get("dbtype", "postgresql") == "mysql+pymysql"
-
-    @staticmethod
     def get_connection_exception() -> ExceptionsList:
-        # type is ignored here due to untyped psycopg2
         return (
             OperationalError,
             PsycopgOperationalError,
-        )  # type: ignore
+        )  # type: ignore[return-value]
 
     def connect(self, **kwargs: str) -> "SQLAlchemy":
+        variables = self.variables | kwargs
 
-        variables = self.variables.copy()
-        variables.update(kwargs)
-
-        query = None
-        if self.is_mysql() and not Connector.is_external(variables.get("host", "")):
-            query = {"charset": "utf8mb4"}
-
-        uri = URL.create(  # type: ignore
+        uri = URL.create(
             drivername=variables.get("dbtype", "postgresql"),
             username=variables.get("user"),
             password=variables.get("password"),
             host=variables.get("host"),
-            port=variables.get("port"),
+            port=Env.to_int(variables.get("port"), 5432),
             database=variables.get("db"),
-            query=query,
+            query={},
         )
-        # TODO: in case we need different connection binds
-        # (multiple connections with sql) then:
-        # SQLALCHEMY_BINDS = {
-        #     'users':        'mysqldb://localhost/users',
-        #     'appmeta':      'sqlite:////path/to/appmeta.db'
-        # }
-        if self.app:
-            self.app.config["SQLALCHEMY_DATABASE_URI"] = uri
-            # self.app.config['SQLALCHEMY_POOL_TIMEOUT'] = 3
-            self.app.config["SQLALCHEMY_TRACK_MODIFICATIONS"] = False
-
-            # The Alembic package, which handles the migration work, does not recognize
-            # type changes in columns by default. If you want that fine level of
-            # detection you need to enable the compare_type option
-            Migrate(self.app, db, compare_type=True)
-
-        # Overwrite db.session created by flask_alchemy due to errors
-        # with transaction when concurrent requests...
-
-        db.engine_bis = create_engine(uri, encoding="utf8")
-        db.session = scoped_session(sessionmaker(bind=db.engine_bis))
-        db.session.commit = catch_db_exceptions(db.session.commit)  # type: ignore
-        db.session.flush = catch_db_exceptions(db.session.flush)  # type: ignore
-        # db.update_properties = self.update_properties
-        # db.disconnect = self.disconnect
-        # db.is_connected = self.is_connected
 
+        poolsize = Env.to_int(variables.get("poolsize"), 30)
+        if uri not in mem.sqlalchemy_engines:
+            mem.sqlalchemy_engines[uri] = create_engine(
+                uri,
+                pool_size=poolsize,
+                max_overflow=poolsize + 10,
+                execution_options={"isolation_level": "READ COMMITTED"},
+                future=True,
+            )
+        engine = mem.sqlalchemy_engines[uri]
+        if len(mem.sqlalchemy_engines) == 1:
+            # None URL is used as default URL
+            mem.sqlalchemy_engines[None] = mem.sqlalchemy_engines[uri]
+
+        # avoid circular imports
+        from restapi.connectors.sqlalchemy.models import Base as db
+
+        self._session = scoped_session(sessionmaker(bind=engine))
+        self._session.commit = catch_db_exceptions(self._session.commit)  # type: ignore
+        self._session.flush = catch_db_exceptions(self._session.flush)  # type: ignore
         Connection.execute = catch_db_exceptions(Connection.execute)  # type: ignore
-        # Used in case of autoflush
-        Connection._execute_context = catch_db_exceptions(Connection._execute_context)  # type: ignore
+        # Used in case of autoflush - shouldn't be needed with sqlalchemy 2?
+        Connection._execute_context = catch_db_exceptions(Connection._execute_context)  # type: ignore  # noqa
 
-        if self.app:
-            # This is to prevent multiple app initialization and avoid the error:
-            #   A setup function was called after the first request was handled.
-            #   This usually indicates a bug in the application where a module was
-            #   not imported and decorators or other functionality was called too late.
-            #   To fix this make sure to import all your view modules,
-            #   database models and everything related at a central place before
-            #   the application starts serving requests.
-            if "sqlalchemy" not in self.app.extensions:
-                db.init_app(self.app)
-
-            # This is needed to test the connection
-            with self.app.app_context():
-                sql = text("SELECT 1")
-                db.engine.execute(sql)
-        # This is to test the connection when executed from the cli (i.e. outside flask)
-
-        else:
-            sql = text("SELECT 1")
-            db.session.execute(sql)
+        sql = text("SELECT 1")
+        self.session.execute(sql)
 
+        self.load_models()
         self.db = db
         return self
 
     @property
-    def session(self) -> Session:
-        return cast(Session, self.db.session)
+    def session(self) -> scoped_session[Session]:
+        if self._session is None:  # pragma: no cover
+            raise ServiceUnavailable("Session not initialized")
+        return self._session
 
     def disconnect(self) -> None:
-        if self.db:
-            self.db.session.close()
+        if self._session:
+            self._session.remove()
         self.disconnected = True
 
     def is_connected(self) -> bool:
         log.warning("sqlalchemy.is_connected method is not implemented")
         return not self.disconnected
 
     def initialize(self) -> None:
-
         instance = self.get_instance()
+        sql = text("SELECT 1")
+        instance.session.execute(sql)
 
-        if self.app:
-            with self.app.app_context():
-
-                sql = text("SELECT 1")
-                instance.db.engine.execute(sql)
+        SQLAlchemy.DB_INITIALIZING = True
 
-                SQLAlchemy.DB_INITIALIZING = True
-                instance.db.create_all()
-                SQLAlchemy.DB_INITIALIZING = False
+        # Get default URL
+        engine = mem.sqlalchemy_engines.get(None)
+        if not engine:
+            return None
+        instance.db.metadata.create_all(engine)
+        SQLAlchemy.DB_INITIALIZING = False
 
     def destroy(self) -> None:
-
         instance = self.get_instance()
+        sql = text("SELECT 1")
+        instance.session.execute(sql)
 
-        if self.app:
-            with self.app.app_context():
-
-                sql = text("SELECT 1")
-                instance.db.engine.execute(sql)
-
-                instance.db.session.remove()
-                close_all_sessions()
-                # massive destruction
-                log.critical("Destroy current SQL data")
-                instance.db.drop_all()
+        # instance.session.remove()
+        close_all_sessions()
+        # Get default URL
+        engine = mem.sqlalchemy_engines.get(None)
+        if not engine:
+            return None
+
+        # Massive destruction
+        log.critical("Destroy current SQL data")
+        instance.db.metadata.drop_all(engine)
 
     @staticmethod
-    # Argument 1 to "update_properties" becomes "Any" due to an unfollowed import
-    def update_properties(instance: Model, properties: Dict[str, Any]) -> None:  # type: ignore
-
+    def update_properties(instance: Any, properties: dict[str, Any]) -> None:
         for field, value in properties.items():
-            # Call to untyped function "set_attribute" in typed context
-            set_attribute(instance, field, value)  # type: ignore
+            set_attribute(instance, field, value)
 
 
 class Authentication(BaseAuthentication):
     def __init__(self) -> None:
         self.db: SQLAlchemy = get_instance()
 
-    # Also used by POST user
-    def create_user(self, userdata: Dict[str, Any], roles: List[str]) -> User:
+    def init_auth_db(self, options: dict[str, bool]) -> None:
+        self.db.initialize()
+        return super().init_auth_db(options)
 
+    # Also used by POST user
+    def create_user(
+        self, userdata: dict[str, Any], roles: list[str], group: Group
+    ) -> User:
         userdata.setdefault("authmethod", "credentials")
         userdata.setdefault("uuid", getUUID())
 
         if "password" in userdata:
             userdata["password"] = self.get_password_hash(userdata["password"])
 
+        userdata["group_id"] = group.id
         userdata, extra_userdata = self.custom_user_properties_pre(userdata)
 
         user = self.db.User(**userdata)
         self.link_roles(user, roles)
 
         self.custom_user_properties_post(user, userdata, extra_userdata, self.db)
 
         self.db.session.add(user)
-
+        # why commit is not needed here!?
         return user
 
-    def link_roles(self, user: User, roles: List[str]) -> None:
-
+    def link_roles(self, user: User, roles: list[str]) -> None:
         if not roles:
             roles = [BaseAuthentication.default_role]
 
-        # link roles into users
-        user.roles = []
+        roles_instances = []
         for role in roles:
-            sqlrole = self.db.Role.query.filter_by(name=role).first()
-            user.roles.append(sqlrole)
+            sqlrole = self.db.session.execute(
+                select(self.db.Role).where(self.db.Role.name == role)
+            ).scalar()
+
+            roles_instances.append(sqlrole)
 
-    def create_group(self, groupdata: Dict[str, Any]) -> Group:
+        user.roles = roles_instances
+        # why commit is not needed here!?
 
+    def create_group(self, groupdata: dict[str, Any]) -> Group:
         groupdata.setdefault("uuid", getUUID())
 
         group = self.db.Group(**groupdata)
 
         self.db.session.add(group)
         self.db.session.commit()
 
         return group
 
     def add_user_to_group(self, user: User, group: Group) -> None:
-
         if user and group:
             user.belongs_to = group
 
             self.db.session.add(user)
             self.db.session.commit()
 
     def get_user(
         self, username: Optional[str] = None, user_id: Optional[str] = None
     ) -> Optional[User]:
         try:
             if username:
-                return self.db.User.query.filter_by(email=username).first()
+                users = self.db.session.execute(
+                    select(self.db.User).where(self.db.User.email == username)
+                ).scalar()
+                # self.db.session.commit()
+                return users
 
             if user_id:
-                return self.db.User.query.filter_by(uuid=user_id).first()
+                users = self.db.session.execute(
+                    select(self.db.User).where(self.db.User.uuid == user_id)
+                ).scalar()
+                # self.db.session.commit()
+                return users
 
-        except (sqlalchemy.exc.StatementError, sqlalchemy.exc.InvalidRequestError) as e:
+        except (StatementError, InvalidRequestError) as e:
             log.error(e)
-            raise ServiceUnavailable("Backend database is unavailable")
+            raise ServiceUnavailable("Backend database is unavailable") from e
         except (
-            sqlalchemy.exc.DatabaseError,
-            sqlalchemy.exc.OperationalError,
+            DatabaseError,
+            OperationalError,
         ) as e:  # pragma: no cover
             raise e
 
         # only reached if both username and user_id are None
         return None
 
-    def get_users(self) -> List[User]:
-        return cast(List[User], self.db.User.query.all())
+    def get_users(self) -> list[User]:
+        users = list(self.db.session.execute(select(self.db.User)).scalars())
+        # self.db.session.commit()
+        return users
 
     def save_user(self, user: User) -> bool:
         if not user:
             return False
 
         self.db.session.add(user)
         self.db.session.commit()
         return True
 
     def delete_user(self, user: User) -> bool:
         if not user:
             return False
 
-        # Call to untyped function "delete" in typed context
-        self.db.session.delete(user)  # type: ignore
+        self.db.session.delete(user)
         self.db.session.commit()
         return True
 
     def get_group(
         self, group_id: Optional[str] = None, name: Optional[str] = None
     ) -> Optional[Group]:
         if group_id:
-            return self.db.Group.query.filter_by(uuid=group_id).first()
+            group = self.db.session.execute(
+                select(self.db.Group).where(self.db.Group.uuid == group_id)
+            ).scalar()
+            # self.db.session.commit()
+            return group
 
         if name:
-            return self.db.Group.query.filter_by(shortname=name).first()
+            group = self.db.session.execute(
+                select(self.db.Group).where(self.db.Group.shortname == name)
+            ).scalar()
+            # self.db.session.commit()
+            return group
 
         return None
 
-    def get_groups(self) -> List[Group]:
-        return cast(List[Group], self.db.Group.query.all())
+    def get_groups(self) -> list[Group]:
+        groups = list(self.db.session.execute(select(self.db.Group)).scalars())
+        # self.db.session.commit()
+        return groups
 
     def get_user_group(self, user: User) -> Group:
-        return user.belongs_to
+        group = user.belongs_to
+        # self.db.session.commit()
+        return group
 
-    def get_group_members(self, group: Group) -> List[User]:
-        return list(group.members)
+    def get_group_members(self, group: Group) -> list[User]:
+        members = list(group.members)
+        # self.db.session.commit()
+        return members
 
     def save_group(self, group: Group) -> bool:
         if not group:
             return False
 
         self.db.session.add(group)
         self.db.session.commit()
         return True
 
     def delete_group(self, group: Group) -> bool:
         if not group:
             return False
 
-        # Call to untyped function "delete" in typed context
-        self.db.session.delete(group)  # type: ignore
+        self.db.session.delete(group)
         self.db.session.commit()
         return True
 
-    def get_roles(self) -> List[RoleObj]:
-        roles = []
-        for role in self.db.Role.query.all():
-            if role:
-                roles.append(role)
+    def get_roles(self) -> list[RoleObj]:
+        # Get default URL
+        engine = mem.sqlalchemy_engines.get(None)
+        if not engine and mem.sqlalchemy_engines:
+            engine = list(mem.sqlalchemy_engines.values())[0]
+        if not engine:
+            return []
 
+        inspect_engine = inspect(engine)
+        if not inspect_engine or not inspect_engine.has_table(
+            "role"
+        ):  # pragma: no cover
+            return []
+        roles = list(self.db.session.execute(select(self.db.Role)).scalars())
+        # self.db.session.commit()
         return roles
 
-    def get_roles_from_user(self, user: Optional[User]) -> List[str]:
-
+    def get_roles_from_user(self, user: Optional[User]) -> list[str]:
         # No user for non authenticated endpoints -> return no role
         if user is None:
             return []
 
-        return [role.name for role in user.roles]
+        roles = [role.name for role in user.roles]
+        # self.db.session.commit()
+        return roles
 
     def create_role(self, name: str, description: str) -> None:
         role = self.db.Role(name=name, description=description)
         self.db.session.add(role)
         self.db.session.commit()
 
     def save_role(self, role: RoleObj) -> bool:
@@ -474,15 +453,14 @@
             self.db.session.commit()
             return True
         return False
 
     def save_token(
         self, user: User, token: str, payload: Payload, token_type: Optional[str] = None
     ) -> None:
-
         ip_address = self.get_remote_ip()
 
         if token_type is None:
             token_type = self.FULL_TOKEN
 
         now = datetime.now(pytz.utc)
         exp = payload.get("exp", now + timedelta(seconds=self.DEFAULT_TOKEN_TTL))
@@ -492,39 +470,39 @@
             token=token,
             token_type=token_type,
             creation=now,
             last_access=now,
             expiration=exp,
             IP=ip_address,
             location="Unknown",
-            # the following two are equivalent
-            # user_id=user.id,
             emitted_for=user,
         )
 
         try:
             self.db.session.add(token_entry)
             # Save user updated in profile endpoint
             self.db.session.add(user)
             self.db.session.commit()
 
         except Exception as e:  # pragma: no cover
             log.error("DB error ({}), rolling back", e)
             self.db.session.rollback()
 
     def verify_token_validity(self, jti: str, user: User) -> bool:
-
-        token_entry = self.db.Token.query.filter_by(jti=jti).first()
+        token_entry = self.db.session.execute(
+            select(self.db.Token).where(self.db.Token.jti == jti)
+        ).scalar()
+        # self.db.session.commit()
 
         if token_entry is None:
             return False
         if token_entry.user_id is None or token_entry.user_id != user.id:
             return False
 
-        now = get_now(token_entry.expiration.tzinfo)
+        now = datetime.now(pytz.utc)
 
         if now > token_entry.expiration:
             self.invalidate_token(token=token_entry.token)
             log.info(
                 "This token is no longer valid: expired since {}",
                 token_entry.expiration.strftime("%d/%m/%Y"),
             )
@@ -554,30 +532,31 @@
         return True
 
     def get_tokens(
         self,
         user: Optional[User] = None,
         token_jti: Optional[str] = None,
         get_all: bool = False,
-    ) -> List[Token]:
-
-        tokens_list: List[Token] = []
+    ) -> list[Token]:
+        tokens_list: list[Token] = []
         tokens = None
 
         if get_all:
-            tokens = self.db.Token.query.all()
+            tokens = self.db.session.execute(select(self.db.Token)).scalars()
+
         elif user:
-            tokens = user.tokens.all()
+            tokens = user.tokens
         elif token_jti:
-            tokens = [self.db.Token.query.filter_by(jti=token_jti).first()]
+            tokens = self.db.session.execute(
+                select(self.db.Token).where(self.db.Token.jti == token_jti)
+            ).scalars()
 
         if tokens:
             for token in tokens:
-
-                if token is None:
+                if token is None:  # pragma: no cover
                     continue
 
                 t: Token = {
                     "id": token.jti,
                     "token": token.token,
                     "token_type": token.token_type,
                     "emitted": token.creation,
@@ -586,48 +565,47 @@
                     "IP": token.IP,
                     "location": token.location,
                 }
                 if get_all:
                     t["user"] = token.emitted_for
                 tokens_list.append(t)
 
+        # self.db.session.commit()
         return tokens_list
 
     def invalidate_token(self, token: str) -> bool:
-
-        token_entry = self.db.Token.query.filter_by(token=token).first()
+        token_entry = self.db.session.execute(
+            select(self.db.Token).where(self.db.Token.token == token)
+        ).scalar()
+        # self.db.session.commit()
         if token_entry:
             try:
-                # Call to untyped function "delete" in typed context
-                self.db.session.delete(token_entry)  # type: ignore
+                self.db.session.delete(token_entry)
                 self.db.session.commit()
                 self.log_event(Events.delete, target=token_entry)
                 return True
             except Exception as e:  # pragma: no cover
                 log.error("Could not invalidate token ({}), rolling back", e)
                 self.db.session.rollback()
                 return False
 
         log.warning("Could not invalidate token")
         return False
 
     def save_login(self, username: str, user: Optional[User], failed: bool) -> None:
-
         date = datetime.now(pytz.utc)
         ip_address = self.get_remote_ip()
 
-        login_data: Dict[str, Any] = {}
+        login_data: dict[str, Any] = {}
 
         login_data["date"] = date
         login_data["username"] = username
         login_data["IP"] = ip_address
         login_data["location"] = "Unknown"
-        # the following two are equivalent
         if user:
-            # login_data["user_id"] = user.id
             login_data["user"] = user
         login_data["failed"] = failed
         # i.e. failed logins are not flushed by default
         # success logins are automatically flushed
         login_data["flushed"] = not failed
 
         login = self.db.Login(**login_data)
@@ -639,39 +617,48 @@
         except Exception as e:  # pragma: no cover
             log.error("DB error ({}), rolling back", e)
             self.db.session.rollback()
             raise
 
     def get_logins(
         self, username: Optional[str] = None, only_unflushed: bool = False
-    ) -> List[Login]:
-
-        if not username:
-            logins = self.db.Login.query.all()
-        elif only_unflushed:
-            logins = self.db.Login.query.filter_by(username=username, flushed=False)
-        else:
-            logins = self.db.Login.query.filter_by(username=username)
-
-        return [x for x in logins]
+    ) -> list[Login]:
+        logins = select(self.db.Login)
+        if username:
+            logins = logins.where(self.db.Login.username == username)
+            if only_unflushed:
+                logins = logins.where(self.db.Login.flushed == False)  # noqa
+        logins_list = list(self.db.session.execute(logins).scalars())
+        # self.db.session.commit()
+        return logins_list
 
     def flush_failed_logins(self, username: str) -> None:
-
-        for login in self.db.Login.query.filter_by(username=username, flushed=False):
+        for login in self.db.session.execute(
+            select(self.db.Login)
+            .where(self.db.Login.username == username)
+            .where(
+                self.db.Login.flushed == False,  # noqa
+            )
+        ).scalars():
             login.flushed = True
             self.db.session.add(login)
 
         self.db.session.commit()
 
 
 instance = SQLAlchemy()
 
 
 def get_instance(
     verification: Optional[int] = None,
     expiration: Optional[int] = None,
+    retries: int = 1,
+    retry_wait: int = 0,
     **kwargs: str,
 ) -> "SQLAlchemy":
-
     return instance.get_instance(
-        verification=verification, expiration=expiration, **kwargs
+        verification=verification,
+        expiration=expiration,
+        retries=retries,
+        retry_wait=retry_wait,
+        **kwargs,
     )
```

### Comparing `rapydo_http-2.4/restapi/customizer.py` & `rapydo_http-3.0/restapi/customizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """
 Base class to let projects to customize core functionalities
 """
+
 import abc
-from typing import Tuple
 
 from flask import Flask
 
 from restapi.connectors import Connector
 from restapi.rest.definition import EndpointResource
 from restapi.services.authentication import User
 from restapi.types import FlaskRequest, Props
 
 FlaskApp = Flask
 
 
 class BaseCustomizer(metaclass=abc.ABCMeta):
-
     # These are scopes used in get_custom_input_fields
     ADMIN = 1
     PROFILE = 2
     REGISTRATION = 3
 
     @staticmethod
     @abc.abstractmethod
     def custom_user_properties_pre(
         properties: Props,
-    ) -> Tuple[Props, Props]:  # pragma: no cover
+    ) -> tuple[Props, Props]:  # pragma: no cover
         """
         executed just before user creation
         use this method to removed or manipulate input properties
         before sending to the database
         """
         return properties, {}
 
@@ -57,15 +56,14 @@
         return data
 
     @staticmethod
     @abc.abstractmethod
     def get_custom_input_fields(
         request: FlaskRequest, scope: int
     ) -> Props:  # pragma: no cover
-
         # required = request and request.method == "POST"
         """
         if scope == BaseCustomizer.ADMIN:
             return {
                 'custom_field': fields.Int(
                     required=required,
                     # validate=validate.Range(min=0, max=???),
```

### Comparing `rapydo_http-2.4/restapi/decorators.py` & `rapydo_http-3.0/restapi/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Decorators used to configure endpoints with metadata, authentication, caching
 , pagination, input validation, output serialization, etc
 """
+
 import inspect
 from functools import wraps
 from typing import (
     Any,
     Callable,
-    Dict,
     Optional,
     Union,
     cast,
     get_args,
     get_origin,
     get_type_hints,
 )
@@ -64,25 +64,24 @@
     )
 
 
 def endpoint(
     path: str,
     summary: Optional[str] = None,
     description: Optional[str] = None,
-    responses: Optional[Dict[Union[str, int], str]] = None,
+    responses: Optional[dict[Union[str, int], str]] = None,
     **kwargs: Any,
 ) -> Callable[[EndpointFunction], EndpointFunction]:
     def decorator(func: EndpointFunction) -> EndpointFunction:
-
-        specs: Dict[str, Any] = {}
+        specs: dict[str, Any] = {}
 
         specs["summary"] = summary
         specs["description"] = description
 
-        specs_responses: Dict[str, Dict[str, str]] = {}
+        specs_responses: dict[str, dict[str, str]] = {}
         if responses:
             for code, message in responses.items():
                 specs_responses[str(code)] = {"description": message}
         specs["responses"] = specs_responses
         if not path.startswith("/"):
             normalized_path = f"/{path}"
         else:
@@ -92,33 +91,32 @@
             AUTH_URL
         ):
             normalized_path = f"{API_URL}{normalized_path}"
 
         if hasattr(func, "uri"):  # pragma: no cover
             print_and_exit(
                 "Unsupported multiple endpoint mapping found: {}, {}",
-                getattr(func, "uri"),
+                func.uri,
                 normalized_path,
             )
 
-        setattr(func, "uri", normalized_path)
+        # "EndpointFunction" has no attribute "uri"
+        func.uri = normalized_path  # type: ignore[attr-defined]
         inject_apispec_docs(func, specs, None)
 
         @wraps(func)
         def wrapper(self: Any, *args: Any, **kwargs: Any) -> EndpointFunction:
-
             return cast(EndpointFunction, func(self, *args, **kwargs))
 
         return cast(EndpointFunction, wrapper)
 
     return decorator
 
 
 def match_types(static_type: Any, runtime_value: Any) -> bool:
-
     # parameters annotated as Any are always accepted, regardless the runtime type
     if static_type == Any:
         return True
 
     if inspect.isclass(runtime_value):
         runtime_type = runtime_value
     else:
@@ -141,28 +139,27 @@
 
     if origin_type == Union:
         return any(
             match_types(arg_type, runtime_value) for arg_type in get_args(static_type)
         )
 
     # TODO: typing.get_args(static_type) is not verified
-    # Ths means that [1] will be accepted as List[str]
+    # This means that [1] will be accepted as List[str]
     return match_types(origin_type, runtime_value)
 
 
 # This function takes as input the callback function signature and extracts from both
 # view_args and kwargs the corresponding parameters to be injected at runtime
 # If the parameter is not found in view_args and kwargs or it is found with a wrong
 # type, then a None is returned and the preload decorator will raise a ServerError
 def inject_callback_parameters(
     callback_fn: Callable[..., Optional[Any]],
-    kwargs: Dict[str, Any],
-    view_args: Optional[Dict[str, Any]],
-) -> Optional[Dict[str, Any]]:
-
+    kwargs: dict[str, Any],
+    view_args: Optional[dict[str, Any]],
+) -> Optional[dict[str, Any]]:
     callback_name = callback_fn.__name__
     parameters = get_type_hints(callback_fn)
 
     if "endpoint" not in parameters:
         log.critical(
             "Missing (endpoint: EndpointResource) parameter in {}", callback_name
         )
@@ -173,15 +170,15 @@
             "Wrong type annotation for parameter 'endpoint' in {}, "
             "expected EndpointResource but found {}",
             callback_name,
             parameters["endpoint"].__name__,
         )
         return None
 
-    injected_parameters: Dict[str, Any] = {}
+    injected_parameters: dict[str, Any] = {}
     for name, parameter in parameters.items():
         # endpoint will be injected by the preload decorator and it is not expected
         # to be found in kwargs / view_args
         if name == "endpoint":
             continue
 
         # This is the annotation of the function return, not needed here
@@ -191,18 +188,17 @@
         if view_args and name in view_args:
             input_param = view_args[name]
 
         elif name in kwargs:
             input_param = kwargs[name]
 
         else:
-
             p = inspect.signature(callback_fn).parameters[name]
             # Parameter is missing but it has a default value, so can be safely skipped
-            if p.default is not p.empty:
+            if p.default is not p.empty:  # pragma: no cover
                 continue
 
             log.critical(
                 "Parameter ({}:{}) in {} isn't found and can't be injected",
                 name,
                 parameters[name],
                 callback_name,
@@ -226,21 +222,21 @@
 
 
 # The callback is expected to have a first argument of type EndpointResource and then
 # optional additional parameters automatically injected from kwargs and url parameters
 # I can't define with mypy something like:
 # Callable[[EndpointResource, ...],
 def preload(
-    callback: Callable[..., Dict[str, Any]]
+    callback: Callable[..., dict[str, Any]]
 ) -> Callable[[EndpointFunction], EndpointFunction]:
     """
     callback example:
 
     from flask import request
-    def myfunc(endpoint: EndpointResource, user: User) -> Dict[str, Any]:
+    def myfunc(endpoint: EndpointResource, user: User) -> dict[str, Any]:
 
         if (
             not user
             or not request.view_args
             or request.view_args.get("uuid") != user.uuid
         ):
             raise Unauthorized("You are not authorized")
@@ -250,15 +246,14 @@
         # Otherwise can simply return None to inject nothing
         # return None
     """
 
     def decorator(func: EndpointFunction) -> EndpointFunction:
         @wraps(func)
         def wrapper(self: Any, *args: Any, **kwargs: Any) -> Any:
-
             injected_parameters = inject_callback_parameters(
                 callback, kwargs, request.view_args
             )
             if injected_parameters is None:  # pragma: no cover
                 raise ServerError("Invalid endpoint signature")
 
             # callback can raise exceptions to stop che execution and e.g. implement
@@ -271,68 +266,75 @@
             return func(self, *args, **kwargs)
 
         return cast(EndpointFunction, wrapper)
 
     return decorator
 
 
-# Prevent caching of 5xx errors responses
 def cache_response_filter(response: Response) -> bool:
+    """
+    Prevent caching of 5xx errors responses
+    """
     if not isinstance(response, tuple):
         return True
 
     if len(response) < 3:  # pragma: no cover
-        return True
+        return True  # type: ignore[unreachable]
 
     return response[1] < 500
 
 
-# This is used to manipulate the function name to append a string depending
-# by the Bearer token. This way all cache entries for authenticated endpoints
-# will always user-dependent.
 def make_cache_function_name(name: str) -> str:
-
+    """
+    This is used to manipulate the function name to append a string depending
+    by the Bearer token. This way all cache entries for authenticated endpoints
+    will always user-dependent.
+    """
     # Non authenticated endpoints do not validate the token.
     # Function name is not expanded by any token that could be provided (are ignored)
     if not request.environ.get(TOKEN_VALIDATED_KEY):
         return name
 
     # If the token is validated, the function name is expanded by a token-dependent key
     token = auth.get_authorization_token(allow_access_token_parameter=True)
     new_name = f"{name}-{hash(token)}"
     return new_name
 
 
-# Used to cache endpoint with @decorators.cache(timeout=60)
 def cache(*args: Any, **kwargs: Any) -> Any:
+    """
+    Used to cache endpoint with @decorators.cache(timeout=60)
+    """
     if "response_filter" not in kwargs:
         kwargs["response_filter"] = cache_response_filter
     if "make_name" not in kwargs:
         kwargs["make_name"] = make_cache_function_name
+
+    if not hasattr(mem, "cache"):
+        print_and_exit("Cannot load @decorators.cache, is Redis connector available?")
+
     return mem.cache.memoize(*args, **kwargs)
 
 
 def database_transaction(func: EndpointFunction) -> EndpointFunction:
     @wraps(func)
     def wrapper(self: Any, *args: Any, **kwargs: Any) -> Any:
-
         neo4j_enabled = Connector.check_availability("neo4j")
         sqlalchemy_enabled = Connector.check_availability("sqlalchemy")
         if neo4j_enabled:
             from neomodel import db as neo4j_db
 
         if sqlalchemy_enabled:
             # thanks to connectors cache this should always match the
             # same instance that will be used from inside the endpoint
             from restapi.connectors import sqlalchemy
 
             alchemy_db = sqlalchemy.get_instance()
 
         try:
-
             if neo4j_enabled:
                 neo4j_db.begin()
 
             # Transaction is already open...
             # if sqlalchemy_enabled:
             #     pass
 
@@ -344,15 +346,14 @@
             if sqlalchemy_enabled:
                 alchemy_db.session.commit()
 
             return out
         except Exception as e:
             log.debug("Rolling backend database transaction")
             try:
-
                 if neo4j_enabled:
                     neo4j_db.rollback()
 
                 if sqlalchemy_enabled:
                     alchemy_db.session.rollback()
 
             except Exception as sub_ex:  # pragma: no cover
@@ -380,15 +381,15 @@
     sort_order = fields.Str(
         validate=validate.OneOf(["asc", "desc"]), required=False, load_default="asc"
     )
     sort_by = fields.Str(required=False, load_default=None)
     input_filter = fields.Str(required=False, load_default=None)
 
     @post_load
-    def verify_parameters(self, data: Dict[str, Any], **kwargs: Any) -> Dict[str, Any]:
+    def verify_parameters(self, data: dict[str, Any], **kwargs: Any) -> dict[str, Any]:
         if "get_total" in data:
             data["page"] = None
             data["size"] = None
         else:
             data.setdefault("get_total", False)
             data.setdefault("page", 1)
             data.setdefault("size", 20)
@@ -398,23 +399,21 @@
 
 def get_pagination(func: EndpointFunction) -> EndpointFunction:
     @wraps(func)
     # Should be converted in use_args, if/when available
     # https://github.com/jmcarp/flask-apispec/issues/189
     @use_kwargs(Pagination, location="query")
     def get_wrapper(self: Any, *args: Any, **kwargs: Any) -> Any:
-
         return func(self, *args, **kwargs)
 
     @wraps(func)
     # Should be converted in use_args, if/when available
     # https://github.com/jmcarp/flask-apispec/issues/189
     @use_kwargs(Pagination)
     def wrapper(self: Any, *args: Any, **kwargs: Any) -> Any:
-
         return func(self, *args, **kwargs)
 
     if func.__name__ == "get":
         return cast(EndpointFunction, get_wrapper)
     return cast(EndpointFunction, wrapper)
 
 
@@ -427,15 +426,14 @@
 
 def init_chunk_upload(func: EndpointFunction) -> EndpointFunction:
     @wraps(func)
     # Should be converted in use_args, if/when available
     # https://github.com/jmcarp/flask-apispec/issues/189
     @use_kwargs(ChunkUpload)
     def wrapper(self: Any, *args: Any, **kwargs: Any) -> Any:
-
         return func(self, *args, **kwargs)
 
     return cast(EndpointFunction, wrapper)
 
 
 # This decorator is automatically added to every endpoints... do not use it explicitly
 def catch_exceptions(**kwargs: Any) -> Callable[[EndpointFunction], EndpointFunction]:
@@ -449,15 +447,14 @@
         def wrapper(self: Any, *args: Any, **kwargs: Any) -> Any:
             out = None
 
             try:
                 out = func(self, *args, **kwargs)
             # Catch the exception requested by the user
             except RestApiException as e:
-
                 if e.is_warning:
                     log.warning(e)
                 else:
                     log.exception(e)
                     log.error(e)
 
                 return self.response(
@@ -482,32 +479,31 @@
 
             # errors with RabbitMQ credentials raised when sending Celery tasks
             except AccessRefused as e:  # pragma: no cover
                 log.error(e)
                 return self.response(
                     "Unexpected Server Error", code=500, force_json=True
                 )
-            except Exception as e:
-
-                if SENTRY_URL is not None:  # pragma: no cover
+            except Exception as e:  # pragma: no cover
+                if SENTRY_URL is not None:
                     capture_exception(e)
 
                 excname = e.__class__.__name__
                 message = str(e)
                 if not message:  # pragma: no cover
                     message = "Unknown error"
 
                 error_id = getUUID()
 
                 log.error(
                     "Catched {} exception with ID {}: {}", excname, error_id, message
                 )
                 log.exception(message)
 
-                if excname in ["SystemError"]:  # pragma: no cover
+                if excname in ["SystemError"]:
                     return self.response(
                         "Unexpected Server Error", code=500, force_json=True
                     )
 
                 return self.response(
                     {excname: f"There was an unexpected error. ErrorID: {error_id}"},
                     code=400,
```

### Comparing `rapydo_http-2.4/restapi/endpoints/admin_groups.py` & `rapydo_http-3.0/restapi/endpoints/admin_groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-from typing import Any, Dict, List
+from typing import Any
 
 from restapi import decorators
-from restapi.connectors import Connector
 from restapi.endpoints.schemas import GroupWithMembers, admin_group_input
-from restapi.exceptions import NotFound
+from restapi.exceptions import Forbidden, NotFound
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import Group, Role, User
 
 
-def inject_group(endpoint: EndpointResource, group_id: str) -> Dict[str, Any]:
-
+def inject_group(endpoint: EndpointResource, group_id: str) -> dict[str, Any]:
     group = endpoint.auth.get_group(group_id=group_id)
     if not group:
         raise NotFound("This group cannot be found")
 
     return {"group": group}
 
 
 class AdminGroups(EndpointResource):
-
     depends_on = ["AUTH_ENABLE"]
     labels = ["management"]
     private = True
 
     @decorators.auth.require_any(Role.ADMIN, Role.STAFF)
     @decorators.marshal_with(GroupWithMembers(many=True), code=200)
     @decorators.endpoint(
@@ -30,20 +27,18 @@
         summary="List of groups",
         responses={
             200: "List of groups successfully retrieved",
             409: "Request is invalid due to conflicts",
         },
     )
     def get(self, user: User) -> Response:
-
-        groups: List[Dict[str, Any]] = []
+        groups: list[dict[str, Any]] = []
 
         is_admin = self.auth.is_admin(user)
         for g in self.auth.get_groups():
-
             members = list(g.members)
 
             coordinators = [
                 u
                 for u in members
                 if self.auth.is_coordinator(u)
                 and (is_admin or not self.auth.is_admin(u))
@@ -69,15 +64,14 @@
         summary="Create a new group",
         responses={
             200: "The uuid of the new group is returned",
             409: "Request is invalid due to conflicts",
         },
     )
     def post(self, user: User, **kwargs: Any) -> Response:
-
         group = self.auth.create_group(kwargs)
 
         self.auth.save_group(group)
 
         self.log_event(self.events.create, group, kwargs)
         return self.response(group.uuid)
 
@@ -87,15 +81,14 @@
     @decorators.use_kwargs(admin_group_input)
     @decorators.endpoint(
         path="/admin/groups/<group_id>",
         summary="Modify a group",
         responses={204: "Group successfully modified", 404: "Group not found"},
     )
     def put(self, group_id: str, group: Group, user: User, **kwargs: Any) -> Response:
-
         # mypy correctly raises errors because update_properties is not defined
         # in generic Connector instances, but in this case this is an instance
         # of an auth db and their implementation always contains this method
         self.auth.db.update_properties(group, kwargs)  # type: ignore
 
         self.auth.save_group(group)
 
@@ -107,13 +100,17 @@
     @decorators.preload(callback=inject_group)
     @decorators.endpoint(
         path="/admin/groups/<group_id>",
         summary="Delete a group",
         responses={204: "Group successfully deleted", 404: "Group not found"},
     )
     def delete(self, group_id: str, group: Group, user: User) -> Response:
+        if members := self.auth.get_group_members(group):
+            raise Forbidden(
+                f"Cannot delete this group, it is assigned to {len(members)} user(s)"
+            )
 
         self.auth.delete_group(group)
 
         self.log_event(self.events.delete, group)
 
         return self.empty_response()
```

### Comparing `rapydo_http-2.4/restapi/endpoints/admin_logins.py` & `rapydo_http-3.0/restapi/endpoints/admin_logins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from restapi import decorators
 from restapi.endpoints.schemas import LoginsSchema
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import Role, User
 
 
 class AdminLogins(EndpointResource):
-
     depends_on = ["MAIN_LOGIN_ENABLE", "AUTH_ENABLE"]
     labels = ["management"]
     private = True
 
     @decorators.auth.require_all(Role.ADMIN)
     @decorators.marshal_with(LoginsSchema(many=True), code=200)
     @decorators.endpoint(
         path="/admin/logins",
         summary="Retrieve logins information",
         responses={"200": "Logins data retrieved"},
     )
     def get(self, user: User) -> Response:
-
         logins = self.auth.get_logins(username=None, only_unflushed=False)
         return self.response(logins)
```

### Comparing `rapydo_http-2.4/restapi/endpoints/admin_server_stats.py` & `rapydo_http-3.0/restapi/endpoints/admin_server_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,26 @@
 from restapi import decorators
 from restapi.endpoints.schemas import StatsSchema, StatsType
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import Role, User
 
 
 class AdminStats(EndpointResource):
-
     labels = ["helpers"]
     depends_on = ["AUTH_ENABLE"]
     private = True
 
     @decorators.auth.require_all(Role.ADMIN)
     @decorators.marshal_with(StatsSchema(), code=200)
     @decorators.endpoint(
         path="/admin/stats",
         summary="Retrieve stats from the server",
         responses={"200": "Stats retrieved"},
     )
     def get(self, user: User) -> Response:
-
         # This is the average system load calculated over a given period of time
         # of 1, 5 and 15 minutes.
         # In our case, we will show the load average over a period of 15 minutes.
         # The numbers returned by os.getloadavg() only make sense if
         # related to the number of CPU cores installed on the system.
 
         # Here we are converting the load average into percentage.
```

### Comparing `rapydo_http-2.4/restapi/endpoints/admin_tokens.py` & `rapydo_http-3.0/restapi/endpoints/admin_tokens.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from typing import Any, Dict
+from typing import Any
 
 from glom import glom
 
 from restapi import decorators
 from restapi.endpoints.schemas import TokenAdminSchema, TotalSchema
 from restapi.exceptions import BadRequest, NotFound
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import Role, Token, User
 from restapi.utilities.logs import log
 
 
-def inject_token(endpoint: EndpointResource, token_id: str) -> Dict[str, Any]:
-
+def inject_token(endpoint: EndpointResource, token_id: str) -> dict[str, Any]:
     tokens = endpoint.auth.get_tokens(token_jti=token_id)
 
     if not tokens:
         raise NotFound("This token does not exist")
 
     return {"token": tokens[0]["token"]}
 
@@ -45,15 +44,14 @@
         page: int,
         size: int,
         sort_by: str,
         sort_order: str,
         input_filter: str,
         user: User,
     ) -> Response:
-
         tokens = self.auth.get_tokens(get_all=True)
 
         if input_filter:
             filtered_tokens = []
             for t in tokens:
                 token = t.get("token", "").lower()
                 ip = t.get("IP", "").lower()
@@ -106,12 +104,11 @@
         responses={
             204: "Token has been invalidated",
             404: "Specified token cannot be found",
             400: "Token invalidation is failed",
         },
     )
     def delete(self, token_id: str, token: str, user: User) -> Response:
-
         if not self.auth.invalidate_token(token=token):
             raise BadRequest(f"Failed token invalidation: {token}")  # pragma: no cover
 
         return self.empty_response()
```

### Comparing `rapydo_http-2.4/restapi/endpoints/admin_users.py` & `rapydo_http-3.0/restapi/endpoints/admin_users.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List
+from typing import Any
 
 from restapi import decorators
 from restapi.connectors.smtp.notifications import (
     notify_new_credentials_to_user,
     notify_update_credentials_to_user,
 )
 from restapi.endpoints.schemas import (
@@ -14,16 +14,15 @@
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import BaseAuthentication, Role, User
 from restapi.utilities.time import date_lower_than as dt_lower
 
 # from restapi.utilities.logs import log
 
 
-def inject_user(endpoint: EndpointResource, user_id: str, user: User) -> Dict[str, Any]:
-
+def inject_user(endpoint: EndpointResource, user_id: str, user: User) -> dict[str, Any]:
     target_user = endpoint.auth.get_user(user_id=user_id)
     if target_user is None:
         raise NotFound("This user cannot be found or you are not authorized")
 
     # Non admins (i.e. Staff users) are not allowed to target Admins
     if endpoint.auth.is_admin(target_user) and not endpoint.auth.is_admin(user):
         raise NotFound("This user cannot be found or you are not authorized")
@@ -41,35 +40,32 @@
     @decorators.marshal_with(admin_user_output(many=False), code=200)
     @decorators.endpoint(
         path="/admin/users/<user_id>",
         summary="Return information on a single user",
         responses={200: "User information successfully retrieved"},
     )
     def get(self, user_id: str, target_user: User, user: User) -> Response:
-
         self.log_event(self.events.access, target_user)
 
         return self.response(target_user)
 
 
 class AdminUsers(EndpointResource):
-
     depends_on = ["MAIN_LOGIN_ENABLE", "AUTH_ENABLE"]
     labels = ["management"]
     private = True
 
     @decorators.auth.require_any(Role.ADMIN, Role.STAFF)
     @decorators.marshal_with(admin_user_output(many=True), code=200)
     @decorators.endpoint(
         path="/admin/users",
         summary="Return the list of all defined users",
         responses={200: "List of users successfully retrieved"},
     )
     def get(self, user: User) -> Response:
-
         users = self.auth.get_users()
 
         # Filter out admin users when requested from a Staff user
         if not self.auth.is_admin(user):
             users = [
                 u
                 for u in users
@@ -86,16 +82,15 @@
         summary="Create a new user",
         responses={
             200: "The uuid of the new user is returned",
             409: "This user already exists",
         },
     )
     def post(self, user: User, **kwargs: Any) -> Response:
-
-        roles: List[str] = kwargs.pop("roles", [])
+        roles: list[str] = kwargs.pop("roles", [])
 
         # The role is already refused by webards... This is an additional check
         # to improve the security, but can't be reached
         if not self.auth.is_admin(user) and Role.ADMIN in roles:  # pragma: no cover
             raise Forbidden("This role is not allowed")
 
         payload = kwargs.copy()
@@ -104,22 +99,22 @@
         email_notification = kwargs.pop("email_notification", False)
 
         unhashed_password = kwargs["password"]
 
         # If created by admins users must accept privacy at first login
         kwargs["privacy_accepted"] = False
 
-        user = self.auth.create_user(kwargs, roles)
-        self.auth.save_user(user)
-
         group = self.auth.get_group(group_id=group_id)
         if not group:
             # Can't be reached because group_id is prefiltered by marshmallow
             raise NotFound("This group cannot be found")  # pragma: no cover
 
+        user = self.auth.create_user(kwargs, roles, group)
+        self.auth.save_user(user)
+
         self.auth.add_user_to_group(user, group)
 
         if email_notification and unhashed_password is not None:
             notify_new_credentials_to_user(user, unhashed_password)
 
         self.log_event(self.events.create, user, payload)
 
@@ -133,25 +128,24 @@
         path="/admin/users/<user_id>",
         summary="Modify a user",
         responses={200: "User successfully modified"},
     )
     def put(
         self, user_id: str, target_user: User, user: User, **kwargs: Any
     ) -> Response:
-
         if "password" in kwargs:
             unhashed_password = kwargs["password"]
             kwargs["password"] = BaseAuthentication.get_password_hash(
                 kwargs["password"]
             )
         else:
             unhashed_password = None
 
         payload = kwargs.copy()
-        roles: List[str] = kwargs.pop("roles", [])
+        roles: list[str] = kwargs.pop("roles", [])
 
         # The role is already refused by webards... This is an additional check
         # to improve the security, but can't be reached
         if not self.auth.is_admin(user) and Role.ADMIN in roles:  # pragma: no cover
             raise Forbidden("This role is not allowed")
 
         group_id = kwargs.pop("group", None)
@@ -207,13 +201,12 @@
     @decorators.preload(callback=inject_user)
     @decorators.endpoint(
         path="/admin/users/<user_id>",
         summary="Delete a user",
         responses={200: "User successfully deleted"},
     )
     def delete(self, user_id: str, target_user: User, user: User) -> Response:
-
         self.auth.delete_user(target_user)
 
         self.log_event(self.events.delete, target_user)
 
         return self.empty_response()
```

### Comparing `rapydo_http-2.4/restapi/endpoints/group_users.py` & `rapydo_http-3.0/restapi/endpoints/group_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from restapi import decorators
 from restapi.endpoints.schemas import group_users_output
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import Role, User
 
 
 class GroupUsers(EndpointResource):
-
     depends_on = ["MAIN_LOGIN_ENABLE", "AUTH_ENABLE"]
     labels = ["management"]
 
     @decorators.auth.require_all(Role.COORDINATOR)
     @decorators.marshal_with(group_users_output(), code=200)
     @decorators.endpoint(
         path="/group/users",
         summary="List of users of your group",
         description="This endpoint is restricted to Group Coordinators",
         responses={
             200: "List of users successfully retrieved",
         },
     )
     def get(self, user: User) -> Response:
-
         group = self.auth.get_user_group(user)
 
         members = self.auth.get_group_members(group)
 
         if self.auth.is_admin(user):
             return self.response(members)
```

### Comparing `rapydo_http-2.4/restapi/endpoints/login.py` & `rapydo_http-3.0/restapi/endpoints/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         self,
         username: str,
         password: str,
         new_password: Optional[str] = None,
         password_confirm: Optional[str] = None,
         totp_code: Optional[str] = None,
     ) -> Response:
-
         username = username.lower()
         if not self.auth.SECOND_FACTOR_AUTHENTICATION:
             totp_code = None
 
         # ##################################################
         # Authentication control
 
@@ -54,29 +53,28 @@
             message["errors"].append("You do not provided a valid verification code")
             if message["errors"]:
                 return self.response(message, code=403)
 
         # ##################################################
         # If requested, change the password
         if new_password is not None and password_confirm is not None:
-
             pwd_changed = self.auth.change_password(
                 user, password, new_password, password_confirm
             )
 
             if pwd_changed:
                 password = new_password
                 token, payload, user = self.auth.make_login(
                     username, password, totp_code
                 )
 
         message = self.auth.check_password_validity(
             user, totp_authentication=self.auth.SECOND_FACTOR_AUTHENTICATION
         )
-        if message["errors"]:
+        if message["errors"]:  # pragma: no cover
             return self.response(message, code=403)
 
         # Everything is ok, let's save authentication information
 
         now = datetime.now(pytz.utc)
         if user.first_login is None:
             user.first_login = now
```

### Comparing `rapydo_http-2.4/restapi/endpoints/login_unlock.py` & `rapydo_http-3.0/restapi/endpoints/login_unlock.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This endpoint validates an UNLOCK token to re-enable credentials
 after a block due to too many failed attemps.
 Unlock URL (including token) is sent by email
 """
+
 from jwt.exceptions import ExpiredSignatureError, ImmatureSignatureError
 
 from restapi import decorators
 from restapi.exceptions import BadRequest
 from restapi.rest.definition import EndpointResource, Response
 from restapi.utilities.logs import log
 
@@ -21,37 +22,36 @@
         description="The unlock sent by email is validated here to restore credentials",
         responses={
             200: "Credentials are now unlocked",
             400: "Invalid token",
         },
     )
     def post(self, token: str) -> Response:
-
         token = token.replace("%2B", ".")
         token = token.replace("+", ".")
 
         try:
             # valid, token, jti, user
             _, _, jti, user = self.auth.verify_token(
                 token, raiseErrors=True, token_type=self.auth.UNLOCK_CREDENTIALS
             )
 
         # If token is expired
-        except ExpiredSignatureError:
+        except ExpiredSignatureError as e:
             raise BadRequest(
                 "Invalid unlock token: this request is expired",
-            )
+            ) from e
 
         # if token is not active yet
-        except ImmatureSignatureError:
-            raise BadRequest("Invalid unlock token")
+        except ImmatureSignatureError as e:
+            raise BadRequest("Invalid unlock token") from e
 
         # if token does not exist (or other generic errors)
-        except Exception:
-            raise BadRequest("Invalid unlock token")
+        except Exception as e:
+            raise BadRequest("Invalid unlock token") from e
 
         if user is None:  # pragma: no cover
             raise BadRequest("Invalid unlock token")
 
         # Recovering token object from jti
         token_obj = self.auth.get_tokens(token_jti=jti)
         # Cannot be tested, this is an extra test to prevent any unauthorized access...
```

### Comparing `rapydo_http-2.4/restapi/endpoints/logout.py` & `rapydo_http-3.0/restapi/endpoints/logout.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,13 +13,12 @@
     @decorators.endpoint(
         path="/auth/logout",
         summary="Logout and invalidate the current token",
         description="Invalidate current registered token",
         responses={204: "Token correctly removed"},
     )
     def get(self, user: User) -> Response:
-
         _, token = decorators.auth.get_authorization_token()
         if token:
             self.auth.invalidate_token(token)
         self.log_event(self.events.logout)
         return self.empty_response()
```

### Comparing `rapydo_http-2.4/restapi/endpoints/profile.py` & `rapydo_http-3.0/restapi/endpoints/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,25 @@
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import AuthMissingTOTP, User
 from restapi.utilities.globals import mem
 from restapi.utilities.logs import log
 
 
 class Profile(EndpointResource):
-
     depends_on = ["MAIN_LOGIN_ENABLE", "AUTH_ENABLE"]
     labels = ["profile"]
 
     @decorators.auth.require()
     @decorators.marshal_with(profile_output(), code=200)
     @decorators.endpoint(
         path="/auth/profile",
         summary="List profile attributes",
         responses={200: "User profile is returned"},
     )
     def get(self, user: User) -> Response:
-
         data = {
             "uuid": user.uuid,
             "email": user.email,
             "name": user.name,
             "surname": user.surname,
             "isAdmin": self.auth.is_admin(user),
             "isStaff": self.auth.is_staff(user),
@@ -58,19 +56,18 @@
         self,
         password: str,
         new_password: str,
         password_confirm: str,
         user: User,
         totp_code: Optional[str] = None,
     ) -> Response:
-
         try:
             self.auth.make_login(user.email, password, totp_code)
-        except AuthMissingTOTP:
-            raise Unauthorized("Verification code is missing")
+        except AuthMissingTOTP as e:
+            raise Unauthorized("Verification code is missing") from e
 
         self.auth.change_password(user, password, new_password, password_confirm)
 
         self.auth.save_user(user)
 
         return self.empty_response()
```

### Comparing `rapydo_http-2.4/restapi/endpoints/profile_activation.py` & `rapydo_http-3.0/restapi/endpoints/profile_activation.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,37 +21,36 @@
         responses={
             200: "Account successfully activated",
             400: "Invalid token",
             403: "Account temporarily blocked due to the number of failed logins",
         },
     )
     def put(self, token: str) -> Response:
-
         token = token.replace("%2B", ".")
         token = token.replace("+", ".")
 
         try:
             # valid, token, jti, user
             _, _, jti, user = self.auth.verify_token(
                 token, raiseErrors=True, token_type=self.auth.ACTIVATE_ACCOUNT
             )
 
         # If token is expired
-        except ExpiredSignatureError:
+        except ExpiredSignatureError as e:
             raise BadRequest(
                 "Invalid activation token: this request is expired",
-            )
+            ) from e
 
         # if token is not active yet
-        except ImmatureSignatureError:
-            raise BadRequest("Invalid activation token")
+        except ImmatureSignatureError as e:
+            raise BadRequest("Invalid activation token") from e
 
         # if token does not exist (or other generic errors)
-        except Exception:
-            raise BadRequest("Invalid activation token")
+        except Exception as e:
+            raise BadRequest("Invalid activation token") from e
 
         if user is None:  # pragma: no cover
             raise BadRequest("Invalid activation token")
 
         self.auth.verify_blocked_username(user.email)
 
         # Recovering token object from jti
@@ -87,23 +86,21 @@
         summary="Ask a new activation link",
         responses={
             200: "A new activation link has been sent",
             403: "Account temporarily blocked due to the number of failed logins",
         },
     )
     def post(self, username: str) -> Response:
-
         self.auth.verify_blocked_username(username)
 
         user = self.auth.get_user(username=username)
 
         # if user is None this endpoint does nothing but the response
         # remain the same to prevent any user guessing
         if user is not None:
-
             auth = Connector.get_authentication_instance()
 
             activation_token, payload = auth.create_temporary_token(
                 user, auth.ACTIVATE_ACCOUNT
             )
 
             server_url = get_frontend_url()
```

### Comparing `rapydo_http-2.4/restapi/endpoints/profile_registration.py` & `rapydo_http-3.0/restapi/endpoints/profile_registration.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from restapi.services.authentication import DEFAULT_GROUP_NAME
 from restapi.utilities.logs import log
 
 # This endpoint needs to send the activation token via email
 if Connector.check_availability("smtp"):
 
     class ProfileRegistration(EndpointResource):
-
         depends_on = ["MAIN_LOGIN_ENABLE", "ALLOW_REGISTRATION", "AUTH_ENABLE"]
         labels = ["profile"]
 
         @decorators.use_kwargs(user_registration_input)
         @decorators.endpoint(
             path="/auth/profile",
             summary="Register new user",
@@ -61,24 +60,21 @@
                 raise Conflict(msg)
 
             kwargs["name"] = name
             kwargs["surname"] = surname
             kwargs["email"] = email
             kwargs["password"] = password
             kwargs["is_active"] = False
-            user = self.auth.create_user(kwargs, [self.auth.default_role])
-
-            default_group = self.auth.get_group(name=DEFAULT_GROUP_NAME)
-            self.auth.add_user_to_group(user, default_group)
+            group = self.auth.get_group(name=DEFAULT_GROUP_NAME)
+            user = self.auth.create_user(kwargs, [self.auth.default_role], group)
             self.auth.save_user(user)
 
             self.log_event(self.events.create, user, kwargs)
 
             try:
-
                 auth = Connector.get_authentication_instance()
 
                 activation_token, payload = auth.create_temporary_token(
                     user, auth.ACTIVATE_ACCOUNT
                 )
 
                 server_url = get_frontend_url()
@@ -97,13 +93,15 @@
 
                 # Sending an email to the administrator
                 if Env.get_bool("REGISTRATION_NOTIFICATIONS"):
                     send_registration_notification(user)
 
             except Exception as e:  # pragma: no cover
                 self.auth.delete_user(user)
-                raise ServiceUnavailable(f"Errors during account registration: {e}")
+                raise ServiceUnavailable(
+                    f"Errors during account registration: {e}"
+                ) from e
 
             return self.response(
                 "We are sending an email to your email address where "
                 "you will find the link to activate your account"
             )
```

### Comparing `rapydo_http-2.4/restapi/endpoints/reset_password.py` & `rapydo_http-3.0/restapi/endpoints/reset_password.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 auth = Connector.get_authentication_instance()
 
 
 # This endpoint require the server to send the reset token via email
 if Connector.check_availability("smtp"):
 
     class RecoverPassword(EndpointResource):
-
         depends_on = ["MAIN_LOGIN_ENABLE", "ALLOW_PASSWORD_RESET", "AUTH_ENABLE"]
         labels = ["authentication"]
 
         @decorators.use_kwargs({"reset_email": fields.Email(required=True)})
         @decorators.endpoint(
             path="/auth/reset",
             summary="Request password reset via email",
@@ -31,15 +30,14 @@
             responses={
                 200: "Reset email is valid",
                 400: "Invalid reset email",
                 403: "Account not found or already active",
             },
         )
         def post(self, reset_email: str) -> Response:
-
             reset_email = reset_email.lower()
 
             self.auth.verify_blocked_username(reset_email)
 
             user = self.auth.get_user(username=reset_email)
 
             if user is None:
@@ -102,36 +100,35 @@
         )
         def put(
             self,
             token: str,
             new_password: Optional[str] = None,
             password_confirm: Optional[str] = None,
         ) -> Response:
-
             token = token.replace("%2B", ".")
             token = token.replace("+", ".")
 
             try:
                 # valid, token, jti, user
                 _, _, jti, user = self.auth.verify_token(
                     token, raiseErrors=True, token_type=self.auth.PWD_RESET
                 )
 
             # If token is expired
-            except jwt.exceptions.ExpiredSignatureError:
-                raise BadRequest("Invalid reset token: this request is expired")
+            except jwt.exceptions.ExpiredSignatureError as e:
+                raise BadRequest("Invalid reset token: this request is expired") from e
 
             # if token is not active yet
             except jwt.exceptions.ImmatureSignatureError as e:
                 log.info(e)
-                raise BadRequest("Invalid reset token")
+                raise BadRequest("Invalid reset token") from e
             # if token does not exist (or other generic errors)
             except Exception as e:
                 log.info(e)
-                raise BadRequest("Invalid reset token")
+                raise BadRequest("Invalid reset token") from e
 
             if user is None:  # pragma: no cover
                 raise BadRequest("Invalid activation token")
 
             # Recovering token object from jti
             tokens_obj = self.auth.get_tokens(token_jti=jti)
             # Can't happen because the token is refused from verify_token function
@@ -147,15 +144,14 @@
                 last_change = user.last_login
             # If user changed the pwd after the token emission invalidate the token
             # Can't happen because the change password also invalidated the token
             elif user.last_password_change is not None:  # pragma: no cover
                 last_change = user.last_password_change
 
             if last_change is not None:
-
                 # Can't happen because the change password also invalidated the token
                 if last_change > emitted:  # pragma: no cover
                     self.auth.invalidate_token(token)
                     raise BadRequest(
                         "Invalid reset token: this request is no longer valid",
                     )
```

### Comparing `rapydo_http-2.4/restapi/endpoints/schemas.py` & `rapydo_http-3.0/restapi/endpoints/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from datetime import datetime
-from typing import Dict, Type, TypedDict, Union
+from typing import TypedDict, Union
 
 from restapi.connectors import Connector
 from restapi.customizer import FlaskRequest
 from restapi.models import ISO8601UTC, Schema, fields, validate
 from restapi.rest.bearer import HTTPTokenAuth
 from restapi.services.authentication import Role as RoleEnum
 from restapi.utilities.globals import mem
 
 auth = Connector.get_authentication_instance()
 
 # as defined in Marshmallow.schema.from_dict
-MarshmallowSchema = Dict[str, Union[fields.Field, type]]
+MarshmallowSchema = dict[str, Union[fields.Field, type]]
 
 #########################################
 # #############   Schemas   #############
 #########################################
 
 
 class User(Schema):
@@ -215,16 +215,15 @@
 
     schema = Schema.from_dict(attributes, name="UserData")
     return schema(many=True)  # type: ignore
 
 
 # Can't use request.method because it is not passed at loading time, i.e. the Specs will
 # be created with empty request
-def admin_user_input(request: FlaskRequest, is_post: bool) -> Type[Schema]:
-
+def admin_user_input(request: FlaskRequest, is_post: bool) -> type[Schema]:
     is_admin = HTTPTokenAuth.is_session_user_admin(request, auth)
 
     attributes: MarshmallowSchema = {}
     if is_post:
         attributes["email"] = fields.Email(
             required=is_post, validate=validate.Length(max=100)
         )
@@ -313,25 +312,24 @@
         request=request, scope=mem.customizer.ADMIN
     ):
         attributes.update(custom_fields)
 
     return Schema.from_dict(attributes, name="UserDefinition")
 
 
-def admin_user_post_input(request: FlaskRequest) -> Type[Schema]:
+def admin_user_post_input(request: FlaskRequest) -> type[Schema]:
     return admin_user_input(request, True)
 
 
-def admin_user_put_input(request: FlaskRequest) -> Type[Schema]:
+def admin_user_put_input(request: FlaskRequest) -> type[Schema]:
     return admin_user_input(request, False)
 
 
 # Should to transformed again in a Schema
-def admin_group_input(request: FlaskRequest) -> Type[Schema]:
-
+def admin_group_input(request: FlaskRequest) -> type[Schema]:
     attributes: MarshmallowSchema = {}
 
     attributes["shortname"] = fields.Str(
         required=True, metadata={"description": "Short name"}
     )
     attributes["fullname"] = fields.Str(
         required=True, metadata={"description": "Full name"}
@@ -388,16 +386,15 @@
     if custom_fields := mem.customizer.get_custom_output_fields(None):
         attributes.update(custom_fields)
 
     schema = Schema.from_dict(attributes, name="UserProfile")
     return schema()  # type: ignore
 
 
-def user_registration_input(request: FlaskRequest) -> Type[Schema]:
-
+def user_registration_input(request: FlaskRequest) -> type[Schema]:
     attributes: MarshmallowSchema = {}
 
     attributes["name"] = fields.Str(required=True)
     attributes["surname"] = fields.Str(required=True)
     attributes["email"] = fields.Email(
         required=True,
         metadata={"label": "Username (email address)"},
```

### Comparing `rapydo_http-2.4/restapi/endpoints/send_mail.py` & `rapydo_http-3.0/restapi/endpoints/send_mail.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Optional
 
 from restapi import decorators
 from restapi.connectors import smtp
 from restapi.connectors.smtp.notifications import _get_html_template, convert_html2text
 from restapi.endpoints.schemas import MailInput, MailOutput
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import Role, User
 
 # from restapi.utilities.logs import log
 
 
 class SendMail(EndpointResource):
-
     depends_on = ["AUTH_ENABLE"]
     labels = ["management"]
     private = True
 
     @decorators.auth.require_all(Role.ADMIN)
     @decorators.use_kwargs(MailInput)
     @decorators.marshal_with(MailOutput, code=200)
@@ -26,20 +25,19 @@
     )
     def post(
         self,
         user: User,
         subject: str,
         body: str,
         to: str,
-        cc: Optional[List[str]] = None,
-        bcc: Optional[List[str]] = None,
+        cc: Optional[list[str]] = None,
+        bcc: Optional[list[str]] = None,
         dry_run: bool = False,
     ) -> Response:
-
-        replaces: Dict[str, Any] = {}
+        replaces: dict[str, Any] = {}
 
         header_html = _get_html_template("email_header.html", replaces)
         footer_html = _get_html_template("email_footer.html", replaces)
 
         body = body.replace("\n", "<br/>")
 
         html_body = f"{header_html}{body}{footer_html}"
```

### Comparing `rapydo_http-2.4/restapi/endpoints/status.py` & `rapydo_http-3.0/restapi/endpoints/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 from restapi import decorators
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import User
 
 
 class Status(EndpointResource):
-
     labels = ["status"]
 
     @decorators.endpoint(
         path="/status",
         summary="Check if the API server is currently reachable",
         description="Use this endpoint to monitor network or server problems",
         responses={200: "Server is alive"},
     )
     def get(self) -> Response:
-
         return self.response("Server is alive", allow_html=True)
 
 
 class AuthStatus(EndpointResource):
-
     depends_on = ["AUTH_ENABLE"]
     labels = ["authentication"]
 
     @decorators.auth.require()
     @decorators.endpoint(
         path="/auth/status",
         summary="Verify the validity of the provided token",
         description="Use this endpoint to verify if an auth token is valid",
         responses={200: "Auth token is valid"},
     )
     def get(self, user: User) -> Response:
-
         return self.response(True)
```

### Comparing `rapydo_http-2.4/restapi/endpoints/swagger_specs.py` & `rapydo_http-3.0/restapi/endpoints/swagger_specs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Optional
 
 from glom import glom
 
 from restapi import decorators
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import User
 from restapi.utilities.globals import mem
 from restapi.utilities.logs import log
 
 
-def add_model(definitions: Dict[str, bool], def_name: str, is_private: bool) -> None:
+def add_model(definitions: dict[str, bool], def_name: str, is_private: bool) -> None:
     def_name = def_name.replace("#/definitions/", "")
 
     definitions.setdefault(def_name, True)
     # Will be True if all occurrences are private
     definitions[def_name] = definitions[def_name] and is_private
 
 
@@ -27,74 +27,68 @@
     @decorators.auth.optional(allow_access_token_parameter=True)
     @decorators.endpoint(
         path="/specs",
         summary="Endpoints specifications based on OpenAPI 2.0 format",
         responses={200: "Endpoints JSON based on OpenAPI Specifications"},
     )
     def get(self, user: Optional[User]) -> Response:
-
         specs = mem.docs.spec.to_dict()
         if user:
             # Set security requirements for endpoint
             for key, data in specs.items():
                 if key == "paths":
                     for uri, endpoint in data.items():
                         u = uri.replace("{", "<").replace("}", ">")
                         for method, definition in endpoint.items():
-
                             auth_required = glom(
                                 mem.authenticated_endpoints,
                                 f"{u}.{method}",
                                 default=False,
                             )
 
                             if auth_required:
                                 definition["security"] = [{"Bearer": []}]
 
             return self.response(specs)
 
         log.debug("Unauthenticated request, filtering out private endpoints")
         # Remove sensible data
-        filtered_specs: Dict[str, Dict[str, Dict[str, Any]]] = {}
+        filtered_specs: dict[str, dict[str, dict[str, Any]]] = {}
         # schemaName => True|False (private|public)
-        privatedefs: Dict[str, bool] = {}
+        privatedefs: dict[str, bool] = {}
         # schemaName => [list of definitions including this]
-        parentdefs: Dict[str, List[Any]] = {}
+        parentdefs: dict[str, list[Any]] = {}
         for key, data in specs.items():
-
             # Find endpoint mapping flagged as private
             if key == "paths":
                 for uri, endpoint in data.items():
                     u = uri.replace("{", "<").replace("}", ">")
                     for method, definition in endpoint.items():
-
                         is_private = glom(
                             mem.private_endpoints,
                             f"{u}.{method}",
                             default=False,
                         )
 
                         defs = definition.get("parameters", [])[:]
                         for p in defs:
-
                             if "schema" not in p:
                                 continue
                             if "$ref" in p["schema"]:
                                 ref = p["schema"]["$ref"]
                                 add_model(privatedefs, ref, is_private)
                             elif (
                                 "items" in p["schema"]
                                 and "$ref" in p["schema"]["items"]
-                            ):
+                            ):  # pragma: no cover
                                 ref = p["schema"]["items"]["$ref"]
                                 add_model(privatedefs, ref, is_private)
 
-                        for code, response in definition.get("responses", {}).items():
+                        for _, response in definition.get("responses", {}).items():
                             if "schema" in response:
-
                                 if "$ref" in response["schema"]:
                                     ref = response["schema"]["$ref"]
                                     add_model(privatedefs, ref, is_private)
                                 elif (
                                     "items" in response["schema"]
                                     and "$ref" in response["schema"]["items"]
                                 ):
@@ -116,24 +110,22 @@
 
                         filtered_specs.setdefault(key, {})
                         filtered_specs[key].setdefault(uri, {})
                         filtered_specs[key][uri].setdefault(method, definition)
 
                         # definitions
             elif key == "definitions":
-
                 # Saving definition inclusion, will be used later to determine
                 # if a definition is private or not
                 # If a definition is referenced by an endpoint, the definition
                 # visibility matches the endpoint visibility
                 # If a definition is referenced by other definitions, its visibility
                 # will be calculated as AND(parent definitions)
                 # Verification postponed
                 for schema, definition in data.items():
-
                     # parentdefs
                     for d in definition.get("properties", {}).values():
                         # Generated by Nested without allow_none
                         if "$ref" in d:
                             ref = d["$ref"]
                             def_name = ref.replace("#/definitions/", "")
 
@@ -154,33 +146,30 @@
 
                                 parentdefs.setdefault(def_name, [])
                                 parentdefs[def_name].append(schema)
             else:
                 filtered_specs.setdefault(key, data)
 
         if "definitions" in specs:
-
             filtered_specs.setdefault("definitions", {})
             for schema, definition in specs["definitions"].items():
-
                 if self.is_definition_private(schema, privatedefs, parentdefs):
                     log.debug("Skipping private definition {}", schema)
                     continue
                 filtered_specs["definitions"].setdefault(schema, definition)
 
         return self.response(filtered_specs)
 
     def is_definition_private(
         self,
         schema_name: str,
-        privatedefs: Dict[str, bool],
-        parentdefs: Dict[str, Any],
+        privatedefs: dict[str, bool],
+        parentdefs: dict[str, Any],
         recursion: int = 0,
     ) -> bool:
-
         # can be True|False|None
         from_private_endpoint = privatedefs.get(schema_name, None)
 
         # Can be None|empty list|list
         parents = parentdefs.get(schema_name, None)
 
         # This definition is not used by any endpoint or other definitions
```

### Comparing `rapydo_http-2.4/restapi/endpoints/test_authentication.py` & `rapydo_http-3.0/restapi/endpoints/test_authentication.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 from restapi import decorators
 from restapi.config import TESTING
 from restapi.exceptions import Unauthorized
 from restapi.models import fields
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import Role, User
@@ -13,104 +13,96 @@
         @decorators.endpoint(
             path="/tests/noauth",
             summary="Only resp a fixed response, no authenticataion is required",
             description="Only enabled in testing mode",
             responses={200: "Tests executed"},
         )
         def get(self) -> Response:
-
             return self.response("OK")
 
     class TestAuthentication(EndpointResource):
         @decorators.auth.require()
         @decorators.endpoint(
             path="/tests/authentication",
             summary="Only echos received token and corresponding user",
             description="Only enabled in testing mode",
             responses={200: "Tests executed"},
         )
         def get(self, user: User) -> Response:
-
             return self.response({"email": user.email})
 
     class TestOptionalAuthentication(EndpointResource):
         @decorators.auth.optional()
         @decorators.endpoint(
             path="/tests/optionalauthentication",
             summary="Only echos received token and corresponding user, if any",
             description="Only enabled in testing mode",
             responses={
                 200: "Tests executed with auth",
                 204: "Tests executed without auth",
             },
         )
         def get(self, user: Optional[User]) -> Response:
-
             if user:
                 return self.response({"email": user.email})
             return self.empty_response()
 
     class TestQueryParameterAuthentication(EndpointResource):
         @decorators.auth.require(allow_access_token_parameter=True)
         @decorators.endpoint(
             path="/tests/queryauthentication",
             summary="Only echos received token and corresponding user",
             description="Only enabled in testing mode",
             responses={200: "Tests executed"},
         )
         def get(self, user: User) -> Response:
-
             return self.response({"email": user.email})
 
     class TestOptionalQueryParameterAuthentication(EndpointResource):
         @decorators.auth.optional(allow_access_token_parameter=True)
         @decorators.endpoint(
             path="/tests/optionalqueryauthentication",
             summary="Only echos received token and corresponding user, if any",
             description="Only enabled in testing mode",
             responses={
                 200: "Tests executed with auth",
                 204: "Tests executed without auth",
             },
         )
         def get(self, user: Optional[User]) -> Response:
-
             if user:
                 return self.response({"email": user.email})
             return self.empty_response()
 
     class TestAuthenticationWithMultipleRoles(EndpointResource):
         @decorators.auth.require_any(Role.ADMIN, Role.USER)
         @decorators.endpoint(
             path="/tests/manyrolesauthentication",
             summary="Only echos received token and corresponding user",
             description="Only enabled in testing mode",
             responses={200: "Tests executed"},
         )
         def get(self, user: User) -> Response:
-
             return self.response({"email": user.email})
 
     # Note: this endpoint requires a role that does not exist!
     class TestAuthenticationWithMissingRole(EndpointResource):
         @decorators.auth.require_any("UnknownRole")
         @decorators.endpoint(
             path="/tests/unknownroleauthentication",
             summary="Only echos received token and corresponding user, if any",
             description="Only enabled in testing mode",
             responses={200: "Tests executed"},
         )
         # no cover because this endpoint will be never called
         # because it requires an Unknown Role to be accessed
         def get(self, user: User) -> Response:  # pragma: no cover
-
             return self.response({"email": user.email})
 
-    def verify_uuid_value(endpoint: EndpointResource, uuid: str) -> Dict[str, Any]:
-
+    def verify_uuid_value(endpoint: EndpointResource, uuid: str) -> dict[str, Any]:
         user = endpoint.auth.get_user(user_id=uuid)
         if not user or not endpoint.auth.is_admin(user):
             raise Unauthorized("You are not authorized")
 
         # Returned values if any will be injected into the endpoint as fn parameters
         return {"target_user": user}
         # Otherwise can simply return None to inject nothing
```

### Comparing `rapydo_http-2.4/restapi/endpoints/test_autocomplete.py` & `rapydo_http-3.0/restapi/endpoints/test_autocomplete.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from typing import Dict, List, Tuple
-
 from restapi import decorators
 from restapi.config import TESTING
 from restapi.models import Schema, fields
 from restapi.rest.definition import EndpointResource, Response
 
 if TESTING:
-
     names = ["oliver", "jack", "harry", "charlie", "thomas"]
     surnames = ["smith", "jones", "taylor", "brown", "williams"]
     nicknames = ["kid", "good", "bad", "ugly", "ripper"]
 
     class MyElement(Schema):
         my_id = fields.Str(required=True)
         my_label = fields.Str(required=True)
@@ -40,15 +37,15 @@
                 "autocomplete_label_bind": "my_label",
                 "autocomplete_show_id": True,
             },
         )
 
     class TestAutocomplete(EndpointResource):
         @staticmethod
-        def get_element(name: str, surname: str, nickname: str) -> Tuple[str, str]:
+        def get_element(name: str, surname: str, nickname: str) -> tuple[str, str]:
             return (
                 f"{name[0].upper()}{surname[0].upper()}{nickname[0].upper()}",
                 f"{name.title()} {surname.title()} the {nickname.title()}",
             )
 
         # This is the autocomplete endpoint
         # It receive a string and return a list of elements matching the input
@@ -56,16 +53,15 @@
         @decorators.endpoint(
             path="/tests/autocomplete/<query>",
             summary="Return list of elements matching the input",
             description="Only enabled in testing mode",
             responses={200: "Tests executed"},
         )
         def get(self, query: str) -> Response:
-
-            elements: List[Dict[str, str]] = []
+            elements: list[dict[str, str]] = []
 
             for k1 in names:
                 for k2 in surnames:
                     for k3 in nicknames:
                         k, v = self.get_element(k1, k2, k3)
 
                         if query.lower() in v.lower():
@@ -76,21 +72,19 @@
         @decorators.use_kwargs(ListInput)
         @decorators.endpoint(
             path="/tests/autocomplete",
             summary="Receives a list of MyElements",
             description="Only enabled in testing mode",
             responses={204: "Tests executed", 400: "Bad Input"},
         )
-        def post(self, elements: List[str]) -> Response:
-
+        def post(self, elements: list[str]) -> Response:
             return self.empty_response()
 
         @decorators.use_kwargs(SingleInput)
         @decorators.endpoint(
             path="/tests/autocomplete",
             summary="Receives a single MyElement",
             description="Only enabled in testing mode",
             responses={204: "Tests executed", 400: "Bad Input"},
         )
         def put(self, element: str) -> Response:
-
             return self.empty_response()
```

### Comparing `rapydo_http-2.4/restapi/endpoints/test_cache.py` & `rapydo_http-3.0/restapi/endpoints/test_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
             description="Only enabled in testing mode",
             responses={
                 200: "Content sent",
             },
         )
         @decorators.cache(timeout=1)
         def get(self) -> Response:
-
             TestShortCache.counter += 1
             return self.response(TestShortCache.counter)
 
     class TestLongCache(EndpointResource):
         """
         Used to test cache cleaning with manual methods
         """
@@ -44,28 +43,26 @@
             description="Only enabled in testing mode",
             responses={
                 200: "Content sent",
             },
         )
         @decorators.cache(timeout=200)
         def get(self) -> Response:
-
             TestLongCache.counter += 1
             return self.response(TestLongCache.counter)
 
         @decorators.endpoint(
             path="/tests/cache/long",
             summary="Clear endpoint cache",
             description="Only enabled in testing mode",
             responses={
                 204: "Endpoint cache cleared",
             },
         )
         def delete(self) -> Response:
-
             self.clear_endpoint_cache()
             return self.empty_response()
 
     class TestAuthCache(EndpointResource):
         """
         Used to test cache of authenticated endpoints
         (cache keys are token dependent)
@@ -82,15 +79,14 @@
             description="Only enabled in testing mode",
             responses={
                 200: "Content sent",
             },
         )
         @decorators.cache(timeout=200)
         def get(self, user: User) -> Response:
-
             TestAuthCache.counter += 1
             return self.response((user.uuid, TestAuthCache.counter))
 
     class TestOptionalAuthCache(EndpointResource):
         """
         Used to test cache of optionally authenticated endpoints
         (cache keys are token dependent, if tokens are provided and valid)
@@ -107,15 +103,14 @@
             description="Only enabled in testing mode",
             responses={
                 200: "Content sent",
             },
         )
         @decorators.cache(timeout=200)
         def get(self, user: Optional[User]) -> Response:
-
             TestOptionalAuthCache.counter += 1
             uuid = user.uuid if user else "N/A"
             return self.response((uuid, TestOptionalAuthCache.counter))
 
     class TestParamAuthCache(EndpointResource):
         """
         Used to test cache of authenticated endpoints that accept access token param
@@ -133,15 +128,14 @@
             description="Only enabled in testing mode",
             responses={
                 200: "Content sent",
             },
         )
         @decorators.cache(timeout=200)
         def get(self, user: User) -> Response:
-
             TestParamAuthCache.counter += 1
             return self.response((user.uuid, TestParamAuthCache.counter))
 
     class TestOptionalParamAuthCache(EndpointResource):
         """
         Used to test cache of optionally authenticated endpoints
         that accept access token param
@@ -159,11 +153,10 @@
             description="Only enabled in testing mode",
             responses={
                 200: "Content sent",
             },
         )
         @decorators.cache(timeout=200)
         def get(self, user: Optional[User]) -> Response:
-
             TestOptionalParamAuthCache.counter += 1
             uuid = user.uuid if user else "N/A"
             return self.response((uuid, TestOptionalParamAuthCache.counter))
```

### Comparing `rapydo_http-2.4/restapi/endpoints/test_databases.py` & `rapydo_http-3.0/restapi/endpoints/test_databases.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,56 +6,48 @@
 from restapi.exceptions import BadRequest, DatabaseDuplicatedEntry, ServerError
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import DEFAULT_GROUP_NAME
 
 # from restapi.utilities.logs import log
 
 if TESTING:
-
     # This endpoint will try to create database object with unique keys
     # A duplicated entry exception will be raised and catched by the
     # database_transaction that will restore previous modifications
     class TestDatabase(EndpointResource):
-
         labels = ["tests"]
 
         @decorators.database_transaction
         @decorators.endpoint(
             path="/tests/database/<data>",
             summary="Execute tests on database functionalities",
             description="Only enabled in testing mode",
             responses={
                 200: "Tests executed",
                 400: "Bad input",
                 409: "Group already exists",
             },
         )
         def post(self, data: str) -> Response:
-
             # Special value! This will try to create a group without shortname
             # A BadRequest will be raised due to the missing property
             if data == "400":
                 group = self.auth.create_group({"fullname": data})
                 # The following two lines will be never executed because the
                 # create group above is intended to fail due to the missing property
                 self.auth.save_group(group)  # pragma: no cover
                 return self.response("0")  # pragma: no cover
 
-            # This was just to limit schemathesis to create troubles :-)
-            if not re.match(r"^[A-Za-z]+$", data):
-                raise BadRequest(f"Invalid input name {data}")
-
             # Only DatabaseDuplicatedEntry will be raised by this endpoint
             # Any other exceptions will be suppressed. This will ensure that
             # DatabaseDuplicatedEntry is raised and no others.
             # As a side effect this endpoint will modifiy the fullname of the default
             # Group if the exception is not raised. Otherwise this modification will
             # be undo by the database_transaction decorator
             try:
-
                 default_group = self.auth.get_group(name=DEFAULT_GROUP_NAME)
 
                 if default_group is None:  # pragma: no cover
                     raise ServerError("Default group is missing")
 
                 default_group.fullname = f"{default_group.fullname}_exteded"
                 # Don't commit with alchemy or the transaction can't be rollbacked
```

### Comparing `rapydo_http-2.4/restapi/endpoints/test_depends_on.py` & `rapydo_http-3.0/restapi/endpoints/test_depends_on.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 from restapi import decorators
 from restapi.config import TESTING
 from restapi.rest.definition import EndpointResource, Response
 
 if TESTING:
-
     # This endpoint is activated only if neo4j is enabled
     class TestDependsOn(EndpointResource):
-
         labels = ["tests"]
         depends_on = ["NEO4J_ENABLE"]
 
         @decorators.endpoint(
             path="/tests/depends_on/neo4j",
             summary="Execute tests on depends on option",
             description="Only enabled in testing mode",
             responses={
                 200: "Content sent",
             },
         )
         def get(self) -> Response:
-
             return self.response("1")
 
     # This endpoint is activated only if neo4j is NOT enabled
     class TestDependsOnNOT(EndpointResource):
-
         labels = ["tests"]
         depends_on = ["not NEO4J_ENABLE"]
 
         @decorators.endpoint(
             path="/tests/depends_on_not/neo4j",
             summary="Execute tests on depends on option",
             description="Only enabled in testing mode",
             responses={
                 200: "Content sent",
             },
         )
         def get(self) -> Response:
-
             return self.response("1")
```

### Comparing `rapydo_http-2.4/restapi/endpoints/test_download.py` & `rapydo_http-3.0/restapi/endpoints/test_download.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from restapi.models import fields
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.download import Downloader
 
 if TESTING:
 
     class TestDownload(EndpointResource):
-
         labels = ["tests"]
 
         @decorators.use_kwargs({"stream": fields.Bool()}, location="query")
         @decorators.endpoint(
             # forgot the leading slash to test the automatic fix
             path="tests/download/<folder>/<fname>",
             summary="Execute tests with the downloader",
```

### Comparing `rapydo_http-2.4/restapi/endpoints/test_inputs.py` & `rapydo_http-3.0/restapi/endpoints/test_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,20 +99,18 @@
         @decorators.endpoint(
             path="/tests/inputs",
             summary="Accept inputs based on a rich model",
             description="Only enabled in testing mode",
             responses={204: "Tests executed"},
         )
         def post(self, user: Optional[User], **kwargs: Any) -> Response:
-
             return self.empty_response()
 
 
 if TESTING and Connector.check_availability("neo4j"):
-
     CHOICES = (("A", "AAA"), ("B", "BBB"), ("C", "CCC"))
 
     class InputNeo4jSchema(Schema):
         # include a Neo4jChoice to test the deserialize
         choice = fields.Neo4jChoice(CHOICES, required=True)
 
     class UUID(Schema):
@@ -134,15 +132,14 @@
         @decorators.marshal_with(OutputNeo4jSchema)
         @decorators.endpoint(
             path="/tests/neo4jinputs",
             summary="Accept inputs based on a neo4j-related schema",
             responses={204: "Tests executed"},
         )
         def post(self, choice: str, user: User) -> Response:
-
             data = {
                 "choice": choice,
                 "relationship_many": user.tokens,
                 "relationship_single": user.belongs_to,
                 "relationship_count": user.tokens,
             }
             return self.response(data)
```

### Comparing `rapydo_http-2.4/restapi/endpoints/test_neo4j.py` & `rapydo_http-3.0/restapi/endpoints/test_neo4j.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from restapi.connectors import Connector, neo4j
 from restapi.exceptions import BadRequest
 from restapi.models import Neo4jSchema, Schema, fields
 from restapi.rest.definition import EndpointResource, Response
 from restapi.utilities.logs import log
 
 if TESTING and Connector.check_availability("neo4j"):
-
     from neomodel import (
         DateProperty,
         FloatProperty,
         IntegerProperty,
         StringProperty,
         StructuredNode,
         UniqueIdProperty,
@@ -57,15 +56,14 @@
         group7 = Neo4jSchema(Group, fields=None)
         custom = Neo4jSchema(Custom, fields="*")
 
         choices1 = fields.Neo4jChoice(CHOICES_tuple)
         choices2 = fields.Neo4jChoice(CHOICES_dict)
 
     class TestNeo4j(EndpointResource):
-
         depends_on = ["NEO4J_ENABLE_CONNECTOR"]
         labels = ["tests"]
 
         @decorators.marshal_with(Output, code=200)
         @decorators.endpoint(
             path="/tests/neo4j/<test>",
             summary="Execute tests against the neo4j connector",
@@ -88,12 +86,10 @@
                     n = self.neo4j.NodeTest(p_str="")
                     n.save()
                     data["created"] = n.created
                     data["modified1"] = n.modified
                     n.save()
                     data["modified2"] = n.modified
                     return self.response(data)
-                else:
-                    log.info("No Test")
             except Exception as e:
-                raise BadRequest(str(e))
+                raise BadRequest(str(e)) from e
             return self.response({"val": 1})
```

### Comparing `rapydo_http-2.4/restapi/endpoints/test_outputs.py` & `rapydo_http-3.0/restapi/endpoints/test_outputs.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,14 @@
         # @decorators.marshal_with(OutputSchema)
         @decorators.endpoint(
             path="/tests/outputs/<out_type>",
             summary="Produce outputs based on the out_type url parameters",
             responses={200: "Tests executed"},
         )
         def post(self, out_type: str) -> Response:
-
             if out_type == "list":
                 return self.response(["a", "b", "c", "c"])
 
             if out_type == "tuple":
                 return self.response(("a", "b", "c", "c"))
 
             if out_type == "set":
```

### Comparing `rapydo_http-2.4/restapi/endpoints/test_pagination.py` & `rapydo_http-3.0/restapi/endpoints/test_pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from restapi import decorators
 from restapi.config import TESTING
 from restapi.rest.definition import EndpointResource, Response
 
 if TESTING:
 
     class TestPagination(EndpointResource):
-
         # 150 integers from 1 to 150
         values = list(range(1, 151))
 
         @decorators.get_pagination
         @decorators.endpoint(
             path="/tests/pagination",
             summary="Execute tests on a paginated endpoint",
```

### Comparing `rapydo_http-2.4/restapi/endpoints/test_parameters_injection.py` & `rapydo_http-3.0/restapi/endpoints/test_parameters_injection.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,9 +12,8 @@
             summary="Verify injected parameters",
             description="Only enabled in testing mode",
             responses={200: "Tests executed"},
         )
         def get(
             self, param: str, user: User, unknown: str = "default_value"
         ) -> Response:
-
             return self.response([user.email, param, unknown])
```

### Comparing `rapydo_http-2.4/restapi/endpoints/test_upload.py` & `rapydo_http-3.0/restapi/endpoints/test_upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,37 +7,34 @@
 
 if TESTING:
 
     class Force(PartialSchema):
         force = fields.Bool()
 
     class TestUpload(EndpointResource, Uploader):
-
         labels = ["tests"]
 
         @decorators.use_kwargs(Force)
         @decorators.endpoint(
             # forget the leading slash to test the automatic fix
             path="tests/upload",
             summary="Execute tests with the uploader",
             description="Only enabled in testing mode",
             responses={200: "Tests executed"},
         )
         def put(self, force: bool = False) -> Response:
-
             # This is just to test the allowed exts without adding a new parameter..
             if not force:
                 self.set_allowed_exts(["txt"])
             response = self.upload(
                 subfolder=DATA_PATH.joinpath("fixsubfolder"), force=force
             )
             return response
 
     class TestChunkedUpload(EndpointResource, Uploader):
-
         labels = ["tests"]
 
         @decorators.init_chunk_upload
         @decorators.use_kwargs(Force)
         @decorators.endpoint(
             # forgot the leading slash to test the automatic fix
             path="tests/chunkedupload",
@@ -49,15 +46,14 @@
             self,
             name: str,
             mimeType: str,
             size: int,
             lastModified: int,
             force: bool = False,
         ) -> Response:
-
             # This is just to test the allowed exts without adding a new parameter..
             if not force:
                 self.set_allowed_exts(["txt"])
 
             path = DATA_PATH.joinpath("fixed")
             return self.init_chunk_upload(path, name, force=force)
 
@@ -66,15 +62,14 @@
             # forgot the leading slash to test the automatic fix
             path="tests/chunkedupload/<filename>",
             summary="Execute tests with the chunked uploader",
             description="Only enabled in testing mode",
             responses={200: "Tests executed"},
         )
         def put(self, filename: str, force: bool = False) -> Response:
-
             path = DATA_PATH.joinpath("fixed")
             completed, response = self.chunk_upload(path, filename)
 
             if completed:
                 log.info("Upload completed")
 
             return response
```

### Comparing `rapydo_http-2.4/restapi/endpoints/tokens.py` & `rapydo_http-3.0/restapi/endpoints/tokens.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from typing import Any, Dict
+from typing import Any
 
 from restapi import decorators
 from restapi.endpoints.schemas import TokenSchema
 from restapi.exceptions import BadRequest, Forbidden
 from restapi.rest.definition import EndpointResource, Response
 from restapi.services.authentication import User
 
 # from restapi.utilities.logs import log
 
 
 def inject_token(
     endpoint: EndpointResource, token_id: str, user: User
-) -> Dict[str, Any]:
-
+) -> dict[str, Any]:
     tokens = endpoint.auth.get_tokens(user=user)
 
     for token in tokens:
         if token["id"] == token_id:
             return {"token": token["token"]}
 
     raise Forbidden("Token not emitted for your account or does not exist")
@@ -32,29 +31,27 @@
     @decorators.marshal_with(TokenSchema(many=True), code=200)
     @decorators.endpoint(
         path="/auth/tokens",
         summary="Retrieve all emitted tokens",
         responses={200: "List of tokens"},
     )
     def get(self, user: User) -> Response:
-
         tokens = self.auth.get_tokens(user=user)
 
         return self.response(tokens)
 
     # token_id = uuid associated to the token you want to select
     @decorators.auth.require()
     @decorators.preload(callback=inject_token)
     @decorators.endpoint(
         path="/auth/tokens/<token_id>",
         summary="Invalidate the specified token",
         responses={204: "Token has been invalidated"},
     )
     def delete(self, token_id: str, token: str, user: User) -> Response:
-
         if self.auth.invalidate_token(token=token):
             return self.empty_response()
 
         # Added just to make very sure, but it can never happen because
         # invalidate_token can only fail if the token is invalid
         # since this is an authenticated endpoint the token is already verified
         raise BadRequest(f"Failed token invalidation: {token}")  # pragma: no cover
```

### Comparing `rapydo_http-2.4/restapi/env.py` & `rapydo_http-3.0/restapi/env.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Utilities to work with environment variables
 """
+
 import os
 from functools import lru_cache
-from typing import Dict, Union
+from typing import Union
 
 
 class Env:
     @staticmethod
     @lru_cache
     def get(var: str, default: str) -> str:
         return os.getenv(var, default)
@@ -21,15 +22,14 @@
     @lru_cache
     def get_int(var: str, default: int = 0) -> int:
         return Env.to_int(Env.get(var, ""), default)
 
     @staticmethod
     @lru_cache
     def to_bool(var: Union[None, str, bool], default: bool = False) -> bool:
-
         if var is None or var == "":
             return default
 
         if isinstance(var, bool):
             return var
 
         # if not directly a bool, try an interpretation
@@ -50,45 +50,40 @@
                 return True
 
         return default
 
     @staticmethod
     @lru_cache
     def to_int(var: Union[None, str, int], default: int = 0) -> int:
-
         if var is None or var == "":
             return default
 
         if isinstance(var, int):
             return var
 
         try:
             return int(var)
         except ValueError:
             pass
 
         return default
 
     @staticmethod
-    def load_variables_group(prefix: str) -> Dict[str, str]:
-
+    def load_variables_group(prefix: str) -> dict[str, str]:
         prefix += "_"
 
-        variables: Dict[str, str] = {}
+        variables: dict[str, str] = {}
 
         for var, value in os.environ.items():
-
             var = var.lower()
 
             if not var.startswith(prefix):
                 continue
 
             # Fix key and value before saving
-            # Can't be enabled due to mistral stuck at py38
-            # key = var.removeprefix(prefix)
-            key = var[len(prefix) :]
+            key = var.removeprefix(prefix)
             # One thing that we must avoid is any quote around our value
             value = value.strip('"').strip("'")
             # save
             variables[key] = value
 
         return variables
```

### Comparing `rapydo_http-2.4/restapi/exceptions.py` & `rapydo_http-3.0/restapi/exceptions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Set of Exceptions used to raise HTTP error statuses from endpoints
 """
+
 from typing import Union
 
 ExceptionType = Union[str, Exception]
 
 
 class RestApiException(Exception):
     def __init__(
         self,
         exception: ExceptionType,
         status_code: int = 404,
         is_warning: bool = False,
     ):
-
         super().__init__(exception)
         self.status_code = status_code or 404
         self.is_warning = is_warning
 
 
 class BadRequest(RestApiException):
     def __init__(self, exception: ExceptionType, is_warning: bool = False):
```

### Comparing `rapydo_http-2.4/restapi/mocks.py` & `rapydo_http-3.0/restapi/mocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Mock classes used to replace customization classes when building the documentation
 """
-from typing import Tuple
 
 from restapi.connectors import Connector
 from restapi.customizer import BaseCustomizer, FlaskRequest, Props, User
 from restapi.rest.definition import EndpointResource
 
 
 class Initializer:
@@ -22,15 +21,15 @@
         pass
 
 
 class Customizer(BaseCustomizer):
     @staticmethod
     def custom_user_properties_pre(
         properties: Props,
-    ) -> Tuple[Props, Props]:
+    ) -> tuple[Props, Props]:
         """
         executed just before user creation
         use this method to removed or manipulate input properties
         before sending to the database
         """
         extra_properties: Props = {}
         # if "myfield" in properties:
@@ -57,15 +56,14 @@
         """
         # data["CustomField"] = user.custom_field
 
         return data
 
     @staticmethod
     def get_custom_input_fields(request: FlaskRequest, scope: int) -> Props:
-
         # required = request and request.method == "POST"
         """
         if scope == BaseCustomizer.ADMIN:
             return {
                 'custom_field': fields.Int(
                     required=required,
                     # validate=validate.Range(min=0, max=???),
```

### Comparing `rapydo_http-2.4/restapi/models/__init__.py` & `rapydo_http-3.0/restapi/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Extension of input and output Schemas and Fields
 """
+
 from typing import Any
 
 from marshmallow import pre_load, validate
 from webargs.flaskparser import parser
 
 from restapi.models import fields
 from restapi.models.schema import GET_SCHEMA_KEY, Neo4jSchema, PartialSchema, Schema
```

### Comparing `rapydo_http-2.4/restapi/models/fields.py` & `rapydo_http-3.0/restapi/models/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
-from typing import Any, Mapping, Optional, Tuple, Union
+from collections.abc import Mapping
+from typing import Any, Optional, Union
 
 import orjson
 from marshmallow import ValidationError, types
 from marshmallow.utils import missing as missing_
 from webargs import fields
 
 from restapi.config import TESTING
@@ -44,15 +45,14 @@
     def _deserialize(
         self,
         value: Any,
         attr: Optional[str],
         data: Optional[Mapping[str, Any]],
         **kwargs: Any,
     ) -> Any:
-
         # this is the case when requests (or pytest) send some json-dumped lists
         # for example for a multi-value select
         if isinstance(value, str):
             try:
                 value = orjson.loads(value)
             except Exception:
                 pass
@@ -73,25 +73,24 @@
         return value
 
 
 class Nested(fields.Nested):
     def __init__(
         self,
         # nested: Union[SchemaABC, type, str, Callable[[], SchemaABC]],
-        # the above type is from marshmallow, but it fails with Dict[str, Any] (imc)
+        # the above type is from marshmallow, but it fails with dict[str, Any] (imc)
         nested: Any,
         *,
         default: Any = missing_,
         only: Optional[types.StrSequenceOrSet] = None,
         exclude: types.StrSequenceOrSet = (),
         many: bool = False,
         unknown: Optional[str] = None,
         **kwargs: Any,
     ):
-
         super().__init__(
             nested,
             default=default,
             only=only,
             exclude=exclude,
             many=many,
             unknown=unknown,
@@ -99,18 +98,17 @@
         )
 
     def _deserialize(
         self,
         value: Any,
         attr: Optional[str],
         data: Optional[Mapping[str, Any]],
-        partial: Optional[Union[bool, Tuple[str]]] = None,
+        partial: Optional[Union[bool, tuple[str]]] = None,
         **kwargs: Any,
     ) -> Any:
-
         # this is the case when requests (or pytest) send some json-dumped object
         if isinstance(value, str):
             try:
                 value = orjson.loads(value)
             except Exception as e:  # pragma: no cover
                 log.warning(e)
         # This is because Nested is not typed on marshmallow
@@ -137,15 +135,14 @@
     def _deserialize(
         self,
         value: Any,
         attr: Optional[str],
         data: Optional[Mapping[str, Any]],
         **kwargs: Any,
     ) -> Any:
-
         if not value:
             return value
 
         # This is because List is not typed on marshmallow
         values = super()._deserialize(value, attr, data, **kwargs)  # type: ignore
 
         if self.no_duplicates and len(values) != len(set(values)):
@@ -171,15 +168,17 @@
             self.choices_dict = choices_model
         else:
             # convert the tuple of tuple into as a dictionary for convenience
             self.choices_dict = {}
             for k, v in choices_model:
                 self.choices_dict.setdefault(k, v)
 
-    def _serialize(self, value: Any, attr: str, obj: Any, **kwargs: Any) -> Any:
+    def _serialize(
+        self, value: Any, attr: Optional[str], obj: Any, **kwargs: Any
+    ) -> Any:
         return {
             "key": value,
             # the value correspondance from choices_dict or value as default
             "description": self.choices_dict.get(value, value),
         }
 
     def _deserialize(
@@ -193,53 +192,54 @@
 
 
 class Neo4jRelationshipToMany(Nested):
     # value: StructuredRel
     # Signature of "_serialize" incompatible with supertype "Nested"
     # This is because Nested is not typed on marshmallow
     def _serialize(  # type: ignore
-        self, value: Any, attr: str, obj: Any, **kwargs: Any
+        self, value: Any, attr: Optional[str], obj: Any, **kwargs: Any
     ) -> Any:
         self.many = True
         # This is because Nested is not typed on marshmallow
         return super()._serialize(value.all(), attr, obj, **kwargs)  # type: ignore
 
 
 class Neo4jRelationshipToSingle(Nested):
     # value: StructuredRel
     # Signature of "_serialize" incompatible with supertype "Nested"
     # This is because Nested is not typed on marshmallow
     def _serialize(  # type: ignore
         self,
         value: Any,
-        attr: str,
+        attr: Optional[str],
         obj: Any,
         **kwargs: Any,
     ) -> Any:
         self.many = False
         self.schema.many = False
         # This is because Nested is not typed on marshmallow
         return super()._serialize(value.single(), attr, obj, **kwargs)  # type: ignore
 
 
 class Neo4jRelationshipToCount(fields.Int):
     # value: StructuredRel
-    def _serialize(self, value: Any, attr: str, obj: Any, **kwargs: Any) -> Any:
+    def _serialize(
+        self, value: Any, attr: Optional[str], obj: Any, **kwargs: Any
+    ) -> Any:
         return self._format_num(len(value))
 
 
 class TOTP(String):
     def _deserialize(
         self,
         value: Any,
         attr: Optional[str],
         data: Optional[Mapping[str, Any]],
         **kwargs: Any,
     ) -> Any:
-
         value = super()._deserialize(value, attr, data, **kwargs)
 
         if not re.match(r"^[0-9]{6}$", value):
             if TESTING:
                 log.error("Invalid TOTP format: {}", value)
             raise ValidationError("Invalid TOTP format")
```

### Comparing `rapydo_http-2.4/restapi/models/schema.py` & `rapydo_http-3.0/restapi/models/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,78 +1,75 @@
 import inspect
-from typing import Any, Dict, Optional, Type, Union, cast
+from typing import Any, Optional, Union, cast
 
 from marshmallow import EXCLUDE
 from marshmallow import Schema as MarshmallowSchema
 from marshmallow import ValidationError, pre_load
 from neomodel import StructuredNode, StructuredRel, properties
 
 from restapi.models import fields
 from restapi.utilities.logs import log
 
 GET_SCHEMA_KEY = "get_schema"
 
 
 class Schema(MarshmallowSchema):
     def __init__(self, strip_required: bool = False, *args: Any, **kwargs: Any) -> None:
-
         super().__init__(**kwargs)
         if strip_required:
             for k in self.declared_fields:
                 self.declared_fields[k].required = False
 
     @classmethod
     def from_dict(
         cls,
-        fields: Dict[str, Union[fields.Field, type]],
+        fields: dict[str, Union[fields.Field, type]],
         *,
         name: str = "GeneratedSchema",
     ) -> type:
         return super().from_dict(fields, name=name)
 
     # instruct marshmallow to serialize data to a collections.OrderedDict
     class Meta:
         ordered = True
 
     # NOTE: self is not used, but @pre_load cannot be static
     @pre_load
     def raise_get_schema(
         self,
-        data: Dict[str, Any],
+        data: dict[str, Any],
         **kwargs: Any,
-    ) -> Dict[str, Any]:
-
+    ) -> dict[str, Any]:
         if GET_SCHEMA_KEY in data:
             raise ValidationError("Schema requested")
 
         if "access_token" not in data:
             return data
 
         # data is Immutable if it comes from args, is mutable otherwise
         try:
             data.pop("access_token")
             return data
             # Why isinstance is not working here!?
             # isinstance(data, ImmutableMultiDict)
         except TypeError:  # pragma: no cover
-
             mutable_data = data.to_dict()  # type: ignore
             mutable_data.pop("access_token")
-            return cast(Dict[str, Any], mutable_data)
+            return cast(dict[str, Any], mutable_data)
 
 
 class PartialSchema(Schema):
     class Meta:
         ordered = True
         unknown = EXCLUDE
 
 
 class Neo4jSchema(Schema):
     def __init__(
-        self, model: Type[Any], fields: Optional[Any], *args: Any, **kwargs: Any
+        self, model: type[Any], fields: Optional[Any], *args: Any, **kwargs: Any
     ) -> None:
         super().__init__(**kwargs)
 
         if not fields:
             fields = ()
         elif fields == "*":
             fields = None
@@ -87,16 +84,15 @@
             fields = ()
 
         self.fields = fields  # type: ignore
         # Leave the constructor to avoid variable shadowing between
         # this fields and the from marshmallow import fields above
         self.build_schema(model)
 
-    def build_schema(self, model: Type[Any]) -> None:
-
+    def build_schema(self, model: type[Any]) -> None:
         # Get the full list of parent classes from model to object
         classes = inspect.getmro(model)
 
         starting_point = False
         # Iterate in reversed order to start from object
         for c in reversed(classes):
             # Skip all parentes up to StructuredNode and StructuredRel (included)
```

### Comparing `rapydo_http-2.4/restapi/rest/annotations.py` & `rapydo_http-3.0/restapi/rest/annotations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Any, List, Optional
+from typing import Any, Optional
 
 from flask_apispec.utils import Annotation
 
 
-def inject_apispec_docs(fn: Any, conf: Any, labels: Optional[List[str]]) -> None:
-
+def inject_apispec_docs(fn: Any, conf: Any, labels: Optional[list[str]]) -> None:
     # retrieve attributes already set with @docs decorator
     fn.__apispec__ = fn.__dict__.get("__apispec__", {})
     docs = {}
     # it is normally available after loading the endpoint
     # but it is still un-initialized when using the @endpoint decorator
     if "docs" not in fn.__apispec__:
         fn.__apispec__["docs"] = []
```

### Comparing `rapydo_http-2.4/restapi/rest/bearer.py` & `rapydo_http-3.0/restapi/rest/bearer.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,79 +6,65 @@
 'Authorization: Bearer ' + tokenString to the HTTP header;
 cf. RFC6749 section 7.1.
 
 Note that anyone can validate a token as it is a bearer token:
 there is no client id nor is client authentication required.
 """
 
+from collections.abc import Iterable
 from functools import wraps
-from typing import Any, Callable, Iterable, Optional, Tuple, Union, cast
+from typing import Any, Callable, Optional, Union, cast
 
 from flask import request
+from werkzeug.datastructures import Authorization
 
 from restapi.customizer import FlaskRequest
 from restapi.env import Env
 from restapi.services.authentication import (
     ALL_ROLES,
     ANY_ROLE,
     BaseAuthentication,
     Role,
 )
 from restapi.types import EndpointFunction
 from restapi.utilities import print_and_exit
 from restapi.utilities.logs import log
 from restapi.utilities.meta import Meta
 
-HTTPAUTH_SCHEME = "Bearer"
+HTTPAUTH_SCHEME = "bearer"
 HTTPAUTH_AUTH_FIELD = "Authorization"
 # Base header for errors
 HTTPAUTH_ERR_HEADER = {
     "WWW-Authenticate": f'{HTTPAUTH_SCHEME} realm="Authentication Required"'
 }
 ALLOW_ACCESS_TOKEN_PARAMETER = Env.get_bool("ALLOW_ACCESS_TOKEN_PARAMETER")
 TOKEN_VALIDATED_KEY = "TOKEN_VALIDATED"
 
 
 class HTTPTokenAuth:
-    """
-    A class to implement a Generic Token (oauth2-like) authentication.
-    Started on a draft of the great miguel: http://bit.ly/2nTqQKA
-    """
-
     @staticmethod
     def get_authorization_token(
         allow_access_token_parameter: bool = False,
-    ) -> Tuple[Optional[str], Optional[str]]:
-        # Basic authenticaton is now allowed
+    ) -> tuple[Optional[str], Optional[str]]:
         if request.authorization is not None:
-            return None, None
-
-        if HTTPAUTH_AUTH_FIELD in request.headers:
-            # Flask/Werkzeug do not recognize any authentication types
-            # other than Basic or Digest, so here we parse the header by hand
-            try:
-                auth_header: str = request.headers.get(HTTPAUTH_AUTH_FIELD, "")
-                # Do not return directly auth_header.split
-                # Otherwise in case of malformed tokens the exception will be raised
-                # outside this function and probably not properly catched
-                # e.g. {'Authorization': 'Bearer'}  # no token provided
-                # will raise not enough values to unpack (expected 2, got 1)
-                auth_type, token = auth_header.split(None, 1)
-                return auth_type, token
-            except ValueError:
-                # The Authorization header is either empty or has no token
+            auth_type = request.authorization.type
+            token = request.authorization.token
+            return auth_type, token
+        elif HTTPAUTH_AUTH_FIELD in request.headers:
+            parsed_auth_header = Authorization.from_header(
+                request.headers.get(HTTPAUTH_AUTH_FIELD)
+            )
+            if parsed_auth_header is None:
                 return None, None
-
+            auth_type = parsed_auth_header.type
+            token = parsed_auth_header.token
         elif ALLOW_ACCESS_TOKEN_PARAMETER or allow_access_token_parameter:
-
             if not (token := request.args.get("access_token", "")):
                 return None, None
-
             return HTTPAUTH_SCHEME, token
-
         return None, None
 
     @staticmethod
     def is_session_user_admin(request: FlaskRequest, auth: BaseAuthentication) -> bool:
         if not request:
             return False
 
@@ -117,15 +103,14 @@
                     )
 
                 if (
                     auth_type is not None
                     and auth_type == HTTPAUTH_SCHEME
                     and request.method != "OPTIONS"
                 ):
-
                     # valid, token, jti, user
                     valid, token, _, user = caller.auth.verify_token(token)
 
                     # Check authentication. Optional authentication is valid if:
                     # 1) token is missing
                     # 2) token is valid
                     # Invalid tokens are rejected
@@ -219,15 +204,14 @@
                     return caller.response(
                         msg, code=401, headers=HTTPAUTH_ERR_HEADER, allow_html=True
                     )
 
                 # Handling OPTIONS forwarded to our application:
                 # ignore headers and let go, avoid unwanted interactions with CORS
                 if request.method != "OPTIONS":
-
                     # valid, token, jti, user
                     valid, token, _, user = caller.auth.verify_token(token)
                     # Check authentication
                     if not valid:
                         # Clear TCP receive buffer of any pending data
                         _ = request.data
                         # Mimic the response from a normal endpoint
```

### Comparing `rapydo_http-2.4/restapi/rest/definition.py` & `rapydo_http-3.0/restapi/rest/definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import Any, Dict, List, Optional
+from typing import Any, Optional
 
 from flask import Response as FlaskResponse
 from flask import request
 from flask.views import MethodView
 from flask_apispec import MethodResource
 
 from restapi.connectors import Connector
@@ -18,16 +18,15 @@
 PERPAGE_KEY = "perpage"
 DEFAULT_PERPAGE = 10
 
 
 # Base type MethodResource becomes "Any" due to an unfollowed import
 # Base type Resource becomes "Any" due to an unfollowed import
 class EndpointResource(MethodResource, MethodView):  # type: ignore
-
-    depends_on: List[str] = []
+    depends_on: list[str] = []
     labels = ["undefined"]
     private = False
     events = Events
 
     def __init__(self) -> None:
         super().__init__()
 
@@ -53,20 +52,19 @@
         )
         return self.auth.get_user(user_id=self.authorized_user)
 
     @staticmethod
     def response(
         content: ResponseContent = None,
         code: Optional[int] = None,
-        headers: Optional[Dict[str, str]] = None,
+        headers: Optional[dict[str, str]] = None,
         head_method: bool = False,
         allow_html: bool = False,
         force_json: bool = False,
     ) -> Response:
-
         if headers is None:
             headers = {}
 
         if code is None:
             code = 200
 
         if content is None and code != 204 and not head_method:
@@ -108,18 +106,17 @@
         Cache.invalidate(self.get)
 
     # Mostly copied in authentication.py
     def log_event(
         self,
         event: Events,
         target: Optional[Any] = None,
-        payload: Optional[Dict[str, Any]] = None,
+        payload: Optional[dict[str, Any]] = None,
         user: Optional[Any] = None,
     ) -> None:
-
         if not user:
             user = self.auth.get_user(user_id=self.authorized_user)
 
         save_event_log(
             event=event,
             target=target,
             payload=payload,
```

### Comparing `rapydo_http-2.4/restapi/rest/loader.py` & `rapydo_http-3.0/restapi/rest/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 
 Customization based on configuration 'blueprint' files
 """
 
 import re
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Set, Tuple, Type, get_type_hints
+from typing import Any, Optional, get_type_hints
 
 from attr import ib as attribute
 from attr import s as ClassOfAttributes
 
 from restapi import decorators
 from restapi.config import ABS_RESTAPI_PATH, CONF_PATH, CUSTOM_PACKAGE
 from restapi.env import Env
@@ -28,40 +28,39 @@
 ERR404_AUTH = {"description": "The resource cannot be found or you are not authorized"}
 
 uri_pattern = re.compile(r"\<([^\>]+)\>")
 
 
 @ClassOfAttributes
 class EndpointElements:
-    cls: Type[EndpointResource] = attribute(default=None)
-    uris: Set[str] = attribute(default=set())
+    cls: type[EndpointResource] = attribute(default=None)
+    uris: set[str] = attribute(default=set())
     # {'method': path, 'get': path, 'post': path}
-    methods: Dict[str, str] = attribute(default={})
-    tags: List[str] = attribute(default=[])
+    methods: dict[str, str] = attribute(default={})
+    tags: list[str] = attribute(default=[])
     private: bool = attribute(default=False)
 
 
 class EndpointsLoader:
     def __init__(self) -> None:
-
         # Used by server.py to load endpoints definitions
-        self.endpoints: List[EndpointElements] = []
+        self.endpoints: list[EndpointElements] = []
         # Used by server.py to remove unmapped methods
-        self.uri2methods: Dict[str, List[str]] = {}
+        self.uri2methods: dict[str, list[str]] = {}
         # Used by server.py to configure ApiSpec
-        self.tags: List[Dict[str, str]] = []
+        self.tags: list[dict[str, str]] = []
 
         # Used by swagger specs endpoints to show authentication info
-        self.authenticated_endpoints: Dict[str, Dict[str, bool]] = {}
+        self.authenticated_endpoints: dict[str, dict[str, bool]] = {}
         # Used by swagger spec endpoint to remove private endpoints from public requests
-        self.private_endpoints: Dict[str, Dict[str, bool]] = {}
+        self.private_endpoints: dict[str, dict[str, bool]] = {}
 
-        self._used_tags: Set[str] = set()
+        self._used_tags: set[str] = set()
 
-    def load_configuration(self) -> Dict[str, Any]:
+    def load_configuration(self) -> dict[str, Any]:
         # Reading configuration
 
         CONF_FOLDERS = Env.load_variables_group(prefix="project_confs")
         defaults_path = Path(CONF_FOLDERS.get("defaults_path", CONF_PATH))
         base_path = Path(CONF_FOLDERS.get("base_path", CONF_PATH))
         projects_path = Path(CONF_FOLDERS.get("projects_path", CONF_PATH))
         submodules_path = Path(CONF_FOLDERS.get("submodules_path", CONF_PATH))
@@ -75,15 +74,14 @@
             )
         except AttributeError as e:  # pragma: no cover
             print_and_exit(str(e))
 
         return configuration
 
     def load_endpoints(self) -> None:
-
         # core endpoints folder (rapydo/http-api)
         self.load_endpoints_folder(ABS_RESTAPI_PATH)
 
         # endpoints folder from extended project, if any
         if self._extended_project is not None:
             self.load_endpoints_folder(Path(self._extended_project))
 
@@ -94,15 +92,15 @@
         self.tags = EndpointsLoader.remove_unused_tags(
             mem.configuration["tags"], self._used_tags
         )
 
         self.detect_endpoints_shadowing()
 
     @staticmethod
-    def skip_endpoint(depends_on: List[str]) -> Tuple[bool, Optional[str]]:
+    def skip_endpoint(depends_on: list[str]) -> tuple[bool, Optional[str]]:
         for var in depends_on:
             pieces = var.strip().split(" ")
             pieces_num = len(pieces)
             if pieces_num == 1:
                 dependency = pieces.pop()
                 negate = False
             elif pieces_num == 2:
@@ -117,25 +115,23 @@
 
             # Skip if not meeting the requirements of the dependency
             if not check:
                 return True, dependency
 
         return False, None
 
-    def extract_endpoints(self, base_dir: Path) -> List[Type[EndpointResource]]:
-
-        endpoints_classes: List[Type[EndpointResource]] = []
+    def extract_endpoints(self, base_dir: Path) -> list[type[EndpointResource]]:
+        endpoints_classes: list[type[EndpointResource]] = []
         # get last item of the path
         # normpath is required to strip final / if any
         base_module = base_dir.name
 
         apis_dir = base_dir.joinpath("endpoints")
         apiclass_module = f"{base_module}.endpoints"
         for epfile in apis_dir.glob("*.py"):
-
             # get module name (es: endpoints.filename)
 
             module_name = f"{apiclass_module}.{epfile.stem}"
             # Convert module name into a module
             log.debug("Importing {}", module_name)
             module = Meta.get_module_from_string(
                 module_name,
@@ -170,30 +166,28 @@
 
         return endpoints_classes
 
     def load_endpoints_folder(self, base_dir: Path) -> None:
         # Walk folders looking for endpoints
 
         for epclss in self.extract_endpoints(base_dir):
-
             if not epclss.methods:  # pragma: no cover
                 continue
 
             # Building endpoint
             endpoint = EndpointElements(
                 uris=set(),
                 methods={},
                 cls=epclss,
                 tags=epclss.labels,
                 private=epclss.private,
             )
 
             # m = GET|PUT|POST|DELETE|PATCH|...
             for m in epclss.methods:
-
                 # method_fn = get|post|put|delete|patch|...
                 method_fn = m.lower()
 
                 # get, post, put, patch, delete functions
                 fn = getattr(epclss, method_fn)
 
                 # Adding the catch_exceptions decorator to every endpoint
@@ -214,15 +208,14 @@
                     else:
                         expected_annotation = Optional[User]
 
                     if (
                         "user" not in parameters
                         or parameters["user"] != expected_annotation
                     ):  # pragma: no cover
-
                         if "user" in parameters:
                             log.critical(
                                 "Wrong user parameter in {}.{} (function {}), "
                                 "expected {} but found {}",
                                 epclss.__name__,
                                 method_fn,
                                 fn.__name__,
@@ -259,15 +252,15 @@
                 self.authenticated_endpoints.setdefault(fn.uri, {})
                 # method_fn is equivalent to m.lower()
                 self.authenticated_endpoints[fn.uri].setdefault(
                     method_fn, auth_required
                 )
 
                 # Set default responses
-                responses: Dict[str, Dict[str, str]] = {}
+                responses: dict[str, dict[str, str]] = {}
 
                 responses.setdefault("400", ERR400)
                 if auth_required:
                     responses.setdefault("401", ERR401)
                     responses.setdefault("404", ERR404_AUTH)
                 elif auth_optional:
                     responses.setdefault("401", ERR401)
@@ -289,32 +282,32 @@
                 self.uri2methods[fn.uri].append(method_fn)
 
                 self._used_tags.update(endpoint.tags)
             self.endpoints.append(endpoint)
 
     @staticmethod
     def remove_unused_tags(
-        all_tags: Dict[str, str], used_tags: Set[str]
-    ) -> List[Dict[str, str]]:
-        tags: List[Dict[str, str]] = []
+        all_tags: dict[str, str], used_tags: set[str]
+    ) -> list[dict[str, str]]:
+        tags: list[dict[str, str]] = []
         for tag, desc in all_tags.items():
             if tag not in used_tags:  # pragma: no cover
                 log.debug("Skipping unsed tag: {}", tag)
                 continue
             tags.append({"name": tag, "description": desc})
         return tags
 
     def detect_endpoints_shadowing(self) -> None:
         # Verify mapping duplication or shadowing
         # Example of shadowing:
         # /xyz/<variable>
         # /xyz/abc
         # The second endpoint is shadowed by the first one
-        mappings: Dict[str, Set[str]] = {}
-        classes: Dict[str, Dict[str, Type[EndpointResource]]] = {}
+        mappings: dict[str, set[str]] = {}
+        classes: dict[str, dict[str, type[EndpointResource]]] = {}
         # duplicates are found while filling the dictionaries
         for endpoint in self.endpoints:
             for method, uri in endpoint.methods.items():
                 mappings.setdefault(method, set())
                 classes.setdefault(method, {})
 
                 if uri in mappings[method]:  # pragma: no cover
```

### Comparing `rapydo_http-2.4/restapi/rest/response.py` & `rapydo_http-3.0/restapi/rest/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import decimal
 import gzip
 import sys
 import time
 from datetime import date, datetime
+from decimal import Decimal
 from io import BytesIO
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, cast
+from typing import Any, Optional, Union, cast
 from urllib import parse as urllib_parse
 
 import orjson
 from flask import Response as FlaskResponse
 from flask import jsonify, render_template, request
-from flask.json import JSONEncoder
+from flask.json.provider import JSONProvider
 from marshmallow import fields as marshmallow_fields
 from marshmallow.utils import _Missing
 from werkzeug.exceptions import HTTPException
 
 from restapi import __version__ as version
 from restapi.config import (
     GZIP_ENABLE,
@@ -25,55 +25,50 @@
 )
 from restapi.models import GET_SCHEMA_KEY, Schema, fields, validate
 from restapi.services.authentication import BaseAuthentication
 from restapi.types import Response, ResponseContent
 from restapi.utilities.logs import handle_log_output, log, obfuscate_dict
 
 
-def jsonifier(content: Any) -> Any:
-    if isinstance(content, set):
-        return jsonifier(list(content))
-    if isinstance(content, (datetime, date)):
-        return jsonifier(content.isoformat())
-    if isinstance(content, decimal.Decimal):
-        return jsonifier(float(content))
-    if isinstance(content, Path):
-        return jsonifier(str(content))
-
-    return orjson.dumps(content).decode("UTF8")
-
-
-class ExtendedJSONEncoder(JSONEncoder):
-    def default(self, o: Any) -> Any:
-        if isinstance(o, set):
-            return list(o)
-        if isinstance(o, (datetime, date)):
-            return o.isoformat()
-        if isinstance(o, decimal.Decimal):
-            return float(o)
-        if isinstance(o, Path):
-            return str(o)
-        # Otherwise: TypeError: Object of type xxx is not JSON serializable
-        return super().default(o)  # pragma: no cover
+def jsonifier(content: Any) -> str:
+    def default(obj: Any) -> Any:
+        if isinstance(obj, set):
+            return list(obj)
+        if isinstance(obj, (datetime, date)):  # pragma: no cover
+            return obj.isoformat()
+        if isinstance(obj, Decimal):
+            return float(obj)
+        if isinstance(obj, Path):
+            return str(obj)
+        raise TypeError  # pragma: no cover
+
+    return orjson.dumps(
+        content, default=default, option=orjson.OPT_NON_STR_KEYS
+    ).decode("UTF8")
+
+
+class ExtendedJSONEncoder(JSONProvider):
+    def dumps(self, obj: Any, **kwargs: Any) -> str:
+        return jsonifier(obj)
 
+    def loads(self, s: Union[str, bytes], **kwargs: Any) -> Any:
+        return orjson.loads(s)
 
-def handle_http_errors(error: HTTPException) -> Response:
 
+def handle_http_errors(error: HTTPException) -> Response:
     return FlaskResponse(
         jsonifier({"message": error.description}),
         status=error.code,
         mimetype="application/json",
         headers={"Content-Type": "application/json"},
     )
 
 
 def handle_marshmallow_errors(error: HTTPException) -> Response:
-
     try:
-
         if request.args:
             if request.args.get(GET_SCHEMA_KEY, False):  # pragma: no cover
                 schema = cast(Schema, error.data.get("schema"))  # type: ignore
                 return ResponseMaker.respond_with_schema(schema)
 
         elif j := request.get_json():
             if j.get(GET_SCHEMA_KEY, False):  # pragma: no cover
@@ -87,15 +82,15 @@
 
     except Exception as e:  # pragma: no cover
         log.error(e)
 
     errors = {}
 
     error_messages = cast(
-        Dict[str, Dict[str, str]], error.data.get("messages")  # type: ignore
+        dict[str, dict[str, str]], error.data.get("messages")  # type: ignore
     )
     for key, messages in error_messages.items():
         for k, msg in messages.items():
             if not msg:  # pragma: no cover
                 continue
             log.error("[{}] {}: {}", key, k, msg)
             errors[k] = msg
@@ -140,15 +135,14 @@
     except Exception as e:  # pragma: no cover
         log.debug(e)
 
     return ""
 
 
 def handle_response(response: FlaskResponse) -> FlaskResponse:
-
     response.headers["_RV"] = str(version)
 
     PROJECT_VERSION = get_project_configuration("project.version", default="0")
     if PROJECT_VERSION is not None:
         response.headers["Version"] = str(PROJECT_VERSION)
 
     data_string = get_data_from_request()
@@ -196,19 +190,18 @@
             resp,
         )
 
     return response
 
 
 class ResponseMaker:
-
     # Have a look here: (from flask import request)
     # request.user_agent.browser
     @staticmethod
-    def get_accepted_formats() -> List[str]:
+    def get_accepted_formats() -> list[str]:
         """
         Possible outputs:
         '*/*'
         'application/json'
         'text/html'
         'application/xml'
         'text/csv'
@@ -242,17 +235,16 @@
             return True
 
         log.warning("Unknown Content-Type: {}", content_type)
         return False
 
     @staticmethod
     def get_html(
-        content: ResponseContent, code: int, headers: Dict[str, str]
-    ) -> Tuple[str, Dict[str, str]]:
-
+        content: ResponseContent, code: int, headers: dict[str, str]
+    ) -> tuple[str, dict[str, str]]:
         if isinstance(content, list):  # pragma: no cover
             content = content.pop()
 
         headers["Content-Type"] = "text/html; charset=UTF-8"
 
         html_data = {"body_content": content, "is_error": code >= 400}
         html_page = render_template("index.html", **html_data)
@@ -261,15 +253,15 @@
 
     @staticmethod
     def gzip_response(
         content: bytes,
         code: int,
         content_encoding: Optional[str],
         content_type: Optional[str],
-    ) -> Tuple[Optional[bytes], Dict[str, str]]:
+    ) -> tuple[Optional[bytes], dict[str, str]]:
         if code < 200 or code >= 300 or content_encoding is not None:
             return None, {}
 
         # Do not compress binary contents (like images) due to small benefits expected
         if ResponseMaker.is_binary(content_type):  # pragma: no cover
             # log.warning("Skipping gzip compression on {}", content_type)
             return None, {}
@@ -318,20 +310,18 @@
                 "Small benefit due to gzip compression on Content-Type: {} ({:.2f} %)",
                 content_type,
                 100 * ratio,
             )
         return gzipped_content, headers
 
     @staticmethod
-    def convert_model_to_schema(schema: Schema) -> List[Dict[str, Any]]:
-
+    def convert_model_to_schema(schema: Schema) -> list[dict[str, Any]]:
         schema_fields = []
         for field, field_def in schema.declared_fields.items():
-
-            f: Dict[str, Any] = {}
+            f: dict[str, Any] = {}
 
             f["key"] = field_def.data_key or field
 
             if "label" in field_def.metadata:
                 f["label"] = field_def.metadata["label"]
             elif f["key"] == f["key"].lower():
                 f["label"] = f["key"].title()
@@ -365,55 +355,51 @@
                 f["autocomplete_label_bind"] = autocomplete_label_bind
 
             if not isinstance(field_def.dump_default, _Missing):
                 f["default"] = field_def.dump_default
             elif not isinstance(field_def.load_default, _Missing):  # pragma: no cover
                 f["default"] = field_def.load_default
 
-            validators: List[validate.Validator] = []
+            validators: list[validate.Validator] = []
             if field_def.validate:
                 validators.append(field_def.validate)  # type: ignore
 
             # activated in case of fields.List(fields.SomeThing) with an inner validator
             if isinstance(field_def, fields.List) and field_def.inner.validate:
                 validators.append(field_def.inner.validate)
 
             for validator in validators:
                 if isinstance(validator, validate.Length):
-
                     if validator.min is not None:
                         f["min"] = validator.min
                     if validator.max is not None:
                         f["max"] = validator.max
                     if validator.equal is not None:
                         f["min"] = validator.equal
                         f["max"] = validator.equal
 
                 elif isinstance(validator, validate.Range):
-
                     if validator.min is not None:
                         f["min"] = validator.min
                         if not validator.min_inclusive:
                             f["min"] += 1
 
                     if validator.max is not None:
                         f["max"] = validator.max
                         if not validator.max_inclusive:
                             f["max"] -= 1
 
                 elif isinstance(validator, validate.OneOf):
-
                     choices = validator.choices
                     labels = validator.labels
                     if len(tuple(labels)) != len(tuple(choices)):
                         labels = choices
                     f["options"] = dict(zip(choices, labels))
 
                 else:  # pragma: no cover
-
                     log.warning(
                         "Unsupported validation schema: {}.{}",
                         type(validator).__module__,
                         type(validator).__name__,
                     )
 
             if f["type"] == "nested":
@@ -422,28 +408,26 @@
                 )
 
             schema_fields.append(f)
         return schema_fields
 
     @staticmethod
     def respond_with_schema(schema: Schema) -> Response:
-
         try:
             fields = ResponseMaker.convert_model_to_schema(schema)
             return (jsonify(fields), 200, {})
         except Exception as e:  # pragma: no cover
             log.error(e)
             content = {"Server internal error": "Failed to retrieve input schema"}
             return (jsonify(content), 500, {})
 
     @staticmethod
     def get_schema_type(
         field: str, schema: marshmallow_fields.Field, default: Optional[Any] = None
     ) -> str:
-
         if schema.metadata.get("password", False):
             return "password"
         # types from https://github.com/danohu/py2ng
         # https://github.com/danohu/py2ng/blob/master/py2ng/__init__.py
         if isinstance(schema, fields.Bool) or isinstance(schema, fields.Boolean):
             return "boolean"
         if isinstance(schema, fields.Date):
```

### Comparing `rapydo_http-2.4/restapi/server.py` & `rapydo_http-3.0/restapi/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 The Main server factory. All internal flask components are created here
 """
+
 import logging
 import signal
 import sys
 import time
 import warnings
 from enum import Enum
 from threading import Lock
 from types import FrameType
-from typing import Dict, Optional
+from typing import Optional
 
 import werkzeug.exceptions
 from apispec import APISpec
 from apispec.ext.marshmallow import MarshmallowPlugin
 from flask import Flask
 from flask_apispec import FlaskApiSpec
 from flask_cors import CORS
@@ -65,35 +66,34 @@
 # def inspect_request():
 #     log.critical(request.headers)
 
 
 def teardown_handler(
     signal: int, frame: Optional[FrameType]
 ) -> None:  # pragma: no cover
-
     with lock:
-
         Connector.disconnect_all()
 
     # This is needed to let connectors to complete the disconnection and prevent
     # errors like this on rabbitMQ:
     # closing AMQP connection <0.2684.0> ([...], vhost: '/', user: [...]):
     # client unexpectedly closed TCP connection
     time.sleep(1)
     print("Disconnection completed")
     sys.exit(0)
 
 
 def create_app(
-    name: str = __name__,
-    mode: ServerModes = ServerModes.NORMAL,
-    options: Optional[Dict[str, bool]] = None,
+    name: str,
+    mode: ServerModes,
+    options: dict[str, bool],
 ) -> Flask:
     """Create the server istance for Flask application"""
 
+    mem.boot_completed = False
     if PRODUCTION and TESTING and not FORCE_PRODUCTION_TESTS:  # pragma: no cover
         print_and_exit("Unable to execute tests in production")
 
     # TERM is not catched by Flask
     # https://github.com/docker/compose/issues/4199#issuecomment-426109482
     # signal.signal(signal.SIGTERM, teardown_handler)
     # SIGINT is registered as STOPSIGNAL in Dockerfile
@@ -101,15 +101,14 @@
 
     # Flask app instance
     # template_folder = template dir for output in HTML
     flask_app = Flask(name, template_folder=str(ABS_RESTAPI_PATH.joinpath("templates")))
 
     # CORS
     if not PRODUCTION:
-
         if TESTING:
             cors_origin = "*"
         else:  # pragma: no cover
             cors_origin = get_frontend_url()
             # Beware, this only works because get_frontend_url never append a port
             cors_origin += ":*"
 
@@ -128,19 +127,15 @@
             resources={r"*": {"origins": cors_origin}},
         )
 
         log.debug("CORS Enabled")
 
     # Flask configuration from config file
     flask_app.config.from_object(config)
-    flask_app.json_encoder = ExtendedJSONEncoder
-
-    # Used to force flask to avoid json sorting and ensure that
-    # the output to reflect the order of field in the Marshmallow schema
-    flask_app.config["JSON_SORT_KEYS"] = False
+    flask_app.json = ExtendedJSONEncoder(flask_app)
 
     log.debug("Flask app configured")
 
     if PRODUCTION:
         log.info("Production server mode is ON")
 
     endpoints_loader = EndpointsLoader()
@@ -152,15 +147,14 @@
         log.critical("Loading Mocked Initializer and Customizer classes")
         from restapi.mocks import Customizer, Initializer
 
         mem.initializer = Initializer
         mem.customizer = Customizer()
 
     else:
-
         mem.configuration = endpoints_loader.load_configuration()
         mem.initializer = Meta.get_class("initialization", "Initializer")
         if not mem.initializer:  # pragma: no cover
             print_and_exit("Invalid Initializer class")
 
         customizer = Meta.get_class("customization", "Customizer")
         if not customizer:  # pragma: no cover
@@ -176,15 +170,14 @@
         Connector.project_init(options=options)
 
     if mode == ServerModes.DESTROY:
         Connector.project_clean()
 
     # Restful plugin with endpoint mapping (skipped in INIT|DESTROY|WORKER modes)
     if mode == ServerModes.NORMAL:
-
         logging.getLogger("werkzeug").setLevel(logging.ERROR)
 
         # warnings levels:
         # default  # Warn once per call location
         # error    # Convert to exceptions
         # always   # Warn every time
         # module   # Warn once per calling module
@@ -221,20 +214,14 @@
             warnings.simplefilter("error", UnicodeWarning)
             warnings.simplefilter("error", BytesWarning)
             # Can't set this an error due to false positives with downloads
             # a lot of issues like: https://github.com/pallets/flask/issues/2468
             warnings.simplefilter("always", ResourceWarning)
             warnings.simplefilter("default", Neo4jExperimentalWarning)
 
-            # Remove me in a near future, this is due to hypothesis with pytest 7
-            # https://github.com/HypothesisWorks/hypothesis/issues/3222
-            warnings.filterwarnings(
-                "ignore", message="A private pytest class or function was used."
-            )
-
         elif PRODUCTION:  # pragma: no cover
             warnings.simplefilter("ignore", Warning)
             warnings.simplefilter("always", UserWarning)
             warnings.simplefilter("default", DeprecationWarning)
             warnings.simplefilter("ignore", SyntaxWarning)
             warnings.simplefilter("ignore", RuntimeWarning)
             warnings.simplefilter("ignore", FutureWarning)
@@ -266,33 +253,25 @@
         warnings.filterwarnings(
             "ignore", message="Multiple schemas resolved to the name "
         )
 
         # ignore warning messages on flask socket after teardown
         warnings.filterwarnings("ignore", message="unclosed <socket.socket")
 
-        # from flask_caching 1.10.1 with python 3.10 on core tests...
-        # try to remove this once upgraded flask_caching in a near future
-        warnings.filterwarnings(
-            "ignore",
-            message="_SixMetaPathImporter.find_spec",
-        )
-
         # Raised from sentry_sdk 1.5.11 with python 3.10 events
         warnings.filterwarnings(
             "ignore",
             message="SelectableGroups dict interface is deprecated. Use select.",
         )
 
-        # Raised from apispec 5.2.2 with setuptools 65
+        # Raise from neo4j 5
         warnings.filterwarnings(
             "ignore",
-            message="distutils Version classes are deprecated.",
+            message="Relying on Driver's destructor to close the session is deprecated.",
         )
-
         if Connector.check_availability("redis"):
             mem.cache = Cache.get_instance(flask_app)
 
         endpoints_loader.load_endpoints()
         mem.authenticated_endpoints = endpoints_loader.authenticated_endpoints
         mem.private_endpoints = endpoints_loader.private_endpoints
 
@@ -343,15 +322,14 @@
 
         mem.docs = FlaskApiSpec(flask_app)
 
         # Clean app routes
         ignore_verbs = {"HEAD", "OPTIONS"}
 
         for rule in flask_app.url_map.iter_rules():
-
             view_function = flask_app.view_functions[rule.endpoint]
             if not hasattr(view_function, "view_class"):
                 continue
 
             newmethods = ignore_verbs.copy()
             rulename = str(rule)
 
@@ -382,15 +360,14 @@
     flask_app.register_error_handler(500, handle_http_errors)
 
     # flask_app.before_request(inspect_request)
     # Logging responses
     flask_app.after_request(handle_response)
 
     if SENTRY_URL is not None:  # pragma: no cover
-
         if PRODUCTION:
             sentry_sdk_init(
                 dsn=SENTRY_URL,
                 # already catched by handle_marshmallow_errors
                 ignore_errors=[werkzeug.exceptions.UnprocessableEntity],
                 integrations=[FlaskIntegration()],
             )
@@ -412,8 +389,9 @@
                 ),
                 "rapydo": restapi_version,
             },
             user=None,
             target=None,
         )
 
+    mem.boot_completed = True
     return flask_app
```

### Comparing `rapydo_http-2.4/restapi/services/authentication.py` & `rapydo_http-3.0/restapi/services/authentication.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,26 @@
 import base64
 import re
 from abc import ABCMeta, abstractmethod
 from datetime import datetime, timedelta
 from enum import Enum
-from functools import lru_cache
 from io import BytesIO
 from pathlib import Path
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    TypedDict,
-    Union,
-    cast,
-)
+from typing import TYPE_CHECKING, Any, Optional, TypedDict, Union, cast
 
+import bcrypt
 import jwt
 import pyotp
 import pytz
 import segno
 from cryptography.fernet import Fernet
 from cryptography.fernet import InvalidToken as InvalidFernetToken
 from flask import request
 from glom import glom
 from jwt.exceptions import ExpiredSignatureError, ImmatureSignatureError
-from passlib.context import CryptContext
 
 from restapi.config import (
     BACKEND_HOSTNAME,
     HOST_TYPE,
     JWT_SECRET_FILE,
     PRODUCTION,
     PROXIED_CONNECTION,
@@ -50,15 +39,15 @@
     ServiceUnavailable,
     Unauthorized,
 )
 from restapi.types import Props
 from restapi.utilities import print_and_exit
 from restapi.utilities.globals import mem
 from restapi.utilities.logs import Events, log, save_event_log
-from restapi.utilities.time import EPOCH, get_now
+from restapi.utilities.time import EPOCH
 from restapi.utilities.uuid import getUUID
 
 # Trick to avoid circular dependencies
 if TYPE_CHECKING:  # pragma: no cover
     from restapi.connectors import Connector
 User = Any
 Group = Any
@@ -67,31 +56,28 @@
 
 
 class AuthMissingTOTP(Exception):
     pass
 
 
 def import_secret(abs_filename: Path) -> bytes:
-
     if HOST_TYPE != BACKEND_HOSTNAME:  # pragma: no cover
         return Fernet.generate_key()
 
     try:
         return open(abs_filename, "rb").read()
     # Can't be covered because it is execute once before the tests...
     except OSError:  # pragma: no cover
         key = Fernet.generate_key()
         with open(abs_filename, "wb") as key_file:
             key_file.write(key)
         abs_filename.chmod(0o400)
         return key
 
 
-pwd_context = CryptContext(schemes=["bcrypt"], deprecated="auto")
-
 ALL_ROLES = "all"
 ANY_ROLE = "any"
 ROLE_DISABLED = "disabled"
 DEFAULT_GROUP_NAME = "Default"
 DEFAULT_GROUP_DESCR = "Default group"
 
 DISABLE_UNUSED_CREDENTIALS_AFTER_MIN_TESTNIG_VALUE = 60
@@ -143,47 +129,43 @@
 class InvalidToken(Exception):
     pass
 
 
 # ##############################################################################
 # Utility functions used to adapt security settings to Testable values
 def get_timedelta(val: int, min_testing_val: int = 0) -> Optional[timedelta]:
-
     if val == 0:
         return None
 
     if TESTING:
         return timedelta(seconds=max(val, min_testing_val))
     # Of course cannot be tested
     return timedelta(days=val)  # pragma: no cover
 
 
 def get_max_login_attempts(val: int) -> int:
-
     if TESTING and val:
         # min 10 failures, otherwise normal tests will start to fail
         return max(val, MAX_LOGIN_ATTEMPTS_MIN_TESTING_VALUE)
 
     return val
 
 
 def get_login_ban_time(val: int) -> int:
-
     if TESTING and val:
         # max 10 seconds, otherwise tests will hang
         return min(val, LOGIN_BAN_TIME_MAX_TESTING_VALUE)
 
-    return val
+    return val  # pragma: no cover
 
 
 # ##############################################################################
 
 
 class BaseAuthentication(metaclass=ABCMeta):
-
     """
     An almost abstract class with methods
     to be implemented with a new service
     that aims to store credentials of users and roles.
     """
 
     JWT_SECRET: str = import_secret(JWT_SECRET_FILE).decode()
@@ -236,44 +218,42 @@
 
     FAILED_LOGINS_EXPIRATION: timedelta = timedelta(
         seconds=get_login_ban_time(Env.get_int("AUTH_LOGIN_BAN_TIME", 3600))
     )
 
     default_user: Optional[str] = None
     default_password: Optional[str] = None
-    roles: List[str] = []
-    roles_data: Dict[str, str] = {}
+    roles: list[str] = []
+    roles_data: dict[str, str] = {}
     default_role: str = Role.USER.value
-    role_descriptions: Dict[str, str] = {}
+    role_descriptions: dict[str, str] = {}
 
     # This is to let inform mypy about the existence of self.db
     def __init__(self) -> None:  # pragma: no cover
         self.db: "Connector"
 
     # Executed once by Connector in init_app
     @classmethod
     def module_initialization(cls) -> None:
         cls.load_default_user()
         cls.load_roles()
 
     @staticmethod
     def load_default_user() -> None:
-
         BaseAuthentication.default_user = Env.get("AUTH_DEFAULT_USERNAME", "")
         BaseAuthentication.default_password = Env.get("AUTH_DEFAULT_PASSWORD", "")
         if (
             not BaseAuthentication.default_user
             or not BaseAuthentication.default_password
         ):  # pragma: no cover
             print_and_exit("Default credentials are unavailable!")
 
     @staticmethod
     def load_roles() -> None:
-
-        empty_dict: Dict[str, str] = {}
+        empty_dict: dict[str, str] = {}
         BaseAuthentication.roles_data = glom(
             mem.configuration, "variables.roles", default=empty_dict
         ).copy()
         if not BaseAuthentication.roles_data:  # pragma: no cover
             print_and_exit("No roles configured")
 
         BaseAuthentication.default_role = BaseAuthentication.roles_data.pop(
@@ -290,29 +270,28 @@
         BaseAuthentication.roles = []
         for role, description in BaseAuthentication.roles_data.items():
             if description != ROLE_DISABLED:
                 BaseAuthentication.roles.append(role)
 
     def make_login(
         self, username: str, password: str, totp_code: Optional[str]
-    ) -> Tuple[str, Payload, User]:
-
+    ) -> tuple[str, Payload, User]:
         self.verify_blocked_username(username)
 
         try:
             user = self.get_user(username=username)
         except ValueError as e:  # pragma: no cover
             # SqlAlchemy can raise the following error:
             # A string literal cannot contain NUL (0x00) characters.
             log.error(e)
-            raise BadRequest("Invalid input received")
+            raise BadRequest("Invalid input received") from e
         except Exception as e:  # pragma: no cover
             log.error("Unable to connect to auth backend\n[{}] {}", type(e), e)
 
-            raise ServiceUnavailable("Unable to connect to auth backend")
+            raise ServiceUnavailable("Unable to connect to auth backend") from e
 
         if user is None:
             self.register_failed_login(username, user=None)
 
             self.log_event(
                 Events.failed_login,
                 payload={"username": username},
@@ -348,35 +327,46 @@
 
         self.save_login(username, user, failed=False)
         self.log_event(Events.login, user=user)
         return token, full_payload, user
 
     # #####################
     # # Password handling #
-    ####################
+    # #####################
     @staticmethod
-    def verify_password(plain_password: str, hashed_password: str) -> bool:
+    def is_bcrypt_hashed(password: str) -> bool:
         try:
-            return cast(bool, pwd_context.verify(plain_password, hashed_password))
-        except ValueError as e:  # pragma: no cover
-            log.error(e)
-
+            bcrypt.checkpw(b"password", password.encode("utf-8"))
+            return True
+        except ValueError:
             return False
 
     @staticmethod
+    def verify_password(plain_password: str, hashed_password: str) -> bool:
+        if not BaseAuthentication.is_bcrypt_hashed(hashed_password):
+            hashed_password = BaseAuthentication.get_password_hash(hashed_password)
+        password_byte_enc = plain_password.encode("utf-8", errors="strict")
+        hashed_password_byte_enc = hashed_password.encode("utf-8", errors="strict")
+        return bcrypt.checkpw(
+            password=password_byte_enc, hashed_password=hashed_password_byte_enc
+        )
+
+    @staticmethod
     def get_password_hash(password: Optional[str]) -> str:
         if not password:
             raise Unauthorized("Invalid password")
-        # CryptContext is no typed.. but this is a string!
-        return cast(str, pwd_context.hash(password))
+        hashed_password = bcrypt.hashpw(
+            password=password.encode("utf-8"),
+            salt=bcrypt.gensalt(),
+        ).decode("utf-8")
+        return hashed_password
 
     @staticmethod
     def get_remote_ip(raise_warnings: bool = True) -> str:
         try:
-
             # Syntax: X-Forwarded-For: <client>, <proxy1>, <proxy2>
             #   <client> The client IP address
             #   <proxy1>, <proxy2> If a request goes through multiple proxies, the
             #        IP addresses of each successive proxy is listed. This means, the
             #        right-most IP address is the IP address of the most recent proxy
             #        and the left-most IP address is the IP address of the originating
             #        client.
@@ -411,20 +401,20 @@
     # ###################
     # # Tokens handling #
     # ###################
     @classmethod
     def create_token(cls, payload: Payload) -> str:
         """Generate a str token with JWT library to encrypt the payload"""
         return jwt.encode(
-            cast(Dict[str, Any], payload), cls.JWT_SECRET, algorithm=cls.JWT_ALGO
+            cast(dict[str, Any], payload), cls.JWT_SECRET, algorithm=cls.JWT_ALGO
         )
 
     def create_temporary_token(
         self, user: User, token_type: str, duration: int = 86400
-    ) -> Tuple[str, Payload]:
+    ) -> tuple[str, Payload]:
         # invalidate previous tokens with same token_type
         for t in self.get_tokens(user=user):
             ttype = t.get("token_type")
             if ttype is None:  # pragma: no cover
                 continue
             if ttype != token_type:
                 continue
@@ -440,15 +430,14 @@
         token = self.create_token(payload)
         return token, full_payload
 
     @classmethod
     def unpack_token(
         cls, token: str, raiseErrors: bool = False
     ) -> Optional[DecodedPayload]:
-
         try:
             return cast(
                 DecodedPayload,
                 jwt.decode(token, cls.JWT_SECRET, algorithms=[cls.JWT_ALGO]),
             )
         # now > exp
         except ExpiredSignatureError as e:
@@ -473,24 +462,23 @@
 
     @staticmethod
     def unpacked_token(
         valid: bool,
         token: Optional[str] = None,
         jti: Optional[str] = None,
         user: Optional[User] = None,
-    ) -> Tuple[bool, Optional[str], Optional[str], Optional[User]]:
+    ) -> tuple[bool, Optional[str], Optional[str], Optional[User]]:
         return (valid, token, jti, user)
 
     def verify_token(
         self,
         token: Optional[str],
         raiseErrors: bool = False,
         token_type: Optional[str] = None,
-    ) -> Tuple[bool, Optional[str], Optional[str], Optional[User]]:
-
+    ) -> tuple[bool, Optional[str], Optional[str], Optional[User]]:
         if token is None:
             if raiseErrors:
                 raise InvalidToken("Missing token")
             return self.unpacked_token(False)
 
         # Decode the current token
         payload = self.unpack_token(token, raiseErrors=raiseErrors)
@@ -529,15 +517,15 @@
         return self.unpacked_token(True, token=token, jti=payload["jti"], user=user)
 
     def fill_payload(
         self,
         user: User,
         expiration: Optional[datetime] = None,
         token_type: Optional[str] = None,
-    ) -> Tuple[Payload, Payload]:
+    ) -> tuple[Payload, Payload]:
         """Informations to store inside the JWT token,
         starting from the user obtained from the current service
 
         Claim attributes listed here:
         http://blog.apcelent.com/json-web-token-tutorial-example-python.html
 
         TTL is measured in seconds
@@ -592,19 +580,18 @@
     def is_coordinator(self, user: User) -> bool:
         """Check if current user has Coordinator role"""
         return self.verify_roles(user, [Role.COORDINATOR], warnings=False)
 
     def verify_roles(
         self,
         user: User,
-        roles: Optional[List[Union[str, Role]]],
+        roles: Optional[list[Union[str, Role]]],
         required_roles: str = ALL_ROLES,
         warnings: bool = True,
     ) -> bool:
-
         if not roles:
             return True
 
         current_roles = self.get_roles_from_user(user)
 
         if required_roles == ALL_ROLES:
             for role in roles:
@@ -633,22 +620,22 @@
             return False
 
         log.critical("Unknown role authorization requirement: {}", required_roles)
         return False
 
     @staticmethod
     def custom_user_properties_pre(
-        userdata: Dict[str, Any]
-    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        userdata: dict[str, Any]
+    ) -> tuple[dict[str, Any], dict[str, Any]]:
         try:
             userdata, extradata = mem.customizer.custom_user_properties_pre(userdata)
         except RestApiException:  # pragma: no cover
             raise
         except Exception as e:  # pragma: no cover
-            raise BadRequest(f"Unable to pre-customize user properties: {e}")
+            raise BadRequest(f"Unable to pre-customize user properties: {e}") from e
 
         if "email" in userdata:
             userdata["email"] = userdata["email"].lower()
 
         return userdata, extradata
 
     @staticmethod
@@ -658,24 +645,23 @@
         try:
             mem.customizer.custom_user_properties_post(
                 user, userdata, extra_userdata, db
             )
         except RestApiException:  # pragma: no cover
             raise
         except Exception as e:  # pragma: no cover
-            raise BadRequest(f"Unable to post-customize user properties: {e}")
+            raise BadRequest(f"Unable to post-customize user properties: {e}") from e
 
         return userdata
 
     # ###########################
     # # Login attempts handling #
     # ###########################
 
     def register_failed_login(self, username: str, user: Optional[User]) -> None:
-
         self.save_login(username, user, failed=True)
 
         if self.MAX_LOGIN_ATTEMPTS == 0:
             log.debug("Failed login are not considered in this configuration")
             return
 
         if self.count_failed_login(username) < self.MAX_LOGIN_ATTEMPTS:
@@ -708,87 +694,80 @@
                 user,
                 reversed(failed_logins),
                 self.FAILED_LOGINS_EXPIRATION.seconds,
                 url,
             )
 
     def count_failed_login(self, username: str) -> int:
-
         failed_logins = self.get_logins(username, only_unflushed=True)
         if not failed_logins:
             return 0
 
         last_failed = failed_logins[-1]
         exp = last_failed.date + self.FAILED_LOGINS_EXPIRATION
 
-        if get_now(exp.tzinfo) > exp:
+        if datetime.now(pytz.utc) > exp:
             self.flush_failed_logins(username)
             return 0
 
         return len(failed_logins)
 
     def get_totp_secret(self, user: User) -> str:
-
         if not user.mfa_hash:
             random_hash = pyotp.random_base32()
             user.mfa_hash = self.fernet.encrypt(random_hash.encode()).decode()
             self.save_user(user)
 
         try:
             return self.fernet.decrypt(user.mfa_hash.encode()).decode()
         # to test this exception change the fernet key used to encrypt mfa_hash
-        except InvalidFernetToken:
-            raise ServerError("Invalid server signature")
+        except InvalidFernetToken as e:  # pragma: no cover
+            raise ServerError("Invalid server signature") from e
 
     def verify_totp(self, user: User, totp_code: Optional[str]) -> bool:
-
         if totp_code is None:
             raise Unauthorized("Verification code is missing")
 
         # Used to mock tests
         if TESTING and totp_code == "111111":  # pragma: no cover
             return True
 
         secret = self.get_totp_secret(user)
         totp = pyotp.TOTP(secret)
         if not totp.verify(totp_code, valid_window=self.TOTP_VALIDITY_WINDOW):
-
             self.log_event(
                 Events.failed_login,
                 payload={"totp": totp_code},
                 user=user,
             )
 
             self.register_failed_login(user.email, user=user)
             raise Unauthorized("Verification code is not valid")
 
         return True
 
     def get_qrcode(self, user: User) -> str:
-
         secret = self.get_totp_secret(user)
         totp = pyotp.TOTP(secret)
 
         project_name = get_project_configuration("project.title", "No project name")
 
         otpauth_url = totp.provisioning_uri(project_name)
         qr_url = segno.make(otpauth_url)
         qr_stream = BytesIO()
         qr_url.save(qr_stream, kind="png", scale=5)
         return base64.b64encode(qr_stream.getvalue()).decode("utf-8")
 
     def verify_password_strength(
         self, pwd: str, old_pwd: Optional[str], email: str, name: str, surname: str
-    ) -> Tuple[bool, str]:
-
+    ) -> tuple[bool, str]:
         if old_pwd:
             if pwd == old_pwd:
                 return False, "The new password cannot match the previous password"
 
-            # in case old_pwd is a hash
             if self.verify_password(pwd, old_pwd):
                 return False, "The new password cannot match the previous password"
 
         if len(pwd) < self.MIN_PASSWORD_LENGTH:
             MIN = self.MIN_PASSWORD_LENGTH
             return False, f"Password is too short, use at least {MIN} characters"
 
@@ -823,15 +802,14 @@
     def change_password(
         self,
         user: User,
         password: str,
         new_password: Optional[str],
         password_confirm: Optional[str],
     ) -> bool:
-
         if new_password is None:
             raise BadRequest("Missing new password")
 
         if password_confirm is None:
             raise BadRequest("Missing password confirmation")
 
         if new_password != password_confirm:
@@ -860,48 +838,45 @@
             except Exception as e:  # pragma: no cover
                 log.critical("Failed to invalidate token {}", e)
 
         return True
 
     def check_password_validity(
         self, user: User, totp_authentication: bool
-    ) -> Dict[str, List[str]]:
-
+    ) -> dict[str, list[str]]:
         # ##################################################
         # Check if something is missing in the authentication and ask additional actions
         # raises exceptions in case of errors
 
-        message: Dict[str, List[str]] = {"actions": [], "errors": []}
+        message: dict[str, list[str]] = {"actions": [], "errors": []}
         last_pwd_change = user.last_password_change
         if last_pwd_change is None or last_pwd_change == 0:
             last_pwd_change = EPOCH
 
         if self.FORCE_FIRST_PASSWORD_CHANGE and last_pwd_change == EPOCH:
             message["actions"].append("FIRST LOGIN")
             message["errors"].append("Please change your temporary password")
             self.log_event(Events.password_expired, user=user)
 
             if totp_authentication:
-
                 message["qr_code"] = [self.get_qrcode(user)]
 
         elif self.MAX_PASSWORD_VALIDITY:
             valid_until = last_pwd_change + self.MAX_PASSWORD_VALIDITY
-            now = get_now(last_pwd_change.tzinfo)
+            now = datetime.now(pytz.utc)
             expired = last_pwd_change == EPOCH or valid_until < now
 
             if expired:
                 message["actions"].append("PASSWORD EXPIRED")
                 message["errors"].append("Your password is expired, please change it")
                 self.log_event(Events.password_expired, user=user)
 
         return message
 
     def verify_blocked_username(self, username: str) -> None:
-
         # We do not count failed logins
         if self.MAX_LOGIN_ATTEMPTS <= 0:
             return
 
         # We register failed logins but the user does not reached it yet
         if self.count_failed_login(username) < self.MAX_LOGIN_ATTEMPTS:
             return
@@ -918,83 +893,78 @@
         raise Forbidden(
             "Sorry, this account is temporarily blocked "
             "due to the number of failed login attempts."
         )
 
     @classmethod
     def verify_user_status(cls, user: User) -> None:
-
         if not user.is_active:
-
             cls.log_event(
                 Events.refused_login,
                 payload={"username": user.email, "motivation": "account not active"},
             )
 
             # Beware, frontend leverages on this exact message,
             # do not modified it without fix also on frontend side
             raise Forbidden("Sorry, this account is not active")
 
         now: Optional[datetime] = None
 
         if cls.DISABLE_UNUSED_CREDENTIALS_AFTER and user.last_login:
-
             if TESTING and user.email == cls.default_user:
                 log.info("Default user can't be blocked for inactivity during tests")
             else:
-                now = get_now(user.last_login.tzinfo)
+                now = datetime.now(pytz.utc)
                 if user.last_login + cls.DISABLE_UNUSED_CREDENTIALS_AFTER < now:
                     cls.log_event(
                         Events.refused_login,
                         payload={
                             "username": user.email,
                             "motivation": "account blocked due to inactivity",
                         },
                     )
                     raise Forbidden("Sorry, this account is blocked for inactivity")
 
         if user.expiration:
             # Reuse the now instance, if previously inizialized
             # tzinfo should be the same for both last_login and expiration fields
             if not now:
-                now = get_now(user.expiration.tzinfo)
+                now = datetime.now(pytz.utc)
 
             if user.expiration < now:
                 cls.log_event(
                     Events.refused_login,
                     payload={"username": user.email, "motivation": "account expired"},
                 )
                 raise Forbidden("Sorry, this account is expired")
 
     # Mostly copied in definition.py
     @classmethod
     def log_event(
         cls,
         event: Events,
         target: Optional[Any] = None,
-        payload: Optional[Dict[str, Any]] = None,
+        payload: Optional[dict[str, Any]] = None,
         user: Optional[Any] = None,
     ) -> None:
-
         try:
             url_path = request.path
         except RuntimeError:
             url_path = "-"
 
         save_event_log(
             event=event,
             payload=payload,
             user=user,
             target=target,
             ip=cls.get_remote_ip(),
             url=url_path,
         )
 
-    def init_auth_db(self, options: Dict[str, bool]) -> None:
-
+    def init_auth_db(self, options: dict[str, bool]) -> None:
         self.init_roles()
 
         default_group = self.init_groups(force=options.get("force_group", False))
 
         self.init_users(
             default_group, self.roles, force=options.get("force_user", False)
         )
@@ -1007,15 +977,14 @@
         num_of_unique_roles = len(list(set(role_names)))
         if num_of_roles != num_of_unique_roles:
             print_and_exit("Found duplicated role names: {}", str(sorted(role_names)))
 
         for role_name in self.roles:
             description = self.roles_data.get(role_name, ROLE_DISABLED)
             if r := current_roles.get(role_name):
-
                 if r.description == description:
                     log.info("Role {} already exists", role_name)
                 else:
                     log.info("Role {} already exists, updating description", role_name)
 
                     r.description = description
                     self.save_role(r)
@@ -1025,15 +994,14 @@
                 self.create_role(name=role_name, description=description)
 
         for r in current_roles:
             if r not in self.roles:
                 log.warning("Unknown role found: {}", r)
 
     def init_groups(self, force: bool) -> Group:
-
         create = False
         update = False
 
         default_group = self.get_group(name=DEFAULT_GROUP_NAME)
 
         # If there are no groups, let's create the default group
         if not self.get_groups():
@@ -1064,16 +1032,15 @@
         elif default_group:
             log.info("Default group already exists")
         else:
             log.info("Default group does not exist but other groups do")
 
         return default_group
 
-    def init_users(self, default_group: Group, roles: List[str], force: bool) -> User:
-
+    def init_users(self, default_group: Group, roles: list[str], force: bool) -> User:
         create = False
         update = False
 
         default_user = self.get_user(username=self.default_user)
 
         # If there are no users, let's create the default user
         if not self.get_users():
@@ -1086,26 +1053,25 @@
 
         if self.FORCE_FIRST_PASSWORD_CHANGE:
             last_password_change = None
         else:
             last_password_change = datetime.now(pytz.utc)
 
         if create:
-
             default_user = self.create_user(
                 {
                     "email": self.default_user,
                     "name": "Default",
                     "surname": "User",
                     "password": self.default_password,
                     "last_password_change": last_password_change,
                 },
                 roles=roles,
+                group=default_group,
             )
-            self.add_user_to_group(default_user, default_group)
             # This is required to execute the commit on sqlalchemy...
             self.save_user(default_user)
             log.info("Injected default user")
 
         elif update:
             # Added to make the life easier to mypy... but cannot be False
             if default_user:
@@ -1144,15 +1110,15 @@
         How to retrieve a single user from the current authentication db,
         based on the unique username or the user_id
         return None if no filter parameter is given
         """
         ...
 
     @abstractmethod
-    def get_users(self) -> List[User]:
+    def get_users(self) -> list[User]:
         """
         How to retrieve a list of all users from the current authentication db
         """
         ...
 
     @abstractmethod
     def save_user(self, user: User) -> bool:
@@ -1170,49 +1136,47 @@
     ) -> Optional[Group]:
         """
         How to retrieve a single group from the current authentication db
         """
         ...
 
     @abstractmethod
-    def get_groups(self) -> List[Group]:
+    def get_groups(self) -> list[Group]:
         """
         How to retrieve groups list from the current authentication db
         """
         ...
 
     @abstractmethod
     def get_user_group(self, user: User) -> Group:
         """
         How to retrieve the group that the user belongs to from the current auth db
         """
         ...
 
     @abstractmethod
-    def get_group_members(self, group: Group) -> List[User]:
+    def get_group_members(self, group: Group) -> list[User]:
         """
         How to retrieve group users list from the current authentication db
         """
         ...
 
     @abstractmethod
-    def save_group(self, group: Group) -> bool:
-        ...
+    def save_group(self, group: Group) -> bool: ...
 
     @abstractmethod
-    def delete_group(self, group: Group) -> bool:
-        ...
+    def delete_group(self, group: Group) -> bool: ...
 
     @abstractmethod
     def get_tokens(
         self,
         user: Optional[User] = None,
         token_jti: Optional[str] = None,
         get_all: bool = False,
-    ) -> List[Token]:
+    ) -> list[Token]:
         """
         Return the list of tokens
         """
         ...
 
     @abstractmethod
     def verify_token_validity(self, jti: str, user: User) -> bool:
@@ -1233,57 +1197,58 @@
         """
         With this method the specified token must be invalidated
         as expected after a user logout
         """
         ...
 
     @abstractmethod
-    def get_roles(self) -> List[RoleObj]:
+    def get_roles(self) -> list[RoleObj]:
         """
         How to retrieve all the roles
         """
         ...
 
     @abstractmethod
-    def get_roles_from_user(self, user: Optional[User]) -> List[str]:
+    def get_roles_from_user(self, user: Optional[User]) -> list[str]:
         """
         Retrieve roles from a user object from the current auth service
         """
         ...
 
     @abstractmethod
     def create_role(self, name: str, description: str) -> None:
         """
         A method to create a new role
         """
         ...
 
     @abstractmethod
-    def save_role(self, role: RoleObj) -> bool:
-        ...
+    def save_role(self, role: RoleObj) -> bool: ...
 
     # ################
     # # Create Users #
     # ################
     @abstractmethod
-    def create_user(self, userdata: Dict[str, Any], roles: List[str]) -> User:
+    def create_user(
+        self, userdata: dict[str, Any], roles: list[str], group: Group
+    ) -> User:
         """
         A method to create a new user
         """
         ...
 
     @abstractmethod
-    def link_roles(self, user: User, roles: List[str]) -> None:
+    def link_roles(self, user: User, roles: list[str]) -> None:
         """
         A method to assign roles to a user
         """
         ...
 
     @abstractmethod
-    def create_group(self, groupdata: Dict[str, Any]) -> Group:
+    def create_group(self, groupdata: dict[str, Any]) -> Group:
         """
         A method to create a new group
         """
         ...
 
     @abstractmethod
     def add_user_to_group(self, user: User, group: Group) -> None:
@@ -1298,82 +1263,82 @@
         Save login information
         """
         ...
 
     @abstractmethod
     def get_logins(
         self, username: Optional[str] = None, only_unflushed: bool = False
-    ) -> List[Login]:
+    ) -> list[Login]:
         """
         Save login information
         """
         ...
 
     @abstractmethod
     def flush_failed_logins(self, username: str) -> None:
         """
         Flush failed logins for the give username
         """
         ...
 
 
 class NoAuthentication(BaseAuthentication):  # pragma: no cover
-
     # Also used by POST user
-    def create_user(self, userdata: Dict[str, Any], roles: List[str]) -> User:
+    def create_user(
+        self, userdata: dict[str, Any], roles: list[str], group: Group
+    ) -> User:
         raise NotImplementedError("Create User not implemented with No Authentication")
 
-    def link_roles(self, user: User, roles: List[str]) -> None:
+    def link_roles(self, user: User, roles: list[str]) -> None:
         return None
 
-    def create_group(self, groupdata: Dict[str, Any]) -> Group:
+    def create_group(self, groupdata: dict[str, Any]) -> Group:
         raise NotImplementedError("Create Group not implemented with No Authentication")
 
     def add_user_to_group(self, user: User, group: Group) -> None:
         return None
 
     def get_user(
         self, username: Optional[str] = None, user_id: Optional[str] = None
     ) -> Optional[User]:
-
         return None
 
-    def get_users(self) -> List[User]:
+    def get_users(self) -> list[User]:
         return []
 
     def save_user(self, user: User) -> bool:
         return False
 
     def delete_user(self, user: User) -> bool:
         return False
 
     def get_group(
         self, group_id: Optional[str] = None, name: Optional[str] = None
     ) -> Optional[Group]:
         return None
 
-    def get_groups(self) -> List[Group]:
+    def get_groups(self) -> list[Group]:
         return []
 
     def get_user_group(self, user: User) -> Group:
         raise NotImplementedError("Get Group not implemented with No Authentication")
 
-    def get_group_members(self, group: Group) -> List[User]:
+    def get_group_members(self, group: Group) -> list[User]:
         return []
 
     def save_group(self, group: Group) -> bool:
         return False
 
     def delete_group(self, group: Group) -> bool:
         return False
 
-    def get_roles(self) -> List[RoleObj]:
+    def get_roles(self) -> list[RoleObj]:
         return []
 
-    def get_roles_from_user(self, user: Optional[User]) -> List[str]:
+    def get_roles_from_user(self, user: Optional[User]) -> list[str]:
         return []
 
     def create_role(self, name: str, description: str) -> None:
         return None
 
     def save_role(self, role: RoleObj) -> bool:
         return False
@@ -1387,24 +1352,23 @@
         return False
 
     def get_tokens(
         self,
         user: Optional[User] = None,
         token_jti: Optional[str] = None,
         get_all: bool = False,
-    ) -> List[Token]:
-
+    ) -> list[Token]:
         return []
 
     def invalidate_token(self, token: str) -> bool:
         return False
 
     def save_login(self, username: str, user: Optional[User], failed: bool) -> None:
         return None
 
     def get_logins(
         self, username: Optional[str] = None, only_unflushed: bool = False
-    ) -> List[Login]:
+    ) -> list[Login]:
         raise NotImplementedError("Get Login not implemented with No Authentication")
 
     def flush_failed_logins(self, username: str) -> None:
         return None
```

### Comparing `rapydo_http-2.4/restapi/services/cache.py` & `rapydo_http-3.0/restapi/services/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 from restapi.exceptions import ServiceUnavailable
 from restapi.utilities.globals import mem
 
 
 class Cache:
     @staticmethod
     def get_instance(app: Flask) -> FlaskCache:
-
         if not Connector.check_availability("redis"):
             raise ServiceUnavailable("Can't enable the cache without Redis")
 
         # This check prevents KeyError raised during tests
         # Exactly as reported here:
         # https://github.com/sh4nks/flask-caching/issues/191
         if not hasattr(mem, "cache"):
-
             redis = Env.load_variables_group(prefix="redis")
             mem.cache = FlaskCache(
                 config={
                     "CACHE_TYPE": "RedisCache",
                     "CACHE_REDIS_HOST": redis.get("host"),
                     "CACHE_REDIS_PORT": redis.get("port"),
                     "CACHE_REDIS_PASSWORD": redis.get("password"),
```

### Comparing `rapydo_http-2.4/restapi/services/download.py` & `rapydo_http-3.0/restapi/services/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Download data from APIs
 """
+
+from collections.abc import Iterator
 from mimetypes import MimeTypes
 from pathlib import Path
-from typing import Iterator, Optional
+from typing import Optional
 
 from flask import Response, send_from_directory, stream_with_context
 from werkzeug.utils import secure_filename
 
 from restapi.config import DATA_PATH
 from restapi.exceptions import NotFound
 from restapi.services.uploader import Uploader
@@ -29,15 +31,14 @@
     # It is also good for media files by sending Range header
     @staticmethod
     def send_file_content(
         filename: str,
         subfolder: Path,
         mime: Optional[str] = None,
     ) -> Response:
-
         Uploader.validate_upload_folder(subfolder)
 
         filename = secure_filename(filename)
         filepath = subfolder.joinpath(filename)
         if not filepath.is_file():
             raise NotFound("The requested file does not exist")
 
@@ -65,15 +66,14 @@
     @staticmethod
     def send_file_streamed(
         filename: str,
         subfolder: Path,
         mime: Optional[str] = None,
         out_filename: Optional[str] = None,
     ) -> Response:
-
         Uploader.validate_upload_folder(subfolder)
 
         filename = secure_filename(filename)
         filepath = subfolder.joinpath(filename)
 
         if not filepath.is_file():
             raise NotFound("The requested file does not exist")
@@ -88,9 +88,9 @@
             mimetype=mime,
         )
 
         if not out_filename:
             out_filename = filepath.name
 
         response.headers["Content-Disposition"] = f"attachment; filename={out_filename}"
-        response.headers["Content-Length"] = filepath.stat().st_size
+        response.headers["Content-Length"] = str(filepath.stat().st_size)
         return response
```

### Comparing `rapydo_http-2.4/restapi/services/uploader.py` & `rapydo_http-3.0/restapi/services/uploader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple
+from typing import Optional
 
 from flask import request
 from plumbum.cmd import file
 from werkzeug.http import parse_content_range_header
 from werkzeug.utils import secure_filename
 
 from restapi.config import DATA_PATH, get_backend_url
@@ -12,30 +12,28 @@
 from restapi.utilities.logs import log
 
 # Equivalent to -r--r-----
 DEFAULT_PERMISSIONS = 0o440
 
 
 class Uploader:
+    allowed_exts: list[str] = []
 
-    allowed_exts: List[str] = []
-
-    def set_allowed_exts(self, exts: List[str]) -> None:
+    def set_allowed_exts(self, exts: list[str]) -> None:
         self.allowed_exts = exts
 
     def allowed_file(self, filename: str) -> bool:
         if not self.allowed_exts:
             return True
         return (
             "." in filename and filename.rsplit(".", 1)[1].lower() in self.allowed_exts
         )
 
     @staticmethod
     def validate_upload_folder(path: Path) -> None:
-
         if "\x00" in str(path):
             raise BadRequest("Invalid null byte in subfolder parameter")
 
         if path != path.resolve():
             log.error("Invalid path: path is relative or contains double-dots")
             raise Forbidden("Invalid file path")
 
@@ -44,30 +42,29 @@
                 "Invalid root path: {} is expected to be a child of {}",
                 path,
                 DATA_PATH,
             )
             raise Forbidden("Invalid file path")
 
     @staticmethod
-    def get_file_metadata(abs_file: Path) -> Dict[str, str]:
+    def get_file_metadata(abs_file: Path) -> dict[str, str]:
         try:
             # Check the type
             # Example of output:
             # text/plain; charset=us-ascii
             out = file["-ib", str(abs_file)]().split(";")
             return {"type": out[0].strip(), "charset": out[1].split("=")[1].strip()}
         except Exception:
             log.warning("Unknown type for '{}'", abs_file)
             return {}
 
     # this method is used by mistral
     def upload(self, subfolder: Path, force: bool = False) -> Response:
-
         if "file" not in request.files:
-            raise BadRequest("No files specified")
+            raise BadRequest("No files specified")  # pragma: no cover
 
         myfile = request.files["file"]
 
         if not myfile.filename:  # pragma: no cover
             raise BadRequest("Invalid filename")
 
         if not self.allowed_file(myfile.filename):
@@ -92,15 +89,17 @@
 
         # Save the file
         try:
             myfile.save(abs_file)
             log.debug("Absolute file path should be '{}'", abs_file)
         except Exception as e:  # pragma: no cover
             log.error(e)
-            raise ServiceUnavailable("Permission denied: failed to write the file")
+            raise ServiceUnavailable(
+                "Permission denied: failed to write the file"
+            ) from e
 
         # Check exists - but it is basicaly a test that cannot fail...
         # The has just been uploaded!
         if not abs_file.exists():  # pragma: no cover
             raise ServiceUnavailable("Unable to retrieve the uploaded file")
 
         ########################
@@ -119,15 +118,14 @@
 
     # Compatible with
     # https://developers.google.com/drive/api/v3/manage-uploads#resumable
     # and with https://www.npmjs.com/package/ngx-uploadx and with
     def init_chunk_upload(
         self, upload_dir: Path, filename: str, force: bool = True
     ) -> Response:
-
         if not self.allowed_file(filename):
             raise BadRequest("File extension not allowed")
 
         Uploader.validate_upload_folder(upload_dir)
 
         if not upload_dir.exists():
             upload_dir.mkdir(parents=True, exist_ok=True)
@@ -156,16 +154,15 @@
             headers={"Access-Control-Expose-Headers": "Location", "Location": url},
             code=201,
         )
 
     @staticmethod
     def parse_content_range(
         range_header: Optional[str],
-    ) -> Tuple[Optional[int], Optional[int], Optional[int]]:
-
+    ) -> tuple[Optional[int], Optional[int], Optional[int]]:
         if range_header is None:
             return None, None, None
 
         content_range = parse_content_range_header(range_header)
 
         if content_range is None:
             log.error("Unable to parse Content-Range: {}", range_header)
@@ -202,16 +199,15 @@
     # PUT request is way different compared to POST request. With PUT request
     # the file contents can be accessed using either request.data or request.stream.
     # The first one stores incoming data as string, while request.stream acts
     # more like a file object, making it more suitable for binary data
     # Ref. http://stackoverflow.com/a/9533843/2114395
     def chunk_upload(
         self, upload_dir: Path, filename: str, chunk_size: Optional[int] = None
-    ) -> Tuple[bool, Response]:
-
+    ) -> tuple[bool, Response]:
         Uploader.validate_upload_folder(upload_dir)
 
         filename = secure_filename(filename)
 
         range_header = request.headers.get("Content-Range", "")
         total_length, start, stop = self.parse_content_range(range_header)
 
@@ -236,16 +232,18 @@
             with open(file_path, "ab") as f:
                 while True:
                     chunk = request.stream.read(chunk_size)
                     if not chunk:
                         break
                     f.seek(start)
                     f.write(chunk)
-        except PermissionError:
-            raise ServiceUnavailable("Permission denied: failed to write the file")
+        except PermissionError as e:
+            raise ServiceUnavailable(
+                "Permission denied: failed to write the file"
+            ) from e
 
         if completed:
             file_path.chmod(DEFAULT_PERMISSIONS)
             return (
                 completed,
                 EndpointResource.response(
                     {"filename": filename, "meta": self.get_file_metadata(file_path)},
```

### Comparing `rapydo_http-2.4/restapi/templates/index.html` & `rapydo_http-3.0/restapi/templates/index.html`

 * *Files identical despite different names*

### Comparing `rapydo_http-2.4/restapi/tests.py` & `rapydo_http-3.0/restapi/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Base class for unit tests
 """
+
 import base64
 import os
 import re
 import urllib.parse
 import uuid
 from collections import namedtuple
+from collections.abc import Generator
 from contextlib import contextmanager
 from datetime import datetime, timedelta
 from pathlib import Path
-from typing import Any, Dict, Generator, List, Optional, Tuple, TypedDict, Union, cast
+from typing import Any, Optional, TypedDict, Union, cast
 
 import jwt
 import orjson
 import pyotp
 import pytest
 import pytz
 from faker import Faker
@@ -36,15 +38,15 @@
 from restapi.services.authentication import BaseAuthentication, Role
 from restapi.utilities.faker import get_faker
 from restapi.utilities.logs import LOGS_FOLDER, Events, log
 
 
 class MockedEmail(TypedDict):
     # from: str
-    cc: List[str]
+    cc: list[str]
     msg: str
     # body and headers are added by read_mock_email function
     body: str
     headers: str
 
 
 SERVER_URI = f"http://{DEFAULT_HOST}:{DEFAULT_PORT}"
@@ -66,19 +68,18 @@
         os.chdir(CODE_DIR)
         yield
     finally:
         os.chdir(origin)
 
 
 class BaseTests:
-
     faker: Faker = get_faker()
     # This will store credentials to be used to test unused credentials ban
     # Tuple = (email, password, uuid)
-    unused_credentials: Optional[Tuple[str, str, str]] = None
+    unused_credentials: Optional[tuple[str, str, str]] = None
 
     @classmethod
     def save(cls, variable: str, value: Any) -> None:
         """
         Save a variable in the class, to be re-used in further tests
         """
 
@@ -94,17 +95,17 @@
 
         raise AttributeError(f"Class variable {variable} not found")  # pragma: no cover
 
     @staticmethod
     def get_dynamic_input_schema(
         client: FlaskClient,
         endpoint: str,
-        headers: Optional[Dict[str, str]],
+        headers: Optional[dict[str, str]],
         method: str = "post",
-    ) -> List[Dict[str, Any]]:
+    ) -> list[dict[str, Any]]:
         """
         Retrieve a dynamic data schema associated with a endpoint
         """
 
         method = method.lower()
 
         if method == "post":
@@ -123,16 +124,15 @@
         for f in schema:
             assert isinstance(f, dict)
         return schema
 
     @staticmethod
     def get_content(
         http_out: Response,
-    ) -> Union[str, float, int, bool, List[Any], Dict[str, Any]]:
-
+    ) -> Union[str, float, int, bool, list[Any], dict[str, Any]]:
         try:
             response = orjson.loads(http_out.get_data().decode())
             if isinstance(
                 response,
                 (
                     str,
                     bool,
@@ -145,15 +145,15 @@
                 return response
 
             raise ValueError(  # pragma: no cover
                 f"Unknown response type: {type(response)}"
             )
         except Exception as e:  # pragma: no cover
             log.error("Failed to load response:\n{}", e)
-            raise ValueError(f"Malformed response: {http_out}")
+            raise ValueError(f"Malformed response: {http_out}") from e
 
     @staticmethod
     def generate_totp(email: Optional[str]) -> str:
         assert email is not None
         auth = Connector.get_authentication_instance()
 
         user = auth.get_user(username=email.lower())
@@ -165,17 +165,17 @@
     @classmethod
     def do_login(
         cls,
         client: FlaskClient,
         USER: Optional[str],
         PWD: Optional[str],
         status_code: int = 200,
-        data: Optional[Dict[str, Any]] = None,
+        data: Optional[dict[str, Any]] = None,
         test_failures: bool = False,
-    ) -> Tuple[Optional[Dict[str, str]], str]:
+    ) -> tuple[Optional[dict[str, str]], str]:
         """
         Make login and return both token and authorization header
         """
 
         if not Connector.check_availability("authentication"):  # pragma: no cover
             pytest.fail("Authentication is not enabled")
 
@@ -196,15 +196,14 @@
         data["username"] = USER
         data["password"] = PWD
 
         r = client.post(f"{AUTH_URI}/login", json=data)
         content = orjson.loads(r.data.decode("utf-8"))
 
         if r.status_code == 403:
-
             # This 403 is expected, return an invalid value or you can enter a loop!
             if status_code == 403:
                 return None, content
 
             if isinstance(content, dict) and content.get("actions"):
                 actions = content.get("actions", [])
 
@@ -215,15 +214,14 @@
                         continue
                     if action == "PASSWORD EXPIRED":
                         continue
 
                 data = {}
 
                 if "FIRST LOGIN" in actions or "PASSWORD EXPIRED" in actions:
-
                     events = cls.get_last_events(1)
                     assert events[0].event == Events.password_expired.value
                     # assert events[0].user == USER
 
                     newpwd = cls.faker.password(strong=True)
                     if test_failures:
                         data["new_password"] = newpwd
@@ -328,31 +326,33 @@
 
         return {"Authorization": f"Bearer {content}"}, content
 
     @classmethod
     def create_user(
         cls,
         client: FlaskClient,
-        data: Optional[Dict[str, Any]] = None,
-        roles: Optional[List[Union[str, Role]]] = None,
-    ) -> Tuple[str, Dict[str, Any]]:
-
+        data: Optional[dict[str, Any]] = None,
+        roles: Optional[list[Union[str, Role]]] = None,
+        group: Optional[str] = None,
+    ) -> tuple[str, dict[str, Any]]:
         assert Env.get_bool("MAIN_LOGIN_ENABLE")
 
         admin_headers, _ = cls.do_login(client, None, None)
         assert admin_headers is not None
         schema = cls.get_dynamic_input_schema(client, "admin/users", admin_headers)
         user_data = cls.buildData(schema)
         if Connector.check_availability("smtp"):
             user_data["email_notification"] = False
         user_data["is_active"] = True
         user_data["expiration"] = None
 
-        if roles:
+        if group:
+            user_data["group"] = group
 
+        if roles:
             for idx, role in enumerate(roles):
                 if isinstance(role, Role):
                     roles[idx] = role.value
 
             user_data["roles"] = orjson.dumps(roles).decode("UTF8")
 
         if data:
@@ -363,27 +363,25 @@
         uuid = cls.get_content(r)
         assert isinstance(uuid, str)
 
         return uuid, user_data
 
     @classmethod
     def delete_user(cls, client: FlaskClient, uuid: str) -> None:
-
         assert Env.get_bool("MAIN_LOGIN_ENABLE")
 
         admin_headers, _ = cls.do_login(client, None, None)
         assert admin_headers is not None
         r = client.delete(f"{API_URI}/admin/users/{uuid}", headers=admin_headers)
         assert r.status_code == 204
 
     @classmethod
     def create_group(
-        cls, client: FlaskClient, data: Optional[Dict[str, Any]] = None
-    ) -> Tuple[str, Dict[str, Any]]:
-
+        cls, client: FlaskClient, data: Optional[dict[str, Any]] = None
+    ) -> tuple[str, dict[str, Any]]:
         assert Env.get_bool("MAIN_LOGIN_ENABLE")
 
         admin_headers, _ = cls.do_login(client, None, None)
         assert admin_headers is not None
         schema = cls.get_dynamic_input_schema(client, "admin/groups", admin_headers)
         group_data = cls.buildData(schema)
         if data:
@@ -455,22 +453,21 @@
             return f"{email_username * 4}@{email_tokens[1]}"
 
         return cls.get_random_email(  # pragma: no cover
             faker, surname, surname, recursion=recursion + 1
         )
 
     @classmethod
-    def buildData(cls, schema: List[Dict[str, Any]]) -> Dict[str, Any]:
+    def buildData(cls, schema: list[dict[str, Any]]) -> dict[str, Any]:
         """
         Input: a Marshmallow schema
         Output: a dictionary of random data
         """
-        data: Dict[str, Any] = {}
+        data: dict[str, Any] = {}
         for d in schema:
-
             assert "key" in d
             assert "type" in d
 
             key = d.get("key")
             field_type = d.get("type")
 
             assert key is not None
@@ -492,43 +489,41 @@
                 # else:  # pragma: no cover
                 #     pytest.fail(f"BuildData for {key}: invalid options (empty?)")
             elif field_type == "number" or field_type == "int":
                 min_value = d.get("min", 0)
                 max_value = d.get("max", 9999)
                 data[key] = cls.faker.pyint(min_value=min_value, max_value=max_value)
             elif field_type == "date":
-
                 min_date = None
                 max_date = None
 
-                if min_value := d.get("min"):
+                if min_value := d.get("min"):  # pragma: no cover
                     min_date = datetime.fromisoformat(min_value)
 
-                if max_value := d.get("max"):
+                if max_value := d.get("max"):  # pragma: no cover
                     max_date = datetime.fromisoformat(max_value)
 
                 random_date = cls.faker.date_time_between_dates(
                     datetime_start=min_date, datetime_end=max_date
                 )
                 data[key] = random_date.date()
             elif field_type == "datetime":
-
                 min_date = None
                 max_date = None
 
                 if min_value := d.get("min"):
                     min_date = datetime.fromisoformat(min_value)
 
                 if max_value := d.get("max"):
                     max_date = datetime.fromisoformat(max_value)
 
                 random_date = cls.faker.date_time_between_dates(
                     datetime_start=min_date, datetime_end=max_date
                 )
-                data[key] = f"{random_date.isoformat()}.000Z"
+                data[key] = f"{random_date.isoformat(timespec='seconds')}.000Z"
             elif field_type == "email":
                 data[key] = cls.faker.ascii_email()
             elif field_type == "boolean":
                 data[key] = cls.faker.pybool()
             elif field_type == "password":
                 data[key] = cls.faker.password(strong=True)
             elif field_type == "string":
@@ -642,30 +637,29 @@
         token_type: str,
         user_id: Optional[str] = None,
         expired: bool = False,
         immature: bool = False,
         wrong_secret: bool = False,
         wrong_algorithm: bool = False,
     ) -> str:
-
         if wrong_secret:
             secret = cls.faker.password()
         else:
             with open(JWT_SECRET_FILE, "rb") as f:
                 secret = f.read()
 
         if wrong_algorithm:
             algorithm = "HS256"
         else:
             algorithm = BaseAuthentication.JWT_ALGO
 
         if user_id is None:
             user_id = str(uuid.uuid4())
 
-        payload: Dict[str, Any] = {"user_id": user_id, "jti": str(uuid.uuid4())}
+        payload: dict[str, Any] = {"user_id": user_id, "jti": str(uuid.uuid4())}
         payload["t"] = token_type
         now = datetime.now(pytz.utc)
         payload["iat"] = now
         if immature:
             payload["nbf"] = now + timedelta(seconds=999)
         else:
             payload["nbf"] = now - timedelta(seconds=999)
@@ -673,16 +667,15 @@
             payload["exp"] = now - timedelta(seconds=999)
         else:
             payload["exp"] = now + timedelta(seconds=999)
 
         return jwt.encode(payload, secret, algorithm=algorithm)
 
     @staticmethod
-    def event_matches_filters(event: Event, filters: Dict[str, str]) -> bool:
-
+    def event_matches_filters(event: Event, filters: dict[str, str]) -> bool:
         for filt, value in filters.items():  # pragma: no cover
             if filt == "date" and event.date != value:
                 return False
             if filt == "ip" and event.ip != value:
                 return False
             if filt == "user" and event.user != value:
                 return False
@@ -693,30 +686,28 @@
             if filt == "target_id" and event.target_id != value:
                 return False
             # filter by payload ... ?
         return True
 
     @classmethod
     def get_last_events(
-        cls, num: int = 1, filters: Optional[Dict[str, str]] = None
-    ) -> List[Event]:
-
+        cls, num: int = 1, filters: Optional[dict[str, str]] = None
+    ) -> list[Event]:
         fpath = LOGS_FOLDER.joinpath("security-events.log")
         if not fpath.exists():  # pragma: no cover
             return []
 
         with open(fpath) as file:
             # Not efficient read the whole file to get the last lines, to be improved!
             lines = file.readlines()
             lines.reverse()
 
-            events: List[Event] = []
+            events: list[Event] = []
             # read last num lines
             for line in lines:
-
                 # Found enough events, let's stop
                 if len(events) == num:
                     break
 
                 tokens = line.strip().split(" ")
 
                 payload = orjson.loads(" ".join(tokens[8:])) if len(tokens) >= 9 else {}
@@ -736,25 +727,26 @@
                     tokens[6] if len(tokens) >= 7 else "",
                     # Target ID or empty
                     tokens[7] if len(tokens) >= 8 else "",
                     # Payload dictionary
                     payload,
                 )
 
-                if filters and not cls.event_matches_filters(event, filters):
+                if filters and not cls.event_matches_filters(
+                    event, filters
+                ):  # pragma: no cover
                     continue
 
                 events.append(event)
 
         events.reverse()
         return events
 
     @staticmethod
     def send_task(app: Flask, task_name: str, *args: Any, **kwargs: Any) -> Any:
-
         c = celery.get_instance()
         c.app = app
 
         # Celery type hints are wrong!?
         # Mypy complains about: error: "Callable[[], Any]" has no attribute "get"
         # But .tasks is a TaskRegistry and it is child of dict...
         # so that .get is totally legit!
```

### Comparing `rapydo_http-2.4/restapi/tests_initialization.py` & `rapydo_http-3.0/restapi/tests_initialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Initialization script for unit tests
 """
+
 from datetime import datetime
 
 import pytz
 
 from restapi.config import TESTING
 from restapi.services.authentication import DEFAULT_GROUP_NAME, BaseAuthentication
 from restapi.utilities.faker import get_faker
 
 
 def initialize_testing_environment(auth: BaseAuthentication) -> None:
-
     assert TESTING
 
     faker = get_faker()
     email = faker.ascii_email()
     password = faker.password(strong=True)
     default_group = auth.get_group(name=DEFAULT_GROUP_NAME)
     user = auth.create_user(
@@ -24,16 +24,16 @@
             "name": "Default",
             "surname": "User",
             "password": password,
             "last_password_change": datetime.now(pytz.utc),
         },
         # It will be expanded with the default role
         roles=[],
+        group=default_group,
     )
-    auth.add_user_to_group(user, default_group)
     # This is required to execute the commit on sqlalchemy...
     auth.save_user(user)
 
     for _ in range(0, 20):
         payload, full_payload = auth.fill_payload(user)
         token = auth.create_token(payload)
         auth.save_token(user, token, full_payload)
```

### Comparing `rapydo_http-2.4/restapi/types.py` & `rapydo_http-3.0/restapi/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Python hints definitions
 """
 
-from typing import Any, Callable, Dict, Optional, Tuple, TypeVar, Union
+from typing import Any, Callable, Optional, TypeVar, Union
 
 from flask import Response as FlaskResponse
 from werkzeug.wrappers import Response as WerkzeugResponse
 
-Response = Union[FlaskResponse, WerkzeugResponse, Tuple[Any, int, Dict[str, str]]]
+Response = Union[FlaskResponse, WerkzeugResponse, tuple[Any, int, dict[str, str]]]
 ResponseContent = Optional[Any]
-Props = Dict[str, Any]
+Props = dict[str, Any]
 FlaskRequest = Any
 # instead of ... should be [EndpointResource, anything else]
 # but mypy only allows to specify all or none input parameters
 EndpointFunction = TypeVar("EndpointFunction", bound=Callable[..., Response])
```

### Comparing `rapydo_http-2.4/restapi/utilities/configuration.py` & `rapydo_http-3.0/restapi/utilities/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from pathlib import Path
-from typing import Any, Dict, Optional, Tuple, cast
+from typing import Any, Optional, cast
 
 import yaml
 
 from restapi.utilities import print_and_exit
 from restapi.utilities.logs import log
 
 PROJECTS_DEFAULTS_FILE = Path("projects_defaults.yaml")
 PROJECT_CONF_FILENAME = Path("project_configuration.yaml")
 
 
-ConfigurationType = Dict[str, Any]
+ConfigurationType = dict[str, Any]
 
 
 def read_configuration(
     default_file_path: Path,
     base_project_path: Path,
     projects_path: Path,
     submodules_path: Path,
-) -> Tuple[ConfigurationType, Optional[str], Optional[Path]]:
+) -> tuple[ConfigurationType, Optional[str], Optional[Path]]:
     """
     Read default configuration
     """
 
     custom_configuration = load_yaml_file(
         base_project_path.joinpath(PROJECT_CONF_FILENAME)
     )
@@ -63,17 +63,15 @@
     extend_file = Path(f"extended_{PROJECT_CONF_FILENAME}")
     extended_configuration = load_yaml_file(extend_path.joinpath(extend_file))
     m1 = mix(base_configuration, extended_configuration)
     return mix(m1, custom_configuration), extended_project, extend_path
 
 
 def mix(base: ConfigurationType, custom: ConfigurationType) -> ConfigurationType:
-
     for key, elements in custom.items():
-
         if key not in base:
             base[key] = custom[key]
             continue
 
         if elements is None:
             if isinstance(base[key], dict):
                 log.warning("Cannot replace {} with empty list", key)
@@ -88,15 +86,14 @@
         else:
             base[key] = elements
 
     return base
 
 
 def load_yaml_file(filepath: Path) -> ConfigurationType:
-
     if not filepath.exists():
         raise AttributeError(f"YAML file does not exist: {filepath}")
 
     with open(filepath) as fh:
         try:
             docs = list(yaml.safe_load_all(fh))
 
@@ -106,8 +103,8 @@
             return cast(ConfigurationType, docs[0])
 
         except Exception as e:
             # # IF dealing with a strange exception string (escaped)
             # import codecs
             # error, _ = codecs.getdecoder("unicode_escape")(str(error))
 
-            raise AttributeError(f"Failed to read file {filepath}: {e}")
+            raise AttributeError(f"Failed to read file {filepath}: {e}") from e
```

### Comparing `rapydo_http-2.4/restapi/utilities/faker.py` & `rapydo_http-3.0/restapi/utilities/faker.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         length: int = 8,
         strong: bool = False,  # this enables all low, up, digits and symbols
         low: bool = True,
         up: bool = False,
         digits: bool = False,
         symbols: bool = False,
     ) -> str:
-
         if strong:
             if length < 16:
                 length = 16
             low = True
             up = True
             digits = True
             symbols = True
@@ -119,15 +118,14 @@
                 length, strong=strong, low=low, up=up, digits=digits, symbols=symbols
             )
 
         return randstr
 
 
 def get_faker() -> Faker:
-
     loc = secrets.choice(list(FAKER_LOCALES.keys()))
     log.warning(f"Today I'm {FAKER_LOCALES.get(loc)}")
     faker = Faker(loc)
 
     faker.add_provider(PasswordProvider)
 
     return faker
```

### Comparing `rapydo_http-2.4/restapi/utilities/logs.py` & `rapydo_http-3.0/restapi/utilities/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 import sys
 import urllib.parse
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Optional
 
 import orjson
 from loguru import logger as log
 
 from restapi.config import HOST_TYPE, PRODUCTION
 from restapi.env import Env
 
@@ -122,17 +122,16 @@
 fmt += "<fg #666>{name}:{line}</fg #666>] "
 fmt += "<fg #FFF>{message}</fg #FFF>"
 
 
 # Set the default logger with the given log level and save the log_id as static variable
 # Further call to this function will remove the previous logger (based on saved log_id)
 def set_logger(level: str) -> None:
-
-    if hasattr(set_logger, "log_id"):
-        log_id = getattr(set_logger, "log_id")
+    if hasattr(set_logger, "log_id"):  # pragma: no cover
+        log_id = set_logger.log_id
         log.remove(log_id)
 
     log_id = log.add(
         sys.stderr,
         level=level,
         colorize=True,
         format=fmt,
@@ -142,15 +141,15 @@
         # Display variables values in exception trace to eases the debugging.
         # Disabled in production to avoid leaking sensitive data.
         # Note: enabled in development mode on the File Logger
         diagnose=False,
         filter=print_message_on_stderr,
     )
 
-    setattr(set_logger, "log_id", log_id)
+    set_logger.log_id = log_id
 
 
 set_logger(log_level)
 
 # Logs utilities
 
 # Can't understand why mypy is unable to understand Env.get_int, since it is annotated
@@ -169,15 +168,15 @@
     "new_password",
     "password_confirm",
     "totp",
     "totp_code",
 ]
 
 
-def handle_log_output(original_parameters_string: Optional[Any]) -> Dict[str, Any]:
+def handle_log_output(original_parameters_string: Optional[Any]) -> dict[str, Any]:
     """Print a log line by preventing the exposure of sensitive information"""
     if original_parameters_string is None:
         return {}
 
     if isinstance(original_parameters_string, bytes):
         mystr = original_parameters_string.decode("utf-8")
     elif isinstance(original_parameters_string, str):
@@ -192,36 +191,34 @@
     try:
         parameters = orjson.loads(mystr)
     except orjson.JSONDecodeError:
         try:
             parameters = urllib.parse.parse_qs(mystr)
             urlencoded = True
         except Exception:  # pragma: no cover
-
             return original_parameters_string
 
     return obfuscate_dict(parameters, urlencoded=urlencoded)
 
 
 def obfuscate_url(url: str) -> str:
     """Obfuscate a sensitive information with a placeholder"""
     return re.sub(r"\/\/.*:.*@", "//***:***@", url)
 
 
 def obfuscate_dict(
-    parameters: Dict[str, Any], urlencoded: bool = False, max_len: int = MAX_CHAR_LEN
-) -> Dict[str, Any]:
+    parameters: dict[str, Any], urlencoded: bool = False, max_len: int = MAX_CHAR_LEN
+) -> dict[str, Any]:
     """Obfuscate sensitive information in a dictionary by looking at sensitive keys"""
 
     if not isinstance(parameters, dict):
         return parameters
 
     output = {}
     for key, value in parameters.items():
-
         if key in OBSCURED_FIELDS:
             value = OBSCURE_VALUE
         elif urlencoded and isinstance(value, list):
             # urllib.parse.parse_qs converts all elements in single-elements lists...
             # converting back to the original element
             if len(value) == 1:
                 value = value[0]
@@ -234,34 +231,34 @@
                 pass
 
         output[key] = value
 
     return output
 
 
-def parse_event_target(target: Any) -> Tuple[str, str]:
+def parse_event_target(target: Any) -> tuple[str, str]:
     """Extract from an object an ID to be stored in logs"""
     if not target:
         return "", ""
 
     target_type = type(target).__name__
 
     if hasattr(target, "uuid"):
-        return target_type, getattr(target, "uuid")
+        return target_type, target.uuid
 
     if hasattr(target, "id"):
-        return target_type, getattr(target, "id")
+        return target_type, target.id
 
     return target_type, ""
 
 
 def save_event_log(
     event: Events,
     target: Optional[Any] = None,
-    payload: Optional[Dict[str, Any]] = None,
+    payload: Optional[dict[str, Any]] = None,
     user: Optional[Any] = None,
     ip: str = "-",
     url: str = "",
 ) -> None:
     """Save a log entry in security-events.log"""
 
     target_type, target_id = parse_event_target(target)
@@ -270,15 +267,15 @@
         p = orjson.dumps(obfuscate_dict(payload, max_len=999)).decode("UTF8")
     else:
         p = ""
 
     log.log(
         "EVENT",
         "",
-        event=event,
+        event=event.value,
         ip=ip,
         user=user.email if user else "-",
         target_id=target_id,
         target_type=target_type,
         payload=p,
         url=url,
     )
```

### Comparing `rapydo_http-2.4/restapi/utilities/meta.py` & `rapydo_http-3.0/restapi/utilities/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 http://python-3-patterns-idioms-test.readthedocs.org/en/latest/Metaprogramming.html
 """
 
 import inspect
 import pkgutil
 from importlib import import_module
 from types import ModuleType
-from typing import Any, Callable, Dict, List, Optional, Type
+from typing import Any, Callable, Optional
 
 from restapi.config import BACKEND_PACKAGE, CUSTOM_PACKAGE
 from restapi.utilities import print_and_exit
 from restapi.utilities.logs import log
 
 
 class Meta:
     """Utilities with meta in mind"""
 
     @staticmethod
-    def get_classes_from_module(module: ModuleType) -> Dict[str, Type[Any]]:
+    def get_classes_from_module(module: ModuleType) -> dict[str, type[Any]]:
         """
         Find classes inside a python module file.
         """
 
         try:
             return {
                 name: cls
@@ -33,15 +33,15 @@
             }
         except AttributeError:
             log.warning("Could not find any class in module {}", module)
 
         return {}
 
     @staticmethod
-    def get_new_classes_from_module(module: ModuleType) -> Dict[str, Type[Any]]:
+    def get_new_classes_from_module(module: ModuleType) -> dict[str, type[Any]]:
         """
         Skip classes not originated inside the module.
         """
 
         classes = {}
         for name, value in Meta.get_classes_from_module(module).items():
             if module.__name__ in value.__module__:
@@ -88,16 +88,15 @@
             if cls_attribute is not None and inspect.isclass(cls_attribute):
                 return args[0]
         return None
 
     @staticmethod
     def import_models(
         name: str, package: str, mandatory: bool = False
-    ) -> Dict[str, Type[Any]]:
-
+    ) -> dict[str, type[Any]]:
         if package == BACKEND_PACKAGE:
             module_name = f"{package}.connectors.{name}.models"
         else:
             module_name = f"{package}.models.{name}"
 
         try:
             module = Meta.get_module_from_string(module_name, exit_on_fail=True)
@@ -111,22 +110,22 @@
                 print_and_exit("Cannot load {} models from {}", name, module_name)
 
             return {}
 
         return Meta.get_new_classes_from_module(module)
 
     @staticmethod
-    def get_celery_tasks(package_name: str) -> List[Callable[..., Any]]:
+    def get_celery_tasks(package_name: str) -> list[Callable[..., Any]]:
         """
         Extract all celery tasks from a module.
         Celery tasks are functions decorated by @CeleryExt.celery_app.task(...)
         This decorator transform the function into a class child of
         celery.local.PromiseProxy
         """
-        tasks: List[Callable[..., Any]] = []
+        tasks: list[Callable[..., Any]] = []
         # package = tasks folder
         package = Meta.get_module_from_string(package_name)
         if package is None:
             return tasks
 
         # get all modules in package (i.e. py files)
         path = package.__path__
@@ -144,29 +143,27 @@
                 module_path,
                 exit_on_fail=True,
             )
 
             # get all functions in py file
             functions = inspect.getmembers(submodule)
             for func in functions:
-
                 obj_type = type(func[1])
 
                 if obj_type.__module__ != "celery.local":
                     continue
 
                 # This was a dict name => func
                 # tasks[func[0]] = func[1]
                 # Now it is a list
                 tasks.append(func[1])
         return tasks
 
     @staticmethod
     def get_class(module_relpath: str, class_name: str) -> Optional[Any]:
-
         abspath = f"{CUSTOM_PACKAGE}.{module_relpath}"
 
         module = Meta.get_module_from_string(abspath)
 
         if module is None:
             log.debug("{} path does not exist", abspath)
             return None
```

### Comparing `rapydo_http-2.4/restapi/utilities/processes.py` & `rapydo_http-3.0/restapi/utilities/processes.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import math
 import os
 import signal
 import socket
 import time
 from datetime import datetime
 from types import FrameType
-from typing import List, Optional
+from typing import Optional
 
 import psutil
 
 from restapi.config import TESTING
 from restapi.exceptions import ServiceUnavailable
 from restapi.utilities.logs import log
 
@@ -32,28 +32,26 @@
 
 def stop_timeout() -> None:
     signal.alarm(0)
 
 
 def find_process(
     process_name: str,
-    keywords: Optional[List[str]] = None,
+    keywords: Optional[list[str]] = None,
     prefix: Optional[str] = None,
 ) -> bool:
-
     if keywords is None:
         keywords = []
 
     if prefix:
         keywords.append(f"{prefix}{process_name}")
 
     current_pid = os.getpid()
 
     for pid in psutil.pids():
-
         if pid == current_pid or not psutil.pid_exists(pid):
             continue  # pragma: no cover
         process = psutil.Process(pid)
 
         if process.name() != process_name:
             continue
         cmd = process.cmdline()
@@ -70,26 +68,23 @@
 
     return False
 
 
 def wait_socket(
     host: str, port: int, service_name: str, retries: int = DEFAULT_MAX_RETRIES
 ) -> None:
-
     SLEEP_TIME = 2
     TIMEOUT = 1
 
     log.debug("Waiting for {} ({}:{})", service_name, host, port)
 
     counter = 0
     begin = time.time()
     while True:
-
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-
             s.settimeout(TIMEOUT)
 
             try:
                 result = s.connect_ex((host, port))
             except socket.gaierror:
                 result = errno.ESRCH
```

### Comparing `rapydo_http-2.4/tests/base/test_cli.py` & `rapydo_http-3.0/tests/base/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import pytest
 from click.testing import CliRunner
 
 from restapi import __commands__ as cli
 from restapi import decorators
 from restapi.connectors import Connector
+from restapi.server import ServerModes
 
 
 def test_cli() -> None:
     runner = CliRunner()
 
     response = runner.invoke(cli.verify, ["test"])
     assert response.exit_code == 2
@@ -73,15 +74,15 @@
     assert h == "myvalue"
     assert isinstance(p, int)
     assert p == 111
 
     from restapi.server import create_app
 
     if Connector.check_availability("redis"):
-        create_app(name="Cache clearing")
+        create_app(name="Cache clearing", mode=ServerModes.NORMAL, options={})
 
         # make_name prevents the use of rapydo default make_name function, that is only
         # working on endpoints context since it is based on tokens from flask.request
         @decorators.cache(timeout=3600, make_name=None)
         def random_values() -> int:
             return random.randrange(0, 100000)
```

### Comparing `rapydo_http-2.4/tests/base/test_connector_celery.py` & `rapydo_http-3.0/tests/base/test_connector_celery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 from datetime import timedelta
+from unittest.mock import patch
 
 import celery
 import pytest
 from faker import Faker
 from flask import Flask
 
 from restapi.config import get_project_configuration
@@ -20,27 +21,25 @@
 CONNECTOR_AVAILABLE = Connector.check_availability(CONNECTOR)
 
 
 @pytest.mark.skipif(
     CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be not available"
 )
 def test_no_celery() -> None:
-
     with pytest.raises(ServiceUnavailable):
         connector.get_instance()
 
     log.warning("Skipping {} tests: service not available", CONNECTOR)
     return None
 
 
 @pytest.mark.skipif(
     not CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be available"
 )
 def test_celery(app: Flask, faker: Faker) -> None:
-
     log.info("Executing {} tests", CONNECTOR)
 
     obj = connector.get_instance()
     assert obj is not None
 
     task = obj.celery_app.send_task("test_task", args=("myinput",))
 
@@ -186,24 +185,23 @@
 
     # ... close connection again ... nothing should happen
     obj.disconnect()
 
     with connector.get_instance() as obj:
         assert obj is not None
 
-    app = create_app(mode=ServerModes.WORKER)
+    app = create_app(name="Flask Tests", mode=ServerModes.WORKER, options={})
     assert app is not None
 
 
 @pytest.mark.skipif(
     not CONNECTOR_AVAILABLE or Env.get_bool("CELERYBEAT_ENABLED"),
     reason="This test needs celery-beat to be NOT available",
 )
 def test_no_celerybeat() -> None:
-
     obj = connector.get_instance()
     assert obj is not None
 
     with pytest.raises(
         AttributeError, match=r"Unsupported celery-beat scheduler: None"
     ):
         # get_periodic_task with unknown CELERYBEAT_SCHEDULER
@@ -231,15 +229,14 @@
 
 
 @pytest.mark.skipif(
     not CONNECTOR_AVAILABLE or not Env.get_bool("CELERYBEAT_ENABLED"),
     reason="This test needs celery-beat to be available",
 )
 def test_celerybeat() -> None:
-
     obj = connector.get_instance()
     assert obj is not None
 
     assert obj.get_periodic_task("does_not_exist") is None
     assert not obj.delete_periodic_task("does_not_exist")
 
     obj.create_periodic_task(name="task1", task="task.does.not.exists", every="60")
@@ -279,15 +276,14 @@
         kwargs={"a": 1, "b": 2, "c": 3},
     )
 
     assert obj.delete_periodic_task("task2_bis")
     assert not obj.delete_periodic_task("task2_bis")
 
     if CeleryExt.CELERYBEAT_SCHEDULER == "REDIS":
-
         obj.create_periodic_task(
             name="task3",
             task="task.does.not.exists",
             every=60,
         )
         assert obj.delete_periodic_task("task3")
```

### Comparing `rapydo_http-2.4/tests/base/test_connector_ftp.py` & `rapydo_http-3.0/tests/base/test_connector_ftp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import tempfile
 import time
 from pathlib import Path
+from unittest.mock import patch
 
 import pytest
 from faker import Faker
 from flask import Flask
 
 from restapi.connectors import Connector
 from restapi.connectors import ftp as connector
@@ -15,27 +16,25 @@
 CONNECTOR_AVAILABLE = Connector.check_availability(CONNECTOR)
 
 
 @pytest.mark.skipif(
     CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be not available"
 )
 def test_no_ftp() -> None:
-
     with pytest.raises(ServiceUnavailable):
         connector.get_instance()
 
     log.warning("Skipping {} tests: service not available", CONNECTOR)
     return None
 
 
 @pytest.mark.skipif(
     not CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be available"
 )
 def test_ftp(app: Flask, faker: Faker) -> None:
-
     log.info("Executing {} tests", CONNECTOR)
 
     with pytest.raises(ServiceUnavailable):
         connector.get_instance(host="invalidhostname", port="123")
 
     obj = connector.get_instance()
     assert obj is not None
@@ -101,7 +100,35 @@
             # Command for Downloading the file "RETR filename"
             # or retrbinary for binary mode
             obj.connection.retrlines(f"RETR {ftp_filename}", download_handle.write)
 
         with open(download_file) as download_handle:
             downloaded_content = download_handle.read()
             assert downloaded_content == tmp_content
+
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry value: 0"):
+        connector.get_instance(retries=0, retry_wait=0)
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry value: -1"):
+        connector.get_instance(retries=-1, retry_wait=0)
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry wait value: -1"):
+        connector.get_instance(retries=1, retry_wait=-1)
+    obj = connector.get_instance(retries=1, retry_wait=0)
+    assert obj is not None
+
+    MOCKED_RETURN = connector.get_instance()
+    # Clean the cache
+    Connector.disconnect_all()
+    WAIT = 1
+    with patch.object(Connector, "initialize_connection") as mock:
+        start = time.time()
+        mock.side_effect = [
+            ServiceUnavailable("first"),
+            ServiceUnavailable("second"),
+            MOCKED_RETURN,
+        ]
+        obj = connector.get_instance(retries=10, retry_wait=WAIT)
+
+        assert mock.call_count == 3
+        assert obj == MOCKED_RETURN
+        end = time.time()
+
+        assert end - start > WAIT
```

### Comparing `rapydo_http-2.4/tests/base/test_connector_neo4j.py` & `rapydo_http-3.0/tests/base/test_connector_neo4j.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 from datetime import datetime
+from unittest.mock import patch
 
 import dateutil.parser
 import pytest
 import pytz
 from faker import Faker
 from flask import Flask
 from neo4j.exceptions import CypherSyntaxError
@@ -20,15 +21,14 @@
 CONNECTOR_AVAILABLE = Connector.check_availability(CONNECTOR)
 
 
 @pytest.mark.skipif(
     CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be not available"
 )
 def test_no_neo4j() -> None:
-
     with pytest.raises(ServiceUnavailable):
         connector.get_instance()
 
     log.warning("Skipping {} tests: service not available", CONNECTOR)
     return None
 
 
@@ -51,15 +51,14 @@
         data["modified1"] = dateutil.parser.parse(data["modified1"])
         data["modified2"] = dateutil.parser.parse(data["modified2"])
         assert data["created"] < data["modified1"]
         assert data["modified1"] < data["modified2"]
 
     @staticmethod
     def test_connector(app: Flask, faker: Faker) -> None:
-
         obj = connector.get_instance()
         assert obj is not None
 
         with pytest.raises(AttributeError, match=r"Model InvalidModel not found"):
             obj.InvalidModel
 
         for row in obj.cypher("MATCH (u: User) RETURN u limit 1"):
@@ -74,15 +73,15 @@
             token=v,
             token_type=BaseAuthentication.FULL_TOKEN,
             creation=datetime.now(pytz.utc),
         ).save()
         assert t.emitted_for.single() is None
         t.delete()
 
-        with pytest.raises(CypherSyntaxError, match=r"{code: None} {message: None}"):
+        with pytest.raises(CypherSyntaxError, match=r"Failed to execute Cypher Query"):
             obj.cypher("MATCH (n) RETURN n with a syntax error")
         # Query information are removed from the CypherSyntaxError exception
 
         assert obj.sanitize_input("x") == "x"
         assert obj.sanitize_input("x ") == "x"
         assert obj.sanitize_input(" x") == "x"
         assert obj.sanitize_input("*x") == "x"
@@ -135,17 +134,44 @@
 
         with pytest.raises(ServiceUnavailable):
             connector.get_instance(host="invalidhostname", port="123")
 
         with pytest.raises(ServiceUnavailable):
             connector.get_instance(user="invaliduser")
 
+        with pytest.raises(ServiceUnavailable, match=r"Invalid retry value: 0"):
+            connector.get_instance(retries=0, retry_wait=0)
+        with pytest.raises(ServiceUnavailable, match=r"Invalid retry value: -1"):
+            connector.get_instance(retries=-1, retry_wait=0)
+        with pytest.raises(ServiceUnavailable, match=r"Invalid retry wait value: -1"):
+            connector.get_instance(retries=1, retry_wait=-1)
+        obj = connector.get_instance(retries=1, retry_wait=0)
+        assert obj is not None
+
+        MOCKED_RETURN = connector.get_instance()
+        # Clean the cache
+        Connector.disconnect_all()
+        WAIT = 1
+        with patch.object(Connector, "initialize_connection") as mock:
+            start = time.time()
+            mock.side_effect = [
+                ServiceUnavailable("first"),
+                ServiceUnavailable("second"),
+                MOCKED_RETURN,
+            ]
+            obj = connector.get_instance(retries=10, retry_wait=WAIT)
+
+            assert mock.call_count == 3
+            assert obj == MOCKED_RETURN
+            end = time.time()
+
+            assert end - start > WAIT
+
     @staticmethod
     def test_parser() -> None:
-
         with pytest.raises(ValueError):
             # missing :type
             node1 = NodeDump("TestNode1", fields=["f1"])
 
         node1 = NodeDump("TestNode1", fields=["f1:string", "f2:int", "f3:float"])
 
         node2 = NodeDump("TestNode2", fields=["f1:string", "f2:int", "f3:float"])
```

### Comparing `rapydo_http-2.4/tests/base/test_connector_rabbit.py` & `rapydo_http-3.0/tests/base/test_connector_rabbit.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from unittest.mock import patch
 
 import pytest
 from faker import Faker
 from flask import Flask
 
 from restapi.connectors import Connector
 from restapi.connectors import rabbitmq as connector
@@ -13,27 +14,25 @@
 CONNECTOR_AVAILABLE = Connector.check_availability(CONNECTOR)
 
 
 @pytest.mark.skipif(
     CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be not available"
 )
 def test_no_rabbit() -> None:
-
     with pytest.raises(ServiceUnavailable):
         connector.get_instance()
 
     log.warning("Skipping {} tests: service not available", CONNECTOR)
     return None
 
 
 @pytest.mark.skipif(
     not CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be available"
 )
 def test_rabbit(app: Flask, faker: Faker) -> None:
-
     log.info("Executing {} tests", CONNECTOR)
 
     with pytest.raises(ServiceUnavailable):
         connector.get_instance(host="invalidhostname", port="123")
 
     obj = connector.get_instance()
     assert obj is not None
@@ -156,7 +155,35 @@
     assert not obj.is_connected()
 
     # ... close connection again ... nothing should happen
     obj.disconnect()
 
     with connector.get_instance() as obj:
         assert obj is not None
+
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry value: 0"):
+        connector.get_instance(retries=0, retry_wait=0)
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry value: -1"):
+        connector.get_instance(retries=-1, retry_wait=0)
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry wait value: -1"):
+        connector.get_instance(retries=1, retry_wait=-1)
+    obj = connector.get_instance(retries=1, retry_wait=0)
+    assert obj is not None
+
+    MOCKED_RETURN = connector.get_instance()
+    # Clean the cache
+    Connector.disconnect_all()
+    WAIT = 1
+    with patch.object(Connector, "initialize_connection") as mock:
+        start = time.time()
+        mock.side_effect = [
+            ServiceUnavailable("first"),
+            ServiceUnavailable("second"),
+            MOCKED_RETURN,
+        ]
+        obj = connector.get_instance(retries=10, retry_wait=WAIT)
+
+        assert mock.call_count == 3
+        assert obj == MOCKED_RETURN
+        end = time.time()
+
+        assert end - start > WAIT
```

### Comparing `rapydo_http-2.4/tests/base/test_connector_redis.py` & `rapydo_http-3.0/tests/base/test_connector_redis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from unittest.mock import patch
 
 import pytest
 from flask import Flask
 
 from restapi.connectors import Connector
 from restapi.connectors import redis as connector
 from restapi.exceptions import ServiceUnavailable
@@ -12,27 +13,25 @@
 CONNECTOR_AVAILABLE = Connector.check_availability(CONNECTOR)
 
 
 @pytest.mark.skipif(
     CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be not available"
 )
 def test_no_redis() -> None:
-
     with pytest.raises(ServiceUnavailable):
         connector.get_instance()
 
     log.warning("Skipping {} tests: service not available", CONNECTOR)
     return None
 
 
 @pytest.mark.skipif(
     not CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be available"
 )
 def test_redis(app: Flask) -> None:
-
     log.info("Executing {} tests", CONNECTOR)
 
     obj = connector.get_instance(host="invalidhostname", port="123")
     assert obj is not None
     assert not obj.is_connected()
 
     obj = connector.get_instance()
@@ -70,7 +69,35 @@
     # assert not oj.is_connected()
 
     # ... close connection again ... nothing should happen
     obj.disconnect()
 
     with connector.get_instance() as obj:
         assert obj is not None
+
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry value: 0"):
+        connector.get_instance(retries=0, retry_wait=0)
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry value: -1"):
+        connector.get_instance(retries=-1, retry_wait=0)
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry wait value: -1"):
+        connector.get_instance(retries=1, retry_wait=-1)
+    obj = connector.get_instance(retries=1, retry_wait=0)
+    assert obj is not None
+
+    MOCKED_RETURN = connector.get_instance()
+    # Clean the cache
+    Connector.disconnect_all()
+    WAIT = 1
+    with patch.object(Connector, "initialize_connection") as mock:
+        start = time.time()
+        mock.side_effect = [
+            ServiceUnavailable("first"),
+            ServiceUnavailable("second"),
+            MOCKED_RETURN,
+        ]
+        obj = connector.get_instance(retries=10, retry_wait=WAIT)
+
+        assert mock.call_count == 3
+        assert obj == MOCKED_RETURN
+        end = time.time()
+
+        assert end - start > WAIT
```

### Comparing `rapydo_http-2.4/tests/base/test_connector_smtp.py` & `rapydo_http-3.0/tests/base/test_connector_smtp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import time
+from unittest.mock import patch
+
 import pytest
 from faker import Faker
 from flask import Flask
 
 from restapi.connectors import Connector
 from restapi.connectors import smtp as connector
 from restapi.exceptions import ServiceUnavailable
@@ -13,27 +16,25 @@
 
 
 # mailmock is always enabled during core tests
 @pytest.mark.skipif(
     CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be not available"
 )
 def test_no_smtp() -> None:  # pragma: no cover
-
     with pytest.raises(ServiceUnavailable):
         connector.get_instance()
 
     log.warning("Skipping {} tests: service not available", CONNECTOR)
     return None
 
 
 @pytest.mark.skipif(
     not CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be available"
 )
 def test_smtp(app: Flask, faker: Faker) -> None:
-
     obj = connector.get_instance()
     assert obj is not None
     assert obj.smtp is not None
 
     obj = connector.get_instance(port="465")
     assert obj is not None
     assert obj.smtp is not None
@@ -86,15 +87,15 @@
     headers = mail.get("headers")
     assert body is not None
     assert headers is not None
     # Subject: is a key in the MIMEText
     assert "Subject: subject" in headers
     assert mail.get("from") == "from_addr"
     # format is [to, [cc...], [bcc...]]
-    assert mail.get("cc") == ["to_addr", ["test1", "test2"], ["test3", "test4"]]
+    assert mail.get("cc") == ["to_addr", "test1", "test2", "test3", "test4"]
 
     # This is a special from_address, used to raise SMTPException
     assert not obj.send("body", "subject", "to_addr", "invalid1")
     # This is a special from_address, used to raise Exception
     obj = connector.get_instance()
     assert not obj.send("body", "subject", "to_addr", "invalid2")
     # This is NOT a special from_address
@@ -137,7 +138,35 @@
     assert obj.is_connected()
     obj.disconnect()
 
     # a second disconnect should not raise any error
     obj.disconnect()
 
     assert not obj.is_connected()
+
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry value: 0"):
+        connector.get_instance(retries=0, retry_wait=0)
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry value: -1"):
+        connector.get_instance(retries=-1, retry_wait=0)
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry wait value: -1"):
+        connector.get_instance(retries=1, retry_wait=-1)
+    obj = connector.get_instance(retries=1, retry_wait=0)
+    assert obj is not None
+
+    MOCKED_RETURN = connector.get_instance()
+    # Clean the cache
+    Connector.disconnect_all()
+    WAIT = 1
+    with patch.object(Connector, "initialize_connection") as mock:
+        start = time.time()
+        mock.side_effect = [
+            ServiceUnavailable("first"),
+            ServiceUnavailable("second"),
+            MOCKED_RETURN,
+        ]
+        obj = connector.get_instance(retries=10, retry_wait=WAIT)
+
+        assert mock.call_count == 3
+        assert obj == MOCKED_RETURN
+        end = time.time()
+
+        assert end - start > WAIT
```

### Comparing `rapydo_http-2.4/tests/base/test_connector_sqlalchemy.py` & `rapydo_http-3.0/tests/base/test_connector_sqlalchemy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from unittest.mock import patch
 
 import pytest
 from flask import Flask
 
 from restapi.connectors import Connector
 from restapi.connectors import sqlalchemy as connector
 from restapi.exceptions import ServiceUnavailable
@@ -12,32 +13,29 @@
 CONNECTOR_AVAILABLE = Connector.check_availability(CONNECTOR)
 
 
 @pytest.mark.skipif(
     CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be not available"
 )
 def test_no_sqlalchemy() -> None:
-
     with pytest.raises(ServiceUnavailable):
         connector.get_instance()
 
     log.warning("Skipping {} tests: service not available", CONNECTOR)
     return None
 
 
 @pytest.mark.skipif(
     not CONNECTOR_AVAILABLE, reason=f"This test needs {CONNECTOR} to be available"
 )
 def test_sqlalchemy(app: Flask) -> None:
-
     log.info("Executing {} tests", CONNECTOR)
 
-    if not connector.SQLAlchemy.is_mysql():
-        with pytest.raises(ServiceUnavailable):
-            connector.get_instance(host="invalidhostname", port="123")
+    with pytest.raises(ServiceUnavailable):
+        connector.get_instance(host="invalidhostname", port="123")
 
     with pytest.raises(ServiceUnavailable):
         connector.get_instance(user="invaliduser")
 
     obj = connector.get_instance()
     assert obj is not None
 
@@ -77,7 +75,35 @@
 
     # ... close connection again ... nothing should happen
     obj.disconnect()
 
     # sqlalchemy connector does not support with context
     # with connector.get_instance() as obj:
     #     assert obj is not None
+
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry value: 0"):
+        connector.get_instance(retries=0, retry_wait=0)
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry value: -1"):
+        connector.get_instance(retries=-1, retry_wait=0)
+    with pytest.raises(ServiceUnavailable, match=r"Invalid retry wait value: -1"):
+        connector.get_instance(retries=1, retry_wait=-1)
+    obj = connector.get_instance(retries=1, retry_wait=0)
+    assert obj is not None
+
+    MOCKED_RETURN = connector.get_instance()
+    # Clean the cache
+    Connector.disconnect_all()
+    WAIT = 1
+    with patch.object(Connector, "initialize_connection") as mock:
+        start = time.time()
+        mock.side_effect = [
+            ServiceUnavailable("first"),
+            ServiceUnavailable("second"),
+            MOCKED_RETURN,
+        ]
+        obj = connector.get_instance(retries=10, retry_wait=WAIT)
+
+        assert mock.call_count == 3
+        assert obj == MOCKED_RETURN
+        end = time.time()
+
+        assert end - start > WAIT
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_admin_groups.py` & `rapydo_http-3.0/tests/base/test_endpoints_admin_groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Set
-
 import orjson
 import pytest
 from faker import Faker
 
 from restapi.connectors import Connector
 from restapi.env import Env
 from restapi.services.authentication import BaseAuthentication, Role
@@ -15,26 +13,24 @@
     # faker.company alone is not always enough and some
     # "Group already exists with shortname" occasionally occur during tests
     return f"{faker.company()}-{faker.pyint(2, 100)}"
 
 
 class TestApp(BaseTests):
     def test_admin_groups(self, client: FlaskClient, faker: Faker) -> None:
-
         if not Env.get_bool("MAIN_LOGIN_ENABLE") or not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping admin/groups tests")
             return
 
         auth = Connector.get_authentication_instance()
         staff_role_enabled = Role.STAFF.value in [r.name for r in auth.get_roles()]
         for role in (
             Role.ADMIN,
             Role.STAFF,
         ):
-
             if not staff_role_enabled:  # pragma: no cover
                 log.warning(
                     "Skipping tests of admin/groups endpoints, role Staff not enabled"
                 )
                 continue
             else:
                 log.warning("Testing admin/groups endpoints as {}", role)
@@ -84,15 +80,14 @@
             assert "members" in groups[0]
             assert len(groups[0]["members"]) > 0
             assert "coordinators" in groups[0]
 
             fullname = None
             for g in groups:
                 if g.get("uuid") == uuid:
-
                     fullname = g.get("fullname")
                     break
             else:  # pragma: no cover
                 pytest.fail("Group not found")
 
             assert fullname is not None
 
@@ -137,22 +132,27 @@
 
             r = client.get(f"{API_URI}/admin/groups", headers=headers)
             assert r.status_code == 200
             groups = self.get_content(r)
             assert isinstance(groups, list)
             for g in groups:
                 if g.get("uuid") == uuid:
-
                     assert g.get("fullname") == newdata.get("fullname")
                     assert g.get("fullname") != data.get("fullname")
                     assert g.get("fullname") != fullname
 
             r = client.put(f"{API_URI}/admin/groups/xyz", json=data, headers=headers)
             assert r.status_code == 404
 
+            # members = auth.get_group_members(group)
+            # with pytest.raises(
+            #     Forbidden,
+            #     match=rf"Cannot delete this group, it is assigned to {len(members)} user(s)",
+            # ):
+
             # Event 3: delete
             r = client.delete(f"{API_URI}/admin/groups/{uuid}", headers=headers)
             assert r.status_code == 204
 
             events = self.get_last_events(1, filters={"target_type": "Group"})
             # Group is deleted (same target_id as above)
             assert events[0].event == Events.delete.value
@@ -248,15 +248,15 @@
             r = client.get(f"{API_URI}/admin/groups", headers=headers)
             assert r.status_code == 200
             groups = self.get_content(r)
             assert isinstance(groups, list)
             assert len(groups) > 0
 
             # Extract all coordinators:
-            coordinators: Set[str] = set()
+            coordinators: set[str] = set()
             for group in groups:
                 for coordinator in group["coordinators"]:
                     coordinators.add(coordinator["email"])
 
             assert user_email in coordinators
 
             if role == Role.ADMIN:
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_admin_logins.py` & `rapydo_http-3.0/tests/base/test_endpoints_admin_logins.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from restapi.services.authentication import BaseAuthentication
 from restapi.tests import API_URI, BaseTests, FlaskClient
 from restapi.utilities.logs import log
 
 
 class TestApp(BaseTests):
     def test_admin_stats(self, client: FlaskClient, faker: Faker) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping admin/logins tests")
             return
 
         r = client.get(f"{API_URI}/admin/logins")
         assert r.status_code == 401
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_admin_stats.py` & `rapydo_http-3.0/tests/base/test_endpoints_admin_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from restapi.env import Env
 from restapi.tests import API_URI, BaseTests, FlaskClient
 from restapi.utilities.logs import log
 
 
 class TestApp(BaseTests):
     def test_admin_stats(self, client: FlaskClient) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping admin/stats tests")
             return
 
         r = client.get(f"{API_URI}/admin/stats")
         assert r.status_code == 401
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_admin_users.py` & `rapydo_http-3.0/tests/base/test_endpoints_admin_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,29 +8,27 @@
 from restapi.services.authentication import BaseAuthentication, Role
 from restapi.tests import API_URI, AUTH_URI, BaseTests, FlaskClient
 from restapi.utilities.logs import OBSCURE_VALUE, Events, log
 
 
 class TestApp(BaseTests):
     def test_admin_users(self, client: FlaskClient, faker: Faker) -> None:
-
         if not Env.get_bool("MAIN_LOGIN_ENABLE") or not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping admin/users tests")
             return
 
         project_tile = get_project_configuration("project.title", default="YourProject")
 
         auth = Connector.get_authentication_instance()
         staff_role_enabled = Role.STAFF.value in [r.name for r in auth.get_roles()]
 
         for role in (
             Role.ADMIN,
             Role.STAFF,
         ):
-
             if not staff_role_enabled:  # pragma: no cover
                 log.warning(
                     "Skipping tests of admin/users endpoints, role Staff not enabled"
                 )
                 continue
             else:
                 log.warning("Testing admin/users endpoints as {}", role)
@@ -381,15 +379,14 @@
             # Verify that the password is obfuscated in the log:
             assert events[0].payload["password"] == OBSCURE_VALUE
 
             r = client.get(f"{AUTH_URI}/logout", headers=headers)
             assert r.status_code == 204
 
     def test_staff_restrictions(self, client: FlaskClient, faker: Faker) -> None:
-
         if not Env.get_bool("MAIN_LOGIN_ENABLE") or not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping admin/users tests")
             return
 
         auth = Connector.get_authentication_instance()
         staff_role_enabled = Role.STAFF.value in [r.name for r in auth.get_roles()]
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_authentication.py` & `rapydo_http-3.0/tests/base/test_endpoints_authentication.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from restapi.services.authentication import BaseAuthentication, Role
 from restapi.tests import API_URI, BaseTests, FlaskClient
 from restapi.utilities.logs import log
 
 
 class TestApp(BaseTests):
     def test_no_auth(self, client: FlaskClient) -> None:
-
         r = client.get(f"{API_URI}/tests/noauth")
         assert r.status_code == 200
         assert self.get_content(r) == "OK"
 
         if Env.get_bool("AUTH_ENABLE"):
             headers, _ = self.do_login(client, None, None)
 
@@ -24,15 +23,14 @@
         r = client.get(
             f"{API_URI}/tests/noauth", headers={"Authorization": "Bearer invalid"}
         )
         assert r.status_code == 200
         assert self.get_content(r) == "OK"
 
     def test_auth(self, client: FlaskClient) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping authentication tests")
             return
 
         r = client.get(f"{API_URI}/tests/authentication")
         assert r.status_code == 401
 
@@ -48,23 +46,39 @@
         assert r.status_code == 200
         content = self.get_content(r)
         assert isinstance(content, dict)
         assert len(content) == 1
         assert "email" in content
         assert content["email"] == BaseAuthentication.default_user
 
+        # Token type is case insensitive.
+        r = client.get(
+            f"{API_URI}/tests/authentication",
+            headers={"Authorization": f"bearer {token}"},
+        )
+        assert r.status_code == 200
+        r = client.get(
+            f"{API_URI}/tests/authentication",
+            headers={"Authorization": f"BEARER {token}"},
+        )
+        assert r.status_code == 200
+        r = client.get(
+            f"{API_URI}/tests/authentication",
+            headers={"Authorization": f"BeArEr {token}"},
+        )
+        assert r.status_code == 200
+
         if not Env.get_bool("ALLOW_ACCESS_TOKEN_PARAMETER"):
             # access token parameter is not allowed by default
             r = client.get(
                 f"{API_URI}/tests/authentication", query_string={"access_token": token}
             )
             assert r.status_code == 401
 
     def test_optional_auth(self, client: FlaskClient) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping authentication tests")
             return
 
         # Optional authentication can accept missing tokens
         r = client.get(f"{API_URI}/tests/optionalauthentication")
         assert r.status_code == 204
@@ -100,15 +114,14 @@
                 f"{API_URI}/tests/optionalauthentication",
                 query_string={"access_token": "invalid"},
             )
             # invalid tokens should be rejected, but query token is ignored
             assert r.status_code == 204
 
     def test_access_token_parameter(self, client: FlaskClient) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping authentication tests")
             return
 
         r = client.get(f"{API_URI}/tests/queryauthentication")
         assert r.status_code == 401
 
@@ -141,15 +154,14 @@
         r = client.get(
             f"{API_URI}/tests/queryauthentication",
             query_string={"access_token": "invalid"},
         )
         assert r.status_code == 401
 
     def test_optional_access_token_parameter(self, client: FlaskClient) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping authentication tests")
             return
 
         # Optional authentication can accept missing tokens
         r = client.get(f"{API_URI}/tests/optionalqueryauthentication")
         assert r.status_code == 204
@@ -187,15 +199,14 @@
             f"{API_URI}/tests/optionalqueryauthentication",
             query_string={"access_token": "invalid"},
         )
         # invalid tokens should be rejected, but query token is ignored
         assert r.status_code == 401
 
     def test_authentication_with_multiple_roles(self, client: FlaskClient) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping authentication tests")
             return
 
         r = client.get(f"{API_URI}/tests/manyrolesauthentication")
         assert r.status_code == 401
 
@@ -239,15 +250,14 @@
                 f"{API_URI}/tests/unknownroleauthentication", headers=user_header
             )
             assert r.status_code == 401
 
             self.delete_user(client, uuid)
 
     def test_authentication_with_auth_callback(self, client: FlaskClient) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping authentication tests")
             return
 
         auth = Connector.get_authentication_instance()
         user = auth.get_user(username=BaseAuthentication.default_user)
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_authorizations.py` & `rapydo_http-3.0/tests/base/test_endpoints_authorizations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Dict, List, Optional
+from typing import Optional
 
 import pytest
 
 from restapi.config import ABS_RESTAPI_PATH
 from restapi.connectors import Connector
 from restapi.env import Env
 from restapi.rest.loader import EndpointsLoader
@@ -20,42 +20,39 @@
         path = re.sub(r"\<[a-zA-Z0-9_]+\>", "VARIABLE", path)
         return f"{method} {path}"
 
     # This utility returns a list of _core_ paths with the form:
     # METHOD /path, e.g.
     # GET /api/admin/users
     # POST /api/admin/users
-    def get_paths(self, client: FlaskClient) -> List[str]:
-
+    def get_paths(self, client: FlaskClient) -> list[str]:
         loader = EndpointsLoader()
         loader.load_endpoints_folder(ABS_RESTAPI_PATH)
 
-        paths: List[str] = []
+        paths: list[str] = []
         for endpoint_class in loader.endpoints:
             for method, path in endpoint_class.methods.items():
-
                 if path.startswith("/api/tests/"):
                     continue
 
                 paths.append(self.get_path(method, path))
 
         return paths
 
     # Test a single endpoint, remove the path from the list and return the new list
     # Once tested all paths, the list should be empty
     def check_endpoint(
         self,
         client: FlaskClient,
         method: str,
         endpoint: str,
-        headers: Optional[Dict[str, str]],
+        headers: Optional[dict[str, str]],
         expected_authorized: bool,
-        paths: List[str],
-    ) -> List[str]:
-
+        paths: list[str],
+    ) -> list[str]:
         assert method in (
             "GET",
             "POST",
             "PUT",
             "PATCH",
             "DELETE",
         )
@@ -85,15 +82,14 @@
         else:
             assert r.status_code != 400
 
         paths.remove(path)
         return paths
 
     def test_admin(self, client: FlaskClient) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping admin authorizations tests")
             return
 
         # List of all paths to be tested. After each test a path will be removed.
         # At the end the list is expected to be empty
         paths = self.get_paths(client)
@@ -202,15 +198,14 @@
         paths = self.check_endpoint(client, "GET", "/auth/logout", headers, True, paths)
 
         assert paths == []
 
         self.delete_user(client, uuid)
 
     def test_staff(self, client: FlaskClient) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping staff authorizations tests")
             return
 
         auth = Connector.get_authentication_instance()
         auth.get_roles()
 
@@ -328,15 +323,14 @@
         paths = self.check_endpoint(client, "GET", "/auth/logout", headers, True, paths)
 
         assert paths == []
 
         self.delete_user(client, uuid)
 
     def test_coordinator(self, client: FlaskClient) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping coordinator authorizations tests")
             return
 
         # List of all paths to be tested. After each test a path will be removed.
         # At the end the list is expected to be empty
         paths = self.get_paths(client)
@@ -445,15 +439,14 @@
         paths = self.check_endpoint(client, "GET", "/auth/logout", headers, True, paths)
 
         assert paths == []
 
         self.delete_user(client, uuid)
 
     def test_user(self, client: FlaskClient) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping user authorizations tests")
             return
 
         # List of all paths to be tested. After each test a path will be removed.
         # At the end the list is expected to be empty
         paths = self.get_paths(client)
@@ -571,15 +564,14 @@
         paths = self.get_paths(client)
         headers = None
         # These are public
         paths = self.check_endpoint(client, "GET", "/api/status", headers, True, paths)
         paths = self.check_endpoint(client, "GET", "/api/specs", headers, True, paths)
 
         if not Env.get_bool("AUTH_ENABLE"):
-
             assert paths == []
 
             log.warning("Skipping other public authorizations tests")
             return
 
         paths = self.check_endpoint(client, "POST", "/auth/login", headers, True, paths)
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_autocomplete.py` & `rapydo_http-3.0/tests/base/test_endpoints_autocomplete.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import orjson
 
 from restapi.tests import API_URI, SERVER_URI, BaseTests, FlaskClient
 
 
 class TestApp(BaseTests):
     def test_autocomplete(self, client: FlaskClient) -> None:
-
         # This test verifies that buildData is always able to randomly create
         # valid inputs for endpoints with inputs defined by marshamallow schemas
         schema = self.get_dynamic_input_schema(client, "tests/autocomplete", {})
 
         assert schema[0]["key"] == "elements"
         assert schema[0]["type"] == "string[]"
         assert "autocomplete_endpoint" in schema[0]
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_caching.py` & `rapydo_http-3.0/tests/base/test_endpoints_caching.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,29 +18,24 @@
 
 
 @pytest.mark.skipif(
     CONNECTOR_AVAILABLE, reason="This test needs Redis to be not available"
 )
 class TestAppNoRedis(BaseTests):
     def test_caching_autocleaning(self, app: Flask) -> None:
-
         with pytest.raises(ServiceUnavailable):
             Cache.get_instance(app)
 
 
 @pytest.mark.skipif(
     not CONNECTOR_AVAILABLE, reason="This test needs Redis to be available"
 )
 class TestAppWithRedis(BaseTests):
     def test_caching_autocleaning(self, client: FlaskClient) -> None:
-
-        if Env.get_bool("AUTH_ENABLE"):
-            headers, _ = self.do_login(client, None, None)
-        else:
-            headers = None
+        headers, _ = self.do_login(client, None, None)
 
         # Syncronize this test to start at the beginning of the next second and
         # prevent the test to overlap a change of second
         # Since the caching is rounded to the second, few milliseconds cann make the
         # difference, for example:
         # A first request at 00:00:00.997 is cached
         # A second request at 00:00:01.002 is no longer cached, even if only 5 millisec
@@ -84,19 +79,15 @@
         r = client.get(
             f"{API_URI}/tests/cache/short", headers={"Authorization": "Bearer invalid"}
         )
         assert r.status_code == 200
         assert self.get_content(r) == counter2
 
     def test_caching_general_clearing(self, client: FlaskClient) -> None:
-
-        if Env.get_bool("AUTH_ENABLE"):
-            headers, _ = self.do_login(client, None, None)
-        else:
-            headers = None
+        headers, _ = self.do_login(client, None, None)
 
         # get method is cached for 200 seconds
 
         # First response is not cached
         r = client.get(f"{API_URI}/tests/cache/long")
         assert r.status_code == 200
         counter1 = self.get_content(r)
@@ -143,19 +134,14 @@
         r = client.get(
             f"{API_URI}/tests/cache/long", headers={"Authorization": "Bearer invalid"}
         )
         assert r.status_code == 200
         assert self.get_content(r) == counter3
 
     def test_cached_authenticated_endpoint(self, client: FlaskClient) -> None:
-
-        if not Env.get_bool("AUTH_ENABLE"):
-            log.warning("Skipping cache with authentication tests")
-            return
-
         headers1, _ = self.do_login(client, None, None)
 
         r = client.get(f"{API_URI}/tests/cache/auth", headers=headers1)
         assert r.status_code == 200
         resp1 = self.get_content(r)
         assert isinstance(resp1, list)
         # counter is 1 because this is the first request to this endpoint
@@ -219,19 +205,14 @@
             assert resp5[UUID] == resp4[UUID]
             # Same counter as above, because the response is replied from the cache
             assert resp5[COUNTER] == 3
 
             self.delete_user(client, uuid)
 
     def test_cached_semiauthenticated_endpoint(self, client: FlaskClient) -> None:
-
-        if not Env.get_bool("AUTH_ENABLE"):
-            log.warning("Skipping cache with authentication tests")
-            return
-
         r = client.get(f"{API_URI}/tests/cache/optionalauth")
         assert r.status_code == 200
         nonauthenticated1 = self.get_content(r)
         assert isinstance(nonauthenticated1, list)
         assert nonauthenticated1[UUID] == "N/A"
         # counter is 1 because this is the first request to this endpoint
         assert nonauthenticated1[COUNTER] == 1
@@ -275,19 +256,14 @@
         r = client.get(
             f"{API_URI}/tests/cache/optionalauth",
             headers={"Authorization": "Bearer invalid"},
         )
         assert r.status_code == 401
 
     def test_cached_authenticated_param_endpoint(self, client: FlaskClient) -> None:
-
-        if not Env.get_bool("AUTH_ENABLE"):
-            log.warning("Skipping cache with authentication tests")
-            return
-
         headers1, _ = self.do_login(client, None, None)
 
         r = client.get(f"{API_URI}/tests/cache/paramauth", headers=headers1)
         assert r.status_code == 200
         resp1 = self.get_content(r)
         assert isinstance(resp1, list)
         # counter is 1 because this is the first request to this endpoint
@@ -335,19 +311,14 @@
         assert isinstance(resp5, list)
         assert resp5[UUID] == resp1[UUID]
         # Same counter as above, because the response is replied from the cache
         assert resp5[COUNTER] == resp3[COUNTER]
         assert resp5[COUNTER] == 2
 
     def test_cached_semiauthenticated_param_endpoint(self, client: FlaskClient) -> None:
-
-        if not Env.get_bool("AUTH_ENABLE"):
-            log.warning("Skipping cache with authentication tests")
-            return
-
         r = client.get(f"{API_URI}/tests/cache/optionalparamauth")
         assert r.status_code == 200
         nonauthenticated1 = self.get_content(r)
         assert isinstance(nonauthenticated1, list)
         assert nonauthenticated1[UUID] == "N/A"
         # counter is 1 because this is the first request to this endpoint
         assert nonauthenticated1[COUNTER] == 1
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_db_exceptions.py` & `rapydo_http-3.0/tests/base/test_endpoints_db_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from restapi.services.authentication import DEFAULT_GROUP_NAME
 from restapi.tests import API_URI, BaseTests, FlaskClient
 from restapi.utilities.logs import log
 
 
 class TestApp(BaseTests):
     def test_database_exceptions(self, client: FlaskClient, faker: Faker) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping dabase exceptions tests")
             return
 
         # This is a special value. The endpoint will try to create a group without
         # shortname. A BadRequest is expected because the database should refuse the
         # entry due to the missing property
@@ -47,14 +46,17 @@
         new_fullname = default_group.fullname
 
         # This will try to create again a group with short/full name == random_name
         # but this will fail due to unique keys
         r = client.post(f"{API_URI}/tests/database/{random_name}")
         assert r.status_code == 409
         # This is the message of a DatabaseDuplicatedEntry
-        self.get_content(r) == "A Group already exists with 'shortname': '400'"
+        assert (
+            self.get_content(r)
+            == f"A Group already exists with shortname: {random_name}"
+        )
         # The default group will not change again because the
         # database_transaction decorator will undo the change
         default_group = auth.get_group(name=DEFAULT_GROUP_NAME)
         assert default_group is not None
 
         assert default_group.fullname == new_fullname
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_depends_on.py` & `rapydo_http-3.0/tests/base/test_endpoints_depends_on.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from restapi.connectors import Connector
 from restapi.tests import API_URI, BaseTests, FlaskClient
 
 
 class TestApp(BaseTests):
     def test_depends_on(self, client: FlaskClient) -> None:
-
         if Connector.check_availability("neo4j"):
-
             r = client.get(f"{API_URI}/tests/depends_on/neo4j")
             assert r.status_code == 200
 
             r = client.get(f"{API_URI}/tests/depends_on_not/neo4j")
             assert r.status_code == 404
 
         else:
-
             r = client.get(f"{API_URI}/tests/depends_on/neo4j")
             assert r.status_code == 404
 
             r = client.get(f"{API_URI}/tests/depends_on_not/neo4j")
             assert r.status_code == 200
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_encoding.py` & `rapydo_http-3.0/tests/base/test_endpoints_encoding.py`

 * *Files identical despite different names*

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_group_users.py` & `rapydo_http-3.0/tests/base/test_endpoints_group_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from restapi.services.authentication import Role
 from restapi.tests import API_URI, BaseTests, FlaskClient
 from restapi.utilities.logs import log
 
 
 class TestApp(BaseTests):
     def test_group_users(self, client: FlaskClient, faker: Faker) -> None:
-
         if not Env.get_bool("MAIN_LOGIN_ENABLE") or not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping group/users tests")
             return
 
         # Create group 1 with 1 Coordinator and 1 User
         group1_uuid, _ = self.create_group(client)
         _, user1_data = self.create_user(
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_inputs.py` & `rapydo_http-3.0/tests/base/test_endpoints_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 from restapi.connectors import Connector
 from restapi.env import Env
 from restapi.tests import API_URI, BaseTests, FlaskClient
 
 
 class TestApp(BaseTests):
     def test_inputs(self, client: FlaskClient) -> None:
-
         # This test verifies that buildData is always able to randomly create
         # valid inputs for endpoints with inputs defined by marshamallow schemas
         schema = self.get_dynamic_input_schema(client, "tests/inputs", {})
         # Expected number of fields
         assert len(schema) == 14
         for field in schema:
-
             # Always in the schema
             assert "key" in field
             assert "type" in field
             assert "label" in field
             assert "description" in field
             assert "required" in field
 
@@ -222,15 +220,14 @@
         assert r.status_code == 400
 
     @pytest.mark.skipif(
         not Connector.check_availability("neo4j"),
         reason="This test needs neo4j to be available",
     )
     def test_neo4j_inputs(self, client: FlaskClient) -> None:
-
         headers, _ = self.do_login(client, None, None)
         schema = self.get_dynamic_input_schema(client, "tests/neo4jinputs", headers)
         assert len(schema) == 1
 
         field = schema[0]
         assert field["key"] == "choice"
         # This is because the Neo4jChoice field is not completed for deserialization
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_login_ban.py` & `rapydo_http-3.0/tests/base/test_endpoints_login_ban.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 if not Env.get_bool("MAIN_LOGIN_ENABLE") or not Env.get_bool("AUTH_ENABLE"):
     log.warning("Skipping login ban tests")
 
 elif max_login_attempts == 0:
 
     class TestApp1(BaseTests):
         def test_01_login_ban_not_enabled(self, client: FlaskClient) -> None:
-
             uuid, data = self.create_user(client)
             # Login attempts are not registered, let's try to fail the login many times
             for _ in range(0, 10):
                 self.do_login(client, data["email"], "wrong", status_code=401)
 
             events = self.get_last_events(1)
             assert events[0].event == Events.failed_login.value
@@ -50,22 +49,20 @@
             r = client.post(f"{AUTH_URI}/login/unlock/token")
             assert r.status_code == 404
 
             # Goodbye temporary user
             self.delete_user(client, uuid)
 
 else:
-
     # This test executes a sleep(ban_duration)... this assert is to prevent to
     # block the tests due to a too-long ban duration
     assert ban_duration < 60
 
     class TestApp2(BaseTests):
         def verify_credentials_ban_notification(self) -> str:
-
             # Verify email sent to notify credentials block,
             # + extract and return the unlock url
             mail = self.read_mock_email()
             body = mail.get("body", "")
             project_tile = get_project_configuration(
                 "project.title", default="YourProject"
             )
@@ -81,15 +78,14 @@
             # assert "Your credentials will be automatically unlocked in" in body
 
             token = self.get_token_from_body(body)
             assert token is not None
             return token
 
         def test_01_failed_login_ban(self, client: FlaskClient) -> None:
-
             if not Env.get_bool("MAIN_LOGIN_ENABLE"):  # pragma: no cover
                 log.warning("Skipping admin/users tests")
                 return
 
             uuid, data = self.create_user(client)
 
             self.delete_mock_email()
@@ -155,15 +151,14 @@
             r = client.get(f"{AUTH_URI}/status", headers=headers)
             assert r.status_code == 200
 
             # Goodbye temporary user
             self.delete_user(client, uuid)
 
         def test_02_unlock_token(self, client: FlaskClient) -> None:
-
             if not Env.get_bool("MAIN_LOGIN_ENABLE"):  # pragma: no cover
                 log.warning("Skipping admin/users tests")
                 return
 
             uuid, data = self.create_user(client)
 
             self.delete_mock_email()
@@ -318,15 +313,14 @@
             c = self.get_content(r)
             assert c == "Invalid unlock token: this request is expired"
 
         def test_03_registration_and_login_ban(
             self, client: FlaskClient, faker: Faker
         ) -> None:
             if Env.get_bool("ALLOW_REGISTRATION"):
-
                 registration_data = {}
                 registration_data["email"] = faker.ascii_email()
                 registration_data["name"] = faker.first_name()
                 registration_data["surname"] = faker.last_name()
                 registration_data["password"] = faker.password(strong=True)
                 registration_data["password_confirm"] = registration_data["password"]
                 r = client.post(f"{AUTH_URI}/profile", json=registration_data)
@@ -422,15 +416,14 @@
                     json={"username": registration_data["email"]},
                 )
                 assert r.status_code == 200
 
         if Env.get_bool("AUTH_SECOND_FACTOR_AUTHENTICATION"):
 
             def test_04_totp_and_login_ban(self, client: FlaskClient) -> None:
-
                 uuid, data = self.create_user(client)
 
                 # Verify that login still works (TOTP will be automatically added)
                 headers, _ = self.do_login(client, data["email"], data["password"])
                 assert headers is not None
 
                 # Verify that TOTP is required
@@ -508,15 +501,14 @@
 
                 # Goodbye temporary user
                 self.delete_user(client, uuid)
 
         def test_05_no_notification_email_for_wrong_usernames(
             self, client: FlaskClient, faker: Faker
         ) -> None:
-
             if not Env.get_bool("MAIN_LOGIN_ENABLE"):  # pragma: no cover
                 log.warning("Skipping admin/users tests")
                 return
 
             uuid, data = self.create_user(client)
 
             self.delete_mock_email()
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_login_expiration.py` & `rapydo_http-3.0/tests/base/test_endpoints_login_expiration.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from restapi.env import Env
 from restapi.tests import API_URI, AUTH_URI, BaseTests, FlaskClient
 from restapi.utilities.logs import Events, log
 
 
 class TestApp2(BaseTests):
     def test_01_login_expiration(self, client: FlaskClient) -> None:
-
         if not Env.get_bool("MAIN_LOGIN_ENABLE") or not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping login expiration tests")
             return
 
         # Let's create a new user with an expiration time of N seconds
         expiration_time = 10
         expiration = datetime.now(pytz.utc) + timedelta(seconds=expiration_time)
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_login_profile_logout.py` & `rapydo_http-3.0/tests/base/test_endpoints_login_profile_logout.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,27 +170,27 @@
         r = client.get(f"{AUTH_URI}/status", headers=headers)
         assert r.status_code == 401
 
         headers = {"Authorization": f"Bearer '{faker.pystr()}"}
         r = client.get(f"{AUTH_URI}/status", headers=headers)
         assert r.status_code == 401
 
-        # Bearer realm is expected to be case sensitive
+        # Bearer realm is expected to be case insensitive
         token = self.get("auth_token")
         headers = {"Authorization": f"Bearer {token}"}
         r = client.get(f"{AUTH_URI}/status", headers=headers)
         assert r.status_code == 200
 
         headers = {"Authorization": f"bearer {token}"}
         r = client.get(f"{AUTH_URI}/status", headers=headers)
-        assert r.status_code == 401
+        assert r.status_code == 200
 
         headers = {"Authorization": f"BEARER {token}"}
         r = client.get(f"{AUTH_URI}/status", headers=headers)
-        assert r.status_code == 401
+        assert r.status_code == 200
 
         token = self.get("auth_token")
         headers = {"Authorization": f"Bear {token}"}
         r = client.get(f"{AUTH_URI}/status", headers=headers)
         assert r.status_code == 401
 
         USER = BaseAuthentication.default_user
@@ -209,15 +209,14 @@
         # }
         assert r.status_code == 400
 
         r = client.get(f"{AUTH_URI}/status", headers=headers)
         assert r.status_code == 401
 
     def test_03_change_profile(self, client: FlaskClient, faker: Faker) -> None:
-
         if not Env.get_bool("MAIN_LOGIN_ENABLE") or not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping change profile tests")
             return
 
         headers, _ = self.do_login(client, None, None)
 
         # update profile, no auth
@@ -415,15 +414,14 @@
             headers, _ = self.do_login(
                 client, data["email"], data["password"], test_failures=True
             )
             r = client.get(f"{AUTH_URI}/logout", headers=headers)
             assert r.status_code == 204
 
     def test_06_token_ip_validity(self, client: FlaskClient, faker: Faker) -> None:
-
         if Env.get_bool("MAIN_LOGIN_ENABLE") and Env.get_bool("AUTH_ENABLE"):
             if Env.get_int("AUTH_TOKEN_IP_GRACE_PERIOD") < 10:
                 headers, _ = self.do_login(client, None, None)
 
                 r = client.get(f"{AUTH_URI}/status", headers=headers)
                 assert r.status_code == 200
 
@@ -454,15 +452,14 @@
                     headers["X-Forwarded-For"] = faker.ipv4()  # type: ignore
                     r = client.get(f"{AUTH_URI}/status", headers=headers)
                     assert r.status_code == 401
 
     if Env.get_bool("AUTH_SECOND_FACTOR_AUTHENTICATION"):
 
         def test_07_totp_failures(self, client: FlaskClient, faker: Faker) -> None:
-
             uuid, data = self.create_user(client)
 
             username = data["email"]
             password = data["password"]
             new_password = faker.password(strong=True)
 
             invalid_totp = (
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_outputs.py` & `rapydo_http-3.0/tests/base/test_endpoints_outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from restapi.tests import API_URI, BaseTests, FlaskClient
 
 
 class TestApp(BaseTests):
     def test_outputs(self, client: FlaskClient) -> None:
-
         r = client.post(f"{API_URI}/tests/outputs/string")
         assert r.status_code == 200
         response = self.get_content(r)
         assert isinstance(response, str)
         assert response == "string"
 
         r = client.post(f"{API_URI}/tests/outputs/whatever")
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_pagination.py` & `rapydo_http-3.0/tests/base/test_endpoints_pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from restapi.tests import API_URI, BaseTests, FlaskClient
 
 # from restapi.utilities.logs import log
 
 
 class TestApp(BaseTests):
     def test_GET_specs(self, client: FlaskClient) -> None:
-
         r = client.get(f"{API_URI}/tests/pagination")
         assert r.status_code == 200
         content = self.get_content(r)
         assert isinstance(content, list)
         assert len(content) == 20
         assert content[0] == 1
         assert content[19] == 20
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_parameters_injection.py` & `rapydo_http-3.0/tests/base/test_endpoints_parameters_injection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from restapi.env import Env
 from restapi.services.authentication import BaseAuthentication
 from restapi.tests import API_URI, BaseTests, FlaskClient
 
 
 class TestApp(BaseTests):
     def test_parameter_injection(self, client: FlaskClient) -> None:
-
         if Env.get_bool("AUTH_ENABLE"):
             headers, _ = self.do_login(client, None, None)
             r = client.get(f"{API_URI}/tests/inject/myparam", headers=headers)
             assert r.status_code == 200
 
             response = self.get_content(r)
             assert isinstance(response, list)
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_password_reset.py` & `rapydo_http-3.0/tests/base/test_endpoints_password_reset.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from restapi.env import Env
 from restapi.tests import AUTH_URI, BaseAuthentication, BaseTests, FlaskClient
 from restapi.utilities.logs import Events, log
 
 
 class TestApp(BaseTests):
     def test_password_reset(self, client: FlaskClient, faker: Faker) -> None:
-
         if not Env.get_bool("ALLOW_PASSWORD_RESET") or not Env.get_bool("AUTH_ENABLE"):
             log.warning("Password reset is disabled, skipping tests")
             return
 
         project_tile = get_project_configuration("project.title", default="YourProject")
         proto = "https" if PRODUCTION else "http"
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_registration_and_activation.py` & `rapydo_http-3.0/tests/base/test_endpoints_registration_and_activation.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from restapi.env import Env
 from restapi.tests import API_URI, AUTH_URI, BaseAuthentication, BaseTests, FlaskClient
 from restapi.utilities.logs import OBSCURE_VALUE, Events, log
 
 
 class TestApp(BaseTests):
     def test_registration(self, client: FlaskClient, faker: Faker) -> None:
-
         if not Env.get_bool("ALLOW_REGISTRATION") or not Env.get_bool("AUTH_ENABLE"):
             log.warning("User registration is disabled, skipping tests")
             return
 
         project_tile = get_project_configuration("project.title", default="YourProject")
         proto = "https" if PRODUCTION else "http"
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_send_mail.py` & `rapydo_http-3.0/tests/base/test_endpoints_send_mail.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import json
-from typing import Any, Dict
+from typing import Any
 
 import pytest
 from faker import Faker
 
 from restapi.connectors import Connector
 from restapi.env import Env
 from restapi.tests import API_URI, BaseTests, FlaskClient
@@ -11,30 +10,29 @@
 
 @pytest.mark.skipif(
     not Connector.check_availability("smtp") or not Env.get_bool("AUTH_ENABLE"),
     reason="This test needs smtp and auth to be available",
 )
 class TestApp(BaseTests):
     def test_sendmail(self, client: FlaskClient, faker: Faker) -> None:
-
         headers, _ = self.do_login(client, None, None)
 
         r = client.get(f"{API_URI}/admin/mail", headers=headers)
         assert r.status_code == 405
 
         r = client.put(f"{API_URI}/admin/mail", headers=headers)
         assert r.status_code == 405
 
         r = client.patch(f"{API_URI}/admin/mail", headers=headers)
         assert r.status_code == 405
 
         r = client.delete(f"{API_URI}/admin/mail", headers=headers)
         assert r.status_code == 405
 
-        data: Dict[str, Any] = {"dry_run": False}
+        data: dict[str, Any] = {"dry_run": False}
         r = client.post(f"{API_URI}/admin/mail", json=data, headers=headers)
         assert r.status_code == 400
 
         data["subject"] = faker.pystr()
         r = client.post(f"{API_URI}/admin/mail", json=data, headers=headers)
         assert r.status_code == 400
 
@@ -127,9 +125,11 @@
         email_headers = mail.get("headers", "")
         assert body is not None
         assert email_headers is not None
         # Subject: is a key in the MIMEText
         assert f"Subject: {data['subject']}" in email_headers
         ccs = mail.get("cc", [])
         assert ccs[0] == data["to"]
-        assert ccs[1] == data["cc"].split(",")
-        assert ccs[2] == data["bcc"].split(",")
+        assert ccs[1] == data["cc"].split(",")[0]
+        assert ccs[2] == data["cc"].split(",")[1]
+        assert ccs[3] == data["bcc"].split(",")[0]
+        assert ccs[4] == data["bcc"].split(",")[1]
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_specs.py` & `rapydo_http-3.0/tests/base/test_endpoints_specs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from restapi.env import Env
 from restapi.tests import API_URI, BaseTests, FlaskClient
 
 
 class TestApp(BaseTests):
     def test_GET_specs(self, client: FlaskClient) -> None:
-
         r = client.get(f"{API_URI}/specs")
         assert r.status_code == 200
         content = self.get_content(r)
         assert isinstance(content, dict)
         assert "host" in content
         assert "info" in content
         assert "swagger" in content
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_status.py` & `rapydo_http-3.0/tests/base/test_endpoints_status.py`

 * *Files identical despite different names*

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_tokens.py` & `rapydo_http-3.0/tests/base/test_endpoints_tokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from restapi.env import Env
 from restapi.tests import API_URI, AUTH_URI, BaseTests, FlaskClient
 from restapi.utilities.logs import Events, log
 
 
 class TestApp(BaseTests):
     def test_tokens(self, client: FlaskClient, faker: Faker) -> None:
-
         if not Env.get_bool("AUTH_ENABLE"):
             log.warning("Skipping tokens tests")
             return
 
         last_token = None
         last_tokens_header = None
         token_id = None
@@ -27,15 +26,14 @@
         content = self.get_content(r)
         assert isinstance(content, list)
 
         # Probably due to password expiration:
         # change password invalidated tokens created before
         # => create tokens again
         if len(content) < 3:  # pragma: no cover
-
             for _ in range(3):
                 header, token = self.do_login(client, None, None)
                 last_tokens_header = header
                 last_token = token
 
             # TEST GET ALL TOKENS
             r = client.get(f"{AUTH_URI}/tokens", headers=last_tokens_header)
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_upload_download.py` & `rapydo_http-3.0/tests/base/test_endpoints_upload_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import io
 import os
 import warnings
-from typing import Dict
 
 from faker import Faker
 
 from restapi.config import DATA_PATH, PRODUCTION, get_backend_url
 from restapi.tests import API_URI, SERVER_URI, BaseTests, FlaskClient
 
 
-def get_location_header(headers: Dict[str, str], expected: str) -> str:
+def get_location_header(headers: dict[str, str], expected: str) -> str:
     assert "Location" in headers
     location = headers["Location"]
 
     if PRODUCTION:
         assert location.startswith("https://")
 
     host = get_backend_url()
@@ -23,19 +22,17 @@
     return location
 
 
 class TestUploadAndDownload(BaseTests):
     def test_simple_upload_and_download(
         self, client: FlaskClient, faker: Faker
     ) -> None:
-
         warnings.filterwarnings(
             "ignore", message="unclosed file <_io.BufferedReader name="
         )
-
         self.fcontent = faker.paragraph()
         self.save("fcontent", self.fcontent)
         # as defined in test_upload.py for normal uploads
         upload_folder = "fixsubfolder"
 
         self.fname = f"{faker.pystr()}.notallowed"
 
@@ -141,15 +138,14 @@
             query_string={"stream": True},
         )
         assert r.status_code == 404
 
     def test_chunked_upload_and_download(
         self, client: FlaskClient, faker: Faker
     ) -> None:
-
         warnings.filterwarnings(
             "ignore", message="unclosed file <_io.BufferedReader name="
         )
 
         self.fname = self.get("fname")
         self.fcontent = self.get("fcontent")
```

### Comparing `rapydo_http-2.4/tests/base/test_endpoints_users_custom_fields.py` & `rapydo_http-3.0/tests/base/test_endpoints_users_custom_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     @pytest.mark.skipif(
         not Env.get_bool("AUTH_ENABLE")
         or not Env.get_bool("MAIN_LOGIN_ENABLE")
         or not Env.get_bool("ALLOW_REGISTRATION"),
         reason="This test needs authentication and registration to be available",
     )
     def test_users_custom_fields(self, client: FlaskClient) -> None:
-
         output_fields = mem.customizer.get_custom_output_fields(None)
 
         profile_inputs = mem.customizer.get_custom_input_fields(
             request=None, scope=mem.customizer.PROFILE
         )
         registration_inputs = mem.customizer.get_custom_input_fields(
             request=None, scope=mem.customizer.REGISTRATION
```

### Comparing `rapydo_http-2.4/tests/base/test_module_authentication.py` & `rapydo_http-3.0/tests/base/test_module_authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from datetime import datetime, timedelta
-from typing import List, Optional
+from typing import Optional
 
 import pyotp
 import pytest
 import pytz
 from faker import Faker
 
 from restapi.connectors import Connector
@@ -45,15 +45,14 @@
 
 @pytest.mark.skipif(
     not Connector.check_availability("authentication"),
     reason="This test needs authentication to be available",
 )
 class TestApp(BaseTests):
     def test_password_management(self, faker: Faker) -> None:
-
         # Ensure name and surname longer than 3
         name = self.get_first_name(faker)
         surname = self.get_last_name(faker)
         # Ensure an email not containing name and surname
         email = self.get_random_email(faker, name, surname)
 
         auth = Connector.get_authentication_instance()
@@ -211,29 +210,25 @@
             auth.get_password_hash("")
 
         with pytest.raises(Unauthorized, match=r"Invalid password"):
             # Hashing a None password!
             auth.get_password_hash(None)
 
         assert auth.verify_password(pwd1, hash_1)
-        with pytest.raises(TypeError):
-            # Hashing a None password
-            auth.verify_password(None, hash_1)  # type: ignore
-
-        assert not auth.verify_password(pwd1, None)  # type: ignore
 
-        assert not auth.verify_password(None, None)  # type: ignore
+        assert not auth.is_bcrypt_hashed("test")
+        test_hash = auth.get_password_hash(pwd1)
+        assert auth.is_bcrypt_hashed(test_hash)
 
     @staticmethod
     @pytest.mark.skipif(
         not Env.get_bool("AUTH_SECOND_FACTOR_AUTHENTICATION"),
         reason="This test needs 2FA to be available",
     )
     def test_totp_management() -> None:
-
         auth = Connector.get_authentication_instance()
 
         with pytest.raises(Unauthorized, match=r"Verification code is missing"):
             # NULL totp
             auth.verify_totp(None, None)
 
         user = auth.get_user(username=auth.default_user)
@@ -273,15 +268,14 @@
 
         with pytest.raises(Unauthorized, match=r"Verification code is not valid"):
             # Past totp
             auth.verify_totp(user, totp.at(now - t30s - t30s - t30s))
 
     @staticmethod
     def test_login_management(faker: Faker) -> None:
-
         auth = Connector.get_authentication_instance()
 
         if BaseAuthentication.default_user:
             logins = auth.get_logins(BaseAuthentication.default_user)
 
             assert isinstance(logins, list)
             assert len(logins) > 0
@@ -302,15 +296,14 @@
         assert len(logins) == 0
 
         logins = auth.get_logins(faker.pystr())
         assert isinstance(logins, list)
         assert len(logins) == 0
 
     def test_tokens_management(self, client: FlaskClient, faker: Faker) -> None:
-
         auth = Connector.get_authentication_instance()
 
         # Just to verify that the function works
         verify_token_is_not_valid(auth, faker.pystr())
         verify_token_is_not_valid(auth, faker.pystr(), auth.PWD_RESET)
         verify_token_is_not_valid(auth, faker.pystr(), auth.ACTIVATE_ACCOUNT)
 
@@ -391,33 +384,33 @@
                 break
         assert jti is not None
         assert user is not None
 
         assert auth.verify_token_validity(jti, user)
 
         # Verify token against a wrong user
-
+        group = auth.get_group(name=DEFAULT_GROUP_NAME)
         another_user = auth.create_user(
             {
                 "email": faker.ascii_email(),
                 "name": "Default",
                 "surname": "User",
                 "password": faker.password(strong=True),
                 "last_password_change": datetime.now(pytz.utc),
             },
             # It will be expanded with the default role
             roles=[],
+            group=group,
         )
         auth.save_user(another_user)
 
         assert not auth.verify_token_validity(jti, another_user)
 
     @staticmethod
     def test_users_groups_roles(faker: Faker) -> None:
-
         auth = Connector.get_authentication_instance()
 
         user = auth.get_user(username=BaseAuthentication.default_user)
         group = auth.get_group(name="Default")
         assert user is not None
 
         user = auth.get_user(user_id=user.uuid)
@@ -465,18 +458,22 @@
         assert user is not None
         group = auth.get_group(name="Default")
         assert group is not None
 
         assert not auth.delete_user(None)
         assert not auth.delete_group(None)
 
+        # Delete default user, default group and all users belonging to it
+        members = auth.get_group_members(group)
+        for u in members:
+            assert auth.delete_user(u)
         assert auth.delete_user(user)
         assert auth.delete_group(group)
 
-        # Verify that user/group are now deleted
+        # Verify that both user and group are now deleted
         assert auth.get_user(username=BaseAuthentication.default_user) is None
         assert auth.get_group(name="Default") is None
 
         # init_auth_db should restore missing default user and group.
         # But previous tests created additional users and groups, so that
         # the init auth db without force flags is not able to re-add
         # the missing and user and group
@@ -514,15 +511,15 @@
         # assert user.password != expected_pwd
         assert Role.ADMIN.value not in auth.get_roles_from_user(user)
         assert Role.USER.value in auth.get_roles_from_user(user)
 
         group = auth.get_group(name="Default")
         assert group.fullname == "Changed"
 
-        roles: List[RoleObj] = auth.get_roles()
+        roles: list[RoleObj] = auth.get_roles()
         assert isinstance(roles, list)
         assert len(roles) > 0
 
         # Pick one of the default roles and change the description
         role: RoleObj = roles[0]
         assert role is not None
         default_name = role.name
@@ -595,15 +592,14 @@
         assert Role.USER.value in auth.get_roles_from_user(user)
 
         group = auth.get_group(name="Default")
         assert group.fullname != "Changed"
 
     @staticmethod
     def test_authentication_abstract_methods(faker: Faker) -> None:
-
         # Super trick!
         # https://clamytoe.github.io/articles/2020/Mar/12/testing-abcs-with-abstract-methods-with-pytest
         abstractmethods = BaseAuthentication.__abstractmethods__
         BaseAuthentication.__abstractmethods__ = frozenset()
 
         auth = Connector.get_authentication_instance()
         user = auth.get_user(username=BaseAuthentication.default_user)
@@ -647,15 +643,16 @@
         assert auth.get_roles() is None
 
         assert auth.get_roles_from_user(user=user) is None
 
         assert auth.create_role(name=faker.pystr(), description=faker.pystr()) is None
         assert auth.save_role(role=role) is None
 
-        assert auth.create_user(userdata={}, roles=[faker.pystr()]) is None
+        group = auth.get_group(name=DEFAULT_GROUP_NAME)
+        assert auth.create_user(userdata={}, roles=[faker.pystr()], group=group) is None
 
         assert auth.link_roles(user=user, roles=[faker.pystr()]) is None
         assert auth.create_group(groupdata={}) is None
 
         assert auth.add_user_to_group(user=user, group=group) is None
 
         assert (
```

### Comparing `rapydo_http-2.4/tests/base/test_module_miscellanous.py` & `rapydo_http-3.0/tests/base/test_module_miscellanous.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import tempfile
 import time
-from datetime import timedelta
+from datetime import date, datetime, timedelta
+from decimal import Decimal
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Optional, Union
 
 import psutil
 import pytest
 from faker import Faker
 from marshmallow.exceptions import ValidationError
 
 from restapi.config import (
@@ -28,15 +29,15 @@
     RestApiException,
     ServerError,
     ServiceUnavailable,
     Unauthorized,
 )
 from restapi.models import Schema, fields
 from restapi.rest.definition import EndpointResource
-from restapi.rest.response import ResponseMaker
+from restapi.rest.response import ResponseMaker, jsonifier
 from restapi.services.uploader import Uploader
 from restapi.tests import BaseTests
 from restapi.utilities.configuration import load_yaml_file, mix
 from restapi.utilities.logs import handle_log_output, obfuscate_dict
 from restapi.utilities.meta import Meta
 from restapi.utilities.processes import (
     Timeout,
@@ -45,20 +46,18 @@
     stop_timeout,
     wait_socket,
 )
 from restapi.utilities.time import get_timedelta, seconds_to_human
 
 
 class TestApp(BaseTests):
-
     # #######################################
     # ####      Env
     #########################################
     def test_env(self, faker: Faker) -> None:
-
         assert not Env.to_bool(None)
         assert Env.to_bool(None, True)
         assert not Env.to_bool(False)
         assert Env.to_bool(True)
         assert not Env.to_bool(0)
         assert Env.to_bool(1)
         assert Env.to_bool(1 + faker.pyint())
@@ -189,19 +188,31 @@
         response = EndpointResource.response("", code=200)
         assert response[1] == 200  # type: ignore
         response = EndpointResource.response(None, code=200)
         assert response[1] == 204  # type: ignore
         response = EndpointResource.response(None, code=200, head_method=True)
         assert response[1] == 200  # type: ignore
 
+    def test_jsonifier(self) -> None:
+        assert jsonifier("x") == '"x"'
+        assert jsonifier("1") == '"1"'
+        assert jsonifier(1) == "1"
+        assert jsonifier(1.2) == "1.2"
+        assert jsonifier(Decimal("1.2")) == "1.2"
+        assert jsonifier(["x"]) == '["x"]'
+        assert jsonifier({"x"}) == '["x"]'
+        assert jsonifier(("x",)) == '["x"]'
+        assert jsonifier(Path("test")) == '"test"'
+        assert jsonifier(date(2023, 1, 21)) == '"2023-01-21"'
+        assert jsonifier(datetime(2023, 1, 21, 11, 34, 21)) == '"2023-01-21T11:34:21"'
+
     # #######################################
     # ####      Meta
     #########################################
     def test_meta(self) -> None:
-
         # This is a valid package containing other packages... but no task will be found
         tasks = Meta.get_celery_tasks("restapi.utilities")
         assert isinstance(tasks, list)
         assert len(tasks) == 0
 
         tasks = Meta.get_celery_tasks("this-should-not-exist")
         assert isinstance(tasks, list)
@@ -241,33 +252,31 @@
         assert isinstance(models, dict)
         assert len(models) == 0
 
     # #######################################
     # ####      Templates
     #########################################
     def test_templates(self) -> None:
-
         h, p = get_html_template("this-should-not-exist", {})
         assert h is None
         assert p is None
 
     # #######################################
     # ####      Config Utilities
     #########################################
     def test_conf_utilities(self, faker: Faker) -> None:
-
         assert get_host_type("backend-server") == "backend-server"
+        assert get_host_type("docs-generation") == "docs-generation"
         assert get_host_type("celery") == "celery"
         assert get_host_type("celery-beat") == "celery-beat"
         assert get_host_type("flower") == "flower"
         assert get_host_type("whateverelse") == "celery"
         assert get_host_type(faker.pystr()) == "celery"
 
     def test_get_backend_url(self) -> None:
-
         # bypass the lru_cache decorator
         func = get_backend_url.__wrapped__
 
         if PRODUCTION:
             assert func() == f"https://{DOMAIN}"
         else:
             assert func() == f"http://{DOMAIN}:8080"
@@ -342,15 +351,14 @@
 
         if PRODUCTION:
             assert func() == f"https://{DOMAIN}/abc"
         else:
             assert func() == f"http://{DOMAIN}/abc:8080"
 
     def test_get_frontend_url(self) -> None:
-
         # bypass the lru_cache decorator
         func = get_frontend_url.__wrapped__
 
         if PRODUCTION:
             assert func() == f"https://{DOMAIN}"
         else:
             assert func() == f"http://{DOMAIN}"
@@ -419,15 +427,14 @@
         else:
             assert func() == f"http://{DOMAIN}/abc"
 
     # #######################################
     # ####      Timeouts
     #########################################
     def test_timeouts(self) -> None:
-
         start_timeout(1)
         with pytest.raises(Timeout, match=r"Operation timeout: interrupted"):
             # This operation will be interrupted because slower than timeout
             time.sleep(2)
 
         start_timeout(1)
         try:
@@ -437,15 +444,14 @@
         except Exception:  # pragma: no cover
             pytest.fail("Operation interrupted")
 
     # #######################################
     # ####      Logging
     #########################################
     def test_logging(self) -> None:
-
         log_output = handle_log_output(None)
         assert isinstance(log_output, dict)
         assert len(log_output) == 0
 
         log_output = handle_log_output(" ")
         assert isinstance(log_output, dict)
         assert len(log_output) == 0
@@ -467,21 +473,20 @@
         assert obfuscate_dict({"new_password": "y"}) == {"new_password": "****"}
         assert obfuscate_dict({"password_confirm": "y"}) == {"password_confirm": "****"}
 
     # #######################################
     # ####      YAML data load and mix
     #########################################
     def test_yaml(self) -> None:
-
-        data: Dict[str, Any] = {"a": 1}
+        data: dict[str, Any] = {"a": 1}
         assert mix({}, data) == data
 
-        data1: Dict[str, Any] = {"a": {"b": 1}, "c": 1}
-        data2: Dict[str, Any] = {"a": {"b": 2}}
-        expected: Dict[str, Any] = {"a": {"b": 2}, "c": 1}
+        data1: dict[str, Any] = {"a": {"b": 1}, "c": 1}
+        data2: dict[str, Any] = {"a": {"b": 2}}
+        expected: dict[str, Any] = {"a": {"b": 2}, "c": 1}
 
         assert mix(data1, data2) == expected
 
         data1 = {"a": {"b": 1}, "c": 1}
         data2 = {"a": None}
         # Cannot replace with an empty list
         assert mix(data1, data2) == data1
@@ -509,15 +514,14 @@
             load_yaml_file(Path(tmpf.name))
         tmpf.close()
 
     # #######################################
     # ####      Uploader
     #########################################
     def test_uploader(self) -> None:
-
         meta = Uploader.get_file_metadata("invalid_file")  # type: ignore
         assert isinstance(meta, dict)
         assert len(meta) == 0
 
         metadata_file_path = "confs/projects_defaults.yaml"
         meta = Uploader.get_file_metadata(metadata_file_path)  # type: ignore
         assert isinstance(meta, dict)
@@ -598,19 +602,24 @@
             Uploader.validate_upload_folder(Path("/uploads/\x00"))
 
         with pytest.raises(
             BadRequest, match=r"Invalid null byte in subfolder parameter"
         ):
             Uploader.validate_upload_folder(Path("/uploads/AA\x00BB"))
 
+        with pytest.raises(Forbidden, match=r"Invalid file path"):
+            Uploader.validate_upload_folder(Path("/etc/"))
+
+        with pytest.raises(Forbidden, match=r"Invalid file path"):
+            Uploader.validate_upload_folder(Path("../../tmp/"))
+
     # #######################################
     # ####      Time
     #########################################
     def test_time(self, faker: Faker) -> None:
-
         every = faker.pyint()
 
         t = get_timedelta(every, "seconds")
         assert t is not None
         assert isinstance(t, timedelta)
         assert 86400 * t.days + t.seconds == every
         assert t.microseconds == 0
@@ -706,15 +715,14 @@
         assert seconds_to_human(22222222) == "257 days, 4 hours, 50 minutes, 22 seconds"
         assert seconds_to_human(63072000) == "730 days"
 
     # #######################################
     # ####      Exceptions
     #########################################
     def test_exceptions(self) -> None:
-
         with pytest.raises(RestApiException) as e:
             raise BadRequest("test")
         assert e.value.status_code == 400
 
         with pytest.raises(RestApiException) as e:
             raise Unauthorized("test")
         assert e.value.status_code == 401
@@ -1078,25 +1086,14 @@
         assert match_types(Optional[str], type(None))
         assert not match_types(Optional[str], 1)
         assert not match_types(Optional[str], [])
         assert not match_types(Optional[str], {})
         assert not match_types(Optional[str], ["test"])
         assert not match_types(Optional[str], {"test": 1})
 
-        assert not match_types(List[str], EndpointResource)
-        assert not match_types(List[str], "EndpointResource")
-        assert not match_types(List[str], None)
-        assert not match_types(List[str], 1)
-        assert match_types(List[str], [])
-        assert not match_types(List[str], {})
-        assert match_types(List[str], ["test"])
-        # list args are not verifed, so [1] is currently accepted as List[str]
-        assert match_types(List[str], [1])
-        assert not match_types(List[str], {"test": 1})
-
         assert match_types(Union[str, int], 1)
         assert match_types(Union[str, int], "1")
         assert not match_types(Union[str, int], [])
 
         assert match_types(bool, True)
         assert match_types(bool, False)
         assert not match_types(bool, 0)
@@ -1110,15 +1107,14 @@
         # before adding as specific case in match_types
         assert not match_types(not Union[str, int], [])
 
     # #######################################
     # ####      Processes
     #########################################
     def test_processes(self) -> None:
-
         assert not find_process("this-should-not-exist")
         assert find_process("restapi")
         assert find_process("dumb-init")
         # current process is not retrieved by find_process
         current_pid = os.getpid()
         process = psutil.Process(current_pid)
         assert not find_process(process.name())
```

### Comparing `rapydo_http-2.4/tests/base/test_xxx_unused_credentials_step2.py` & `rapydo_http-3.0/tests/base/test_xxx_unused_credentials_step2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 This will used credentials created at the beginning of the suite
 to verify that unused credentialas are banned
 """
+
 from faker import Faker
 
 from restapi.env import Env
 from restapi.tests import AUTH_URI, BaseTests, FlaskClient
 from restapi.utilities.logs import Events
 
 if Env.get_int("AUTH_DISABLE_UNUSED_CREDENTIALS_AFTER") > 0:
 
     class TestApp1(BaseTests):
         def test_test_unused_credentials(
             self, client: FlaskClient, faker: Faker
         ) -> None:
-
             assert BaseTests.unused_credentials is not None
             assert len(BaseTests.unused_credentials) == 3
 
             data = {
                 "username": BaseTests.unused_credentials[0],
                 "password": faker.password(strong=True),
             }
@@ -36,16 +36,15 @@
 
             # Login is blocked due to inactivity
             r = client.post(f"{AUTH_URI}/login", json=data)
             assert r.status_code == 403
             resp = self.get_content(r)
             assert resp == "Sorry, this account is blocked for inactivity"
 
-            # Also password reset and blocked... how to recover the account !?
-
+            # Also password reset is blocked... how to recover the account !?
             reset_data = {"reset_email": BaseTests.unused_credentials[0]}
             r = client.post(f"{AUTH_URI}/reset", json=reset_data)
             assert r.status_code == 403
             resp = self.get_content(r)
             assert resp == "Sorry, this account is blocked for inactivity"
 
             events = self.get_last_events(2)
```

### Comparing `rapydo_http-2.4/tests/base/test_zzz1_destroy.py` & `rapydo_http-3.0/tests/base/test_zzz1_destroy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This test is intended to be executed as second-last, just before the re-init test
 (this is why it is prefixed as zzz1)
 Beware: if env TEST_DESTROY_MODE == 1 this test will destroy your database, be careful
 """
+
 import os
 
 import pytest
 
 from restapi.connectors import Connector
 from restapi.exceptions import ServiceUnavailable
 from restapi.server import ServerModes, create_app
@@ -16,21 +17,20 @@
 # Only executed if tests are run with --destroy flag
 @pytest.mark.skipif(
     not Connector.check_availability("authentication")
     or os.getenv("TEST_DESTROY_MODE", "0") != "1",
     reason="This test needs authentication and TEST_DESTROY_MODE to be enabled",
 )
 def test_destroy() -> None:
-
     auth = Connector.get_authentication_instance()
 
     user = auth.get_user(username=BaseAuthentication.default_user)
     assert user is not None
 
-    create_app(mode=ServerModes.DESTROY)
+    create_app(name="Flask Tests", mode=ServerModes.DESTROY, options={})
 
     if Connector.check_availability("sqlalchemy"):
         with pytest.raises(ServiceUnavailable):
             auth = Connector.get_authentication_instance()
             user = auth.get_user(username=BaseAuthentication.default_user)
     else:
         auth = Connector.get_authentication_instance()
```

### Comparing `rapydo_http-2.4/tests/base/test_zzz2_re-init.py` & `rapydo_http-3.0/tests/base/test_zzz2_re-init.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This test is intended to be executed as last, just after the destroy test
 (this is why it is prefixed as zzz2)
 Beware: if env TEST_DESTROY_MODE == 1 this test will destroy your database, be careful
 """
+
 import os
 
 import pytest
 
 from restapi.connectors import Connector
 from restapi.server import ServerModes, create_app
 from restapi.services.authentication import BaseAuthentication
@@ -21,18 +22,18 @@
 def test_init() -> None:
     if Connector.check_availability("sqlalchemy"):
         # Prevents errors like:
         # sqlalchemy.exc.ResourceClosedError: This Connection is closed
         Connector.disconnect_all()
 
     try:
-        create_app(mode=ServerModes.INIT)
+        create_app(name="Flask Tests", mode=ServerModes.INIT, options={})
         # This is only a rough retry to prevent random errors from sqlalchemy
     except Exception:  # pragma: no cover
-        create_app(mode=ServerModes.INIT)
+        create_app(name="Flask Tests", mode=ServerModes.INIT, options={})
 
     auth = Connector.get_authentication_instance()
     try:
         user = auth.get_user(username=BaseAuthentication.default_user)
     # SqlAlchemy sometimes can raise an:
     # AttributeError: 'NoneType' object has no attribute 'twophase'
     # due to the multiple app created... should be an issue specific of this test
```

