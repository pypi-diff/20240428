# Comparing `tmp/pierskarsenbarg_pulumi_sdm-1.8.0.tar.gz` & `tmp/pierskarsenbarg_pulumi_sdm-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pierskarsenbarg_pulumi_sdm-1.8.0.tar", last modified: Mon Nov 27 14:43:48 2023, max compression
+gzip compressed data, was "pierskarsenbarg_pulumi_sdm-1.9.0.tar", last modified: Tue Apr  9 10:48:43 2024, max compression
```

## Comparing `pierskarsenbarg_pulumi_sdm-1.8.0.tar` & `pierskarsenbarg_pulumi_sdm-1.9.0.tar`

### file list

```diff
@@ -1,53 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:43:48.000000 pierskarsenbarg_pulumi_sdm-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2023-11-27 14:43:48.000000 pierskarsenbarg_pulumi_sdm-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:43:48.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   780057 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/account_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:43:48.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    10341 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_peering_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_peering_group_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_peering_group_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_peering_group_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     8564 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     9022 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_workflow_approver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_workflow_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/node.py
--rw-r--r--   0 runner    (1001) docker     (127)  1344098 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/peering_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/peering_group_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/peering_group_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/peering_group_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10596 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)   153256 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12958 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    23150 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/secret_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    20304 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/workflow_approver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/workflow_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:43:48.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2023-11-27 14:43:48.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-11-27 14:43:48.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 14:43:48.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 14:43:48.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-27 14:43:48.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-27 14:43:48.000000 pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 14:43:48.000000 pierskarsenbarg_pulumi_sdm-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-11-27 14:43:47.000000 pierskarsenbarg_pulumi_sdm-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:48:43.648919 pierskarsenbarg_pulumi_sdm-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 10:48:43.648919 pierskarsenbarg_pulumi_sdm-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:48:43.644919 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   828219 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/account_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/approval_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/approval_workflow_approval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/approval_workflow_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:48:43.648919 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_approval_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_approval_workflow_approver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_approval_workflow_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_peering_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_peering_group_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_peering_group_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_peering_group_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10218 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_workflow_approver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_workflow_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1440147 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/peering_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/peering_group_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/peering_group_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/peering_group_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154782 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41162 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22859 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10804 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/workflow_approver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/workflow_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:48:43.648919 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:48:43.648919 pierskarsenbarg_pulumi_sdm-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-09 10:48:43.000000 pierskarsenbarg_pulumi_sdm-1.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/PKG-INFO` & `pierskarsenbarg_pulumi_sdm-1.9.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 Metadata-Version: 2.1
 Name: pierskarsenbarg_pulumi_sdm
-Version: 1.8.0
+Version: 1.9.0
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
-Description: # StrongDM Resource Provider
-        
-        The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
-        
-        ## Installing
-        
-        This package is available for several languages/platforms:
-        
-        ### Node.js (JavaScript/TypeScript)
-        
-        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-        
-        ```bash
-        npm install @pierskarsenbarg/sdm
-        ```
-        
-        or `yarn`:
-        
-        ```bash
-        yarn add @pierskarsenbarg/sdm
-        ```
-        
-        ### Python
-        
-        To use from Python, install using `pip`:
-        
-        ```bash
-        pip install pierskarsenbarg-pulumi-sdm
-        ```
-        
-        ### Go
-        
-        To use from Go, use `go get` to grab the latest version of the library:
-        
-        ```bash
-        go get github.com/pierskarsenbarg/pulumi-sdm/sdk/go/...
-        ```
-        
-        ### .NET
-        
-        To use from .NET, install using `dotnet add package`:
-        
-        ```bash
-        dotnet add package PiersKarsenbarg.Sdm
-        ```
-        
-        ## Configuration
-        
-        The following configuration points are available for the `sdm` provider:
-        
-        - `sdm:apiAccessKey` (environment: `SDM_API_ACCESS_KEY`) - the API key for `Strong DM`
-        - `sdm:apiSecretKey` (environment: `SDM_API_SECRET_KEY`) - the corresponding secret key for the above API key
-        
-        ## Todo
-        
-        * Add Java language support
-        * Add YAML language support
-        
-        <!-- ## Reference
-        
-        For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/). -->
-        
 Keywords: pulumi sdm category/cloud
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+# StrongDM Resource Provider
+
+The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
+
+## Installing
+
+This package is available for several languages/platforms:
+
+### Node.js (JavaScript/TypeScript)
+
+To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+
+```bash
+npm install @pierskarsenbarg/sdm
+```
+
+or `yarn`:
+
+```bash
+yarn add @pierskarsenbarg/sdm
+```
+
+### Python
+
+To use from Python, install using `pip`:
+
+```bash
+pip install pierskarsenbarg-pulumi-sdm
+```
+
+### Go
+
+To use from Go, use `go get` to grab the latest version of the library:
+
+```bash
+go get github.com/pierskarsenbarg/pulumi-sdm/sdk/go/...
+```
+
+### .NET
+
+To use from .NET, install using `dotnet add package`:
+
+```bash
+dotnet add package PiersKarsenbarg.Sdm
+```
+
+## Configuration
+
+The following configuration points are available for the `sdm` provider:
+
+- `sdm:apiAccessKey` (environment: `SDM_API_ACCESS_KEY`) - the API key for `Strong DM`
+- `sdm:apiSecretKey` (environment: `SDM_API_SECRET_KEY`) - the corresponding secret key for the above API key
+
+## Todo
+
+* Add Java language support
+* Add YAML language support
+
+<!-- ## Reference
+
+For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/). -->
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/README.md` & `pierskarsenbarg_pulumi_sdm-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/__init__.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,16 +3,22 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .account import *
 from .account_attachment import *
+from .approval_workflow import *
+from .approval_workflow_approval import *
+from .approval_workflow_step import *
 from .get_account import *
 from .get_account_attachment import *
+from .get_approval_workflow import *
+from .get_approval_workflow_approver import *
+from .get_approval_workflow_step import *
 from .get_node import *
 from .get_peering_group import *
 from .get_peering_group_node import *
 from .get_peering_group_peer import *
 from .get_peering_group_resource import *
 from .get_remote_identity import *
 from .get_remote_identity_group import *
@@ -63,14 +69,38 @@
   "fqn": "pierskarsenbarg_pulumi_sdm",
   "classes": {
    "sdm:index/accountAttachment:AccountAttachment": "AccountAttachment"
   }
  },
  {
   "pkg": "sdm",
+  "mod": "index/approvalWorkflow",
+  "fqn": "pierskarsenbarg_pulumi_sdm",
+  "classes": {
+   "sdm:index/approvalWorkflow:ApprovalWorkflow": "ApprovalWorkflow"
+  }
+ },
+ {
+  "pkg": "sdm",
+  "mod": "index/approvalWorkflowApproval",
+  "fqn": "pierskarsenbarg_pulumi_sdm",
+  "classes": {
+   "sdm:index/approvalWorkflowApproval:ApprovalWorkflowApproval": "ApprovalWorkflowApproval"
+  }
+ },
+ {
+  "pkg": "sdm",
+  "mod": "index/approvalWorkflowStep",
+  "fqn": "pierskarsenbarg_pulumi_sdm",
+  "classes": {
+   "sdm:index/approvalWorkflowStep:ApprovalWorkflowStep": "ApprovalWorkflowStep"
+  }
+ },
+ {
+  "pkg": "sdm",
   "mod": "index/node",
   "fqn": "pierskarsenbarg_pulumi_sdm",
   "classes": {
    "sdm:index/node:Node": "Node"
   }
  },
  {
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/_inputs.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     'ResourceNeptuneIamArgs',
     'ResourceOracleArgs',
     'ResourcePostgresArgs',
     'ResourcePrestoArgs',
     'ResourceRabbitmqAmqp091Args',
     'ResourceRawTcpArgs',
     'ResourceRdpArgs',
+    'ResourceRdpCertArgs',
     'ResourceRdsPostgresIamArgs',
     'ResourceRedisArgs',
     'ResourceRedshiftArgs',
     'ResourceSingleStoreArgs',
     'ResourceSnowflakeArgs',
     'ResourceSnowsightArgs',
     'ResourceSqlServerArgs',
@@ -95,36 +96,45 @@
     'ResourceSshArgs',
     'ResourceSshCertArgs',
     'ResourceSshCustomerKeyArgs',
     'ResourceSybaseArgs',
     'ResourceSybaseIqArgs',
     'ResourceTeradataArgs',
     'ResourceTrinoArgs',
+    'SecretStoreActiveDirectoryStoreArgs',
     'SecretStoreAwsArgs',
+    'SecretStoreAwsCertX509Args',
     'SecretStoreAzureStoreArgs',
     'SecretStoreCyberarkConjurArgs',
     'SecretStoreCyberarkPamArgs',
     'SecretStoreCyberarkPamExperimentalArgs',
     'SecretStoreDelineaStoreArgs',
+    'SecretStoreGcpCertX509StoreArgs',
     'SecretStoreGcpStoreArgs',
     'SecretStoreVaultApproleArgs',
+    'SecretStoreVaultApproleCertSshArgs',
+    'SecretStoreVaultApproleCertX509Args',
     'SecretStoreVaultTlsArgs',
+    'SecretStoreVaultTlsCertSshArgs',
+    'SecretStoreVaultTlsCertX509Args',
     'SecretStoreVaultTokenArgs',
+    'SecretStoreVaultTokenCertSshArgs',
+    'SecretStoreVaultTokenCertX509Args',
 ]
 
 @pulumi.input_type
 class AccountServiceArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  suspended: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  token: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Service.
-        :param pulumi.Input[bool] suspended: The User's suspended state.
+        :param pulumi.Input[bool] suspended: The Service's suspended state.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         if suspended is not None:
             pulumi.set(__self__, "suspended", suspended)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
@@ -143,15 +153,15 @@
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def suspended(self) -> Optional[pulumi.Input[bool]]:
         """
-        The User's suspended state.
+        The Service's suspended state.
         """
         return pulumi.get(self, "suspended")
 
     @suspended.setter
     def suspended(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "suspended", value)
 
@@ -190,16 +200,16 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] email: The User's email address. Must be unique.
         :param pulumi.Input[str] first_name: The User's first name.
         :param pulumi.Input[str] last_name: The User's last name.
         :param pulumi.Input[str] external_id: External ID is an alternative unique ID this user is represented by within an external service.
         :param pulumi.Input[str] managed_by: Managed By is a read only field for what service manages this user, e.g. StrongDM, Okta, Azure.
-        :param pulumi.Input[str] permission_level: PermissionLevel is a read only field for the user's permission level e.g. admin, DBA, user.
-        :param pulumi.Input[bool] suspended: The User's suspended state.
+        :param pulumi.Input[str] permission_level: PermissionLevel is the user's permission level e.g. admin, DBA, user.
+        :param pulumi.Input[bool] suspended: The Service's suspended state.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "email", email)
         pulumi.set(__self__, "first_name", first_name)
         pulumi.set(__self__, "last_name", last_name)
         if external_id is not None:
             pulumi.set(__self__, "external_id", external_id)
@@ -272,27 +282,27 @@
     def managed_by(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "managed_by", value)
 
     @property
     @pulumi.getter(name="permissionLevel")
     def permission_level(self) -> Optional[pulumi.Input[str]]:
         """
-        PermissionLevel is a read only field for the user's permission level e.g. admin, DBA, user.
+        PermissionLevel is the user's permission level e.g. admin, DBA, user.
         """
         return pulumi.get(self, "permission_level")
 
     @permission_level.setter
     def permission_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "permission_level", value)
 
     @property
     @pulumi.getter
     def suspended(self) -> Optional[pulumi.Input[bool]]:
         """
-        The User's suspended state.
+        The Service's suspended state.
         """
         return pulumi.get(self, "suspended")
 
     @suspended.setter
     def suspended(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "suspended", value)
 
@@ -14842,14 +14852,211 @@
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
 
 @pulumi.input_type
