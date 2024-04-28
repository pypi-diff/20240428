# Comparing `tmp/fractal_toolkit-4.1.3.tar.gz` & `tmp/fractal_toolkit-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_toolkit-4.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fractal_toolkit-5.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fractal_toolkit-4.1.3.tar` & `fractal_toolkit-5.0.0.tar`

### file list

```diff
@@ -1,144 +1,141 @@
--rw-r--r--   0        0        0      187 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/.coveragerc
--rw-r--r--   0        0        0      100 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/.flake8
--rw-r--r--   0        0        0      943 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/.gitignore
--rw-r--r--   0        0        0      161 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/.isort.cfg
--rw-r--r--   0        0        0     1964 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1062 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/LICENSE
--rw-r--r--   0        0        0     1563 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/Makefile
--rw-r--r--   0        0        0    15008 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/README.md
--rw-r--r--   0        0        0      780 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/align_version.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/examples/basic/app/adapters/__init__.py
--rw-r--r--   0        0        0      245 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/examples/basic/app/adapters/products.py
--rw-r--r--   0        0        0      701 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/examples/basic/app/context.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/examples/basic/app/domain/__init__.py
--rw-r--r--   0        0        0      317 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/examples/basic/app/domain/products.py
--rw-r--r--   0        0        0      204 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/examples/basic/app/main.py
--rw-r--r--   0        0        0      369 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/examples/basic/app/settings.py
--rw-r--r--   0        0        0      720 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/fractal/__init__.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/fractal/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/fractal/contrib/django/__init__.py
--rw-r--r--   0        0        0     1660 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/fractal/contrib/django/middleware.py
--rw-r--r--   0        0        0      778 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/fractal/contrib/django/projectors.py
--rw-r--r--   0        0        0       27 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/fractal/contrib/django/requirements.txt
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/fractal/contrib/fastapi/__init__.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/fractal/contrib/fastapi/exceptions/__init__.py
--rw-r--r--   0        0        0       95 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/fractal/contrib/fastapi/exceptions/error_message.py
--rw-r--r--   0        0        0     2297 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/fractal/contrib/fastapi/install.py
--rw-r--r--   0        0        0       68 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/fractal/contrib/fastapi/requirements.txt
--rw-r--r--   0        0        0       48 2023-10-15 14:49:16.217165 fractal_toolkit-4.1.3/fractal/contrib/fastapi/routers/__init__.py
--rw-r--r--   0        0        0     9125 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/fastapi/routers/default.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/fastapi/routers/domain/__init__.py
--rw-r--r--   0        0        0      207 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/fastapi/routers/domain/models.py
--rw-r--r--   0        0        0     2948 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/fastapi/routers/tokens.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/fastapi/utils/__init__.py
--rw-r--r--   0        0        0      298 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/fastapi/utils/json_encoder.py
--rw-r--r--   0        0        0      216 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/gcp/cloudstorage/__init__.py
--rw-r--r--   0        0        0     2450 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/gcp/cloudstorage/repositories.py
--rw-r--r--   0        0        0       21 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/gcp/cloudstorage/requirements.txt
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0      328 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/gcp/firestore/event_store.py
--rw-r--r--   0        0        0       38 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/gcp/firestore/requirements.txt
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/gcp/pubsub/__init__.py
--rw-r--r--   0        0        0     3056 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/gcp/pubsub/event_bus.py
--rw-r--r--   0        0        0     2466 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/gcp/pubsub/projectors.py
--rw-r--r--   0        0        0       20 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/gcp/pubsub/requirements.txt
--rw-r--r--   0        0        0     1192 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/kafka/README.md
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/kafka/__init__.py
--rw-r--r--   0        0        0     1293 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/kafka/docker-compose.yml
--rw-r--r--   0        0        0     2233 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/kafka/event_bus.py
--rw-r--r--   0        0        0     1670 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/kafka/projectors.py
--rw-r--r--   0        0        0       13 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/kafka/requirements.txt
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/rabbitmq/__init__.py
--rw-r--r--   0        0        0     3176 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/rabbitmq/event_bus.py
--rw-r--r--   0        0        0     2011 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/rabbitmq/projectors.py
--rw-r--r--   0        0        0        5 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/rabbitmq/requirements.txt
--rw-r--r--   0        0        0      603 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/contrib/rabbitmq/utils.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/__init__.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/command_bus/__init__.py
--rw-r--r--   0        0        0       71 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/command_bus/command.py
--rw-r--r--   0        0        0     1077 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/command_bus/command_bus.py
--rw-r--r--   0        0        0      376 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/command_bus/command_handler.py
--rw-r--r--   0        0        0      613 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/command_bus/commands.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/__init__.py
--rw-r--r--   0        0        0      982 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/event.py
--rw-r--r--   0        0        0       52 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/event_bus.py
--rw-r--r--   0        0        0      297 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/event_projector.py
--rw-r--r--   0        0        0      907 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/event_publisher.py
--rw-r--r--   0        0        0     6447 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/event_store.py
--rw-r--r--   0        0        0      303 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/event_stream.py
--rw-r--r--   0        0        0      289 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/message.py
--rw-r--r--   0        0        0      397 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/models.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/projectors/__init__.py
--rw-r--r--   0        0        0      985 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/projectors/command_bus_projector.py
--rw-r--r--   0        0        0      588 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/projectors/event_store_projector.py
--rw-r--r--   0        0        0      769 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/projectors/print_projector.py
--rw-r--r--   0        0        0     1713 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/event_sourcing/repositories.py
--rw-r--r--   0        0        0      968 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/process/__init__.py
--rw-r--r--   0        0        0      195 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/process/action.py
--rw-r--r--   0        0        0     3752 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/process/actions/__init__.py
--rw-r--r--   0        0        0     1671 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/process/actions/control_flow.py
--rw-r--r--   0        0        0      473 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/process/process.py
--rw-r--r--   0        0        0      613 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/process/process_scope.py
--rw-r--r--   0        0        0      225 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/services/__init__.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/utils/__init__.py
--rw-r--r--   0        0        0     9665 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/utils/application_context.py
--rw-r--r--   0        0        0      411 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/utils/fractal.py
--rw-r--r--   0        0        0      636 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/utils/json_encoder.py
--rw-r--r--   0        0        0      447 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/utils/loggers.py
--rw-r--r--   0        0        0     1296 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/utils/settings.py
--rw-r--r--   0        0        0     1414 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/utils/string.py
--rw-r--r--   0        0        0      144 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/core/utils/subclasses.py
--rw-r--r--   0        0        0       77 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/fractal/py.typed
--rw-r--r--   0        0        0     1688 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/pyproject.toml
--rw-r--r--   0        0        0       69 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/setup.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/__init__.py
--rw-r--r--   0        0        0       45 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/contrib/fastapi/__init__.py
--rw-r--r--   0        0        0     2158 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/contrib/fastapi/test_routers.py
--rw-r--r--   0        0        0      451 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/contrib/fastapi/test_tokens.py
--rw-r--r--   0        0        0      392 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/contrib/fastapi/test_utils.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/__init__.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/command_bus/__init__.py
--rw-r--r--   0        0        0      844 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/command_bus/test_command_bus.py
--rw-r--r--   0        0        0      113 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/command_bus/test_command_handler.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/event_sourcing/__init__.py
--rw-r--r--   0        0        0      376 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/event_sourcing/test_event_publisher.py
--rw-r--r--   0        0        0     1675 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/event_sourcing/test_event_store.py
--rw-r--r--   0        0        0      294 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/event_sourcing/test_projectors.py
--rw-r--r--   0        0        0     1529 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/event_sourcing/test_repositories.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/services/__init__.py
--rw-r--r--   0        0        0      237 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/services/test_service.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/utils/__init__.py
--rw-r--r--   0        0        0     1638 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/utils/test_application_context.py
--rw-r--r--   0        0        0      850 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/utils/test_json_encoder.py
--rw-r--r--   0        0        0      542 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/utils/test_settings.py
--rw-r--r--   0        0        0      507 2023-10-15 14:49:16.221165 fractal_toolkit-4.1.3/tests/core/utils/test_string.py
--rw-r--r--   0        0        0      103 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      420 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/django/__init__.py
--rw-r--r--   0        0        0     2163 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/fastapi.py
--rw-r--r--   0        0        0       67 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0        0 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/mongo/__init__.py
--rw-r--r--   0        0        0       68 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/roles/__init__.py
--rw-r--r--   0        0        0      619 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/roles/services.py
--rw-r--r--   0        0        0       77 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     7365 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/sqlalchemy/repositories.py
--rw-r--r--   0        0        0      203 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/tokens/__init__.py
--rw-r--r--   0        0        0      485 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/tokens/fractal.py
--rw-r--r--   0        0        0      195 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/tokens/services.py
--rw-r--r--   0        0        0     1388 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/contrib/tokens/utils.py
--rw-r--r--   0        0        0      363 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/core/__init__.py
--rw-r--r--   0        0        0     1048 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/core/command_bus.py
--rw-r--r--   0        0        0     3938 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/core/event_sourcing.py
--rw-r--r--   0        0        0     1230 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/core/fractal.py
--rw-r--r--   0        0        0     1513 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/core/repositories.py
--rw-r--r--   0        0        0      457 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/core/services.py
--rw-r--r--   0        0        0     1781 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tests/fixtures/core/utils.py
--rw-r--r--   0        0        0      645 2023-10-15 14:49:16.225165 fractal_toolkit-4.1.3/tox.ini
--rw-r--r--   0        0        0    15968 1970-01-01 00:00:00.000000 fractal_toolkit-4.1.3/PKG-INFO
+-rw-r--r--   0        0        0      187 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/.coveragerc
+-rw-r--r--   0        0        0      100 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/.flake8
+-rw-r--r--   0        0        0      969 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/.gitignore
+-rw-r--r--   0        0        0      161 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/.isort.cfg
+-rw-r--r--   0        0        0     1964 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1062 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/LICENSE
+-rw-r--r--   0        0        0     1540 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/Makefile
+-rw-r--r--   0        0        0    15008 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/README.md
+-rw-r--r--   0        0        0      780 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/align_version.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/examples/basic/app/adapters/__init__.py
+-rw-r--r--   0        0        0      245 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/examples/basic/app/adapters/products.py
+-rw-r--r--   0        0        0      701 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/examples/basic/app/context.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/examples/basic/app/domain/__init__.py
+-rw-r--r--   0        0        0      317 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/examples/basic/app/domain/products.py
+-rw-r--r--   0        0        0      204 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/examples/basic/app/main.py
+-rw-r--r--   0        0        0      369 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/examples/basic/app/settings.py
+-rw-r--r--   0        0        0      720 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/django/__init__.py
+-rw-r--r--   0        0        0     1660 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/django/middleware.py
+-rw-r--r--   0        0        0      778 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/django/projectors.py
+-rw-r--r--   0        0        0       27 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/django/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/fastapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/fastapi/exceptions/__init__.py
+-rw-r--r--   0        0        0       95 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/fastapi/exceptions/error_message.py
+-rw-r--r--   0        0        0     2536 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/fastapi/install.py
+-rw-r--r--   0        0        0       68 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/fastapi/requirements.txt
+-rw-r--r--   0        0        0       48 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/fastapi/routers/__init__.py
+-rw-r--r--   0        0        0     9165 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/fastapi/routers/default.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/fastapi/routers/domain/__init__.py
+-rw-r--r--   0        0        0      207 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/fastapi/routers/domain/models.py
+-rw-r--r--   0        0        0     2949 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/fastapi/routers/tokens.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/fastapi/utils/__init__.py
+-rw-r--r--   0        0        0      298 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/fastapi/utils/json_encoder.py
+-rw-r--r--   0        0        0      216 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0      328 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/gcp/firestore/event_store.py
+-rw-r--r--   0        0        0       38 2024-04-28 07:55:01.117323 fractal_toolkit-5.0.0/fractal/contrib/gcp/firestore/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/gcp/pubsub/__init__.py
+-rw-r--r--   0        0        0     3056 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/gcp/pubsub/event_bus.py
+-rw-r--r--   0        0        0     2466 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/gcp/pubsub/projectors.py
+-rw-r--r--   0        0        0       20 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/gcp/pubsub/requirements.txt
+-rw-r--r--   0        0        0     1192 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/kafka/README.md
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/kafka/__init__.py
+-rw-r--r--   0        0        0     1293 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/kafka/docker-compose.yml
+-rw-r--r--   0        0        0     2233 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/kafka/event_bus.py
+-rw-r--r--   0        0        0     1670 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/kafka/projectors.py
+-rw-r--r--   0        0        0       13 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/kafka/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     3176 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/rabbitmq/event_bus.py
+-rw-r--r--   0        0        0     2011 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/rabbitmq/projectors.py
+-rw-r--r--   0        0        0        5 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/rabbitmq/requirements.txt
+-rw-r--r--   0        0        0      603 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/contrib/rabbitmq/utils.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/command_bus/__init__.py
+-rw-r--r--   0        0        0       71 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/command_bus/command.py
+-rw-r--r--   0        0        0     1077 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/command_bus/command_bus.py
+-rw-r--r--   0        0        0      376 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/command_bus/command_handler.py
+-rw-r--r--   0        0        0      613 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/command_bus/commands.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/__init__.py
+-rw-r--r--   0        0        0      982 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/event.py
+-rw-r--r--   0        0        0       52 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/event_bus.py
+-rw-r--r--   0        0        0      297 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/event_projector.py
+-rw-r--r--   0        0        0      907 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/event_publisher.py
+-rw-r--r--   0        0        0     6447 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/event_store.py
+-rw-r--r--   0        0        0      303 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/event_stream.py
+-rw-r--r--   0        0        0      289 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/message.py
+-rw-r--r--   0        0        0      397 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/models.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/projectors/__init__.py
+-rw-r--r--   0        0        0      985 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/projectors/command_bus_projector.py
+-rw-r--r--   0        0        0      588 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/projectors/event_store_projector.py
+-rw-r--r--   0        0        0      769 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/projectors/print_projector.py
+-rw-r--r--   0        0        0     1713 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/event_sourcing/repositories.py
+-rw-r--r--   0        0        0      968 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/process/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/process/action.py
+-rw-r--r--   0        0        0     3752 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/process/actions/__init__.py
+-rw-r--r--   0        0        0     1671 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/process/actions/control_flow.py
+-rw-r--r--   0        0        0      473 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/process/process.py
+-rw-r--r--   0        0        0      613 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/process/process_scope.py
+-rw-r--r--   0        0        0      225 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/utils/__init__.py
+-rw-r--r--   0        0        0     9865 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/utils/application_context.py
+-rw-r--r--   0        0        0      411 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/utils/fractal.py
+-rw-r--r--   0        0        0      636 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/utils/json_encoder.py
+-rw-r--r--   0        0        0      447 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/utils/loggers.py
+-rw-r--r--   0        0        0     1296 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/utils/settings.py
+-rw-r--r--   0        0        0     1414 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/utils/string.py
+-rw-r--r--   0        0        0      144 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/core/utils/subclasses.py
+-rw-r--r--   0        0        0       77 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/fractal/py.typed
+-rw-r--r--   0        0        0     1688 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/setup.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/tests/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/tests/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/tests/contrib/fastapi/__init__.py
+-rw-r--r--   0        0        0     2158 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/tests/contrib/fastapi/test_routers.py
+-rw-r--r--   0        0        0      451 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/tests/contrib/fastapi/test_tokens.py
+-rw-r--r--   0        0        0      392 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/tests/contrib/fastapi/test_utils.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.121323 fractal_toolkit-5.0.0/tests/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/command_bus/__init__.py
+-rw-r--r--   0        0        0      844 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/command_bus/test_command_bus.py
+-rw-r--r--   0        0        0      113 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/command_bus/test_command_handler.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/event_sourcing/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/event_sourcing/test_event_publisher.py
+-rw-r--r--   0        0        0     1675 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/event_sourcing/test_event_store.py
+-rw-r--r--   0        0        0      294 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/event_sourcing/test_projectors.py
+-rw-r--r--   0        0        0     1529 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/event_sourcing/test_repositories.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/services/__init__.py
+-rw-r--r--   0        0        0      237 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/services/test_service.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/utils/__init__.py
+-rw-r--r--   0        0        0     1638 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/utils/test_application_context.py
+-rw-r--r--   0        0        0      850 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/utils/test_json_encoder.py
+-rw-r--r--   0        0        0      542 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/utils/test_settings.py
+-rw-r--r--   0        0        0      507 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/core/utils/test_string.py
+-rw-r--r--   0        0        0      103 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      420 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2163 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/fastapi.py
+-rw-r--r--   0        0        0       67 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0       68 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/roles/__init__.py
+-rw-r--r--   0        0        0      619 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/roles/services.py
+-rw-r--r--   0        0        0       77 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     7365 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0      203 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/tokens/__init__.py
+-rw-r--r--   0        0        0      485 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/tokens/fractal.py
+-rw-r--r--   0        0        0      195 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/tokens/services.py
+-rw-r--r--   0        0        0     1388 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/contrib/tokens/utils.py
+-rw-r--r--   0        0        0      363 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/core/__init__.py
+-rw-r--r--   0        0        0     1048 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/core/command_bus.py
+-rw-r--r--   0        0        0     3938 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/core/event_sourcing.py
+-rw-r--r--   0        0        0     1230 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/core/fractal.py
+-rw-r--r--   0        0        0     1513 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/core/repositories.py
+-rw-r--r--   0        0        0      457 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/core/services.py
+-rw-r--r--   0        0        0     1781 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tests/fixtures/core/utils.py
+-rw-r--r--   0        0        0      693 2024-04-28 07:55:01.125323 fractal_toolkit-5.0.0/tox.ini
+-rw-r--r--   0        0        0    15968 1970-01-01 00:00:00.000000 fractal_toolkit-5.0.0/PKG-INFO
```

