# Comparing `tmp/ccdexplorer_fundamentals-0.2.1.tar.gz` & `tmp/ccdexplorer_fundamentals-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdexplorer_fundamentals-0.2.1.tar", last modified: Fri Apr 19 14:05:17 2024, max compression
+gzip compressed data, was "ccdexplorer_fundamentals-0.2.2.tar", last modified: Sun Apr 28 07:49:41 2024, max compression
```

## Comparing `ccdexplorer_fundamentals-0.2.1.tar` & `ccdexplorer_fundamentals-0.2.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:17.540528 ccdexplorer_fundamentals-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-19 14:05:17.536528 ccdexplorer_fundamentals-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:17.524528 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:17.528528 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:17.528528 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/CCD_Types/
--rw-r--r--   0 runner    (1001) docker     (127)    38515 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/CCD_Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:17.528528 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/concordium/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/concordium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:17.528528 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/concordium/health/
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/concordium/health/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:17.528528 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/concordium/v2/
--rw-r--r--   0 runner    (1001) docker     (127)   190426 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/concordium/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/health_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/health_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/health_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:17.532528 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_CheckHealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11072 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountList.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetAnonymityRevokers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerEarliestWinTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerList.py
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockChainParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockPendingUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockSpecialEvents.py
--rw-r--r--   0 runner    (1001) docker     (127)    28792 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockTransactionEvents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlocksAtHeight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetConsensusInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetElectionInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetFinalizedBlocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetIdentityProviders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceList.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetModuleSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegationInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetTokenomicsInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_InvokeInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)    38653 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_SharedConverters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    99596 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)   131737 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)   198939 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/types_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/wadze.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:17.536528 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13652 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_accountByAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_bakerByBakerId.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_bakers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20427 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_blockByBlockHash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_passiveDelegation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_paydayStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForBakerPool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_rewardMetricsForAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_transactionByTransactionHash.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_transactionMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/exchange_account_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/ql_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    41243 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/cis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/cns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/env.py
--rw-r--r--   0 runner    (1001) docker     (127)    15657 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:17.536528 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb_queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb_queries/_apy_calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb_queries/_baker_distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb_queries/_search_transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15024 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb_queries/_store_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb_queries/_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/rewards.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/tooter.py
--rw-r--r--   0 runner    (1001) docker     (127)    46983 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/user_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:17.536528 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-19 14:05:17.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-19 14:05:17.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:05:17.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-19 14:05:17.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 14:05:17.000000 ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:05:17.540528 ccdexplorer_fundamentals-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:17.536528 ccdexplorer_fundamentals-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:13.000000 ccdexplorer_fundamentals-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:41.701074 ccdexplorer_fundamentals-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-28 07:49:41.701074 ccdexplorer_fundamentals-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:41.689074 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:41.693074 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:41.693074 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/CCD_Types/
+-rw-r--r--   0 runner    (1001) docker     (127)    38515 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/CCD_Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:41.693074 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/concordium/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/concordium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:41.693074 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/concordium/health/
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/concordium/health/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:41.693074 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/concordium/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)   190426 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/concordium/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/health_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/health_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/health_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:41.697074 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_CheckHealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11072 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetAnonymityRevokers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerEarliestWinTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockChainParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockPendingUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockSpecialEvents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28792 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockTransactionEvents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlocksAtHeight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetConsensusInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetElectionInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetFinalizedBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetIdentityProviders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetModuleSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegationInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetTokenomicsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_InvokeInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38653 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_SharedConverters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    99596 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131737 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   198939 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/types_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/wadze.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:41.701074 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13652 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_accountByAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_bakerByBakerId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_bakers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20427 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_blockByBlockHash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_passiveDelegation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_paydayStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForBakerPool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_rewardMetricsForAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_transactionByTransactionHash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_transactionMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/exchange_account_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/ql_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41243 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/cis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/cns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15760 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:41.701074 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb_queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb_queries/_apy_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb_queries/_baker_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb_queries/_search_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15024 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb_queries/_store_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb_queries/_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/tooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46983 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/user_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:41.701074 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-28 07:49:41.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-28 07:49:41.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 07:49:41.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-28 07:49:41.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-28 07:49:41.000000 ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 07:49:41.701074 ccdexplorer_fundamentals-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:41.701074 ccdexplorer_fundamentals-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:49:38.000000 ccdexplorer_fundamentals-0.2.2/tests/__init__.py
```

### Comparing `ccdexplorer_fundamentals-0.2.1/LICENSE.md` & `ccdexplorer_fundamentals-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/PKG-INFO` & `ccdexplorer_fundamentals-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdexplorer-fundamentals
-Version: 0.2.1
+Version: 0.2.2
 Summary: Shared code for CCDExplorer.io and its Notification Bot.
 Home-page: https://github.com/ccdexplorer/ccdexplorer-fundamentals
 Author: Sander de Ruiter
 Author-email: sdr@ccdexplorer.io
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `ccdexplorer_fundamentals-0.2.1/README.md` & `ccdexplorer_fundamentals-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/CCD_Types/__init__.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/CCD_Types/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/__init__.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/concordium/health/__init__.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/concordium/health/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/concordium/v2/__init__.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/concordium/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/health_pb2.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/health_pb2.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/health_pb2_grpc.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_CheckHealth.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_CheckHealth.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountInfo.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountList.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetAccountList.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetAnonymityRevokers.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetAnonymityRevokers.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerEarliestWinTime.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerEarliestWinTime.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerList.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBakerList.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockChainParameters.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockChainParameters.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockInfo.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockPendingUpdates.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockPendingUpdates.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockSpecialEvents.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockSpecialEvents.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockTransactionEvents.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlockTransactionEvents.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlocksAtHeight.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetBlocksAtHeight.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetConsensusInfo.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetConsensusInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetElectionInfo.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetElectionInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetFinalizedBlocks.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetFinalizedBlocks.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetIdentityProviders.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetIdentityProviders.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceInfo.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceList.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetInstanceList.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetModuleSource.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetModuleSource.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegationInfo.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegationInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegators.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegators.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegators.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegators.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolInfo.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetPoolInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_GetTokenomicsInfo.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_GetTokenomicsInfo.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_InvokeInstance.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_InvokeInstance.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/queries/_SharedConverters.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/queries/_SharedConverters.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/service_pb2.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/service_pb2_grpc.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/types_pb2.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/types_pb2.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/types_pb2.pyi` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/GRPCClient/wadze.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/GRPCClient/wadze.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/block.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/block.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_accountByAddress.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_accountByAddress.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_accounts.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_accounts.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_bakerByBakerId.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_bakerByBakerId.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_bakers.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_bakers.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_blockByBlockHash.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_blockByBlockHash.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_blocks.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_blocks.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_passiveDelegation.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_passiveDelegation.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_paydayStatus.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_paydayStatus.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForBakerPool.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForBakerPool.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_rewardMetricsForAccount.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_rewardMetricsForAccount.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_search.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_search.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_transactionByTransactionHash.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_transactionByTransactionHash.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/_transactionMetrics.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/_transactionMetrics.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/exchange_account_updates.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/exchange_account_updates.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/ccdscan_queries/ql_support.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/ccdscan_queries/ql_support.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/cis.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/cis.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/cns.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/cns.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/credential.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/credential.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/env.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/env.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import datetime as dt
 from enum import Enum
 from typing import Dict, Optional, Union
 
 import motor.motor_asyncio
 from motor.motor_asyncio import AsyncIOMotorCollection
 from pydantic import BaseModel, ConfigDict, Field