+class ResourceRdpCertArgs:
+    def __init__(__self__, *,
+                 hostname: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 bind_interface: Optional[pulumi.Input[str]] = None,
+                 egress_filter: Optional[pulumi.Input[str]] = None,
+                 port: Optional[pulumi.Input[int]] = None,
+                 port_override: Optional[pulumi.Input[int]] = None,
+                 remote_identity_group_id: Optional[pulumi.Input[str]] = None,
+                 remote_identity_healthcheck_username: Optional[pulumi.Input[str]] = None,
+                 secret_store_id: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] hostname: The host to dial to initiate a connection from the egress node to this resource.
+        :param pulumi.Input[str] name: Unique human-readable name of the Resource.
+        :param pulumi.Input[str] bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param pulumi.Input[int] port: The port to dial to initiate a connection from the egress node to this resource.
+        :param pulumi.Input[int] port_override: The local port used by clients to connect to this resource.
+        :param pulumi.Input[str] remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param pulumi.Input[str] remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        :param pulumi.Input[str] username: The username to authenticate with.
+        """
+        pulumi.set(__self__, "hostname", hostname)
+        pulumi.set(__self__, "name", name)
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
+        if remote_identity_group_id is not None:
+            pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
+        if remote_identity_healthcheck_username is not None:
+            pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def hostname(self) -> pulumi.Input[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
+        return pulumi.get(self, "hostname")
+
+    @hostname.setter
+    def hostname(self, value: pulumi.Input[str]):
+        pulumi.set(self, "hostname", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[pulumi.Input[str]]:
+        """
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @bind_interface.setter
+    def bind_interface(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "bind_interface", value)
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[pulumi.Input[str]]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @egress_filter.setter
+    def egress_filter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "egress_filter", value)
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[pulumi.Input[int]]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
+        return pulumi.get(self, "port")
+
+    @port.setter
+    def port(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port", value)
+
+    @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[pulumi.Input[int]]:
+        """
+        The local port used by clients to connect to this resource.
+        """
+        return pulumi.get(self, "port_override")
+
+    @port_override.setter
+    def port_override(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port_override", value)
+
+    @property
+    @pulumi.getter(name="remoteIdentityGroupId")
+    def remote_identity_group_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
+        return pulumi.get(self, "remote_identity_group_id")
+
+    @remote_identity_group_id.setter
+    def remote_identity_group_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "remote_identity_group_id", value)
+
+    @property
+    @pulumi.getter(name="remoteIdentityHealthcheckUsername")
+    def remote_identity_healthcheck_username(self) -> Optional[pulumi.Input[str]]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
+        return pulumi.get(self, "remote_identity_healthcheck_username")
+
+    @remote_identity_healthcheck_username.setter
+    def remote_identity_healthcheck_username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "remote_identity_healthcheck_username", value)
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @secret_store_id.setter
+    def secret_store_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_id", value)
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[pulumi.Input[str]]:
+        """
+        The username to authenticate with.
+        """
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
+
+
+@pulumi.input_type
 class ResourceRdsPostgresIamArgs:
     def __init__(__self__, *,
                  database: pulumi.Input[str],
                  hostname: pulumi.Input[str],
                  name: pulumi.Input[str],
                  region: pulumi.Input[str],
                  bind_interface: Optional[pulumi.Input[str]] = None,
@@ -18275,14 +18482,67 @@
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
 
 @pulumi.input_type
+class SecretStoreActiveDirectoryStoreArgs:
+    def __init__(__self__, *,
+                 name: pulumi.Input[str],
+                 server_address: pulumi.Input[str],
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
+        :param pulumi.Input[str] server_address: The URL of the Vault to target
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "server_address", server_address)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> pulumi.Input[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @server_address.setter
+    def server_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "server_address", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+
+@pulumi.input_type
 class SecretStoreAwsArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  region: pulumi.Input[str],
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
@@ -18328,14 +18588,127 @@
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
 
 @pulumi.input_type
+class SecretStoreAwsCertX509Args:
+    def __init__(__self__, *,
+                 ca_arn: pulumi.Input[str],
+                 certificate_template_arn: pulumi.Input[str],
+                 issued_cert_ttl_minutes: pulumi.Input[int],
+                 name: pulumi.Input[str],
+                 region: pulumi.Input[str],
+                 signing_algo: pulumi.Input[str],
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] ca_arn: The ARN of the CA in AWS Private CA
+        :param pulumi.Input[str] certificate_template_arn: The ARN of the AWS certificate template for requested certificates. Must allow SAN, key usage, and ext key usage passthrough from CSR
+        :param pulumi.Input[int] issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
+        :param pulumi.Input[str] region: The AWS region to target e.g. us-east-1
+        :param pulumi.Input[str] signing_algo: The specified signing algorithm family (RSA or ECDSA) must match the algorithm family of the CA's secret key. e.g. SHA256WITHRSA
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "ca_arn", ca_arn)
+        pulumi.set(__self__, "certificate_template_arn", certificate_template_arn)
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "signing_algo", signing_algo)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="caArn")
+    def ca_arn(self) -> pulumi.Input[str]:
+        """
+        The ARN of the CA in AWS Private CA
+        """
+        return pulumi.get(self, "ca_arn")
+
+    @ca_arn.setter
+    def ca_arn(self, value: pulumi.Input[str]):
+        pulumi.set(self, "ca_arn", value)
+
+    @property
+    @pulumi.getter(name="certificateTemplateArn")
+    def certificate_template_arn(self) -> pulumi.Input[str]:
+        """
+        The ARN of the AWS certificate template for requested certificates. Must allow SAN, key usage, and ext key usage passthrough from CSR
+        """
+        return pulumi.get(self, "certificate_template_arn")
+
+    @certificate_template_arn.setter
+    def certificate_template_arn(self, value: pulumi.Input[str]):
+        pulumi.set(self, "certificate_template_arn", value)
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> pulumi.Input[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @issued_cert_ttl_minutes.setter
+    def issued_cert_ttl_minutes(self, value: pulumi.Input[int]):
+        pulumi.set(self, "issued_cert_ttl_minutes", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def region(self) -> pulumi.Input[str]:
+        """
+        The AWS region to target e.g. us-east-1
+        """
+        return pulumi.get(self, "region")
+
+    @region.setter
+    def region(self, value: pulumi.Input[str]):
+        pulumi.set(self, "region", value)
+
+    @property
+    @pulumi.getter(name="signingAlgo")
+    def signing_algo(self) -> pulumi.Input[str]:
+        """
+        The specified signing algorithm family (RSA or ECDSA) must match the algorithm family of the CA's secret key. e.g. SHA256WITHRSA
+        """
+        return pulumi.get(self, "signing_algo")
+
+    @signing_algo.setter
+    def signing_algo(self, value: pulumi.Input[str]):
+        pulumi.set(self, "signing_algo", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+
+@pulumi.input_type
 class SecretStoreAzureStoreArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  vault_uri: pulumi.Input[str],
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
@@ -18614,14 +18987,128 @@
 
     @tenant_name.setter
     def tenant_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tenant_name", value)
 
 
 @pulumi.input_type
+class SecretStoreGcpCertX509StoreArgs:
+    def __init__(__self__, *,
+                 ca_pool_id: pulumi.Input[str],
+                 issued_cert_ttl_minutes: pulumi.Input[int],
+                 location: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 project_id: pulumi.Input[str],
+                 ca_id: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] ca_pool_id: The ID of the target CA pool
+        :param pulumi.Input[int] issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param pulumi.Input[str] location: The Region for the CA in GCP format e.g. us-west1
+        :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
+        :param pulumi.Input[str] project_id: The GCP project ID to target.
+        :param pulumi.Input[str] ca_id: The ID of the target CA
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "ca_pool_id", ca_pool_id)
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "location", location)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "project_id", project_id)
+        if ca_id is not None:
+            pulumi.set(__self__, "ca_id", ca_id)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="caPoolId")
+    def ca_pool_id(self) -> pulumi.Input[str]:
+        """
+        The ID of the target CA pool
+        """
+        return pulumi.get(self, "ca_pool_id")
+
+    @ca_pool_id.setter
+    def ca_pool_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "ca_pool_id", value)
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> pulumi.Input[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @issued_cert_ttl_minutes.setter
+    def issued_cert_ttl_minutes(self, value: pulumi.Input[int]):
+        pulumi.set(self, "issued_cert_ttl_minutes", value)
+
+    @property
+    @pulumi.getter
+    def location(self) -> pulumi.Input[str]:
+        """
+        The Region for the CA in GCP format e.g. us-west1
+        """
+        return pulumi.get(self, "location")
+
+    @location.setter
+    def location(self, value: pulumi.Input[str]):
+        pulumi.set(self, "location", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> pulumi.Input[str]:
+        """
+        The GCP project ID to target.
+        """
+        return pulumi.get(self, "project_id")
+
+    @project_id.setter
+    def project_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project_id", value)
+
+    @property
+    @pulumi.getter(name="caId")
+    def ca_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of the target CA
+        """
+        return pulumi.get(self, "ca_id")
+
+    @ca_id.setter
+    def ca_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ca_id", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+
+@pulumi.input_type
 class SecretStoreGcpStoreArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  project_id: pulumi.Input[str],
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
@@ -18736,14 +19223,242 @@
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
 
 @pulumi.input_type
+class SecretStoreVaultApproleCertSshArgs:
+    def __init__(__self__, *,
+                 issued_cert_ttl_minutes: pulumi.Input[int],
+                 name: pulumi.Input[str],
+                 server_address: pulumi.Input[str],
+                 signing_role: pulumi.Input[str],
+                 ssh_mount_point: pulumi.Input[str],
+                 namespace: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[int] issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
+        :param pulumi.Input[str] server_address: The URL of the Vault to target
+        :param pulumi.Input[str] signing_role: The signing role to be used for signing certificates
+        :param pulumi.Input[str] ssh_mount_point: The mount point of the SSH engine configured with the desired CA
+        :param pulumi.Input[str] namespace: The namespace to make requests within
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "server_address", server_address)
+        pulumi.set(__self__, "signing_role", signing_role)
+        pulumi.set(__self__, "ssh_mount_point", ssh_mount_point)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> pulumi.Input[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @issued_cert_ttl_minutes.setter
+    def issued_cert_ttl_minutes(self, value: pulumi.Input[int]):
+        pulumi.set(self, "issued_cert_ttl_minutes", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> pulumi.Input[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @server_address.setter
+    def server_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "server_address", value)
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> pulumi.Input[str]:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @signing_role.setter
+    def signing_role(self, value: pulumi.Input[str]):
+        pulumi.set(self, "signing_role", value)
+
+    @property
+    @pulumi.getter(name="sshMountPoint")
+    def ssh_mount_point(self) -> pulumi.Input[str]:
+        """
+        The mount point of the SSH engine configured with the desired CA
+        """
+        return pulumi.get(self, "ssh_mount_point")
+
+    @ssh_mount_point.setter
+    def ssh_mount_point(self, value: pulumi.Input[str]):
+        pulumi.set(self, "ssh_mount_point", value)
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[pulumi.Input[str]]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @namespace.setter
+    def namespace(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "namespace", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+
+@pulumi.input_type
+class SecretStoreVaultApproleCertX509Args:
+    def __init__(__self__, *,
+                 issued_cert_ttl_minutes: pulumi.Input[int],
+                 name: pulumi.Input[str],
+                 pki_mount_point: pulumi.Input[str],
+                 server_address: pulumi.Input[str],
+                 signing_role: pulumi.Input[str],
+                 namespace: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[int] issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
+        :param pulumi.Input[str] pki_mount_point: The mount point of the PKI engine configured with the desired CA
+        :param pulumi.Input[str] server_address: The URL of the Vault to target
+        :param pulumi.Input[str] signing_role: The signing role to be used for signing certificates
+        :param pulumi.Input[str] namespace: The namespace to make requests within
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "pki_mount_point", pki_mount_point)
+        pulumi.set(__self__, "server_address", server_address)
+        pulumi.set(__self__, "signing_role", signing_role)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> pulumi.Input[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @issued_cert_ttl_minutes.setter
+    def issued_cert_ttl_minutes(self, value: pulumi.Input[int]):
+        pulumi.set(self, "issued_cert_ttl_minutes", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="pkiMountPoint")
+    def pki_mount_point(self) -> pulumi.Input[str]:
+        """
+        The mount point of the PKI engine configured with the desired CA
+        """
+        return pulumi.get(self, "pki_mount_point")
+
+    @pki_mount_point.setter
+    def pki_mount_point(self, value: pulumi.Input[str]):
+        pulumi.set(self, "pki_mount_point", value)
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> pulumi.Input[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @server_address.setter
+    def server_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "server_address", value)
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> pulumi.Input[str]:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @signing_role.setter
+    def signing_role(self, value: pulumi.Input[str]):
+        pulumi.set(self, "signing_role", value)
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[pulumi.Input[str]]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @namespace.setter
+    def namespace(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "namespace", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+
+@pulumi.input_type
 class SecretStoreVaultTlsArgs:
     def __init__(__self__, *,
                  client_cert_path: pulumi.Input[str],
                  client_key_path: pulumi.Input[str],
                  name: pulumi.Input[str],
                  server_address: pulumi.Input[str],
                  ca_cert_path: Optional[pulumi.Input[str]] = None,
@@ -18851,14 +19566,334 @@
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
 
 @pulumi.input_type
+class SecretStoreVaultTlsCertSshArgs:
+    def __init__(__self__, *,
+                 client_cert_path: pulumi.Input[str],
+                 client_key_path: pulumi.Input[str],
+                 issued_cert_ttl_minutes: pulumi.Input[int],
+                 name: pulumi.Input[str],
+                 server_address: pulumi.Input[str],
+                 signing_role: pulumi.Input[str],
+                 ssh_mount_point: pulumi.Input[str],
+                 ca_cert_path: Optional[pulumi.Input[str]] = None,
+                 namespace: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] client_cert_path: A path to a client certificate file accessible by a Node
+        :param pulumi.Input[str] client_key_path: A path to a client key file accessible by a Node
+        :param pulumi.Input[int] issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
+        :param pulumi.Input[str] server_address: The URL of the Vault to target
+        :param pulumi.Input[str] signing_role: The signing role to be used for signing certificates
+        :param pulumi.Input[str] ssh_mount_point: The mount point of the SSH engine configured with the desired CA
+        :param pulumi.Input[str] ca_cert_path: A path to a CA file accessible by a Node
+        :param pulumi.Input[str] namespace: The namespace to make requests within
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "client_cert_path", client_cert_path)
+        pulumi.set(__self__, "client_key_path", client_key_path)
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "server_address", server_address)
+        pulumi.set(__self__, "signing_role", signing_role)
+        pulumi.set(__self__, "ssh_mount_point", ssh_mount_point)
+        if ca_cert_path is not None:
+            pulumi.set(__self__, "ca_cert_path", ca_cert_path)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="clientCertPath")
+    def client_cert_path(self) -> pulumi.Input[str]:
+        """
+        A path to a client certificate file accessible by a Node
+        """
+        return pulumi.get(self, "client_cert_path")
+
+    @client_cert_path.setter
+    def client_cert_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "client_cert_path", value)
+
+    @property
+    @pulumi.getter(name="clientKeyPath")
+    def client_key_path(self) -> pulumi.Input[str]:
+        """
+        A path to a client key file accessible by a Node
+        """
+        return pulumi.get(self, "client_key_path")
+
+    @client_key_path.setter
+    def client_key_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "client_key_path", value)
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> pulumi.Input[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @issued_cert_ttl_minutes.setter
+    def issued_cert_ttl_minutes(self, value: pulumi.Input[int]):
+        pulumi.set(self, "issued_cert_ttl_minutes", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> pulumi.Input[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @server_address.setter
+    def server_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "server_address", value)
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> pulumi.Input[str]:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @signing_role.setter
+    def signing_role(self, value: pulumi.Input[str]):
+        pulumi.set(self, "signing_role", value)
+
+    @property
+    @pulumi.getter(name="sshMountPoint")
+    def ssh_mount_point(self) -> pulumi.Input[str]:
+        """
+        The mount point of the SSH engine configured with the desired CA
+        """
+        return pulumi.get(self, "ssh_mount_point")
+
+    @ssh_mount_point.setter
+    def ssh_mount_point(self, value: pulumi.Input[str]):
+        pulumi.set(self, "ssh_mount_point", value)
+
+    @property
+    @pulumi.getter(name="caCertPath")
+    def ca_cert_path(self) -> Optional[pulumi.Input[str]]:
+        """
+        A path to a CA file accessible by a Node
+        """
+        return pulumi.get(self, "ca_cert_path")
+
+    @ca_cert_path.setter
+    def ca_cert_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ca_cert_path", value)
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[pulumi.Input[str]]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @namespace.setter
+    def namespace(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "namespace", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+
+@pulumi.input_type
+class SecretStoreVaultTlsCertX509Args:
+    def __init__(__self__, *,
+                 client_cert_path: pulumi.Input[str],
+                 client_key_path: pulumi.Input[str],
+                 issued_cert_ttl_minutes: pulumi.Input[int],
+                 name: pulumi.Input[str],
+                 pki_mount_point: pulumi.Input[str],
+                 server_address: pulumi.Input[str],
+                 signing_role: pulumi.Input[str],
+                 ca_cert_path: Optional[pulumi.Input[str]] = None,
+                 namespace: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] client_cert_path: A path to a client certificate file accessible by a Node
+        :param pulumi.Input[str] client_key_path: A path to a client key file accessible by a Node
+        :param pulumi.Input[int] issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
+        :param pulumi.Input[str] pki_mount_point: The mount point of the PKI engine configured with the desired CA
+        :param pulumi.Input[str] server_address: The URL of the Vault to target
+        :param pulumi.Input[str] signing_role: The signing role to be used for signing certificates
+        :param pulumi.Input[str] ca_cert_path: A path to a CA file accessible by a Node
+        :param pulumi.Input[str] namespace: The namespace to make requests within
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "client_cert_path", client_cert_path)
+        pulumi.set(__self__, "client_key_path", client_key_path)
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "pki_mount_point", pki_mount_point)
+        pulumi.set(__self__, "server_address", server_address)
+        pulumi.set(__self__, "signing_role", signing_role)
+        if ca_cert_path is not None:
+            pulumi.set(__self__, "ca_cert_path", ca_cert_path)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="clientCertPath")
+    def client_cert_path(self) -> pulumi.Input[str]:
+        """
+        A path to a client certificate file accessible by a Node
+        """
+        return pulumi.get(self, "client_cert_path")
+
+    @client_cert_path.setter
+    def client_cert_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "client_cert_path", value)
+
+    @property
+    @pulumi.getter(name="clientKeyPath")
+    def client_key_path(self) -> pulumi.Input[str]:
+        """
+        A path to a client key file accessible by a Node
+        """
+        return pulumi.get(self, "client_key_path")
+
+    @client_key_path.setter
+    def client_key_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "client_key_path", value)
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> pulumi.Input[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @issued_cert_ttl_minutes.setter
+    def issued_cert_ttl_minutes(self, value: pulumi.Input[int]):
+        pulumi.set(self, "issued_cert_ttl_minutes", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="pkiMountPoint")
+    def pki_mount_point(self) -> pulumi.Input[str]:
+        """
+        The mount point of the PKI engine configured with the desired CA
+        """
+        return pulumi.get(self, "pki_mount_point")
+
+    @pki_mount_point.setter
+    def pki_mount_point(self, value: pulumi.Input[str]):
+        pulumi.set(self, "pki_mount_point", value)
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> pulumi.Input[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @server_address.setter
+    def server_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "server_address", value)
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> pulumi.Input[str]:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @signing_role.setter
+    def signing_role(self, value: pulumi.Input[str]):
+        pulumi.set(self, "signing_role", value)
+
+    @property
+    @pulumi.getter(name="caCertPath")
+    def ca_cert_path(self) -> Optional[pulumi.Input[str]]:
+        """
+        A path to a CA file accessible by a Node
+        """
+        return pulumi.get(self, "ca_cert_path")
+
+    @ca_cert_path.setter
+    def ca_cert_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ca_cert_path", value)
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[pulumi.Input[str]]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @namespace.setter
+    def namespace(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "namespace", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+
+@pulumi.input_type
 class SecretStoreVaultTokenArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  server_address: pulumi.Input[str],
                  namespace: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
@@ -18900,14 +19935,242 @@
 
     @property
     @pulumi.getter
     def namespace(self) -> Optional[pulumi.Input[str]]:
         """
         The namespace to make requests within
         """
+        return pulumi.get(self, "namespace")
+
+    @namespace.setter
+    def namespace(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "namespace", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+
+@pulumi.input_type
+class SecretStoreVaultTokenCertSshArgs:
+    def __init__(__self__, *,
+                 issued_cert_ttl_minutes: pulumi.Input[int],
+                 name: pulumi.Input[str],
+                 server_address: pulumi.Input[str],
+                 signing_role: pulumi.Input[str],
+                 ssh_mount_point: pulumi.Input[str],
+                 namespace: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[int] issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
+        :param pulumi.Input[str] server_address: The URL of the Vault to target
+        :param pulumi.Input[str] signing_role: The signing role to be used for signing certificates
+        :param pulumi.Input[str] ssh_mount_point: The mount point of the SSH engine configured with the desired CA
+        :param pulumi.Input[str] namespace: The namespace to make requests within
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "server_address", server_address)
+        pulumi.set(__self__, "signing_role", signing_role)
+        pulumi.set(__self__, "ssh_mount_point", ssh_mount_point)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> pulumi.Input[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @issued_cert_ttl_minutes.setter
+    def issued_cert_ttl_minutes(self, value: pulumi.Input[int]):
+        pulumi.set(self, "issued_cert_ttl_minutes", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> pulumi.Input[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @server_address.setter
+    def server_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "server_address", value)
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> pulumi.Input[str]:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @signing_role.setter
+    def signing_role(self, value: pulumi.Input[str]):
+        pulumi.set(self, "signing_role", value)
+
+    @property
+    @pulumi.getter(name="sshMountPoint")
+    def ssh_mount_point(self) -> pulumi.Input[str]:
+        """
+        The mount point of the SSH engine configured with the desired CA
+        """
+        return pulumi.get(self, "ssh_mount_point")
+
+    @ssh_mount_point.setter
+    def ssh_mount_point(self, value: pulumi.Input[str]):
+        pulumi.set(self, "ssh_mount_point", value)
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[pulumi.Input[str]]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @namespace.setter
+    def namespace(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "namespace", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+
+@pulumi.input_type
+class SecretStoreVaultTokenCertX509Args:
+    def __init__(__self__, *,
+                 issued_cert_ttl_minutes: pulumi.Input[int],
+                 name: pulumi.Input[str],
+                 pki_mount_point: pulumi.Input[str],
+                 server_address: pulumi.Input[str],
+                 signing_role: pulumi.Input[str],
+                 namespace: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[int] issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
+        :param pulumi.Input[str] pki_mount_point: The mount point of the PKI engine configured with the desired CA
+        :param pulumi.Input[str] server_address: The URL of the Vault to target
+        :param pulumi.Input[str] signing_role: The signing role to be used for signing certificates
+        :param pulumi.Input[str] namespace: The namespace to make requests within
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "pki_mount_point", pki_mount_point)
+        pulumi.set(__self__, "server_address", server_address)
+        pulumi.set(__self__, "signing_role", signing_role)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> pulumi.Input[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @issued_cert_ttl_minutes.setter
+    def issued_cert_ttl_minutes(self, value: pulumi.Input[int]):
+        pulumi.set(self, "issued_cert_ttl_minutes", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="pkiMountPoint")
+    def pki_mount_point(self) -> pulumi.Input[str]:
+        """
+        The mount point of the PKI engine configured with the desired CA
+        """
+        return pulumi.get(self, "pki_mount_point")
+
+    @pki_mount_point.setter
+    def pki_mount_point(self, value: pulumi.Input[str]):
+        pulumi.set(self, "pki_mount_point", value)
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> pulumi.Input[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @server_address.setter
+    def server_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "server_address", value)
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> pulumi.Input[str]:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @signing_role.setter
+    def signing_role(self, value: pulumi.Input[str]):
+        pulumi.set(self, "signing_role", value)
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[pulumi.Input[str]]:
+        """
+        The namespace to make requests within
+        """
         return pulumi.get(self, "namespace")
 
     @namespace.setter
     def namespace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "namespace", value)
 
     @property
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/_utilities.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/_utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 
+import asyncio
+import importlib.metadata
 import importlib.util
 import inspect
 import json
 import os
-import pkg_resources
 import sys
 import typing
 
 import pulumi
 import pulumi.runtime
+from pulumi.runtime.sync_await import _sync_await
 
 from semver import VersionInfo as SemverVersion
 from parver import Version as PEP440Version
 
 
 def get_env(*args):
     for v in args:
@@ -66,15 +68,15 @@
     # pkg_resources uses setuptools to inspect the set of installed packages. We use it here to ask
     # for the currently installed version of the root package (i.e. us) and get its version.
 
     # Unfortunately, PEP440 and semver differ slightly in incompatible ways. The Pulumi engine expects
     # to receive a valid semver string when receiving requests from the language host, so it's our
     # responsibility as the library to convert our own PEP440 version into a valid semver string.
 
-    pep440_version_string = pkg_resources.require(root_package)[0].version
+    pep440_version_string = importlib.metadata.version(root_package)
     pep440_version = PEP440Version.parse(pep440_version_string)
     (major, minor, patch) = pep440_version.release
     prerelease = None
     if pep440_version.pre_tag == 'a':
         prerelease = f"alpha.{pep440_version.pre}"
     elif pep440_version.pre_tag == 'b':
         prerelease = f"beta.{pep440_version.pre}"
@@ -242,9 +244,48 @@
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
+
+def call_plain(
+    tok: str,
+    props: pulumi.Inputs,
+    res: typing.Optional[pulumi.Resource] = None,
+    typ: typing.Optional[type] = None,
+) -> typing.Any:
+    """
+    Wraps pulumi.runtime.plain to force the output and return it plainly.
+    """
+
+    output = pulumi.runtime.call(tok, props, res, typ)
+
+    # Ingoring deps silently. They are typically non-empty, r.f() calls include r as a dependency.
+    result, known, secret, _ = _sync_await(asyncio.ensure_future(_await_output(output)))
+
+    problem = None
+    if not known:
+        problem = ' an unknown value'
+    elif secret:
+        problem = ' a secret value'
+
+    if problem:
+        raise AssertionError(
+            f"Plain resource method '{tok}' incorrectly returned {problem}. "
+            + "This is an error in the provider, please report this to the provider developer."
+        )
+
+    return result
+
+
+async def _await_output(o: pulumi.Output[typing.Any]) -> typing.Tuple[object, bool, bool, set]:
+    return (
+        await o._future,
+        await o._is_known,
+        await o._is_secret,
+        await o._resources,
+    )
+
 def get_plugin_download_url():
 	return "github://api.github.com/pierskarsenbarg/pulumi-sdm"
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/account.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,15 @@
                  __props__=None):
         """
         Accounts are users that have access to strongDM. There are two types of accounts:
          1. **Users:** humans who are authenticated through username and password or SSO.
          2. **Service Accounts:** machines that are authenticated using a service token.
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pierskarsenbarg_pulumi_sdm as sdm
 
         test_user = sdm.Account("test-user", user=sdm.AccountUserArgs(
             email="albob@strongdm.com",
             first_name="al",
@@ -128,22 +129,23 @@
             name="test-service",
             tags={
                 "env": "dev",
                 "region": "us-west",
             },
         ))
         ```
+        <!--End PulumiCodeChooser -->
         This resource can be imported using the import command.
 
         ## Import
 
         A Account can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/account:Account example a-12345678
+        $ pulumi import sdm:index/account:Account example a-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['AccountServiceArgs']] service: A Service is a service account that can connect to resources they are granted directly, or granted via roles. Services
                are typically automated jobs.
         :param pulumi.Input[pulumi.InputType['AccountUserArgs']] user: A User can connect to resources they are granted directly, or granted via roles.
@@ -156,14 +158,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Accounts are users that have access to strongDM. There are two types of accounts:
          1. **Users:** humans who are authenticated through username and password or SSO.
          2. **Service Accounts:** machines that are authenticated using a service token.
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pierskarsenbarg_pulumi_sdm as sdm
 
         test_user = sdm.Account("test-user", user=sdm.AccountUserArgs(
             email="albob@strongdm.com",
             first_name="al",
@@ -177,22 +180,23 @@
             name="test-service",
             tags={
                 "env": "dev",
                 "region": "us-west",
             },
         ))
         ```
+        <!--End PulumiCodeChooser -->
         This resource can be imported using the import command.
 
         ## Import
 
         A Account can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/account:Account example a-12345678
+        $ pulumi import sdm:index/account:Account example a-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param AccountArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/account_attachment.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/account_attachment.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,30 +97,32 @@
                  account_id: Optional[pulumi.Input[str]] = None,
                  role_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         AccountAttachments assign an account to a role.
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pierskarsenbarg_pulumi_sdm as sdm
 
         test_account_attachment = sdm.AccountAttachment("testAccountAttachment",
             account_id="a-00000054",
             role_id="r-12355562")
         ```
+        <!--End PulumiCodeChooser -->
         This resource can be imported using the import command.
 
         ## Import
 
         A AccountAttachment can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/accountAttachment:AccountAttachment example aa-12345678
+        $ pulumi import sdm:index/accountAttachment:AccountAttachment example aa-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] account_id: The id of the account of this AccountAttachment.
         :param pulumi.Input[str] role_id: The id of the attached role of this AccountAttachment.
         """
@@ -130,30 +132,32 @@
                  resource_name: str,
                  args: AccountAttachmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         AccountAttachments assign an account to a role.
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pierskarsenbarg_pulumi_sdm as sdm
 
         test_account_attachment = sdm.AccountAttachment("testAccountAttachment",
             account_id="a-00000054",
             role_id="r-12355562")
         ```
+        <!--End PulumiCodeChooser -->
         This resource can be imported using the import command.
 
         ## Import
 
         A AccountAttachment can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/accountAttachment:AccountAttachment example aa-12345678
+        $ pulumi import sdm:index/accountAttachment:AccountAttachment example aa-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param AccountAttachmentArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/config/vars.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/config/vars.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_account.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_account.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetAccountResult:
     """
     A collection of values returned by getAccount.
     """
-    def __init__(__self__, accounts=None, email=None, external_id=None, first_name=None, id=None, ids=None, last_name=None, name=None, suspended=None, tags=None, type=None):
+    def __init__(__self__, accounts=None, email=None, external_id=None, first_name=None, id=None, ids=None, last_name=None, name=None, permission_level=None, suspended=None, tags=None, type=None):
         if accounts and not isinstance(accounts, list):
             raise TypeError("Expected argument 'accounts' to be a list")
         pulumi.set(__self__, "accounts", accounts)
         if email and not isinstance(email, str):
             raise TypeError("Expected argument 'email' to be a str")
         pulumi.set(__self__, "email", email)
         if external_id and not isinstance(external_id, str):
@@ -43,14 +43,17 @@
         pulumi.set(__self__, "ids", ids)
         if last_name and not isinstance(last_name, str):
             raise TypeError("Expected argument 'last_name' to be a str")
         pulumi.set(__self__, "last_name", last_name)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
+        if permission_level and not isinstance(permission_level, str):
+            raise TypeError("Expected argument 'permission_level' to be a str")
+        pulumi.set(__self__, "permission_level", permission_level)
         if suspended and not isinstance(suspended, bool):
             raise TypeError("Expected argument 'suspended' to be a bool")
         pulumi.set(__self__, "suspended", suspended)
         if tags and not isinstance(tags, dict):
             raise TypeError("Expected argument 'tags' to be a dict")
         pulumi.set(__self__, "tags", tags)
         if type and not isinstance(type, str):
@@ -119,18 +122,26 @@
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Service.
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="permissionLevel")
+    def permission_level(self) -> Optional[str]:
+        """
+        PermissionLevel is the user's permission level e.g. admin, DBA, user.
+        """
+        return pulumi.get(self, "permission_level")
+
+    @property
     @pulumi.getter
     def suspended(self) -> Optional[bool]:
         """
-        The User's suspended state.
+        Suspended is a read only field for the User's suspended state.
         """
         return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, Any]]:
         """
@@ -154,65 +165,71 @@
             email=self.email,
             external_id=self.external_id,
             first_name=self.first_name,
             id=self.id,
             ids=self.ids,
             last_name=self.last_name,
             name=self.name,
+            permission_level=self.permission_level,
             suspended=self.suspended,
             tags=self.tags,
             type=self.type)
 
 
 def get_account(email: Optional[str] = None,
                 external_id: Optional[str] = None,
                 first_name: Optional[str] = None,
                 id: Optional[str] = None,
                 last_name: Optional[str] = None,
                 name: Optional[str] = None,
+                permission_level: Optional[str] = None,
                 suspended: Optional[bool] = None,
                 tags: Optional[Mapping[str, Any]] = None,
                 type: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAccountResult:
     """
     Accounts are users that have access to strongDM. There are two types of accounts:
      1. **Users:** humans who are authenticated through username and password or SSO.
      2. **Service Accounts:** machines that are authenticated using a service token.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     user_queries = sdm.get_account(email="*@strongdm.com",
         tags={
             "env": "dev",
             "region": "us-west",
         },
         type="user")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str email: The User's email address. Must be unique.
     :param str external_id: External ID is an alternative unique ID this user is represented by within an external service.
     :param str first_name: The User's first name.
     :param str id: Unique identifier of the User.
     :param str last_name: The User's last name.
     :param str name: Unique human-readable name of the Service.
-    :param bool suspended: The User's suspended state.
+    :param str permission_level: PermissionLevel is the user's permission level e.g. admin, DBA, user.
+    :param bool suspended: The Service's suspended state.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
-    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
+    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters) for more information.
     """
     __args__ = dict()
     __args__['email'] = email
     __args__['externalId'] = external_id
     __args__['firstName'] = first_name
     __args__['id'] = id
     __args__['lastName'] = last_name
     __args__['name'] = name
+    __args__['permissionLevel'] = permission_level
     __args__['suspended'] = suspended
     __args__['tags'] = tags
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getAccount:getAccount', __args__, opts=opts, typ=GetAccountResult).value
 
     return AwaitableGetAccountResult(
@@ -220,53 +237,58 @@
         email=pulumi.get(__ret__, 'email'),
         external_id=pulumi.get(__ret__, 'external_id'),
         first_name=pulumi.get(__ret__, 'first_name'),
         id=pulumi.get(__ret__, 'id'),
         ids=pulumi.get(__ret__, 'ids'),
         last_name=pulumi.get(__ret__, 'last_name'),
         name=pulumi.get(__ret__, 'name'),
+        permission_level=pulumi.get(__ret__, 'permission_level'),
         suspended=pulumi.get(__ret__, 'suspended'),
         tags=pulumi.get(__ret__, 'tags'),
         type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_account)
 def get_account_output(email: Optional[pulumi.Input[Optional[str]]] = None,
                        external_id: Optional[pulumi.Input[Optional[str]]] = None,
                        first_name: Optional[pulumi.Input[Optional[str]]] = None,
                        id: Optional[pulumi.Input[Optional[str]]] = None,
                        last_name: Optional[pulumi.Input[Optional[str]]] = None,
                        name: Optional[pulumi.Input[Optional[str]]] = None,
+                       permission_level: Optional[pulumi.Input[Optional[str]]] = None,
                        suspended: Optional[pulumi.Input[Optional[bool]]] = None,
                        tags: Optional[pulumi.Input[Optional[Mapping[str, Any]]]] = None,
                        type: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAccountResult]:
     """
     Accounts are users that have access to strongDM. There are two types of accounts:
      1. **Users:** humans who are authenticated through username and password or SSO.
      2. **Service Accounts:** machines that are authenticated using a service token.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     user_queries = sdm.get_account(email="*@strongdm.com",
         tags={
             "env": "dev",
             "region": "us-west",
         },
         type="user")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str email: The User's email address. Must be unique.
     :param str external_id: External ID is an alternative unique ID this user is represented by within an external service.
     :param str first_name: The User's first name.
     :param str id: Unique identifier of the User.
     :param str last_name: The User's last name.
     :param str name: Unique human-readable name of the Service.