### Comparing `fractal_toolkit-4.1.3/.github/workflows/build.yml` & `fractal_toolkit-5.0.0/.github/workflows/build.yml`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     workflow_dispatch:
 
 jobs:
     build:
         runs-on: ubuntu-latest
         strategy:
             matrix:
-                python-version: [3.9]
+                python-version: ["3.8", "3.9", "3.10", "3.11"]
 
         env:
             USING_COVERAGE: "3.9"
 
         steps:
             - name: Checkout sources
               uses: actions/checkout@v2
@@ -31,11 +31,11 @@
                   make deps
 
             - name: Run tox
               run: |
                   make tox
 
             - name: Upload coverage to Codecov
-              uses: codecov/codecov-action@v1
+              uses: codecov/codecov-action@v3
               if: contains(env.USING_COVERAGE, matrix.python-version)
               with:
-                  fail_ci_if_error: true
+                  fail_ci_if_error: false
```

### Comparing `fractal_toolkit-4.1.3/.github/workflows/publish.yml` & `fractal_toolkit-5.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/.gitignore` & `fractal_toolkit-5.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/.pre-commit-config.yaml` & `fractal_toolkit-5.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/LICENSE` & `fractal_toolkit-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/Makefile` & `fractal_toolkit-5.0.0/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 
 coverage:  ## Run tests with coverage
 	rm .coverage ||:
 	rm coverage.xml ||:
 	pytest --cov fractal --cov-report=xml
 
 deps:  ## Install dependencies