-from pymongo import MongoClient
+from pymongo import MongoClient, ReadPreference
 from pymongo.collection import Collection
 from rich.console import Console
 
 from ccdexplorer_fundamentals.env import MONGO_URI
 from ccdexplorer_fundamentals.GRPCClient.CCD_Types import *  # noqa: F403
 from ccdexplorer_fundamentals.mongodb_queries._apy_calculations import (
     Mixin as _apy_calculations,
@@ -330,32 +330,27 @@
 
 class Collections(Enum):
     blocks = "blocks"
     transactions = "transactions"
     special_events = "special_events"
     instances = "instances"
     modules = "modules"
-    messages = "messages"
     paydays = "paydays"
     paydays_performance = "paydays_performance"
     paydays_rewards = "paydays_rewards"
     paydays_apy_intermediate = "paydays_apy_intermediate"
     paydays_current_payday = "paydays_current_payday"
     paydays_helpers = "paydays_helpers"
-    involved_accounts_all = "involved_accounts_all"
-    involved_accounts_all_top_list = "involved_accounts_all_top_list"
     involved_accounts_transfer = "involved_accounts_transfer"
-    involved_contracts = "involved_contracts"
     nightly_accounts = "nightly_accounts"
     blocks_at_end_of_day = "blocks_at_end_of_day"
     blocks_per_day = "blocks_per_day"
     helpers = "helpers"
     memo_transaction_hashes = "memo_transaction_hashes"
     cns_domains = "cns_domains"
-    bot_messages = "bot_messages"
     dashboard_nodes = "dashboard_nodes"
     tokens_accounts = "tokens_accounts"
     tokens_links_v2 = "tokens_links_v2"
     tokens_token_addresses_v2 = "tokens_token_addresses_v2"
     tokens_tags = "tokens_tags"
     tokens_logged_events = "tokens_logged_events"
     tokens_token_addresses = "tokens_token_addresses"
@@ -376,16 +371,14 @@
     tokens_impacted_addresses = "tokens_impacted_addresses"
     schema_logged_events = "schema_logged_events"
 
 
 class CollectionsUtilities(Enum):
     labeled_accounts = "labeled_accounts"
     labeled_accounts_metadata = "labeled_accounts_metadata"
-    users_prod = "users_prod"
-    users_dev = "users_dev"
     exchange_rates = "exchange_rates"
     exchange_rates_historical = "exchange_rates_historical"
     users_v2_prod = "users_v2_prod"
     users_v2_dev = "users_v2_dev"
     message_log = "message_log"
     preferences_explanations = "preferences_explanations"
     release_notes = "release_notes"
@@ -398,18 +391,21 @@
 class MongoDB(
     _search_transfers,
     _subscriptions,
     _distributions,
     _store_block,
     _apy_calculations,
 ):
-    def __init__(self, tooter: Tooter):
+    def __init__(self, tooter: Tooter, nearest: bool = False):
         self.tooter: Tooter = tooter
         try:
-            con = MongoClient(MONGO_URI)
+            if nearest:
+                con = MongoClient(MONGO_URI, read_preference=ReadPreference.NEAREST)
+            else:
+                con = MongoClient(MONGO_URI)
             self.connection: MongoClient = con
 
             self.mainnet_db = con["concordium_mainnet"]
             self.mainnet: Dict[Collections, Collection] = {}
             for collection in Collections:
                 self.mainnet[collection] = self.mainnet_db[collection.value]
 
@@ -441,18 +437,23 @@
 class MongoMotor(
     _search_transfers,
     _subscriptions,
     _distributions,
     _store_block,
     _apy_calculations,
 ):
-    def __init__(self, tooter: Tooter):
+    def __init__(self, tooter: Tooter, nearest: bool = False):
         self.tooter: Tooter = tooter
         try:
-            con = motor.motor_asyncio.AsyncIOMotorClient(MONGO_URI)
+            if nearest:
+                con = motor.motor_asyncio.AsyncIOMotorClient(
+                    MONGO_URI, read_preference=ReadPreference.NEAREST
+                )
+            else:
+                con = motor.motor_asyncio.AsyncIOMotorClient(MONGO_URI)
             self.connection = con
 
             self.mainnet_db = con["concordium_mainnet"]
             self.mainnet: Dict[Collections, AsyncIOMotorCollection] = {}  # type: ignore
             for collection in Collections:
                 self.mainnet[collection] = self.mainnet_db[collection.value]
```

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb_queries/_apy_calculations.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb_queries/_apy_calculations.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb_queries/_baker_distributions.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb_queries/_baker_distributions.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb_queries/_search_transfers.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb_queries/_search_transfers.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb_queries/_store_block.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb_queries/_store_block.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/mongodb_queries/_subscriptions.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/mongodb_queries/_subscriptions.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/node.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/node.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/pool.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/pool.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/tooter.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/tooter.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/transaction.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/transaction.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals/user_v2.py` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals/user_v2.py`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals.egg-info/PKG-INFO` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdexplorer-fundamentals
-Version: 0.2.1
+Version: 0.2.2
 Summary: Shared code for CCDExplorer.io and its Notification Bot.
 Home-page: https://github.com/ccdexplorer/ccdexplorer-fundamentals
 Author: Sander de Ruiter
 Author-email: sdr@ccdexplorer.io
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `ccdexplorer_fundamentals-0.2.1/ccdexplorer_fundamentals.egg-info/SOURCES.txt` & `ccdexplorer_fundamentals-0.2.2/ccdexplorer_fundamentals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdexplorer_fundamentals-0.2.1/setup.py` & `ccdexplorer_fundamentals-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="ccdexplorer-fundamentals",
-    version="0.2.1",
+    version="0.2.2",
     author="Sander de Ruiter",
     author_email="sdr@ccdexplorer.io",
     description="Shared code for CCDExplorer.io and its Notification Bot.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ccdexplorer/ccdexplorer-fundamentals",
     project_urls={},
```