-    :param bool suspended: The User's suspended state.
+    :param str permission_level: PermissionLevel is the user's permission level e.g. admin, DBA, user.
+    :param bool suspended: The Service's suspended state.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
-    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
+    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters) for more information.
     """
     ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,20 +97,22 @@
                            id: Optional[str] = None,
                            role_id: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAccountAttachmentResult:
     """
     AccountAttachments assign an account to a role.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     account_attachment_query = sdm.get_account_attachment(account_id="a-00000054")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str account_id: The id of the account of this AccountAttachment.
     :param str id: Unique identifier of the AccountAttachment.
     :param str role_id: The id of the attached role of this AccountAttachment.
     """
     __args__ = dict()
@@ -133,20 +135,22 @@
                                   id: Optional[pulumi.Input[Optional[str]]] = None,
                                   role_id: Optional[pulumi.Input[Optional[str]]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAccountAttachmentResult]:
     """
     AccountAttachments assign an account to a role.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     account_attachment_query = sdm.get_account_attachment(account_id="a-00000054")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str account_id: The id of the account of this AccountAttachment.
     :param str id: Unique identifier of the AccountAttachment.
     :param str role_id: The id of the attached role of this AccountAttachment.
     """
     ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_node.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,32 +137,34 @@
     """
     Nodes make up the strongDM network, and allow your users to connect securely to your resources.
      There are two types of nodes:
      1. **Relay:** creates connectivity to your datasources, while maintaining the egress-only nature of your firewall
      2. **Gateways:** a relay that also listens for connections from strongDM clients
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     gateway_query = sdm.get_node(tags={
             "env": "dev",
             "region": "us-west",
         },
         type="gateway")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str bind_address: The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
     :param str id: Unique identifier of the Relay.
     :param str listen_address: The public hostname/port tuple at which the gateway will be accessible to clients.
     :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
-    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
+    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters) for more information.
     """
     __args__ = dict()
     __args__['bindAddress'] = bind_address
     __args__['id'] = id
     __args__['listenAddress'] = listen_address
     __args__['name'] = name
     __args__['tags'] = tags
@@ -192,27 +194,29 @@
     """
     Nodes make up the strongDM network, and allow your users to connect securely to your resources.
      There are two types of nodes:
      1. **Relay:** creates connectivity to your datasources, while maintaining the egress-only nature of your firewall
      2. **Gateways:** a relay that also listens for connections from strongDM clients
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     gateway_query = sdm.get_node(tags={
             "env": "dev",
             "region": "us-west",
         },
         type="gateway")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str bind_address: The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
     :param str id: Unique identifier of the Relay.
     :param str listen_address: The public hostname/port tuple at which the gateway will be accessible to clients.
     :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
-    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
+    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters) for more information.
     """
     ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_peering_group.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_peering_group.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_peering_group_node.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_peering_group_node.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_peering_group_peer.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_peering_group_peer.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_peering_group_resource.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_peering_group_resource.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,21 +111,23 @@
                         username: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRemoteIdentityResult:
     """
     RemoteIdentities define the username to be used for a specific account
      when connecting to a remote resource using that group.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     user = sdm.get_remote_identity(id="i-0900909",
         username="user")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str account_id: The account for this remote identity.
     :param str id: Unique identifier of the RemoteIdentity.
     :param str remote_identity_group_id: The remote identity group.
     :param str username: The username to be used as the remote identity for this account.
     """
@@ -153,21 +155,23 @@
                                username: Optional[pulumi.Input[Optional[str]]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRemoteIdentityResult]:
     """
     RemoteIdentities define the username to be used for a specific account
      when connecting to a remote resource using that group.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     user = sdm.get_remote_identity(id="i-0900909",
         username="user")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str account_id: The account for this remote identity.
     :param str id: Unique identifier of the RemoteIdentity.
     :param str remote_identity_group_id: The remote identity group.
     :param str username: The username to be used as the remote identity for this account.
     """
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,20 +84,22 @@
 def get_remote_identity_group(id: Optional[str] = None,
                               name: Optional[str] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRemoteIdentityGroupResult:
     """
     A RemoteIdentityGroup defines a group of remote identities.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     default = sdm.get_remote_identity_group(name="default")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str id: Unique identifier of the RemoteIdentityGroup.
     :param str name: Unique human-readable name of the RemoteIdentityGroup.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -116,19 +118,21 @@
 def get_remote_identity_group_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                                      name: Optional[pulumi.Input[Optional[str]]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRemoteIdentityGroupResult]:
     """
     A RemoteIdentityGroup defines a group of remote identities.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     default = sdm.get_remote_identity_group(name="default")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str id: Unique identifier of the RemoteIdentityGroup.
     :param str name: Unique human-readable name of the RemoteIdentityGroup.
     """
     ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_resource.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,33 +148,35 @@
                  username: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetResourceResult:
     """
     A Resource is a database, server, cluster, website, or cloud that strongDM
      delegates access to.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     mysql_datasources = sdm.get_resource(name="us-west*",
         tags={
             "env": "dev",
             "region": "us-west",
         },
         type="mysql")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
     :param str id: Unique identifier of the Resource.
     :param str name: Unique human-readable name of the Resource.
     :param int port: The port to dial to initiate a connection from the egress node to this resource.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
-    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
+    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters) for more information.
     :param str username: The username to authenticate with.
     """
     __args__ = dict()
     __args__['hostname'] = hostname
     __args__['id'] = id
     __args__['name'] = name
     __args__['port'] = port
