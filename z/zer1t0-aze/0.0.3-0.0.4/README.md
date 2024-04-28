# Comparing `tmp/zer1t0_aze-0.0.3.tar.gz` & `tmp/zer1t0_aze-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zer1t0_aze-0.0.3.tar", last modified: Sun Apr 21 19:34:30 2024, max compression
+gzip compressed data, was "zer1t0_aze-0.0.4.tar", last modified: Sun Apr 28 17:47:31 2024, max compression
```

## Comparing `zer1t0_aze-0.0.3.tar` & `zer1t0_aze-0.0.4.tar`

### file list

```diff
@@ -1,75 +1,78 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.973899 zer1t0_aze-0.0.3/
--rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     1913 2024-04-21 19:34:30.973899 zer1t0_aze-0.0.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1493 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.957899 zer1t0_aze-0.0.3/aze/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_brute_passwords.py
--rw-rw-r--   0 user      (1000) user      (1000)     4079 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_brute_service_subdomains.py
--rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_brute_usernames.py
--rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_get_login_info.py
--rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_get_tenant_domains.py
--rw-rw-r--   0 user      (1000) user      (1000)      982 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_get_tenant_id.py
--rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_inspect_token.py
--rw-rw-r--   0 user      (1000) user      (1000)     9035 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_login_with_token.py
--rw-rw-r--   0 user      (1000) user      (1000)     2764 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_search_token_in_cache.py
--rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_whoami.py
--rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/error.py
--rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/read_in.py
--rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/tenant.py
--rw-rw-r--   0 user      (1000) user      (1000)     1252 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/tokens.py
--rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/version.py
--rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-21 19:34:30.973899 zer1t0_aze-0.0.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1293 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.973899 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     1913 2024-04-21 19:34:30.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      751 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     2375 2024-04-21 19:34:30.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/SOURCES.txt
--rwxrwxr-x   0 user      (1000) user      (1000)      107 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/az-get-login-info
--rwxrwxr-x   0 user      (1000) user      (1000)      106 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/az-inspect-token
--rwxrwxr-x   0 user      (1000) user      (1000)      109 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/az-login-with-token
--rwxrwxr-x   0 user      (1000) user      (1000)      102 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/az-tenant-id
--rwxrwxr-x   0 user      (1000) user      (1000)       99 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/az-whoami
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.965899 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.969899 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/
--rw-rw-r--   0 user      (1000) user      (1000)      132 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     3158 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      869 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     5617 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     8123 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     1106 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      380 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_whoami.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     1063 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      695 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      733 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     3319 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_get_login_info.py
--rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_inspect_token.py
--rw-rw-r--   0 user      (1000) user      (1000)    10027 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_login_with_token.py
--rw-rw-r--   0 user      (1000) user      (1000)      895 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_tenant_id.py
--rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_whoami.py
--rw-rw-r--   0 user      (1000) user      (1000)      836 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/read_in.py
--rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/tenant.py
--rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/version.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.969899 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      415 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      341 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      229 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-21 19:34:30.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/dependency_links.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.973899 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/dist/
--rw-rw-r--   0 user      (1000) user      (1000)    19900 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz
--rw-rw-r--   0 user      (1000) user      (1000)    21497 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl
--rw-rw-r--   0 user      (1000) user      (1000)      518 2024-04-21 19:34:30.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-21 19:34:30.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1141 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/setup.py
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-21 19:34:30.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.448376 zer1t0_aze-0.0.4/
+-rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     2002 2024-04-28 17:47:31.448376 zer1t0_aze-0.0.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1582 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.432376 zer1t0_aze-0.0.4/aze/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1136 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/arm_api.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_brute_passwords.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4079 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_brute_service_subdomains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_brute_usernames.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_get_login_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_get_tenant_domains.py
+-rw-rw-r--   0 user      (1000) user      (1000)      982 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_get_tenant_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_inspect_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1632 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_list_role_assignment.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9516 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_login_with_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2434 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_search_token_in_cache.py
+-rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_whoami.py
+-rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/error.py
+-rw-rw-r--   0 user      (1000) user      (1000)      444 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/profile.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/read_in.py
+-rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/tenant.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1802 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/tokens.py
+-rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/version.py
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-28 17:47:31.448376 zer1t0_aze-0.0.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1353 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.448376 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     2002 2024-04-28 17:47:31.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      751 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     2436 2024-04-28 17:47:31.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/SOURCES.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)      107 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/az-get-login-info
+-rwxrwxr-x   0 user      (1000) user      (1000)      106 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/az-inspect-token
+-rwxrwxr-x   0 user      (1000) user      (1000)      109 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/az-login-with-token
+-rwxrwxr-x   0 user      (1000) user      (1000)      102 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/az-tenant-id
+-rwxrwxr-x   0 user      (1000) user      (1000)       99 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/az-whoami
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.440376 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.444376 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/
+-rw-rw-r--   0 user      (1000) user      (1000)      132 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     3158 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      869 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     5617 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     8123 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     1106 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      380 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_whoami.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     1063 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      695 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      733 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     3319 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_get_login_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_inspect_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10027 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_login_with_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)      895 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_tenant_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_whoami.py
+-rw-rw-r--   0 user      (1000) user      (1000)      836 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/read_in.py
+-rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/tenant.py
+-rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.444376 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      415 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      341 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      229 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-28 17:47:31.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/dependency_links.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.448376 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/dist/
+-rw-rw-r--   0 user      (1000) user      (1000)    19900 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz
+-rw-rw-r--   0 user      (1000) user      (1000)    21497 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl
+-rw-rw-r--   0 user      (1000) user      (1000)      632 2024-04-28 17:47:31.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-28 17:47:31.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1141 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/setup.py
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-28 17:47:31.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/top_level.txt
```

### Comparing `zer1t0_aze-0.0.3/LICENSE` & `zer1t0_aze-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/PKG-INFO` & `zer1t0_aze-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zer1t0-aze
-Version: 0.0.3
+Version: 0.0.4
 Summary: Enhance azure cli
 Home-page: https://gitlab.com/Zer1t0/aze
 Author: Eloy Pérez González
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -29,14 +29,15 @@
 - **az-brute-passwords**: Validate Azure credentials (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
   subdomains.
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
+- **az-list-role-assignment**: List roles without requiring a graph access token (Auth).
 - **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
 - **az-whoami**: Shorcut for "az ad signed-in-user show".
 
 ## Installation
 
 ```
```

### Comparing `zer1t0_aze-0.0.3/README.md` & `zer1t0_aze-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 - **az-brute-passwords**: Validate Azure credentials (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
   subdomains.
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
+- **az-list-role-assignment**: List roles without requiring a graph access token (Auth).
 - **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
 - **az-whoami**: Shorcut for "az ad signed-in-user show".
 
 ## Installation
 
 ```
```

### Comparing `zer1t0_aze-0.0.3/aze/az_brute_passwords.py` & `zer1t0_aze-0.0.4/aze/az_brute_passwords.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/aze/az_brute_service_subdomains.py` & `zer1t0_aze-0.0.4/aze/az_brute_service_subdomains.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/aze/az_brute_usernames.py` & `zer1t0_aze-0.0.4/aze/az_brute_usernames.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/aze/az_get_login_info.py` & `zer1t0_aze-0.0.4/aze/az_get_login_info.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/aze/az_get_tenant_domains.py` & `zer1t0_aze-0.0.4/aze/az_get_tenant_domains.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/aze/az_get_tenant_id.py` & `zer1t0_aze-0.0.4/aze/az_get_tenant_id.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/aze/az_inspect_token.py` & `zer1t0_aze-0.0.4/aze/az_inspect_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/aze/az_login_with_token.py` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_login_with_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 import json
 import time
 import configparser
 import os
 import codecs
 from . import utils
 from .tenant import resolve_tenant_id
-from .error import AzeError
-from .tokens import load_token_cache
+
+from msal_extensions import (FilePersistenceWithDataProtection, KeychainPersistence, LibsecretPersistence, FilePersistence, PersistedTokenCache)
+
+class AzeError(Exception):
+    pass
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Login with Azure Tokens")
     main_token_group = parser.add_mutually_exclusive_group(required=True)
     main_token_group.add_argument(
         "-a", "--access-token",
         help="Access token for any Azure service.",
@@ -59,16 +62,15 @@
             scope=tokens["scope"],
             client_info=tokens["client_info"],
             expires_in=tokens["expires_in"],
             ext_expires_in=tokens["ext_expires_in"],
         )
         t_infos = [at_info]
 
-    token_cache = load_token_cache()
-    store_tokens(t_infos, token_cache)
+    store_tokens(t_infos)
     set_subscriptions(t_infos[0], resp_subscriptions)
 
 
 
 
 # A simple implementation of Profile._set_subscriptions
 # https://github.com/Azure/azure-cli/blob/6771b2b1ef04ed2f8e71b636eccce5cf68a7d76d/src/azure-cli-core/azure/cli/core/_profile.py#L454
@@ -189,24 +191,29 @@
     if resp.status_code != 200:
         raise AzeError(
             "Unable to get access token: error code {}".format(resp.status_code)
         )
 
     return resp.json()
 
-
-def store_tokens(tokens_info, token_cache):
+def store_tokens(tokens_info):
     if not tokens_info:
         return
 
     tokens_events = [create_event_from_token_info(t_info) for t_info in tokens_info]
+    token_cache = load_persisted_token_cache(
+        "{}/.azure/msal_token_cache.json".format(os.environ["HOME"]),
+        False
+    )
     for t_event in tokens_events:
         token_cache.add(t_event)
 
 
+
+
 class TokenInformation:
 
     def __init__(
             self,
             access_token,
             refresh_token=None,
             id_token=None,
@@ -299,7 +306,30 @@
         "token_endpoint": "https://login.microsoftonline.com/{}".format(tenant_id),
         "grant_type": "",
         "response": resp,
         # "params": {},
         # "data": {},
     }
 
+def load_persisted_token_cache(location, encrypt):
+    persistence = build_persistence(location, encrypt)
+    return PersistedTokenCache(persistence)
+
+def build_persistence(location, encrypt):
+    if encrypt:
+        if sys.platform.startswith('win'):
+            return FilePersistenceWithDataProtection(location)
+        if sys.platform.startswith('darwin'):
+            return KeychainPersistence(
+                location,
+                "my_service_name",
+                "my_account_name"
+            )
+        if sys.platform.startswith('linux'):
+            return LibsecretPersistence(
+                location,
+                schema_name="my_schema_name",
+                attributes={"my_attr1": "foo", "my_attr2": "bar"}
+            )
+    else:
+        return FilePersistence(location)
+
```

### Comparing `zer1t0_aze-0.0.3/aze/az_search_token_in_cache.py` & `zer1t0_aze-0.0.4/aze/az_search_token_in_cache.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from .tokens import load_token_cache
+from .tokens import search_token_in_cache, CredentialType
 import json
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description="Retrieve items from token cache based on the filters."
     )
     parser.add_argument(
@@ -49,53 +49,44 @@
         help="Search for App Metadata tokens",
         action="store_true",
     )
 
     return parser.parse_args()
 
 
