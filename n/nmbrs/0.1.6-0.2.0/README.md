# Comparing `tmp/nmbrs-0.1.6.tar.gz` & `tmp/nmbrs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmbrs-0.1.6.tar", last modified: Sun Apr 21 18:19:30 2024, max compression
+gzip compressed data, was "nmbrs-0.2.0.tar", last modified: Sun Apr 28 18:06:29 2024, max compression
```

## Comparing `nmbrs-0.1.6.tar` & `nmbrs-0.2.0.tar`

### file list

```diff
@@ -1,108 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.573650 nmbrs-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-21 18:19:13.000000 nmbrs-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 18:19:13.000000 nmbrs-0.1.6/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-21 18:19:30.573650 nmbrs-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-21 18:19:13.000000 nmbrs-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-21 18:19:13.000000 nmbrs-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:19:30.573650 nmbrs-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-21 18:19:13.000000 nmbrs-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.553650 nmbrs-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.557650 nmbrs-0.1.6/src/nmbrs/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-21 18:19:28.000000 nmbrs-0.1.6/src/nmbrs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.557650 nmbrs-0.1.6/src/nmbrs/data_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17712 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/data_classes/company.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/data_classes/data_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/data_classes/debtor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16254 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/data_classes/employee.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/data_classes/general.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.561650 nmbrs-0.1.6/src/nmbrs/data_classes/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/data_classes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/data_classes/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.561650 nmbrs-0.1.6/src/nmbrs/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.561650 nmbrs-0.1.6/src/nmbrs/exceptions/nmbrs_exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.561650 nmbrs-0.1.6/src/nmbrs/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/company_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/debtor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14775 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/employee_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.561650 nmbrs-0.1.6/src/nmbrs/service/microservices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.565650 nmbrs-0.1.6/src/nmbrs/service/microservices/company/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/cost_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/hour_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/labout_aggreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/pension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/salary_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/salary_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/wage_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/wage_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/company/wage_tax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.565650 nmbrs-0.1.6/src/nmbrs/service/microservices/debtor/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/debtor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/debtor/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/debtor/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/debtor/title.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/debtor/webook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.573650 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/absence.py
--rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/child.py
--rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/days.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/employment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/hour_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/labour_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/lease_car.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/leave.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/levensloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/partner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/personal_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/salary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/spaarloon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/time_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/time_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/employee/wage_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/microservices/micro_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/service/sso_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.573650 nmbrs-0.1.6/src/nmbrs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/utils/find_empty_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/utils/nmbrs_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-21 18:19:13.000000 nmbrs-0.1.6/src/nmbrs/utils/return_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:19:30.573650 nmbrs-0.1.6/src/nmbrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-21 18:19:30.000000 nmbrs-0.1.6/src/nmbrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-21 18:19:30.000000 nmbrs-0.1.6/src/nmbrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:19:30.000000 nmbrs-0.1.6/src/nmbrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-21 18:19:30.000000 nmbrs-0.1.6/src/nmbrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 18:19:30.000000 nmbrs-0.1.6/src/nmbrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.209584 nmbrs-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-28 18:06:16.000000 nmbrs-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-28 18:06:16.000000 nmbrs-0.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-04-28 18:06:29.209584 nmbrs-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-28 18:06:16.000000 nmbrs-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-28 18:06:16.000000 nmbrs-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 18:06:29.209584 nmbrs-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-28 18:06:16.000000 nmbrs-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.193584 nmbrs-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.193584 nmbrs-0.2.0/src/nmbrs/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-28 18:06:27.000000 nmbrs-0.2.0/src/nmbrs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.197584 nmbrs-0.2.0/src/nmbrs/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/auth/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.197584 nmbrs-0.2.0/src/nmbrs/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17708 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/data_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/debtor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17450 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/employee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/general.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.197584 nmbrs-0.2.0/src/nmbrs/data_classes/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/data_classes/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.197584 nmbrs-0.2.0/src/nmbrs/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.197584 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.197584 nmbrs-0.2.0/src/nmbrs/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12663 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/company_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14957 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/debtor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13705 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/employee_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.201584 nmbrs-0.2.0/src/nmbrs/service/microservices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.201584 nmbrs-0.2.0/src/nmbrs/service/microservices/company/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/cost_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/hour_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/labout_aggreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/pension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/salary_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/salary_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_tax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.201584 nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/webook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.205584 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/absence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/employment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/hour_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/labour_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/lease_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/leave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/levensloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/personal_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/salary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/spaarloon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/time_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/time_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9525 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/employee/wage_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/microservices/micro_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/service/sso_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.209584 nmbrs-0.2.0/src/nmbrs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/utils/find_empty_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/utils/nmbrs_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-28 18:06:16.000000 nmbrs-0.2.0/src/nmbrs/utils/return_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:06:29.209584 nmbrs-0.2.0/src/nmbrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-04-28 18:06:29.000000 nmbrs-0.2.0/src/nmbrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-28 18:06:29.000000 nmbrs-0.2.0/src/nmbrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 18:06:29.000000 nmbrs-0.2.0/src/nmbrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-28 18:06:29.000000 nmbrs-0.2.0/src/nmbrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 18:06:29.000000 nmbrs-0.2.0/src/nmbrs.egg-info/top_level.txt
```

### Comparing `nmbrs-0.1.6/LICENSE` & `nmbrs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.6/PKG-INFO` & `nmbrs-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmbrs
-Version: 0.1.6
+Version: 0.2.0
 Summary: Python SDK for the Visma Nmbrs SOAP API.
 Author: Lars Kluijtmans
 Author-email: info@lk-software.com
 Maintainer: Lars Kluijtmans
 Maintainer-email: info@lk-software.com
 License: Lars Kluijtmans
 Project-URL: Homepage, https://github.com/LarsKluijtmans/nmbrs_api
@@ -189,54 +189,52 @@
 #### Username and Token
 
 ```python
 from nmbrs import SingleSingOnService
 
 sso_service = SingleSingOnService()
 
-sso_token = sso_service.sso_auth_with_token("__username__", "__token__")
+sso_token = sso_service.get_token_with_api_token("__username__", "__token__")
 
 print(sso_token)
 ```
 
 #### Username and Password
 
 ```python
 from nmbrs import SingleSingOnService
 
 sso_service = SingleSingOnService()
 
-
-sso_token = sso_service.sso_auth_with_password("__username__", "__token__")
+sso_token = sso_service.get_token_with_password("__username__", "__token__")
 
 print(sso_token)
 ```
 
 **Note:** this function will raise an exception if you have accounts in multiple Nmbrs environments. In this case use the following call where you specify the domain you want to log in to. 
 
 #### Username, password, and domain
 
 ```python
 from nmbrs import SingleSingOnService
 
 sso_service = SingleSingOnService()
 
-
-sso_token = sso_service.sso_auth_with_domain("__username__", "__password__", "__domain__")
+sso_token = sso_service.get_token_with_domain("__username__", "__password__", "__domain__")
 
 print(sso_token)
 ```
 
 ### SSO url:
 
 Using the token reverence from the aforementioned functions we can create an url that automatically refers the user to nmbrs.
 
 ```python
 from nmbrs import SingleSingOnService
 
 sso_service = SingleSingOnService()
 
-sso_token = sso_service.sso_auth_with_password("__username__", "__password__")
+sso_token = sso_service.get_token_with_password("__username__", "__password__")
 sso_url = sso_service.get_sso_url(sso_token, "__domain__")
 
 print(sso_url)
 ```
```

### Comparing `nmbrs-0.1.6/README.md` & `nmbrs-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -166,54 +166,52 @@
 #### Username and Token
 
 ```python
 from nmbrs import SingleSingOnService
 
 sso_service = SingleSingOnService()
 
-sso_token = sso_service.sso_auth_with_token("__username__", "__token__")
+sso_token = sso_service.get_token_with_api_token("__username__", "__token__")
 
 print(sso_token)
 ```
 
 #### Username and Password
 
 ```python
 from nmbrs import SingleSingOnService
 
 sso_service = SingleSingOnService()
 
-
-sso_token = sso_service.sso_auth_with_password("__username__", "__token__")
+sso_token = sso_service.get_token_with_password("__username__", "__token__")
 
 print(sso_token)
 ```
 
 **Note:** this function will raise an exception if you have accounts in multiple Nmbrs environments. In this case use the following call where you specify the domain you want to log in to. 
 
 #### Username, password, and domain
 
 ```python
 from nmbrs import SingleSingOnService
 
 sso_service = SingleSingOnService()
 
-
-sso_token = sso_service.sso_auth_with_domain("__username__", "__password__", "__domain__")
+sso_token = sso_service.get_token_with_domain("__username__", "__password__", "__domain__")
 
 print(sso_token)
 ```
 
 ### SSO url:
 
 Using the token reverence from the aforementioned functions we can create an url that automatically refers the user to nmbrs.
 
 ```python
 from nmbrs import SingleSingOnService
 
 sso_service = SingleSingOnService()
 
-sso_token = sso_service.sso_auth_with_password("__username__", "__password__")
+sso_token = sso_service.get_token_with_password("__username__", "__password__")
 sso_url = sso_service.get_sso_url(sso_token, "__domain__")
 
 print(sso_url)
 ```
```

### Comparing `nmbrs-0.1.6/setup.py` & `nmbrs-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.6/src/nmbrs/__version__.py` & `nmbrs-0.2.0/src/nmbrs/__version__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Versioning details."""
 
 __title__ = "nmbrs"
-__version__ = '0.1.6'
+__version__ = '0.2.0'
 __author__ = "Lars Kluijtmans"
 __author_email__ = "info@lk-software.com"
 __maintainer__ = "Lars Kluijtmans"
 __maintainer_email__ = "info@lk-software.com"
 __description__ = "Python SDK for the Visma Nmbrs SOAP API."
 __license__ = "Lars Kluijtmans"
```

### Comparing `nmbrs-0.1.6/src/nmbrs/data_classes/company.py` & `nmbrs-0.2.0/src/nmbrs/data_classes/company.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         self.id: int = data.get("ID")
         self.number: int = data.get("Number")
         self.year: int = data.get("Year")
         self.period_start: int = data.get("PeriodStart")
         self.period_end: int = data.get("PeriodEnd")
         self.description: int = data.get("Description")
         self.run_at: datetime = data.get("RunAt")
-        self.locked: datetime = data.get("IsLocked")
+        self.locked: bool = data.get("IsLocked")
 
 
 class SalaryTable(DataClass):
     """A class representing a salary table."""
 
     def __init__(self, company_id: int, data: dict) -> None:
         self.company_id = company_id
```

### Comparing `nmbrs-0.1.6/src/nmbrs/data_classes/data_class.py` & `nmbrs-0.2.0/src/nmbrs/data_classes/data_class.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.6/src/nmbrs/data_classes/debtor.py` & `nmbrs-0.2.0/src/nmbrs/data_classes/debtor.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from .utils.xml import parse_xml_to_dict
 
 
 class Domain(DataClass):
     """A class representing domain."""
 
     def __init__(self, data: dict) -> None:
-        self.domain: int = data.get("Domain")
-        self.sub_domain: int = data.get("SubDomain")
+        self.domain: str = data.get("Domain")
+        self.sub_domain: str = data.get("SubDomain")
 
 
 class AbsenceVerzuim(DataClass):
     """A class representing absence data."""
 
     def __init__(self, data: dict) -> None:
         self.debtor_id: int = data.get("DebtorID")
```

### Comparing `nmbrs-0.1.6/src/nmbrs/data_classes/employee.py` & `nmbrs-0.2.0/src/nmbrs/data_classes/employee.py`

 * *Files 4% similar despite different names*

```diff
@@ -221,51 +221,87 @@
     def __init__(self, employee_id: int, data: dict):
         self.employee_id = employee_id
         self.id: int = data.get("Id")
         self.code: str = data.get("Code")
         self.description: str = data.get("Description")
 
 
-class Department(DataClass):
+class DepartmentAll(DataClass):
     """A class representing a department."""
 
     def __init__(self, employee_id: int, data: dict):
         self.employee_id = employee_id
         self.id = data.get("Id")
         self.code = data.get("Code")
         self.description = data.get("Description")
         self.creation_date = data.get("CreationDate")
         self.start_period = data.get("StartPeriod")
         self.start_year = data.get("StartYear")
 
 
+class Department(DataClass):
+    """A class representing a department."""
+
+    def __init__(self, employee_id: int, data: dict):
+        self.employee_id = employee_id
+        self.id = data.get("Id")
+        self.code = data.get("Code")
+        self.description = data.get("Description")
+
+
 class Employment(DataClass):
     """A class representing an employment."""
 
     def __init__(self, employee_id: int, data: dict):
         self.employee_id = employee_id
         self.id: int = data.get("EmploymentId")
         self.creation_date: datetime = data.get("CreationDate")
         self.start_date: datetime = data.get("StartDate")
         self.end_date: datetime = data.get("EndDate")
         self.initial_start_date: datetime = data.get("InitialStartDate")
 
 
-class Function(DataClass):
+class FunctionAll(DataClass):
     """A class representing a functions."""
 
     def __init__(self, employee_id: int, data: dict):
         self.employee_id = employee_id
         self.record_id: int = data.get("RecordId")
         self.function_id: int = data.get("Function").get("Id")
         self.creation_date: datetime = data.get("CreationDate")
         self.start_period: datetime = data.get("StartPeriod")
         self.start_year: datetime = data.get("StartYear")
 
 
+class Function(DataClass):
+    """A class representing a functions."""
+
+    def __init__(self, employee_id: int, data: dict):
+        self.employee_id = employee_id
+        self.id: int = data.get("Id")
+        self.code: int = data.get("Code")
+        self.description: str = data.get("Description")
+
+
+class Manager(DataClass):
+    """A class representing a manager."""
+
+    def __init__(self, employee_id: int, data: dict):
+        self.employee_id = employee_id
+        self.number: int = data.get("Number")
+        self.first_name: str = data.get("FirstName")
+        self.name: str = data.get("Name")
+        self.department: str = data.get("Department")
+        self.function: str = data.get("Function")
+        self.phone_number: str = data.get("PhoneNumber")
+        self.mobile: str = data.get("Mobile")
+        self.fax: str = data.get("Fax")
+        self.email: str = data.get("Email")
+
+
 class LeaseCar(DataClass):
     """A class representing a lease car."""
 
     def __init__(self, employee_id: int, data: dict):
         self.employee_id = employee_id
         self.id: int = data.get("Id")
         self.brand: str = data.get("Brand")
```

### Comparing `nmbrs-0.1.6/src/nmbrs/data_classes/utils/xml.py` & `nmbrs-0.2.0/src/nmbrs/data_classes/utils/xml.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.6/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py` & `nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.6/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py` & `nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.6/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py` & `nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.6/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py` & `nmbrs-0.2.0/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.6/src/nmbrs/service/company_service.py` & `nmbrs-0.2.0/src/nmbrs/service/company_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     CompanyWageComponentService,
     CompanySvwService,
     CompanyWageCostService,
     CompanyWageModelService,
     CompanyWageTaxService,
 )
 from .service import Service
+from ..auth.token_manager import AuthManager
 from ..utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ..utils.return_list import return_list
 from ..data_classes.company import (
     Company,
     Period,
     ContactPerson,
     GuidConvertor,
@@ -34,78 +35,51 @@
     PayrollWorkflowTrack,
 )
 
 
 class CompanyService(Service):
     """A class representing Company Service for interacting with Nmbrs company-related functionalities."""
 
-    def __init__(self, sandbox: bool = True) -> None:
-        super().__init__(sandbox)
+    def __init__(self, auth_manager: AuthManager, sandbox: bool = True):
+        super().__init__(auth_manager, sandbox)
 
         # Initialize nmbrs client
         self.client = Client(f"{self.base_uri}{self.company_uri}")
 
         # Micro services
-        self.address = CompanyAddressService(self.client)
-        self.bank_account = CompanyBankAccountService(self.client)
-        self.cost_center = CompanyCostCenterService(self.client)
-        self.cost_unit = CompanyCostUnitService(self.client)
-        self.hour_model = CompanyHourModelService(self.client)
-        self.journal = CompanyJournalService(self.client)  # TO BE implemented
-        self.labour_agreement = CompanyLabourAgreementService(self.client)
-        self.pension = CompanyPensionService(self.client)
-        self.run = CompanyRunService(self.client)
-        self.salary_documents = CompanySalaryDocumentService(self.client)  # TO BE implemented
-        self.salary_table = CompanySalaryTableService(self.client)
-        self.svw = CompanySvwService(self.client)
-        self.wage_component = CompanyWageComponentService(self.client)
-        self.wage_cost = CompanyWageCostService(self.client)
-        self.wage_model = CompanyWageModelService(self.client)
-        self.wage_tax = CompanyWageTaxService(self.client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        """
-        Method to set the authentication.
-
-        Args:
-            auth_header (dict): A dictionary containing authentication details.
-        """
-        self.auth_header = auth_header
-
-        # Micro services
-        self.address.set_auth_header(auth_header)
-        self.bank_account.set_auth_header(auth_header)
-        self.cost_center.set_auth_header(auth_header)
-        self.cost_unit.set_auth_header(auth_header)
-        self.hour_model.set_auth_header(auth_header)
-        self.journal.set_auth_header(auth_header)
-        self.labour_agreement.set_auth_header(auth_header)
-        self.pension.set_auth_header(auth_header)
-        self.run.set_auth_header(auth_header)
-        self.salary_documents.set_auth_header(auth_header)
-        self.salary_table.set_auth_header(auth_header)
-        self.svw.set_auth_header(auth_header)
-        self.wage_component.set_auth_header(auth_header)
-        self.wage_cost.set_auth_header(auth_header)
-        self.wage_model.set_auth_header(auth_header)
-        self.wage_tax.set_auth_header(auth_header)
+        self.address = CompanyAddressService(self.auth_manager, self.client)
+        self.bank_account = CompanyBankAccountService(self.auth_manager, self.client)
+        self.cost_center = CompanyCostCenterService(self.auth_manager, self.client)
+        self.cost_unit = CompanyCostUnitService(self.auth_manager, self.client)
+        self.hour_model = CompanyHourModelService(self.auth_manager, self.client)
+        self.journal = CompanyJournalService(self.auth_manager, self.client)  # TO BE implemented
+        self.labour_agreement = CompanyLabourAgreementService(self.auth_manager, self.client)
+        self.pension = CompanyPensionService(self.auth_manager, self.client)
+        self.run = CompanyRunService(self.auth_manager, self.client)
+        self.salary_documents = CompanySalaryDocumentService(self.auth_manager, self.client)  # TO BE implemented
+        self.salary_table = CompanySalaryTableService(self.auth_manager, self.client)
+        self.svw = CompanySvwService(self.auth_manager, self.client)
+        self.wage_component = CompanyWageComponentService(self.auth_manager, self.client)
+        self.wage_cost = CompanyWageCostService(self.auth_manager, self.client)
+        self.wage_model = CompanyWageModelService(self.auth_manager, self.client)
+        self.wage_tax = CompanyWageTaxService(self.auth_manager, self.client)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:List_GetAll")
     def get_all(self) -> list[Company]:
         """
         Retrieve all companies.
 
         For more information, refer to the official documentation:
             [Soap call List_GetAll](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=List_GetAll)
 
         Returns:
             list[Company]: A list of Company objects.
         """
-        companies = self.client.service.List_GetAll(_soapheaders=self.auth_header)
+        companies = self.client.service.List_GetAll(_soapheaders=self.auth_manager.header)
         companies = [Company(company) for company in serialize_object(companies)]
         return companies
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:List_GetByDebtor")
     def get_by_debtor(self, debtor_id: int) -> list[Company]:
         """
@@ -116,15 +90,15 @@
 
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             list[Company]: A list of Company objects.
         """
-        companies = self.client.service.List_GetByDebtor(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        companies = self.client.service.List_GetByDebtor(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         companies = [Company(company) for company in serialize_object(companies)]
         return companies
 
     @nmbrs_exception_handler(resource="CompanyService:Company_GetCurrentByEmployeeId")
     def get_by_employee(self, employee_id: int) -> Company | None:
         """
         Get company by employee id.