-	python -m pip install --upgrade pip
-	python -m pip install autoflake black coverage django fastapi flake8 flit fractal-repositories fractal-roles fractal-specifications fractal-tokens httpx isort mccabe mypy pre-commit pylint pytest pytest-cov pytest-asyncio pytest-lazy-fixture python-dotenv python-jose requests 'sqlalchemy<2.0' tox tox-gh-actions
-	python -m pip install cryptography
+	python -m pip install -U pip
+	python -m pip install -U autoflake black coverage cryptography django fastapi flake8 flit fractal-repositories fractal-roles fractal-specifications fractal-tokens httpx isort mccabe mypy pre-commit pylint 'pytest<7' pytest-cov pytest-asyncio pytest-lazy-fixture python-dotenv python-jose requests 'sqlalchemy<2.0' tox tox-gh-actions
 
 lint:  ## Lint and static-check
 	pre-commit run --all-files
 
 publish:  ## Publish to PyPi
 	python -m flit publish
```

### Comparing `fractal_toolkit-4.1.3/README.md` & `fractal_toolkit-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/align_version.py` & `fractal_toolkit-5.0.0/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/examples/basic/app/context.py` & `fractal_toolkit-5.0.0/examples/basic/app/context.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/__init__.py` & `fractal_toolkit-5.0.0/fractal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Fractal is a scaffolding toolkit for building SOLID logic for your Python applications."""
 
-__version__ = "4.1.3"
+__version__ = "5.0.0"
 
 from abc import ABC
 
 from fractal.core.utils.application_context import ApplicationContext
 from fractal.core.utils.settings import Settings
```

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/django/middleware.py` & `fractal_toolkit-5.0.0/fractal/contrib/django/middleware.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/django/projectors.py` & `fractal_toolkit-5.0.0/fractal/contrib/django/projectors.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/fastapi/install.py` & `fractal_toolkit-5.0.0/fractal/contrib/fastapi/install.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,58 +18,65 @@
 
 
 def install_fastapi(settings: Settings):
     app = FastAPI(
         title=getattr(settings, "APP_NAME", "Fractal service"),
         version=getattr(settings, "APP_VERSION", "0.1.0"),
         root_path=getattr(settings, "OPENAPI_PREFIX_PATH", ""),
-        openapi_url="/openapi.json"
-        if str(getattr(settings, "APIDOCS_ENABLED", "true")).lower()
-        in ["1", "yes", "true"]
-        else None,
+        openapi_url=(
+            "/openapi.json"
+            if str(getattr(settings, "APIDOCS_ENABLED", "true")).lower()
+            in ["1", "yes", "true"]
+            else None
+        ),
     )
 
     app.add_middleware(
         CORSMiddleware,
         allow_origins=getattr(settings, "ALLOW_ORIGINS", "").split(","),
         allow_credentials=True,
         allow_methods=["*"],
         allow_headers=["*"],
     )
 
     if sentry:
         if sentry_dsn := getattr(settings, "SENTRY_DSN", ""):
-            sentry_sdk.init(dsn=sentry_dsn)
+            sentry_sdk.init(
+                dsn=sentry_dsn,
+                traces_sample_rate=getattr(settings, "SENTRY_TRACES_SAMPLE_RATE", 0.1),
+                send_default_pii=True,
+                enable_tracing=True,
+            )
 
     @app.exception_handler(DomainException)
     def unicorn_domain_exception_handler(request: Request, exc: DomainException):
         logger = logging.getLogger("app")
         if isinstance(exc.status_code, int) and 400 <= exc.status_code < 500:
             logger.warning(f"{exc.code} - {exc.message}")
         else:
             logger.error(f"{exc.code} - {exc.message}")
 
-        if sentry:
-            sentry_sdk.capture_exception(exc)
+        # if sentry:
+        #     sentry_sdk.capture_exception(exc)
 
         return JSONResponse(
             status_code=exc.status_code,
             content=ErrorMessage(
                 code=exc.code,
                 message=exc.message,
             ).dict(),
             headers=exc.headers,
         )
 
     @app.exception_handler(Exception)
     def unicorn_exception_handler(request: Request, exc: Exception):
         logging.error(exc)
 
-        if sentry:
-            sentry_sdk.capture_exception(exc)
+        # if sentry:
+        #     sentry_sdk.capture_exception(exc)
 
         return JSONResponse(
             status_code=500,
             content=ErrorMessage(
                 code=exc.__class__.__name__,
                 message=str(exc),
             ).dict(),
```

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/fastapi/routers/default.py` & `fractal_toolkit-5.0.0/fractal/contrib/fastapi/routers/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 
 def inject_default_routes(fractal: Fractal):
     router = APIRouter()
 
     @router.get(Routes.ROOT)
     def read_root():
         return {
-            "FastAPI": fractal.settings.APP_NAME
-            if fractal.settings and hasattr(fractal.settings, "APP_NAME")
-            else "Fractal Service",
+            "FastAPI": (
+                fractal.settings.APP_NAME
+                if fractal.settings and hasattr(fractal.settings, "APP_NAME")
+                else "Fractal Service"
+            ),
         }
 
     @router.get(Routes.INFO, responses={200: {"model": Info}})
     def info(
         payload: TokenPayload = Depends(get_payload(fractal)),
     ):
         adapters = list(fractal.context.adapters())
```

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/fastapi/routers/tokens.py` & `fractal_toolkit-5.0.0/fractal/contrib/fastapi/routers/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from fractal.core.services import Service
 
 oauth2_scheme = OAuth2PasswordBearer(tokenUrl="login")
 
 
 @dataclass
 class TokenPayload(Model, BaseTokenPayload):
-    ...
+    pass
 
 
 @dataclass
 class TokenPayloadRoles(Model, TokenPayloadRolesMixin, BaseTokenPayload):
     roles: Optional[List[Role]] = None
     account: str = ""
```

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/gcp/pubsub/event_bus.py` & `fractal_toolkit-5.0.0/fractal/contrib/gcp/pubsub/event_bus.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/gcp/pubsub/projectors.py` & `fractal_toolkit-5.0.0/fractal/contrib/gcp/pubsub/projectors.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/kafka/README.md` & `fractal_toolkit-5.0.0/fractal/contrib/kafka/README.md`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/kafka/docker-compose.yml` & `fractal_toolkit-5.0.0/fractal/contrib/kafka/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/kafka/event_bus.py` & `fractal_toolkit-5.0.0/fractal/contrib/kafka/event_bus.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/kafka/projectors.py` & `fractal_toolkit-5.0.0/fractal/contrib/kafka/projectors.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/rabbitmq/event_bus.py` & `fractal_toolkit-5.0.0/fractal/contrib/rabbitmq/event_bus.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/rabbitmq/projectors.py` & `fractal_toolkit-5.0.0/fractal/contrib/rabbitmq/projectors.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/contrib/rabbitmq/utils.py` & `fractal_toolkit-5.0.0/fractal/contrib/rabbitmq/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/command_bus/command_bus.py` & `fractal_toolkit-5.0.0/fractal/core/command_bus/command_bus.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/command_bus/commands.py` & `fractal_toolkit-5.0.0/fractal/core/command_bus/commands.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/event_sourcing/event.py` & `fractal_toolkit-5.0.0/fractal/core/event_sourcing/event.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/event_sourcing/event_publisher.py` & `fractal_toolkit-5.0.0/fractal/core/event_sourcing/event_publisher.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/event_sourcing/event_store.py` & `fractal_toolkit-5.0.0/fractal/core/event_sourcing/event_store.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/event_sourcing/projectors/command_bus_projector.py` & `fractal_toolkit-5.0.0/fractal/core/event_sourcing/projectors/command_bus_projector.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/event_sourcing/projectors/event_store_projector.py` & `fractal_toolkit-5.0.0/fractal/core/event_sourcing/projectors/event_store_projector.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/event_sourcing/projectors/print_projector.py` & `fractal_toolkit-5.0.0/fractal/core/event_sourcing/projectors/print_projector.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/event_sourcing/repositories.py` & `fractal_toolkit-5.0.0/fractal/core/event_sourcing/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/exceptions/__init__.py` & `fractal_toolkit-5.0.0/fractal/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/process/actions/__init__.py` & `fractal_toolkit-5.0.0/fractal/core/process/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/process/actions/control_flow.py` & `fractal_toolkit-5.0.0/fractal/core/process/actions/control_flow.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/process/process_scope.py` & `fractal_toolkit-5.0.0/fractal/core/process/process_scope.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/utils/application_context.py` & `fractal_toolkit-5.0.0/fractal/core/utils/application_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,31 +90,35 @@
         for service in self.services:
             yield service
 
     def load_internal_services(self):
         """Load services for internal use of the domain."""
         for name, service in self.registered_internal_services:
             _service = self.install_service(
-                service(self.settings)
-                if isinstance(service, FunctionType)
-                else service,
+                (
+                    service(self.settings)
+                    if isinstance(service, FunctionType)
+                    else service
+                ),
                 name=name,
             )
             setattr(self, name, _service())
 
     def load_repositories(self):
         """Load repositories for data access"""
         for name, repository in self.registered_repositories:
             setattr(
                 self,
                 name,
                 self.install_repository(
-                    repository(self.settings)
-                    if isinstance(repository, FunctionType)
-                    else repository,
+                    (
+                        repository(self.settings)
+                        if isinstance(repository, FunctionType)
+                        else repository
+                    ),
                     name=name,
                 ),
             )
         self.load_event_store()
 
     def load_event_store(self):
         if (
@@ -168,17 +172,19 @@
                 event_store_repository=self.event_store_repository,
             )
 
     def load_egress_services(self):
         """Load services to external interfaces that are initiated by this service (outbound)"""
         for name, service in self.registered_egress_services:
             _service = self.install_service(
-                service(self.settings)
-                if isinstance(service, FunctionType)
-                else service,
+                (
+                    service(self.settings)
+                    if isinstance(service, FunctionType)
+                    else service
+                ),
                 name=name,
             )
             setattr(self, name, _service())
 
     def load_event_publisher(self):
         from fractal.core.event_sourcing.event_publisher import EventPublisher
 
@@ -234,17 +240,19 @@
         for handler in self.registered_command_handlers:
             handler.install(self)
 
     def load_ingress_services(self):
         """Load services to external interfaces that are initiated by the external services (inbound)"""
         for name, service in self.registered_ingress_services:
             _service = self.install_service(
-                service(self.settings)
-                if isinstance(service, FunctionType)
-                else service,
+                (
+                    service(self.settings)
+                    if isinstance(service, FunctionType)
+                    else service
+                ),
                 name=name,
             )
             setattr(self, name, _service())
 
     def install_repository(self, repository, *, name=""):
         if not name:
             from fractal.core.utils.string import camel_to_snake
```

### Comparing `fractal_toolkit-4.1.3/fractal/core/utils/json_encoder.py` & `fractal_toolkit-5.0.0/fractal/core/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/utils/settings.py` & `fractal_toolkit-5.0.0/fractal/core/utils/settings.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/fractal/core/utils/string.py` & `fractal_toolkit-5.0.0/fractal/core/utils/string.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/pyproject.toml` & `fractal_toolkit-5.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-toolkit"
-version = "4.1.3"
+version = "5.0.0"
 description = "Fractal is a scaffolding toolkit for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `fractal_toolkit-4.1.3/tests/contrib/fastapi/test_routers.py` & `fractal_toolkit-5.0.0/tests/contrib/fastapi/test_routers.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/core/command_bus/test_command_bus.py` & `fractal_toolkit-5.0.0/tests/core/command_bus/test_command_bus.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/core/event_sourcing/test_event_store.py` & `fractal_toolkit-5.0.0/tests/core/event_sourcing/test_event_store.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/core/event_sourcing/test_repositories.py` & `fractal_toolkit-5.0.0/tests/core/event_sourcing/test_repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/core/utils/test_application_context.py` & `fractal_toolkit-5.0.0/tests/core/utils/test_application_context.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/core/utils/test_json_encoder.py` & `fractal_toolkit-5.0.0/tests/core/utils/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/core/utils/test_settings.py` & `fractal_toolkit-5.0.0/tests/core/utils/test_settings.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/fixtures/contrib/fastapi.py` & `fractal_toolkit-5.0.0/tests/fixtures/contrib/fastapi.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/fixtures/contrib/roles/services.py` & `fractal_toolkit-5.0.0/tests/fixtures/contrib/roles/services.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/fixtures/contrib/sqlalchemy/repositories.py` & `fractal_toolkit-5.0.0/tests/fixtures/contrib/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/fixtures/contrib/tokens/utils.py` & `fractal_toolkit-5.0.0/tests/fixtures/contrib/tokens/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/fixtures/core/command_bus.py` & `fractal_toolkit-5.0.0/tests/fixtures/core/command_bus.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/fixtures/core/event_sourcing.py` & `fractal_toolkit-5.0.0/tests/fixtures/core/event_sourcing.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/fixtures/core/fractal.py` & `fractal_toolkit-5.0.0/tests/fixtures/core/fractal.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/fixtures/core/repositories.py` & `fractal_toolkit-5.0.0/tests/fixtures/core/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tests/fixtures/core/utils.py` & `fractal_toolkit-5.0.0/tests/fixtures/core/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.1.3/tox.ini` & `fractal_toolkit-5.0.0/tox.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 [gh-actions]
 python =
+    3.8: py38
     3.9: py39
+    3.10: py310
+    3.11: py311
 
 [tox]
 isolated_build = True
 envlist = py38,py39,py310,py311
 
 [testenv]
 deps =
@@ -19,15 +22,15 @@
     fractal-specifications
     fractal-tokens
     httpx
     isort
     mccabe
     mypy
     pylint
-    pytest
+    pytest<7
     pytest-asyncio
     pytest-lazy-fixture
     python-jose
     requests
     sqlalchemy<2.0
 commands =
     black fractal
```

### Comparing `fractal_toolkit-4.1.3/PKG-INFO` & `fractal_toolkit-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-toolkit
-Version: 4.1.3
+Version: 5.0.0
 Summary: Fractal is a scaffolding toolkit for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