-# class CredentialType:
-#         ACCESS_TOKEN = "AccessToken"
-#         REFRESH_TOKEN = "RefreshToken"
-#         ACCOUNT = "Account"  # Not exactly a credential type, but we put it here
-#         ID_TOKEN = "IdToken"
-#         APP_METADATA = "AppMetadata"
-
 def main():
     args = parse_args()
     client_id = args.client_id
     environment = None # usually "login.microsoft.com"
     realm = args.realm
     home_id = None
 
-    token_cache = load_token_cache()
-
     scopes = args.scope
 
     if args.refresh:
-        token_type = token_cache.CredentialType.REFRESH_TOKEN
+        token_type = CredentialType.REFRESH_TOKEN
     elif args.account:
-        token_type = token_cache.CredentialType.ACCOUNT
+        token_type = CredentialType.ACCOUNT
     elif args.id:
-        token_type = token_cache.CredentialType.ID_TOKEN
+        token_type = CredentialType.ID_TOKEN
     elif args.metadata:
-        token_type = token_cache.CredentialType.APP_METADATA
+        token_type = CredentialType.APP_METADATA
     else:
-        token_type = token_cache.CredentialType.ACCESS_TOKEN
+        token_type = CredentialType.ACCESS_TOKEN
 
 
     query = {}
     if client_id:
         query["client_id"] = client_id
     if environment:
         query["environment"] = environment
     if realm:
         query["realm"] = realm
     if home_id:
         query["home_account_id"] = home_id
 