@@ -134,15 +108,15 @@
 
         Args:
             employee_id (int): The ID of the employee.
 
         Returns:
             Company: A list of Company objects.
         """
-        company = self.client.service.Company_GetCurrentByEmployeeId(EmployeeId=employee_id, _soapheaders=self.auth_header)
+        company = self.client.service.Company_GetCurrentByEmployeeId(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
         if company is None:
             return None
         return Company(serialize_object(company))
 
     @nmbrs_exception_handler(resource="CompanyService:Company_GetCurrentPeriod")
     def get_current_period(self, company_id: int) -> Period | None:
         """
@@ -153,21 +127,21 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             Period: year, period and period type and the company.
         """
-        period = self.client.service.Company_GetCurrentPeriod(CompanyId=company_id, _soapheaders=self.auth_header)
+        period = self.client.service.Company_GetCurrentPeriod(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         if period is None:
             return None
         return Period(company_id=company_id, data=serialize_object(period))
 
     @nmbrs_exception_handler(resource="CompanyService:Company_Insert")
-    def insert(
+    def post(
         self, debtor_id: int, name: str, period_type: int, default_id: int, labour_agreement_group_id: str, pay_in_advance: bool
     ) -> int:
         """
         Insert a new company.
 
         This method inserts a new debtor with the provided details into the Nmbrs system.
 