@@ -206,29 +208,31 @@
                         username: Optional[pulumi.Input[Optional[str]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetResourceResult]:
     """
     A Resource is a database, server, cluster, website, or cloud that strongDM
      delegates access to.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     mysql_datasources = sdm.get_resource(name="us-west*",
         tags={
             "env": "dev",
             "region": "us-west",
         },
         type="mysql")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
     :param str id: Unique identifier of the Resource.
     :param str name: Unique human-readable name of the Resource.
     :param int port: The port to dial to initiate a connection from the egress node to this resource.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
-    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
+    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters) for more information.
     :param str username: The username to authenticate with.
     """
     ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_role.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_role.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="secretStores")
     def secret_stores(self) -> Sequence['outputs.GetSecretStoreSecretStoreResult']:
         """
         A single element list containing a map, where each key lists one of the following objects:
-        * aws:
+        * active_directory_store:
         """
         return pulumi.get(self, "secret_stores")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, Any]]:
         """
@@ -112,15 +112,15 @@
     A SecretStore is a server where resource secrets (passwords, keys) are stored.
      Coming soon support for HashiCorp Vault and AWS Secret Store.
 
 
     :param str id: Unique identifier of the SecretStore.
     :param str name: Unique human-readable name of the SecretStore.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
-    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
+    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters) for more information.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     __args__['tags'] = tags
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -145,10 +145,10 @@
     A SecretStore is a server where resource secrets (passwords, keys) are stored.
      Coming soon support for HashiCorp Vault and AWS Secret Store.
 
 
     :param str id: Unique identifier of the SecretStore.
     :param str name: Unique human-readable name of the SecretStore.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
-    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
+    :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters) for more information.
     """
     ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,20 +59,22 @@
 def get_ssh_ca_pubkey(id: Optional[str] = None,
                       public_key: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSshCaPubkeyResult:
     """
     The SSH CA Pubkey is a public key used for setting up SSH resources.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     ssh_pubkey_query = sdm.get_ssh_ca_pubkey()
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str id: a generated id representing this request.
     :param str public_key: the SSH Certificate Authority public key.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -89,19 +91,21 @@
 def get_ssh_ca_pubkey_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                              public_key: Optional[pulumi.Input[Optional[str]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSshCaPubkeyResult]:
     """
     The SSH CA Pubkey is a public key used for setting up SSH resources.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     ssh_pubkey_query = sdm.get_ssh_ca_pubkey()
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str id: a generated id representing this request.
     :param str public_key: the SSH Certificate Authority public key.
     """
     ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_workflow.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_workflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 ]
 
 @pulumi.output_type
 class GetWorkflowResult:
     """
     A collection of values returned by getWorkflow.
     """
-    def __init__(__self__, auto_grant=None, description=None, enabled=None, id=None, ids=None, name=None, weight=None, workflows=None):
+    def __init__(__self__, approval_flow_id=None, auto_grant=None, description=None, enabled=None, id=None, ids=None, name=None, weight=None, workflows=None):
+        if approval_flow_id and not isinstance(approval_flow_id, str):
+            raise TypeError("Expected argument 'approval_flow_id' to be a str")
+        pulumi.set(__self__, "approval_flow_id", approval_flow_id)
         if auto_grant and not isinstance(auto_grant, bool):
             raise TypeError("Expected argument 'auto_grant' to be a bool")
         pulumi.set(__self__, "auto_grant", auto_grant)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
         if enabled and not isinstance(enabled, bool):
@@ -45,14 +48,22 @@
             raise TypeError("Expected argument 'weight' to be a int")
         pulumi.set(__self__, "weight", weight)
         if workflows and not isinstance(workflows, list):
             raise TypeError("Expected argument 'workflows' to be a list")
         pulumi.set(__self__, "workflows", workflows)
 
     @property
+    @pulumi.getter(name="approvalFlowId")
+    def approval_flow_id(self) -> Optional[str]:
+        """
+        Optional approval flow ID identifies an approval flow that linked to the workflow
+        """
+        return pulumi.get(self, "approval_flow_id")
+
+    @property
     @pulumi.getter(name="autoGrant")
     def auto_grant(self) -> Optional[bool]:
         """
         Optional auto grant setting to automatically approve requests or not, defaults to false.
         """
         return pulumi.get(self, "auto_grant")
 
@@ -115,97 +126,108 @@
 
 class AwaitableGetWorkflowResult(GetWorkflowResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetWorkflowResult(
+            approval_flow_id=self.approval_flow_id,
             auto_grant=self.auto_grant,
             description=self.description,
             enabled=self.enabled,
             id=self.id,
             ids=self.ids,
             name=self.name,
             weight=self.weight,
             workflows=self.workflows)
 
 
-def get_workflow(auto_grant: Optional[bool] = None,
+def get_workflow(approval_flow_id: Optional[str] = None,
+                 auto_grant: Optional[bool] = None,
                  description: Optional[str] = None,
                  enabled: Optional[bool] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  weight: Optional[int] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetWorkflowResult:
     """
     Workflows are the collection of rules that define the resources to which access can be requested,
      the users that can request that access, and the mechanism for approving those requests which can either
      but automatic approval or a set of users authorized to approve the requests.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     workflow_query = sdm.get_workflow(auto_grant=True,
         name="workflow example")
     ```
+    <!--End PulumiCodeChooser -->
 
 
+    :param str approval_flow_id: Optional approval flow ID identifies an approval flow that linked to the workflow
     :param bool auto_grant: Optional auto grant setting to automatically approve requests or not, defaults to false.
     :param str description: Optional description of the Workflow.
     :param bool enabled: Optional enabled state for workflow. This setting may be overridden by the system if the workflow doesn't meet the requirements to be enabled or if other conditions prevent enabling the workflow. The requirements to enable a workflow are that the workflow must be either set up for with auto grant enabled or have one or more WorkflowApprovers created for the workflow.
     :param str id: Unique identifier of the Workflow.
     :param str name: Unique human-readable name of the Workflow.
     :param int weight: Optional weight for workflow to specify it's priority in matching a request.
     """
     __args__ = dict()
+    __args__['approvalFlowId'] = approval_flow_id
     __args__['autoGrant'] = auto_grant
     __args__['description'] = description
     __args__['enabled'] = enabled
     __args__['id'] = id
     __args__['name'] = name
     __args__['weight'] = weight
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getWorkflow:getWorkflow', __args__, opts=opts, typ=GetWorkflowResult).value
 
     return AwaitableGetWorkflowResult(
+        approval_flow_id=pulumi.get(__ret__, 'approval_flow_id'),
         auto_grant=pulumi.get(__ret__, 'auto_grant'),
         description=pulumi.get(__ret__, 'description'),
         enabled=pulumi.get(__ret__, 'enabled'),
         id=pulumi.get(__ret__, 'id'),
         ids=pulumi.get(__ret__, 'ids'),
         name=pulumi.get(__ret__, 'name'),
         weight=pulumi.get(__ret__, 'weight'),
         workflows=pulumi.get(__ret__, 'workflows'))
 
 
 @_utilities.lift_output_func(get_workflow)
-def get_workflow_output(auto_grant: Optional[pulumi.Input[Optional[bool]]] = None,
+def get_workflow_output(approval_flow_id: Optional[pulumi.Input[Optional[str]]] = None,
+                        auto_grant: Optional[pulumi.Input[Optional[bool]]] = None,
                         description: Optional[pulumi.Input[Optional[str]]] = None,
                         enabled: Optional[pulumi.Input[Optional[bool]]] = None,
                         id: Optional[pulumi.Input[Optional[str]]] = None,
                         name: Optional[pulumi.Input[Optional[str]]] = None,
                         weight: Optional[pulumi.Input[Optional[int]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetWorkflowResult]:
     """
     Workflows are the collection of rules that define the resources to which access can be requested,
      the users that can request that access, and the mechanism for approving those requests which can either
      but automatic approval or a set of users authorized to approve the requests.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
     workflow_query = sdm.get_workflow(auto_grant=True,
         name="workflow example")
     ```
+    <!--End PulumiCodeChooser -->
 
 
+    :param str approval_flow_id: Optional approval flow ID identifies an approval flow that linked to the workflow
     :param bool auto_grant: Optional auto grant setting to automatically approve requests or not, defaults to false.
     :param str description: Optional description of the Workflow.
     :param bool enabled: Optional enabled state for workflow. This setting may be overridden by the system if the workflow doesn't meet the requirements to be enabled or if other conditions prevent enabling the workflow. The requirements to enable a workflow are that the workflow must be either set up for with auto grant enabled or have one or more WorkflowApprovers created for the workflow.
     :param str id: Unique identifier of the Workflow.
     :param str name: Unique human-readable name of the Workflow.
     :param int weight: Optional weight for workflow to specify it's priority in matching a request.
     """
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/get_workflow_approver.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_workflow_role.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,148 +7,154 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
-    'GetWorkflowApproverResult',
-    'AwaitableGetWorkflowApproverResult',
-    'get_workflow_approver',
-    'get_workflow_approver_output',
+    'GetWorkflowRoleResult',
+    'AwaitableGetWorkflowRoleResult',
+    'get_workflow_role',
+    'get_workflow_role_output',
 ]
 
 @pulumi.output_type
-class GetWorkflowApproverResult:
+class GetWorkflowRoleResult:
     """
-    A collection of values returned by getWorkflowApprover.
+    A collection of values returned by getWorkflowRole.
     """
-    def __init__(__self__, approver_id=None, id=None, ids=None, workflow_approvers=None, workflow_id=None):
-        if approver_id and not isinstance(approver_id, str):
-            raise TypeError("Expected argument 'approver_id' to be a str")
-        pulumi.set(__self__, "approver_id", approver_id)
+    def __init__(__self__, id=None, ids=None, role_id=None, workflow_id=None, workflow_roles=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if ids and not isinstance(ids, list):
             raise TypeError("Expected argument 'ids' to be a list")
         pulumi.set(__self__, "ids", ids)
-        if workflow_approvers and not isinstance(workflow_approvers, list):
-            raise TypeError("Expected argument 'workflow_approvers' to be a list")
-        pulumi.set(__self__, "workflow_approvers", workflow_approvers)
+        if role_id and not isinstance(role_id, str):
+            raise TypeError("Expected argument 'role_id' to be a str")
+        pulumi.set(__self__, "role_id", role_id)
         if workflow_id and not isinstance(workflow_id, str):
             raise TypeError("Expected argument 'workflow_id' to be a str")
         pulumi.set(__self__, "workflow_id", workflow_id)
-
-    @property
-    @pulumi.getter(name="approverId")
-    def approver_id(self) -> Optional[str]:
-        """
-        The approver id.
-        """
-        return pulumi.get(self, "approver_id")
+        if workflow_roles and not isinstance(workflow_roles, list):
+            raise TypeError("Expected argument 'workflow_roles' to be a list")
+        pulumi.set(__self__, "workflow_roles", workflow_roles)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
-        Unique identifier of the WorkflowApprover.
+        Unique identifier of the WorkflowRole.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def ids(self) -> Sequence[str]:
         """
         a list of strings of ids of data sources that match the given arguments.
         """
         return pulumi.get(self, "ids")
 
     @property
-    @pulumi.getter(name="workflowApprovers")
-    def workflow_approvers(self) -> Sequence['outputs.GetWorkflowApproverWorkflowApproverResult']:
+    @pulumi.getter(name="roleId")
+    def role_id(self) -> Optional[str]:
         """
-        A list where each element has the following attributes:
+        The role id.
         """
-        return pulumi.get(self, "workflow_approvers")
+        return pulumi.get(self, "role_id")
 
     @property
     @pulumi.getter(name="workflowId")
     def workflow_id(self) -> Optional[str]:
         """
         The workflow id.
         """
         return pulumi.get(self, "workflow_id")
 
+    @property
+    @pulumi.getter(name="workflowRoles")
+    def workflow_roles(self) -> Sequence['outputs.GetWorkflowRoleWorkflowRoleResult']:
+        """
+        A list where each element has the following attributes:
+        """
+        return pulumi.get(self, "workflow_roles")
+
 
-class AwaitableGetWorkflowApproverResult(GetWorkflowApproverResult):
+class AwaitableGetWorkflowRoleResult(GetWorkflowRoleResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetWorkflowApproverResult(
-            approver_id=self.approver_id,
+        return GetWorkflowRoleResult(
             id=self.id,
             ids=self.ids,
-            workflow_approvers=self.workflow_approvers,
-            workflow_id=self.workflow_id)
+            role_id=self.role_id,
+            workflow_id=self.workflow_id,
+            workflow_roles=self.workflow_roles)
 
 
-def get_workflow_approver(approver_id: Optional[str] = None,
-                          id: Optional[str] = None,
-                          workflow_id: Optional[str] = None,
-                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetWorkflowApproverResult:
+def get_workflow_role(id: Optional[str] = None,
+                      role_id: Optional[str] = None,
+                      workflow_id: Optional[str] = None,
+                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetWorkflowRoleResult:
     """
-    WorkflowApprover is an account with the ability to approve requests bound to a workflow.
+    WorkflowRole links a role to a workflow. The linked roles indicate which roles a user must be a part of
+     to request access to a resource via the workflow.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
-    workflow_approver_query = sdm.get_workflow_approver(approver_id="a-2496542",
-        workflow_id="aw-541894")
+    workflow_role_query = sdm.get_workflow_role(role_id="r-9862923",
+        workflow_id="aw-7935485")
     ```
+    <!--End PulumiCodeChooser -->
 
 
-    :param str approver_id: The approver id.
-    :param str id: Unique identifier of the WorkflowApprover.
+    :param str id: Unique identifier of the WorkflowRole.
+    :param str role_id: The role id.
     :param str workflow_id: The workflow id.
     """
     __args__ = dict()
-    __args__['approverId'] = approver_id
     __args__['id'] = id
+    __args__['roleId'] = role_id
     __args__['workflowId'] = workflow_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('sdm:index/getWorkflowApprover:getWorkflowApprover', __args__, opts=opts, typ=GetWorkflowApproverResult).value
+    __ret__ = pulumi.runtime.invoke('sdm:index/getWorkflowRole:getWorkflowRole', __args__, opts=opts, typ=GetWorkflowRoleResult).value
 
-    return AwaitableGetWorkflowApproverResult(
-        approver_id=pulumi.get(__ret__, 'approver_id'),
+    return AwaitableGetWorkflowRoleResult(
         id=pulumi.get(__ret__, 'id'),
         ids=pulumi.get(__ret__, 'ids'),
-        workflow_approvers=pulumi.get(__ret__, 'workflow_approvers'),
-        workflow_id=pulumi.get(__ret__, 'workflow_id'))
+        role_id=pulumi.get(__ret__, 'role_id'),
+        workflow_id=pulumi.get(__ret__, 'workflow_id'),
+        workflow_roles=pulumi.get(__ret__, 'workflow_roles'))
 
 
-@_utilities.lift_output_func(get_workflow_approver)
-def get_workflow_approver_output(approver_id: Optional[pulumi.Input[Optional[str]]] = None,
-                                 id: Optional[pulumi.Input[Optional[str]]] = None,
-                                 workflow_id: Optional[pulumi.Input[Optional[str]]] = None,
-                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetWorkflowApproverResult]:
+@_utilities.lift_output_func(get_workflow_role)
+def get_workflow_role_output(id: Optional[pulumi.Input[Optional[str]]] = None,
+                             role_id: Optional[pulumi.Input[Optional[str]]] = None,
+                             workflow_id: Optional[pulumi.Input[Optional[str]]] = None,
+                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetWorkflowRoleResult]:
     """
-    WorkflowApprover is an account with the ability to approve requests bound to a workflow.
+    WorkflowRole links a role to a workflow. The linked roles indicate which roles a user must be a part of
+     to request access to a resource via the workflow.
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_sdm as sdm
 
-    workflow_approver_query = sdm.get_workflow_approver(approver_id="a-2496542",
-        workflow_id="aw-541894")
+    workflow_role_query = sdm.get_workflow_role(role_id="r-9862923",
+        workflow_id="aw-7935485")
     ```
+    <!--End PulumiCodeChooser -->
 
 
-    :param str approver_id: The approver id.
-    :param str id: Unique identifier of the WorkflowApprover.
+    :param str id: Unique identifier of the WorkflowRole.
+    :param str role_id: The role id.
     :param str workflow_id: The workflow id.
     """
     ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/node.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,15 @@
         """
         Nodes make up the strongDM network, and allow your users to connect securely to your resources.
          There are two types of nodes:
          1. **Relay:** creates connectivity to your datasources, while maintaining the egress-only nature of your firewall
          2. **Gateways:** a relay that also listens for connections from strongDM clients
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pierskarsenbarg_pulumi_sdm as sdm
 
         gateway = sdm.Node("gateway", gateway=sdm.NodeGatewayArgs(
             bind_address="0.0.0.0:21222",
             listen_address="165.23.40.1:21222",
@@ -125,22 +126,23 @@
             name="test-relay",
             tags={
                 "env": "dev",
                 "region": "us-west",
             },
         ))
         ```
+        <!--End PulumiCodeChooser -->
         This resource can be imported using the import command.
 
         ## Import
 
         A Node can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/node:Node example n-12345678
+        $ pulumi import sdm:index/node:Node example n-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['NodeGatewayArgs']] gateway: Gateway represents a StrongDM CLI installation running in gateway mode.
         :param pulumi.Input[pulumi.InputType['NodeRelayArgs']] relay: Relay represents a StrongDM CLI installation running in relay mode.
         """
@@ -153,14 +155,15 @@
         """
         Nodes make up the strongDM network, and allow your users to connect securely to your resources.
          There are two types of nodes:
          1. **Relay:** creates connectivity to your datasources, while maintaining the egress-only nature of your firewall
          2. **Gateways:** a relay that also listens for connections from strongDM clients
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pierskarsenbarg_pulumi_sdm as sdm
 
         gateway = sdm.Node("gateway", gateway=sdm.NodeGatewayArgs(
             bind_address="0.0.0.0:21222",
             listen_address="165.23.40.1:21222",
@@ -174,22 +177,23 @@
             name="test-relay",
             tags={
                 "env": "dev",
                 "region": "us-west",
             },
         ))
         ```
+        <!--End PulumiCodeChooser -->
         This resource can be imported using the import command.
 
         ## Import
 
         A Node can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/node:Node example n-12345678
+        $ pulumi import sdm:index/node:Node example n-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param NodeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/outputs.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     'ResourceNeptuneIam',
     'ResourceOracle',
     'ResourcePostgres',
     'ResourcePresto',
     'ResourceRabbitmqAmqp091',
     'ResourceRawTcp',
     'ResourceRdp',
+    'ResourceRdpCert',
     'ResourceRdsPostgresIam',
     'ResourceRedis',
     'ResourceRedshift',
     'ResourceSingleStore',
     'ResourceSnowflake',
     'ResourceSnowsight',
     'ResourceSqlServer',
@@ -96,28 +97,40 @@
     'ResourceSsh',
     'ResourceSshCert',
     'ResourceSshCustomerKey',
     'ResourceSybase',
     'ResourceSybaseIq',
     'ResourceTeradata',
     'ResourceTrino',
+    'SecretStoreActiveDirectoryStore',
     'SecretStoreAws',
+    'SecretStoreAwsCertX509',
     'SecretStoreAzureStore',
     'SecretStoreCyberarkConjur',
     'SecretStoreCyberarkPam',
     'SecretStoreCyberarkPamExperimental',
     'SecretStoreDelineaStore',
+    'SecretStoreGcpCertX509Store',
     'SecretStoreGcpStore',
     'SecretStoreVaultApprole',
+    'SecretStoreVaultApproleCertSsh',
+    'SecretStoreVaultApproleCertX509',
     'SecretStoreVaultTls',
+    'SecretStoreVaultTlsCertSsh',
+    'SecretStoreVaultTlsCertX509',
     'SecretStoreVaultToken',
+    'SecretStoreVaultTokenCertSsh',
+    'SecretStoreVaultTokenCertX509',
     'GetAccountAccountResult',
     'GetAccountAccountServiceResult',
     'GetAccountAccountUserResult',
     'GetAccountAttachmentAccountAttachmentResult',
+    'GetApprovalWorkflowApprovalWorkflowResult',
+    'GetApprovalWorkflowApproverApprovalWorkflowApproverResult',
+    'GetApprovalWorkflowStepApprovalWorkflowStepResult',
     'GetNodeNodeResult',
     'GetNodeNodeGatewayResult',
     'GetNodeNodeGatewayMaintenanceWindowResult',
     'GetNodeNodeRelayResult',
     'GetNodeNodeRelayMaintenanceWindowResult',
     'GetPeeringGroupNodePeeringGroupNodeResult',
     'GetPeeringGroupPeerPeeringGroupPeerResult',
@@ -189,14 +202,15 @@
     'GetResourceResourceNeptuneIamResult',
     'GetResourceResourceOracleResult',
     'GetResourceResourcePostgreResult',
     'GetResourceResourcePrestoResult',
     'GetResourceResourceRabbitmqAmqp091Result',
     'GetResourceResourceRawTcpResult',
     'GetResourceResourceRdpResult',
+    'GetResourceResourceRdpCertResult',
     'GetResourceResourceRdsPostgresIamResult',
     'GetResourceResourceRediResult',
     'GetResourceResourceRedshiftResult',
     'GetResourceResourceSingleStoreResult',
     'GetResourceResourceSnowflakeResult',
     'GetResourceResourceSnowsightResult',
     'GetResourceResourceSqlServerResult',
@@ -207,39 +221,48 @@
     'GetResourceResourceSshCustomerKeyResult',
     'GetResourceResourceSybaseResult',
     'GetResourceResourceSybaseIqResult',
     'GetResourceResourceTeradataResult',
     'GetResourceResourceTrinoResult',
     'GetRoleRoleResult',
     'GetSecretStoreSecretStoreResult',
+    'GetSecretStoreSecretStoreActiveDirectoryStoreResult',
     'GetSecretStoreSecretStoreAwResult',
+    'GetSecretStoreSecretStoreAwsCertX509Result',
     'GetSecretStoreSecretStoreAzureStoreResult',
     'GetSecretStoreSecretStoreCyberarkConjurResult',
     'GetSecretStoreSecretStoreCyberarkPamResult',
     'GetSecretStoreSecretStoreCyberarkPamExperimentalResult',
     'GetSecretStoreSecretStoreDelineaStoreResult',
+    'GetSecretStoreSecretStoreGcpCertX509StoreResult',
     'GetSecretStoreSecretStoreGcpStoreResult',
     'GetSecretStoreSecretStoreVaultApproleResult',
+    'GetSecretStoreSecretStoreVaultApproleCertSshResult',
+    'GetSecretStoreSecretStoreVaultApproleCertX509Result',
     'GetSecretStoreSecretStoreVaultTlResult',
+    'GetSecretStoreSecretStoreVaultTlsCertSshResult',
+    'GetSecretStoreSecretStoreVaultTlsCertX509Result',
     'GetSecretStoreSecretStoreVaultTokenResult',
+    'GetSecretStoreSecretStoreVaultTokenCertSshResult',
+    'GetSecretStoreSecretStoreVaultTokenCertX509Result',
     'GetWorkflowApproverWorkflowApproverResult',
     'GetWorkflowRoleWorkflowRoleResult',
     'GetWorkflowWorkflowResult',
 ]
 
 @pulumi.output_type
 class AccountService(dict):
     def __init__(__self__, *,
                  name: str,
                  suspended: Optional[bool] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Service.
-        :param bool suspended: The User's suspended state.
+        :param bool suspended: The Service's suspended state.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         if suspended is not None:
             pulumi.set(__self__, "suspended", suspended)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
@@ -254,15 +277,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def suspended(self) -> Optional[bool]:
         """
-        The User's suspended state.
+        The Service's suspended state.
         """
         return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
@@ -314,16 +337,16 @@
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str email: The User's email address. Must be unique.
         :param str first_name: The User's first name.
         :param str last_name: The User's last name.
         :param str external_id: External ID is an alternative unique ID this user is represented by within an external service.
         :param str managed_by: Managed By is a read only field for what service manages this user, e.g. StrongDM, Okta, Azure.
-        :param str permission_level: PermissionLevel is a read only field for the user's permission level e.g. admin, DBA, user.
-        :param bool suspended: The User's suspended state.
+        :param str permission_level: PermissionLevel is the user's permission level e.g. admin, DBA, user.
+        :param bool suspended: The Service's suspended state.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "email", email)
         pulumi.set(__self__, "first_name", first_name)
         pulumi.set(__self__, "last_name", last_name)
         if external_id is not None:
             pulumi.set(__self__, "external_id", external_id)
@@ -376,23 +399,23 @@
         """
         return pulumi.get(self, "managed_by")
 
     @property
     @pulumi.getter(name="permissionLevel")
     def permission_level(self) -> Optional[str]:
         """
-        PermissionLevel is a read only field for the user's permission level e.g. admin, DBA, user.
+        PermissionLevel is the user's permission level e.g. admin, DBA, user.
         """
         return pulumi.get(self, "permission_level")
 
     @property
     @pulumi.getter
     def suspended(self) -> Optional[bool]:
         """
-        The User's suspended state.
+        The Service's suspended state.
         """
         return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
@@ -13357,14 +13380,190 @@
         """
         The username to authenticate with.
         """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
+class ResourceRdpCert(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "bindInterface":
+            suggest = "bind_interface"
+        elif key == "egressFilter":
+            suggest = "egress_filter"
+        elif key == "portOverride":
+            suggest = "port_override"
+        elif key == "remoteIdentityGroupId":
+            suggest = "remote_identity_group_id"
+        elif key == "remoteIdentityHealthcheckUsername":
+            suggest = "remote_identity_healthcheck_username"
+        elif key == "secretStoreId":
+            suggest = "secret_store_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ResourceRdpCert. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ResourceRdpCert.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ResourceRdpCert.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 hostname: str,
+                 name: str,
+                 bind_interface: Optional[str] = None,
+                 egress_filter: Optional[str] = None,
+                 port: Optional[int] = None,
+                 port_override: Optional[int] = None,
+                 remote_identity_group_id: Optional[str] = None,
+                 remote_identity_healthcheck_username: Optional[str] = None,
+                 secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None,
+                 username: Optional[str] = None):
+        """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
+        :param str name: Unique human-readable name of the Resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
+        """
+        pulumi.set(__self__, "hostname", hostname)
+        pulumi.set(__self__, "name", name)
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
+        if remote_identity_group_id is not None:
+            pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
+        if remote_identity_healthcheck_username is not None:
+            pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
+        return pulumi.get(self, "hostname")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[str]:
+        """
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[str]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
+        return pulumi.get(self, "port")
+
+    @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
+        return pulumi.get(self, "port_override")
+
+    @property
+    @pulumi.getter(name="remoteIdentityGroupId")
+    def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
+        return pulumi.get(self, "remote_identity_group_id")
+
+    @property
+    @pulumi.getter(name="remoteIdentityHealthcheckUsername")
+    def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
+        return pulumi.get(self, "remote_identity_healthcheck_username")
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[str]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
+        return pulumi.get(self, "username")
+
+
+@pulumi.output_type
 class ResourceRdsPostgresIam(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bindInterface":
             suggest = "bind_interface"
         elif key == "egressFilter":
@@ -16378,14 +16577,72 @@
         """
         The username to authenticate with.
         """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
+class SecretStoreActiveDirectoryStore(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "serverAddress":
+            suggest = "server_address"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SecretStoreActiveDirectoryStore. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SecretStoreActiveDirectoryStore.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SecretStoreActiveDirectoryStore.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 name: str,
+                 server_address: str,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str server_address: The URL of the Vault to target
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "server_address", server_address)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> str:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class SecretStoreAws(dict):
     def __init__(__self__, *,
                  name: str,
                  region: str,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the SecretStore.
@@ -16419,14 +16676,122 @@
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
+class SecretStoreAwsCertX509(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "caArn":
+            suggest = "ca_arn"
+        elif key == "certificateTemplateArn":
+            suggest = "certificate_template_arn"
+        elif key == "issuedCertTtlMinutes":
+            suggest = "issued_cert_ttl_minutes"
+        elif key == "signingAlgo":
+            suggest = "signing_algo"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SecretStoreAwsCertX509. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SecretStoreAwsCertX509.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SecretStoreAwsCertX509.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 ca_arn: str,
+                 certificate_template_arn: str,
+                 issued_cert_ttl_minutes: int,
+                 name: str,
+                 region: str,
+                 signing_algo: str,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str ca_arn: The ARN of the CA in AWS Private CA
+        :param str certificate_template_arn: The ARN of the AWS certificate template for requested certificates. Must allow SAN, key usage, and ext key usage passthrough from CSR
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str region: The AWS region to target e.g. us-east-1
+        :param str signing_algo: The specified signing algorithm family (RSA or ECDSA) must match the algorithm family of the CA's secret key. e.g. SHA256WITHRSA
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "ca_arn", ca_arn)
+        pulumi.set(__self__, "certificate_template_arn", certificate_template_arn)
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "signing_algo", signing_algo)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="caArn")
+    def ca_arn(self) -> str:
+        """
+        The ARN of the CA in AWS Private CA
+        """
+        return pulumi.get(self, "ca_arn")
+
+    @property
+    @pulumi.getter(name="certificateTemplateArn")
+    def certificate_template_arn(self) -> str:
+        """
+        The ARN of the AWS certificate template for requested certificates. Must allow SAN, key usage, and ext key usage passthrough from CSR
+        """
+        return pulumi.get(self, "certificate_template_arn")
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> int:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def region(self) -> str:
+        """
+        The AWS region to target e.g. us-east-1
+        """
+        return pulumi.get(self, "region")
+
+    @property
+    @pulumi.getter(name="signingAlgo")
+    def signing_algo(self) -> str:
+        """
+        The specified signing algorithm family (RSA or ECDSA) must match the algorithm family of the CA's secret key. e.g. SHA256WITHRSA
+        """
+        return pulumi.get(self, "signing_algo")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class SecretStoreAzureStore(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "vaultUri":
             suggest = "vault_uri"
 
@@ -16728,14 +17093,123 @@
         The tenant name to target
         * gcp_store:
         """
         return pulumi.get(self, "tenant_name")
 
 
 @pulumi.output_type
+class SecretStoreGcpCertX509Store(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "caPoolId":
+            suggest = "ca_pool_id"
+        elif key == "issuedCertTtlMinutes":
+            suggest = "issued_cert_ttl_minutes"
+        elif key == "projectId":
+            suggest = "project_id"
+        elif key == "caId":
+            suggest = "ca_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SecretStoreGcpCertX509Store. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SecretStoreGcpCertX509Store.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SecretStoreGcpCertX509Store.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 ca_pool_id: str,
+                 issued_cert_ttl_minutes: int,
+                 location: str,
+                 name: str,
+                 project_id: str,
+                 ca_id: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str ca_pool_id: The ID of the target CA pool
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str location: The Region for the CA in GCP format e.g. us-west1
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str project_id: The GCP project ID to target.
+        :param str ca_id: The ID of the target CA
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "ca_pool_id", ca_pool_id)
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "location", location)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "project_id", project_id)
+        if ca_id is not None:
+            pulumi.set(__self__, "ca_id", ca_id)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="caPoolId")
+    def ca_pool_id(self) -> str:
+        """
+        The ID of the target CA pool
+        """
+        return pulumi.get(self, "ca_pool_id")
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> int:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def location(self) -> str:
+        """
+        The Region for the CA in GCP format e.g. us-west1
+        """
+        return pulumi.get(self, "location")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> str:
+        """
+        The GCP project ID to target.
+        """
+        return pulumi.get(self, "project_id")
+
+    @property
+    @pulumi.getter(name="caId")
+    def ca_id(self) -> Optional[str]:
+        """
+        The ID of the target CA
+        """
+        return pulumi.get(self, "ca_id")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class SecretStoreGcpStore(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "projectId":
             suggest = "project_id"
 
@@ -16856,14 +17330,232 @@
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
+class SecretStoreVaultApproleCertSsh(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "issuedCertTtlMinutes":
+            suggest = "issued_cert_ttl_minutes"
+        elif key == "serverAddress":
+            suggest = "server_address"
+        elif key == "signingRole":
+            suggest = "signing_role"
+        elif key == "sshMountPoint":
+            suggest = "ssh_mount_point"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SecretStoreVaultApproleCertSsh. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SecretStoreVaultApproleCertSsh.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SecretStoreVaultApproleCertSsh.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 issued_cert_ttl_minutes: int,
+                 name: str,
+                 server_address: str,
+                 signing_role: str,
+                 ssh_mount_point: str,
+                 namespace: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str server_address: The URL of the Vault to target
+        :param str signing_role: The signing role to be used for signing certificates
+        :param str ssh_mount_point: The mount point of the SSH engine configured with the desired CA
+        :param str namespace: The namespace to make requests within
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "server_address", server_address)
+        pulumi.set(__self__, "signing_role", signing_role)
+        pulumi.set(__self__, "ssh_mount_point", ssh_mount_point)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> int:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> str:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> str:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @property
+    @pulumi.getter(name="sshMountPoint")
+    def ssh_mount_point(self) -> str:
+        """
+        The mount point of the SSH engine configured with the desired CA
+        """
+        return pulumi.get(self, "ssh_mount_point")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
+class SecretStoreVaultApproleCertX509(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "issuedCertTtlMinutes":
+            suggest = "issued_cert_ttl_minutes"
+        elif key == "pkiMountPoint":
+            suggest = "pki_mount_point"
+        elif key == "serverAddress":
+            suggest = "server_address"
+        elif key == "signingRole":
+            suggest = "signing_role"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SecretStoreVaultApproleCertX509. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SecretStoreVaultApproleCertX509.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SecretStoreVaultApproleCertX509.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 issued_cert_ttl_minutes: int,
+                 name: str,
+                 pki_mount_point: str,
+                 server_address: str,
+                 signing_role: str,
+                 namespace: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str pki_mount_point: The mount point of the PKI engine configured with the desired CA
+        :param str server_address: The URL of the Vault to target
+        :param str signing_role: The signing role to be used for signing certificates
+        :param str namespace: The namespace to make requests within
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "pki_mount_point", pki_mount_point)
+        pulumi.set(__self__, "server_address", server_address)
+        pulumi.set(__self__, "signing_role", signing_role)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> int:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="pkiMountPoint")
+    def pki_mount_point(self) -> str:
+        """
+        The mount point of the PKI engine configured with the desired CA
+        """
+        return pulumi.get(self, "pki_mount_point")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> str:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> str:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class SecretStoreVaultTls(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "clientCertPath":
             suggest = "client_cert_path"
         elif key == "clientKeyPath":
@@ -16966,14 +17658,312 @@
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
+class SecretStoreVaultTlsCertSsh(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "clientCertPath":
+            suggest = "client_cert_path"
+        elif key == "clientKeyPath":
+            suggest = "client_key_path"
+        elif key == "issuedCertTtlMinutes":
+            suggest = "issued_cert_ttl_minutes"
+        elif key == "serverAddress":
+            suggest = "server_address"
+        elif key == "signingRole":
+            suggest = "signing_role"
+        elif key == "sshMountPoint":
+            suggest = "ssh_mount_point"
+        elif key == "caCertPath":
+            suggest = "ca_cert_path"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SecretStoreVaultTlsCertSsh. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SecretStoreVaultTlsCertSsh.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SecretStoreVaultTlsCertSsh.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 client_cert_path: str,
+                 client_key_path: str,
+                 issued_cert_ttl_minutes: int,
+                 name: str,
+                 server_address: str,
+                 signing_role: str,
+                 ssh_mount_point: str,
+                 ca_cert_path: Optional[str] = None,
+                 namespace: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str client_cert_path: A path to a client certificate file accessible by a Node
+        :param str client_key_path: A path to a client key file accessible by a Node
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str server_address: The URL of the Vault to target
+        :param str signing_role: The signing role to be used for signing certificates
+        :param str ssh_mount_point: The mount point of the SSH engine configured with the desired CA
+        :param str ca_cert_path: A path to a CA file accessible by a Node
+        :param str namespace: The namespace to make requests within
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "client_cert_path", client_cert_path)
+        pulumi.set(__self__, "client_key_path", client_key_path)
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "server_address", server_address)
+        pulumi.set(__self__, "signing_role", signing_role)
+        pulumi.set(__self__, "ssh_mount_point", ssh_mount_point)
+        if ca_cert_path is not None:
+            pulumi.set(__self__, "ca_cert_path", ca_cert_path)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="clientCertPath")
+    def client_cert_path(self) -> str:
+        """
+        A path to a client certificate file accessible by a Node
+        """
+        return pulumi.get(self, "client_cert_path")
+
+    @property
+    @pulumi.getter(name="clientKeyPath")
+    def client_key_path(self) -> str:
+        """
+        A path to a client key file accessible by a Node
+        """
+        return pulumi.get(self, "client_key_path")
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> int:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> str:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> str:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @property
+    @pulumi.getter(name="sshMountPoint")
+    def ssh_mount_point(self) -> str:
+        """
+        The mount point of the SSH engine configured with the desired CA
+        """
+        return pulumi.get(self, "ssh_mount_point")
+
+    @property
+    @pulumi.getter(name="caCertPath")
+    def ca_cert_path(self) -> Optional[str]:
+        """
+        A path to a CA file accessible by a Node
+        """
+        return pulumi.get(self, "ca_cert_path")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
+class SecretStoreVaultTlsCertX509(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "clientCertPath":
+            suggest = "client_cert_path"
+        elif key == "clientKeyPath":
+            suggest = "client_key_path"
+        elif key == "issuedCertTtlMinutes":
+            suggest = "issued_cert_ttl_minutes"
+        elif key == "pkiMountPoint":
+            suggest = "pki_mount_point"
+        elif key == "serverAddress":
+            suggest = "server_address"
+        elif key == "signingRole":
+            suggest = "signing_role"
+        elif key == "caCertPath":
+            suggest = "ca_cert_path"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SecretStoreVaultTlsCertX509. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SecretStoreVaultTlsCertX509.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SecretStoreVaultTlsCertX509.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 client_cert_path: str,
+                 client_key_path: str,
+                 issued_cert_ttl_minutes: int,
+                 name: str,
+                 pki_mount_point: str,
+                 server_address: str,
+                 signing_role: str,
+                 ca_cert_path: Optional[str] = None,
+                 namespace: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str client_cert_path: A path to a client certificate file accessible by a Node
+        :param str client_key_path: A path to a client key file accessible by a Node
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str pki_mount_point: The mount point of the PKI engine configured with the desired CA
+        :param str server_address: The URL of the Vault to target
+        :param str signing_role: The signing role to be used for signing certificates
+        :param str ca_cert_path: A path to a CA file accessible by a Node
+        :param str namespace: The namespace to make requests within
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "client_cert_path", client_cert_path)
+        pulumi.set(__self__, "client_key_path", client_key_path)
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "pki_mount_point", pki_mount_point)
+        pulumi.set(__self__, "server_address", server_address)
+        pulumi.set(__self__, "signing_role", signing_role)
+        if ca_cert_path is not None:
+            pulumi.set(__self__, "ca_cert_path", ca_cert_path)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="clientCertPath")
+    def client_cert_path(self) -> str:
+        """
+        A path to a client certificate file accessible by a Node
+        """
+        return pulumi.get(self, "client_cert_path")
+
+    @property
+    @pulumi.getter(name="clientKeyPath")
+    def client_key_path(self) -> str:
+        """
+        A path to a client key file accessible by a Node
+        """
+        return pulumi.get(self, "client_key_path")
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> int:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="pkiMountPoint")
+    def pki_mount_point(self) -> str:
+        """
+        The mount point of the PKI engine configured with the desired CA
+        """
+        return pulumi.get(self, "pki_mount_point")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> str:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> str:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @property
+    @pulumi.getter(name="caCertPath")
+    def ca_cert_path(self) -> Optional[str]:
+        """
+        A path to a CA file accessible by a Node
+        """
+        return pulumi.get(self, "ca_cert_path")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class SecretStoreVaultToken(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "serverAddress":
             suggest = "server_address"
 
@@ -17036,43 +18026,271 @@
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
+class SecretStoreVaultTokenCertSsh(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "issuedCertTtlMinutes":
+            suggest = "issued_cert_ttl_minutes"
+        elif key == "serverAddress":
+            suggest = "server_address"
+        elif key == "signingRole":
+            suggest = "signing_role"
+        elif key == "sshMountPoint":
+            suggest = "ssh_mount_point"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SecretStoreVaultTokenCertSsh. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SecretStoreVaultTokenCertSsh.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SecretStoreVaultTokenCertSsh.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 issued_cert_ttl_minutes: int,
+                 name: str,
+                 server_address: str,
+                 signing_role: str,
+                 ssh_mount_point: str,
+                 namespace: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str server_address: The URL of the Vault to target
+        :param str signing_role: The signing role to be used for signing certificates
+        :param str ssh_mount_point: The mount point of the SSH engine configured with the desired CA
+        :param str namespace: The namespace to make requests within
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "server_address", server_address)
+        pulumi.set(__self__, "signing_role", signing_role)
+        pulumi.set(__self__, "ssh_mount_point", ssh_mount_point)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> int:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> str:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> str:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @property
+    @pulumi.getter(name="sshMountPoint")
+    def ssh_mount_point(self) -> str:
+        """
+        The mount point of the SSH engine configured with the desired CA
+        """
+        return pulumi.get(self, "ssh_mount_point")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
+class SecretStoreVaultTokenCertX509(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "issuedCertTtlMinutes":
+            suggest = "issued_cert_ttl_minutes"
+        elif key == "pkiMountPoint":
+            suggest = "pki_mount_point"
+        elif key == "serverAddress":
+            suggest = "server_address"
+        elif key == "signingRole":
+            suggest = "signing_role"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SecretStoreVaultTokenCertX509. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SecretStoreVaultTokenCertX509.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SecretStoreVaultTokenCertX509.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 issued_cert_ttl_minutes: int,
+                 name: str,
+                 pki_mount_point: str,
+                 server_address: str,
+                 signing_role: str,
+                 namespace: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str pki_mount_point: The mount point of the PKI engine configured with the desired CA
+        :param str server_address: The URL of the Vault to target
+        :param str signing_role: The signing role to be used for signing certificates
+        :param str namespace: The namespace to make requests within
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "pki_mount_point", pki_mount_point)
+        pulumi.set(__self__, "server_address", server_address)
+        pulumi.set(__self__, "signing_role", signing_role)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> int:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="pkiMountPoint")
+    def pki_mount_point(self) -> str:
+        """
+        The mount point of the PKI engine configured with the desired CA
+        """
+        return pulumi.get(self, "pki_mount_point")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> str:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> str:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class GetAccountAccountResult(dict):
     def __init__(__self__, *,
                  services: Sequence['outputs.GetAccountAccountServiceResult'],
                  users: Sequence['outputs.GetAccountAccountUserResult']):
+        """
+        :param Sequence['GetAccountAccountServiceArgs'] services: A Service is a service account that can connect to resources they are granted directly, or granted via roles. Services are typically automated jobs.
+        :param Sequence['GetAccountAccountUserArgs'] users: A User can connect to resources they are granted directly, or granted via roles.
+        """
         pulumi.set(__self__, "services", services)
         pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter
     def services(self) -> Sequence['outputs.GetAccountAccountServiceResult']:
+        """
+        A Service is a service account that can connect to resources they are granted directly, or granted via roles. Services are typically automated jobs.
+        """
         return pulumi.get(self, "services")
 
     @property
     @pulumi.getter
     def users(self) -> Sequence['outputs.GetAccountAccountUserResult']:
+        """
+        A User can connect to resources they are granted directly, or granted via roles.
+        """
         return pulumi.get(self, "users")
 
 
 @pulumi.output_type
 class GetAccountAccountServiceResult(dict):
     def __init__(__self__, *,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  suspended: Optional[bool] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str id: Unique identifier of the User.
         :param str name: Unique human-readable name of the Service.
-        :param bool suspended: The User's suspended state.
+        :param bool suspended: The Service's suspended state.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if suspended is not None:
@@ -17096,15 +18314,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def suspended(self) -> Optional[bool]:
         """
-        The User's suspended state.
+        The Service's suspended state.
         """
         return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
@@ -17113,65 +18331,65 @@
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
 class GetAccountAccountUserResult(dict):
     def __init__(__self__, *,
                  managed_by: str,
-                 permission_level: str,
+                 suspended: bool,
                  email: Optional[str] = None,
                  external_id: Optional[str] = None,
                  first_name: Optional[str] = None,
                  id: Optional[str] = None,
                  last_name: Optional[str] = None,
-                 suspended: Optional[bool] = None,
+                 permission_level: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str managed_by: Managed By is a read only field for what service manages this user, e.g. StrongDM, Okta, Azure.
-        :param str permission_level: PermissionLevel is a read only field for the user's permission level e.g. admin, DBA, user.
+        :param bool suspended: The Service's suspended state.
         :param str email: The User's email address. Must be unique.
         :param str external_id: External ID is an alternative unique ID this user is represented by within an external service.
         :param str first_name: The User's first name.
         :param str id: Unique identifier of the User.
         :param str last_name: The User's last name.
-        :param bool suspended: The User's suspended state.
+        :param str permission_level: PermissionLevel is the user's permission level e.g. admin, DBA, user.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "managed_by", managed_by)
-        pulumi.set(__self__, "permission_level", permission_level)
+        pulumi.set(__self__, "suspended", suspended)
         if email is not None:
             pulumi.set(__self__, "email", email)
         if external_id is not None:
             pulumi.set(__self__, "external_id", external_id)
         if first_name is not None:
             pulumi.set(__self__, "first_name", first_name)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if last_name is not None:
             pulumi.set(__self__, "last_name", last_name)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
+        if permission_level is not None:
+            pulumi.set(__self__, "permission_level", permission_level)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="managedBy")
     def managed_by(self) -> str:
         """
         Managed By is a read only field for what service manages this user, e.g. StrongDM, Okta, Azure.
         """
         return pulumi.get(self, "managed_by")
 
     @property
-    @pulumi.getter(name="permissionLevel")
-    def permission_level(self) -> str:
+    @pulumi.getter
+    def suspended(self) -> bool:
         """
-        PermissionLevel is a read only field for the user's permission level e.g. admin, DBA, user.
+        The Service's suspended state.
         """
-        return pulumi.get(self, "permission_level")
+        return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
     def email(self) -> Optional[str]:
         """
         The User's email address. Must be unique.
         """
@@ -17206,20 +18424,20 @@
     def last_name(self) -> Optional[str]:
         """
         The User's last name.
         """
         return pulumi.get(self, "last_name")
 
     @property
-    @pulumi.getter
-    def suspended(self) -> Optional[bool]:
+    @pulumi.getter(name="permissionLevel")
+    def permission_level(self) -> Optional[str]:
         """
-        The User's suspended state.
+        PermissionLevel is the user's permission level e.g. admin, DBA, user.
         """
-        return pulumi.get(self, "suspended")
+        return pulumi.get(self, "permission_level")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
@@ -17266,29 +18484,192 @@
         """
         The id of the attached role of this AccountAttachment.
         """
         return pulumi.get(self, "role_id")
 
 
 @pulumi.output_type
+class GetApprovalWorkflowApprovalWorkflowResult(dict):
+    def __init__(__self__, *,
+                 approval_mode: Optional[str] = None,
+                 description: Optional[str] = None,
+                 id: Optional[str] = None,
+                 name: Optional[str] = None):
+        """
+        :param str approval_mode: Approval mode of the ApprovalWorkflow
+        :param str description: Optional description of the ApprovalWorkflow.
+        :param str id: Unique identifier of the ApprovalWorkflow.
+        :param str name: Unique human-readable name of the ApprovalWorkflow.
+        """
+        if approval_mode is not None:
+            pulumi.set(__self__, "approval_mode", approval_mode)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter(name="approvalMode")
+    def approval_mode(self) -> Optional[str]:
+        """
+        Approval mode of the ApprovalWorkflow
+        """
+        return pulumi.get(self, "approval_mode")
+
+    @property
+    @pulumi.getter
+    def description(self) -> Optional[str]:
+        """
+        Optional description of the ApprovalWorkflow.
+        """
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the ApprovalWorkflow.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the ApprovalWorkflow.
+        """
+        return pulumi.get(self, "name")
+
+
+@pulumi.output_type
+class GetApprovalWorkflowApproverApprovalWorkflowApproverResult(dict):
+    def __init__(__self__, *,
+                 account_id: Optional[str] = None,
+                 approval_flow_id: Optional[str] = None,
+                 approval_step_id: Optional[str] = None,
+                 id: Optional[str] = None,
+                 role_id: Optional[str] = None):
+        """
+        :param str account_id: The approver account id.
+        :param str approval_flow_id: The approval flow id specified the approval workflow that this approver belongs to
+        :param str approval_step_id: The approval step id specified the approval flow step that this approver belongs to
+        :param str id: Unique identifier of the ApprovalWorkflowApprover.
+        :param str role_id: The approver role id
+        """
+        if account_id is not None:
+            pulumi.set(__self__, "account_id", account_id)
+        if approval_flow_id is not None:
+            pulumi.set(__self__, "approval_flow_id", approval_flow_id)
+        if approval_step_id is not None:
+            pulumi.set(__self__, "approval_step_id", approval_step_id)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if role_id is not None:
+            pulumi.set(__self__, "role_id", role_id)
+
+    @property
+    @pulumi.getter(name="accountId")
+    def account_id(self) -> Optional[str]:
+        """
+        The approver account id.
+        """
+        return pulumi.get(self, "account_id")
+
+    @property
+    @pulumi.getter(name="approvalFlowId")
+    def approval_flow_id(self) -> Optional[str]:
+        """
+        The approval flow id specified the approval workflow that this approver belongs to
+        """
+        return pulumi.get(self, "approval_flow_id")
+
+    @property
+    @pulumi.getter(name="approvalStepId")
+    def approval_step_id(self) -> Optional[str]:
+        """
+        The approval step id specified the approval flow step that this approver belongs to
+        """
+        return pulumi.get(self, "approval_step_id")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the ApprovalWorkflowApprover.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="roleId")
+    def role_id(self) -> Optional[str]:
+        """
+        The approver role id
+        """
+        return pulumi.get(self, "role_id")
+
+
+@pulumi.output_type
+class GetApprovalWorkflowStepApprovalWorkflowStepResult(dict):
+    def __init__(__self__, *,
+                 approval_flow_id: Optional[str] = None,
+                 id: Optional[str] = None):
+        """
+        :param str approval_flow_id: The approval flow id specified the approval workfflow that this step belongs to
+        :param str id: Unique identifier of the ApprovalWorkflowStep.
+        """
+        if approval_flow_id is not None:
+            pulumi.set(__self__, "approval_flow_id", approval_flow_id)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+
+    @property
+    @pulumi.getter(name="approvalFlowId")
+    def approval_flow_id(self) -> Optional[str]:
+        """
+        The approval flow id specified the approval workfflow that this step belongs to
+        """
+        return pulumi.get(self, "approval_flow_id")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the ApprovalWorkflowStep.
+        """
+        return pulumi.get(self, "id")
+
+
+@pulumi.output_type
 class GetNodeNodeResult(dict):
     def __init__(__self__, *,
                  gateways: Sequence['outputs.GetNodeNodeGatewayResult'],
                  relays: Sequence['outputs.GetNodeNodeRelayResult']):
+        """
+        :param Sequence['GetNodeNodeGatewayArgs'] gateways: Gateway represents a StrongDM CLI installation running in gateway mode.
+        :param Sequence['GetNodeNodeRelayArgs'] relays: Relay represents a StrongDM CLI installation running in relay mode.
+        """
         pulumi.set(__self__, "gateways", gateways)
         pulumi.set(__self__, "relays", relays)
 
     @property
     @pulumi.getter
     def gateways(self) -> Sequence['outputs.GetNodeNodeGatewayResult']:
+        """
+        Gateway represents a StrongDM CLI installation running in gateway mode.
+        """
         return pulumi.get(self, "gateways")
 
     @property
     @pulumi.getter
     def relays(self) -> Sequence['outputs.GetNodeNodeRelayResult']:
+        """
+        Relay represents a StrongDM CLI installation running in relay mode.
+        """
         return pulumi.get(self, "relays")
 
 
 @pulumi.output_type
 class GetNodeNodeGatewayResult(dict):
     def __init__(__self__, *,
                  device: str,
@@ -17861,14 +19242,15 @@
                  neptune_iams: Sequence['outputs.GetResourceResourceNeptuneIamResult'],
                  neptunes: Sequence['outputs.GetResourceResourceNeptuneResult'],
                  oracles: Sequence['outputs.GetResourceResourceOracleResult'],
                  postgres: Sequence['outputs.GetResourceResourcePostgreResult'],
                  prestos: Sequence['outputs.GetResourceResourcePrestoResult'],
                  rabbitmq_amqp091s: Sequence['outputs.GetResourceResourceRabbitmqAmqp091Result'],
                  raw_tcps: Sequence['outputs.GetResourceResourceRawTcpResult'],
+                 rdp_certs: Sequence['outputs.GetResourceResourceRdpCertResult'],
                  rdps: Sequence['outputs.GetResourceResourceRdpResult'],
                  rds_postgres_iams: Sequence['outputs.GetResourceResourceRdsPostgresIamResult'],
                  redis: Sequence['outputs.GetResourceResourceRediResult'],
                  redshifts: Sequence['outputs.GetResourceResourceRedshiftResult'],
                  single_stores: Sequence['outputs.GetResourceResourceSingleStoreResult'],
                  snowflakes: Sequence['outputs.GetResourceResourceSnowflakeResult'],
                  snowsights: Sequence['outputs.GetResourceResourceSnowsightResult'],
@@ -17944,14 +19326,15 @@
         pulumi.set(__self__, "neptune_iams", neptune_iams)
         pulumi.set(__self__, "neptunes", neptunes)
         pulumi.set(__self__, "oracles", oracles)
         pulumi.set(__self__, "postgres", postgres)
         pulumi.set(__self__, "prestos", prestos)
         pulumi.set(__self__, "rabbitmq_amqp091s", rabbitmq_amqp091s)
         pulumi.set(__self__, "raw_tcps", raw_tcps)
+        pulumi.set(__self__, "rdp_certs", rdp_certs)
         pulumi.set(__self__, "rdps", rdps)
         pulumi.set(__self__, "rds_postgres_iams", rds_postgres_iams)
         pulumi.set(__self__, "redis", redis)
         pulumi.set(__self__, "redshifts", redshifts)
         pulumi.set(__self__, "single_stores", single_stores)
         pulumi.set(__self__, "snowflakes", snowflakes)
         pulumi.set(__self__, "snowsights", snowsights)
@@ -18293,14 +19676,19 @@
 
     @property
     @pulumi.getter(name="rawTcps")
     def raw_tcps(self) -> Sequence['outputs.GetResourceResourceRawTcpResult']:
         return pulumi.get(self, "raw_tcps")
 
     @property
+    @pulumi.getter(name="rdpCerts")
+    def rdp_certs(self) -> Sequence['outputs.GetResourceResourceRdpCertResult']:
+        return pulumi.get(self, "rdp_certs")
+
+    @property
     @pulumi.getter
     def rdps(self) -> Sequence['outputs.GetResourceResourceRdpResult']:
         return pulumi.get(self, "rdps")
 
     @property
     @pulumi.getter(name="rdsPostgresIams")
     def rds_postgres_iams(self) -> Sequence['outputs.GetResourceResourceRdsPostgresIamResult']:
@@ -30086,14 +31474,177 @@
         """
         The username to authenticate with.
         """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
+class GetResourceResourceRdpCertResult(dict):
+    def __init__(__self__, *,
+                 bind_interface: Optional[str] = None,
+                 egress_filter: Optional[str] = None,
+                 hostname: Optional[str] = None,
+                 id: Optional[str] = None,
+                 name: Optional[str] = None,
+                 port: Optional[int] = None,
+                 port_override: Optional[int] = None,
+                 remote_identity_group_id: Optional[str] = None,
+                 remote_identity_healthcheck_username: Optional[str] = None,
+                 secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None,
+                 username: Optional[str] = None):
+        """
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
+        :param str id: Unique identifier of the Resource.
+        :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
+        """
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if hostname is not None:
+            pulumi.set(__self__, "hostname", hostname)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
+        if remote_identity_group_id is not None:
+            pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
+        if remote_identity_healthcheck_username is not None:
+            pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[str]:
+        """
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[str]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @property
+    @pulumi.getter
+    def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
+        return pulumi.get(self, "hostname")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the Resource.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
+        return pulumi.get(self, "port")
+
+    @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
+        return pulumi.get(self, "port_override")
+
+    @property
+    @pulumi.getter(name="remoteIdentityGroupId")
+    def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
+        return pulumi.get(self, "remote_identity_group_id")
+
+    @property
+    @pulumi.getter(name="remoteIdentityHealthcheckUsername")
+    def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
+        return pulumi.get(self, "remote_identity_healthcheck_username")
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[str]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
+        return pulumi.get(self, "username")
+
+
+@pulumi.output_type
 class GetResourceResourceRdsPostgresIamResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
                  database: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
@@ -32979,41 +34530,69 @@
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
 class GetSecretStoreSecretStoreResult(dict):
     def __init__(__self__, *,
+                 active_directory_stores: Sequence['outputs.GetSecretStoreSecretStoreActiveDirectoryStoreResult'],
                  aws: Sequence['outputs.GetSecretStoreSecretStoreAwResult'],
+                 aws_cert_x509s: Sequence['outputs.GetSecretStoreSecretStoreAwsCertX509Result'],
                  azure_stores: Sequence['outputs.GetSecretStoreSecretStoreAzureStoreResult'],
                  cyberark_conjurs: Sequence['outputs.GetSecretStoreSecretStoreCyberarkConjurResult'],
                  cyberark_pam_experimentals: Sequence['outputs.GetSecretStoreSecretStoreCyberarkPamExperimentalResult'],
                  cyberark_pams: Sequence['outputs.GetSecretStoreSecretStoreCyberarkPamResult'],
                  delinea_stores: Sequence['outputs.GetSecretStoreSecretStoreDelineaStoreResult'],
+                 gcp_cert_x509_stores: Sequence['outputs.GetSecretStoreSecretStoreGcpCertX509StoreResult'],
                  gcp_stores: Sequence['outputs.GetSecretStoreSecretStoreGcpStoreResult'],
+                 vault_approle_cert_sshes: Sequence['outputs.GetSecretStoreSecretStoreVaultApproleCertSshResult'],
+                 vault_approle_cert_x509s: Sequence['outputs.GetSecretStoreSecretStoreVaultApproleCertX509Result'],
                  vault_approles: Sequence['outputs.GetSecretStoreSecretStoreVaultApproleResult'],
                  vault_tls: Sequence['outputs.GetSecretStoreSecretStoreVaultTlResult'],
+                 vault_tls_cert_sshes: Sequence['outputs.GetSecretStoreSecretStoreVaultTlsCertSshResult'],
+                 vault_tls_cert_x509s: Sequence['outputs.GetSecretStoreSecretStoreVaultTlsCertX509Result'],
+                 vault_token_cert_sshes: Sequence['outputs.GetSecretStoreSecretStoreVaultTokenCertSshResult'],
+                 vault_token_cert_x509s: Sequence['outputs.GetSecretStoreSecretStoreVaultTokenCertX509Result'],
                  vault_tokens: Sequence['outputs.GetSecretStoreSecretStoreVaultTokenResult']):
+        pulumi.set(__self__, "active_directory_stores", active_directory_stores)
         pulumi.set(__self__, "aws", aws)
+        pulumi.set(__self__, "aws_cert_x509s", aws_cert_x509s)
         pulumi.set(__self__, "azure_stores", azure_stores)
         pulumi.set(__self__, "cyberark_conjurs", cyberark_conjurs)
         pulumi.set(__self__, "cyberark_pam_experimentals", cyberark_pam_experimentals)
         pulumi.set(__self__, "cyberark_pams", cyberark_pams)
         pulumi.set(__self__, "delinea_stores", delinea_stores)
+        pulumi.set(__self__, "gcp_cert_x509_stores", gcp_cert_x509_stores)
         pulumi.set(__self__, "gcp_stores", gcp_stores)
+        pulumi.set(__self__, "vault_approle_cert_sshes", vault_approle_cert_sshes)
+        pulumi.set(__self__, "vault_approle_cert_x509s", vault_approle_cert_x509s)
         pulumi.set(__self__, "vault_approles", vault_approles)
         pulumi.set(__self__, "vault_tls", vault_tls)
+        pulumi.set(__self__, "vault_tls_cert_sshes", vault_tls_cert_sshes)
+        pulumi.set(__self__, "vault_tls_cert_x509s", vault_tls_cert_x509s)
+        pulumi.set(__self__, "vault_token_cert_sshes", vault_token_cert_sshes)
+        pulumi.set(__self__, "vault_token_cert_x509s", vault_token_cert_x509s)
         pulumi.set(__self__, "vault_tokens", vault_tokens)
 
     @property
+    @pulumi.getter(name="activeDirectoryStores")
+    def active_directory_stores(self) -> Sequence['outputs.GetSecretStoreSecretStoreActiveDirectoryStoreResult']:
+        return pulumi.get(self, "active_directory_stores")
+
+    @property
     @pulumi.getter
     def aws(self) -> Sequence['outputs.GetSecretStoreSecretStoreAwResult']:
         return pulumi.get(self, "aws")
 
     @property
+    @pulumi.getter(name="awsCertX509s")
+    def aws_cert_x509s(self) -> Sequence['outputs.GetSecretStoreSecretStoreAwsCertX509Result']:
+        return pulumi.get(self, "aws_cert_x509s")
+
+    @property
     @pulumi.getter(name="azureStores")
     def azure_stores(self) -> Sequence['outputs.GetSecretStoreSecretStoreAzureStoreResult']:
         return pulumi.get(self, "azure_stores")
 
     @property
     @pulumi.getter(name="cyberarkConjurs")
     def cyberark_conjurs(self) -> Sequence['outputs.GetSecretStoreSecretStoreCyberarkConjurResult']:
@@ -33031,35 +34610,125 @@
 
     @property
     @pulumi.getter(name="delineaStores")
     def delinea_stores(self) -> Sequence['outputs.GetSecretStoreSecretStoreDelineaStoreResult']:
         return pulumi.get(self, "delinea_stores")
 
     @property
+    @pulumi.getter(name="gcpCertX509Stores")
+    def gcp_cert_x509_stores(self) -> Sequence['outputs.GetSecretStoreSecretStoreGcpCertX509StoreResult']:
+        return pulumi.get(self, "gcp_cert_x509_stores")
+
+    @property
     @pulumi.getter(name="gcpStores")
     def gcp_stores(self) -> Sequence['outputs.GetSecretStoreSecretStoreGcpStoreResult']:
         return pulumi.get(self, "gcp_stores")
 
     @property
+    @pulumi.getter(name="vaultApproleCertSshes")
+    def vault_approle_cert_sshes(self) -> Sequence['outputs.GetSecretStoreSecretStoreVaultApproleCertSshResult']:
+        return pulumi.get(self, "vault_approle_cert_sshes")
+
+    @property
+    @pulumi.getter(name="vaultApproleCertX509s")
+    def vault_approle_cert_x509s(self) -> Sequence['outputs.GetSecretStoreSecretStoreVaultApproleCertX509Result']:
+        return pulumi.get(self, "vault_approle_cert_x509s")
+
+    @property
     @pulumi.getter(name="vaultApproles")
     def vault_approles(self) -> Sequence['outputs.GetSecretStoreSecretStoreVaultApproleResult']:
         return pulumi.get(self, "vault_approles")
 
     @property
     @pulumi.getter(name="vaultTls")
     def vault_tls(self) -> Sequence['outputs.GetSecretStoreSecretStoreVaultTlResult']:
         return pulumi.get(self, "vault_tls")
 
     @property
+    @pulumi.getter(name="vaultTlsCertSshes")
+    def vault_tls_cert_sshes(self) -> Sequence['outputs.GetSecretStoreSecretStoreVaultTlsCertSshResult']:
+        return pulumi.get(self, "vault_tls_cert_sshes")
+
+    @property
+    @pulumi.getter(name="vaultTlsCertX509s")
+    def vault_tls_cert_x509s(self) -> Sequence['outputs.GetSecretStoreSecretStoreVaultTlsCertX509Result']:
+        return pulumi.get(self, "vault_tls_cert_x509s")
+
+    @property
+    @pulumi.getter(name="vaultTokenCertSshes")
+    def vault_token_cert_sshes(self) -> Sequence['outputs.GetSecretStoreSecretStoreVaultTokenCertSshResult']:
+        return pulumi.get(self, "vault_token_cert_sshes")
+
+    @property
+    @pulumi.getter(name="vaultTokenCertX509s")
+    def vault_token_cert_x509s(self) -> Sequence['outputs.GetSecretStoreSecretStoreVaultTokenCertX509Result']:
+        return pulumi.get(self, "vault_token_cert_x509s")
+
+    @property
     @pulumi.getter(name="vaultTokens")
     def vault_tokens(self) -> Sequence['outputs.GetSecretStoreSecretStoreVaultTokenResult']:
         return pulumi.get(self, "vault_tokens")
 
 
 @pulumi.output_type
+class GetSecretStoreSecretStoreActiveDirectoryStoreResult(dict):
+    def __init__(__self__, *,
+                 id: Optional[str] = None,
+                 name: Optional[str] = None,
+                 server_address: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str id: Unique identifier of the SecretStore.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str server_address: The URL of the Vault to target
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if server_address is not None:
+            pulumi.set(__self__, "server_address", server_address)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the SecretStore.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> Optional[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class GetSecretStoreSecretStoreAwResult(dict):
     def __init__(__self__, *,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  region: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
@@ -33107,14 +34776,117 @@
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
+class GetSecretStoreSecretStoreAwsCertX509Result(dict):
+    def __init__(__self__, *,
+                 ca_arn: Optional[str] = None,
+                 certificate_template_arn: Optional[str] = None,
+                 id: Optional[str] = None,
+                 issued_cert_ttl_minutes: Optional[int] = None,
+                 name: Optional[str] = None,
+                 region: Optional[str] = None,
+                 signing_algo: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str ca_arn: The ARN of the CA in AWS Private CA
+        :param str certificate_template_arn: The ARN of the AWS certificate template for requested certificates. Must allow SAN, key usage, and ext key usage passthrough from CSR
+        :param str id: Unique identifier of the SecretStore.
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str region: The AWS region to target e.g. us-east-1
+        :param str signing_algo: The specified signing algorithm family (RSA or ECDSA) must match the algorithm family of the CA's secret key. e.g. SHA256WITHRSA
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if ca_arn is not None:
+            pulumi.set(__self__, "ca_arn", ca_arn)
+        if certificate_template_arn is not None:
+            pulumi.set(__self__, "certificate_template_arn", certificate_template_arn)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if issued_cert_ttl_minutes is not None:
+            pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if region is not None:
+            pulumi.set(__self__, "region", region)
+        if signing_algo is not None:
+            pulumi.set(__self__, "signing_algo", signing_algo)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="caArn")
+    def ca_arn(self) -> Optional[str]:
+        """
+        The ARN of the CA in AWS Private CA
+        """
+        return pulumi.get(self, "ca_arn")
+
+    @property
+    @pulumi.getter(name="certificateTemplateArn")
+    def certificate_template_arn(self) -> Optional[str]:
+        """
+        The ARN of the AWS certificate template for requested certificates. Must allow SAN, key usage, and ext key usage passthrough from CSR
+        """
+        return pulumi.get(self, "certificate_template_arn")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the SecretStore.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> Optional[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def region(self) -> Optional[str]:
+        """
+        The AWS region to target e.g. us-east-1
+        """
+        return pulumi.get(self, "region")
+
+    @property
+    @pulumi.getter(name="signingAlgo")
+    def signing_algo(self) -> Optional[str]:
+        """
+        The specified signing algorithm family (RSA or ECDSA) must match the algorithm family of the CA's secret key. e.g. SHA256WITHRSA
+        """
+        return pulumi.get(self, "signing_algo")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class GetSecretStoreSecretStoreAzureStoreResult(dict):
     def __init__(__self__, *,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  vault_uri: Optional[str] = None):
         """
@@ -33398,14 +35170,117 @@
         The tenant name to target
         * gcp_store:
         """
         return pulumi.get(self, "tenant_name")
 
 
 @pulumi.output_type
+class GetSecretStoreSecretStoreGcpCertX509StoreResult(dict):
+    def __init__(__self__, *,
+                 ca_id: Optional[str] = None,
+                 ca_pool_id: Optional[str] = None,
+                 id: Optional[str] = None,
+                 issued_cert_ttl_minutes: Optional[int] = None,
+                 location: Optional[str] = None,
+                 name: Optional[str] = None,
+                 project_id: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str ca_id: The ID of the target CA
+        :param str ca_pool_id: The ID of the target CA pool
+        :param str id: Unique identifier of the SecretStore.
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str location: The Region for the CA in GCP format e.g. us-west1
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str project_id: The GCP project ID to target.
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if ca_id is not None:
+            pulumi.set(__self__, "ca_id", ca_id)
+        if ca_pool_id is not None:
+            pulumi.set(__self__, "ca_pool_id", ca_pool_id)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if issued_cert_ttl_minutes is not None:
+            pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        if location is not None:
+            pulumi.set(__self__, "location", location)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if project_id is not None:
+            pulumi.set(__self__, "project_id", project_id)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="caId")
+    def ca_id(self) -> Optional[str]:
+        """
+        The ID of the target CA
+        """
+        return pulumi.get(self, "ca_id")
+
+    @property
+    @pulumi.getter(name="caPoolId")
+    def ca_pool_id(self) -> Optional[str]:
+        """
+        The ID of the target CA pool
+        """
+        return pulumi.get(self, "ca_pool_id")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the SecretStore.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> Optional[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def location(self) -> Optional[str]:
+        """
+        The Region for the CA in GCP format e.g. us-west1
+        """
+        return pulumi.get(self, "location")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> Optional[str]:
+        """
+        The GCP project ID to target.
+        """
+        return pulumi.get(self, "project_id")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class GetSecretStoreSecretStoreGcpStoreResult(dict):
     def __init__(__self__, *,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  project_id: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
@@ -33520,14 +35395,220 @@
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
+class GetSecretStoreSecretStoreVaultApproleCertSshResult(dict):
+    def __init__(__self__, *,
+                 id: Optional[str] = None,
+                 issued_cert_ttl_minutes: Optional[int] = None,
+                 name: Optional[str] = None,
+                 namespace: Optional[str] = None,
+                 server_address: Optional[str] = None,
+                 signing_role: Optional[str] = None,
+                 ssh_mount_point: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str id: Unique identifier of the SecretStore.
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str namespace: The namespace to make requests within
+        :param str server_address: The URL of the Vault to target
+        :param str signing_role: The signing role to be used for signing certificates
+        :param str ssh_mount_point: The mount point of the SSH engine configured with the desired CA
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if issued_cert_ttl_minutes is not None:
+            pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if server_address is not None:
+            pulumi.set(__self__, "server_address", server_address)
+        if signing_role is not None:
+            pulumi.set(__self__, "signing_role", signing_role)
+        if ssh_mount_point is not None:
+            pulumi.set(__self__, "ssh_mount_point", ssh_mount_point)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the SecretStore.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> Optional[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> Optional[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> Optional[str]:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @property
+    @pulumi.getter(name="sshMountPoint")
+    def ssh_mount_point(self) -> Optional[str]:
+        """
+        The mount point of the SSH engine configured with the desired CA
+        """
+        return pulumi.get(self, "ssh_mount_point")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
+class GetSecretStoreSecretStoreVaultApproleCertX509Result(dict):
+    def __init__(__self__, *,
+                 id: Optional[str] = None,
+                 issued_cert_ttl_minutes: Optional[int] = None,
+                 name: Optional[str] = None,
+                 namespace: Optional[str] = None,
+                 pki_mount_point: Optional[str] = None,
+                 server_address: Optional[str] = None,
+                 signing_role: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str id: Unique identifier of the SecretStore.
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str namespace: The namespace to make requests within
+        :param str pki_mount_point: The mount point of the PKI engine configured with the desired CA
+        :param str server_address: The URL of the Vault to target
+        :param str signing_role: The signing role to be used for signing certificates
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if issued_cert_ttl_minutes is not None:
+            pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if pki_mount_point is not None:
+            pulumi.set(__self__, "pki_mount_point", pki_mount_point)
+        if server_address is not None:
+            pulumi.set(__self__, "server_address", server_address)
+        if signing_role is not None:
+            pulumi.set(__self__, "signing_role", signing_role)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the SecretStore.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> Optional[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
+    @pulumi.getter(name="pkiMountPoint")
+    def pki_mount_point(self) -> Optional[str]:
+        """
+        The mount point of the PKI engine configured with the desired CA
+        """
+        return pulumi.get(self, "pki_mount_point")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> Optional[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> Optional[str]:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class GetSecretStoreSecretStoreVaultTlResult(dict):
     def __init__(__self__, *,
                  ca_cert_path: Optional[str] = None,
                  client_cert_path: Optional[str] = None,
                  client_key_path: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
@@ -33623,14 +35704,292 @@
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
+class GetSecretStoreSecretStoreVaultTlsCertSshResult(dict):
+    def __init__(__self__, *,
+                 ca_cert_path: Optional[str] = None,
+                 client_cert_path: Optional[str] = None,
+                 client_key_path: Optional[str] = None,
+                 id: Optional[str] = None,
+                 issued_cert_ttl_minutes: Optional[int] = None,
+                 name: Optional[str] = None,
+                 namespace: Optional[str] = None,
+                 server_address: Optional[str] = None,
+                 signing_role: Optional[str] = None,
+                 ssh_mount_point: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str ca_cert_path: A path to a CA file accessible by a Node
+        :param str client_cert_path: A path to a client certificate file accessible by a Node
+        :param str client_key_path: A path to a client key file accessible by a Node
+        :param str id: Unique identifier of the SecretStore.
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str namespace: The namespace to make requests within
+        :param str server_address: The URL of the Vault to target
+        :param str signing_role: The signing role to be used for signing certificates
+        :param str ssh_mount_point: The mount point of the SSH engine configured with the desired CA
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if ca_cert_path is not None:
+            pulumi.set(__self__, "ca_cert_path", ca_cert_path)
+        if client_cert_path is not None:
+            pulumi.set(__self__, "client_cert_path", client_cert_path)
+        if client_key_path is not None:
+            pulumi.set(__self__, "client_key_path", client_key_path)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if issued_cert_ttl_minutes is not None:
+            pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if server_address is not None:
+            pulumi.set(__self__, "server_address", server_address)
+        if signing_role is not None:
+            pulumi.set(__self__, "signing_role", signing_role)
+        if ssh_mount_point is not None:
+            pulumi.set(__self__, "ssh_mount_point", ssh_mount_point)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="caCertPath")
+    def ca_cert_path(self) -> Optional[str]:
+        """
+        A path to a CA file accessible by a Node
+        """
+        return pulumi.get(self, "ca_cert_path")
+
+    @property
+    @pulumi.getter(name="clientCertPath")
+    def client_cert_path(self) -> Optional[str]:
+        """
+        A path to a client certificate file accessible by a Node
+        """
+        return pulumi.get(self, "client_cert_path")
+
+    @property
+    @pulumi.getter(name="clientKeyPath")
+    def client_key_path(self) -> Optional[str]:
+        """
+        A path to a client key file accessible by a Node
+        """
+        return pulumi.get(self, "client_key_path")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the SecretStore.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> Optional[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> Optional[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> Optional[str]:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @property
+    @pulumi.getter(name="sshMountPoint")
+    def ssh_mount_point(self) -> Optional[str]:
+        """
+        The mount point of the SSH engine configured with the desired CA
+        """
+        return pulumi.get(self, "ssh_mount_point")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
+class GetSecretStoreSecretStoreVaultTlsCertX509Result(dict):
+    def __init__(__self__, *,
+                 ca_cert_path: Optional[str] = None,
+                 client_cert_path: Optional[str] = None,
+                 client_key_path: Optional[str] = None,
+                 id: Optional[str] = None,
+                 issued_cert_ttl_minutes: Optional[int] = None,
+                 name: Optional[str] = None,
+                 namespace: Optional[str] = None,
+                 pki_mount_point: Optional[str] = None,
+                 server_address: Optional[str] = None,
+                 signing_role: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str ca_cert_path: A path to a CA file accessible by a Node
+        :param str client_cert_path: A path to a client certificate file accessible by a Node
+        :param str client_key_path: A path to a client key file accessible by a Node
+        :param str id: Unique identifier of the SecretStore.
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str namespace: The namespace to make requests within
+        :param str pki_mount_point: The mount point of the PKI engine configured with the desired CA
+        :param str server_address: The URL of the Vault to target
+        :param str signing_role: The signing role to be used for signing certificates
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if ca_cert_path is not None:
+            pulumi.set(__self__, "ca_cert_path", ca_cert_path)
+        if client_cert_path is not None:
+            pulumi.set(__self__, "client_cert_path", client_cert_path)
+        if client_key_path is not None:
+            pulumi.set(__self__, "client_key_path", client_key_path)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if issued_cert_ttl_minutes is not None:
+            pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if pki_mount_point is not None:
+            pulumi.set(__self__, "pki_mount_point", pki_mount_point)
+        if server_address is not None:
+            pulumi.set(__self__, "server_address", server_address)
+        if signing_role is not None:
+            pulumi.set(__self__, "signing_role", signing_role)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="caCertPath")
+    def ca_cert_path(self) -> Optional[str]:
+        """
+        A path to a CA file accessible by a Node
+        """
+        return pulumi.get(self, "ca_cert_path")
+
+    @property
+    @pulumi.getter(name="clientCertPath")
+    def client_cert_path(self) -> Optional[str]:
+        """
+        A path to a client certificate file accessible by a Node
+        """
+        return pulumi.get(self, "client_cert_path")
+
+    @property
+    @pulumi.getter(name="clientKeyPath")
+    def client_key_path(self) -> Optional[str]:
+        """
+        A path to a client key file accessible by a Node
+        """
+        return pulumi.get(self, "client_key_path")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the SecretStore.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> Optional[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
+    @pulumi.getter(name="pkiMountPoint")
+    def pki_mount_point(self) -> Optional[str]:
+        """
+        The mount point of the PKI engine configured with the desired CA
+        """
+        return pulumi.get(self, "pki_mount_point")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> Optional[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> Optional[str]:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class GetSecretStoreSecretStoreVaultTokenResult(dict):
     def __init__(__self__, *,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  namespace: Optional[str] = None,
                  server_address: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
@@ -33690,48 +36049,266 @@
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
+class GetSecretStoreSecretStoreVaultTokenCertSshResult(dict):
+    def __init__(__self__, *,
+                 id: Optional[str] = None,
+                 issued_cert_ttl_minutes: Optional[int] = None,
+                 name: Optional[str] = None,
+                 namespace: Optional[str] = None,
+                 server_address: Optional[str] = None,
+                 signing_role: Optional[str] = None,
+                 ssh_mount_point: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str id: Unique identifier of the SecretStore.
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str namespace: The namespace to make requests within
+        :param str server_address: The URL of the Vault to target
+        :param str signing_role: The signing role to be used for signing certificates
+        :param str ssh_mount_point: The mount point of the SSH engine configured with the desired CA
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if issued_cert_ttl_minutes is not None:
+            pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if server_address is not None:
+            pulumi.set(__self__, "server_address", server_address)
+        if signing_role is not None:
+            pulumi.set(__self__, "signing_role", signing_role)
+        if ssh_mount_point is not None:
+            pulumi.set(__self__, "ssh_mount_point", ssh_mount_point)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the SecretStore.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> Optional[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> Optional[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> Optional[str]:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @property
+    @pulumi.getter(name="sshMountPoint")
+    def ssh_mount_point(self) -> Optional[str]:
+        """
+        The mount point of the SSH engine configured with the desired CA
+        """
+        return pulumi.get(self, "ssh_mount_point")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
+class GetSecretStoreSecretStoreVaultTokenCertX509Result(dict):
+    def __init__(__self__, *,
+                 id: Optional[str] = None,
+                 issued_cert_ttl_minutes: Optional[int] = None,
+                 name: Optional[str] = None,
+                 namespace: Optional[str] = None,
+                 pki_mount_point: Optional[str] = None,
+                 server_address: Optional[str] = None,
+                 signing_role: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str id: Unique identifier of the SecretStore.
+        :param int issued_cert_ttl_minutes: The lifetime of certificates issued by this CA represented in minutes.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param str namespace: The namespace to make requests within
+        :param str pki_mount_point: The mount point of the PKI engine configured with the desired CA
+        :param str server_address: The URL of the Vault to target
+        :param str signing_role: The signing role to be used for signing certificates
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if issued_cert_ttl_minutes is not None:
+            pulumi.set(__self__, "issued_cert_ttl_minutes", issued_cert_ttl_minutes)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
+        if pki_mount_point is not None:
+            pulumi.set(__self__, "pki_mount_point", pki_mount_point)
+        if server_address is not None:
+            pulumi.set(__self__, "server_address", server_address)
+        if signing_role is not None:
+            pulumi.set(__self__, "signing_role", signing_role)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the SecretStore.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="issuedCertTtlMinutes")
+    def issued_cert_ttl_minutes(self) -> Optional[int]:
+        """
+        The lifetime of certificates issued by this CA represented in minutes.
+        """
+        return pulumi.get(self, "issued_cert_ttl_minutes")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
+    @pulumi.getter(name="pkiMountPoint")
+    def pki_mount_point(self) -> Optional[str]:
+        """
+        The mount point of the PKI engine configured with the desired CA
+        """
+        return pulumi.get(self, "pki_mount_point")
+
+    @property
+    @pulumi.getter(name="serverAddress")
+    def server_address(self) -> Optional[str]:
+        """
+        The URL of the Vault to target
+        """
+        return pulumi.get(self, "server_address")
+
+    @property
+    @pulumi.getter(name="signingRole")
+    def signing_role(self) -> Optional[str]:
+        """
+        The signing role to be used for signing certificates
+        """
+        return pulumi.get(self, "signing_role")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class GetWorkflowApproverWorkflowApproverResult(dict):
     def __init__(__self__, *,
-                 approver_id: Optional[str] = None,
+                 account_id: Optional[str] = None,
                  id: Optional[str] = None,
+                 role_id: Optional[str] = None,
                  workflow_id: Optional[str] = None):
         """
-        :param str approver_id: The approver id.
+        :param str account_id: The approver account id.
         :param str id: Unique identifier of the WorkflowApprover.
+        :param str role_id: The approver role id
         :param str workflow_id: The workflow id.
         """
-        if approver_id is not None:
-            pulumi.set(__self__, "approver_id", approver_id)
+        if account_id is not None:
+            pulumi.set(__self__, "account_id", account_id)
         if id is not None:
             pulumi.set(__self__, "id", id)
+        if role_id is not None:
+            pulumi.set(__self__, "role_id", role_id)
         if workflow_id is not None:
             pulumi.set(__self__, "workflow_id", workflow_id)
 
     @property
-    @pulumi.getter(name="approverId")
-    def approver_id(self) -> Optional[str]:
+    @pulumi.getter(name="accountId")
+    def account_id(self) -> Optional[str]:
         """
-        The approver id.
+        The approver account id.
         """
-        return pulumi.get(self, "approver_id")
+        return pulumi.get(self, "account_id")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the WorkflowApprover.
         """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="roleId")
+    def role_id(self) -> Optional[str]:
+        """
+        The approver role id
+        """
+        return pulumi.get(self, "role_id")
+
+    @property
     @pulumi.getter(name="workflowId")
     def workflow_id(self) -> Optional[str]:
         """
         The workflow id.
         """
         return pulumi.get(self, "workflow_id")
 
@@ -33779,31 +36356,35 @@
         return pulumi.get(self, "workflow_id")
 
 
 @pulumi.output_type
 class GetWorkflowWorkflowResult(dict):
     def __init__(__self__, *,
                  access_rules: Optional[str] = None,
+                 approval_flow_id: Optional[str] = None,
                  auto_grant: Optional[bool] = None,
                  description: Optional[str] = None,
                  enabled: Optional[bool] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  weight: Optional[int] = None):
         """
         :param str access_rules: AccessRules is a list of access rules defining the resources this Workflow provides access to.
+        :param str approval_flow_id: Optional approval flow ID identifies an approval flow that linked to the workflow
         :param bool auto_grant: Optional auto grant setting to automatically approve requests or not, defaults to false.
         :param str description: Optional description of the Workflow.
         :param bool enabled: Optional enabled state for workflow. This setting may be overridden by the system if the workflow doesn't meet the requirements to be enabled or if other conditions prevent enabling the workflow. The requirements to enable a workflow are that the workflow must be either set up for with auto grant enabled or have one or more WorkflowApprovers created for the workflow.
         :param str id: Unique identifier of the Workflow.
         :param str name: Unique human-readable name of the Workflow.
         :param int weight: Optional weight for workflow to specify it's priority in matching a request.
         """
         if access_rules is not None:
             pulumi.set(__self__, "access_rules", access_rules)
+        if approval_flow_id is not None:
+            pulumi.set(__self__, "approval_flow_id", approval_flow_id)
         if auto_grant is not None:
             pulumi.set(__self__, "auto_grant", auto_grant)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if id is not None:
@@ -33818,14 +36399,22 @@
     def access_rules(self) -> Optional[str]:
         """
         AccessRules is a list of access rules defining the resources this Workflow provides access to.
         """
         return pulumi.get(self, "access_rules")
 
     @property
+    @pulumi.getter(name="approvalFlowId")
+    def approval_flow_id(self) -> Optional[str]:
+        """
+        Optional approval flow ID identifies an approval flow that linked to the workflow
+        """
+        return pulumi.get(self, "approval_flow_id")
+
+    @property
     @pulumi.getter(name="autoGrant")
     def auto_grant(self) -> Optional[bool]:
         """
         Optional auto grant setting to automatically approve requests or not, defaults to false.
         """
         return pulumi.get(self, "auto_grant")
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/peering_group.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/peering_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         This resource can be imported using the import command.
 
         ## Import
 
         A PeeringGroup can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/peeringGroup:PeeringGroup example g-12345678
+        $ pulumi import sdm:index/peeringGroup:PeeringGroup example g-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: Unique human-readable name of the PeeringGroup.
         """
         ...
@@ -95,15 +95,15 @@
         This resource can be imported using the import command.
 
         ## Import
 
         A PeeringGroup can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/peeringGroup:PeeringGroup example g-12345678
+        $ pulumi import sdm:index/peeringGroup:PeeringGroup example g-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param PeeringGroupArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/peering_group_node.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/peering_group_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         This resource can be imported using the import command.
 
         ## Import
 
         A PeeringGroupNode can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/peeringGroupNode:PeeringGroupNode example gn-12345678
+        $ pulumi import sdm:index/peeringGroupNode:PeeringGroupNode example gn-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] group_id: Peering Group ID to which the node will be attached to.
         :param pulumi.Input[str] node_id: Node ID to be attached.
         """
@@ -127,15 +127,15 @@
         This resource can be imported using the import command.
 
         ## Import
 
         A PeeringGroupNode can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/peeringGroupNode:PeeringGroupNode example gn-12345678
+        $ pulumi import sdm:index/peeringGroupNode:PeeringGroupNode example gn-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param PeeringGroupNodeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/peering_group_peer.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/peering_group_peer.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         This resource can be imported using the import command.
 
         ## Import
 
         A PeeringGroupPeer can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/peeringGroupPeer:PeeringGroupPeer example gp-12345678
+        $ pulumi import sdm:index/peeringGroupPeer:PeeringGroupPeer example gp-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] group_id: Group ID from which the link will originate.
         :param pulumi.Input[str] peers_with_group_id: Peering Group ID to which Group ID will link.
         """
@@ -127,15 +127,15 @@
         This resource can be imported using the import command.
 
         ## Import
 
         A PeeringGroupPeer can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/peeringGroupPeer:PeeringGroupPeer example gp-12345678
+        $ pulumi import sdm:index/peeringGroupPeer:PeeringGroupPeer example gp-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param PeeringGroupPeerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/peering_group_resource.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/peering_group_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         This resource can be imported using the import command.
 
         ## Import
 
         A PeeringGroupResource can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/peeringGroupResource:PeeringGroupResource example gr-12345678
+        $ pulumi import sdm:index/peeringGroupResource:PeeringGroupResource example gr-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] group_id: Peering Group ID to which the resource will be attached to.
         :param pulumi.Input[str] resource_id: Resource ID to be attached.
         """
@@ -127,15 +127,15 @@
         This resource can be imported using the import command.
 
         ## Import
 
         A PeeringGroupResource can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/peeringGroupResource:PeeringGroupResource example gr-12345678
+        $ pulumi import sdm:index/peeringGroupResource:PeeringGroupResource example gr-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param PeeringGroupResourceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/provider.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/provider.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/remote_identity.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/remote_identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,21 +128,20 @@
                  account_id: Optional[pulumi.Input[str]] = None,
                  remote_identity_group_id: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         RemoteIdentities define the username to be used for a specific account
          when connecting to a remote resource using that group.
-
         ## Import
 
         A RemoteIdentity can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/remoteIdentity:RemoteIdentity example i-12345678
+        $ pulumi import sdm:index/remoteIdentity:RemoteIdentity example i-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] account_id: The account for this remote identity.
         :param pulumi.Input[str] remote_identity_group_id: The remote identity group.
         :param pulumi.Input[str] username: The username to be used as the remote identity for this account.
@@ -152,21 +151,20 @@
     def __init__(__self__,
                  resource_name: str,
                  args: RemoteIdentityArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         RemoteIdentities define the username to be used for a specific account
          when connecting to a remote resource using that group.
-
         ## Import
 
         A RemoteIdentity can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/remoteIdentity:RemoteIdentity example i-12345678
+        $ pulumi import sdm:index/remoteIdentity:RemoteIdentity example i-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param RemoteIdentityArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/resource.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
                  neptune_iam: Optional[pulumi.Input['ResourceNeptuneIamArgs']] = None,
                  oracle: Optional[pulumi.Input['ResourceOracleArgs']] = None,
                  postgres: Optional[pulumi.Input['ResourcePostgresArgs']] = None,
                  presto: Optional[pulumi.Input['ResourcePrestoArgs']] = None,
                  rabbitmq_amqp091: Optional[pulumi.Input['ResourceRabbitmqAmqp091Args']] = None,
                  raw_tcp: Optional[pulumi.Input['ResourceRawTcpArgs']] = None,
                  rdp: Optional[pulumi.Input['ResourceRdpArgs']] = None,
+                 rdp_cert: Optional[pulumi.Input['ResourceRdpCertArgs']] = None,
                  rds_postgres_iam: Optional[pulumi.Input['ResourceRdsPostgresIamArgs']] = None,
                  redis: Optional[pulumi.Input['ResourceRedisArgs']] = None,
                  redshift: Optional[pulumi.Input['ResourceRedshiftArgs']] = None,
                  single_store: Optional[pulumi.Input['ResourceSingleStoreArgs']] = None,
                  snowflake: Optional[pulumi.Input['ResourceSnowflakeArgs']] = None,
                  snowsight: Optional[pulumi.Input['ResourceSnowsightArgs']] = None,
                  sql_server: Optional[pulumi.Input['ResourceSqlServerArgs']] = None,
@@ -237,14 +238,16 @@
             pulumi.set(__self__, "presto", presto)
         if rabbitmq_amqp091 is not None:
             pulumi.set(__self__, "rabbitmq_amqp091", rabbitmq_amqp091)
         if raw_tcp is not None:
             pulumi.set(__self__, "raw_tcp", raw_tcp)
         if rdp is not None:
             pulumi.set(__self__, "rdp", rdp)
+        if rdp_cert is not None:
+            pulumi.set(__self__, "rdp_cert", rdp_cert)
         if rds_postgres_iam is not None:
             pulumi.set(__self__, "rds_postgres_iam", rds_postgres_iam)
         if redis is not None:
             pulumi.set(__self__, "redis", redis)
         if redshift is not None:
             pulumi.set(__self__, "redshift", redshift)
         if single_store is not None:
@@ -886,14 +889,23 @@
         return pulumi.get(self, "rdp")
 
     @rdp.setter
     def rdp(self, value: Optional[pulumi.Input['ResourceRdpArgs']]):
         pulumi.set(self, "rdp", value)
 
     @property
+    @pulumi.getter(name="rdpCert")
+    def rdp_cert(self) -> Optional[pulumi.Input['ResourceRdpCertArgs']]:
+        return pulumi.get(self, "rdp_cert")
+
+    @rdp_cert.setter
+    def rdp_cert(self, value: Optional[pulumi.Input['ResourceRdpCertArgs']]):
+        pulumi.set(self, "rdp_cert", value)
+
+    @property
     @pulumi.getter(name="rdsPostgresIam")
     def rds_postgres_iam(self) -> Optional[pulumi.Input['ResourceRdsPostgresIamArgs']]:
         return pulumi.get(self, "rds_postgres_iam")
 
     @rds_postgres_iam.setter
     def rds_postgres_iam(self, value: Optional[pulumi.Input['ResourceRdsPostgresIamArgs']]):
         pulumi.set(self, "rds_postgres_iam", value)
@@ -1103,14 +1115,15 @@
                  neptune_iam: Optional[pulumi.Input['ResourceNeptuneIamArgs']] = None,
                  oracle: Optional[pulumi.Input['ResourceOracleArgs']] = None,
                  postgres: Optional[pulumi.Input['ResourcePostgresArgs']] = None,
                  presto: Optional[pulumi.Input['ResourcePrestoArgs']] = None,
                  rabbitmq_amqp091: Optional[pulumi.Input['ResourceRabbitmqAmqp091Args']] = None,
                  raw_tcp: Optional[pulumi.Input['ResourceRawTcpArgs']] = None,
                  rdp: Optional[pulumi.Input['ResourceRdpArgs']] = None,
+                 rdp_cert: Optional[pulumi.Input['ResourceRdpCertArgs']] = None,
                  rds_postgres_iam: Optional[pulumi.Input['ResourceRdsPostgresIamArgs']] = None,
                  redis: Optional[pulumi.Input['ResourceRedisArgs']] = None,
                  redshift: Optional[pulumi.Input['ResourceRedshiftArgs']] = None,
                  single_store: Optional[pulumi.Input['ResourceSingleStoreArgs']] = None,
                  snowflake: Optional[pulumi.Input['ResourceSnowflakeArgs']] = None,
                  snowsight: Optional[pulumi.Input['ResourceSnowsightArgs']] = None,
                  sql_server: Optional[pulumi.Input['ResourceSqlServerArgs']] = None,
@@ -1261,14 +1274,16 @@
             pulumi.set(__self__, "presto", presto)
         if rabbitmq_amqp091 is not None:
             pulumi.set(__self__, "rabbitmq_amqp091", rabbitmq_amqp091)
         if raw_tcp is not None:
             pulumi.set(__self__, "raw_tcp", raw_tcp)
         if rdp is not None:
             pulumi.set(__self__, "rdp", rdp)
+        if rdp_cert is not None:
+            pulumi.set(__self__, "rdp_cert", rdp_cert)
         if rds_postgres_iam is not None:
             pulumi.set(__self__, "rds_postgres_iam", rds_postgres_iam)
         if redis is not None:
             pulumi.set(__self__, "redis", redis)
         if redshift is not None:
             pulumi.set(__self__, "redshift", redshift)
         if single_store is not None:
@@ -1910,14 +1925,23 @@
         return pulumi.get(self, "rdp")
 
     @rdp.setter
     def rdp(self, value: Optional[pulumi.Input['ResourceRdpArgs']]):
         pulumi.set(self, "rdp", value)
 
     @property
+    @pulumi.getter(name="rdpCert")
+    def rdp_cert(self) -> Optional[pulumi.Input['ResourceRdpCertArgs']]:
+        return pulumi.get(self, "rdp_cert")
+
+    @rdp_cert.setter
+    def rdp_cert(self, value: Optional[pulumi.Input['ResourceRdpCertArgs']]):
+        pulumi.set(self, "rdp_cert", value)
+
+    @property
     @pulumi.getter(name="rdsPostgresIam")
     def rds_postgres_iam(self) -> Optional[pulumi.Input['ResourceRdsPostgresIamArgs']]:
         return pulumi.get(self, "rds_postgres_iam")
 
     @rds_postgres_iam.setter
     def rds_postgres_iam(self, value: Optional[pulumi.Input['ResourceRdsPostgresIamArgs']]):
         pulumi.set(self, "rds_postgres_iam", value)
@@ -2129,14 +2153,15 @@
                  neptune_iam: Optional[pulumi.Input[pulumi.InputType['ResourceNeptuneIamArgs']]] = None,
                  oracle: Optional[pulumi.Input[pulumi.InputType['ResourceOracleArgs']]] = None,
                  postgres: Optional[pulumi.Input[pulumi.InputType['ResourcePostgresArgs']]] = None,
                  presto: Optional[pulumi.Input[pulumi.InputType['ResourcePrestoArgs']]] = None,
                  rabbitmq_amqp091: Optional[pulumi.Input[pulumi.InputType['ResourceRabbitmqAmqp091Args']]] = None,
                  raw_tcp: Optional[pulumi.Input[pulumi.InputType['ResourceRawTcpArgs']]] = None,
                  rdp: Optional[pulumi.Input[pulumi.InputType['ResourceRdpArgs']]] = None,
+                 rdp_cert: Optional[pulumi.Input[pulumi.InputType['ResourceRdpCertArgs']]] = None,
                  rds_postgres_iam: Optional[pulumi.Input[pulumi.InputType['ResourceRdsPostgresIamArgs']]] = None,
                  redis: Optional[pulumi.Input[pulumi.InputType['ResourceRedisArgs']]] = None,
                  redshift: Optional[pulumi.Input[pulumi.InputType['ResourceRedshiftArgs']]] = None,
                  single_store: Optional[pulumi.Input[pulumi.InputType['ResourceSingleStoreArgs']]] = None,
                  snowflake: Optional[pulumi.Input[pulumi.InputType['ResourceSnowflakeArgs']]] = None,
                  snowsight: Optional[pulumi.Input[pulumi.InputType['ResourceSnowsightArgs']]] = None,
                  sql_server: Optional[pulumi.Input[pulumi.InputType['ResourceSqlServerArgs']]] = None,
@@ -2152,15 +2177,15 @@
                  __props__=None):
         """
         ## Import
 
         A Resource can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/resource:Resource example rs-12345678
+        $ pulumi import sdm:index/resource:Resource example rs-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ResourceMongoHostArgs']] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoReplicaSetArgs']] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoShardedClusterArgs']] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
@@ -2175,15 +2200,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
         A Resource can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/resource:Resource example rs-12345678
+        $ pulumi import sdm:index/resource:Resource example rs-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param ResourceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -2260,14 +2285,15 @@
                  neptune_iam: Optional[pulumi.Input[pulumi.InputType['ResourceNeptuneIamArgs']]] = None,
                  oracle: Optional[pulumi.Input[pulumi.InputType['ResourceOracleArgs']]] = None,
                  postgres: Optional[pulumi.Input[pulumi.InputType['ResourcePostgresArgs']]] = None,
                  presto: Optional[pulumi.Input[pulumi.InputType['ResourcePrestoArgs']]] = None,
                  rabbitmq_amqp091: Optional[pulumi.Input[pulumi.InputType['ResourceRabbitmqAmqp091Args']]] = None,
                  raw_tcp: Optional[pulumi.Input[pulumi.InputType['ResourceRawTcpArgs']]] = None,
                  rdp: Optional[pulumi.Input[pulumi.InputType['ResourceRdpArgs']]] = None,
+                 rdp_cert: Optional[pulumi.Input[pulumi.InputType['ResourceRdpCertArgs']]] = None,
                  rds_postgres_iam: Optional[pulumi.Input[pulumi.InputType['ResourceRdsPostgresIamArgs']]] = None,
                  redis: Optional[pulumi.Input[pulumi.InputType['ResourceRedisArgs']]] = None,
                  redshift: Optional[pulumi.Input[pulumi.InputType['ResourceRedshiftArgs']]] = None,
                  single_store: Optional[pulumi.Input[pulumi.InputType['ResourceSingleStoreArgs']]] = None,
                  snowflake: Optional[pulumi.Input[pulumi.InputType['ResourceSnowflakeArgs']]] = None,
                  snowsight: Optional[pulumi.Input[pulumi.InputType['ResourceSnowsightArgs']]] = None,
                  sql_server: Optional[pulumi.Input[pulumi.InputType['ResourceSqlServerArgs']]] = None,
@@ -2352,14 +2378,15 @@
             __props__.__dict__["neptune_iam"] = neptune_iam
             __props__.__dict__["oracle"] = oracle
             __props__.__dict__["postgres"] = postgres
             __props__.__dict__["presto"] = presto
             __props__.__dict__["rabbitmq_amqp091"] = rabbitmq_amqp091
             __props__.__dict__["raw_tcp"] = raw_tcp
             __props__.__dict__["rdp"] = rdp
+            __props__.__dict__["rdp_cert"] = rdp_cert
             __props__.__dict__["rds_postgres_iam"] = rds_postgres_iam
             __props__.__dict__["redis"] = redis
             __props__.__dict__["redshift"] = redshift
             __props__.__dict__["single_store"] = single_store
             __props__.__dict__["snowflake"] = snowflake
             __props__.__dict__["snowsight"] = snowsight
             __props__.__dict__["sql_server"] = sql_server
@@ -2445,14 +2472,15 @@
             neptune_iam: Optional[pulumi.Input[pulumi.InputType['ResourceNeptuneIamArgs']]] = None,
             oracle: Optional[pulumi.Input[pulumi.InputType['ResourceOracleArgs']]] = None,
             postgres: Optional[pulumi.Input[pulumi.InputType['ResourcePostgresArgs']]] = None,
             presto: Optional[pulumi.Input[pulumi.InputType['ResourcePrestoArgs']]] = None,
             rabbitmq_amqp091: Optional[pulumi.Input[pulumi.InputType['ResourceRabbitmqAmqp091Args']]] = None,
             raw_tcp: Optional[pulumi.Input[pulumi.InputType['ResourceRawTcpArgs']]] = None,
             rdp: Optional[pulumi.Input[pulumi.InputType['ResourceRdpArgs']]] = None,
+            rdp_cert: Optional[pulumi.Input[pulumi.InputType['ResourceRdpCertArgs']]] = None,
             rds_postgres_iam: Optional[pulumi.Input[pulumi.InputType['ResourceRdsPostgresIamArgs']]] = None,
             redis: Optional[pulumi.Input[pulumi.InputType['ResourceRedisArgs']]] = None,
             redshift: Optional[pulumi.Input[pulumi.InputType['ResourceRedshiftArgs']]] = None,
             single_store: Optional[pulumi.Input[pulumi.InputType['ResourceSingleStoreArgs']]] = None,
             snowflake: Optional[pulumi.Input[pulumi.InputType['ResourceSnowflakeArgs']]] = None,
             snowsight: Optional[pulumi.Input[pulumi.InputType['ResourceSnowsightArgs']]] = None,
             sql_server: Optional[pulumi.Input[pulumi.InputType['ResourceSqlServerArgs']]] = None,
@@ -2545,14 +2573,15 @@
         __props__.__dict__["neptune_iam"] = neptune_iam
         __props__.__dict__["oracle"] = oracle
         __props__.__dict__["postgres"] = postgres
         __props__.__dict__["presto"] = presto
         __props__.__dict__["rabbitmq_amqp091"] = rabbitmq_amqp091
         __props__.__dict__["raw_tcp"] = raw_tcp
         __props__.__dict__["rdp"] = rdp
+        __props__.__dict__["rdp_cert"] = rdp_cert
         __props__.__dict__["rds_postgres_iam"] = rds_postgres_iam
         __props__.__dict__["redis"] = redis
         __props__.__dict__["redshift"] = redshift
         __props__.__dict__["single_store"] = single_store
         __props__.__dict__["snowflake"] = snowflake
         __props__.__dict__["snowsight"] = snowsight
         __props__.__dict__["sql_server"] = sql_server
@@ -2911,14 +2940,19 @@
 
     @property
     @pulumi.getter
     def rdp(self) -> pulumi.Output[Optional['outputs.ResourceRdp']]:
         return pulumi.get(self, "rdp")
 
     @property
+    @pulumi.getter(name="rdpCert")
+    def rdp_cert(self) -> pulumi.Output[Optional['outputs.ResourceRdpCert']]:
+        return pulumi.get(self, "rdp_cert")
+
+    @property
     @pulumi.getter(name="rdsPostgresIam")
     def rds_postgres_iam(self) -> pulumi.Output[Optional['outputs.ResourceRdsPostgresIam']]:
         return pulumi.get(self, "rds_postgres_iam")
 
     @property
     @pulumi.getter
     def redis(self) -> pulumi.Output[Optional['outputs.ResourceRedis']]:
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/role.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
                  __props__=None):
         """
         A Role has a list of access rules which determine which Resources the members
          of the Role have access to. An Account can be a member of multiple Roles via
          AccountAttachments.
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pierskarsenbarg_pulumi_sdm as sdm
 
         engineers = sdm.Role("engineers", tags={
             "foo": "bar",
@@ -176,22 +177,23 @@
                 },
             },
             {
                 "ids": ["rs-093e6f3061eb4dad"],
             },
         ]))
         ```
+        <!--End PulumiCodeChooser -->
         This resource can be imported using the import command.
 
         ## Import
 
         A Role can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/role:Role example r-12345678
+        $ pulumi import sdm:index/role:Role example r-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_rules: AccessRules is a list of access rules defining the resources this Role has access to.
         :param pulumi.Input[str] name: Unique human-readable name of the Role.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
@@ -204,14 +206,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         A Role has a list of access rules which determine which Resources the members
          of the Role have access to. An Account can be a member of multiple Roles via
          AccountAttachments.
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pierskarsenbarg_pulumi_sdm as sdm
 
         engineers = sdm.Role("engineers", tags={
             "foo": "bar",
@@ -230,22 +233,23 @@
                 },
             },
             {
                 "ids": ["rs-093e6f3061eb4dad"],
             },
         ]))
         ```
+        <!--End PulumiCodeChooser -->
         This resource can be imported using the import command.
 
         ## Import
 
         A Role can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/role:Role example r-12345678
+        $ pulumi import sdm:index/role:Role example r-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param RoleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/workflow.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,30 +11,34 @@
 
 __all__ = ['WorkflowArgs', 'Workflow']
 
 @pulumi.input_type
 class WorkflowArgs:
     def __init__(__self__, *,
                  access_rules: Optional[pulumi.Input[str]] = None,
+                 approval_flow_id: Optional[pulumi.Input[str]] = None,
                  auto_grant: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a Workflow resource.
         :param pulumi.Input[str] access_rules: AccessRules is a list of access rules defining the resources this Workflow provides access to.
+        :param pulumi.Input[str] approval_flow_id: Optional approval flow ID identifies an approval flow that linked to the workflow
         :param pulumi.Input[bool] auto_grant: Optional auto grant setting to automatically approve requests or not, defaults to false.
         :param pulumi.Input[str] description: Optional description of the Workflow.
         :param pulumi.Input[bool] enabled: Optional enabled state for workflow. This setting may be overridden by the system if the workflow doesn't meet the requirements to be enabled or if other conditions prevent enabling the workflow. The requirements to enable a workflow are that the workflow must be either set up for with auto grant enabled or have one or more WorkflowApprovers created for the workflow.
         :param pulumi.Input[str] name: Unique human-readable name of the Workflow.
         :param pulumi.Input[int] weight: Optional weight for workflow to specify it's priority in matching a request.
         """
         if access_rules is not None:
             pulumi.set(__self__, "access_rules", access_rules)
+        if approval_flow_id is not None:
+            pulumi.set(__self__, "approval_flow_id", approval_flow_id)
         if auto_grant is not None:
             pulumi.set(__self__, "auto_grant", auto_grant)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if name is not None:
@@ -51,14 +55,26 @@
         return pulumi.get(self, "access_rules")
 
     @access_rules.setter
     def access_rules(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_rules", value)
 
     @property
+    @pulumi.getter(name="approvalFlowId")
+    def approval_flow_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Optional approval flow ID identifies an approval flow that linked to the workflow
+        """
+        return pulumi.get(self, "approval_flow_id")
+
+    @approval_flow_id.setter
+    def approval_flow_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "approval_flow_id", value)
+
+    @property
     @pulumi.getter(name="autoGrant")
     def auto_grant(self) -> Optional[pulumi.Input[bool]]:
         """
         Optional auto grant setting to automatically approve requests or not, defaults to false.
         """
         return pulumi.get(self, "auto_grant")
 
@@ -115,30 +131,34 @@
         pulumi.set(self, "weight", value)
 
 
 @pulumi.input_type
 class _WorkflowState:
     def __init__(__self__, *,
                  access_rules: Optional[pulumi.Input[str]] = None,
+                 approval_flow_id: Optional[pulumi.Input[str]] = None,
                  auto_grant: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering Workflow resources.
         :param pulumi.Input[str] access_rules: AccessRules is a list of access rules defining the resources this Workflow provides access to.
+        :param pulumi.Input[str] approval_flow_id: Optional approval flow ID identifies an approval flow that linked to the workflow
         :param pulumi.Input[bool] auto_grant: Optional auto grant setting to automatically approve requests or not, defaults to false.
         :param pulumi.Input[str] description: Optional description of the Workflow.
         :param pulumi.Input[bool] enabled: Optional enabled state for workflow. This setting may be overridden by the system if the workflow doesn't meet the requirements to be enabled or if other conditions prevent enabling the workflow. The requirements to enable a workflow are that the workflow must be either set up for with auto grant enabled or have one or more WorkflowApprovers created for the workflow.
         :param pulumi.Input[str] name: Unique human-readable name of the Workflow.
         :param pulumi.Input[int] weight: Optional weight for workflow to specify it's priority in matching a request.
         """
         if access_rules is not None:
             pulumi.set(__self__, "access_rules", access_rules)
+        if approval_flow_id is not None:
+            pulumi.set(__self__, "approval_flow_id", approval_flow_id)
         if auto_grant is not None:
             pulumi.set(__self__, "auto_grant", auto_grant)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if name is not None:
@@ -155,14 +175,26 @@
         return pulumi.get(self, "access_rules")
 
     @access_rules.setter
     def access_rules(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_rules", value)
 
     @property
+    @pulumi.getter(name="approvalFlowId")
+    def approval_flow_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Optional approval flow ID identifies an approval flow that linked to the workflow
+        """
+        return pulumi.get(self, "approval_flow_id")
+
+    @approval_flow_id.setter
+    def approval_flow_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "approval_flow_id", value)
+
+    @property
     @pulumi.getter(name="autoGrant")
     def auto_grant(self) -> Optional[pulumi.Input[bool]]:
         """
         Optional auto grant setting to automatically approve requests or not, defaults to false.
         """
         return pulumi.get(self, "auto_grant")
 
@@ -221,26 +253,28 @@
 
 class Workflow(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_rules: Optional[pulumi.Input[str]] = None,
+                 approval_flow_id: Optional[pulumi.Input[str]] = None,
                  auto_grant: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Workflows are the collection of rules that define the resources to which access can be requested,
          the users that can request that access, and the mechanism for approving those requests which can either
          but automatic approval or a set of users authorized to approve the requests.
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pierskarsenbarg_pulumi_sdm as sdm
 
         auto_grant_workflow = sdm.Workflow("autoGrantWorkflow",
             auto_grant=True,
@@ -256,27 +290,29 @@
             access_rules=json.dumps([{
                 "type": "redis",
                 "tags": {
                     "region": "us-east",
                 },
             }]))
         ```
+        <!--End PulumiCodeChooser -->
         This resource can be imported using the import command.
 
         ## Import
 
         A Workflow can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/workflow:Workflow example aw-12345678
+        $ pulumi import sdm:index/workflow:Workflow example aw-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_rules: AccessRules is a list of access rules defining the resources this Workflow provides access to.
+        :param pulumi.Input[str] approval_flow_id: Optional approval flow ID identifies an approval flow that linked to the workflow
         :param pulumi.Input[bool] auto_grant: Optional auto grant setting to automatically approve requests or not, defaults to false.
         :param pulumi.Input[str] description: Optional description of the Workflow.
         :param pulumi.Input[bool] enabled: Optional enabled state for workflow. This setting may be overridden by the system if the workflow doesn't meet the requirements to be enabled or if other conditions prevent enabling the workflow. The requirements to enable a workflow are that the workflow must be either set up for with auto grant enabled or have one or more WorkflowApprovers created for the workflow.
         :param pulumi.Input[str] name: Unique human-readable name of the Workflow.
         :param pulumi.Input[int] weight: Optional weight for workflow to specify it's priority in matching a request.
         """
         ...
@@ -287,14 +323,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Workflows are the collection of rules that define the resources to which access can be requested,
          the users that can request that access, and the mechanism for approving those requests which can either
          but automatic approval or a set of users authorized to approve the requests.
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pierskarsenbarg_pulumi_sdm as sdm
 
         auto_grant_workflow = sdm.Workflow("autoGrantWorkflow",
             auto_grant=True,
@@ -310,22 +347,23 @@
             access_rules=json.dumps([{
                 "type": "redis",
                 "tags": {
                     "region": "us-east",
                 },
             }]))
         ```
+        <!--End PulumiCodeChooser -->
         This resource can be imported using the import command.
 
         ## Import
 
         A Workflow can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/workflow:Workflow example aw-12345678
+        $ pulumi import sdm:index/workflow:Workflow example aw-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param WorkflowArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -336,14 +374,15 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_rules: Optional[pulumi.Input[str]] = None,
+                 approval_flow_id: Optional[pulumi.Input[str]] = None,
                  auto_grant: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
@@ -351,14 +390,15 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = WorkflowArgs.__new__(WorkflowArgs)
 
             __props__.__dict__["access_rules"] = access_rules
+            __props__.__dict__["approval_flow_id"] = approval_flow_id
             __props__.__dict__["auto_grant"] = auto_grant
             __props__.__dict__["description"] = description
             __props__.__dict__["enabled"] = enabled
             __props__.__dict__["name"] = name
             __props__.__dict__["weight"] = weight
         super(Workflow, __self__).__init__(
             'sdm:index/workflow:Workflow',
@@ -367,38 +407,41 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             access_rules: Optional[pulumi.Input[str]] = None,
+            approval_flow_id: Optional[pulumi.Input[str]] = None,
             auto_grant: Optional[pulumi.Input[bool]] = None,
             description: Optional[pulumi.Input[str]] = None,
             enabled: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
             weight: Optional[pulumi.Input[int]] = None) -> 'Workflow':
         """
         Get an existing Workflow resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_rules: AccessRules is a list of access rules defining the resources this Workflow provides access to.
+        :param pulumi.Input[str] approval_flow_id: Optional approval flow ID identifies an approval flow that linked to the workflow
         :param pulumi.Input[bool] auto_grant: Optional auto grant setting to automatically approve requests or not, defaults to false.
         :param pulumi.Input[str] description: Optional description of the Workflow.
         :param pulumi.Input[bool] enabled: Optional enabled state for workflow. This setting may be overridden by the system if the workflow doesn't meet the requirements to be enabled or if other conditions prevent enabling the workflow. The requirements to enable a workflow are that the workflow must be either set up for with auto grant enabled or have one or more WorkflowApprovers created for the workflow.
         :param pulumi.Input[str] name: Unique human-readable name of the Workflow.
         :param pulumi.Input[int] weight: Optional weight for workflow to specify it's priority in matching a request.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _WorkflowState.__new__(_WorkflowState)
 
         __props__.__dict__["access_rules"] = access_rules
+        __props__.__dict__["approval_flow_id"] = approval_flow_id
         __props__.__dict__["auto_grant"] = auto_grant
         __props__.__dict__["description"] = description
         __props__.__dict__["enabled"] = enabled
         __props__.__dict__["name"] = name
         __props__.__dict__["weight"] = weight
         return Workflow(resource_name, opts=opts, __props__=__props__)
 
@@ -407,14 +450,22 @@
     def access_rules(self) -> pulumi.Output[str]:
         """
         AccessRules is a list of access rules defining the resources this Workflow provides access to.
         """
         return pulumi.get(self, "access_rules")
 
     @property
+    @pulumi.getter(name="approvalFlowId")
+    def approval_flow_id(self) -> pulumi.Output[Optional[str]]:
+        """
+        Optional approval flow ID identifies an approval flow that linked to the workflow
+        """
+        return pulumi.get(self, "approval_flow_id")
+
+    @property
     @pulumi.getter(name="autoGrant")
     def auto_grant(self) -> pulumi.Output[Optional[bool]]:
         """
         Optional auto grant setting to automatically approve requests or not, defaults to false.
         """
         return pulumi.get(self, "auto_grant")
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/workflow_approver.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/get_approval_workflow_approver.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,229 +4,199 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
 
-__all__ = ['WorkflowApproverArgs', 'WorkflowApprover']
-
-@pulumi.input_type
-class WorkflowApproverArgs:
-    def __init__(__self__, *,
-                 approver_id: pulumi.Input[str],
-                 workflow_id: pulumi.Input[str]):
-        """
-        The set of arguments for constructing a WorkflowApprover resource.
-        :param pulumi.Input[str] approver_id: The approver id.
-        :param pulumi.Input[str] workflow_id: The workflow id.
-        """
-        pulumi.set(__self__, "approver_id", approver_id)
-        pulumi.set(__self__, "workflow_id", workflow_id)
-
-    @property
-    @pulumi.getter(name="approverId")
-    def approver_id(self) -> pulumi.Input[str]:
-        """
-        The approver id.
-        """
-        return pulumi.get(self, "approver_id")
-
-    @approver_id.setter
-    def approver_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "approver_id", value)
-
-    @property
-    @pulumi.getter(name="workflowId")
-    def workflow_id(self) -> pulumi.Input[str]:
-        """
-        The workflow id.
-        """
-        return pulumi.get(self, "workflow_id")
-
-    @workflow_id.setter
-    def workflow_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "workflow_id", value)
-
-
-@pulumi.input_type
-class _WorkflowApproverState:
-    def __init__(__self__, *,
-                 approver_id: Optional[pulumi.Input[str]] = None,
-                 workflow_id: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering WorkflowApprover resources.
-        :param pulumi.Input[str] approver_id: The approver id.
-        :param pulumi.Input[str] workflow_id: The workflow id.
-        """
-        if approver_id is not None:
-            pulumi.set(__self__, "approver_id", approver_id)
-        if workflow_id is not None:
-            pulumi.set(__self__, "workflow_id", workflow_id)
-
-    @property
-    @pulumi.getter(name="approverId")
-    def approver_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        The approver id.
-        """
-        return pulumi.get(self, "approver_id")
-
-    @approver_id.setter
-    def approver_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "approver_id", value)
-
-    @property
-    @pulumi.getter(name="workflowId")
-    def workflow_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        The workflow id.
-        """
-        return pulumi.get(self, "workflow_id")
-
-    @workflow_id.setter
-    def workflow_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "workflow_id", value)
-
-
-class WorkflowApprover(pulumi.CustomResource):
-    @overload
-    def __init__(__self__,
-                 resource_name: str,
-                 opts: Optional[pulumi.ResourceOptions] = None,
-                 approver_id: Optional[pulumi.Input[str]] = None,
-                 workflow_id: Optional[pulumi.Input[str]] = None,
-                 __props__=None):
-        """
-        WorkflowApprover is an account with the ability to approve requests bound to a workflow.
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pierskarsenbarg_pulumi_sdm as sdm
-
-        workflow_approver_example = sdm.WorkflowApprover("workflowApproverExample",
-            approver_id="a-234605",
-            workflow_id="aw-6799234")
-        ```
-        This resource can be imported using the import command.
-
-        ## Import
-
-        A WorkflowApprover can be imported using the id, e.g.,
-
-        ```sh
-         $ pulumi import sdm:index/workflowApprover:WorkflowApprover example nt-12345678
-        ```
-
-        :param str resource_name: The name of the resource.
-        :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] approver_id: The approver id.
-        :param pulumi.Input[str] workflow_id: The workflow id.
-        """
-        ...
-    @overload
-    def __init__(__self__,
-                 resource_name: str,
-                 args: WorkflowApproverArgs,
-                 opts: Optional[pulumi.ResourceOptions] = None):
-        """
-        WorkflowApprover is an account with the ability to approve requests bound to a workflow.
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pierskarsenbarg_pulumi_sdm as sdm
-
-        workflow_approver_example = sdm.WorkflowApprover("workflowApproverExample",
-            approver_id="a-234605",
-            workflow_id="aw-6799234")
-        ```
-        This resource can be imported using the import command.
-
-        ## Import
-
-        A WorkflowApprover can be imported using the id, e.g.,
-
-        ```sh
-         $ pulumi import sdm:index/workflowApprover:WorkflowApprover example nt-12345678
-        ```
-
-        :param str resource_name: The name of the resource.
-        :param WorkflowApproverArgs args: The arguments to use to populate this resource's properties.
-        :param pulumi.ResourceOptions opts: Options for the resource.
-        """
-        ...
-    def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(WorkflowApproverArgs, pulumi.ResourceOptions, *args, **kwargs)
-        if resource_args is not None:
-            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
-        else:
-            __self__._internal_init(resource_name, *args, **kwargs)
-
-    def _internal_init(__self__,
-                 resource_name: str,
-                 opts: Optional[pulumi.ResourceOptions] = None,
-                 approver_id: Optional[pulumi.Input[str]] = None,
-                 workflow_id: Optional[pulumi.Input[str]] = None,
-                 __props__=None):
-        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
-        if not isinstance(opts, pulumi.ResourceOptions):
-            raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.id is None:
-            if __props__ is not None:
-                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = WorkflowApproverArgs.__new__(WorkflowApproverArgs)
-
-            if approver_id is None and not opts.urn:
-                raise TypeError("Missing required property 'approver_id'")
-            __props__.__dict__["approver_id"] = approver_id
-            if workflow_id is None and not opts.urn:
-                raise TypeError("Missing required property 'workflow_id'")
-            __props__.__dict__["workflow_id"] = workflow_id
-        super(WorkflowApprover, __self__).__init__(
-            'sdm:index/workflowApprover:WorkflowApprover',
-            resource_name,
-            __props__,
-            opts)
-
-    @staticmethod
-    def get(resource_name: str,
-            id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None,
-            approver_id: Optional[pulumi.Input[str]] = None,
-            workflow_id: Optional[pulumi.Input[str]] = None) -> 'WorkflowApprover':
-        """
-        Get an existing WorkflowApprover resource's state with the given name, id, and optional extra
-        properties used to qualify the lookup.
-
-        :param str resource_name: The unique name of the resulting resource.
-        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
-        :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] approver_id: The approver id.
-        :param pulumi.Input[str] workflow_id: The workflow id.
-        """
-        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
-
-        __props__ = _WorkflowApproverState.__new__(_WorkflowApproverState)
-
-        __props__.__dict__["approver_id"] = approver_id
-        __props__.__dict__["workflow_id"] = workflow_id
-        return WorkflowApprover(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter(name="approverId")
-    def approver_id(self) -> pulumi.Output[str]:
-        """
-        The approver id.
-        """
-        return pulumi.get(self, "approver_id")
-
-    @property
-    @pulumi.getter(name="workflowId")
-    def workflow_id(self) -> pulumi.Output[str]:
-        """
-        The workflow id.
-        """
-        return pulumi.get(self, "workflow_id")
-
+__all__ = [
+    'GetApprovalWorkflowApproverResult',
+    'AwaitableGetApprovalWorkflowApproverResult',
+    'get_approval_workflow_approver',
+    'get_approval_workflow_approver_output',
+]
+
+@pulumi.output_type
+class GetApprovalWorkflowApproverResult:
+    """
+    A collection of values returned by getApprovalWorkflowApprover.
+    """
+    def __init__(__self__, account_id=None, approval_flow_id=None, approval_step_id=None, approval_workflow_approvers=None, id=None, ids=None, role_id=None):
+        if account_id and not isinstance(account_id, str):
+            raise TypeError("Expected argument 'account_id' to be a str")
+        pulumi.set(__self__, "account_id", account_id)
+        if approval_flow_id and not isinstance(approval_flow_id, str):
+            raise TypeError("Expected argument 'approval_flow_id' to be a str")
+        pulumi.set(__self__, "approval_flow_id", approval_flow_id)
+        if approval_step_id and not isinstance(approval_step_id, str):
+            raise TypeError("Expected argument 'approval_step_id' to be a str")
+        pulumi.set(__self__, "approval_step_id", approval_step_id)
+        if approval_workflow_approvers and not isinstance(approval_workflow_approvers, list):
+            raise TypeError("Expected argument 'approval_workflow_approvers' to be a list")
+        pulumi.set(__self__, "approval_workflow_approvers", approval_workflow_approvers)
+        if id and not isinstance(id, str):
+            raise TypeError("Expected argument 'id' to be a str")
+        pulumi.set(__self__, "id", id)
+        if ids and not isinstance(ids, list):
+            raise TypeError("Expected argument 'ids' to be a list")
+        pulumi.set(__self__, "ids", ids)
+        if role_id and not isinstance(role_id, str):
+            raise TypeError("Expected argument 'role_id' to be a str")
+        pulumi.set(__self__, "role_id", role_id)
+
+    @property
+    @pulumi.getter(name="accountId")
+    def account_id(self) -> Optional[str]:
+        """
+        The approver account id.
+        """
+        return pulumi.get(self, "account_id")
+
+    @property
+    @pulumi.getter(name="approvalFlowId")
+    def approval_flow_id(self) -> Optional[str]:
+        """
+        The approval flow id specified the approval workflow that this approver belongs to
+        """
+        return pulumi.get(self, "approval_flow_id")
+
+    @property
+    @pulumi.getter(name="approvalStepId")
+    def approval_step_id(self) -> Optional[str]:
+        """
+        The approval step id specified the approval flow step that this approver belongs to
+        """
+        return pulumi.get(self, "approval_step_id")
+
+    @property
+    @pulumi.getter(name="approvalWorkflowApprovers")
+    def approval_workflow_approvers(self) -> Sequence['outputs.GetApprovalWorkflowApproverApprovalWorkflowApproverResult']:
+        """
+        A list where each element has the following attributes:
+        """
+        return pulumi.get(self, "approval_workflow_approvers")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the ApprovalWorkflowApprover.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def ids(self) -> Sequence[str]:
+        """
+        a list of strings of ids of data sources that match the given arguments.
+        """
+        return pulumi.get(self, "ids")
+
+    @property
+    @pulumi.getter(name="roleId")
+    def role_id(self) -> Optional[str]:
+        """
+        The approver role id
+        """
+        return pulumi.get(self, "role_id")
+
+
+class AwaitableGetApprovalWorkflowApproverResult(GetApprovalWorkflowApproverResult):
+    # pylint: disable=using-constant-test
+    def __await__(self):
+        if False:
+            yield self
+        return GetApprovalWorkflowApproverResult(
+            account_id=self.account_id,
+            approval_flow_id=self.approval_flow_id,
+            approval_step_id=self.approval_step_id,
+            approval_workflow_approvers=self.approval_workflow_approvers,
+            id=self.id,
+            ids=self.ids,
+            role_id=self.role_id)
+
+
+def get_approval_workflow_approver(account_id: Optional[str] = None,
+                                   approval_flow_id: Optional[str] = None,
+                                   approval_step_id: Optional[str] = None,
+                                   id: Optional[str] = None,
+                                   role_id: Optional[str] = None,
+                                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetApprovalWorkflowApproverResult:
+    """
+    ApprovalWorkflowApprover links an approval workflow approver to an ApprovalWorkflowStep
+    ## Example Usage
+
+    <!--Start PulumiCodeChooser -->
+    ```python
+    import pulumi
+    import pulumi_sdm as sdm
+
+    approval_workflow_approver_account_query = sdm.get_approval_workflow_approver(account_id="a-234605",
+        approval_flow_id="af-6799234",
+        approval_step_id="afs-2956266")
+    approval_workflow_approver_role_query = sdm.get_approval_workflow_approver(approval_flow_id="af-1935694",
+        approval_step_id="afs-9245942",
+        role_id="r-542982")
+    ```
+    <!--End PulumiCodeChooser -->
+
+
+    :param str account_id: The approver account id.
+    :param str approval_flow_id: The approval flow id specified the approval workflow that this approver belongs to
+    :param str approval_step_id: The approval step id specified the approval flow step that this approver belongs to
+    :param str id: Unique identifier of the ApprovalWorkflowApprover.
+    :param str role_id: The approver role id
+    """
+    __args__ = dict()
+    __args__['accountId'] = account_id
+    __args__['approvalFlowId'] = approval_flow_id
+    __args__['approvalStepId'] = approval_step_id
+    __args__['id'] = id
+    __args__['roleId'] = role_id
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
+    __ret__ = pulumi.runtime.invoke('sdm:index/getApprovalWorkflowApprover:getApprovalWorkflowApprover', __args__, opts=opts, typ=GetApprovalWorkflowApproverResult).value
+
+    return AwaitableGetApprovalWorkflowApproverResult(
+        account_id=pulumi.get(__ret__, 'account_id'),
+        approval_flow_id=pulumi.get(__ret__, 'approval_flow_id'),
+        approval_step_id=pulumi.get(__ret__, 'approval_step_id'),
+        approval_workflow_approvers=pulumi.get(__ret__, 'approval_workflow_approvers'),
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'),
+        role_id=pulumi.get(__ret__, 'role_id'))
+
+
+@_utilities.lift_output_func(get_approval_workflow_approver)
+def get_approval_workflow_approver_output(account_id: Optional[pulumi.Input[Optional[str]]] = None,
+                                          approval_flow_id: Optional[pulumi.Input[Optional[str]]] = None,
+                                          approval_step_id: Optional[pulumi.Input[Optional[str]]] = None,
+                                          id: Optional[pulumi.Input[Optional[str]]] = None,
+                                          role_id: Optional[pulumi.Input[Optional[str]]] = None,
+                                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetApprovalWorkflowApproverResult]:
+    """
+    ApprovalWorkflowApprover links an approval workflow approver to an ApprovalWorkflowStep
+    ## Example Usage
+
+    <!--Start PulumiCodeChooser -->
+    ```python
+    import pulumi
+    import pulumi_sdm as sdm
+
+    approval_workflow_approver_account_query = sdm.get_approval_workflow_approver(account_id="a-234605",
+        approval_flow_id="af-6799234",
+        approval_step_id="afs-2956266")
+    approval_workflow_approver_role_query = sdm.get_approval_workflow_approver(approval_flow_id="af-1935694",
+        approval_step_id="afs-9245942",
+        role_id="r-542982")
+    ```
+    <!--End PulumiCodeChooser -->
+
+
+    :param str account_id: The approver account id.
+    :param str approval_flow_id: The approval flow id specified the approval workflow that this approver belongs to
+    :param str approval_step_id: The approval step id specified the approval flow step that this approver belongs to
+    :param str id: Unique identifier of the ApprovalWorkflowApprover.
+    :param str role_id: The approver role id
+    """
+    ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm/workflow_role.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm/workflow_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,30 +98,32 @@
                  workflow_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         WorkflowRole links a role to a workflow. The linked roles indicate which roles a user must be a part of
          to request access to a resource via the workflow.
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pierskarsenbarg_pulumi_sdm as sdm
 
         workflow_role_example = sdm.WorkflowRole("workflowRoleExample",
             role_id="r-243561",
             workflow_id="aw-343865")
         ```
+        <!--End PulumiCodeChooser -->
         This resource can be imported using the import command.
 
         ## Import
 
         A WorkflowRole can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/workflowRole:WorkflowRole example wr-12345678
+        $ pulumi import sdm:index/workflowRole:WorkflowRole example wr-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] role_id: The role id.
         :param pulumi.Input[str] workflow_id: The workflow id.
         """
@@ -132,30 +134,32 @@
                  args: WorkflowRoleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         WorkflowRole links a role to a workflow. The linked roles indicate which roles a user must be a part of
          to request access to a resource via the workflow.
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pierskarsenbarg_pulumi_sdm as sdm
 
         workflow_role_example = sdm.WorkflowRole("workflowRoleExample",
             role_id="r-243561",
             workflow_id="aw-343865")
         ```
+        <!--End PulumiCodeChooser -->
         This resource can be imported using the import command.
 
         ## Import
 
         A WorkflowRole can be imported using the id, e.g.,
 
         ```sh
-         $ pulumi import sdm:index/workflowRole:WorkflowRole example wr-12345678
+        $ pulumi import sdm:index/workflowRole:WorkflowRole example wr-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param WorkflowRoleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 Metadata-Version: 2.1
 Name: pierskarsenbarg-pulumi-sdm
-Version: 1.8.0
+Version: 1.9.0
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
-Description: # StrongDM Resource Provider
-        
-        The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
-        
-        ## Installing
-        
-        This package is available for several languages/platforms:
-        
-        ### Node.js (JavaScript/TypeScript)
-        
-        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-        
-        ```bash
-        npm install @pierskarsenbarg/sdm
-        ```
-        
-        or `yarn`:
-        
-        ```bash
-        yarn add @pierskarsenbarg/sdm
-        ```
-        
-        ### Python
-        
-        To use from Python, install using `pip`:
-        
-        ```bash
-        pip install pierskarsenbarg-pulumi-sdm
-        ```
-        
-        ### Go
-        
-        To use from Go, use `go get` to grab the latest version of the library:
-        
-        ```bash
-        go get github.com/pierskarsenbarg/pulumi-sdm/sdk/go/...
-        ```
-        
-        ### .NET
-        
-        To use from .NET, install using `dotnet add package`:
-        
-        ```bash
-        dotnet add package PiersKarsenbarg.Sdm
-        ```
-        
-        ## Configuration
-        
-        The following configuration points are available for the `sdm` provider:
-        
-        - `sdm:apiAccessKey` (environment: `SDM_API_ACCESS_KEY`) - the API key for `Strong DM`
-        - `sdm:apiSecretKey` (environment: `SDM_API_SECRET_KEY`) - the corresponding secret key for the above API key
-        
-        ## Todo
-        
-        * Add Java language support
-        * Add YAML language support
-        
-        <!-- ## Reference
-        
-        For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/). -->
-        
 Keywords: pulumi sdm category/cloud
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+# StrongDM Resource Provider
+
+The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
+
+## Installing
+
+This package is available for several languages/platforms:
+
+### Node.js (JavaScript/TypeScript)
+
+To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+
+```bash
+npm install @pierskarsenbarg/sdm
+```
+
+or `yarn`:
+
+```bash
+yarn add @pierskarsenbarg/sdm
+```
+
+### Python
+
+To use from Python, install using `pip`:
+
+```bash
+pip install pierskarsenbarg-pulumi-sdm
+```
+
+### Go
+
+To use from Go, use `go get` to grab the latest version of the library:
+
+```bash
+go get github.com/pierskarsenbarg/pulumi-sdm/sdk/go/...
+```
+
+### .NET
+
+To use from .NET, install using `dotnet add package`:
+
+```bash
+dotnet add package PiersKarsenbarg.Sdm
+```
+
+## Configuration
+
+The following configuration points are available for the `sdm` provider:
+
+- `sdm:apiAccessKey` (environment: `SDM_API_ACCESS_KEY`) - the API key for `Strong DM`
+- `sdm:apiSecretKey` (environment: `SDM_API_SECRET_KEY`) - the corresponding secret key for the above API key
+
+## Todo
+
+* Add Java language support
+* Add YAML language support
+
+<!-- ## Reference
+
+For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/). -->
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt` & `pierskarsenbarg_pulumi_sdm-1.9.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 README.md
 setup.py
 pierskarsenbarg_pulumi_sdm/__init__.py
 pierskarsenbarg_pulumi_sdm/_inputs.py
 pierskarsenbarg_pulumi_sdm/_utilities.py
 pierskarsenbarg_pulumi_sdm/account.py
 pierskarsenbarg_pulumi_sdm/account_attachment.py
+pierskarsenbarg_pulumi_sdm/approval_workflow.py
+pierskarsenbarg_pulumi_sdm/approval_workflow_approval.py
+pierskarsenbarg_pulumi_sdm/approval_workflow_step.py
 pierskarsenbarg_pulumi_sdm/get_account.py
 pierskarsenbarg_pulumi_sdm/get_account_attachment.py
+pierskarsenbarg_pulumi_sdm/get_approval_workflow.py
+pierskarsenbarg_pulumi_sdm/get_approval_workflow_approver.py
+pierskarsenbarg_pulumi_sdm/get_approval_workflow_step.py
 pierskarsenbarg_pulumi_sdm/get_node.py
 pierskarsenbarg_pulumi_sdm/get_peering_group.py
 pierskarsenbarg_pulumi_sdm/get_peering_group_node.py
 pierskarsenbarg_pulumi_sdm/get_peering_group_peer.py
 pierskarsenbarg_pulumi_sdm/get_peering_group_resource.py
 pierskarsenbarg_pulumi_sdm/get_remote_identity.py
 pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.8.0/setup.py` & `pierskarsenbarg_pulumi_sdm-1.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.8.0"
+VERSION = "1.9.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "sdm Pulumi Package - Development Version"
 
 
 setup(name='pierskarsenbarg_pulumi_sdm',
-      python_requires='>=3.7',
+      python_requires='>=3.8',
       version=VERSION,
       description="A Pulumi package for creating and managing StrongDM cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       keywords='pulumi sdm category/cloud',
       url='https://github.com/pierskarsenbarg/pulumi-sdm',
       project_urls={
```

