# Comparing `tmp/hvac-2.1.0.tar.gz` & `tmp/hvac-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hvac-2.1.0.tar", max compression
+gzip compressed data, was "hvac-2.2.0.tar", max compression
```

## Comparing `hvac-2.1.0.tar` & `hvac-2.2.0.tar`

### file list

```diff
@@ -1,254 +1,258 @@
--rw-r--r--   0        0        0    11358 2024-01-03 16:35:23.436840 hvac-2.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2236 2024-01-03 16:35:23.436840 hvac-2.1.0/README.md
--rw-r--r--   0        0        0      624 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/Makefile
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/__init__.py
--rw-r--r--   0        0        0    53552 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/_static/hvac_logo_800px.png
--rw-r--r--   0        0        0     8396 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/advanced_usage.rst
--rw-r--r--   0        0        0       31 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/changelog.rst
--rw-r--r--   0        0        0     3604 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/conf.py
--rw-r--r--   0        0        0      198 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/contrib/index.rst
--rw-r--r--   0        0        0     6802 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/contrib/niquests_http2.rst
--rw-r--r--   0        0        0       34 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/contributing.rst
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/ext/__init__.py
--rw-r--r--   0        0        0    24179 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/ext/hvac_doctest.py
--rw-r--r--   0        0        0      367 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/index.rst
--rw-r--r--   0        0        0     5899 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/overview.rst
--rw-r--r--   0        0        0      116 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/source/hvac_adapters.rst
--rw-r--r--   0        0        0      101 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/source/hvac_api.rst
--rw-r--r--   0        0        0      140 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/source/hvac_api_auth_methods.rst
--rw-r--r--   0        0        0      149 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/source/hvac_api_secrets_engines.rst
--rw-r--r--   0        0        0      146 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/source/hvac_api_system_backend.rst
--rw-r--r--   0        0        0      121 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/source/hvac_aws_utils.rst
--rw-r--r--   0        0        0      122 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/source/hvac_exceptions.rst
--rw-r--r--   0        0        0      107 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/source/hvac_utils.rst
--rw-r--r--   0        0        0       98 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/source/hvac_v1.rst
--rw-r--r--   0        0        0      236 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/source/index.rst
--rw-r--r--   0        0        0     1651 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/usage/auth_methods/approle.rst
--rw-r--r--   0        0        0    16350 2024-01-03 16:35:23.436840 hvac-2.1.0/docs/usage/auth_methods/aws.rst
--rw-r--r--   0        0        0     3421 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/auth_methods/azure.rst
--rw-r--r--   0        0        0     5758 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/auth_methods/gcp.rst
--rw-r--r--   0        0        0     4018 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/auth_methods/github.rst
--rw-r--r--   0        0        0     1158 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/auth_methods/index.rst
--rw-r--r--   0        0        0     6310 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/auth_methods/jwt-oidc.rst
--rw-r--r--   0        0        0      381 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/auth_methods/kubernetes.rst
--rw-r--r--   0        0        0     5594 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/auth_methods/ldap.rst
--rw-r--r--   0        0        0     3947 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/auth_methods/legacymfa.rst
--rw-r--r--   0        0        0     4613 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/auth_methods/okta.rst
--rw-r--r--   0        0        0     1461 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/auth_methods/token.rst
--rw-r--r--   0        0        0      277 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/auth_methods/userpass.rst
--rw-r--r--   0        0        0      816 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/index.rst
--rw-r--r--   0        0        0     4106 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/activedirectory.rst
--rw-r--r--   0        0        0     4688 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/aws.rst
--rw-r--r--   0        0        0     2593 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/azure.rst
--rw-r--r--   0        0        0     8003 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/database.rst
--rw-r--r--   0        0        0    10747 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/gcp.rst
--rw-r--r--   0        0        0    15355 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/identity.rst
--rw-r--r--   0        0        0      184 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/index.rst
--rw-r--r--   0        0        0     1126 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/kv.rst
--rw-r--r--   0        0        0     2443 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/kv_v1.rst
--rw-r--r--   0        0        0     9107 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/kv_v2.rst
--rw-r--r--   0        0        0     9704 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/pki.rst
--rw-r--r--   0        0        0    17669 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/transform.rst
--rw-r--r--   0        0        0    11399 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/secrets_engines/transit.rst
--rw-r--r--   0        0        0     2534 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/audit.rst
--rw-r--r--   0        0        0     2678 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/auth.rst
--rw-r--r--   0        0        0      493 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/health.rst
--rw-r--r--   0        0        0      203 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/index.rst
--rw-r--r--   0        0        0     1990 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/init.rst
--rw-r--r--   0        0        0     8322 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/key.rst
--rw-r--r--   0        0        0      688 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/leader.rst
--rw-r--r--   0        0        0     4232 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/lease.rst
--rw-r--r--   0        0        0     3334 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/mount.rst
--rw-r--r--   0        0        0     2435 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/namespace.rst
--rw-r--r--   0        0        0     7177 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/policies.rst
--rw-r--r--   0        0        0     3309 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/policy.rst
--rw-r--r--   0        0        0     1695 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/quota.rst
--rw-r--r--   0        0        0      857 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/raft.rst
--rw-r--r--   0        0        0     1965 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/seal.rst
--rw-r--r--   0        0        0     1782 2024-01-03 16:35:23.440840 hvac-2.1.0/docs/usage/system_backend/wrapping.rst
--rw-r--r--   0        0        0       50 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/__init__.py
--rw-r--r--   0        0        0    15613 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/adapters.py
--rw-r--r--   0        0        0      423 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/__init__.py
--rw-r--r--   0        0        0     1473 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/__init__.py
--rw-r--r--   0        0        0    20691 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/approle.py
--rw-r--r--   0        0        0    40094 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/aws.py
--rw-r--r--   0        0        0    13324 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/azure.py
--rw-r--r--   0        0        0    14682 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/cert.py
--rw-r--r--   0        0        0    18931 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/gcp.py
--rw-r--r--   0        0        0     8498 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/github.py
--rw-r--r--   0        0        0    19614 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/jwt.py
--rw-r--r--   0        0        0    12165 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/kubernetes.py
--rw-r--r--   0        0        0    22974 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/ldap.py
--rw-r--r--   0        0        0     6552 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/legacy_mfa.py
--rw-r--r--   0        0        0     8743 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/oidc.py
--rw-r--r--   0        0        0    11401 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/okta.py
--rw-r--r--   0        0        0     8447 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/radius.py
--rw-r--r--   0        0        0    25885 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/token.py
--rw-r--r--   0        0        0     5582 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/auth_methods/userpass.py
--rw-r--r--   0        0        0     1639 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/secrets_engines/__init__.py
--rw-r--r--   0        0        0     7150 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/secrets_engines/active_directory.py
--rw-r--r--   0        0        0    17328 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/secrets_engines/aws.py
--rw-r--r--   0        0        0     7356 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/secrets_engines/azure.py
--rw-r--r--   0        0        0     6728 2024-01-03 16:35:23.440840 hvac-2.1.0/hvac/api/secrets_engines/consul.py
--rw-r--r--   0        0        0    15199 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/secrets_engines/database.py
--rw-r--r--   0        0        0    27976 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/secrets_engines/gcp.py
--rw-r--r--   0        0        0    60059 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/secrets_engines/identity.py
--rw-r--r--   0        0        0     3000 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/secrets_engines/kv.py
--rw-r--r--   0        0        0     5811 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/secrets_engines/kv_v1.py
--rw-r--r--   0        0        0    20348 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/secrets_engines/kv_v2.py
--rw-r--r--   0        0        0    28739 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/secrets_engines/pki.py
--rw-r--r--   0        0        0     5823 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/secrets_engines/rabbitmq.py
--rw-r--r--   0        0        0    21482 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/secrets_engines/ssh.py
--rw-r--r--   0        0        0    45096 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/secrets_engines/transform.py
--rw-r--r--   0        0        0    52082 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/secrets_engines/transit.py
--rw-r--r--   0        0        0     1888 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/__init__.py
--rw-r--r--   0        0        0     3741 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/audit.py
--rw-r--r--   0        0        0     9289 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/auth.py
--rw-r--r--   0        0        0     1668 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/capabilities.py
--rw-r--r--   0        0        0     3310 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/health.py
--rw-r--r--   0        0        0     6253 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/init.py
--rw-r--r--   0        0        0    15889 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/key.py
--rw-r--r--   0        0        0     1235 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/leader.py
--rw-r--r--   0        0        0     4326 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/lease.py
--rw-r--r--   0        0        0    10108 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/mount.py
--rw-r--r--   0        0        0     1393 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/namespace.py
--rw-r--r--   0        0        0     8182 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/policies.py
--rw-r--r--   0        0        0     2794 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/policy.py
--rw-r--r--   0        0        0     3773 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/quota.py
--rw-r--r--   0        0        0     5816 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/raft.py
--rw-r--r--   0        0        0     3471 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/seal.py
--rw-r--r--   0        0        0      265 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/system_backend_mixin.py
--rw-r--r--   0        0        0     1146 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/system_backend/wrapping.py
--rw-r--r--   0        0        0      479 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/vault_api_base.py
--rw-r--r--   0        0        0     3678 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/api/vault_api_category.py
--rw-r--r--   0        0        0     3607 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/aws_utils.py
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/constants/__init__.py
--rw-r--r--   0        0        0      220 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/constants/approle.py
--rw-r--r--   0        0        0      363 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/constants/aws.py
--rw-r--r--   0        0        0      221 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/constants/azure.py
--rw-r--r--   0        0        0      927 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/constants/client.py
--rw-r--r--   0        0        0      515 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/constants/gcp.py
--rw-r--r--   0        0        0      137 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/constants/identity.py
--rw-r--r--   0        0        0      900 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/constants/transit.py
--rw-r--r--   0        0        0     1450 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/exceptions.py
--rw-r--r--   0        0        0    18109 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/utils.py
--rw-r--r--   0        0        0    17275 2024-01-03 16:35:23.444840 hvac-2.1.0/hvac/v1/__init__.py
--rw-r--r--   0        0        0     2416 2024-01-03 16:35:23.444840 hvac-2.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0      319 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/README.md
--rw-r--r--   0        0        0     1127 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/ca-cert.pem
--rw-r--r--   0        0        0     1679 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/ca-key.pem
--rw-r--r--   0        0        0      274 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/ca.cnf
--rw-r--r--   0        0        0     1907 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/client-cert.pem
--rw-r--r--   0        0        0     3268 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/client-key.pem
--rw-r--r--   0        0        0      162 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/client.cnf
--rw-r--r--   0        0        0      156 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/example.jwt
--rw-r--r--   0        0        0     2318 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/example.jwt.json
--rw-r--r--   0        0        0       14 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/generated/.gitignore
--rw-r--r--   0        0        0     1078 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/identity_document.p7b
--rw-r--r--   0        0        0     1704 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/oidc_private.pem
--rw-r--r--   0        0        0      451 2024-01-03 16:35:23.444840 hvac-2.1.0/tests/config_files/oidc_public.pem
--rw-r--r--   0        0        0     2333 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/config_files/pgp_key.asc.b64
--rw-r--r--   0        0        0      891 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/config_files/server-cert.csr
--rw-r--r--   0        0        0     1046 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/config_files/server-cert.pem
--rw-r--r--   0        0        0     1704 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/config_files/server-key.pem
--rw-r--r--   0        0        0      241 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/config_files/server.cnf
--rw-r--r--   0        0        0     2602 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/config_files/ssh-key
--rw-r--r--   0        0        0      568 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/config_files/ssh-key.pub
--rw-r--r--   0        0        0      257 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/config_files/vault-doctest.hcl
--rw-r--r--   0        0        0      309 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/config_files/vault-ha-node1.hcl
--rw-r--r--   0        0        0      348 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/config_files/vault-ha-node2.hcl
--rw-r--r--   0        0        0      222 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/config_files/vault-tls.hcl
--rw-r--r--   0        0        0     2334 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/doctest/__init__.py
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/__init__.py
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/__init__.py
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/__init__.py
--rw-r--r--   0        0        0     9889 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/test_approle.py
--rw-r--r--   0        0        0    11672 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/test_azure.py
--rw-r--r--   0        0        0     5750 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/test_cert.py
--rw-r--r--   0        0        0    15222 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/test_gcp.py
--rw-r--r--   0        0        0    10709 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/test_github.py
--rw-r--r--   0        0        0    11017 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/test_jwt.py
--rw-r--r--   0        0        0    13573 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/test_kubernetes.py
--rw-r--r--   0        0        0    20378 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/test_ldap.py
--rw-r--r--   0        0        0     9320 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/test_legacy_mfa.py
--rw-r--r--   0        0        0    13200 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/test_oidc.py
--rw-r--r--   0        0        0    16548 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/test_okta.py
--rw-r--r--   0        0        0     8713 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/auth_methods/test_token.py
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/secrets_engines/__init__.py
--rw-r--r--   0        0        0    12139 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_aws.py
--rw-r--r--   0        0        0     4259 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_azure.py
--rw-r--r--   0        0        0     2167 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_gcp.py
--rw-r--r--   0        0        0    81593 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_identity.py
--rw-r--r--   0        0        0     6936 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_kv_v1.py
--rw-r--r--   0        0        0    34950 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_kv_v2.py
--rw-r--r--   0        0        0    26443 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_pki.py
--rw-r--r--   0        0        0    15239 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_ssh.py
--rw-r--r--   0        0        0    18194 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_transform.py
--rw-r--r--   0        0        0    34788 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_transit.py
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/__init__.py
--rw-r--r--   0        0        0     2705 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_audit.py
--rw-r--r--   0        0        0     1973 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_auth.py
--rw-r--r--   0        0        0     4127 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_health.py
--rw-r--r--   0        0        0      624 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_init.py
--rw-r--r--   0        0        0     4757 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_key.py
--rw-r--r--   0        0        0      326 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_leader.py
--rw-r--r--   0        0        0     3472 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_lease.py
--rw-r--r--   0        0        0     2758 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_mount.py
--rw-r--r--   0        0        0      949 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_namespace.py
--rw-r--r--   0        0        0    17152 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_policies.py
--rw-r--r--   0        0        0     3441 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_policy.py
--rw-r--r--   0        0        0    12303 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_quota.py
--rw-r--r--   0        0        0     1146 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_seal.py
--rw-r--r--   0        0        0     1148 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/api/system_backend/test_wrapping.py
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/v1/__init__.py
--rw-r--r--   0        0        0     5699 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/v1/test_approle.py
--rw-r--r--   0        0        0    13233 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/v1/test_integration.py
--rw-r--r--   0        0        0    17527 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/integration_tests/v1/test_system_backend.py
--rwxr-xr-x   0        0        0      884 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/scripts/generate_test_cert.sh
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/unit_tests/api/__init__.py
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/unit_tests/api/auth_methods/__init__.py
--rw-r--r--   0        0        0    22385 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/unit_tests/api/auth_methods/test_approle.py
--rw-r--r--   0        0        0     2968 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/unit_tests/api/auth_methods/test_azure.py
--rw-r--r--   0        0        0     2140 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/unit_tests/api/auth_methods/test_gcp.py
--rw-r--r--   0        0        0     8572 2024-01-03 16:35:23.448840 hvac-2.1.0/tests/unit_tests/api/auth_methods/test_github.py
--rw-r--r--   0        0        0     4844 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/auth_methods/test_jwt.py
--rw-r--r--   0        0        0    11287 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/auth_methods/test_kubernetes.py
--rw-r--r--   0        0        0    14136 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/auth_methods/test_ldap.py
--rw-r--r--   0        0        0     5326 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/auth_methods/test_legacy_mfa.py
--rw-r--r--   0        0        0     2310 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/auth_methods/test_okta.py
--rw-r--r--   0        0        0     1709 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/auth_methods/test_token.py
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/secrets_engines/__init__.py
--rw-r--r--   0        0        0     3584 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/secrets_engines/test_aws.py
--rw-r--r--   0        0        0     3883 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/secrets_engines/test_azure.py
--rw-r--r--   0        0        0     3286 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/secrets_engines/test_database.py
--rw-r--r--   0        0        0    46432 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/secrets_engines/test_gcp.py
--rw-r--r--   0        0        0     4337 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/secrets_engines/test_kv.py
--rw-r--r--   0        0        0     5124 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/system_backend/test_init.py
--rw-r--r--   0        0        0     2011 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/api/test_vault_api_category.py
--rw-r--r--   0        0        0      697 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/conftest.py
--rw-r--r--   0        0        0    10715 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/test_adapters.py
--rw-r--r--   0        0        0    21128 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/utils/test_utils.py
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/v1/__init__.py
--rw-r--r--   0        0        0    22690 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/v1/test_approle_routes.py
--rw-r--r--   0        0        0     2363 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/v1/test_auth_methods.py
--rw-r--r--   0        0        0    15255 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/v1/test_aws_ec2_methods.py
--rw-r--r--   0        0        0     2363 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/v1/test_aws_iam_methods.py
--rw-r--r--   0        0        0      577 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/v1/test_client.py
--rw-r--r--   0        0        0     2271 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/v1/test_gcp_methods.py
--rw-r--r--   0        0        0     5535 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/unit_tests/v1/test_system_backend_methods.py
--rw-r--r--   0        0        0    11067 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     7344 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/hvac_integration_test_case.py
--rw-r--r--   0        0        0     2629 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/mock_github_request_handler.py
--rw-r--r--   0        0        0     2243 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/mock_ldap_server.py
--rw-r--r--   0        0        0        0 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/mock_oauth_provider/__init__.py
--rw-r--r--   0        0        0      961 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/mock_oauth_provider/app.py
--rwxr-xr-x   0        0        0     5115 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/mock_oauth_provider/mock_oauth_provider.py
--rw-r--r--   0        0        0     1539 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/mock_oauth_provider/models.py
--rw-r--r--   0        0        0     4587 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/mock_oauth_provider/oauth2.py
--rw-r--r--   0        0        0     4591 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/mock_oauth_provider/routes.py
--rw-r--r--   0        0        0      125 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/mock_oauth_provider/settings.py
--rw-r--r--   0        0        0     2350 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/mock_okta_request_handler.py
--rw-r--r--   0        0        0    14537 2024-01-03 16:35:23.452840 hvac-2.1.0/tests/utils/server_manager.py
--rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 hvac-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-27 22:39:01.440236 hvac-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2236 2024-04-27 22:39:01.440236 hvac-2.2.0/README.md
+-rw-r--r--   0        0        0      624 2024-04-27 22:39:01.440236 hvac-2.2.0/docs/Makefile
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/__init__.py
+-rw-r--r--   0        0        0    53552 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/_static/hvac_logo_800px.png
+-rw-r--r--   0        0        0     8396 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/advanced_usage.rst
+-rw-r--r--   0        0        0       31 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/changelog.rst
+-rw-r--r--   0        0        0     3604 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/conf.py
+-rw-r--r--   0        0        0      198 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/contrib/index.rst
+-rw-r--r--   0        0        0     6802 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/contrib/niquests_http2.rst
+-rw-r--r--   0        0        0       34 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/contributing.rst
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/ext/__init__.py
+-rw-r--r--   0        0        0    24179 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/ext/hvac_doctest.py
+-rw-r--r--   0        0        0      367 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/index.rst
+-rw-r--r--   0        0        0     5899 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/overview.rst
+-rw-r--r--   0        0        0      116 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/source/hvac_adapters.rst
+-rw-r--r--   0        0        0      101 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/source/hvac_api.rst
+-rw-r--r--   0        0        0      140 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/source/hvac_api_auth_methods.rst
+-rw-r--r--   0        0        0      149 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/source/hvac_api_secrets_engines.rst
+-rw-r--r--   0        0        0      146 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/source/hvac_api_system_backend.rst
+-rw-r--r--   0        0        0      121 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/source/hvac_aws_utils.rst
+-rw-r--r--   0        0        0      122 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/source/hvac_exceptions.rst
+-rw-r--r--   0        0        0      107 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/source/hvac_utils.rst
+-rw-r--r--   0        0        0       98 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/source/hvac_v1.rst
+-rw-r--r--   0        0        0      236 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1651 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/approle.rst
+-rw-r--r--   0        0        0    16350 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/aws.rst
+-rw-r--r--   0        0        0     3421 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/azure.rst
+-rw-r--r--   0        0        0     5758 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/gcp.rst
+-rw-r--r--   0        0        0     4018 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/github.rst
+-rw-r--r--   0        0        0     1158 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/index.rst
+-rw-r--r--   0        0        0     6310 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/jwt-oidc.rst
+-rw-r--r--   0        0        0      381 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/kubernetes.rst
+-rw-r--r--   0        0        0     5594 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/ldap.rst
+-rw-r--r--   0        0        0     3947 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/legacymfa.rst
+-rw-r--r--   0        0        0     4613 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/okta.rst
+-rw-r--r--   0        0        0     1461 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/token.rst
+-rw-r--r--   0        0        0      277 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/auth_methods/userpass.rst
+-rw-r--r--   0        0        0      816 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/index.rst
+-rw-r--r--   0        0        0     4106 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/activedirectory.rst
+-rw-r--r--   0        0        0     4688 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/aws.rst
+-rw-r--r--   0        0        0     2593 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/azure.rst
+-rw-r--r--   0        0        0     8003 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/database.rst
+-rw-r--r--   0        0        0    10747 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/gcp.rst
+-rw-r--r--   0        0        0    15355 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/identity.rst
+-rw-r--r--   0        0        0      192 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/index.rst
+-rw-r--r--   0        0        0     1126 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/kv.rst
+-rw-r--r--   0        0        0     2443 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/kv_v1.rst
+-rw-r--r--   0        0        0     9107 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/kv_v2.rst
+-rw-r--r--   0        0        0     4985 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/ldap.rst
+-rw-r--r--   0        0        0     9704 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/pki.rst
+-rw-r--r--   0        0        0    17669 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/transform.rst
+-rw-r--r--   0        0        0    11399 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/secrets_engines/transit.rst
+-rw-r--r--   0        0        0     2534 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/audit.rst
+-rw-r--r--   0        0        0     2678 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/auth.rst
+-rw-r--r--   0        0        0      493 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/health.rst
+-rw-r--r--   0        0        0      203 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/index.rst
+-rw-r--r--   0        0        0     1990 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/init.rst
+-rw-r--r--   0        0        0     8322 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/key.rst
+-rw-r--r--   0        0        0      688 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/leader.rst
+-rw-r--r--   0        0        0     4232 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/lease.rst
+-rw-r--r--   0        0        0     3334 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/mount.rst
+-rw-r--r--   0        0        0     2435 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/namespace.rst
+-rw-r--r--   0        0        0     7177 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/policies.rst
+-rw-r--r--   0        0        0     3309 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/policy.rst
+-rw-r--r--   0        0        0     1695 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/quota.rst
+-rw-r--r--   0        0        0      857 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/raft.rst
+-rw-r--r--   0        0        0     1965 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/seal.rst
+-rw-r--r--   0        0        0     1782 2024-04-27 22:39:01.444236 hvac-2.2.0/docs/usage/system_backend/wrapping.rst
+-rw-r--r--   0        0        0       50 2024-04-27 22:39:01.444236 hvac-2.2.0/hvac/__init__.py
+-rw-r--r--   0        0        0    15613 2024-04-27 22:39:01.444236 hvac-2.2.0/hvac/adapters.py
+-rw-r--r--   0        0        0      423 2024-04-27 22:39:01.444236 hvac-2.2.0/hvac/api/__init__.py
+-rw-r--r--   0        0        0     1473 2024-04-27 22:39:01.444236 hvac-2.2.0/hvac/api/auth_methods/__init__.py
+-rw-r--r--   0        0        0    20691 2024-04-27 22:39:01.444236 hvac-2.2.0/hvac/api/auth_methods/approle.py
+-rw-r--r--   0        0        0    41982 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/aws.py
+-rw-r--r--   0        0        0    13324 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/azure.py
+-rw-r--r--   0        0        0    14682 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/cert.py
+-rw-r--r--   0        0        0    18931 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/gcp.py
+-rw-r--r--   0        0        0     8498 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/github.py
+-rw-r--r--   0        0        0    19920 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/jwt.py
+-rw-r--r--   0        0        0    12165 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/kubernetes.py
+-rw-r--r--   0        0        0    22974 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/ldap.py
+-rw-r--r--   0        0        0     6552 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/legacy_mfa.py
+-rw-r--r--   0        0        0     8743 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/oidc.py
+-rw-r--r--   0        0        0    11397 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/okta.py
+-rw-r--r--   0        0        0     8447 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/radius.py
+-rw-r--r--   0        0        0    25885 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/token.py
+-rw-r--r--   0        0        0     5582 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/auth_methods/userpass.py
+-rw-r--r--   0        0        0     1712 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/__init__.py
+-rw-r--r--   0        0        0     7150 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/active_directory.py
+-rw-r--r--   0        0        0    17328 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/aws.py
+-rw-r--r--   0        0        0     7356 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/azure.py
+-rw-r--r--   0        0        0     6728 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/consul.py
+-rw-r--r--   0        0        0    15199 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/database.py
+-rw-r--r--   0        0        0    27976 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/gcp.py
+-rw-r--r--   0        0        0    60046 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/identity.py
+-rw-r--r--   0        0        0     3000 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/kv.py
+-rw-r--r--   0        0        0     5811 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/kv_v1.py
+-rw-r--r--   0        0        0    20348 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/kv_v2.py
+-rw-r--r--   0        0        0    10096 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/ldap.py
+-rw-r--r--   0        0        0    28739 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/pki.py
+-rw-r--r--   0        0        0     5823 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/rabbitmq.py
+-rw-r--r--   0        0        0    21482 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/ssh.py
+-rw-r--r--   0        0        0    45096 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/transform.py
+-rw-r--r--   0        0        0    52778 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/secrets_engines/transit.py
+-rw-r--r--   0        0        0     1888 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/__init__.py
+-rw-r--r--   0        0        0     3741 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/audit.py
+-rw-r--r--   0        0        0     9289 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/auth.py
+-rw-r--r--   0        0        0     1668 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/capabilities.py
+-rw-r--r--   0        0        0     3310 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/health.py
+-rw-r--r--   0        0        0     6253 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/init.py
+-rw-r--r--   0        0        0    15889 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/key.py
+-rw-r--r--   0        0        0     1235 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/leader.py
+-rw-r--r--   0        0        0     4326 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/lease.py
+-rw-r--r--   0        0        0    10108 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/mount.py
+-rw-r--r--   0        0        0     1393 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/namespace.py
+-rw-r--r--   0        0        0     8182 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/policies.py
+-rw-r--r--   0        0        0     2794 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/policy.py
+-rw-r--r--   0        0        0     3773 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/quota.py
+-rw-r--r--   0        0        0     5816 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/raft.py
+-rw-r--r--   0        0        0     3471 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/seal.py
+-rw-r--r--   0        0        0      265 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/system_backend_mixin.py
+-rw-r--r--   0        0        0     1146 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/system_backend/wrapping.py
+-rw-r--r--   0        0        0      479 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/vault_api_base.py
+-rw-r--r--   0        0        0     3678 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/api/vault_api_category.py
+-rw-r--r--   0        0        0     3607 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/aws_utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/constants/__init__.py
+-rw-r--r--   0        0        0      220 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/constants/approle.py
+-rw-r--r--   0        0        0      363 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/constants/aws.py
+-rw-r--r--   0        0        0      221 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/constants/azure.py
+-rw-r--r--   0        0        0      927 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/constants/client.py
+-rw-r--r--   0        0        0      515 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/constants/gcp.py
+-rw-r--r--   0        0        0      170 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/constants/identity.py
+-rw-r--r--   0        0        0      900 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/constants/transit.py
+-rw-r--r--   0        0        0     1550 2024-04-27 22:39:01.448236 hvac-2.2.0/hvac/exceptions.py
+-rw-r--r--   0        0        0    18109 2024-04-27 22:39:01.452236 hvac-2.2.0/hvac/utils.py
+-rw-r--r--   0        0        0    17275 2024-04-27 22:39:01.452236 hvac-2.2.0/hvac/v1/__init__.py
+-rw-r--r--   0        0        0     2601 2024-04-27 22:39:01.452236 hvac-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      319 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/README.md
+-rw-r--r--   0        0        0     1127 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/ca-cert.pem
+-rw-r--r--   0        0        0     1679 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/ca-key.pem
+-rw-r--r--   0        0        0      274 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/ca.cnf
+-rw-r--r--   0        0        0     1907 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/client-cert.pem
+-rw-r--r--   0        0        0     3268 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/client-key.pem
+-rw-r--r--   0        0        0      162 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/client.cnf
+-rw-r--r--   0        0        0      156 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/example.jwt
+-rw-r--r--   0        0        0     2318 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/example.jwt.json
+-rw-r--r--   0        0        0       14 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/generated/.gitignore
+-rw-r--r--   0        0        0     1078 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/identity_document.p7b
+-rw-r--r--   0        0        0     1704 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/oidc_private.pem
+-rw-r--r--   0        0        0      451 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/oidc_public.pem
+-rw-r--r--   0        0        0     2333 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/pgp_key.asc.b64
+-rw-r--r--   0        0        0      891 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/server-cert.csr
+-rw-r--r--   0        0        0     1046 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/server-cert.pem
+-rw-r--r--   0        0        0     1704 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/server-key.pem
+-rw-r--r--   0        0        0      241 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/server.cnf
+-rw-r--r--   0        0        0     2602 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/ssh-key
+-rw-r--r--   0        0        0      568 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/ssh-key.pub
+-rw-r--r--   0        0        0      257 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/vault-doctest.hcl
+-rw-r--r--   0        0        0      309 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/vault-ha-node1.hcl
+-rw-r--r--   0        0        0      348 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/vault-ha-node2.hcl
+-rw-r--r--   0        0        0      222 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/config_files/vault-tls.hcl
+-rw-r--r--   0        0        0     2334 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/doctest/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/__init__.py
+-rw-r--r--   0        0        0     9889 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_approle.py
+-rw-r--r--   0        0        0     4315 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_aws.py
+-rw-r--r--   0        0        0    11672 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_azure.py
+-rw-r--r--   0        0        0     5750 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_cert.py
+-rw-r--r--   0        0        0    15222 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_gcp.py
+-rw-r--r--   0        0        0    10709 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_github.py
+-rw-r--r--   0        0        0    11491 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_jwt.py
+-rw-r--r--   0        0        0    13573 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_kubernetes.py
+-rw-r--r--   0        0        0    20350 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_ldap.py
+-rw-r--r--   0        0        0     9320 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_legacy_mfa.py
+-rw-r--r--   0        0        0    13200 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_oidc.py
+-rw-r--r--   0        0        0    16548 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_okta.py
+-rw-r--r--   0        0        0     8713 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/auth_methods/test_token.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/secrets_engines/__init__.py
+-rw-r--r--   0        0        0    12139 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_aws.py
+-rw-r--r--   0        0        0     4259 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_azure.py
+-rw-r--r--   0        0        0     2167 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_gcp.py
+-rw-r--r--   0        0        0    81593 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_identity.py
+-rw-r--r--   0        0        0     6936 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_kv_v1.py
+-rw-r--r--   0        0        0    34950 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_kv_v2.py
+-rw-r--r--   0        0        0    26443 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_pki.py
+-rw-r--r--   0        0        0    15239 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_ssh.py
+-rw-r--r--   0        0        0    18194 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_transform.py
+-rw-r--r--   0        0        0    34788 2024-04-27 22:39:01.452236 hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_transit.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/__init__.py
+-rw-r--r--   0        0        0     2705 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_audit.py
+-rw-r--r--   0        0        0     1973 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_auth.py
+-rw-r--r--   0        0        0     4127 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_health.py
+-rw-r--r--   0        0        0      624 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_init.py
+-rw-r--r--   0        0        0     4757 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_key.py
+-rw-r--r--   0        0        0      326 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_leader.py
+-rw-r--r--   0        0        0     3472 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_lease.py
+-rw-r--r--   0        0        0     2758 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_mount.py
+-rw-r--r--   0        0        0      949 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_namespace.py
+-rw-r--r--   0        0        0    17152 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_policies.py
+-rw-r--r--   0        0        0     3441 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_policy.py
+-rw-r--r--   0        0        0    12303 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_quota.py
+-rw-r--r--   0        0        0     1146 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_seal.py
+-rw-r--r--   0        0        0     1148 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/api/system_backend/test_wrapping.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/v1/__init__.py
+-rw-r--r--   0        0        0     5699 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/v1/test_approle.py
+-rw-r--r--   0        0        0    13233 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/v1/test_integration.py
+-rw-r--r--   0        0        0    17527 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/integration_tests/v1/test_system_backend.py
+-rwxr-xr-x   0        0        0      884 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/scripts/generate_test_cert.sh
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/auth_methods/__init__.py
+-rw-r--r--   0        0        0    22385 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/auth_methods/test_approle.py
+-rw-r--r--   0        0        0     2968 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/auth_methods/test_azure.py
+-rw-r--r--   0        0        0     2140 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/auth_methods/test_gcp.py
+-rw-r--r--   0        0        0     8572 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/auth_methods/test_github.py
+-rw-r--r--   0        0        0     4844 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/auth_methods/test_jwt.py
+-rw-r--r--   0        0        0    11287 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/auth_methods/test_kubernetes.py
+-rw-r--r--   0        0        0    14136 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/auth_methods/test_ldap.py
+-rw-r--r--   0        0        0     5326 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/auth_methods/test_legacy_mfa.py
+-rw-r--r--   0        0        0     2310 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/auth_methods/test_okta.py
+-rw-r--r--   0        0        0     1709 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/auth_methods/test_token.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/secrets_engines/__init__.py
+-rw-r--r--   0        0        0     3584 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/secrets_engines/test_aws.py
+-rw-r--r--   0        0        0     3883 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/secrets_engines/test_azure.py
+-rw-r--r--   0        0        0     3286 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/secrets_engines/test_database.py
+-rw-r--r--   0        0        0    46432 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/secrets_engines/test_gcp.py
+-rw-r--r--   0        0        0     4337 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/secrets_engines/test_kv.py
+-rw-r--r--   0        0        0    11378 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/secrets_engines/test_ldap.py
+-rw-r--r--   0        0        0     5124 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/system_backend/test_init.py
+-rw-r--r--   0        0        0     2011 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/api/test_vault_api_category.py
+-rw-r--r--   0        0        0      697 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/conftest.py
+-rw-r--r--   0        0        0    10715 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/test_adapters.py
+-rw-r--r--   0        0        0    21128 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/utils/test_utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/v1/__init__.py
+-rw-r--r--   0        0        0    22690 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/v1/test_approle_routes.py
+-rw-r--r--   0        0        0     2363 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/v1/test_auth_methods.py
+-rw-r--r--   0        0        0    15255 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/v1/test_aws_ec2_methods.py
+-rw-r--r--   0        0        0     2363 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/v1/test_aws_iam_methods.py
+-rw-r--r--   0        0        0      577 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/v1/test_client.py
+-rw-r--r--   0        0        0     2271 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/v1/test_gcp_methods.py
+-rw-r--r--   0        0        0     5535 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/unit_tests/v1/test_system_backend_methods.py
+-rw-r--r--   0        0        0    11400 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     7316 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/hvac_integration_test_case.py
+-rw-r--r--   0        0        0     2629 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/mock_github_request_handler.py
+-rw-r--r--   0        0        0     2243 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/mock_ldap_server.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/mock_oauth_provider/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/mock_oauth_provider/app.py
+-rwxr-xr-x   0        0        0     5115 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/mock_oauth_provider/mock_oauth_provider.py
+-rw-r--r--   0        0        0     1539 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/mock_oauth_provider/models.py
+-rw-r--r--   0        0        0     4587 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/mock_oauth_provider/oauth2.py
+-rw-r--r--   0        0        0     4591 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/mock_oauth_provider/routes.py
+-rw-r--r--   0        0        0      125 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/mock_oauth_provider/settings.py
+-rw-r--r--   0        0        0     2350 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/mock_okta_request_handler.py
+-rw-r--r--   0        0        0    15023 2024-04-27 22:39:01.456236 hvac-2.2.0/tests/utils/server_manager.py
+-rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 hvac-2.2.0/PKG-INFO
```

### Comparing `hvac-2.1.0/LICENSE.txt` & `hvac-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/README.md` & `hvac-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/Makefile` & `hvac-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/_static/hvac_logo_800px.png` & `hvac-2.2.0/docs/_static/hvac_logo_800px.png`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/advanced_usage.rst` & `hvac-2.2.0/docs/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/conf.py` & `hvac-2.2.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # -- Project information -----------------------------------------------------
 
 project = "hvac"
 copyright = "2018-2020, Ian Unruh, Jeffrey Hogan"
 author = "Ian Unruh, Jeffrey Hogan"
 
 # The short X.Y version
-version = "2.1.0"
+version = "2.2.0"
 # The full version, including alpha/beta/rc tags
-release = "2.1.0"
+release = "2.2.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 extensions = [
     "docs.ext.hvac_doctest",
     "sphinx.ext.autodoc",
```