-    for entry in token_cache.find(
+    for entry in search_token_in_cache(
             token_type,
             query=query,
-            target=scopes,
+            scopes=scopes,
     ):
         print(json.dumps(entry))
```

### Comparing `zer1t0_aze-0.0.3/aze/read_in.py` & `zer1t0_aze-0.0.4/aze/read_in.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/aze/utils.py` & `zer1t0_aze-0.0.4/aze/utils.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/setup.py` & `zer1t0_aze-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     "az-brute-passwords",
     "az-brute-usernames",
     "az-brute-service-subdomains",
     "az-get-login-info",
     "az-get-tenant-domains",
     "az-get-tenant-id",
     "az-inspect-token",
+    "az-list-subscriptions",
+    "az-list-role-assignment",
     "az-login-with-token",
     "az-search-token-in-cache",
     "az-whoami",
 ]
 
 console_scripts = [
     "{} = {}.{}:main".format(script, name, script.replace("-", "_"))
```

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/LICENSE` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/LICENSE`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/PKG-INFO` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zer1t0-aze
-Version: 0.0.3
+Version: 0.0.4
 Summary: Enhance azure cli
 Home-page: https://gitlab.com/Zer1t0/aze
 Author: Eloy Pérez González
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -29,14 +29,15 @@
 - **az-brute-passwords**: Validate Azure credentials (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
   subdomains.
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
+- **az-list-role-assignment**: List roles without requiring a graph access token (Auth).
 - **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
 - **az-whoami**: Shorcut for "az ad signed-in-user show".
 
 ## Installation
 
 ```
```

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/README.md` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/README.md`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/SOURCES.txt` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 aze/__init__.py
+aze/arm_api.py
 aze/az_brute_passwords.py
 aze/az_brute_service_subdomains.py
 aze/az_brute_usernames.py
 aze/az_get_login_info.py
 aze/az_get_tenant_domains.py
 aze/az_get_tenant_id.py
 aze/az_inspect_token.py
+aze/az_list_role_assignment.py
 aze/az_login_with_token.py
 aze/az_search_token_in_cache.py
 aze/az_whoami.py
 aze/error.py
+aze/profile.py
 aze/read_in.py
 aze/tenant.py
 aze/tokens.py
 aze/utils.py
 aze/version.py
 zer1t0_aze.egg-info/LICENSE
 zer1t0_aze.egg-info/MANIFEST.in
```

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_get_login_info.py` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_get_login_info.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_inspect_token.py` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_inspect_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_login_with_token.py` & `zer1t0_aze-0.0.4/aze/az_login_with_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import argparse
 import requests
 import base64
 import json
 import time
 import configparser
 import os
-import codecs
 from . import utils
 from .tenant import resolve_tenant_id
-
-from msal_extensions import (FilePersistenceWithDataProtection, KeychainPersistence, LibsecretPersistence, FilePersistence, PersistedTokenCache)
-
-class AzeError(Exception):
-    pass
+from .error import AzeError
+from .tokens import load_token_cache
+from . import arm_api
+from . import profile
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Login with Azure Tokens")
     main_token_group = parser.add_mutually_exclusive_group(required=True)
     main_token_group.add_argument(
         "-a", "--access-token",
         help="Access token for any Azure service.",
@@ -41,16 +39,19 @@
     tenant = args.tenant
 
 
     resp_subscriptions = []
     if access_tokens:
         t_infos = [TokenInformation(at) for at in access_tokens]
         for t_info in t_infos:
-            if t_info["aud"] == "https://management.core.windows.net/":
-                resp_subscriptions = request_subscriptions(t_info.access_token)
+            if t_info.endpoint == "https://management.core.windows.net/"\
+               or t_info["aud"] == "https://management.azure.com/":
+                resp_subscriptions = arm_api.list_subscriptions(
+                    t_info.access_token
+                )
                 break
     elif refresh_token:
         if not tenant:
             utils.eprint("--tenant required when using refresh token")
             return -1
         tenant_id = resolve_tenant_id(tenant)
         tokens = request_tokens_from_refresh(tenant_id, refresh_token)
@@ -62,15 +63,16 @@
             scope=tokens["scope"],
             client_info=tokens["client_info"],
             expires_in=tokens["expires_in"],
             ext_expires_in=tokens["ext_expires_in"],
         )
         t_infos = [at_info]
 
-    store_tokens(t_infos)
+    token_cache = load_token_cache()
+    store_tokens(t_infos, token_cache)
     set_subscriptions(t_infos[0], resp_subscriptions)
 
 
 
 
 # A simple implementation of Profile._set_subscriptions
 # https://github.com/Azure/azure-cli/blob/6771b2b1ef04ed2f8e71b636eccce5cf68a7d76d/src/azure-cli-core/azure/cli/core/_profile.py#L454
@@ -78,20 +80,21 @@
     default_subscription_id = store_profiles(at_info, resp_subscriptions)
     set_default_subscription_id(default_subscription_id)
 
 AZURE_CLOUD = "AzureCloud"
 
 def store_profiles(at_info, resp_subscriptions):
     tenant_id = at_info["tid"]
-    username = at_info["upn"]
-    user_type = at_info["idtyp"]
+    username = at_info.username
 
-    azure_profiles_path = "{}/.azure/azureProfile.json".format(os.environ["HOME"])
-    with codecs.open(azure_profiles_path, 'r', 'utf-8-sig') as fi:
-        profile_data = json.load(fi)
+    # To use tokens user type must be "user" since "servicePrincipal"
+    # is reserved to use the secrets store
+    user_type = "user"
+
+    profile_data = profile.load_profile()
 
     cached_subscriptions = {}
     for sub in profile_data["subscriptions"]:
         sub["isDefault"] = False
         cached_subscriptions[sub["id"]] = sub
 
 
@@ -105,15 +108,15 @@
             if is_default:
                 can_be_default = False
 
             new_subscriptions[sub_id] = {
                 "id": sub_id,
                 "name": rsub["displayName"],
                 "state": state,
-                "isDefault": s_is_default,
+                "isDefault": is_default,
                 "tenantId": tenant_id,
                 "environmentName": AZURE_CLOUD,
                 "user": {
                     "name": username,
                     "type": user_type,
                 }
             }
@@ -135,47 +138,27 @@
     default_subscription_id = [
         s["id"]
         for s in cached_subscriptions.values()
         if s["isDefault"]
     ][0]
     profile_data["subscriptions"] = list(cached_subscriptions.values())
 
-    with codecs.open(azure_profiles_path, 'w', 'utf-8-sig') as fo:
-        json.dump(profile_data, fo)
-
+    profile.store_profile(profile_data)
     return default_subscription_id
 
 def set_default_subscription_id(default_subscription_id):
     config_file = "{}/.azure/clouds.config".format(os.environ["HOME"])
     config = configparser.ConfigParser()
     config.read(config_file)
     config.set(AZURE_CLOUD, "subscription", default_subscription_id)
 
     with open(config_file, 'w') as fo:
         config.write(fo)
 
 
-def request_subscriptions(access_token):
-    headers = {
-        "Authorization": "Bearer {}".format(access_token)
-    }
-    resp = requests.get(
-        "https://management.azure.com/subscriptions?api-version=2019-11-01",
-        headers=headers,
-        # verify=False,
-    )
-
-    if resp.status_code != 200:
-        raise AzeError(
-            "Unable to get subscriptions response: error code {}".format(
-                resp.status_code
-        ))
-
-    return resp.json()["value"]
-
 AZCLI_ID = "04b07795-8ddb-461a-bbee-02f9e1bf7b46"
 
 def request_tokens_from_refresh(tenant_id, refresh_token):
     url = "https://login.microsoftonline.com/{}/oauth2/v2.0/token".format(
         tenant_id
     )
     data = {
@@ -191,29 +174,24 @@
     if resp.status_code != 200:
         raise AzeError(
             "Unable to get access token: error code {}".format(resp.status_code)
         )
 
     return resp.json()
 
-def store_tokens(tokens_info):
+
+def store_tokens(tokens_info, token_cache):
     if not tokens_info:
         return
 
     tokens_events = [create_event_from_token_info(t_info) for t_info in tokens_info]
-    token_cache = load_persisted_token_cache(
-        "{}/.azure/msal_token_cache.json".format(os.environ["HOME"]),
-        False
-    )
     for t_event in tokens_events:
         token_cache.add(t_event)
 
 
-
-
 class TokenInformation:
 
     def __init__(
             self,
             access_token,
             refresh_token=None,
             id_token=None,
@@ -232,16 +210,16 @@
         self.id_token = id_token
         self.refresh_token = refresh_token
 
         if client_info:
             self.client_info = client_info
         else:
             self.client_info = base64.b64encode(json.dumps({
-                "uid": self._info["oid"],
-                "utid": self._info["tid"],
+                "uid": self.account_id,
+                "utid": self.tenant_id,
             }).encode()).decode()
 
         now = int(time.time())
         if expires_in:
             self.expires_in = expires_in
         else:
             self.expires_in = int(self._info["exp"]) - now
@@ -252,33 +230,61 @@
             self.ext_expires_in = self.expires_in
 
 
     def __getitem__(self,key):
         return self._info[key]
 
     @property
-    def user_id(self):
-        return self._info["oid"]
+    def account_id(self):
+        if self._info["idtyp"] == "app":
+            return self._info["appid"]
+        else:
+            return self._info["oid"]
+
+    @property
+    def username(self):
+        if self._info["idtyp"] == "app":
+            return self._info["appid"]
+        else:
+            return self._info["upn"]
+
+    @property
+    def endpoint(self):
+        endpoint = self._info["aud"]
+
+        # Seems that management.azure.com is the new endpoint
+        # but still not used by Azure Cli, so we replace it
+        # for the old endpoint to make it compatible
+        if endpoint == "https://management.azure.com/":
+            return "https://management.core.windows.net/"
+        return endpoint
+
 
     @property
     def tenant_id(self):
         return self._info["tid"]
 
+    def get(self, *args, **kwargs):
+        return self._info.get(*args, **kwargs)
+
     @property
     def scopes(self):
         if self._scope:
             scopes = self._scope.split()
         else:
-            endpoint = self._info["aud"]
+            endpoint = self.endpoint
             scopes = ["{}/.default".format(endpoint)]
-            for scope in self._info["scp"].split():
-                if scope in ["email", "profile", "openid"]:
-                    scopes.append(scope)
-                else:
-                    scopes.append("{}/{}".format(endpoint, scope))
+            try:
+                for scope in self._info["scp"].split():
+                    if scope in ["email", "profile", "openid"]:
+                        scopes.append(scope)
+                    else:
+                        scopes.append("{}/{}".format(endpoint, scope))
+            except KeyError:
+                pass
         return scopes
 
 
 
 def create_event_from_token_info(t_info):
     scopes = t_info.scopes
     resp = {
@@ -291,45 +297,24 @@
     }
 
     if t_info.refresh_token:
         resp["refresh_token"] = t_info.refresh_token
     if t_info.id_token:
         resp["id_token"] = t_info.id_token
 
-    client_id = t_info["appid"]
-    username = t_info["upn"]
+    # No matter what is t_info["appid"] since we tell the Azure Cli
+    # to use the token as it belongs to it
+    client_id = AZCLI_ID
+    username = t_info.username
     tenant_id = t_info.tenant_id
     return {
         "username": username,
         "environment": "login.microsoftonline.com",
         "client_id": client_id,
         "scope": scopes,
         "token_endpoint": "https://login.microsoftonline.com/{}".format(tenant_id),
         "grant_type": "",
         "response": resp,
         # "params": {},
         # "data": {},
     }
 
-def load_persisted_token_cache(location, encrypt):
-    persistence = build_persistence(location, encrypt)
-    return PersistedTokenCache(persistence)
-
-def build_persistence(location, encrypt):
-    if encrypt:
-        if sys.platform.startswith('win'):
-            return FilePersistenceWithDataProtection(location)
-        if sys.platform.startswith('darwin'):
-            return KeychainPersistence(
-                location,
-                "my_service_name",
-                "my_account_name"
-            )
-        if sys.platform.startswith('linux'):
-            return LibsecretPersistence(
-                location,
-                schema_name="my_schema_name",
-                attributes={"my_attr1": "foo", "my_attr2": "bar"}
-            )
-    else:
-        return FilePersistence(location)
-
```

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_tenant_id.py` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_tenant_id.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/read_in.py` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/read_in.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/utils.py` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/utils.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/entry_points.txt` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/entry_points.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,10 +2,12 @@
 az-brute-passwords = aze.az_brute_passwords:main
 az-brute-service-subdomains = aze.az_brute_service_subdomains:main
 az-brute-usernames = aze.az_brute_usernames:main
 az-get-login-info = aze.az_get_login_info:main
 az-get-tenant-domains = aze.az_get_tenant_domains:main
 az-get-tenant-id = aze.az_get_tenant_id:main
 az-inspect-token = aze.az_inspect_token:main
+az-list-role-assignment = aze.az_list_role_assignment:main
+az-list-subscriptions = aze.az_list_subscriptions:main
 az-login-with-token = aze.az_login_with_token:main
 az-search-token-in-cache = aze.az_search_token_in_cache:main
 az-whoami = aze.az_whoami:main
```

### Comparing `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/setup.py` & `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/setup.py`

 * *Files identical despite different names*