@@ -188,15 +162,15 @@
         inserted = self.client.service.Company_Insert(
             DebtorId=debtor_id,
             CompanyName=name,
             PeriodType=period_type,
             DefaultCompanyId=default_id,
             LabourAgreementSettingsGroupGuid=labour_agreement_group_id,
             PayInAdvance=pay_in_advance,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return inserted
 
     @nmbrs_exception_handler(resource="CompanyService:ContactPerson_Get")
     def get_contact_person(self, company_id: int) -> ContactPerson:
         """
         Get contact person by company ID.
@@ -206,15 +180,15 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             ContactPerson: The contact person details.
         """
-        contact_person = self.client.service.ContactPerson_Get(CompanyId=company_id, _soapheaders=self.auth_header)
+        contact_person = self.client.service.ContactPerson_Get(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         return ContactPerson(company_id=company_id, data=serialize_object(contact_person))
 
     @nmbrs_exception_handler(resource="CompanyService:Converter_GetByCompany_IntToGuid")
     def get_converter_mappings(self, company_id: int, entity: str) -> GuidConvertor:
         """
         Get converter mappings for the given entity and company ID.
 
@@ -224,15 +198,17 @@
         Args:
             company_id (int): The ID of the company.
             entity (str): The entity type (e.g., Employee, Company, Debtor).
 
         Returns:
             GuidConvertor: The converter mappings response.
         """
-        guids = self.client.service.Converter_GetByCompany_IntToGuid(Entity=entity, CompanyId=company_id, _soapheaders=self.auth_header)
+        guids = self.client.service.Converter_GetByCompany_IntToGuid(
+            Entity=entity, CompanyId=company_id, _soapheaders=self.auth_manager.header
+        )
         return GuidConvertor(company_id=company_id, data=serialize_object(guids))
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:DefaultEmployeeTemplates_GetByCompany")
     def get_default_employee_templates(self, company_id: int) -> list[DefaultEmployeeTemplate]:
         """
         Get available default employee templates by company.
@@ -242,15 +218,17 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[Company]: A list of Company objects.
         """
-        employee_templates = self.client.service.DefaultEmployeeTemplates_GetByCompany(CompanyId=company_id, _soapheaders=self.auth_header)
+        employee_templates = self.client.service.DefaultEmployeeTemplates_GetByCompany(
+            CompanyId=company_id, _soapheaders=self.auth_manager.header
+        )
         employee_templates = [
             DefaultEmployeeTemplate(company_id=company_id, data=employee_template)
             for employee_template in serialize_object(employee_templates)
         ]
         return employee_templates
 
     @nmbrs_exception_handler(resource="CompanyService:FileExplorer_UploadFile")
@@ -273,15 +251,15 @@
         self.client.service.FileExplorer_UploadFile(
             **{
                 "CompanyId": company_id,
                 "StrDocumentName": document_name,
                 "StrDocumentSubFolder": document_sub_folder,
                 "Body": data,
             },
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
 
     @nmbrs_exception_handler(resource="CompanyService:Schedule_GetCurrent")
     def get_current_schedule(self, company_id: int) -> FulltimeSchedules:
         """
         Retrieve the current schedules for a company.
 
@@ -290,30 +268,32 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             FulltimeSchedules: A FulltimeSchedules object.
         """
-        response = self.client.service.Schedule_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
+        response = self.client.service.Schedule_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         return FulltimeSchedules(company_id=company_id, data=serialize_object(response))
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:PayrollWorkflow_Get")
-    def get_payroll_workflow(self, company_id: int, year: int, period: int) -> list[PayrollWorkflowTrack]:
+    def get_payroll_workflows(self, company_id: int, period: int, year: int) -> list[PayrollWorkflowTrack]:
         """
         Get the company's payroll workflow tracks and actions.
 
         For further details, see the official documentation:
             [PayrollWorkflow_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=PayrollWorkflow_Get)
 
         Args:
             company_id (int): The ID of the company.
-            year (int): The year.
             period (int): The period.
+            year (int): The year.
 
         Returns:
             List[PayrollWorkflowTrack]: A list of PayrollWorkflowTrack objects.
         """
-        responses = self.client.service.PayrollWorkflow_Get(CompanyId=company_id, Year=year, Period=period, _soapheaders=self.auth_header)
+        responses = self.client.service.PayrollWorkflow_Get(
+            CompanyId=company_id, Year=year, Period=period, _soapheaders=self.auth_manager.header
+        )
         responses = [PayrollWorkflowTrack(company_id=company_id, data=response) for response in serialize_object(responses)]
         return responses
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/debtor_service.py` & `nmbrs-0.2.0/src/nmbrs/service/debtor_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from datetime import datetime
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from .microservices.debtor import DebtorDepartmentService, DebtorFunctionService, DebtorTitleService, DebtorWebHooksService
 from .service import Service
+from ..auth.token_manager import AuthManager
 from ..utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ..utils.return_list import return_list
 from ..data_classes.debtor import (
     Debtor,
     AbsenceVerzuim,
     Address,
     BankAccount,
@@ -28,40 +29,25 @@
     """
     A class representing Debtor Service for interacting with Nmbrs debtor-related functionalities.
 
     Not implemented calls:
         1 [Converter_GetDebtors_IntToGuid](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Converter_GetDebtors_IntToGuid)
     """
 
-    def __init__(self, sandbox: bool = True) -> None:
-        super().__init__(sandbox)
+    def __init__(self, auth_manager: AuthManager, sandbox: bool = True):
+        super().__init__(auth_manager, sandbox)
 
         # Initialize nmbrs services
-        self.debtor_service = Client(f"{self.base_uri}{self.debtor_uri}")
+        self.client = Client(f"{self.base_uri}{self.debtor_uri}")
 
         # Micro services
-        self.department = DebtorDepartmentService(self.debtor_service)
-        self.function = DebtorFunctionService(self.debtor_service)
-        self.webhook = DebtorWebHooksService(self.debtor_service)
-        self.title = DebtorTitleService(self.debtor_service)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        """
-        Method to set the authentication.
-
-        Args:
-            auth_header (dict): A dictionary containing authentication details.
-        """
-        self.auth_header = auth_header
-
-        # Micro services
-        self.department.set_auth_header(auth_header)
-        self.function.set_auth_header(auth_header)
-        self.webhook.set_auth_header(auth_header)
-        self.title.set_auth_header(auth_header)
+        self.department = DebtorDepartmentService(self.auth_manager, self.client)
+        self.function = DebtorFunctionService(self.auth_manager, self.client)
+        self.webhook = DebtorWebHooksService(self.auth_manager, self.client)
+        self.title = DebtorTitleService(self.auth_manager, self.client)
 
     @nmbrs_exception_handler(resource="DebtorService:Environment_Get")
     def get_domain(self, username: str, token: str) -> Domain:
         """
         Generate authentication header for standard token-based authentication.
 
         For more information, refer to the official documentation:
@@ -70,30 +56,30 @@
         Args:
             username (str): A string representing the username for authentication.
             token (str): A string representing the token for authentication.
 
         Returns:
             Domain: The domain object associated with the token.
         """
-        env = self.debtor_service.service.Environment_Get(_soapheaders={"AuthHeader": {"Username": username, "Token": token}})
+        env = self.client.service.Environment_Get(_soapheaders={"AuthHeader": {"Username": username, "Token": token}})
         return Domain(data=serialize_object(env))
 
     @return_list
     @nmbrs_exception_handler(resource="DebtorService:List_GetAll")
     def get_all(self) -> list[Debtor]:
         """
         Retrieve all debtors.
 
         For more information, refer to the official documentation:
             [Soap call List_GetAll](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=List_GetAll)
 
         Returns:
             list[Debtor]: A list of Debtor objects representing all debtors.
         """
-        debtors = self.debtor_service.service.List_GetAll(_soapheaders=self.auth_header)
+        debtors = self.client.service.List_GetAll(_soapheaders=self.auth_manager.header)
         debtors = [Debtor(debtor) for debtor in serialize_object(debtors)]
         return debtors
 
     @return_list
     @nmbrs_exception_handler(resource="DebtorService:List_GetByNumber")
     def get_all_by_number(self, number: str) -> list[Debtor]:
         """
@@ -104,15 +90,15 @@
 
         Args:
             number (str): The debtor number.
 
         Returns:
             list[Debtor]: A list of Debtor objects representing all debtors.
         """
-        debtors = self.debtor_service.service.List_GetByNumber(Number=number, _soapheaders=self.auth_header)
+        debtors = self.client.service.List_GetByNumber(Number=number, _soapheaders=self.auth_manager.header)
         debtors = [Debtor(debtor) for debtor in serialize_object(debtors)]
         return debtors
 
     @nmbrs_exception_handler(resource="DebtorService:Debtor_Get")
     def get(self, debtor_id: int) -> Debtor | None:
         """
         Retrieve a debtor by ID.
@@ -122,21 +108,21 @@
 
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             Debtor | None: A Debtor object representing the debtor if found, otherwise None.
         """
-        debtor = self.debtor_service.service.Debtor_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        debtor = self.client.service.Debtor_Get(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         if debtor is None:
             return None
         return Debtor(serialize_object(debtor))
 
     @nmbrs_exception_handler(resource="DebtorService:Debtor_Insert")
-    def insert(self, debtor_id: int, number: str, name: str) -> int:
+    def post(self, debtor_id: int, number: str, name: str) -> int:
         """
         Insert a new debtor.
 
         For more information, refer to the official documentation:
             [Soap call Debtor_Insert](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Debtor_Insert)
 
         Args:
@@ -144,15 +130,15 @@
             number (str): The number of the debtor.
             name (str): The name of the debtor.
 
         Returns:
             int: The ID of the inserted debtor if successful.
         """
         data = {"Debtor": {"Id": debtor_id, "Number": number, "Name": name}}
-        inserted = self.debtor_service.service.Debtor_Insert(**data, _soapheaders=self.auth_header)
+        inserted = self.client.service.Debtor_Insert(**data, _soapheaders=self.auth_manager.header)
         return inserted
 
     @nmbrs_exception_handler(resource="DebtorService:Debtor_Update")
     def update(self, debtor_id: int, number: str, name: str) -> None:
         """
         Update an existing debtor.
 
@@ -161,15 +147,15 @@
 
         Args:
             debtor_id (int): The ID of the debtor.
             number (str): The new number of the debtor.
             name (str): The new name of the debtor.
         """
         data = {"Debtor": {"Id": debtor_id, "Number": number, "Name": name}}
-        self.debtor_service.service.Debtor_Update(**data, _soapheaders=self.auth_header)
+        self.client.service.Debtor_Update(**data, _soapheaders=self.auth_manager.header)
 
     @return_list
     @nmbrs_exception_handler(resource="DebtorService:AbsenceXML_Get")
     def get_absence_xml(self, debtor_id: int, start_date: datetime, end_date: datetime) -> list[AbsenceVerzuim]:
         """
         Retrieve absence data for a debtor within a specified date range.
 
@@ -181,15 +167,15 @@
             start_date (datetime): A datetime representing the start date of the period to retrieve data.
             end_date (datetime): A datetime representing the end date of the period to retrieve data.
 
         Returns:
             list[AbsenceVerzuim]: A list of AbsenceVerzuim objects representing the absence data.
         """
         data = {"DebtorId": debtor_id, "from": start_date, "to": end_date}
-        absences = self.debtor_service.service.AbsenceXML_Get(**data, _soapheaders=self.auth_header)
+        absences = self.client.service.AbsenceXML_Get(**data, _soapheaders=self.auth_manager.header)
         absences = [AbsenceVerzuim(absence) for absence in serialize_object(absences)]
         return absences
 
     @return_list
     @nmbrs_exception_handler(resource="DebtorService:AccountantContact_GetList")
     def get_all_accountant_contact_info(self, debtor_id: int) -> list[ContactInfo]:
         """
@@ -200,15 +186,15 @@
 
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             list[ContactInfo]: A list of ContactInfo objects representing the accountant contact information.
         """
-        accountants = self.debtor_service.service.AccountantContact_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        accountants = self.client.service.AccountantContact_GetList(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         accountants = [ContactInfo(debtor_id=debtor_id, data=accountant) for accountant in serialize_object(accountants)]
         return accountants
 
     @nmbrs_exception_handler(resource="DebtorService:Address_Get")
     def get_address(self, debtor_id: int) -> Address | None:
         """
         Retrieve address information for a debtor.
@@ -218,15 +204,15 @@
 
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             Address | None: An Address object representing the address if found, otherwise None.
         """
-        address = self.debtor_service.service.Address_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        address = self.client.service.Address_Get(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         if address is None:
             return None
         return Address(debtor_id=debtor_id, data=serialize_object(address))
 
     @nmbrs_exception_handler(resource="DebtorService:BankAccount_Get")
     def get_bank_account(self, debtor_id: int) -> BankAccount | None:
         """
@@ -237,15 +223,15 @@
 
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             BankAccount | None: A BankAccount object representing the bank account if found, otherwise None.
         """
-        bank_account = self.debtor_service.service.BankAccount_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        bank_account = self.client.service.BankAccount_Get(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         if bank_account is None:
             return None
         return BankAccount(debtor_id=debtor_id, data=serialize_object(bank_account))
 
     @nmbrs_exception_handler(resource="DebtorService:ContactPerson_Get")
     def get_contact_person(self, debtor_id: int) -> ContactInfo | None:
         """
@@ -256,15 +242,15 @@
 
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             ContactInfo | None: A ContactInfo object representing the contact person if found, otherwise None.
         """
-        contact_person = self.debtor_service.service.ContactPerson_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        contact_person = self.client.service.ContactPerson_Get(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         if contact_person is None:
             return None
         return ContactInfo(debtor_id=debtor_id, data=serialize_object(contact_person))
 
     @nmbrs_exception_handler(resource="DebtorService:Debtor_IsOwner")
     def is_owner(self) -> bool:
         """
@@ -272,37 +258,37 @@
 
         For more information, refer to the official documentation:
             [Soap call Debtor_IsOwner](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Debtor_IsOwner)
 
         Returns:
             bool: True if the current user is the owner of the debtor, otherwise False.
         """
-        is_owner = self.debtor_service.service.Debtor_IsOwner(_soapheaders=self.auth_header)
+        is_owner = self.client.service.Debtor_IsOwner(_soapheaders=self.auth_manager.header)
         return is_owner
 
     @return_list
     @nmbrs_exception_handler(resource="DebtorService:LabourAgreementSettings_GetList")
-    def get_all_labour_agreements(self, debtor_id: int, year: int, period: int) -> list[LabourAgreementSettings]:
+    def get_all_labour_agreements(self, debtor_id: int, period: int, year: int) -> list[LabourAgreementSettings]:
         """
         Retrieve all labour agreement settings for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call LabourAgreementSettings_GetList](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=LabourAgreementSettings_GetList)
 
         Args:
             debtor_id (int): The ID of the debtor.
-            year (int): The year for which to retrieve labour agreement settings.
             period (int): The period for which to retrieve labour agreement settings.
+            year (int): The year for which to retrieve labour agreement settings.
 
         Returns:
             list[LabourAgreementSettings]: A list of LabourAgreementSettings objects representing all labour
             agreement settings.
         """
-        labour_agreements = self.debtor_service.service.LabourAgreementSettings_GetList(
-            DebtorId=debtor_id, Year=year, Period=period, _soapheaders=self.auth_header
+        labour_agreements = self.client.service.LabourAgreementSettings_GetList(
+            DebtorId=debtor_id, Year=year, Period=period, _soapheaders=self.auth_manager.header
         )
         labour_agreements = [
             LabourAgreementSettings(debtor_id=debtor_id, data=labour_agreement) for labour_agreement in serialize_object(labour_agreements)
         ]
         return labour_agreements
 
     @return_list
@@ -316,15 +302,15 @@
 
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             list[Manager]: A list of Manager objects representing all managers for the debtor.
         """
-        managers = self.debtor_service.service.Manager_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        managers = self.client.service.Manager_GetList(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         managers = [Manager(debtor_id=debtor_id, data=manager) for manager in serialize_object(managers)]
         return managers
 
     @nmbrs_exception_handler(resource="DebtorService:ServiceLevel_Get")
     def get_service_level(self, debtor_id: int) -> ServiceLevel | None:
         """
         Retrieve service level information for a debtor.
@@ -335,15 +321,15 @@
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             ServiceLevel | None: A ServiceLevel object representing the service level information if found, otherwise
             None.
         """
-        service_level = self.debtor_service.service.ServiceLevel_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        service_level = self.client.service.ServiceLevel_Get(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         if service_level is None:
             return None
         return ServiceLevel(debtor_id=debtor_id, data=serialize_object(service_level))
 
     @return_list
     @nmbrs_exception_handler(resource="DebtorService:Tags_Get")
     def get_tags(self, debtor_id: int) -> list[Tag]:
@@ -355,10 +341,10 @@
 
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             list[Tag]: A list of Tag objects representing all tags associated with the debtor.
         """
-        tags = self.debtor_service.service.Tags_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        tags = self.client.service.Tags_Get(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         tags = [Tag(debtor_id=debtor_id, data=tag) for tag in serialize_object(tags)]
         return tags
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/employee_service.py` & `nmbrs-0.2.0/src/nmbrs/service/employee_service.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,110 +32,72 @@
     EmployeeServiceService,
     EmployeeSpaarloonService,
     EmployeeSvwService,
     EmployeeTimeRegistrationService,
     EmployeeTimeScheduleService,
 )
 from .service import Service
+from ..auth.token_manager import AuthManager
 from ..data_classes.employee import EmployeeTypes, Employee, Period
 from ..utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ..utils.return_list import return_list
 
 
 class EmployeeService(Service):
     """A class representing Employee Service for interacting with Nmbrs employee-related functionalities."""
 
-    def __init__(self, sandbox: bool = True) -> None:
-        super().__init__(sandbox)
+    def __init__(self, auth_manager: AuthManager, sandbox: bool = True):
+        super().__init__(auth_manager, sandbox)
 
         # Initialize nmbrs services
         self.client = Client(f"{self.base_uri}{self.employee_uri}")
 
         # Micro services
-        self.absence = EmployeeAbsenceService(self.client)
-        self.address = EmployeeAddressService(self.client)
-        self.bank_account = EmployeeBankAccountService(self.client)
-        self.child = EmployeeChildService(self.client)
-        self.contract = EmployeeContractService(self.client)
-        self.cost_center = EmployeeCostCenterService(self.client)  # TO BE implemented
-        self.days = EmployeeDaysService(self.client)  # TO BE implemented
-        self.department = EmployeeDepartmentsService(self.client)  # TO BE implemented
-        self.document = EmployeeDocumentService(self.client)  # TO BE implemented
-        self.employment = EmployeeEmploymentService(self.client)  # TO BE implemented
-        self.function = EmployeeFunctionService(self.client)  # TO BE implemented
-        self.hour_component = EmployeeHourComponentFixedService(self.client)  # TO BE implemented
-        self.labour_agreement = EmployeeLabourAgreementService(self.client)  # TO BE implemented
-        self.lease_car = EmployeeLeaseCarService(self.client)  # TO BE implemented
-        self.leave = EmployeeLeaveService(self.client)  # TO BE implemented
-        self.levensloop = EmployeeLevensLoopService(self.client)  # TO BE implemented
-        self.manager = EmployeeManagerService(self.client)  # TO BE implemented
-        self.partner = EmployeePartnerService(self.client)  # TO BE implemented
-        self.personal_info = EmployeePersonalInfoService(self.client)
-        self.salary = EmployeeSalaryService(self.client)  # TO BE implemented
-        self.schedule = EmployeeScheduleService(self.client)  # TO BE implemented
-        self.service = EmployeeServiceService(self.client)  # TO BE implemented
-        self.spaarloon = EmployeeSpaarloonService(self.client)  # TO BE implemented
-        self.svw = EmployeeSvwService(self.client)  # TO BE implemented
-        self.time_registration = EmployeeTimeRegistrationService(self.client)  # TO BE implemented
-        self.time_schedule = EmployeeTimeScheduleService(self.client)  # TO BE implemented
-        self.wage_component = EmployeeWageComponentsService(self.client)  # TO BE implemented
-        self.wage_tax = EmployeeWageTaxService(self.client)  # TO BE implemented
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        """
-        Method to set the authentication.
-
-        Args:
-            auth_header (dict): A dictionary containing authentication details.
-        """
-        self.auth_header = auth_header
-
-        # Micro services
-        self.absence.set_auth_header(auth_header)
-        self.address.set_auth_header(auth_header)
-        self.bank_account.set_auth_header(auth_header)
-        self.child.set_auth_header(auth_header)
-        self.contract.set_auth_header(auth_header)
-        self.cost_center.set_auth_header(auth_header)
-        self.days.set_auth_header(auth_header)
-        self.department.set_auth_header(auth_header)
-        self.document.set_auth_header(auth_header)
-        self.employment.set_auth_header(auth_header)
-        self.function.set_auth_header(auth_header)
-        self.hour_component.set_auth_header(auth_header)
-        self.labour_agreement.set_auth_header(auth_header)
-        self.lease_car.set_auth_header(auth_header)
-        self.leave.set_auth_header(auth_header)
-        self.levensloop.set_auth_header(auth_header)
-        self.manager.set_auth_header(auth_header)
-        self.partner.set_auth_header(auth_header)
-        self.personal_info.set_auth_header(auth_header)
-        self.salary.set_auth_header(auth_header)
-        self.schedule.set_auth_header(auth_header)
-        self.service.set_auth_header(auth_header)
-        self.spaarloon.set_auth_header(auth_header)
-        self.svw.set_auth_header(auth_header)
-        self.time_registration.set_auth_header(auth_header)
-        self.time_schedule.set_auth_header(auth_header)
-        self.wage_component.set_auth_header(auth_header)
-        self.wage_tax.set_auth_header(auth_header)
+        self.absence = EmployeeAbsenceService(self.auth_manager, self.client)
+        self.address = EmployeeAddressService(self.auth_manager, self.client)
+        self.bank_account = EmployeeBankAccountService(self.auth_manager, self.client)
+        self.child = EmployeeChildService(self.auth_manager, self.client)
+        self.contract = EmployeeContractService(self.auth_manager, self.client)
+        self.cost_center = EmployeeCostCenterService(self.auth_manager, self.client)  # TO BE implemented
+        self.days = EmployeeDaysService(self.auth_manager, self.client)  # TO BE implemented
+        self.department = EmployeeDepartmentsService(self.auth_manager, self.client)  # TO BE implemented
+        self.document = EmployeeDocumentService(self.auth_manager, self.client)  # TO BE implemented
+        self.employment = EmployeeEmploymentService(self.auth_manager, self.client)  # TO BE implemented
+        self.function = EmployeeFunctionService(self.auth_manager, self.client)  # TO BE implemented
+        self.hour_component = EmployeeHourComponentFixedService(self.auth_manager, self.client)  # TO BE implemented
+        self.labour_agreement = EmployeeLabourAgreementService(self.auth_manager, self.client)  # TO BE implemented
+        self.lease_car = EmployeeLeaseCarService(self.auth_manager, self.client)  # TO BE implemented
+        self.leave = EmployeeLeaveService(self.auth_manager, self.client)  # TO BE implemented
+        self.levensloop = EmployeeLevensLoopService(self.auth_manager, self.client)  # TO BE implemented
+        self.manager = EmployeeManagerService(self.auth_manager, self.client)
+        self.partner = EmployeePartnerService(self.auth_manager, self.client)  # TO BE implemented
+        self.personal_info = EmployeePersonalInfoService(self.auth_manager, self.client)
+        self.salary = EmployeeSalaryService(self.auth_manager, self.client)  # TO BE implemented
+        self.schedule = EmployeeScheduleService(self.auth_manager, self.client)  # TO BE implemented
+        self.service = EmployeeServiceService(self.auth_manager, self.client)  # TO BE implemented
+        self.spaarloon = EmployeeSpaarloonService(self.auth_manager, self.client)  # TO BE implemented
+        self.svw = EmployeeSvwService(self.auth_manager, self.client)  # TO BE implemented
+        self.time_registration = EmployeeTimeRegistrationService(self.auth_manager, self.client)  # TO BE implemented
+        self.time_schedule = EmployeeTimeScheduleService(self.auth_manager, self.client)  # TO BE implemented
+        self.wage_component = EmployeeWageComponentsService(self.auth_manager, self.client)  # TO BE implemented
+        self.wage_tax = EmployeeWageTaxService(self.auth_manager, self.client)  # TO BE implemented
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:EmployeeType_GetList")
     def get_types(self) -> list[EmployeeTypes]:
         """
         Get the list of all employee types available.
 
         For more information, refer to the official documentation:
             [EmployeeType_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=EmployeeType_GetList)
 
         Returns:
             list[EmployeeTypes]: A list of employee type objects.
         """
-        employee_types = self.client.service.EmployeeType_GetList(_soapheaders=self.auth_header)
+        employee_types = self.client.service.EmployeeType_GetList(_soapheaders=self.auth_manager.header)
         employee_types = [EmployeeTypes(employee_type) for employee_type in serialize_object(employee_types)]
         return employee_types
 
     @nmbrs_exception_handler(resource="EmployeeService:Employee_GetCurrent")
     def get_current_period(self, employee_id: int) -> Period | None:
         """
         Get the employees current period, Format = yyyy-pp-type, example: 2010-5-M or 2010-4-4W.
@@ -145,15 +107,15 @@
 
         Args:
             employee_id (int): The ID of the employee.
 
         Returns:
             Period: year, period and period type and the company.
         """
-        period = self.client.service.Employee_GetCurrent(EmployeeId=employee_id, _soapheaders=self.auth_header)
+        period = self.client.service.Employee_GetCurrent(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
         if period is None:
             return None
         return Period(employee_id=employee_id, data=serialize_object(period))
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:List_GetByCompany")
     def get_by_company(self, company_id: int, employee_type: int) -> list[Employee]:
@@ -166,15 +128,17 @@
         Args:
             company_id (int): The ID of the company.
             employee_type (int): The type of employees to be returned.
 
         Returns:
             list[Employee]: A list of employee objects.
         """
-        employees = self.client.service.List_GetByCompany(CompanyId=company_id, EmployeeType=employee_type, _soapheaders=self.auth_header)
+        employees = self.client.service.List_GetByCompany(
+            CompanyId=company_id, EmployeeType=employee_type, _soapheaders=self.auth_manager.header
+        )
         employees = [Employee(employee) for employee in serialize_object(employees)]
         return employees
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:List_GetByDebtor")
     def get_by_debtor(self, debtor_id: int, employee_type: int) -> list[Employee]:
         """
@@ -186,42 +150,44 @@
         Args:
             debtor_id (int): The ID of the company.
             employee_type (int): The type of employees to be returned.
 
         Returns:
             list[Employee]: A list of employee objects.
         """
-        employees = self.client.service.List_GetByDebtor(DebtorId=debtor_id, EmployeeType=employee_type, _soapheaders=self.auth_header)
+        employees = self.client.service.List_GetByDebtor(
+            DebtorId=debtor_id, EmployeeType=employee_type, _soapheaders=self.auth_manager.header
+        )
         employees = [Employee(employee) for employee in serialize_object(employees)]
         return employees
 
     @nmbrs_exception_handler(resource="EmployeeService:Employee_Insert")
-    def insert(self):
+    def post(self):
         """
         Create a new Employee, returns the id of this Employee.
         If the date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Employee_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Employee_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:Employee_InsertBasedOnDefault")
-    def insert_based_on_default(self):
+    def post_based_on_default(self):
         """
         Insert new employee based on default employee.
         If the date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Employee_InsertBasedOnDefault](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Employee_InsertBasedOnDefault)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:Employee_InsertByEmployeeType")
-    def insert_with_type(self):
+    def post_with_type(self):
         """
         Create a new employee based on the employee type and returns the Id of this employee.
         If the date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Employee_InsertByEmployeeType](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Employee_InsertByEmployeeType)
         """
@@ -274,25 +240,25 @@
 
         For more information, refer to the official documentation:
             [ExtraFields_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=ExtraFields_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:PerformanceReview_Get")
-    def get_performance(self):
+    def get_performance_reviews(self):
         """
         Get the HR Performance Review for the given Employee ID.
 
         For more information, refer to the official documentation:
             [PerformanceReview_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=PerformanceReview_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:PerformanceReview_GetAll_AllEmployeesByCompany")
-    def get_all_performance_by_company(self):
+    def get_all_performance_reviewa_by_company(self):
         """
         Get the HR Performance Reviews for all the employees in the given Company ID.
 
         For more information, refer to the official documentation:
             [PerformanceReview_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=PerformanceReview_GetAll_AllEmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/__init__.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/address.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/address.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 """Microservice responsible for address-related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import Address
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ..micro_service import MicroService
 
 
 class CompanyAddressService(MicroService):
     """Microservice responsible for address-related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="CompanyService:Address_GetCurrent")
-    def get(self, company_id: int) -> Address | None:
+    def get_current(self, company_id: int) -> Address | None:
         """
         Get the current address of the company.
 
         For more information, refer to the official documentation:
             [Address_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=Address_GetCurrent)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             Address | None: An Address object if found, otherwise None.
         """
-        address = self.client.service.Address_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
+        address = self.client.service.Address_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         if address is None:
             return None
         return Address(company_id=company_id, data=serialize_object(address))
 
     @nmbrs_exception_handler(resource="CompanyService:Address_Insert")
-    def insert(
+    def post(
         self,
         company_id: int,
         address_id: int,
         default: bool,
         street: str,
         house_number: str,
         house_number_addon: str,
@@ -81,15 +79,15 @@
                 "HouseNumberAddition": house_number_addon,
                 "PostalCode": postal_code,
                 "City": city,
                 "StateProvince": state_province,
                 "CountryISOCode": country_iso_code,
             },
         }
-        response = self.client.service.Address_Insert(**data, _soapheaders=self.auth_header)
+        response = self.client.service.Address_Insert(**data, _soapheaders=self.auth_manager.header)
         return response
 
     @nmbrs_exception_handler(resource="CompanyService:Address_Update")
     def update(
         self,
         company_id: int,
         address_id: int,
@@ -130,8 +128,8 @@
                 "HouseNumberAddition": house_number_addon,
                 "PostalCode": postal_code,
                 "City": city,
                 "StateProvince": state_province,
                 "CountryISOCode": country_iso_code,
             },
         }
-        self.client.service.Address_Update(**data, _soapheaders=self.auth_header)
+        self.client.service.Address_Update(**data, _soapheaders=self.auth_manager.header)
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/bank_account.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/bank_account.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Microservice responsible for bank account related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import BankAccount
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class CompanyBankAccountService(MicroService):
     """Microservice responsible for bank account related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="CompanyService:BankAccount_GetCurrent")
     def get_current(self, company_id: int) -> BankAccount | None:
         """
         Get the company's current bank account.
 
         For more information, refer to the official documentation:
@@ -27,21 +25,21 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             BankAccount: An BankAccount object.
         """
-        bank_account = self.client.service.BankAccount_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
+        bank_account = self.client.service.BankAccount_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         if bank_account is None:
             return None
         return BankAccount(company_id=company_id, data=serialize_object(bank_account))
 
     @nmbrs_exception_handler(resource="CompanyService:BankAccount_Insert")
-    def insert(
+    def post(
         self,
         company_id: int,
         account_id: int,
         account_number: str,
         description: str,
         iban: str,
         bic: str,
@@ -76,15 +74,17 @@
             "Description": description,
             "IBAN": iban,
             "BIC": bic,
             "City": city,
             "Name": name,
             "Type": account_type,
         }
-        response = self.client.service.BankAccount_Insert(CompanyId=company_id, BankAccount=bank_account, _soapheaders=self.auth_header)
+        response = self.client.service.BankAccount_Insert(
+            CompanyId=company_id, BankAccount=bank_account, _soapheaders=self.auth_manager.header
+        )
         return response
 
     @nmbrs_exception_handler(resource="CompanyService:BankAccount_Update")
     def update(
         self,
         company_id: int,
         account_id: int,
@@ -122,8 +122,8 @@
             "Description": description,
             "IBAN": iban,
             "BIC": bic,
             "City": city,
             "Name": name,
             "Type": account_type,
         }
-        self.client.service.BankAccount_Update(CompanyId=company_id, BankAccount=bank_account, _soapheaders=self.auth_header)
+        self.client.service.BankAccount_Update(CompanyId=company_id, BankAccount=bank_account, _soapheaders=self.auth_manager.header)
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/cost_center.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/cost_center.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 """Microservice responsible for managing cost centers at the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import CostCenter
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class CompanyCostCenterService(MicroService):
     """Microservice responsible for managing cost centers at the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:CostCenter_GetList")
-    def get(self, company_id: int) -> list[CostCenter]:
+    def get_current(self, company_id: int) -> list[CostCenter]:
         """
         Retrieve cost centers associated with a company.
 
         For further details, see the official documentation:
             [CostCenter_GetList](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=CostCenter_GetList)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[CostCenter]: A list of cost center objects.
         """
-        cost_centers = self.client.service.CostCenter_GetList(CompanyId=company_id, _soapheaders=self.auth_header)
+        cost_centers = self.client.service.CostCenter_GetList(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         return [CostCenter(company_id=company_id, data=cost_center) for cost_center in serialize_object(cost_centers)]
 
     @nmbrs_exception_handler(resource="CompanyService:CostCenter_Insert")
-    def insert(self, company_id: int, cost_center_id: int, code: str, description: str) -> int:
+    def post(self, company_id: int, cost_center_id: int, code: str, description: str) -> int:
         """
         Insert or update a cost center within a company.
 
         For further details, see the official documentation:
             [CostCenter_Insert](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=CostCenter_Insert)
 
         Args:
@@ -51,10 +49,10 @@
             description (str): The description of the cost center.
 
         Returns:
             int: The ID of the inserted or updated cost center.
         """
         cost_center = {"Id": cost_center_id, "Code": code, "Description": description}
         cost_center_id = self.client.service.CostCenter_Insert(
-            CompanyId=company_id, kostenplaats=cost_center, _soapheaders=self.auth_header
+            CompanyId=company_id, kostenplaats=cost_center, _soapheaders=self.auth_manager.header
         )
         return cost_center_id
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/cost_unit.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/cost_unit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 """Microservice responsible for cost unit related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import CostUnit
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class CompanyCostUnitService(MicroService):
     """Microservice responsible for cost unit related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:CostUnit_GetList")
-    def get(self, company_id: int) -> list[CostUnit]:
+    def get_current(self, company_id: int) -> list[CostUnit]:
         """
         Get cost units that belong to a company
 
         For more information, refer to the official documentation:
             [CostUnit_GetList](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=CostUnit_GetList)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[CostUnit]: A list of cost unit objects.
         """
-        cost_units = self.client.service.CostUnit_GetList(CompanyId=company_id, _soapheaders=self.auth_header)
+        cost_units = self.client.service.CostUnit_GetList(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         return [CostUnit(company_id=company_id, data=cost_unit) for cost_unit in serialize_object(cost_units)]
 
     @nmbrs_exception_handler(resource="CompanyService:CostUnit_Insert")
-    def insert(self, company_id: int, cost_unit_id: int, code: str, description: str) -> int:
+    def post(self, company_id: int, cost_unit_id: int, code: str, description: str) -> int:
         """
         Update or insert a Cost Unit into a company.
 
         For more information, refer to the official documentation:
             [CostUnit_Insert](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=CostUnit_Insert)
 
         Args:
@@ -50,9 +48,9 @@
             code (str): The code of the cost unit.
             description (str): The description of the cost unit.
 
         Returns:
             int: The ID of the inserted or updated cost unit.
         """
         cost_unit = {"Id": cost_unit_id, "Code": code, "Description": description}
-        cost_unit_id = self.client.service.CostUnit_Insert(CompanyId=company_id, costunit=cost_unit, _soapheaders=self.auth_header)
+        cost_unit_id = self.client.service.CostUnit_Insert(CompanyId=company_id, costunit=cost_unit, _soapheaders=self.auth_manager.header)
         return cost_unit_id
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/hour_model.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/hour_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 """Microservice responsible for hour model related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import HourCode
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class CompanyHourModelService(MicroService):
     """Microservice responsible for hour model related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:HourModel_GetHourCodes")
-    def get(self, company_id: int) -> list[HourCode]:
+    def get_current(self, company_id: int) -> list[HourCode]:
         """
         Get hour codes that belong to a company's hour model.
 
         For more information, refer to the official documentation:
             [HourModel_GetHourCodes](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=HourModel_GetHourCodes)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[HourCode]: A list of hour code objects.
         """
-        hour_codes = self.client.service.HourModel_GetHourCodes(CompanyId=company_id, _soapheaders=self.auth_header)
+        hour_codes = self.client.service.HourModel_GetHourCodes(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         return [HourCode(company_id=company_id, data=hour_code) for hour_code in serialize_object(hour_codes)]
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:HourModel2_GetHourCodes")
-    def get_2(self, company_id: int) -> list[HourCode]:
+    def get_current_2(self, company_id: int) -> list[HourCode]:
         """
         Get hour codes that belong to a company's hour model 2.
 
         For more information, refer to the official documentation:
             [HourModel2_GetHourCodes](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=HourModel2_GetHourCodes)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[HourCode]: A list of hour code objects.
         """
-        hour_codes = self.client.service.HourModel2_GetHourCodes(CompanyId=company_id, _soapheaders=self.auth_header)
+        hour_codes = self.client.service.HourModel2_GetHourCodes(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         return [HourCode(company_id=company_id, data=hour_code) for hour_code in serialize_object(hour_codes)]
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/journal.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/journal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # pylint: disable=line-too-long
 """Microservice responsible for journal related actions on the company level."""
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class CompanyJournalService(MicroService):
     """Microservice responsible for journal related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="CompanyService:Journals_GetByRunCompany")
     def get_run_by_company(self):
         """
         Returns the Journal XML, takes year from active year of the company.
 
         For more information, refer to the official documentation:
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/labout_aggreement.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/labout_aggreement.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """Microservice responsible for labour agreement related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import LabourAgreement, LeaveTypeGroup
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class CompanyLabourAgreementService(MicroService):
     """
     Microservice responsible for labour agreement related actions on the company level.
     """
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:LabourAgreements_Get")
     def get(self, company_id: int, period: int, year: int):
         """
         Get a list of all the labour agreements that are assigned to a company.
 
@@ -37,15 +35,15 @@
         Returns:
             list[LabourAgreement]: A list of LabourAgreement objects.
         """
         labour_agreements = self.client.service.LabourAgreements_Get(
             CompanyId=company_id,
             Period=period,
             Year=year,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         labour_agreements = [
             LabourAgreement(company_id=company_id, data=labour_agreement) for labour_agreement in serialize_object(labour_agreements)
         ]
         return labour_agreements
 
     @return_list
@@ -59,41 +57,41 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[LabourAgreement]: A list of LabourAgreement objects representing the current labour agreements.
         """
-        labour_agreements = self.client.service.LabourAgreements_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
+        labour_agreements = self.client.service.LabourAgreements_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         labour_agreements = [
             LabourAgreement(company_id=company_id, data=labour_agreement) for labour_agreement in serialize_object(labour_agreements)
         ]
         return labour_agreements
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:CompanyLeaveTypeGroups_Get")
     def get_leave_type_groups(
-        self, company_id: int, labour_agreement_settings_group_id: int, year: int, period: int
+        self, company_id: int, labour_agreement_settings_group_id: int, period: int, year: int
     ) -> list[LeaveTypeGroup]:
         """
         Get the company's leave type groups.
 
         For further details, see the official documentation:
             [CompanyLeaveTypeGroups_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=CompanyLeaveTypeGroups_Get)
 
         Args:
             company_id (int): The ID of the company.
             labour_agreement_settings_group_id (int): The ID of the labour agreement settings group.
-            year (int): The year.
             period (int): The period.
+            year (int): The year.
 
         Returns:
             List[LeaveTypeGroup]: A list of LeaveTypeGroup objects.
         """
         responses = self.client.service.CompanyLeaveTypeGroups_Get(
             CompanyId=company_id,
             LabourAgreementSettingsGroupId=labour_agreement_settings_group_id,
             Year=year,
             Period=period,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return [LeaveTypeGroup(company_id=company_id, data=response) for response in serialize_object(responses)]
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/pension.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/pension.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Microservice responsible for pension related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import Pension, PensionXML
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class CompanyPensionService(MicroService):
     """Microservice responsible for pension related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:PensionExport_GetList")
     def get(self, company_id: int, year: int) -> list[Pension]:
         """
         Returns pension exports that belong to a company for a certain year.
 
@@ -30,15 +28,15 @@
         Args:
             company_id (int): The ID of the company.
             year (int): The year to retrieve the pension information for.
 
         Returns:
             list[Pension]: A list of pension objects.
         """
-        pensions = self.client.service.PensionExport_GetList(CompanyId=company_id, intYear=year, _soapheaders=self.auth_header)
+        pensions = self.client.service.PensionExport_GetList(CompanyId=company_id, intYear=year, _soapheaders=self.auth_manager.header)
         return [Pension(company_id=company_id, data=pension) for pension in serialize_object(pensions)]
 
     @nmbrs_exception_handler(resource="CompanyService:PensionExport_GetXML")
     def get_xml(self, company_id: int, pension_export_id: int) -> PensionXML:
         """
         Returns one XML pension export by ID that belong to a company.
 
@@ -49,10 +47,10 @@
             company_id (int): The ID of the company.
             pension_export_id (int): Unique id of a pension export.
 
         Returns:
             list[CostCenter]: A list of cost center objects.
         """
         pension_xml = self.client.service.PensionExport_GetXML(
-            CompanyId=company_id, PensionExportID=pension_export_id, _soapheaders=self.auth_header
+            CompanyId=company_id, PensionExportID=pension_export_id, _soapheaders=self.auth_manager.header
         )
         return PensionXML(serialize_object(pension_xml))
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/run.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """Microservice responsible for run related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import RunRequest, RunInfo
 from ....data_classes.employee import Employee
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class CompanyRunService(MicroService):
     """Microservice responsible for run related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:RunRequest_GetList")
     def get_requests(self, company_id: int, year: int) -> list[RunRequest]:
         """
         Returns a list of requested runs with status for given company and year.
 
@@ -31,29 +29,29 @@
         Args:
             company_id (int): The ID of the company.
             year (int): year.
 
         Returns:
             list[RunRequest]: A list of run requests objects.
         """
-        run_requests = self.client.service.RunRequest_GetList(CompanyId=company_id, Year=year, _soapheaders=self.auth_header)
+        run_requests = self.client.service.RunRequest_GetList(CompanyId=company_id, Year=year, _soapheaders=self.auth_manager.header)
         return [RunRequest(company_id=company_id, data=run_request) for run_request in serialize_object(run_requests)]
 
     @nmbrs_exception_handler(resource="CompanyService:RunRequest_Insert")
     def insert_request(self, company_id: int):
         """
         Requests a run for given company.
 
         For more information, refer to the official documentation:
             [RunRequest_Insert](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=RunRequest_Insert)
 
         Args:
             company_id (int): The ID of the company.
         """
-        self.client.service.RunRequest_Insert(CompanyId=company_id, _soapheaders=self.auth_header)
+        self.client.service.RunRequest_Insert(CompanyId=company_id, _soapheaders=self.auth_manager.header)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:Run_GetList")
     def get(self, company_id: int, year: int) -> list[RunInfo]:
         """
         Get the company's run list for a specified year.
 
@@ -63,15 +61,15 @@
         Args:
             company_id (int): The ID of the company.
             year (int): year.
 
         Returns:
             list[RunInfo]: A list of run info objects.
         """
-        runs = self.client.service.Run_GetList(CompanyId=company_id, Year=year, _soapheaders=self.auth_header)
+        runs = self.client.service.Run_GetList(CompanyId=company_id, Year=year, _soapheaders=self.auth_manager.header)
         return [RunInfo(company_id=company_id, data=run) for run in serialize_object(runs)]
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:Run_GetEmployeesByRunCompany")
     def get_all_employees_by_run(self, company_id: int, year: int, run_id: int) -> list[Employee]:
         """
         Get the employee's list for a specified company id, run id and year
@@ -84,35 +82,35 @@
             year (int): Year.
             run_id (int): The unique identifier for a run.
 
         Returns:
             list[Employee]: A list of employee objects, with the name field empty.
         """
         employees = self.client.service.Run_GetEmployeesByRunCompany(
-            CompanyId=company_id, Year=year, RunId=run_id, _soapheaders=self.auth_header
+            CompanyId=company_id, Year=year, RunId=run_id, _soapheaders=self.auth_manager.header
         )
         return [
             Employee({"Id": employee.get("EmployeeId"), "Number": employee.get("EmployeeNumber")})
             for employee in serialize_object(employees)
         ]
 
     @nmbrs_exception_handler(resource="CompanyService:HrDocuments_EmployerCostPerHour_Year")
-    def get_hr_documents_cost_per_hour_year(self, company_id: int, run_id: int, year: int, period: int) -> bytes:
+    def get_hr_documents_cost_per_hour_year(self, company_id: int, run_id: int, period: int, year: int) -> bytes:
         """
         Get HR Document: Employer Cost per Hour per company per period.
 
         For further details, see the official documentation:
             [HrDocuments_EmployerCostPerHour_Year](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=HrDocuments_EmployerCostPerHour_Year)
 
         Args:
             company_id (int): The ID of the company.
             run_id (int): The ID of the run.
-            year (int): The year.
             period (int): The period.
+            year (int): The year.
 
         Returns:
             bytes: The HR document as base64Binary.
         """
         response = self.client.service.HrDocuments_EmployerCostPerHour_Year(
-            CompanyId=company_id, RunId=run_id, Year=year, Period=period, _soapheaders=self.auth_header
+            CompanyId=company_id, RunId=run_id, Year=year, Period=period, _soapheaders=self.auth_manager.header
         )
         return response
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/salary_document.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/salary_document.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # pylint: disable=line-too-long
 """Microservice responsible for salary documents related actions on the company level."""
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class CompanySalaryDocumentService(MicroService):
     """Microservice responsible for salary documents related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="CompanyService:SalaryDocuments_AnnualDocument_AnualStatement")
     def get_annual_statement(self):
         """
         Get Annual Statement in PDF.
 
         For more information, refer to the official documentation:
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/salary_table.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/salary_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Microservice responsible for salary table related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import SalaryTable, SalaryTableScale, SalaryTableStep
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class CompanySalaryTableService(MicroService):
     """Microservice responsible for salary table related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:SalaryTable_Get")
     def get(self, company_id: int, period: int, year: int) -> list[SalaryTable]:
         """
         Returns a list of available tables for the company.
 
@@ -31,15 +29,17 @@
             company_id (int): The ID of the company.
             period (int): Period.
             year (int): Year.
 
         Returns:
             list[SalaryTable]: A list of salary table objects.
         """
-        salary_tables = self.client.service.SalaryTable_Get(CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header)
+        salary_tables = self.client.service.SalaryTable_Get(
+            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
+        )
         return [SalaryTable(company_id=company_id, data=salary_table) for salary_table in serialize_object(salary_tables)]
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:SalaryTable2_Get")
     def get_2(self, company_id: int, period: int, year: int) -> list[str]:
         """
         Returns a list of available tables for the company with unique identifiers.
@@ -51,15 +51,17 @@
             company_id (int): The ID of the company.
             period (int): Period.
             year (int): Year.
 
         Returns:
             list[str]: A list of salary table guids.
         """
-        salary_tables = self.client.service.SalaryTable2_Get(CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header)
+        salary_tables = self.client.service.SalaryTable2_Get(
+            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
+        )
         return [salary_table.get("GuidSalaryTable") for salary_table in serialize_object(salary_tables)]
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:SalaryTable_GetScales")
     def get_scale(self, company_id: int, period: int, year: int) -> list[SalaryTableScale]:
         """
         Returns a list of available scales for the company salary table.
@@ -71,15 +73,17 @@
             company_id (int): The ID of the company.
             period (int): Period.
             year (int): Year.
 
         Returns:
             list[SalaryTableScale]: A list of salary table scale objects.
         """
-        scales = self.client.service.SalaryTable_GetScales(CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header)
+        scales = self.client.service.SalaryTable_GetScales(
+            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
+        )
         return [SalaryTableScale(company_id=company_id, data=scale) for scale in serialize_object(scales)]
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:SalaryTable2_GetScales")
     def get_scale_2(self, company_id: int, period: int, year: int) -> list[str]:
         """
         Returns a list of available scales for the company salary table with unique identifiers.
@@ -92,15 +96,15 @@
             period (int): Period.
             year (int): Year.
 
         Returns:
             list[str]: A list of salary table scale guids.
         """
         salary_tables = self.client.service.SalaryTable2_GetScales(
-            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header
+            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
         )
         return [salary_table.get("GuidSalaryTableScale") for salary_table in serialize_object(salary_tables)]
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:SalaryTable_GetSteps")
     def get_step(self, company_id: int, period: int, year: int, scale: SalaryTableScale) -> list[SalaryTableStep]:
         """
@@ -122,15 +126,15 @@
             "Scale": scale.scale,
             "SchaalDescription": scale.description,
             "ScaleValue": scale.value,
             "ScalePercentageMax": scale.percentage_max,
             "ScalePercentageMin": scale.percentage_min,
         }
         steps = self.client.service.SalaryTable_GetSteps(
-            CompanyId=company_id, Period=period, Year=year, Scale=_scale, _soapheaders=self.auth_header
+            CompanyId=company_id, Period=period, Year=year, Scale=_scale, _soapheaders=self.auth_manager.header
         )
         return [SalaryTableStep(company_id=company_id, data=step) for step in serialize_object(steps)]
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:SalaryTable2_GetSteps")
     def get_step_2(self, company_id: int, period: int, year: int) -> list[str]:
         """
@@ -144,10 +148,10 @@
             period (int): Period.
             year (int): Year.
 
         Returns:
             list[str]: A list of salary table step guids.
         """
         salary_tables = self.client.service.SalaryTable2_GetSteps(
-            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header
+            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
         )
         return [salary_table.get("GuidSalaryTableStep") for salary_table in serialize_object(salary_tables)]
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/svw.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/svw.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Microservice responsible for svw related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import SVW
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class CompanySvwService(MicroService):
     """Microservice responsible for svw related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="CompanyService:SVW_GetCurrent")
     def get_current(self, company_id: int) -> SVW:
         """
         Get the current SVW settings.
 
         For more information, refer to the official documentation:
@@ -27,26 +25,26 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             SVW: object representing svw settings
         """
-        svw = self.client.service.SVW_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
+        svw = self.client.service.SVW_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         return SVW(company_id=company_id, data=serialize_object(svw))
 
     @nmbrs_exception_handler(resource="CompanyService:SVW_UpdateCurrent")
-    def insert_current(self, company_id: int, svw: SVW) -> None:
+    def post_current(self, company_id: int, svw: SVW) -> None:
         """
         Update the current SVW settings.
 
         For more information, refer to the official documentation:
             [SVW_UpdateCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=SVW_UpdateCurrent)
 
         Args:
             company_id (int): The ID of the company.
             svw (SWV): Object containing svw data.
 
         Returns:
             SVW: object representing svw settings
         """
-        self.client.service.SVW_UpdateCurrent(CompanyId=company_id, SVW=svw.insert_dict(), _soapheaders=self.auth_header)
+        self.client.service.SVW_UpdateCurrent(CompanyId=company_id, SVW=svw.insert_dict(), _soapheaders=self.auth_manager.header)
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/wage_component.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """Microservice responsible for wage component related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import WageComponent
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class CompanyWageComponentService(MicroService):
     """Microservice responsible for wage component related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:WageComponentFixed_Get")
-    def fixed_get(self, company_id: int, year: int, period: int) -> list[WageComponent]:
+    def get_fixed(self, company_id: int, year: int, period: int) -> list[WageComponent]:
         """
         Retrieve all fixed wage components for a specified company, year, and period.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentFixed_Get)
 
         Args:
@@ -32,46 +30,46 @@
             year (int): The year.
             period (int): The period.
 
         Returns:
             list[WageComponent]: A list of fixed wage components.
         """
         wage_components = self.client.service.WageComponentFixed_Get(
-            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header
+            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
         )
         wage_components = [
             WageComponent(company_id=company_id, component_type="fixed", data=wage_component)
             for wage_component in serialize_object(wage_components)
         ]
         return wage_components
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:WageComponentFixed_GetCurrent")
-    def fixed_get_current(self, company_id: int):
+    def get_current_fixed(self, company_id: int):
         """
         Retrieve all fixed wage components for the current period of a specified company.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentFixed_GetCurrent)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[WageComponent]: A list of fixed wage components for the current period.
         """
-        wage_components = self.client.service.WageComponentFixed_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
+        wage_components = self.client.service.WageComponentFixed_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         wage_components = [
             WageComponent(company_id=company_id, component_type="fixed", data=wage_component)
             for wage_component in serialize_object(wage_components)
         ]
         return wage_components
 
     @nmbrs_exception_handler(resource="CompanyService:WageComponentFixed_Insert")
-    def fixed_insert(
+    def post_fixed(
         self,
         wage_component: WageComponent,
         period: int,
         year: int,
         protected_mode: bool,
     ) -> int:
         """
@@ -92,41 +90,41 @@
         new_wage_component = {"Id": wage_component.id, "Code": wage_component.code, "Value": wage_component.value}
         response = self.client.service.WageComponentFixed_Insert(
             CompanyId=wage_component.company_id,
             WageComponent=new_wage_component,
             Period=period,
             Year=year,
             UnprotectedMode=protected_mode,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="CompanyService:WageComponentFixed_InsertCurrent")
-    def fixed_insert_current(self, wage_component: WageComponent) -> int:
+    def post_current_fixed(self, wage_component: WageComponent) -> int:
         """
         Insert a fixed wage component for the current period of a specified company.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_InsertCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentFixed_InsertCurrent)
 
         Args:
             wage_component (WageComponent): The fixed wage component to insert.
 
         Returns:
             int: The ID of the inserted fixed wage component.
         """
         new_wage_component = {"Id": wage_component.id, "Code": wage_component.code, "Value": wage_component.value}
         response = self.client.service.WageComponentFixed_InsertCurrent(
-            CompanyId=wage_component.company_id, WageComponent=new_wage_component, _soapheaders=self.auth_header
+            CompanyId=wage_component.company_id, WageComponent=new_wage_component, _soapheaders=self.auth_manager.header
         )
         return response
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:WageComponentFixed_Insert_Batch")
-    def fixed_insert_batch(
+    def post_batch_fixed(
         self,
         wage_components: list[WageComponent],
         period: int,
         year: int,
         protected_mode: bool,
     ) -> list[int]:
         """
@@ -151,20 +149,24 @@
                     "CompanyId": wage_component.company_id,
                     "Id": wage_component.id,
                     "Code": wage_component.code,
                     "Value": wage_component.value,
                 }
             )
         response = self.client.service.WageComponentFixed_Insert_Batch(
-            WageComponents=new_wage_components, Period=period, Year=year, UnprotectedMode=protected_mode, _soapheaders=self.auth_header
+            WageComponents=new_wage_components,
+            Period=period,
+            Year=year,
+            UnprotectedMode=protected_mode,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="CompanyService:WageComponentFixed_Stop")
-    def fixed_stop(
+    def stop_fixed(
         self,
         company_id: int,
         component_id: int,
         period: int,
         year: int,
         protected_mode: bool,
     ) -> None:
@@ -186,67 +188,67 @@
         """
         self.client.service.WageComponentFixed_Stop(
             CompanyId=company_id,
             WageComponentId=component_id,
             Period=period,
             Year=year,
             UnprotectedMode=protected_mode,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_Get")
-    def variable_get(self, company_id: int, year: int, period: int) -> list[WageComponent]:
+    def get_variable(self, company_id: int, period: int, year: int) -> list[WageComponent]:
         """
         Retrieve all variable wage components for a specified company, year, and period.
 
         For more information, refer to the official documentation:
             [WageComponentVar_Get](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_Get)
 
         Args:
             company_id (int): The ID of the company.
-            year (int): The year.
             period (int): The period.
+            year (int): The year.
 
         Returns:
             list[WageComponent]: A list of variable wage components.
         """
         wage_components = self.client.service.WageComponentVar_Get(
-            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header
+            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
         )
         wage_components = [
             WageComponent(company_id=company_id, component_type="variable", data=wage_component)
             for wage_component in serialize_object(wage_components)
         ]
         return wage_components
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_GetCurrent")
-    def variable_get_current(self, company_id: int) -> list[WageComponent]:
+    def get_current_variable(self, company_id: int) -> list[WageComponent]:
         """
         Retrieve all variable wage components for the current period of a specified company.
 
         For more information, refer to the official documentation:
             [WageComponentVar_GetCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_GetCurrent)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[WageComponent]: A list of variable wage components for the current period.
         """
-        wage_components = self.client.service.WageComponentVar_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_header)
+        wage_components = self.client.service.WageComponentVar_GetCurrent(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         wage_components = [
             WageComponent(company_id=company_id, component_type="variable", data=wage_component)
             for wage_component in serialize_object(wage_components)
         ]
         return wage_components
 
     @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_Insert")
-    def variable_insert(
+    def post_variable(
         self,
         wage_component: WageComponent,
         period: int,
         year: int,
         protected_mode: bool,
     ) -> int:
         """
@@ -267,41 +269,41 @@
         new_wage_component = {"Id": wage_component.id, "Code": wage_component.code, "Value": wage_component.value}
         response = self.client.service.WageComponentVar_Insert(
             CompanyId=wage_component.company_id,
             WageComponent=new_wage_component,
             Period=period,
             Year=year,
             UnprotectedMode=protected_mode,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_InsertCurrent")
-    def variable_insert_current(self, wage_component: WageComponent) -> int:
+    def post_current_variable(self, wage_component: WageComponent) -> int:
         """
         Insert a variable wage component for the current period of a specified company.
 
         For more information, refer to the official documentation:
             [WageComponentVar_InsertCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_InsertCurrent)
 
         Args:
             wage_component (WageComponent): The variable wage component to insert.
 
         Returns:
             int: The ID of the inserted variable wage component.
         """
         new_wage_component = {"Id": wage_component.id, "Code": wage_component.code, "Value": wage_component.value}
         response = self.client.service.WageComponentVar_InsertCurrent(
-            CompanyId=wage_component.company_id, WageComponent=new_wage_component, _soapheaders=self.auth_header
+            CompanyId=wage_component.company_id, WageComponent=new_wage_component, _soapheaders=self.auth_manager.header
         )
         return response
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_Insert_Batch")
-    def variable_insert_batch(
+    def post_batch_variable(
         self,
         wage_components: list[WageComponent],
         period: int,
         year: int,
         protected_mode: bool,
     ) -> list[int]:
         """
@@ -326,20 +328,24 @@
                     "CompanyId": wage_component.company_id,
                     "Id": wage_component.id,
                     "Code": wage_component.code,
                     "Value": wage_component.value,
                 }
             )
         response = self.client.service.WageComponentVar_Insert_Batch(
-            WageComponents=new_wage_components, Period=period, Year=year, UnprotectedMode=protected_mode, _soapheaders=self.auth_header
+            WageComponents=new_wage_components,
+            Period=period,
+            Year=year,
+            UnprotectedMode=protected_mode,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_Clear")
-    def variable_clear(
+    def clear_variable(
         self,
         company_id: int,
         period: int,
         year: int,
         protected_mode: bool,
     ) -> list[int]:
         """
@@ -358,30 +364,30 @@
             list[int]: The IDs of the cleared variable wage components.
         """
         response = self.client.service.WageComponentVar_Clear(
             CompanyId=company_id,
             Period=period,
             Year=year,
             UnprotectedMode=protected_mode,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="CompanyService:WageComponentVar_ClearCurrent")
-    def variable_clear_current(self, company_id: int) -> list[int]:
+    def clear_current_variable(self, company_id: int) -> list[int]:
         """
         Clear all variable wage components for the current period of a specified company.
 
         For more information, refer to the official documentation:
             [WageComponentVar_ClearCurrent](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageComponentVar_ClearCurrent)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[int]: The IDs of the cleared variable wage components.
         """
         response = self.client.service.WageComponentVar_ClearCurrent(
             CompanyId=company_id,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/wage_cost.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_cost.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Microservice responsible for managing wage cost related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import WageCost
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class CompanyWageCostService(MicroService):
     """Microservice responsible for managing wage cost related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:WorkCost_GetList")
     def get(self, company_id: int, year: int) -> list[WageCost]:
         """
         Retrieve the list of work cost values for a given company and year.
 
@@ -30,20 +28,20 @@
         Args:
             company_id (int): The ID of the company.
             year (int): The year.
 
         Returns:
             list[WageCost]: A list of work cost values.
         """
-        wage_costs = self.client.service.WorkCost_GetList(CompanyId=company_id, Year=year, _soapheaders=self.auth_header)
+        wage_costs = self.client.service.WorkCost_GetList(CompanyId=company_id, Year=year, _soapheaders=self.auth_manager.header)
         wage_costs = [WageCost(company_id=company_id, data=wage_cost) for wage_cost in serialize_object(wage_costs)]
         return wage_costs
 
     @nmbrs_exception_handler(resource="CompanyService:WorkCost_Insert")
-    def insert(self, company_id: int, value: float, period: int, year: int):
+    def post(self, company_id: int, value: float, period: int, year: int):
         """
         Insert a work cost value from the financial administration for a specific period.
 
         For more information, refer to the official documentation:
             [WorkCost_Insert](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WorkCost_Insert)
 
         Args:
@@ -56,10 +54,10 @@
             int: The response indicating the success of the operation.
         """
         response = self.client.service.WorkCost_Insert(
             CompanyId=company_id,
             Value=value,
             Period=period,
             Year=year,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/wage_model.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 """Microservice responsible for managing wage model related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import WageModel
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class CompanyWageModelService(MicroService):
     """Microservice responsible for managing wage model related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:WageModel_GetWageCodes")
-    def get(self, company_id: int) -> list[WageModel]:
+    def get_current(self, company_id: int) -> list[WageModel]:
         """
         Retrieve the list of wage codes belonging to a company's wage model.
 
         For more information, refer to the official documentation:
             [WageModel_GetWageCodes](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageModel_GetWageCodes)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[WageModel]: A list of wage codes belonging to the company's wage model.
         """
-        wage_models = self.client.service.WageModel_GetWageCodes(CompanyId=company_id, _soapheaders=self.auth_header)
+        wage_models = self.client.service.WageModel_GetWageCodes(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         wage_models = [WageModel(company_id=company_id, data=wage_model) for wage_model in serialize_object(wage_models)]
         return wage_models
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:WageModel2_GetWageCodes")
-    def get_2(self, company_id: int) -> list[WageModel]:
+    def get_current_2(self, company_id: int) -> list[WageModel]:
         """
         Retrieve the list of wage codes belonging to a company's wage model.
 
         For more information, refer to the official documentation:
             [WageModel2_GetWageCodes](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=WageModel2_GetWageCodes)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[WageModel]: A list of wage codes belonging to the company's wage model.
         """
-        wage_models = self.client.service.WageModel2_GetWageCodes(CompanyId=company_id, _soapheaders=self.auth_header)
+        wage_models = self.client.service.WageModel2_GetWageCodes(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         wage_models = [WageModel(company_id=company_id, data=wage_model) for wage_model in serialize_object(wage_models)]
         return wage_models
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/company/wage_tax.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/company/wage_tax.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Microservice responsible for managing wage tax-related actions on the company level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
+from ....auth.token_manager import AuthManager
 from ....data_classes.company import WageTax, WageTaxXML
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class CompanyWageTaxService(MicroService):
     """Microservice responsible for managing wage tax-related actions on the company level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:WageTax_GetList")
     def get_all_wagetax(self, company_id: int, year: int) -> list[WageTax]:
         """
         Retrieve all wage taxes for a specific company and year.
 
@@ -30,15 +28,15 @@
         Args:
             company_id (int): The ID of the company.
             year (int): The year for which wage taxes are retrieved.
 
         Returns:
             list[WageTax]: A list of WageTax objects for the specified company and year.
         """
-        wage_taxes = self.client.service.WageTax_GetList(CompanyId=company_id, intYear=year, _soapheaders=self.auth_header)
+        wage_taxes = self.client.service.WageTax_GetList(CompanyId=company_id, intYear=year, _soapheaders=self.auth_manager.header)
         wage_taxes = [WageTax(company_id=company_id, data=wage_tax) for wage_tax in serialize_object(wage_taxes)]
         return wage_taxes
 
     @nmbrs_exception_handler(resource="CompanyService:WageTax_GetXML")
     def get_wagetax_details(self, company_id: int, loonaangifte_id: int) -> WageTaxXML:
         """
         Retrieve wage tax details for a specific company and loonaangifte ID.
@@ -52,15 +50,15 @@
 
         Returns:
             WageTaxXML: An wage tax object detailing the specified company and loonaangifte ID.
         """
         wage_tax_details = self.client.service.WageTax_GetXML(
             CompanyId=company_id,
             LoonaangifteID=loonaangifte_id,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         wage_tax_details = WageTaxXML(wage_tax_details)
         return wage_tax_details
 
     @nmbrs_exception_handler(resource="CompanyService:WageTax_SetSentExternal")
     def set_send_as_external(self, company_id: int, loonaangifte_id: int) -> bool:
         """
@@ -75,10 +73,10 @@
 
         Returns:
             bool: A boolean indicating if the wage tax was send externally.
         """
         response = self.client.service.WageTax_SetSentExternal(
             CompanyId=company_id,
             LoonaangifteID=loonaangifte_id,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/debtor/department.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/department.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 """Microservice responsible for department related actions on the debtor level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
+from ....auth.token_manager import AuthManager
 from ....data_classes.debtor import Department
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class DebtorDepartmentService(MicroService):
     """Microservice responsible for department related actions on the debtor level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="DebtorService:Department_Delete")
     def delete(self, debtor_id: int, department_id: int) -> None:
         """
         Delete a department of a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Department_Delete](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Department_Delete)
 
         Args:
             debtor_id (int): The ID of the debtor.
             department_id (int): The ID of the department to delete.
         """
-        self.client.service.Department_Delete(DebtorId=debtor_id, id=department_id, _soapheaders=self.auth_header)
+        self.client.service.Department_Delete(DebtorId=debtor_id, id=department_id, _soapheaders=self.auth_manager.header)
 
     @return_list
     @nmbrs_exception_handler(resource="DebtorService:Department_GetList")
     def get_all(self, debtor_id: int) -> list[Department]:
         """
         Retrieve all departments of a debtor.
 
@@ -43,20 +41,20 @@
 
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             list[Department]: A list of Department objects representing all departments of the debtor.
         """
-        departments = self.client.service.Department_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        departments = self.client.service.Department_GetList(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         departments = [Department(debtor_id=debtor_id, data=department) for department in serialize_object(departments)]
         return departments
 
     @nmbrs_exception_handler(resource="DebtorService:Department_Insert")
-    def insert(self, debtor_id: int, department_id: int, code: int, description: str) -> int:
+    def post(self, debtor_id: int, department_id: int, code: int, description: str) -> int:
         """
         Insert a new department for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Department_Insert](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Department_Insert)
 
         Args:
@@ -72,15 +70,15 @@
             "DebtorId": debtor_id,
             "department": {
                 "Id": department_id,
                 "Code": code,
                 "Description": description,
             },
         }
-        inserted = self.client.service.Department_Insert(**data, _soapheaders=self.auth_header)
+        inserted = self.client.service.Department_Insert(**data, _soapheaders=self.auth_manager.header)
         return inserted
 
     @nmbrs_exception_handler(resource="DebtorService:Department_Update")
     def update(self, debtor_id: int, department_id: int, code: int, description: str) -> None:
         """
         Update an existing department of a debtor.
 
@@ -97,8 +95,8 @@
             "DebtorId": debtor_id,
             "department": {
                 "Id": department_id,
                 "Code": code,
                 "Description": description,
             },
         }
-        self.client.service.Department_Update(**data, _soapheaders=self.auth_header)
+        self.client.service.Department_Update(**data, _soapheaders=self.auth_manager.header)
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/debtor/function.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/function.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 """Microservice responsible for function related actions on the debtor level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
+from ....auth.token_manager import AuthManager
 from ....data_classes.debtor import Function
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class DebtorFunctionService(MicroService):
     """Microservice responsible for function related actions on the debtor level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="DebtorService:Function_Delete")
     def delete(self, debtor_id: int, function_id: int) -> None:
         """
         Delete a function of a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Function_Delete](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Function_Delete)
 
         Args:
             debtor_id (int): The ID of the debtor.
             function_id (int): The ID of the function to be deleted.
         """
-        self.client.service.Function_Delete(DebtorId=debtor_id, id=function_id, _soapheaders=self.auth_header)
+        self.client.service.Function_Delete(DebtorId=debtor_id, id=function_id, _soapheaders=self.auth_manager.header)
 
     @return_list
     @nmbrs_exception_handler(resource="DebtorService:Function_GetList")
     def get_all(self, debtor_id: int) -> list[Function]:
         """
         Retrieve all functions of a debtor.
 
@@ -44,20 +42,20 @@
         Args:
             debtor_id (int): The ID of the debtor.
             function_id (int): The ID of the function.
 
         Returns:
             list[Function]: A list of Function objects representing all functions of the debtor.
         """
-        functions = self.client.service.Function_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        functions = self.client.service.Function_GetList(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         functions = [Function(debtor_id=debtor_id, data=function) for function in serialize_object(functions)]
         return functions
 
     @nmbrs_exception_handler(resource="DebtorService:Function_Insert")
-    def insert(self, debtor_id: int, function_id: int, code: int, description: str) -> int:
+    def post(self, debtor_id: int, function_id: int, code: int, description: str) -> int:
         """
         Insert a new function for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Function_Insert](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Function_Insert)
 
         Args:
@@ -69,15 +67,15 @@
         Returns:
             int: The ID of the inserted function if successful.
         """
         data = {
             "DebtorId": debtor_id,
             "function": {"Id": function_id, "Code": code, "Description": description},
         }
-        inserted = self.client.service.Function_Insert(**data, _soapheaders=self.auth_header)
+        inserted = self.client.service.Function_Insert(**data, _soapheaders=self.auth_manager.header)
         return inserted
 
     @nmbrs_exception_handler(resource="DebtorService:Function_Update")
     def update(self, debtor_id: int, function_id: int, code: int, description: str) -> None:
         """
         Update a function for a debtor.
 
@@ -90,8 +88,8 @@
             code (int): The code of the function.
             description (str): The description of the function.
         """
         data = {
             "DebtorId": debtor_id,
             "function": {"Id": function_id, "Code": code, "Description": description},
         }
-        self.client.service.Function_Update(**data, _soapheaders=self.auth_header)
+        self.client.service.Function_Update(**data, _soapheaders=self.auth_manager.header)
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/debtor/title.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/title.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Microservice responsible for title related actions on the debtor level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class DebtorTitleService(MicroService):
     """Microservice responsible for title related actions on the debtor level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="DebtorService:Title_GetList")
     def get_all(self, debtor_id: int) -> list[str]:
         """
         Retrieve all titles for a debtor.
 
@@ -28,25 +26,25 @@
 
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             list[str]: A list of strings representing all titles associated with the debtor.
         """
-        titles = self.client.service.Title_GetList(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        titles = self.client.service.Title_GetList(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         titles = [title["TitleName"] for title in serialize_object(titles)]
         return titles
 
     @nmbrs_exception_handler(resource="DebtorService:Title_Insert")
-    def insert(self, debtor_id: int, title: str) -> None:
+    def post(self, debtor_id: int, title: str) -> None:
         """
         Insert a title for a debtor.
 
         For more information, refer to the official documentation:
             [Soap call Title_Insert](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=Title_Insert)
 
         Args:
             debtor_id (int): The ID of the debtor.
             title (str): The title to be inserted.
         """
         data = {"DebtorId": debtor_id, "title": {"TitleName": title}}
-        self.client.service.Title_Insert(**data, _soapheaders=self.auth_header)
+        self.client.service.Title_Insert(**data, _soapheaders=self.auth_manager.header)
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/debtor/webook.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/debtor/webook.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Microservice responsible for webhooks related actions on the debtor level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
+from ....auth.token_manager import AuthManager
 from ....data_classes.debtor import WebhookSetting, Event
 from ..micro_service import MicroService
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class DebtorWebHooksService(MicroService):
     """Microservice responsible for webhooks related actions on the debtor level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="DebtorService:WebhookSettings_Delete")
     def delete(self, debtor_id: int, webhook_id: int) -> bool:
         """
         Delete a webhook for a debtor.
 
         For more information, refer to the official documentation:
@@ -32,15 +30,15 @@
 
         Returns:
             bool: True if the webhook is successfully deleted, otherwise False.
         """
         deleted = self.client.service.WebhookSettings_Delete(
             DebtorId=debtor_id,
             WebhookSettingId=webhook_id,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return deleted
 
     @return_list
     @nmbrs_exception_handler(resource="DebtorService:WebhookSettings_Get")
     def get_all(self, debtor_id: int) -> list[WebhookSetting]:
         """
@@ -51,15 +49,15 @@
 
         Args:
             debtor_id (int): The ID of the debtor.
 
         Returns:
             list[WebhookSetting]: A list of WebhookSetting objects representing all webhooks associated with the debtor.
         """
-        webhooks = self.client.service.WebhookSettings_Get(DebtorId=debtor_id, _soapheaders=self.auth_header)
+        webhooks = self.client.service.WebhookSettings_Get(DebtorId=debtor_id, _soapheaders=self.auth_manager.header)
         webhooks = [WebhookSetting(debtor_id=debtor_id, data=webhook) for webhook in serialize_object(webhooks)]
         return webhooks
 
     @return_list
     @nmbrs_exception_handler(resource="DebtorService:WebhookSettings_GetEvents")
     def get_all_events(self) -> list[Event]:
         """
@@ -67,15 +65,15 @@
 
         For more information, refer to the official documentation:
             [Soap call WebhookSettings_GetEvents](https://api.nmbrs.nl/soap/v3/DebtorService.asmx?op=WebhookSettings_GetEvents)
 
         Returns:
             list[Event]: A list of Event objects representing all webhook events.
         """
-        events = self.client.service.WebhookSettings_GetEvents(_soapheaders=self.auth_header)
+        events = self.client.service.WebhookSettings_GetEvents(_soapheaders=self.auth_manager.header)
         events = [Event(event) for event in serialize_object(events)]
         return events
 
     @nmbrs_exception_handler(resource="DebtorService:WebhookSettings_Insert")
     def insert(self, debtor_id: int, insert_webhook_settings: WebhookSetting) -> int:
         """
         Insert a webhook for a debtor.
@@ -90,9 +88,9 @@
         Returns:
             int: The ID of the inserted webhook.
         """
         data = {
             "DebtorId": debtor_id,
             "WebhookSetting": insert_webhook_settings.to_insert_dict(),
         }
-        inserted = self.client.service.WebhookSettings_Insert(**data, _soapheaders=self.auth_header)
+        inserted = self.client.service.WebhookSettings_Insert(**data, _soapheaders=self.auth_manager.header)
         return inserted
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/__init__.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/absence.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/absence.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,62 +2,60 @@
 
 from datetime import datetime
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Absence
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeeAbsenceService(MicroService):
     """Microservice responsible for absence related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:Absence_GetList")
-    def get(self, employee_id: int) -> list[Absence]:
+    def get_current(self, employee_id: int) -> list[Absence]:
         """
         Get a list of all absences.
 
         For more information, refer to the official documentation:
             [Absence_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_GetList)
 
         Args:
             employee_id (int): The ID of the employee.
 
         Returns:
             list[Absence]: A list of Absence objects representing the absences.
         """
-        absences = self.client.service.Absence_GetList(EmployeeId=employee_id, _soapheaders=self.auth_header)
+        absences = self.client.service.Absence_GetList(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
         return [Absence(employee_id=employee_id, data=absence) for absence in serialize_object(absences)]
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:Absence2_GetList")
-    def get_2(self, employee_id: int) -> list[Absence]:
+    def get_current_2(self, employee_id: int) -> list[Absence]:
         """
         Get a list of all absences with their respective cause.
 
         For more information, refer to the official documentation:
             [Absence2_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence2_GetList)
 
         Args:
             employee_id (int): The ID of the employee.
 
         Returns:
             list[Absence]: A list of Absence objects representing the absences.
         """
-        absences = self.client.service.Absence2_GetList(EmployeeId=employee_id, _soapheaders=self.auth_header)
+        absences = self.client.service.Absence2_GetList(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
         return [Absence(employee_id=employee_id, data=absence) for absence in serialize_object(absences)]
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:Absence_GetAll_AllEmployeesByCompany")
     def get_all_by_company(self, company_id: int) -> list[Absence]:
         """
         Get a list of all absence of all company employees.
@@ -67,23 +65,23 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[Absence]: A list of Absence objects representing the absences.
         """
-        absences = self.client.service.Absence_GetAll_AllEmployeesByCompany(CompanyId=company_id, _soapheaders=self.auth_header)
+        absences = self.client.service.Absence_GetAll_AllEmployeesByCompany(CompanyId=company_id, _soapheaders=self.auth_manager.header)
 
         _absences = []
         for employee in serialize_object(absences):
             _absences.append(Absence(employee_id=employee["EmployeeId"], data=employee))
         return _absences
 
     @nmbrs_exception_handler(resource="EmployeeService:Absence_Insert")
-    def insert(self, employee_id: int, absence: Absence) -> int:
+    def post(self, employee_id: int, absence: Absence) -> int:
         """
         Insert an absence, this item will start from the given date in the object.
 
         For more information, refer to the official documentation:
             [Absence_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_Insert)
 
         Args:
@@ -100,19 +98,19 @@
             "Start": absence.start,
             "RegistrationStartDate": absence.registration_start_date,
             "End": absence.end,
             "RegistrationEndDate": absence.registration_end_date,
             "Dossier": absence.dossier,
             "Dossiernr": absence.dossier_number,
         }
-        response = self.client.service.Absence_Insert(EmployeeId=employee_id, Absence=_absence, _soapheaders=self.auth_header)
+        response = self.client.service.Absence_Insert(EmployeeId=employee_id, Absence=_absence, _soapheaders=self.auth_manager.header)
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:Absence2_Insert")
-    def insert_2(self, employee_id: int, absence: Absence) -> int:
+    def post_2(self, employee_id: int, absence: Absence) -> int:
         """
         Insert an absence with cause, this item will start from the given date in the object.
 
         For more information, refer to the official documentation:
             [Absence2_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence2_Insert)
 
         Args:
@@ -130,19 +128,19 @@
             "Start": absence.start,
             "RegistrationStartDate": absence.registration_start_date,
             "End": absence.end,
             "RegistrationEndDate": absence.registration_end_date,
             "Dossier": absence.dossier,
             "Dossiernr": absence.dossier_number,
         }
-        response = self.client.service.Absence2_Insert(EmployeeId=employee_id, Absence=_absence, _soapheaders=self.auth_header)
+        response = self.client.service.Absence2_Insert(EmployeeId=employee_id, Absence=_absence, _soapheaders=self.auth_manager.header)
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:Absence_PartialRecoveryInsert")
-    def insert_partial_recovery(
+    def post_partial_recovery(
         self, employee_id: int, absence_id: int, start_date: datetime, report_data: datetime, percentage: int, comment: str
     ) -> int:
         """
         Insert an absence partial recovery message.
 
         For more information, refer to the official documentation:
             [Absence_PartialRecoveryInsert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_PartialRecoveryInsert)
@@ -161,20 +159,20 @@
         response = self.client.service.Absence_PartialRecoveryInsert(
             EmployeeId=employee_id,
             AbsenceID=absence_id,
             StartDate=start_date,
             Reportdate=report_data,
             Percent=percentage,
             Comment=comment,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:Absence_RecoveryInsert")
-    def insert_recovery(self, employee_id: int, absence_id: int, last_day_absence: datetime, report_data: datetime, comment: str) -> str:
+    def post_recovery(self, employee_id: int, absence_id: int, last_day_absence: datetime, report_data: datetime, comment: str) -> str:
         """
         Insert an absence recovery message.
 
         For more information, refer to the official documentation:
             [Absence_RecoveryInsert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Absence_RecoveryInsert)
 
         Args:
@@ -189,20 +187,20 @@
         """
         response = self.client.service.Absence_RecoveryInsert(
             EmployeeId=employee_id,
             AbsenceID=absence_id,
             Lastdayabsence=last_day_absence,
             Reportdate=report_data,
             Comment=comment,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:AbsenceNotification_Insert")
-    def insert_notification(self, employee_id: int, absence: Absence) -> int:
+    def post_notification(self, employee_id: int, absence: Absence) -> int:
         """
         Insert a new absence date, this item will start from the given date in the object to the requested absence dossier.
 
         For more information, refer to the official documentation:
             [AbsenceNotification_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=AbsenceNotification_Insert)
 
         Args:
@@ -220,9 +218,11 @@
             "Start": absence.start,
             "RegistrationStartDate": absence.registration_start_date,
             "End": absence.end,
             "RegistrationEndDate": absence.registration_end_date,
             "Dossier": absence.dossier,
             "Dossiernr": absence.dossier_number,
         }
-        response = self.client.service.AbsenceNotification_Insert(EmployeeId=employee_id, Absence=_absence, _soapheaders=self.auth_header)
+        response = self.client.service.AbsenceNotification_Insert(
+            EmployeeId=employee_id, Absence=_absence, _soapheaders=self.auth_manager.header
+        )
         return response
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/address.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/address.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Microservice responsible for address related actions on the employee level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Address
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeeAddressService(MicroService):
     """Microservice responsible for address related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:Address_GetList")
     def get(self, employee_id: int, period: int, year: int) -> list[Address]:
         """
         Get all addresses which are active in given period.
 
@@ -31,15 +29,17 @@
             employee_id (int): The ID of the employee.
             period (int): The period.
             year (int): The year.
 
         Returns:
             list[Address]: A list of Address objects representing the addresses.
         """
-        addresses = self.client.service.Address_GetList(EmployeeId=employee_id, Period=period, Year=year, _soapheaders=self.auth_header)
+        addresses = self.client.service.Address_GetList(
+            EmployeeId=employee_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
+        )
         return [Address(employee_id=employee_id, data=address) for address in serialize_object(addresses)]
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:Address_GetListCurrent")
     def get_current(self, employee_id: int) -> list[Address]:
         """
         Get all currently active addresses.
@@ -49,15 +49,15 @@
 
         Args:
             employee_id (int): The ID of the employee.
 
         Returns:
             list[Address]: A list of Address objects representing the addresses.
         """
-        addresses = self.client.service.Address_GetListCurrent(EmployeeId=employee_id, _soapheaders=self.auth_header)
+        addresses = self.client.service.Address_GetListCurrent(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
         return [Address(employee_id=employee_id, data=address) for address in serialize_object(addresses)]
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:Address_GetAll_AllEmployeesByCompany")
     def get_all_by_company(self, company_id: int) -> list[Address]:
         """
         Get all addresses of all employees.
@@ -67,15 +67,15 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[Address]: A list of Address objects representing the addresses.
         """
-        addresses = self.client.service.Address_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_header)
+        addresses = self.client.service.Address_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_manager.header)
 
         _addresses = []
         for employee in serialize_object(addresses):
             for address in employee["EmployeeAddresses"]["EmployeeAddress_V2"]:
                 _addresses.append(Address(employee_id=employee["EmployeeId"], data=address))
         return _addresses
 
@@ -90,15 +90,15 @@
         Args:
             employee_id (int): The ID of the employee.
             address_id (int): The ID of the address.
 
         Returns:
             bool: A boolean indicating the success of the operation.
         """
-        response = self.client.service.Address_Delete(EmployeeId=employee_id, AddressID=address_id, _soapheaders=self.auth_header)
+        response = self.client.service.Address_Delete(EmployeeId=employee_id, AddressID=address_id, _soapheaders=self.auth_manager.header)
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:Address_Update")
     def update(self, employee_id: int, address: Address) -> bool:
         """
         Delete Employee Address.
 
@@ -120,19 +120,19 @@
             "HouseNumberAddition": address.house_number_addition,
             "PostalCode": address.postcode,
             "City": address.city,
             "StateProvince": address.state_province,
             "CountryISOCode": address.country_iso_code,
             "Type": address.type,
         }
-        response = self.client.service.Address_Update(EmployeeId=employee_id, Address=_address, _soapheaders=self.auth_header)
+        response = self.client.service.Address_Update(EmployeeId=employee_id, Address=_address, _soapheaders=self.auth_manager.header)
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:Address_Insert")
-    def insert(self, employee_id: int, address: Address, period: int, year: int, unprotected_mode: bool) -> int:
+    def post(self, employee_id: int, address: Address, period: int, year: int, unprotected_mode: bool) -> int:
         """
         Insert given address to the specified period. If the period is before the company's current period,
         unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Address_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_Insert)
 
@@ -160,20 +160,20 @@
         }
         response = self.client.service.Address_Insert(
             EmployeeId=employee_id,
             Address=_address,
             Period=period,
             Year=year,
             UnprotectedMode=unprotected_mode,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:Address_InsertCurrent")
-    def insert_current(self, employee_id: int, address: Address) -> int:
+    def post_current(self, employee_id: int, address: Address) -> int:
         """
         Insert given address to the current period.
 
         For more information, refer to the official documentation:
             [Address_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Address_InsertCurrent)
 
         Args:
@@ -191,9 +191,11 @@
             "HouseNumberAddition": address.house_number_addition,
             "PostalCode": address.postcode,
             "City": address.city,
             "StateProvince": address.state_province,
             "CountryISOCode": address.country_iso_code,
             "Type": address.type,
         }
-        response = self.client.service.Address_InsertCurrent(EmployeeId=employee_id, Address=_address, _soapheaders=self.auth_header)
+        response = self.client.service.Address_InsertCurrent(
+            EmployeeId=employee_id, Address=_address, _soapheaders=self.auth_manager.header
+        )
         return response
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/bank_account.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/bank_account.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Microservice responsible for bank account related actions on the employee level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.employee import BankAccount
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeeBankAccountService(MicroService):
     """Microservice responsible for bank account related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:BankAccount_GetList")
     def get(self, employee_id: int, period: int, year: int) -> list[BankAccount]:
         """
         Get all active bank accounts for given period.
 
@@ -32,15 +30,15 @@
             period (int): The period.
             year (int): The year.
 
         Returns:
             list[BankAccount]: A list of BankAccount objects representing the bank accounts.
         """
         bank_accounts = self.client.service.BankAccount_GetList(
-            EmployeeId=employee_id, Period=period, Year=year, _soapheaders=self.auth_header
+            EmployeeId=employee_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
         )
         return [BankAccount(employee_id=employee_id, data=bank_account) for bank_account in serialize_object(bank_accounts)]
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:BankAccount_GetListCurrent")
     def get_current(self, employee_id: int) -> list[BankAccount]:
         """
@@ -51,15 +49,15 @@
 
         Args:
             employee_id (int): The ID of the employee.
 
         Returns:
             list[BankAccount]: A list of BankAccount objects representing the bank accounts.
         """
-        bank_accounts = self.client.service.BankAccount_GetListCurrent(EmployeeId=employee_id, _soapheaders=self.auth_header)
+        bank_accounts = self.client.service.BankAccount_GetListCurrent(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
         return [BankAccount(employee_id=employee_id, data=bank_account) for bank_account in serialize_object(bank_accounts)]
 
     @nmbrs_exception_handler(resource="EmployeeService:BankAccount_DeleteCurrent")
     def delete(self, employee_id: int, bank_account_id: int) -> str:
         """
         Delete given bank account.
 
@@ -70,20 +68,20 @@
             employee_id (int): The ID of the employee.
             bank_account_id (int): The ID of the bank account.
 
         Returns:
             str: A str indicating the success of the operation.
         """
         response = self.client.service.BankAccount_DeleteCurrent(
-            EmployeeId=employee_id, BankAccountID=bank_account_id, _soapheaders=self.auth_header
+            EmployeeId=employee_id, BankAccountID=bank_account_id, _soapheaders=self.auth_manager.header
         )
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:BankAccount_Insert")
-    def insert(self, employee_id: int, bank_account: BankAccount, period: int, year: int, unprotected_mode: bool) -> int:
+    def post(self, employee_id: int, bank_account: BankAccount, period: int, year: int, unprotected_mode: bool) -> int:
         """
         Insert given bank account to the given period. Unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [BankAccount_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=BankAccount_Insert)
 
         Args:
@@ -108,20 +106,20 @@
         }
         response = self.client.service.BankAccount_Insert(
             EmployeeId=employee_id,
             BankAccount=_bank_account,
             Period=period,
             Year=year,
             UnprotectedMode=unprotected_mode,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:BankAccount_InsertCurrent")
-    def insert_current(self, employee_id: int, bank_account: BankAccount) -> int:
+    def post_current(self, employee_id: int, bank_account: BankAccount) -> int:
         """
         Insert given bank account to the current period.
 
         For more information, refer to the official documentation:
             [BankAccount_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=BankAccount_InsertCurrent)
 
         Args:
@@ -140,10 +138,10 @@
             "City": bank_account.city,
             "Name": bank_account.name,
             "Type": bank_account.type,
         }
         response = self.client.service.BankAccount_InsertCurrent(
             EmployeeId=employee_id,
             BankAccount=_bank_account,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/child.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/child.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 """Microservice responsible for child related actions on the employee level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Child
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeeChildService(MicroService):
     """Microservice responsible for child related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:Children_Get")
-    def get(self, employee_id: int) -> list[Child]:
+    def get_current(self, employee_id: int) -> list[Child]:
         """
         Get employee childs.
 
         For more information, refer to the official documentation:
             [Children_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Children_Get)
 
         Args:
             employee_id (int): The ID of the employee.
 
         Returns:
             list[Child]: A list of Child objects representing the children.
         """
-        children = self.client.service.Children_Get(EmployeeId=employee_id, _soapheaders=self.auth_header)
+        children = self.client.service.Children_Get(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
         children = serialize_object(children)
 
         _children = []
         for child in children["EmployeeChildren"]["Child"]:
             _children.append(Child(employee_id=children["EmployeeId"], data=child))
         return _children
 
@@ -52,15 +50,15 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[Child]: A list of Child objects representing the children.
         """
-        children = self.client.service.Children_GetAll_Employeesbycompany(CompanyId=company_id, _soapheaders=self.auth_header)
+        children = self.client.service.Children_GetAll_Employeesbycompany(CompanyId=company_id, _soapheaders=self.auth_manager.header)
 
         _children = []
         for employee in serialize_object(children):
             for child in employee["EmployeeChildren"]["Child"]:
                 _children.append(Child(employee_id=employee["EmployeeId"], data=child))
         return _children
 
@@ -75,19 +73,19 @@
         Args:
             employee_id (int): The ID of the employee.
             child_id (int): The ID of the child.
 
         Returns:
             str: The response indicating the success of the operation.
         """
-        response = self.client.service.Child_Delete(EmployeeId=employee_id, ChildId=child_id, _soapheaders=self.auth_header)
+        response = self.client.service.Child_Delete(EmployeeId=employee_id, ChildId=child_id, _soapheaders=self.auth_manager.header)
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:Children_Insert")
-    def insert(self, employee_id: int, child: Child) -> str:
+    def post(self, employee_id: int, child: Child) -> str:
         """
         Insert an employee child.
 
         For more information, refer to the official documentation:
             [Children_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Children_Insert)
 
         Args:
@@ -104,20 +102,20 @@
             "Initials": child.initials,
             "Gender": child.gender,
             "Birthday": child.birthday,
         }
         response = self.client.service.Children_Insert(
             EmployeeId=employee_id,
             child=_child,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:Children_InsertBatch")
-    def insert_batch(self, employee_id: int, children: list[Child]) -> str:
+    def post_batch(self, employee_id: int, children: list[Child]) -> str:
         """
         Insert employee children.
 
         For more information, refer to the official documentation:
             [Children_InsertBatch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Children_InsertBatch)
 
         Args:
@@ -138,15 +136,15 @@
                     "Gender": child.gender,
                     "Birthday": child.birthday,
                 }
             )
         response = self.client.service.Children_InsertBatch(
             EmployeeId=employee_id,
             children=_children,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:Children_Update")
     def update(self, employee_id: int, child: Child) -> str:
         """
         Update employee child.
@@ -168,10 +166,10 @@
             "Initials": child.initials,
             "Gender": child.gender,
             "Birthday": child.birthday,
         }
         response = self.client.service.Children_Update(
             EmployeeId=employee_id,
             child=_child,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/contract.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/contract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 """Microservice responsible for contract related actions on the employee level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Contract
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeeContractService(MicroService):
     """Microservice responsible for contract related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:Contract_GetAll")
-    def get_all(self, employee_id: int) -> list[Contract]:
+    def get(self, employee_id: int) -> list[Contract]:
         """
         Get all contracts for the specified employee.
 
         For more information, refer to the official documentation:
             [Contract_GetAll](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_GetAll)
 
         Args:
             employee_id (int): The ID of the employee.
 
         Returns:
             list[Contract]: A list of Contract objects representing the employees contracts.
         """
-        contracts = self.client.service.Contract_GetAll(EmployeeId=employee_id, _soapheaders=self.auth_header)
+        contracts = self.client.service.Contract_GetAll(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
         return [Contract(employee_id=employee_id, data=contract) for contract in serialize_object(contracts)]
 
     @nmbrs_exception_handler(resource="EmployeeService:Contract_GetCurrentPeriod")
     def get_current(self, employee_id: int) -> list[Contract]:
         """
         Get a list of all active contracts for specified employee in current period.
 
@@ -45,15 +43,15 @@
 
         Args:
             employee_id (int): The ID of the employee.
 
         Returns:
             list[Contract]: A list of Contract objects representing the employees contracts.
         """
-        contracts = self.client.service.Contract_GetCurrentPeriod(EmployeeId=employee_id, _soapheaders=self.auth_header)
+        contracts = self.client.service.Contract_GetCurrentPeriod(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
         contracts = serialize_object(contracts)
 
         _contracts = []
         for contract in contracts["EmployeeContracts"]["EmployeeContract"]:
             _contracts.append(Contract(employee_id=employee_id, data=contract))
 
         return _contracts
@@ -69,15 +67,15 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[Contract]: a list of contract objects
         """
-        contracts = self.client.service.Contract_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_header)
+        contracts = self.client.service.Contract_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_manager.header)
         contracts = serialize_object(contracts)
         _contracts = []
         for employee in contracts:
             for contract in employee["EmployeeContracts"]["EmployeeContract"]:
                 _contracts.append(Contract(employee_id=employee["EmployeeId"], data=contract))
         return _contracts
 
@@ -89,15 +87,15 @@
         For more information, refer to the official documentation:
             [Contract_Delete](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_Delete)
 
         Args:
             employee_id (int): The ID of the employee.
             contract_id (int): The ID of the contract.
         """
-        response = self.client.service.Contract_Delete(EmployeeId=employee_id, Id=contract_id, _soapheaders=self.auth_header)
+        response = self.client.service.Contract_Delete(EmployeeId=employee_id, Id=contract_id, _soapheaders=self.auth_manager.header)
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:Contract_Update")
     def update(self, employee_id: int, contract: Contract, unprotected_mode: bool):
         """
         Update the specified contract for specified employee. Contract start date can’t be updated, this field will be ignored.
 
@@ -122,20 +120,20 @@
             "WrittenContract": contract.written_contract,
             "HoursPerWeek": contract.hours_per_week,
         }
         response = self.client.service.Contract_Update(
             EmployeeId=employee_id,
             EmployeeContract=_contract,
             UnprotectedMode=unprotected_mode,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:Contract_Insert")
-    def insert(self, employee_id: int, contract: Contract, unprotected_mode: bool) -> int:
+    def post(self, employee_id: int, contract: Contract, unprotected_mode: bool) -> int:
         """
         Insert Contract. If the start date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Contract_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_Insert)
 
         Args:
@@ -159,20 +157,20 @@
             "WrittenContract": contract.written_contract,
             "HoursPerWeek": contract.hours_per_week,
         }
         response = self.client.service.Contract_Update(
             EmployeeId=employee_id,
             EmployeeContract=_contract,
             UnprotectedMode=unprotected_mode,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:Contract_InsertCurrentPeriod")
-    def insert_current(self, employee_id: int, contract: Contract, unprotected_mode: bool) -> int:
+    def post_current(self, employee_id: int, contract: Contract, unprotected_mode: bool) -> int:
         """
         Insert Contract in current period for specified employee.
 
         For more information, refer to the official documentation:
             [Contract_InsertCurrentPeriod](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Contract_InsertCurrentPeriod)
 
         Args:
@@ -196,10 +194,10 @@
             "WrittenContract": contract.written_contract,
             "HoursPerWeek": contract.hours_per_week,
         }
         response = self.client.service.Contract_Update(
             EmployeeId=employee_id,
             EmployeeContract=_contract,
             UnprotectedMode=unprotected_mode,
-            _soapheaders=self.auth_header,
+            _soapheaders=self.auth_manager.header,
         )
         return response
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/cost_center.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/cost_center.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,64 @@
 """Microservice responsible for cost center related actions on the employee level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.employee import CostCenter
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeeCostCenterService(MicroService):
     """Microservice responsible for cost center related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:CostCenter_Get")
-    def get(self):
+    def get(self, employee_id: int, period: int, year: int) -> list[CostCenter]:
         """
         Get all cost center per employee.
 
         For more information, refer to the official documentation:
             [CostCenter_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=CostCenter_Get)
+
+        Args:
+            employee_id (int): The ID of the employee.
+            period (int): The period.
+            year (int): The year.
+
+        Returns:
+            list[CostCenter]: a list of CostCenter objects
         """
-        raise NotImplementedError()  # pragma: no cover
+        cost_centers = self.client.service.CostCenter_Get(
+            EmployeeId=employee_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
+        )
+        cost_centers = [CostCenter(employee_id=employee_id, data=cost_center) for cost_center in serialize_object(cost_centers)]
+        return cost_centers
 
     @nmbrs_exception_handler(resource="EmployeeService:CostCenter_GetCurrent")
-    def get_current(self):
+    def get_current(self, employee_id: int) -> list[CostCenter]:
         """
         Get all active cost centers of a specific employee on the current period.
 
         For more information, refer to the official documentation:
             [CostCenter_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=CostCenter_GetCurrent)
+
+        Args:
+            employee_id (int): The ID of the employee.
+
+        Returns:
+            list[CostCenter]: a list of CostCenter objects
         """
-        raise NotImplementedError()  # pragma: no cover
+        cost_centers = self.client.service.CostCenter_GetCurrent(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
+        cost_centers = [CostCenter(employee_id=employee_id, data=cost_center) for cost_center in serialize_object(cost_centers)]
+        return cost_centers
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:CostCenter_GetAllEmployeesByCompany")
     def get_all_by_company(self, company_id: int, period: int, year: int) -> list[CostCenter]:
         """
         Get all cost centers of all employees per company.
 
@@ -52,15 +70,15 @@
             period (int): The period.
             year (int): The year.
 
         Returns:
             list[CostCenter]: a list of CostCenter objects
         """
         cost_centers = self.client.service.CostCenter_GetAllEmployeesByCompany(
-            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header
+            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
         )
         cost_centers = serialize_object(cost_centers)
         _cost_centers = []
         for employee in cost_centers:
             for cost_center in employee["CostCenters"]["EmployeeCostCenter"]:
                 _cost_centers.append(CostCenter(employee_id=employee["EmployeeId"], data=cost_center))
         return _cost_centers
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/days.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/days.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,137 +1,135 @@
 # pylint: disable=line-too-long
 """Microservice responsible for days related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class EmployeeDaysService(MicroService):
     """Microservice responsible for days related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:DaysFixed_Get")
-    def fixed_get(self):
+    def get_fixed(self):
         """
         Get fixed days worked for given period.
 
         For more information, refer to the official documentation:
             [DaysFixed_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysFixed_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:DaysFixed_GetCurrent")
-    def fixed_get_current(self):
+    def get_current_fixed(self):
         """
         Get fixed days worked for the current period.
 
         For more information, refer to the official documentation:
             [DaysFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysFixed_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:DaysFixed_Set")
-    def fixed_set(self):
+    def post_fixed(self):
         """
         Set fixed days for given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [DaysFixed_Set](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysFixed_Set)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:DaysFixed_SetCurrent")
-    def fixed_set_current(self):
+    def post_current_fixed(self):
         """
         Set fixed days worked for the current period.
 
         For more information, refer to the official documentation:
             [DaysFixed_SetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysFixed_SetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:DaysFixed_Set_Batch")
-    def fixed_set_batch(self):
+    def post_batch_fixed(self):
         """
         Set fixed days for given period for a batch of Employees. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [DaysFixed_Set_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysFixed_Set_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:DaysFixed_Stop")
-    def fixed_stop(self):
+    def stop_fixed(self):
         """
         Stop fixed days, the given period is the last for these days. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [DaysFixed_Stop](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysFixed_Stop)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:DaysVar_Get")
-    def variable_get(self):
+    def get_variable(self):
         """
         Get variable days worked for given period.
 
         For more information, refer to the official documentation:
             [DaysVar_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysVar_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:DaysVar_Set_Batch")
-    def variable_set_batch(self):
+    def post_batch_variable(self):
         """
         Set variable days for given period for a batch of Employees. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [DaysVar_Set_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysVar_Set_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:DaysVarWorked_Get")
-    def days_worked_get(self):
+    def get_days_worked(self):
         """
         Get days worked and +/- days for wage components per day filled in for given period.
 
         For more information, refer to the official documentation:
             [DaysVarWorked_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysVarWorked_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:DaysVarWorked_GetCurrent")
-    def days_worked_get_current(self):
+    def get_current_days_worked(self):
         """
         Get days worked and +/- days for wage components per day for the current period.
 
         For more information, refer to the official documentation:
             [DaysVarWorked_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysVarWorked_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:DaysVarWorked_Set")
-    def days_worked_set(self):
+    def post_days_worked(self):
         """
         Get days worked and +/- days for wage components per day for the current period.
 
         For more information, refer to the official documentation:
             [DaysVarWorked_Set](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysVarWorked_Set)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:DaysVarWorked_SetCurrent")
-    def days_worked_set_current(self):
+    def post_current_days_worked(self):
         """
         Set days worked and +/- days for wage components per day for the given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [DaysVarWorked_SetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=DaysVarWorked_SetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/department.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/department.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 # pylint: disable=line-too-long
 """Microservice responsible for departments related actions on the employee level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
-from ....data_classes.employee import Department
+from ....auth.token_manager import AuthManager
+from ....data_classes.employee import Department, DepartmentAll
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeeDepartmentsService(MicroService):
     """Microservice responsible for departments related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:Department_GetCurrent")
-    def get_current(self):
+    def get_current(self, employee_id: int) -> Department:
         """
         Get the currently active department.
 
         For more information, refer to the official documentation:
             [Department_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Department_GetCurrent)
+
+        Args:
+            employee_id (int): The ID of the employee.
+
+        Returns:
+            Department: The Department objects representing the department of the employee.
         """
-        raise NotImplementedError()  # pragma: no cover
+        department = self.client.service.Department_GetCurrent(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
+        return Department(employee_id=employee_id, data=serialize_object(department))
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:Department_GetAll_AllEmployeesByCompany")
-    def get_all_by_company(self, company_id: int) -> list[Department]:
+    def get_all_by_company(self, company_id: int) -> list[DepartmentAll]:
         """
         Get all department history of all employees.
 
         For more information, refer to the official documentation:
             [Department_GetAll_AllEmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Department_GetAll_AllEmployeesByCompany)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
-            list[Department]: a list of Department objects
+            list[DepartmentAll]: a list of Department objects
         """
-        departments = self.client.service.Department_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_header)
+        departments = self.client.service.Department_GetAll_AllEmployeesByCompany(
+            CompanyID=company_id, _soapheaders=self.auth_manager.header
+        )
         departments = serialize_object(departments)
         _departments = []
         for employee in departments:
             for department in employee["EmployeeDepartments"]["Department_V2"]:
-                _departments.append(Department(employee_id=employee["EmployeeId"], data=department))
+                _departments.append(DepartmentAll(employee_id=employee["EmployeeId"], data=department))
         return _departments
 
     @nmbrs_exception_handler(resource="EmployeeService:Department_UpdateCurrent")
     def update_current(self):
         """
         Update the department starting the current period.
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/document.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/document.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Microservice responsible for document related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class EmployeeDocumentService(MicroService):
     """Microservice responsible for document related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:EmployeeDocument_UploadDocument")
     def upload(self):
         """
         Uploads document for employee.
 
         For more information, refer to the official documentation:
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/employment.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/employment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # pylint: disable=line-too-long
 """Microservice responsible for employment related actions on the employee level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Employment
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeeEmploymentService(MicroService):
     """Microservice responsible for employment related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:Employment_GetAll_AllEmployeesByCompany")
     def get_all_by_company(self, company_id: int) -> list[Employment]:
         """
         Get all (historical) employment records for all employees that belong to the company.
 
@@ -30,15 +28,17 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[Employment]: a list of Employment objects
         """
-        employments = self.client.service.Employment_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_header)
+        employments = self.client.service.Employment_GetAll_AllEmployeesByCompany(
+            CompanyID=company_id, _soapheaders=self.auth_manager.header
+        )
         employments = serialize_object(employments)
         _employments = []
         for employee in employments:
             for employment in employee["EmployeeEmployments"]["Employment"]:
                 _employments.append(Employment(employee_id=employee["EmployeeId"], data=employment))
         return _employments
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/function.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/function.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,77 @@
 # pylint: disable=line-too-long
 """Microservice responsible for function related actions on the employee level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
-from ....data_classes.employee import Function
+from ....auth.token_manager import AuthManager
+from ....data_classes.employee import Function, FunctionAll
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeeFunctionService(MicroService):
     """Microservice responsible for function related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:Function_GetFunction")
     def get_by_id(self):
         """
         Get Function by functionID.
 
         For more information, refer to the official documentation:
             [Function_GetFunction](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Function_GetFunction)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:Function_GetCurrent")
-    def get_current(self):
+    def get_current(self, employee_id: int) -> Function:
         """
         Get the currently active function.
 
         For more information, refer to the official documentation:
             [Function_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Function_GetCurrent)
+
+        Args:
+            employee_id (int): The ID of the employee.
+
+        Returns:
+            Function: The Function objects representing the function of the employee.
         """
-        raise NotImplementedError()  # pragma: no cover
+        function = self.client.service.Function_GetCurrent(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
+        return Function(employee_id=employee_id, data=serialize_object(function))
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:Function_GetAll_AllEmployeesByCompany_V2")
-    def get_all_by_company(self, company_id: int) -> list[Function]:
+    def get_all_by_company(self, company_id: int) -> list[FunctionAll]:
         """
         Get all Function history of all employees.
 
         For more information, refer to the official documentation:
             [Function_GetAll_AllEmployeesByCompany_V2](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Function_GetAll_AllEmployeesByCompany_V2)
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
-            list[Function]: a list of Function objects
+            list[FunctionAll]: a list of Function objects
         """
-        functions = self.client.service.Function_GetAll_AllEmployeesByCompany_V2(CompanyID=company_id, _soapheaders=self.auth_header)
+        functions = self.client.service.Function_GetAll_AllEmployeesByCompany_V2(
+            CompanyID=company_id, _soapheaders=self.auth_manager.header
+        )
         functions = serialize_object(functions)
 
         _functions = []
         for employee in functions:
             for function in employee["EmployeeFunctions"]["EmployeeFunction"]:
-                _functions.append(Function(employee_id=employee["EmployeeId"], data=function))
+                _functions.append(FunctionAll(employee_id=employee["EmployeeId"], data=function))
         return _functions
 
     @nmbrs_exception_handler(resource="EmployeeService:Function_Update")
     def update(self):
         """
         Update the function starting from the given period.
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/hour_component.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/hour_component.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,157 +1,155 @@
 # pylint: disable=line-too-long
 """Microservice responsible for hour component related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class EmployeeHourComponentFixedService(MicroService):
     """Microservice responsible for hour component related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_Get")
-    def fixed_get(self):
+    def get_fixed(self):
         """
         Get all extra hour components for given period.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_GetCurrent")
-    def fixed_get_current(self):
+    def get_current_fixed(self):
         """
         Get all extra hour components for the current period.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_Insert")
-    def fixed_insert(self):
+    def post_fixed(self):
         """
         Insert an extra hour component to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_InsertCurrent")
-    def fixed_insert_current(self):
+    def post_current_fixed(self):
         """
         Insert an extra hour component to the current period.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_Insert_Batch")
-    def fixed_insert_batch(self):
+    def post_batch_fixed(self):
         """
         Insert a batch of extra hour components to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_Insert_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_Insert_With_End")
-    def fixed_insert_with_end(self):
+    def post_fixed_with_end(self):
         """
         Insert an extra hour component with end to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_Insert_With_End](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_Insert_With_End)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentFixed_Stop")
-    def fixed_stop(self):
+    def stop_fixed(self):
         """
         Stop an hour component. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [HourComponentFixed_Stop](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentFixed_Stop)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_Get")
-    def variable_get(self):
+    def get_variable(self):
         """
         Get all extra hour components for given period.
 
         For more information, refer to the official documentation:
             [HourComponentVar_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_GetCurrent")
-    def variable_get_current(self):
+    def get_current_variable(self):
         """
         Get all extra hour components for the current period.
 
         For more information, refer to the official documentation:
             [HourComponentVar_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_Insert")
-    def variable_insert(self):
+    def post_variable(self):
         """
         Insert an extra hour component to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [HourComponentVar_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_InsertCurrent")
-    def variable_insert_current(self):
+    def post_current_variable(self):
         """
         Insert an extra hour component to the current period.
 
         For more information, refer to the official documentation:
             [HourComponentVar_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_Insert_Batch")
-    def variable_insert_batch(self):
+    def post_batch_variable(self):
         """
         Insert a batch of extra hour components to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [HourComponentVar_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_Insert_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_Clear")
-    def variable_clear(self):
+    def clear_variable(self):
         """
         Clear all extra hour components for given period.
 
         For more information, refer to the official documentation:
             [HourComponentVar_Clear](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_Clear)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:HourComponentVar_ClearCurrent")
-    def variable_clear_current(self):
+    def clear_current_variable(self):
         """
         Clear all extra hour components for current period.
 
         For more information, refer to the official documentation:
             [HourComponentVar_ClearCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=HourComponentVar_ClearCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/labour_agreement.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/labour_agreement.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Microservice responsible for labour agreement related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class EmployeeLabourAgreementService(MicroService):
     """Microservice responsible for labour agreement related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:LabourAgreements_Get")
     def get(self):
         """
         Get the labour agreement settings to an employee.
 
         For more information, refer to the official documentation:
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/lease_car.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/lease_car.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Microservice responsible for lease car related actions on the employee level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.employee import LeaseCar
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeeLeaseCarService(MicroService):
     """Microservice responsible for lease car related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:LeaseCar_Get")
     def get(self):
         """
         Get the active lease car contract for given period.
 
         For more information, refer to the official documentation:
@@ -62,15 +60,15 @@
             period (int): The period.
             year (int): The year.
 
         Returns:
             list[LeaseCar]: a list of LeaseCar objects
         """
         lease_cars = self.client.service.LeaseCar_GetAll_EmployeesByCompany(
-            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_header
+            CompanyId=company_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
         )
         lease_cars = serialize_object(lease_cars)
         _lease_cars = []
         for employee in lease_cars:
             for department in employee["LeaseCars"]["EmployeeLeaseCar"]:
                 _lease_cars.append(LeaseCar(employee_id=employee["EmployeeId"], data=department))
         return _lease_cars
@@ -82,25 +80,25 @@
 
         For more information, refer to the official documentation:
             [LeaseCar2_GetAll_EmployeesByCompany](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar2_GetAll_EmployeesByCompany)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:LeaseCar_Insert")
-    def insert(self):
+    def post(self):
         """
         Insert a new lease car contract, this contract will start from given date within the object.
 
         For more information, refer to the official documentation:
             [LeaseCar_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:LeaseCar_InsertCurrent")
-    def insert_current(self):
+    def post_current(self):
         """
         Insert a new lease car contract, this contract will start from given date within the object.
 
         For more information, refer to the official documentation:
             [LeaseCar_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaseCar_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/leave.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/leave.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Microservice responsible for leave related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class EmployeeLeaveService(MicroService):
     """Microservice responsible for leave related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:LeaveBalance_Get")
-    def get(self):
+    def get_current(self):
         """
         Get the Leave Balance for the given employee.
 
         For more information, refer to the official documentation:
             [LeaveBalance_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaveBalance_Get)
         """
         raise NotImplementedError()  # pragma: no cover
@@ -52,15 +50,15 @@
 
         For more information, refer to the official documentation:
             [LeaveBalance_GetPerType](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=LeaveBalance_GetPerType)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:Leave_Insert")
-    def insert(self):
+    def post(self):
         """
         Insert a new leave, starting from a specific date.
 
         For more information, refer to the official documentation:
             [Leave_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Leave_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/levensloop.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/levensloop.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 """Microservice responsible for levens loop related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class EmployeeLevensLoopService(MicroService):
     """Microservice responsible for levens loop related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:Levensloop_Get")
     def get(self):
         """
         Get the active levensloop for given period.
 
         For more information, refer to the official documentation:
             [Levensloop_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Levensloop_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:Levensloop_Insert")
-    def insert(self):
+    def post(self):
         """
         Start levensloop for given date and amount.
 
         For more information, refer to the official documentation:
             [Levensloop_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Levensloop_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/partner.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/partner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # pylint: disable=line-too-long
 """Microservice responsible for partner related actions on the employee level."""
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 from ....data_classes.employee import Partner
 
 
 class EmployeePartnerService(MicroService):
     """Microservice responsible for partner related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:Partner_Get")
-    def get(self):
+    def get_current(self):
         """
         Get employee partner.
 
         For more information, refer to the official documentation:
             [Partner_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Partner_Get)
         """
         raise NotImplementedError()  # pragma: no cover
@@ -39,15 +37,15 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[Partner]: A list of Partner objects
         """
-        partners = self.client.service.Partner_GetAll_AllEmployeesByCompany(CompanyId=company_id, _soapheaders=self.auth_header)
+        partners = self.client.service.Partner_GetAll_AllEmployeesByCompany(CompanyId=company_id, _soapheaders=self.auth_manager.header)
         partners = serialize_object(partners)
         _partners = []
         for employee in partners:
             _partners.append(Partner(employee_id=employee["EmployeeId"], data=employee["Partner"]))
         return _partners
 
     @nmbrs_exception_handler(resource="EmployeeService:Partner_Update")
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/personal_info.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/personal_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # pylint: disable=line-too-long
 """Microservice responsible for personal info related actions on the employee level."""
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.employee import PersonalInfo, PersonalInfoContractSalaryAddress
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeePersonalInfoService(MicroService):
     """Microservice responsible for personal info related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:PersonalInfo_Get")
     def get(self, employee_id: int, period: int, year: int) -> PersonalInfo | None:
         """
         Get the active personal info for given period.
 
         For more information, refer to the official documentation:
@@ -31,15 +29,15 @@
             period (int): The period for which personal information is retrieved.
             year (int): The year for which personal information is retrieved.
 
         Returns:
             PersonalInfo | None: The personal information of the employee for the specified period, or None if not found.
         """
         personal_info = self.client.service.PersonalInfo_Get(
-            EmployeeId=employee_id, Period=period, Year=year, _soapheaders=self.auth_header
+            EmployeeId=employee_id, Period=period, Year=year, _soapheaders=self.auth_manager.header
         )
         if not personal_info:
             return None
         return PersonalInfo(employee_id=employee_id, data=serialize_object(personal_info))
 
     @nmbrs_exception_handler(resource="EmployeeService:PersonalInfo_GetCurrent")
     def get_current(self, employee_id: int) -> PersonalInfo | None:
@@ -51,15 +49,15 @@
 
         Args:
             employee_id (int): The ID of the employee.
 
         Returns:
             PersonalInfo | None: The currently active personal information of the employee, or None if not found.
         """
-        personal_info = self.client.service.PersonalInfo_GetCurrent(EmployeeId=employee_id, _soapheaders=self.auth_header)
+        personal_info = self.client.service.PersonalInfo_GetCurrent(EmployeeId=employee_id, _soapheaders=self.auth_manager.header)
         if not personal_info:
             return None
         return PersonalInfo(employee_id=employee_id, data=serialize_object(personal_info))
 
     @return_list
     @nmbrs_exception_handler(resource="EmployeeService:PersonalInfo_GetAll_AllEmployeesByCompany")
     def get_all_by_company(self, company_id: int) -> list[PersonalInfo]:
@@ -71,15 +69,17 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[PersonalInfo]: A list of personal information objects of all employees within the company.
         """
-        people_info = self.client.service.PersonalInfo_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_header)
+        people_info = self.client.service.PersonalInfo_GetAll_AllEmployeesByCompany(
+            CompanyID=company_id, _soapheaders=self.auth_manager.header
+        )
 
         _people_info = []
         for person in serialize_object(people_info):
             for info in person["EmployeePersonalInfos"]["PersonalInfo_V2"]:
                 _people_info.append(PersonalInfo(employee_id=person["EmployeeId"], data=info))
 
         return _people_info
@@ -96,15 +96,15 @@
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[PersonalInfo]: A list of personal information objects of all employees within the company, excluding the BSN.
         """
         people_info = self.client.service.PersonalInfoWithoutBSN_Get_GetAllEmployeesByCompany(
-            CompanyID=company_id, _soapheaders=self.auth_header
+            CompanyID=company_id, _soapheaders=self.auth_manager.header
         )
 
         _people_info = []
         for person in serialize_object(people_info):
             for info in person["EmployeePersonalInfos"]["PersonalInfo_V2"]:
                 _people_info.append(PersonalInfo(employee_id=person["EmployeeId"], data=info))
 
@@ -122,15 +122,15 @@
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[PersonalInfoContractSalaryAddress]: A list of personal information objects including contract and salary address of all employees within the company.
         """
         people_info = self.client.service.PersonalInfoContractSalaryAddress_GetAll_AllEmployeesByCompany(
-            CompanyID=company_id, _soapheaders=self.auth_header
+            CompanyID=company_id, _soapheaders=self.auth_manager.header
         )
         return [
             PersonalInfoContractSalaryAddress(employee_id=person["EmployeeID"], data=person) for person in serialize_object(people_info)
         ]
 
     @nmbrs_exception_handler(resource="EmployeeService:PersonalInfo_Update")
     def update(self, employee_id: int, personal_info: PersonalInfo, period: int, year: int):
@@ -178,15 +178,15 @@
             "DeceasedDate": personal_info.deceased_date,
             "InCaseOfEmergency": personal_info.in_case_of_emergency,
             "InCaseOfEmergencyPhone": personal_info.in_case_of_emergency_phone,
             "InCaseOfEmergencyRelation": personal_info.in_case_of_emergency_relation,
             "TitleAfter": personal_info.title_after,
         }
         response = self.client.service.PersonalInfo_Update(
-            EmployeeId=employee_id, PersonalInfo=new_personal_info, Period=period, Year=year, _soapheaders=self.auth_header
+            EmployeeId=employee_id, PersonalInfo=new_personal_info, Period=period, Year=year, _soapheaders=self.auth_manager.header
         )
         return response
 
     @nmbrs_exception_handler(resource="EmployeeService:PersonalInfo_UpdateCurrent")
     def update_current(self, employee_id: int, personal_info: PersonalInfo):
         """
         Update personal info starting from the current period.
@@ -230,10 +230,10 @@
             "DeceasedDate": personal_info.deceased_date,
             "InCaseOfEmergency": personal_info.in_case_of_emergency,
             "InCaseOfEmergencyPhone": personal_info.in_case_of_emergency_phone,
             "InCaseOfEmergencyRelation": personal_info.in_case_of_emergency_relation,
             "TitleAfter": personal_info.title_after,
         }
         response = self.client.service.PersonalInfo_UpdateCurrent(
-            EmployeeId=employee_id, PersonalInfo=new_personal_info, _soapheaders=self.auth_header
+            EmployeeId=employee_id, PersonalInfo=new_personal_info, _soapheaders=self.auth_manager.header
         )
         return response
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/salary.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/salary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # pylint: disable=line-too-long
 """Microservice responsible for salary related actions on the employee level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Salary
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeeSalaryService(MicroService):
     """Microservice responsible for salary related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:Salary_Get")
     def get(self):
         """
         Get the active salary for the given period.
 
         For more information, refer to the official documentation:
@@ -60,15 +58,15 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[Salary]: A list of Salary objects
         """
-        salaries = self.client.service.Salary_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_header)
+        salaries = self.client.service.Salary_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_manager.header)
         salaries = serialize_object(salaries)
         _salaries = []
         for employee in salaries:
             for salary in employee["EmployeeSalaries"]["Salary_V2"]:
                 _salaries.append(Salary(employee_id=employee["EmployeeId"], data=salary))
         return _salaries
 
@@ -89,25 +87,25 @@
 
         For more information, refer to the official documentation:
             [Salary_GetEstimatedCostPerHour](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Salary_GetEstimatedCostPerHour)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:SalaryTable_Insert")
-    def insert(self):
+    def post(self):
         """
         Insert salary table to salary.
 
         For more information, refer to the official documentation:
             [SalaryTable_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SalaryTable_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:SalaryTable_InsertCurrent")
-    def insert_current(self):
+    def post_current(self):
         """
         Insert salary table to salary of current salary.
 
         For more information, refer to the official documentation:
             [SalaryTable_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=SalaryTable_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/schedule.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/schedule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # pylint: disable=line-too-long
 """Microservice responsible for schedule related actions on the employee level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.employee import Schedule
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class EmployeeScheduleService(MicroService):
     """Microservice responsible for schedule related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:Schedule_GetList")
     def get_all(self):
         """
         Get all schedules, until given period.
 
         For more information, refer to the official documentation:
@@ -58,15 +56,15 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[Contract]: a list of contract objects
         """
-        schedules = self.client.service.Schedule_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_header)
+        schedules = self.client.service.Schedule_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_manager.header)
         schedules = serialize_object(schedules)
         _schedules = []
         for employee in schedules:
             for schedule in employee["EmployeeSchedules"]["Schedule_V2"]:
                 _schedules.append(Schedule(employee_id=employee["EmployeeId"], data=schedule))
         return _schedules
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/service.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 # pylint: disable=line-too-long
 """Microservice responsible for service related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class EmployeeServiceService(MicroService):
     """Microservice responsible for service related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:Service_GetList")
     def get_all(self):
         """
         Get all service intervals.
 
         For more information, refer to the official documentation:
             [Service_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:Service_Insert")
-    def insert(self):
+    def post(self):
         """
         Start a new service interval. If the date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Service_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:Service_Insert2")
-    def insert_2(self):
+    def post_2(self):
         """
         Start a new service interval. If the date is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Service_Insert2](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Service_Insert2)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/spaarloon.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/spaarloon.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # pylint: disable=line-too-long
 """Microservice responsible for spaarloon related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class EmployeeSpaarloonService(MicroService):
     """Microservice responsible for spaarloon related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:Spaarloon_Get")
     def get(self):
         """
         Get the active spaarloon for given period.
 
         For more information, refer to the official documentation:
@@ -33,15 +31,15 @@
 
         For more information, refer to the official documentation:
             [Spaarloon_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Spaarloon_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:Spaarloon_Insert")
-    def insert(self):
+    def post(self):
         """
         Start spaarloon for given date and amount. If the startdate is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [Spaarloon_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=Spaarloon_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/svw.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/svw.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Microservice responsible for svw related actions on the employee level."""
 
 from zeep import Client
 from zeep.helpers import serialize_object
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....data_classes.employee import SVW
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 from ....utils.return_list import return_list
 
 
 class EmployeeSvwService(MicroService):
     """Microservice responsible for svw related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:SVW_Get")
     def get(self):
         """
         Get the active SVW settings for given period.
 
         For more information, refer to the official documentation:
@@ -59,15 +57,15 @@
 
         Args:
             company_id (int): The ID of the company.
 
         Returns:
             list[SVW]: A list of SVW objects
         """
-        svws = self.client.service.SVW_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_header)
+        svws = self.client.service.SVW_GetAll_AllEmployeesByCompany(CompanyID=company_id, _soapheaders=self.auth_manager.header)
         svws = serialize_object(svws)
         _svw = []
         for employee in svws:
             for svw in employee["EmployeeSVWSettings"]["EmployeeSVWSettings"]:
                 _svw.append(SVW(employee_id=employee["EmployeeId"], data=svw))
         return _svw
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/time_registration.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/time_registration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 # pylint: disable=line-too-long
 """Microservice responsible for time registration related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class EmployeeTimeRegistrationService(MicroService):
     """Microservice responsible for time registration related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_GetList")
     def get_all(self):
         """
         Get Time Registration items filtered by time.
 
         For more information, refer to the official documentation:
             [TimeRegistration_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_Insert")
-    def insert(self):
+    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_GetAll_AllTimeRegistrationCodes")
+    def get_codes(self):
         """
-        Register item into the calendar of an employee.
+        Get available TimeRegistrationCodes.
 
         For more information, refer to the official documentation:
-            [TimeRegistration_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_Insert)
+            [TimeRegistration_GetAll_AllTimeRegistrationCodes](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_GetAll_AllTimeRegistrationCodes)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_Insert_Batch")
-    def insert_batch(self):
+    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_Insert")
+    def post(self):
         """
-        Register items into the calendars.
+        Register item into the calendar of an employee.
 
         For more information, refer to the official documentation:
-            [TimeRegistration_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_Insert_Batch)
+            [TimeRegistration_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_GetAll_AllTimeRegistrationCodes")
-    def get_codes(self):
+    @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_Insert_Batch")
+    def post_batch(self):
         """
-        Get available TimeRegistrationCodes.
+        Register items into the calendars.
 
         For more information, refer to the official documentation:
-            [TimeRegistration_GetAll_AllTimeRegistrationCodes](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_GetAll_AllTimeRegistrationCodes)
+            [TimeRegistration_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeRegistration_Insert_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:TimeRegistration_Delete")
     def delete(self):
         """
         Delete Time Registration Item By ID.
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/time_schedule.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/wage_tax.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,84 @@
-# pylint: disable=line-too-long
-"""Microservice responsible for time schedule related actions on the employee level."""
+"""Microservice responsible for wage tax related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
-class EmployeeTimeScheduleService(MicroService):
-    """Microservice responsible for time schedule related actions on the employee level."""
+class EmployeeWageTaxService(MicroService):
+    """Microservice responsible for wage tax related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_Get")
+    def get(self):
+        """
+        Get the active loonheffing settings for given period.
 
-    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_AllEmployee_GetListByPeriod")
-    def get_all_by_company(self):
+        For more information, refer to the official documentation:
+            [WageTax_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Get)
         """
-        Get Time Schedules from employee and period.
+        raise NotImplementedError()  # pragma: no cover
+
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_GetCurrent")
+    def get_current(self):
+        """
+        Get the currently active loonheffing settings.
 
         For more information, refer to the official documentation:
-            [TimeSchedule_AllEmployee_GetListByPeriod](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_AllEmployee_GetListByPeriod)
+            [WageTax_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_GetAll")
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_GetList")
     def get_all(self):
         """
-        Get all Time Schedules from employee.
+        Get a list of all loonheffing settings.
 
         For more information, refer to the official documentation:
-            [TimeSchedule_GetAll](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_GetAll)
+            [WageTax_GetList](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_GetList)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_GetListByPeriod")
-    def get(self):
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_Get_SE")
+    def get_settings(self):
+        """
+        Get active wage tax settings for a specific period.
+
+        For more information, refer to the official documentation:
+            [WageTax_Get_SE](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Get_SE)
+        """
+        raise NotImplementedError()  # pragma: no cover
+
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_Update")
+    def update(self):
         """
-        Get Time Schedules from employee and period.
+        Update loonheffing settings starting from given period
 
         For more information, refer to the official documentation:
-            [TimeSchedule_GetListByPeriod](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_GetListByPeriod)
+            [WageTax_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_Insert")
-    def insert(self):
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_UpdateCurrent")
+    def update_current(self):
         """
-        Add a new TimeSchedule.
+        Update loonheffing settings starting from the current period.
 
         For more information, refer to the official documentation:
-            [TimeSchedule_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_Insert)
+            [WageTax_UpdateCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_UpdateCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
-    @nmbrs_exception_handler(resource="EmployeeService:TimeSchedule_DeleteByID")
-    def delete(self):
+    @nmbrs_exception_handler(resource="EmployeeService:WageTax_Update_SE")
+    def update_settings(self):
         """
-        Delete employee time schedule.
+        Update loonheffing settings starting from given period.
 
         For more information, refer to the official documentation:
-            [TimeSchedule_DeleteByID](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=TimeSchedule_DeleteByID)
+            [WageTax_Update_SE](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageTax_Update_SE)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/employee/wage_component.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/employee/wage_component.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # pylint: disable=line-too-long
 """Microservice responsible for wage components related actions on the employee level."""
 
 from zeep import Client
 
 from ..micro_service import MicroService
+from ....auth.token_manager import AuthManager
 from ....utils.nmbrs_exception_handler import nmbrs_exception_handler
 
 
 class EmployeeWageComponentsService(MicroService):
     """Microservice responsible for wage components related actions on the employee level."""
 
-    def __init__(self, client: Client) -> None:
-        super().__init__(client)
-
-    def set_auth_header(self, auth_header: dict) -> None:
-        self.auth_header = auth_header
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        super().__init__(auth_manager, client)
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponent_Delete")
     def delete(self):
         """
         Delete a wage component by ID.
 
         For more information, refer to the official documentation:
@@ -35,165 +33,165 @@
 
         For more information, refer to the official documentation:
             [WageComponent_Update](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponent_Update)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_Get")
-    def fixed_get(self):
+    def get_fixed(self):
         """
         Get all fixed wage components for given period.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_GetCurrent")
-    def fixed_get_current(self):
+    def get_current_fixed(self):
         """
         Get all fixed wage components for the current period.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_GetCurrent")
-    def fixed_insert(self):
+    def post_fixed(self):
         """
         Insert a wage component to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_Insert_With_End")
-    def fixed_insert_with_end(self):
+    def insert_fixed_with_end(self):
         """
         Insert a wage component to given period of time. If the start period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_Insert_With_End](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Insert_With_End)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_InsertCurrent")
-    def fixed_insert_current(self):
+    def post_current_fixed(self):
         """
         Insert a wage component to the current period.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_InsertCurrent_With_End")
-    def fixed_insert_current_with_end(self):
+    def post_current_fixed_with_end(self):
         """
         Insert a wage component to the current period with end period.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_InsertCurrent_With_End](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_InsertCurrent_With_End)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_Insert_Batch")
-    def fixed_insert_batch(self):
+    def post_batch_fixed(self):
         """
         Insert a batch of wage components to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Insert_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_Insert_Batch_With_End")
-    def fixed_insert_batch_with_end(self):
+    def post_batch_fixed_with_end(self):
         """
         Insert a batch of wage components to given period of time. If the start period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_Insert_Batch_With_End](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Insert_Batch_With_End)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentFixed_Stop")
-    def fixed_stop(self):
+    def stop_fixed(self):
         """
         Stop a wage component ending after given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentFixed_Stop](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentFixed_Stop)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_Get")
-    def variable_get(self):
+    def get_variable(self):
         """
         Get all variable wage components for given period.
 
         For more information, refer to the official documentation:
             [WageComponentVar_Get](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_Get)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_GetCurrent")
-    def variable_get_current(self):
+    def get_current_variable(self):
         """
         Get all variable wage components for the current period.
 
         For more information, refer to the official documentation:
             [WageComponentVar_GetCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_GetCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_Insert")
-    def variable_insert(self):
+    def post_variable(self):
         """
         Insert a wage component to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentVar_Insert](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_Insert)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_InsertCurrent")
-    def variable_insert_current(self):
+    def post_current_varaible(self):
         """
         Insert a wage components to the current period.
 
         For more information, refer to the official documentation:
             [WageComponentVar_InsertCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_InsertCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_Insert_Batch")
-    def variable_insert_batch(self):
+    def post_batch_variable(self):
         """
         Insert a batch of wage components to given period. If the period is before the company's current period, unprotected mode flag is required.
 
         For more information, refer to the official documentation:
             [WageComponentVar_Insert_Batch](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_Insert_Batch)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_Clear")
-    def variable_clear(self):
+    def clear_variable(self):
         """
         Clear all variable wage components for given period.
 
         For more information, refer to the official documentation:
             [WageComponentVar_Clear](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_Clear)
         """
         raise NotImplementedError()  # pragma: no cover
 
     @nmbrs_exception_handler(resource="EmployeeService:WageComponentVar_ClearCurrent")
-    def variable_clear_current(self):
+    def clear_current_variable(self):
         """
         Clear all variable wage components for the current period.
 
         For more information, refer to the official documentation:
             [WageComponentVar_ClearCurrent](https://api.nmbrs.nl/soap/v3/EmployeeService.asmx?op=WageComponentVar_ClearCurrent)
         """
         raise NotImplementedError()  # pragma: no cover
```

### Comparing `nmbrs-0.1.6/src/nmbrs/service/microservices/micro_service.py` & `nmbrs-0.2.0/src/nmbrs/service/microservices/micro_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,32 +2,25 @@
 Abstract base class for defining microservice interfaces.
 """
 
 from abc import ABC, abstractmethod
 
 from zeep import Client
 
+from src.nmbrs.auth.token_manager import AuthManager
+
 
 class MicroService(ABC):
     """
     Abstract base class for defining microservice interfaces.
 
     This class defines the common structure and methods required for interacting with microservices.
 
     Attributes:
         client (Client): A Zeep Client object used for communication with the microservice.
-        auth_header (dict | None): The authentication header used by Nmbrs.
+        auth_manager (AuthManager): An instance of the AuthManager class for managing authentication.
     """
 
     @abstractmethod
-    def __init__(self, client: Client) -> None:
+    def __init__(self, auth_manager: AuthManager, client: Client):
+        self.auth_manager = auth_manager
         self.client = client
-        self.auth_header: dict | None = None
-
-    @abstractmethod
-    def set_auth_header(self, auth_header: dict) -> None:
-        """
-        Method to set the authentication header for requests to the microservice.
-
-        Args:
-            auth_header (dict): New authentication header to be set.
-        """
```

### Comparing `nmbrs-0.1.6/src/nmbrs/utils/find_empty_params.py` & `nmbrs-0.2.0/src/nmbrs/utils/find_empty_params.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.6/src/nmbrs/utils/return_list.py` & `nmbrs-0.2.0/src/nmbrs/utils/return_list.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.6/src/nmbrs.egg-info/PKG-INFO` & `nmbrs-0.2.0/src/nmbrs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmbrs
-Version: 0.1.6
+Version: 0.2.0
 Summary: Python SDK for the Visma Nmbrs SOAP API.
 Author: Lars Kluijtmans
 Author-email: info@lk-software.com
 Maintainer: Lars Kluijtmans
 Maintainer-email: info@lk-software.com
 License: Lars Kluijtmans
 Project-URL: Homepage, https://github.com/LarsKluijtmans/nmbrs_api
@@ -189,54 +189,52 @@
 #### Username and Token
 
 ```python
 from nmbrs import SingleSingOnService
 
 sso_service = SingleSingOnService()
 
-sso_token = sso_service.sso_auth_with_token("__username__", "__token__")
+sso_token = sso_service.get_token_with_api_token("__username__", "__token__")
 
 print(sso_token)
 ```
 
 #### Username and Password
 
 ```python
 from nmbrs import SingleSingOnService
 
 sso_service = SingleSingOnService()
 
-
-sso_token = sso_service.sso_auth_with_password("__username__", "__token__")
+sso_token = sso_service.get_token_with_password("__username__", "__token__")
 
 print(sso_token)
 ```
 
 **Note:** this function will raise an exception if you have accounts in multiple Nmbrs environments. In this case use the following call where you specify the domain you want to log in to. 
 
 #### Username, password, and domain
 
 ```python
 from nmbrs import SingleSingOnService
 
 sso_service = SingleSingOnService()
 
-
-sso_token = sso_service.sso_auth_with_domain("__username__", "__password__", "__domain__")
+sso_token = sso_service.get_token_with_domain("__username__", "__password__", "__domain__")
 
 print(sso_token)
 ```
 
 ### SSO url:
 
 Using the token reverence from the aforementioned functions we can create an url that automatically refers the user to nmbrs.
 
 ```python
 from nmbrs import SingleSingOnService
 
 sso_service = SingleSingOnService()
 
-sso_token = sso_service.sso_auth_with_password("__username__", "__password__")
+sso_token = sso_service.get_token_with_password("__username__", "__password__")
 sso_url = sso_service.get_sso_url(sso_token, "__domain__")
 
 print(sso_url)
 ```
```

### Comparing `nmbrs-0.1.6/src/nmbrs.egg-info/SOURCES.txt` & `nmbrs-0.2.0/src/nmbrs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 src/nmbrs/__version__.py
 src/nmbrs/api.py
 src/nmbrs.egg-info/PKG-INFO
 src/nmbrs.egg-info/SOURCES.txt
 src/nmbrs.egg-info/dependency_links.txt
 src/nmbrs.egg-info/requires.txt
 src/nmbrs.egg-info/top_level.txt
+src/nmbrs/auth/__init__.py
+src/nmbrs/auth/token_manager.py
 src/nmbrs/data_classes/__init__.py
 src/nmbrs/data_classes/company.py
 src/nmbrs/data_classes/data_class.py
 src/nmbrs/data_classes/debtor.py
 src/nmbrs/data_classes/employee.py
 src/nmbrs/data_classes/general.py
 src/nmbrs/data_classes/utils/__init__.py
```