### Comparing `hvac-2.1.0/docs/contrib/niquests_http2.rst` & `hvac-2.2.0/docs/contrib/niquests_http2.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/ext/hvac_doctest.py` & `hvac-2.2.0/docs/ext/hvac_doctest.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/overview.rst` & `hvac-2.2.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/auth_methods/approle.rst` & `hvac-2.2.0/docs/usage/auth_methods/approle.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/auth_methods/aws.rst` & `hvac-2.2.0/docs/usage/auth_methods/aws.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/auth_methods/azure.rst` & `hvac-2.2.0/docs/usage/auth_methods/azure.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/auth_methods/gcp.rst` & `hvac-2.2.0/docs/usage/auth_methods/gcp.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/auth_methods/github.rst` & `hvac-2.2.0/docs/usage/auth_methods/github.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/auth_methods/index.rst` & `hvac-2.2.0/docs/usage/auth_methods/index.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/auth_methods/jwt-oidc.rst` & `hvac-2.2.0/docs/usage/auth_methods/jwt-oidc.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/auth_methods/ldap.rst` & `hvac-2.2.0/docs/usage/auth_methods/ldap.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/auth_methods/legacymfa.rst` & `hvac-2.2.0/docs/usage/auth_methods/legacymfa.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/auth_methods/okta.rst` & `hvac-2.2.0/docs/usage/auth_methods/okta.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/auth_methods/token.rst` & `hvac-2.2.0/docs/usage/auth_methods/token.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/index.rst` & `hvac-2.2.0/docs/usage/index.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/secrets_engines/activedirectory.rst` & `hvac-2.2.0/docs/usage/secrets_engines/activedirectory.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/secrets_engines/aws.rst` & `hvac-2.2.0/docs/usage/secrets_engines/aws.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/secrets_engines/azure.rst` & `hvac-2.2.0/docs/usage/secrets_engines/azure.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/secrets_engines/database.rst` & `hvac-2.2.0/docs/usage/secrets_engines/database.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/secrets_engines/gcp.rst` & `hvac-2.2.0/docs/usage/secrets_engines/gcp.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/secrets_engines/identity.rst` & `hvac-2.2.0/docs/usage/secrets_engines/identity.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/secrets_engines/kv.rst` & `hvac-2.2.0/docs/usage/secrets_engines/kv.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/secrets_engines/kv_v1.rst` & `hvac-2.2.0/docs/usage/secrets_engines/kv_v1.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/secrets_engines/kv_v2.rst` & `hvac-2.2.0/docs/usage/secrets_engines/kv_v2.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/secrets_engines/pki.rst` & `hvac-2.2.0/docs/usage/secrets_engines/pki.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/secrets_engines/transform.rst` & `hvac-2.2.0/docs/usage/secrets_engines/transform.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/secrets_engines/transit.rst` & `hvac-2.2.0/docs/usage/secrets_engines/transit.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/audit.rst` & `hvac-2.2.0/docs/usage/system_backend/audit.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/auth.rst` & `hvac-2.2.0/docs/usage/system_backend/auth.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/init.rst` & `hvac-2.2.0/docs/usage/system_backend/init.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/key.rst` & `hvac-2.2.0/docs/usage/system_backend/key.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/leader.rst` & `hvac-2.2.0/docs/usage/system_backend/leader.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/lease.rst` & `hvac-2.2.0/docs/usage/system_backend/lease.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/mount.rst` & `hvac-2.2.0/docs/usage/system_backend/mount.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/namespace.rst` & `hvac-2.2.0/docs/usage/system_backend/namespace.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/policies.rst` & `hvac-2.2.0/docs/usage/system_backend/policies.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/policy.rst` & `hvac-2.2.0/docs/usage/system_backend/policy.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/quota.rst` & `hvac-2.2.0/docs/usage/system_backend/quota.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/raft.rst` & `hvac-2.2.0/docs/usage/system_backend/raft.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/seal.rst` & `hvac-2.2.0/docs/usage/system_backend/seal.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/docs/usage/system_backend/wrapping.rst` & `hvac-2.2.0/docs/usage/system_backend/wrapping.rst`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/adapters.py` & `hvac-2.2.0/hvac/adapters.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/__init__.py` & `hvac-2.2.0/hvac/api/auth_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/approle.py` & `hvac-2.2.0/hvac/api/auth_methods/approle.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/aws.py` & `hvac-2.2.0/hvac/api/auth_methods/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         access_key=None,
         secret_key=None,
         endpoint=None,
         iam_endpoint=None,
         sts_endpoint=None,
         iam_server_id_header_value=None,
         mount_point=AWS_DEFAULT_MOUNT_POINT,
+        sts_region=None,
     ):
         """Configure the credentials required to perform API calls to AWS as well as custom endpoints to talk to AWS API.
 
         The instance identity document fetched from the PKCS#7 signature will provide the EC2 instance ID.
         The credentials configured using this endpoint will be used to query the status of the instances via
         DescribeInstances API. If static credentials are not provided using this endpoint, then the credentials will be
         retrieved from the environment variables AWS_ACCESS_KEY, AWS_SECRET_KEY and AWS_REGION respectively.
@@ -65,27 +66,31 @@
             validated. If set, clients must include an X-Vault-AWS-IAM-Server-ID header in the headers of login
             requests, and further this header must be among the signed headers validated by AWS. This is to protect
             against different types of replay attacks, for example a signed request sent to a dev server being resent
             to a production server
         :type iam_server_id_header_value: str | unicode
         :param mount_point: The path the AWS auth method was mounted on.
         :type mount_point: str | unicode
+        :param sts_region: Region to override the default region for making AWS STS API calls. Should only be set if
+            sts_endpoint is set. If so, should be set to the region in which the custom sts_endpoint resides
+        :type sts_region: str | unicode
         :return: The response of the request.
         :rtype: requests.Response
         """
 
         params = utils.remove_nones(
             {
                 "max_retries": max_retries,
                 "access_key": access_key,
                 "secret_key": secret_key,
                 "endpoint": endpoint,
                 "iam_endpoint": iam_endpoint,
                 "sts_endpoint": sts_endpoint,
                 "iam_server_id_header_value": iam_server_id_header_value,
+                "sts_region": sts_region,
             }
         )
         api_path = utils.format_url(
             "/v1/auth/{mount_point}/config/client", mount_point=mount_point
         )
         return self._adapter.post(
             url=api_path,
@@ -124,15 +129,20 @@
         """
         api_path = utils.format_url(
             "/v1/auth/{mount_point}/config/client", mount_point=mount_point
         )
         return self._adapter.delete(url=api_path)
 
     def configure_identity_integration(
-        self, iam_alias=None, ec2_alias=None, mount_point=AWS_DEFAULT_MOUNT_POINT
+        self,
+        iam_alias=None,
+        ec2_alias=None,
+        mount_point=AWS_DEFAULT_MOUNT_POINT,
+        iam_metadata=None,
+        ec2_metadata=None,
     ):
         """Configure the way that Vault interacts with the Identity store.
 
         The default (as of Vault 1.0.3) is role_id for both values.
 
         Supported methods:
             POST: /auth/{mount_point}/config/identity Produces: 204 (empty body)
@@ -142,42 +152,52 @@
             unique_id is selected, the IAM Unique ID of the IAM principal (either the user or role) is used as the
             identity alias name. When full_arn is selected, the ARN returned by the sts:GetCallerIdentity call is used
             as the alias name. This is either arn:aws:iam::<account_id>:user/<optional_path/><user_name> or
             arn:aws:sts::<account_id>:assumed-role/<role_name_without_path>/<role_session_name>. Note: if you
             select full_arn and then delete and recreate the IAM role, Vault won't be aware and any identity aliases
             set up for the role name will still be valid
         :type iam_alias: str | unicode
+        :param iam_metadata: The metadata to include on the token returned by the login endpoint.
+            This metadata will be added to both audit logs, and on the ``iam_alias``. By default, it includes ``account_id``
+            and ``auth_type``. Additionally, ``canonical_arn``, ``client_arn``, ``client_user_id``, ``inferred_aws_region``, ``inferred_entity_id``,
+            and ``inferred_entity_type`` are available. To include no metadata, set to an empty list ``[]``.
+            To use only particular fields, select the explicit fields. To restore to defaults, send only a field of ``default``.
+            Only select fields that will have a low rate of change for your ``iam_alias`` because each change triggers a storage
+            write and can have a performance impact at scale.
+        :type iam_metadata: str | unicode | list
         :param ec2_alias: Configures how to generate the identity alias when using the ec2 auth method. Valid choices
             are role_id, instance_id, and image_id. When role_id is selected, the randomly generated ID of the role is
             used. When instance_id is selected, the instance identifier is used as the identity alias name. When
             image_id is selected, AMI ID of the instance is used as the identity alias name
         :type ec2_alias: str | unicode
+        :param ec2_metadata: The metadata to include on the token returned by the login endpoint. This metadata will be
+            added to both audit logs, and on the ``ec2_alias``. By default, it includes ``account_id`` and ``auth_type``. Additionally,
+            ``ami_id``, ``instance_id``, and ``region`` are available. To include no metadata, set to an empty list ``[]``.
+            To use only particular fields, select the explicit fields. To restore to defaults, send only a field of ``default``.
+            Only select fields that will have a low rate of change for your ``ec2_alias`` because each change triggers a storage
+            write and can have a performance impact at scale.
+        :type ec2_metadata: str | unicode | list
         :param mount_point: The path the AWS auth method was mounted on.
         :type mount_point: str | unicode
         :return: The response of the request
         :rtype: request.Response
         """
         if iam_alias is not None and iam_alias not in ALLOWED_IAM_ALIAS_TYPES:
-            error_msg = 'invalid iam alias type provided: "{arg}"; supported iam alias types: "{alias_types}"'
-            raise exceptions.ParamValidationError(
-                error_msg.format(
-                    arg=iam_alias, environments=",".join(ALLOWED_IAM_ALIAS_TYPES)
-                )
-            )
+            error_msg = f"invalid iam alias type provided: '{iam_alias}' - supported iam alias types: '{','.join(ALLOWED_IAM_ALIAS_TYPES)}'"
+            raise exceptions.ParamValidationError(error_msg)
         if ec2_alias is not None and ec2_alias not in ALLOWED_EC2_ALIAS_TYPES:
-            error_msg = 'invalid ec2 alias type provided: "{arg}"; supported ec2 alias types: "{alias_types}"'
-            raise exceptions.ParamValidationError(
-                error_msg.format(
-                    arg=ec2_alias, environments=",".join(ALLOWED_EC2_ALIAS_TYPES)
-                )
-            )
+            error_msg = f"invalid ec2 alias type provided: '{ec2_alias}' - supported ec2 alias types: '{','.join(ALLOWED_EC2_ALIAS_TYPES)}'"
+            raise exceptions.ParamValidationError(error_msg)
+
         params = utils.remove_nones(
             {
                 "iam_alias": iam_alias,
                 "ec2_alias": ec2_alias,
+                "ec2_metadata": ec2_metadata,
+                "iam_metadata": iam_metadata,
             }
         )
         api_auth = "/v1/auth/{mount_point}/config/identity".format(
             mount_point=mount_point
         )
         return self._adapter.post(
             url=api_auth,
```

### Comparing `hvac-2.1.0/hvac/api/auth_methods/azure.py` & `hvac-2.2.0/hvac/api/auth_methods/azure.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/cert.py` & `hvac-2.2.0/hvac/api/auth_methods/cert.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/gcp.py` & `hvac-2.2.0/hvac/api/auth_methods/gcp.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/github.py` & `hvac-2.2.0/hvac/api/auth_methods/github.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/jwt.py` & `hvac-2.2.0/hvac/api/auth_methods/jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         jwks_ca_pem=None,
         jwt_validation_pubkeys=None,
         bound_issuer=None,
         jwt_supported_algs=None,
         default_role=None,
         provider_config=None,
         path=None,
+        namespace_in_state=None,
     ):
         """Configure the validation information to be used globally across all roles.
 
         One (and only one) of oidc_discovery_url and jwt_validation_pubkeys must be set.
 
         Supported methods:
             POST: /auth/{path}/config.
@@ -82,14 +83,17 @@
         :type jwt_supported_algs: str | unicode
         :param default_role: The default role to use if none is provided during login.
         :type default_role: str | unicode
         :param provider_config: TypeError
         :type provider_config: map
         :param path: The "path" the method/backend was mounted on.
         :type path: str | unicode
+        :param namespace_in_state: With this setting, the allowed redirect URL(s) in Vault and on the provider side
+            should not contain a namespace query parameter.
+        :type namespace_in_state: bool
         :return: The response of the configure request.
         :rtype: requests.Response
         """
         params = utils.remove_nones(
             {
                 "oidc_discovery_url": oidc_discovery_url,
                 "oidc_discovery_ca_pem": oidc_discovery_ca_pem,
@@ -100,14 +104,15 @@
                 "jwks_url": jwks_url,
                 "jwks_ca_pem": jwks_ca_pem,
                 "jwt_validation_pubkeys": jwt_validation_pubkeys,
                 "bound_issuer": bound_issuer,
                 "jwt_supported_algs": jwt_supported_algs,
                 "default_role": default_role,
                 "provider_config": provider_config,
+                "namespace_in_state": namespace_in_state,
             }
         )
         api_path = utils.format_url(
             "/v1/auth/{path}/config",
             path=self.resolve_path(path),
         )
         return self._adapter.post(
```

### Comparing `hvac-2.1.0/hvac/api/auth_methods/kubernetes.py` & `hvac-2.2.0/hvac/api/auth_methods/kubernetes.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/ldap.py` & `hvac-2.2.0/hvac/api/auth_methods/ldap.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/legacy_mfa.py` & `hvac-2.2.0/hvac/api/auth_methods/legacy_mfa.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/oidc.py` & `hvac-2.2.0/hvac/api/auth_methods/oidc.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/okta.py` & `hvac-2.2.0/hvac/api/auth_methods/okta.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
             POST: /auth/{mount_point}/login/{username}. Produces: 200 application/json
 
         :param username: Username for this user.
         :type username: str | unicode
         :param password: Password for the authenticating user.
         :type password: str | unicode
         :param use_token: if True, uses the token in the response received from the auth request to set the "token"
-            attribute on the the :py:meth:`hvac.adapters.Adapter` instance under the _adapter Client attribute.
+            attribute on the :py:meth:`hvac.adapters.Adapter` instance under the _adapter Client attribute.
         :type use_token: bool
         :param mount_point: The "path" the method/backend was mounted on.
         :type mount_point: str | unicode
         :return: The response of the login request.
         :rtype: dict
         """
         params = {
```

### Comparing `hvac-2.1.0/hvac/api/auth_methods/radius.py` & `hvac-2.2.0/hvac/api/auth_methods/radius.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/token.py` & `hvac-2.2.0/hvac/api/auth_methods/token.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/auth_methods/userpass.py` & `hvac-2.2.0/hvac/api/auth_methods/userpass.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/__init__.py` & `hvac-2.2.0/hvac/api/secrets_engines/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from hvac.api.secrets_engines.consul import Consul
 from hvac.api.secrets_engines.database import Database
 from hvac.api.secrets_engines.gcp import Gcp
 from hvac.api.secrets_engines.identity import Identity
 from hvac.api.secrets_engines.kv import Kv
 from hvac.api.secrets_engines.kv_v1 import KvV1
 from hvac.api.secrets_engines.kv_v2 import KvV2
+from hvac.api.secrets_engines.ldap import Ldap
 from hvac.api.secrets_engines.pki import Pki
 from hvac.api.secrets_engines.rabbitmq import RabbitMQ
 from hvac.api.secrets_engines.ssh import Ssh
 from hvac.api.secrets_engines.transform import Transform
 from hvac.api.secrets_engines.transit import Transit
 from hvac.api.vault_api_category import VaultApiCategory
 
@@ -21,14 +22,15 @@
     "Azure",
     "Gcp",
     "ActiveDirectory",
     "Identity",
     "Kv",
     "KvV1",
     "KvV2",
+    "Ldap",
     "Pki",
     "Transform",
     "Transit",
     "SecretsEngines",
     "Database",
     "RabbitMQ",
     "Ssh",
@@ -41,14 +43,15 @@
     implemented_classes = [
         Aws,
         Azure,
         Gcp,
         ActiveDirectory,
         Identity,
         Kv,
+        Ldap,
         Pki,
         Transform,
         Transit,
         Database,
         Consul,
         RabbitMQ,
         Ssh,
```

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/active_directory.py` & `hvac-2.2.0/hvac/api/secrets_engines/active_directory.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/aws.py` & `hvac-2.2.0/hvac/api/secrets_engines/aws.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/azure.py` & `hvac-2.2.0/hvac/api/secrets_engines/azure.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/consul.py` & `hvac-2.2.0/hvac/api/secrets_engines/consul.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/database.py` & `hvac-2.2.0/hvac/api/secrets_engines/database.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/gcp.py` & `hvac-2.2.0/hvac/api/secrets_engines/gcp.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/identity.py` & `hvac-2.2.0/hvac/api/secrets_engines/identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python
 """Identity secret engine module."""
 import logging
 
 from hvac import exceptions, utils
 from hvac.api.vault_api_base import VaultApiBase
-from hvac.constants.identity import ALLOWED_GROUP_TYPES
-
-DEFAULT_MOUNT_POINT = "identity"
+from hvac.constants.identity import ALLOWED_GROUP_TYPES, DEFAULT_MOUNT_POINT
 
 logger = logging.getLogger(__name__)
 
 
 class Identity(VaultApiBase):
     """Identity Secrets Engine (API).
```

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/kv.py` & `hvac-2.2.0/hvac/api/secrets_engines/kv.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/kv_v1.py` & `hvac-2.2.0/hvac/api/secrets_engines/kv_v1.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/kv_v2.py` & `hvac-2.2.0/hvac/api/secrets_engines/kv_v2.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/pki.py` & `hvac-2.2.0/hvac/api/secrets_engines/pki.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/rabbitmq.py` & `hvac-2.2.0/hvac/api/secrets_engines/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/ssh.py` & `hvac-2.2.0/hvac/api/secrets_engines/ssh.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/transform.py` & `hvac-2.2.0/hvac/api/secrets_engines/transform.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/secrets_engines/transit.py` & `hvac-2.2.0/hvac/api/secrets_engines/transit.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,14 +318,15 @@
         context=None,
         key_version=None,
         nonce=None,
         batch_input=None,
         type=None,
         convergent_encryption=None,
         mount_point=DEFAULT_MOUNT_POINT,
+        associated_data=None,
     ):
         """Encrypt the provided plaintext using the named key.
 
         This path supports the create and update policy capabilities as follows: if the user has the create capability
         for this endpoint in their policies, and the key does not exist, it will be upserted with default values
         (whether the key requires derivation depends on whether the context parameter is empty or not). If the user only
         has update capability and the key does not exist, an error will be returned.
@@ -336,14 +337,17 @@
         :param name: Specifies the name of the encryption key to encrypt against. This is specified as part of the URL.
         :type name: str | unicode
         :param plaintext: Specifies base64 encoded plaintext to be encoded. Ignored if ``batch_input`` is set, otherwise required.
         :type plaintext: str | unicode
         :param context: Specifies the base64 encoded context for key derivation. This is required if key derivation is
             enabled for this key.
         :type context: str | unicode
+        :param associated_data: Specifies base64 encoded associated data (also known as additional data or AAD) to also be authenticated
+            with AEAD ciphers (aes128-gcm96, aes256-gcm, and chacha20-poly1305)
+        :type associated_data: str | unicode
         :param key_version: Specifies the version of the key to use for encryption. If not set, uses the latest version.
             Must be greater than or equal to the key's min_encryption_version, if set.
         :type key_version: int
         :param nonce: Specifies the base64 encoded nonce value. This must be provided if convergent encryption is
             enabled for this key and the key was generated with Vault 0.6.1. Not required for keys created in 0.6.2+.
             The value must be exactly 96 bits (12 bytes) long and the user must ensure that for any given context (and
             thus, any given encryption key) this nonce value is never reused.
@@ -372,14 +376,15 @@
         params = {
             "plaintext": plaintext,
         }
         params.update(
             utils.remove_nones(
                 {
                     "context": context,
+                    "associated_data": associated_data,
                     "key_version": key_version,
                     "nonce": nonce,
                     "batch_input": batch_input,
                     "type": type,
                     "convergent_encryption": convergent_encryption,
                 }
             )
@@ -398,27 +403,31 @@
         self,
         name,
         ciphertext=None,
         context=None,
         nonce=None,
         batch_input=None,
         mount_point=DEFAULT_MOUNT_POINT,
+        associated_data=None,
     ):
         """Decrypt the provided ciphertext using the named key.
 
         Supported methods:
             POST: /{mount_point}/decrypt/{name}. Produces: 200 application/json
 
         :param name: Specifies the name of the encryption key to decrypt against. This is specified as part of the URL.
         :type name: str | unicode
         :param ciphertext: The ciphertext to decrypt. Ignored if ``batch_input`` is set, otherwise required.
         :type ciphertext: str | unicode
         :param context: Specifies the base64 encoded context for key derivation. This is required if key derivation is
             enabled.
         :type context: str | unicode
+        :param associated_data: Specifies base64 encoded associated data (also known as additional data or AAD) to also
+            be authenticated with AEAD ciphers (aes128-gcm96, aes256-gcm, and chacha20-poly1305)
+        :type associated_data: str | unicode
         :param nonce: Specifies a base64 encoded nonce value used during encryption. Must be provided if convergent
             encryption is enabled for this key and the key was generated with Vault 0.6.1. Not required for keys created
             in 0.6.2+.
         :type nonce: str | unicode
         :param batch_input: Specifies a list of items to be decrypted in a single batch. When this parameter is set, if
             the parameters 'ciphertext', 'context' and 'nonce' are also set, they will be ignored. Format for the input
             goes like this: [dict(context="b64_context", ciphertext="b64_plaintext"), ...]
@@ -433,14 +442,15 @@
         params = {
             "ciphertext": ciphertext,
         }
         params.update(
             utils.remove_nones(
                 {
                     "context": context,
+                    "associated_data": associated_data,
                     "nonce": nonce,
                     "batch_input": batch_input,
                 }
             )
         )
         api_path = utils.format_url(
             "/v1/{mount_point}/decrypt/{name}",
```

### Comparing `hvac-2.1.0/hvac/api/system_backend/__init__.py` & `hvac-2.2.0/hvac/api/system_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/audit.py` & `hvac-2.2.0/hvac/api/system_backend/audit.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/auth.py` & `hvac-2.2.0/hvac/api/system_backend/auth.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/capabilities.py` & `hvac-2.2.0/hvac/api/system_backend/capabilities.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/health.py` & `hvac-2.2.0/hvac/api/system_backend/health.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/init.py` & `hvac-2.2.0/hvac/api/system_backend/init.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/key.py` & `hvac-2.2.0/hvac/api/system_backend/key.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/leader.py` & `hvac-2.2.0/hvac/api/system_backend/leader.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/lease.py` & `hvac-2.2.0/hvac/api/system_backend/lease.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/mount.py` & `hvac-2.2.0/hvac/api/system_backend/mount.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/namespace.py` & `hvac-2.2.0/hvac/api/system_backend/namespace.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/policies.py` & `hvac-2.2.0/hvac/api/system_backend/policies.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/policy.py` & `hvac-2.2.0/hvac/api/system_backend/policy.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/quota.py` & `hvac-2.2.0/hvac/api/system_backend/quota.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/raft.py` & `hvac-2.2.0/hvac/api/system_backend/raft.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/seal.py` & `hvac-2.2.0/hvac/api/system_backend/seal.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/system_backend/wrapping.py` & `hvac-2.2.0/hvac/api/system_backend/wrapping.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/api/vault_api_category.py` & `hvac-2.2.0/hvac/api/vault_api_category.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/aws_utils.py` & `hvac-2.2.0/hvac/aws_utils.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/constants/client.py` & `hvac-2.2.0/hvac/constants/client.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/constants/gcp.py` & `hvac-2.2.0/hvac/constants/gcp.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/constants/transit.py` & `hvac-2.2.0/hvac/constants/transit.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/exceptions.py` & `hvac-2.2.0/hvac/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,14 +45,22 @@
     pass
 
 
 class InvalidPath(VaultError):
     pass
 
 
+class UnsupportedOperation(VaultError):
+    pass
+
+
+class PreconditionFailed(VaultError):
+    pass
+
+
 class RateLimitExceeded(VaultError):
     pass
 
 
 class InternalServerError(VaultError):
     pass
```

### Comparing `hvac-2.1.0/hvac/utils.py` & `hvac-2.2.0/hvac/utils.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/hvac/v1/__init__.py` & `hvac-2.2.0/hvac/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/pyproject.toml` & `hvac-2.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hvac"
-version = "2.1.0"
+version = "2.2.0"
 description = "HashiCorp Vault API client"
 readme = "README.md"
 authors = [
     "Ian Unruh <ianunruh@gmail.com>",
     "Jeffrey Hogan <jeff.hogan1@gmail.com>",
 ]
 maintainers = [
@@ -75,15 +75,19 @@
 # when running doctests, the dev group is needed too
 [tool.poetry.group.docs.dependencies]
 m2r2 = "^0.3.3"
 Sphinx = "^7"
 sphinx-rtd-theme = "^2"
 autodocsumm = "^0.2"
 docutils = "^0.20"
-jinja2 = "<3.1.0"
+jinja2 = "<3.2.0"
+# setuptools is not needed for building the docs in RTD,
+# but it is needed for running the doctests as an
+# undeclared dependency of m2r2.
+# https://github.com/CrossNox/m2r2/issues/63
 setuptools = "^69"
 
 
 [tool.pytest.ini_options]
 addopts = "-n auto --dist worksteal"
 
 [tool.typos.default.extend-words]
```

### Comparing `hvac-2.1.0/tests/config_files/ca-cert.pem` & `hvac-2.2.0/tests/config_files/ca-cert.pem`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/config_files/ca-key.pem` & `hvac-2.2.0/tests/config_files/ca-key.pem`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/config_files/client-cert.pem` & `hvac-2.2.0/tests/config_files/client-cert.pem`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/config_files/client-key.pem` & `hvac-2.2.0/tests/config_files/client-key.pem`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/config_files/example.jwt.json` & `hvac-2.2.0/tests/config_files/example.jwt.json`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/config_files/identity_document.p7b` & `hvac-2.2.0/tests/config_files/identity_document.p7b`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/config_files/oidc_private.pem` & `hvac-2.2.0/tests/config_files/oidc_private.pem`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/config_files/pgp_key.asc.b64` & `hvac-2.2.0/tests/config_files/pgp_key.asc.b64`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/config_files/server-cert.csr` & `hvac-2.2.0/tests/config_files/server-cert.csr`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/config_files/server-cert.pem` & `hvac-2.2.0/tests/config_files/server-cert.pem`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/config_files/server-key.pem` & `hvac-2.2.0/tests/config_files/server-key.pem`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/config_files/ssh-key` & `hvac-2.2.0/tests/config_files/ssh-key`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/config_files/ssh-key.pub` & `hvac-2.2.0/tests/config_files/ssh-key.pub`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/doctest/__init__.py` & `hvac-2.2.0/tests/doctest/__init__.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/auth_methods/test_approle.py` & `hvac-2.2.0/tests/integration_tests/api/auth_methods/test_approle.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/auth_methods/test_azure.py` & `hvac-2.2.0/tests/integration_tests/api/auth_methods/test_azure.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/auth_methods/test_cert.py` & `hvac-2.2.0/tests/integration_tests/api/auth_methods/test_cert.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/auth_methods/test_gcp.py` & `hvac-2.2.0/tests/integration_tests/api/auth_methods/test_gcp.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/auth_methods/test_github.py` & `hvac-2.2.0/tests/integration_tests/api/auth_methods/test_github.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/auth_methods/test_jwt.py` & `hvac-2.2.0/tests/integration_tests/api/auth_methods/test_jwt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from unittest import TestCase
+from unittest import TestCase, skipIf
 
 from parameterized import param, parameterized
 
 from tests import utils
 from tests.utils.hvac_integration_test_case import HvacIntegrationTestCase
 
 
@@ -223,14 +223,24 @@
                 "success",
                 role_name="hvac-jwt",
                 allowed_redirect_uris=["{url}/jwt-test/oidc/callback"],
                 user_claim="sub",
             ),
         ]
     )
+    # skipIf must come after @parameterized
+    @skipIf(
+        utils.vault_version_eq("1.16.1"),
+        (
+            "Known issue with JWT\n"
+            "https://developer.hashicorp.com/vault/docs/upgrading/upgrade-to-1.16.x#error-configuring-the-jwt-auth-method\n"
+            "https://github.com/hashicorp/vault-plugin-auth-jwt/issues/294#issuecomment-2046107870\n"
+            "https://github.com/hashicorp/vault-plugin-auth-jwt/pull/290\n"
+        ),
+    )
     def test_jwt_login(self, label, role_name, allowed_redirect_uris, user_claim):
         issuer = self.client.url
         allowed_redirect_uris = [
             uri.format(url=self.client.url) for uri in allowed_redirect_uris
         ]
         if "%s/" % self.TEST_APPROLE_PATH not in self.client.sys.list_auth_methods():
             self.client.sys.enable_auth_method(
```

### Comparing `hvac-2.1.0/tests/integration_tests/api/auth_methods/test_kubernetes.py` & `hvac-2.2.0/tests/integration_tests/api/auth_methods/test_kubernetes.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/auth_methods/test_ldap.py` & `hvac-2.2.0/tests/integration_tests/api/auth_methods/test_ldap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import distutils.spawn
+import shutil
 import logging
 from unittest import TestCase, SkipTest
 
 from parameterized import parameterized, param
 
 from hvac import exceptions
 from tests import utils
@@ -13,15 +13,15 @@
 class TestLdap(HvacIntegrationTestCase, TestCase):
     TEST_LDAP_PATH = "test-ldap"
     ldap_server = None
 
     @classmethod
     def setUpClass(cls):
         # The mock LDAP server requires Java runtime
-        if not distutils.spawn.find_executable("java"):
+        if not shutil.which("java"):
             raise SkipTest("The mock LDAP server requires Java runtime")
 
         try:
             super().setUpClass()
             logging.getLogger("ldap_test").setLevel(logging.ERROR)
 
             cls.mock_server_port = utils.get_free_port()
```

### Comparing `hvac-2.1.0/tests/integration_tests/api/auth_methods/test_legacy_mfa.py` & `hvac-2.2.0/tests/integration_tests/api/auth_methods/test_legacy_mfa.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/auth_methods/test_oidc.py` & `hvac-2.2.0/tests/integration_tests/api/auth_methods/test_oidc.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/auth_methods/test_okta.py` & `hvac-2.2.0/tests/integration_tests/api/auth_methods/test_okta.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/auth_methods/test_token.py` & `hvac-2.2.0/tests/integration_tests/api/auth_methods/test_token.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_aws.py` & `hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_aws.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_azure.py` & `hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_azure.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_gcp.py` & `hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_gcp.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_identity.py` & `hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_identity.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_kv_v1.py` & `hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_kv_v1.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_kv_v2.py` & `hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_kv_v2.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_pki.py` & `hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_pki.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_ssh.py` & `hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_ssh.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_transform.py` & `hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_transform.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/secrets_engines/test_transit.py` & `hvac-2.2.0/tests/integration_tests/api/secrets_engines/test_transit.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_audit.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_audit.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_auth.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_auth.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_health.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_health.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_init.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_init.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_key.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_key.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_lease.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_lease.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_mount.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_mount.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_namespace.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_namespace.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_policies.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_policies.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_policy.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_policy.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_quota.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_quota.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_seal.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_seal.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/api/system_backend/test_wrapping.py` & `hvac-2.2.0/tests/integration_tests/api/system_backend/test_wrapping.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/v1/test_approle.py` & `hvac-2.2.0/tests/integration_tests/v1/test_approle.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/v1/test_integration.py` & `hvac-2.2.0/tests/integration_tests/v1/test_integration.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/integration_tests/v1/test_system_backend.py` & `hvac-2.2.0/tests/integration_tests/v1/test_system_backend.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/scripts/generate_test_cert.sh` & `hvac-2.2.0/tests/scripts/generate_test_cert.sh`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/auth_methods/test_approle.py` & `hvac-2.2.0/tests/unit_tests/api/auth_methods/test_approle.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/auth_methods/test_azure.py` & `hvac-2.2.0/tests/unit_tests/api/auth_methods/test_azure.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/auth_methods/test_gcp.py` & `hvac-2.2.0/tests/unit_tests/api/auth_methods/test_gcp.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/auth_methods/test_github.py` & `hvac-2.2.0/tests/unit_tests/api/auth_methods/test_github.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/auth_methods/test_jwt.py` & `hvac-2.2.0/tests/unit_tests/api/auth_methods/test_jwt.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/auth_methods/test_kubernetes.py` & `hvac-2.2.0/tests/unit_tests/api/auth_methods/test_kubernetes.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/auth_methods/test_ldap.py` & `hvac-2.2.0/tests/unit_tests/api/auth_methods/test_ldap.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/auth_methods/test_legacy_mfa.py` & `hvac-2.2.0/tests/unit_tests/api/auth_methods/test_legacy_mfa.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/auth_methods/test_okta.py` & `hvac-2.2.0/tests/unit_tests/api/auth_methods/test_okta.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/auth_methods/test_token.py` & `hvac-2.2.0/tests/unit_tests/api/auth_methods/test_token.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/secrets_engines/test_aws.py` & `hvac-2.2.0/tests/unit_tests/api/secrets_engines/test_aws.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/secrets_engines/test_azure.py` & `hvac-2.2.0/tests/unit_tests/api/secrets_engines/test_azure.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/secrets_engines/test_database.py` & `hvac-2.2.0/tests/unit_tests/api/secrets_engines/test_database.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/secrets_engines/test_gcp.py` & `hvac-2.2.0/tests/unit_tests/api/secrets_engines/test_gcp.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/secrets_engines/test_kv.py` & `hvac-2.2.0/tests/unit_tests/api/secrets_engines/test_kv.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/system_backend/test_init.py` & `hvac-2.2.0/tests/unit_tests/api/system_backend/test_init.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/api/test_vault_api_category.py` & `hvac-2.2.0/tests/unit_tests/api/test_vault_api_category.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/conftest.py` & `hvac-2.2.0/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/test_adapters.py` & `hvac-2.2.0/tests/unit_tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/utils/test_utils.py` & `hvac-2.2.0/tests/unit_tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/v1/test_approle_routes.py` & `hvac-2.2.0/tests/unit_tests/v1/test_approle_routes.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/v1/test_auth_methods.py` & `hvac-2.2.0/tests/unit_tests/v1/test_auth_methods.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/v1/test_aws_ec2_methods.py` & `hvac-2.2.0/tests/unit_tests/v1/test_aws_ec2_methods.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/v1/test_aws_iam_methods.py` & `hvac-2.2.0/tests/unit_tests/v1/test_aws_iam_methods.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/v1/test_client.py` & `hvac-2.2.0/tests/unit_tests/v1/test_client.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/v1/test_gcp_methods.py` & `hvac-2.2.0/tests/unit_tests/v1/test_gcp_methods.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/unit_tests/v1/test_system_backend_methods.py` & `hvac-2.2.0/tests/unit_tests/v1/test_system_backend_methods.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/utils/__init__.py` & `hvac-2.2.0/tests/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     elif vault_version_ge("1.0.0"):
         test_otp = "ygs0vL8GIxu0AjRVEmJ5jLCVq8"
     else:
         test_otp = "RSMGkAqBH5WnVLrDTbZ+UQ=="
     return test_otp
 
 
-def create_client(url, use_env=False, **kwargs):
+def create_client(url, use_env=False, session=None, **kwargs):
     """Small helper to instantiate a :py:class:`hvac.v1.Client` class with the appropriate parameters for the test env.
 
     :param url: Vault address to configure the client with.
     :type url: str
     :param use_env: configure vault using environment variable
     :type use_env: bool
     :param kwargs: Dictionary of additional keyword arguments to pass through to the Client instance being created.
@@ -101,18 +101,25 @@
             with mock.patch("hvac.v1.VAULT_CLIENT_CERT", client_cert_path):
                 with mock.patch("hvac.v1.VAULT_CLIENT_KEY", client_key_path):
                     client = Client(
                         url=url,
                         **kwargs,
                     )
     else:
+        # Make sure self-signed certificates for testing will be accepted by either the default session
+        # or specific sessions used by individual tests
+        if session:
+            session.cert = (client_cert_path, client_key_path)
+            session.verify = server_cert_path
+
         client = Client(
             url=url,
             cert=(client_cert_path, client_key_path),
             verify=server_cert_path,
+            session=session,
             **kwargs,
         )
     return client
 
 
 class PortGetter:
     _entered: bool = False
```

### Comparing `hvac-2.1.0/tests/utils/hvac_integration_test_case.py` & `hvac-2.2.0/tests/utils/hvac_integration_test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 import logging
 import re
 import time
 
 from tests.utils import get_config_file_path, create_client, is_enterprise
 from tests.utils.server_manager import ServerManager
-import distutils.spawn
+import shutil
 from hvac import Client
 
 
 class HvacIntegrationTestCase:
     """Base class intended to be used by all hvac integration test cases."""
 
     manager: ServerManager = None
@@ -19,15 +19,15 @@
     server_retry_count: int = 2  # num retries not total tries
     server_retry_delay_seconds: float = 0.1
 
     @classmethod
     def setUpClass(cls):
         """Use the ServerManager class to launch a vault server process."""
         config_paths = [get_config_file_path("vault-tls.hcl")]
-        if distutils.spawn.find_executable("consul") is None and cls.enable_vault_ha:
+        if shutil.which("consul") is None and cls.enable_vault_ha:
             logging.warning(
                 "Unable to run Vault in HA mode, consul binary not found in path."
             )
             cls.enable_vault_ha = False
         if is_enterprise():
             # TODO: figure out why this bit isn't working
             logging.warning(
```

### Comparing `hvac-2.1.0/tests/utils/mock_github_request_handler.py` & `hvac-2.2.0/tests/utils/mock_github_request_handler.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/utils/mock_ldap_server.py` & `hvac-2.2.0/tests/utils/mock_ldap_server.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/utils/mock_oauth_provider/app.py` & `hvac-2.2.0/tests/utils/mock_oauth_provider/app.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/utils/mock_oauth_provider/mock_oauth_provider.py` & `hvac-2.2.0/tests/utils/mock_oauth_provider/mock_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/utils/mock_oauth_provider/models.py` & `hvac-2.2.0/tests/utils/mock_oauth_provider/models.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/utils/mock_oauth_provider/oauth2.py` & `hvac-2.2.0/tests/utils/mock_oauth_provider/oauth2.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/utils/mock_oauth_provider/routes.py` & `hvac-2.2.0/tests/utils/mock_oauth_provider/routes.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/utils/mock_okta_request_handler.py` & `hvac-2.2.0/tests/utils/mock_okta_request_handler.py`

 * *Files identical despite different names*

### Comparing `hvac-2.1.0/tests/utils/server_manager.py` & `hvac-2.2.0/tests/utils/server_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 import os
 import subprocess
 import time
 import requests
 import hcl
 import typing as t
 
-import distutils.spawn
+import shutil
 from unittest import SkipTest
 from tests.utils import (
     get_config_file_path,
     load_config_file,
     create_client,
     PortGetter,
 )
 
 from hvac.v1 import Client
 
+from requests.adapters import HTTPAdapter
+from urllib3.util import Retry
+
 logger = logging.getLogger(__name__)
 
 
 class TestProcessInfo:
     name: str
     process: subprocess.Popen
     extra: t.List[str]
@@ -133,15 +136,15 @@
             }
         self.start_vault(consul_config=consul_config)
 
     def start_vault(
         self, *, consul_config: dict = None, attempt=1, max_attempts=3, delay_s=1
     ):
         """Launch the vault server process and wait until its online and ready."""
-        if distutils.spawn.find_executable("vault") is None:
+        if shutil.which("vault") is None:
             raise SkipTest("Vault executable not found")
 
         with PortGetter() as g:
             self.active_config_paths = [
                 self.patch_config_port(
                     config_path,
                     port_getter=g.get_port,
@@ -221,15 +224,15 @@
                             stderr=stderr,
                         )
                     )
 
     def start_consul(
         self,
     ) -> str:
-        if distutils.spawn.find_executable("consul") is None:
+        if shutil.which("consul") is None:
             raise SkipTest("Consul executable not found")
 
         with PortGetter() as g:
             http_addr, http_port = g.get_port()
             _, server_port = g.get_port(address=http_addr)
             _, serf_lan_port = g.get_port(address=http_addr)
             _, serf_wan_port = g.get_port(address=http_addr)
@@ -373,9 +376,18 @@
             vault_addresses.append(self.get_config_vault_address(config_path))
         return vault_addresses
 
     def unseal(self):
         """Unseal the vault server process."""
         vault_addresses = self.get_active_vault_addresses()
         for vault_address in vault_addresses:
-            client = create_client(url=vault_address)
+            # At this point, the vault server may not be ready yet, resulting in "Connection refused"
+            # failures for requests. Let's retry multiple times before giving up.
+            adapter = HTTPAdapter(
+                max_retries=Retry(total=3, connect=3, backoff_factor=0.1)
+            )
+            session = requests.Session()
+            session.mount("http://", adapter)
+            session.mount("https://", adapter)
+
+            client = create_client(url=vault_address, session=session)
             client.sys.submit_unseal_keys(self.keys)
```

### Comparing `hvac-2.1.0/PKG-INFO` & `hvac-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hvac
-Version: 2.1.0
+Version: 2.2.0
 Summary: HashiCorp Vault API client
 Home-page: https://github.com/hvac/hvac
 License: Apache-2.0
 Keywords: hashicorp,vault
 Author: Ian Unruh
 Author-email: ianunruh@gmail.com
 Maintainer: Brian Scholer
```

