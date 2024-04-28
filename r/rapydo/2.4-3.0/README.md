# Comparing `tmp/rapydo-2.4.tar.gz` & `tmp/rapydo-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapydo-2.4.tar", last modified: Thu Dec  8 14:55:15 2022, max compression
+gzip compressed data, was "rapydo-3.0.tar", last modified: Sun Apr 28 07:06:25 2024, max compression
```

## Comparing `rapydo-2.4.tar` & `rapydo-3.0.tar`

### file list

```diff
@@ -1,180 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.841380 rapydo-2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2022-12-08 14:55:04.000000 rapydo-2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-08 14:55:04.000000 rapydo-2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2022-12-08 14:55:15.841380 rapydo-2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:04.000000 rapydo-2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-08 14:55:04.000000 rapydo-2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.821380 rapydo-2.4/controller/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2022-12-08 14:55:04.000000 rapydo-2.4/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2022-12-08 14:55:04.000000 rapydo-2.4/controller/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42329 2022-12-08 14:55:04.000000 rapydo-2.4/controller/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.825380 rapydo-2.4/controller/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.825380 rapydo-2.4/controller/commands/backup_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/backup_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/backup_modules/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/backup_modules/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/backup_modules/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/backup_modules/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.825380 rapydo-2.4/controller/commands/compose/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/compose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/compose/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/compose/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/compose/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/compose/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9805 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12892 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.829380 rapydo-2.4/controller/commands/password_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/password_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/password_modules/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/password_modules/flower.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/password_modules/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/password_modules/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/password_modules/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/password_modules/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/password_modules/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/reload.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/restore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.829380 rapydo-2.4/controller/commands/restore_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/restore_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/restore_modules/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/restore_modules/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/restore_modules/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/restore_modules/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/start.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.829380 rapydo-2.4/controller/commands/swarm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/swarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/swarm/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/swarm/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/swarm/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/swarm/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/swarm/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/swarm/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.829380 rapydo-2.4/controller/commands/tuning_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/tuning_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/tuning_modules/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/tuning_modules/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/tuning_modules/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2022-12-08 14:55:04.000000 rapydo-2.4/controller/commands/volatile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.833380 rapydo-2.4/controller/confs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-08 14:55:04.000000 rapydo-2.4/controller/confs/angular-development.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2022-12-08 14:55:04.000000 rapydo-2.4/controller/confs/angular.yml
--rw-r--r--   0 runner    (1001) docker     (123)    37841 2022-12-08 14:55:04.000000 rapydo-2.4/controller/confs/backend.yml
--rw-r--r--   0 runner    (1001) docker     (123)      397 2022-12-08 14:55:04.000000 rapydo-2.4/controller/confs/development.yml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-08 14:55:04.000000 rapydo-2.4/controller/confs/production.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14459 2022-12-08 14:55:04.000000 rapydo-2.4/controller/confs/projects_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2022-12-08 14:55:04.000000 rapydo-2.4/controller/confs/projects_prod_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      585 2022-12-08 14:55:04.000000 rapydo-2.4/controller/confs/swarm_angular_prod_options.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2022-12-08 14:55:04.000000 rapydo-2.4/controller/confs/swarm_options.yml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-08 14:55:04.000000 rapydo-2.4/controller/confs/volumes_local.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2022-12-08 14:55:04.000000 rapydo-2.4/controller/confs/volumes_nfs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.833380 rapydo-2.4/controller/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-08 14:55:04.000000 rapydo-2.4/controller/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2022-12-08 14:55:04.000000 rapydo-2.4/controller/deploy/builds.py
--rw-r--r--   0 runner    (1001) docker     (123)    15403 2022-12-08 14:55:04.000000 rapydo-2.4/controller/deploy/compose_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12012 2022-12-08 14:55:04.000000 rapydo-2.4/controller/deploy/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2022-12-08 14:55:04.000000 rapydo-2.4/controller/deploy/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2022-12-08 14:55:04.000000 rapydo-2.4/controller/deploy/swarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2022-12-08 14:55:04.000000 rapydo-2.4/controller/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    18186 2022-12-08 14:55:04.000000 rapydo-2.4/controller/project.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-08 14:55:04.000000 rapydo-2.4/controller/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.837381 rapydo-2.4/controller/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      270 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/activate_account.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      981 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/blocked_credentials.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      272 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/codecov.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/codeql-analysis.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/commons.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      815 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/component_template.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      654 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/component_template.ts.j2
--rw-r--r--   0 runner    (1001) docker     (123)      973 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/component_test_template.spec.ts.j2
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/custom.footer.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      734 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/custom.footer.ts.j2
--rw-r--r--   0 runner    (1001) docker     (123)      993 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/custom.module.ts.j2
--rw-r--r--   0 runner    (1001) docker     (123)      269 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/custom.navbar.brand.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      550 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/custom.navbar.links.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      897 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/custom.navbar.ts.j2
--rw-r--r--   0 runner    (1001) docker     (123)      144 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/custom.profile.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      342 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/custom.profile.ts.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/customization.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/customization.ts.j2
--rw-r--r--   0 runner    (1001) docker     (123)      918 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/cypress_template.spec.ts.j2
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/development.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/email_header.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/endpoint_template.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/endpoint_test_template.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/flake8.j2
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/gitattributes.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/github_actions-backend.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/github_actions-cypress.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/github_actions-frontend.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      502 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/github_actions-mypy.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/gitignore.j2
--rw-r--r--   0 runner    (1001) docker     (123)      605 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/initialization.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/neo4j.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      462 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/new_credentials.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/package.json.j2
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/prettierignore.j2
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/production.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/project_configuration.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/projectrc.j2
--rw-r--r--   0 runner    (1001) docker     (123)      592 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/pyproject.toml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/reset_password.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/semgrep-analysis.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      781 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/service_template.ts.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/sink.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/sink.ts.j2
--rw-r--r--   0 runner    (1001) docker     (123)      277 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)      307 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/sqlalchemy.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/style.scss.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/task_template.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      431 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/types.ts.j2
--rw-r--r--   0 runner    (1001) docker     (123)      458 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/update_credentials.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templates/variables.scss.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2022-12-08 14:55:04.000000 rapydo-2.4/controller/templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.841380 rapydo-2.4/controller/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-08 14:55:04.000000 rapydo-2.4/controller/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24589 2022-12-08 14:55:04.000000 rapydo-2.4/controller/utilities/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11797 2022-12-08 14:55:04.000000 rapydo-2.4/controller/utilities/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2022-12-08 14:55:04.000000 rapydo-2.4/controller/utilities/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2022-12-08 14:55:04.000000 rapydo-2.4/controller/utilities/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2022-12-08 14:55:04.000000 rapydo-2.4/controller/utilities/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.841380 rapydo-2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2022-12-08 14:55:04.000000 rapydo-2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2022-12-08 14:55:04.000000 rapydo-2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 14:55:15.841380 rapydo-2.4/rapydo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2022-12-08 14:55:15.000000 rapydo-2.4/rapydo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2022-12-08 14:55:15.000000 rapydo-2.4/rapydo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 14:55:15.000000 rapydo-2.4/rapydo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-08 14:55:15.000000 rapydo-2.4/rapydo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2022-12-08 14:55:15.000000 rapydo-2.4/rapydo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-08 14:55:15.000000 rapydo-2.4/rapydo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 14:55:15.841380 rapydo-2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.641395 rapydo-3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-28 07:06:18.000000 rapydo-3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-28 07:06:18.000000 rapydo-3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-28 07:06:25.641395 rapydo-3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:18.000000 rapydo-3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-28 07:06:18.000000 rapydo-3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.617395 rapydo-3.0/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-28 07:06:18.000000 rapydo-3.0/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-28 07:06:18.000000 rapydo-3.0/controller/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43916 2024-04-28 07:06:18.000000 rapydo-3.0/controller/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.613396 rapydo-3.0/controller/builds/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.617395 rapydo-3.0/controller/builds/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-28 07:06:18.000000 rapydo-3.0/controller/builds/backend/gunicorn_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.617395 rapydo-3.0/controller/builds/backend-legacy310/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-28 07:06:18.000000 rapydo-3.0/controller/builds/backend-legacy310/gunicorn_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.617395 rapydo-3.0/controller/builds/backend-legacy39/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-28 07:06:18.000000 rapydo-3.0/controller/builds/backend-legacy39/gunicorn_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.621395 rapydo-3.0/controller/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.621395 rapydo-3.0/controller/commands/backup_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/backup_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/backup_modules/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/backup_modules/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/backup_modules/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/backup_modules/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.625395 rapydo-3.0/controller/commands/compose/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/compose/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/compose/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/compose/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/compose/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.625395 rapydo-3.0/controller/commands/password_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/password_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/password_modules/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/password_modules/flower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/password_modules/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/password_modules/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/password_modules/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/password_modules/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/password_modules/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/restore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.625395 rapydo-3.0/controller/commands/restore_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/restore_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/restore_modules/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/restore_modules/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/restore_modules/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/restore_modules/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.625395 rapydo-3.0/controller/commands/swarm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/swarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/swarm/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/swarm/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/swarm/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/swarm/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/swarm/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/swarm/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.625395 rapydo-3.0/controller/commands/tuning_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/tuning_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/tuning_modules/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/tuning_modules/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/tuning_modules/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-28 07:06:18.000000 rapydo-3.0/controller/commands/volatile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.629395 rapydo-3.0/controller/confs/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 07:06:18.000000 rapydo-3.0/controller/confs/angular-development.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-28 07:06:18.000000 rapydo-3.0/controller/confs/angular.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    38274 2024-04-28 07:06:18.000000 rapydo-3.0/controller/confs/backend.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-28 07:06:18.000000 rapydo-3.0/controller/confs/development.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-28 07:06:18.000000 rapydo-3.0/controller/confs/production.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14321 2024-04-28 07:06:18.000000 rapydo-3.0/controller/confs/projects_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-28 07:06:18.000000 rapydo-3.0/controller/confs/projects_prod_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-28 07:06:18.000000 rapydo-3.0/controller/confs/swarm_angular_prod_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-28 07:06:18.000000 rapydo-3.0/controller/confs/swarm_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-28 07:06:18.000000 rapydo-3.0/controller/confs/volumes_local.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-28 07:06:18.000000 rapydo-3.0/controller/confs/volumes_nfs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.629395 rapydo-3.0/controller/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-28 07:06:18.000000 rapydo-3.0/controller/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-28 07:06:18.000000 rapydo-3.0/controller/deploy/builds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15873 2024-04-28 07:06:18.000000 rapydo-3.0/controller/deploy/compose_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-04-28 07:06:18.000000 rapydo-3.0/controller/deploy/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-28 07:06:18.000000 rapydo-3.0/controller/deploy/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-04-28 07:06:18.000000 rapydo-3.0/controller/deploy/swarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12593 2024-04-28 07:06:18.000000 rapydo-3.0/controller/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-04-28 07:06:18.000000 rapydo-3.0/controller/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-28 07:06:18.000000 rapydo-3.0/controller/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.637395 rapydo-3.0/controller/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/activate_account.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/blocked_credentials.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/codecov.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/codeql-analysis.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/commons.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/component_template.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/component_template.ts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/component_test_template.spec.ts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/custom.footer.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/custom.footer.ts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/custom.module.ts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/custom.navbar.brand.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/custom.navbar.controls.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/custom.navbar.links.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/custom.navbar.ts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/custom.profile.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/custom.profile.ts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/customization.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/customization.ts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/cypress_template.spec.ts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/development.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/email_header.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/endpoint_template.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/endpoint_test_template.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/flake8.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/gitattributes.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/github_actions-backend.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/github_actions-cypress.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/github_actions-frontend.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/github_actions-mypy.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/gitignore.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/initialization.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/neo4j.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/new_credentials.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/package.json.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/prettierignore.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/production.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/project_configuration.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/projectrc.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/pyproject.toml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/reset_password.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/semgrep-analysis.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/service_template.ts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/sink.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/sink.ts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/sqlalchemy.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/style.scss.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/task_template.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/types.ts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/update_credentials.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templates/variables.scss.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-28 07:06:18.000000 rapydo-3.0/controller/templating.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.641395 rapydo-3.0/controller/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-28 07:06:18.000000 rapydo-3.0/controller/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23822 2024-04-28 07:06:18.000000 rapydo-3.0/controller/utilities/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-04-28 07:06:18.000000 rapydo-3.0/controller/utilities/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-28 07:06:18.000000 rapydo-3.0/controller/utilities/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-28 07:06:18.000000 rapydo-3.0/controller/utilities/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-28 07:06:18.000000 rapydo-3.0/controller/utilities/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.641395 rapydo-3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-28 07:06:18.000000 rapydo-3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-28 07:06:18.000000 rapydo-3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.641395 rapydo-3.0/rapydo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-28 07:06:25.000000 rapydo-3.0/rapydo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-04-28 07:06:25.000000 rapydo-3.0/rapydo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 07:06:25.000000 rapydo-3.0/rapydo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 07:06:25.000000 rapydo-3.0/rapydo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-28 07:06:25.000000 rapydo-3.0/rapydo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-28 07:06:25.000000 rapydo-3.0/rapydo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-28 07:06:18.000000 rapydo-3.0/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-28 07:06:18.000000 rapydo-3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-28 07:06:18.000000 rapydo-3.0/requirements.types.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 07:06:25.641395 rapydo-3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.613396 rapydo-3.0/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:06:25.641395 rapydo-3.0/stubs/glom/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-28 07:06:18.000000 rapydo-3.0/stubs/glom/__init__.pyi
```

### Comparing `rapydo-2.4/LICENSE` & `rapydo-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/__init__.py` & `rapydo-3.0/controller/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from colorama import Fore as colors  # type: ignore
 from loguru import logger as log
 from python_on_whales.components.compose.models import ComposeConfigService
 
 ComposeServices = Dict[str, ComposeConfigService]
 
-__version__ = "2.4"
+__version__ = "3.0"
 
 __all__ = [colors]
 
 
 COMPOSE_ENVIRONMENT_FILE = Path(".env")
 SUBMODULES_DIR = Path("submodules")
 PROJECT_DIR = Path("projects")
```

### Comparing `rapydo-2.4/controller/__main__.py` & `rapydo-3.0/controller/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 def main() -> None:
-
     # All imports moved here to prevent to slow down the import of main
     import warnings
 
     from controller import TESTING, log, print_and_exit
 
     if TESTING:
         warnings.filterwarnings("error")
```

### Comparing `rapydo-2.4/controller/app.py` & `rapydo-3.0/controller/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Main Application and Configuration module
 """
+
 import enum
 import json
 import os
 import shutil
 import sys
 import time
 import warnings
@@ -279,15 +280,14 @@
         "-v",
         help="Print version information and quit",
         show_default=False,
         callback=version_callback,
         is_eager=True,
     ),
 ) -> None:
-
     # This is needed because during tests both Application and Configuration
     # are persistent and after a run (i.e. after starting the registry)
     # FORCE_COMPOSE_ENGINE remains enabled
     # It would not be needed during the normal use of the controller
     Configuration.FORCE_COMPOSE_ENGINE = False
 
     Configuration.set_action(ctx.invoked_subcommand, ctx.params)
@@ -301,15 +301,14 @@
     Configuration.production = production
     Configuration.testing = testing
     Configuration.project = project
     Configuration.hostname = hostname
     Configuration.remote_engine = remote_engine
     Configuration.environment = {}
     for e in environment:
-
         if "=" not in e:
             print_and_exit("Invalid enviroment, missing value in {}", e)
 
         key, value = e.split("=")
         Configuration.environment[key] = value
 
     if stack:
@@ -344,15 +343,14 @@
         all_services = list(compose_config.keys())
         self.custom_services: List[str] = [
             s for s in all_services if s not in core_services
         ]
 
 
 class Application:
-
     # Typer app
     # Register callback with CLI options and basic initialization/checks
     app = typer.Typer(
         callback=controller_cli_options,
         context_settings={"help_option_names": ["--help", "-h"]},
     )
     # controller app
@@ -362,15 +360,14 @@
     gits: Dict[str, GitRepo] = {}
     env: Dict[str, EnvType] = {}
 
     base_services: ComposeServices
     compose_config: ComposeServices
 
     def __init__(self) -> None:
-
         Application.controller = self
 
         self.active_services: List[str] = []
         self.files: List[Path] = []
         self.base_files: List[Path] = []
         self.services = None
         self.enabled_services: List[str] = []
@@ -388,15 +385,14 @@
 
     @staticmethod
     def serialize_parameter(
         param: str,
         value: CommandParameter,
         IF: CommandParameter = True,
     ) -> Optional[str]:
-
         if isinstance(value, enum.Enum):
             value = value.value
 
         if IF and value is not None:
             if isinstance(value, bool):
                 return f"{param}"
             if isinstance(value, tuple) or isinstance(value, list):
@@ -409,15 +405,14 @@
             # Arguments ( => no param, only a value)
             return str(value)
 
         return None
 
     @staticmethod
     def print_command(*parameters: Optional[str]) -> None:
-
         pre_params = " ".join(
             [p for p in Configuration.parameters if p is not None]
         ).strip()
         post_params = " ".join([p for p in parameters if p is not None]).strip()
 
         if pre_params:
             pre_params = f"{pre_params} "
@@ -531,15 +526,14 @@
             compose_config=compose_config,
         )
 
         return None
 
     @staticmethod
     def load_projectrc() -> None:
-
         projectrc_yaml = cast(
             ProjectRCType,
             configuration.load_yaml_file(file=PROJECTRC, is_optional=True),
         )
 
         Configuration.host_configuration = projectrc_yaml.pop(
             "project_configuration", {}
@@ -549,15 +543,14 @@
         Configuration.swarm_mode = (
             Configuration.projectrc.get("swarm", False)
             or os.environ.get("SWARM_MODE", "0") == "1"
         )
 
     @staticmethod
     def check_installed_software() -> None:
-
         log.debug(
             "python version: {}.{}.{}",
             sys.version_info.major,
             sys.version_info.minor,
             sys.version_info.micro,
         )
 
@@ -588,15 +581,14 @@
         # in case of missing git GitPython will fail and this check will never executed
         # Packages.check_program("git")
 
     def read_specs(self, read_extended: bool = True) -> None:
         """Read project configuration"""
 
         try:
-
             confs = configuration.read_configuration(
                 default_file_path=CONFS_DIR,
                 base_project_path=Configuration.ABS_PROJECT_PATH,
                 projects_path=PROJECT_DIR,
                 submodules_path=SUBMODULES_DIR,
                 read_extended=read_extended,
                 production=Configuration.production,
@@ -645,15 +637,14 @@
                 "RAPyDo version not found in your project_configuration file"
             )
 
         Configuration.rapydo_version = str(Configuration.rapydo_version)
 
     @staticmethod
     def preliminary_version_check() -> None:
-
         specs = configuration.load_yaml_file(
             file=Configuration.ABS_PROJECT_PATH.joinpath(
                 configuration.PROJECT_CONF_FILENAME
             )
         )
 
         Application.verify_rapydo_version(
@@ -705,15 +696,14 @@
         except requests.ConnectionError:  # pragma: no cover
             print_and_exit("Internet connection is unavailable")
 
     @staticmethod
     def working_clone(
         name: str, repo: configuration.Submodule, from_path: Optional[Path] = None
     ) -> Optional[GitRepo]:
-
         # substitute values starting with '$$'
         myvars = {
             ANGULAR: Configuration.frontend == ANGULAR,
         }
 
         condition = repo.get("_if", "")
         if condition.startswith("$$"):
@@ -724,15 +714,14 @@
         default_version = (
             Configuration.rapydo_version
             if Configuration.rapydo_version
             else __version__
         )
 
         if from_path is not None:
-
             local_path = from_path.joinpath(name)
             if not local_path.exists():
                 print_and_exit("Submodule {} not found in {}", name, local_path)
 
             submodule_path = Path(SUBMODULES_DIR, name)
 
             if submodule_path.exists():
@@ -776,15 +765,14 @@
             repo = Application.working_clone(name, submodule, from_path=from_path)
             if repo:
                 Application.gits[name] = repo
 
     def get_compose_configuration(
         self, enabled_services: Optional[Iterable[str]] = None
     ) -> Tuple[ComposeServices, ComposeServices]:
-
         compose_files: List[Path] = []
 
         MODE = f"{Configuration.stack}.yml"
         customconf = Configuration.ABS_PROJECT_PATH.joinpath(CONTAINERS_YAML_DIRNAME)
         angular_loaded = False
 
         def add(p: Path, f: str) -> None:
@@ -843,19 +831,27 @@
         from controller.deploy.docker import Docker
 
         docker = Docker(
             compose_files=self.base_files, verify_swarm=not Configuration.initialize
         )
         base_services = docker.compose.get_config().services
 
+        if base_services is None:  # pragma: no cover
+            log.error("Got invalid compose base config")
+            base_services = {}
+
         docker = Docker(
             compose_files=self.files, verify_swarm=not Configuration.initialize
         )
         compose_config = docker.compose.get_config().services
 
+        if compose_config is None:  # pragma: no cover
+            log.error("Got invalid compose config")
+            compose_config = {}
+
         self.active_services = services.find_active(compose_config)
 
         self.enabled_services = services.get_services(
             Configuration.services_list or enabled_services,
             default=self.active_services,
         )
 
@@ -890,15 +886,14 @@
         if not self.files:
             log.debug("Created temporary default {} file", PROJECTRC)
             PROJECTRC.unlink()
         else:
             log.info("Created default {} file", PROJECTRC)
 
     def make_env(self) -> None:
-
         try:
             COMPOSE_ENVIRONMENT_FILE.unlink()
         except FileNotFoundError:
             pass
 
         Application.env = Configuration.specs.get("variables", {}).get("env", {})
 
@@ -966,15 +961,14 @@
             if env_value is None:
                 continue
             Application.env[e] = env_value
 
         Application.env.update(Configuration.environment)
 
         if Configuration.swarm_mode:
-
             if not Application.env.get("SWARM_MANAGER_ADDRESS"):
                 Application.env["SWARM_MANAGER_ADDRESS"] = system.get_local_ip(
                     Configuration.production
                 )
 
             if not Application.env.get("REGISTRY_HOST"):
                 Application.env["REGISTRY_HOST"] = Application.env[
@@ -992,36 +986,55 @@
             DEPLOY_ENGINE = "swarm"
 
         Application.env["DEPLOY_ENGINE"] = DEPLOY_ENGINE
 
         # Unfortunately this will only work after the creation of the network
         # i.e. will be fallen back to 127.0.0.1 the first time
         try:
-            DOCKER_SUBNET = docker.network.inspect(
+            docker_network = docker.network.inspect(
                 f"{Configuration.project}_{DEPLOY_ENGINE}_default"
-            ).ipam.config[0]["Subnet"]
+            )
+            if docker_network.ipam.config:
+                DOCKER_SUBNET = docker_network.ipam.config[0]["Subnet"]
+            else:
+                DOCKER_SUBNET = "127.0.0.1"
         # The first execution will fail and fallen back to localhost
         except DockerException:
             DOCKER_SUBNET = "127.0.0.1"
         Application.env["DOCKER_SUBNET"] = DOCKER_SUBNET
 
         FAIL2BAN_IPTABLES = "legacy"
         if str(Application.env["ACTIVATE_FAIL2BAN"]) == "1":
             iptables_version = Packages.get_bin_version("iptables", clean_output=False)
             nf_tables = iptables_version and "nf_tables" in iptables_version
             if nf_tables:
                 FAIL2BAN_IPTABLES = "nf_tables"
         Application.env["FAIL2BAN_IPTABLES"] = FAIL2BAN_IPTABLES
 
+        # Set Backend Python version
+        py_version = Application.env.get("BACKEND_PYTHON_VERSION", "v3.11")
+        py_values = configuration.BACKEND_PYTHON_VERSION_VALUES
+        if py_version == py_values.py39.value:
+            build_mode = "backend-legacy39"
+        elif py_version == py_values.py310.value:
+            build_mode = "backend-legacy310"
+        else:
+            build_mode = "backend"
+        Application.env["BACKEND_BUILD_MODE"] = build_mode
+
+        # TODO: replace with removeprefix
+        py_version = str(py_version).replace("v", "")
+        PYTHON_PATH = f"/usr/local/lib/python{py_version}/dist-packages"
+        Application.env["PYTHON_PATH"] = PYTHON_PATH
+
         configuration.validate_env(Application.env)
         log.info("Environment configuration is valid")
 
         with open(COMPOSE_ENVIRONMENT_FILE, "w+") as whandle:
             for key, value in sorted(Application.env.items()):
-
                 if value is None:
                     value = ""
                 else:
                     value = str(value)
                 if " " in value:
                     value = f"'{value}'"
 
@@ -1079,15 +1092,14 @@
             return values
         return [x for x in values if x.startswith(incomplete)]
 
     @staticmethod
     def check_placeholders_and_passwords(
         compose_services: ComposeServices, active_services: List[str]
     ) -> None:
-
         if not active_services:  # pragma: no cover
             print_and_exit(
                 """You have no active service
 \nSuggestion: to activate a top-level service edit your project_configuration
 and add the variable "ACTIVATE_DESIREDSERVICE: 1"
                 """
             )
@@ -1113,43 +1125,51 @@
             # As side effect, non-existing services are not blocked
             if service_name not in compose_services:
                 continue
 
             service = compose_services[service_name]
 
             if service:
+                if service.environment is None:
+                    log.error(
+                        "Invalid env format, cannot check placeholders and passwords"
+                    )
+                    continue
+                if isinstance(service.environment, list):  # pragma: no cover
+                    log.error(
+                        "Unsupported env format, cannot check placeholders and passwords"
+                    )
+                    continue
                 for key, value in service.environment.items():
                     if str(value) == PLACEHOLDER:
                         key = services.normalize_placeholder_variable(key)
                         missing.setdefault(key, set())
                         missing[key].add(service_name)
 
                     elif key.endswith("_PASSWORD") and value:
                         key = services.normalize_placeholder_variable(key)
-                        passwords.setdefault(key, value)
+                        passwords.setdefault(key, cast(str, value))
                         passwords_services.setdefault(key, set())
                         passwords_services[key].add(service_name)
 
         placeholders = []
         for variable, raw_services in missing.items():
-
             if variable in services.vars_to_services_mapping:
                 serv = {services.vars_to_services_mapping[variable]}
             else:
                 serv = raw_services
             active_serv = [s for s in serv if s in all_services]
 
             if active_serv:
                 placeholders.append([variable, ", ".join(active_serv)])
 
         MIN_PASSWORD_SCORE = int(
             Application.env.get("MIN_PASSWORD_SCORE", 2)  # type: ignore
         )
         for variable, raw_services in passwords_services.items():
-
             if variable in services.vars_to_services_mapping:
                 serv = {services.vars_to_services_mapping[variable]}
             else:
                 serv = raw_services
 
             active_serv = [s for s in serv if s in all_services]
             if active_serv:
@@ -1179,15 +1199,14 @@
 
             sys.exit(1)
 
         return None
 
     @staticmethod
     def git_update(ignore_submodule: List[str]) -> None:
-
         for name, gitobj in Application.gits.items():
             if name in ignore_submodule:
                 log.debug("Skipping update on {}", name)
                 continue
 
             if gitobj and not git.can_be_updated(name, gitobj):
                 print_and_exit("Can't continue with updates")
@@ -1210,15 +1229,14 @@
             if not installation_path:  # pragma: no cover
                 log.warning(
                     "Controller is not installed in editable mode, "
                     "rapydo is unable to update it"
                 )
 
             elif Application.gits["do"].working_dir:
-
                 if installation_path.is_symlink():
                     installation_path = installation_path.resolve()
 
                 do_dir = Path(Application.gits["do"].working_dir)
                 if do_dir.is_symlink():
                     do_dir = do_dir.resolve()
                     # This can be used starting from py39
@@ -1236,15 +1254,14 @@
                         do_dir,
                     )
             else:  # pragma: no cover
                 log.warning("Controller submodule folder can't be found")
 
     @staticmethod
     def git_checks(ignore_submodule: List[str]) -> None:
-
         for name, gitobj in Application.gits.items():
             if name in ignore_submodule:
                 log.debug("Skipping checks on {}", name)
                 continue
             if gitobj:
                 git.check_updates(name, gitobj)
                 git.check_unstaged(name, gitobj)
```

### Comparing `rapydo-2.4/controller/commands/__init__.py` & `rapydo-3.0/controller/commands/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 BACKUP_MODULES: Dict[str, ModuleType] = {}
 RESTORE_MODULES: Dict[str, ModuleType] = {}
 PASSWORD_MODULES: Dict[str, ModuleType] = {}
 TUNING_MODULES: Dict[str, ModuleType] = {}
 
 
 def load_module(path: Path) -> Dict[str, ModuleType]:
-
     # Initially it was:
     # for c in commands_folder.glob("[!_|.]*.py"):
     #     import_module(f"controller.commands.{c.stem}")
 
     loaded_modules: Dict[str, ModuleType] = {}
     if path.is_dir():
         for c in path.glob("[!_|.]*.py"):
@@ -32,15 +31,14 @@
                 spec.loader.exec_module(command)
                 loaded_modules[c.stem] = command
 
     return loaded_modules
 
 
 def load_commands(project: Optional[str]) -> None:
-
     # re-initialization needed for tests
     BACKUP_MODULES.clear()
     RESTORE_MODULES.clear()
     PASSWORD_MODULES.clear()
     TUNING_MODULES.clear()
 
     commands_folder = Path(__file__).resolve().parent
```

### Comparing `rapydo-2.4/controller/commands/add.py` & `rapydo-3.0/controller/commands/add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Add a new element to the project (endpoint, task, component, service, test workflow)
 
 """
+
 from enum import Enum
 from pathlib import Path
 from typing import Callable, List
 
 import typer
 from glom import glom
 
@@ -23,15 +24,14 @@
     integration_test = "integration_test"
     workflow = "workflow"
 
 
 def get_function(
     element: ElementTypes,
 ) -> Callable[[Project, str, List[str], str, bool, bool], None]:
-
     if element == "endpoint":
         return create_endpoint
 
     if element == "task":
         return create_task
 
     if element == "component":
@@ -65,15 +65,14 @@
     add_tests: bool = typer.Option(
         False,
         "--add-tests",
         help="Add tests files",
         show_default=False,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--add-tests", add_tests, IF=add_tests),
         Application.serialize_parameter("--force", force, IF=force),
         Application.serialize_parameter("", element_type),
         Application.serialize_parameter("", name),
     )
 
@@ -101,15 +100,14 @@
     target_path: Path,
     name: str,
     services: List[str],
     auth: str,
     force: bool,
     project: str,
 ) -> None:
-
     if not force and target_path.exists():
         print_and_exit("{} already exists", target_path)
 
     template = templating.get_template(
         template_name,
         {"name": name, "services": services, "auth_service": auth, "project": project},
     )
@@ -376,15 +374,14 @@
     project_scaffold: Project,
     name: str,
     services: List[str],
     auth: str,
     force: bool,
     add_tests: bool,
 ) -> None:
-
     if add_tests:
         print_and_exit("Add integration_test does not support --add-tests flag")
 
     path = project_scaffold.p_path("frontend", "e2e")
 
     # Expected name is a route-like string, e.g. app/mypath/:my_id
 
@@ -417,15 +414,14 @@
     project_scaffold: Project,
     name: str,
     services: List[str],
     auth: str,
     force: bool,
     add_tests: bool,
 ) -> None:
-
     if add_tests:
         print_and_exit("Add workflow does not support --add-tests flag")
 
     workflows = ["backend", "frontend", "cypress", "mypy"]
     if name not in workflows:
         print_and_exit("Invalid workflow name, expected: {}", ", ".join(workflows))
```

### Comparing `rapydo-2.4/controller/commands/backup.py` & `rapydo-3.0/controller/commands/backup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Execute a backup of one service
 """
+
 import time
 from datetime import datetime
 from enum import Enum
 from typing import List
 
 import typer
 
@@ -68,15 +69,14 @@
     restart: List[str] = typer.Option(
         [],
         "--restart",
         help="Service to be restarted once completed the backup (multiple allowed)",
         shell_complete=Application.autocomplete_service,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--force", force, IF=force),
         Application.serialize_parameter("--max", max_backups, IF=max_backups),
         Application.serialize_parameter("--dry-run", dry_run, IF=dry_run),
         Application.serialize_parameter("--restart", restart, IF=restart),
         Application.serialize_parameter("", service.value),
     )
```

### Comparing `rapydo-2.4/controller/commands/backup_modules/neo4j.py` & `rapydo-3.0/controller/commands/backup_modules/neo4j.py`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/commands/backup_modules/postgres.py` & `rapydo-3.0/controller/commands/backup_modules/postgres.py`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/commands/backup_modules/rabbit.py` & `rapydo-3.0/controller/commands/backup_modules/rabbit.py`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/commands/backup_modules/redis.py` & `rapydo-3.0/controller/commands/backup_modules/redis.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 SERVICE_NAME = __name__
 
 
 def backup(
     container: Optional[Tuple[str, str]], now: datetime, force: bool, dry_run: bool
 ) -> None:
-
     docker = Docker()
 
     log.info("Starting backup on {}...", SERVICE_NAME)
 
     backup_path = f"/backup/{SERVICE_NAME}/{now}.tar.gz"
     # If running, ask redis to synchronize the database
     if container:
@@ -31,30 +30,30 @@
     # 3. Re-enable rewrites
     # Note: Assuming auto-aof-rewrite-percentage is set with its default value (100)
 
     if container:
         docker.exec_command(
             container,
             user="redis",
-            command="sh -c 'redis-cli --pass \"$REDIS_PASSWORD\" CONFIG SET auto-aof-rewrite-percentage 0'",
+            command="sh -c 'redis-cli --pass \"$REDIS_PASSWORD\" CONFIG SET auto-aof-rewrite-percentage 0'",  # noqa
         )
 
     command = f"tar -zcf {backup_path} -C /data dump.rdb appendonlydir"
     if not dry_run:
         log.info("Compressing the data files...")
         if container:
             docker.exec_command(container, user="redis", command=command)
         else:
             docker.compose.create_volatile_container(SERVICE_NAME, command=command)
 
     if container:
         docker.exec_command(
             container,
             user="redis",
-            command="sh -c 'redis-cli --pass \"$REDIS_PASSWORD\" CONFIG SET auto-aof-rewrite-percentage 100'",
+            command="sh -c 'redis-cli --pass \"$REDIS_PASSWORD\" CONFIG SET auto-aof-rewrite-percentage 100'",  # noqa
         )
 
     # Verify the gz integrity
     command = f"gzip -t {backup_path}"
     if not dry_run:
         log.info("Verifying the integrity of the backup file...")
         if container:
```

### Comparing `rapydo-2.4/controller/commands/build.py` & `rapydo-3.0/controller/commands/build.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Force building of one or more services docker images
 """
+
 from typing import List, Set
 
 import typer
 
 from controller import COMPOSE_FILE, RED, log, print_and_exit
 from controller.app import Application, Configuration
 from controller.deploy.builds import (
@@ -86,15 +87,14 @@
 
     core_builds = find_templates_build(Application.data.base_services)
     all_builds = find_templates_build(Application.data.compose_config)
 
     services_with_custom_builds: List[str] = []
     for image, build in all_builds.items():
         if image not in core_builds:
-
             # this is used to validate the target Dockerfile:
             if p := build.get("path"):
                 get_dockerfile_base_image(p, core_builds)
             services_with_custom_builds.extend(build["services"])
             images.add(image)
 
     targets: List[str] = []
```

### Comparing `rapydo-2.4/controller/commands/check.py` & `rapydo-3.0/controller/commands/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Verify if the current project is compliant to RAPyDo specs
 """
+
 import re
 from datetime import datetime
 from pathlib import Path
 from typing import List, Optional, Tuple
 
 import typer
 
@@ -45,15 +46,14 @@
         "--ignore-submodule",
         "-i",
         help="Ignore submodule",
         show_default=False,
         shell_complete=Application.autocomplete_submodule,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--no-git", no_git, IF=no_git),
         Application.serialize_parameter("--no-builds", no_builds, IF=no_builds),
         Application.serialize_parameter("--ignore-submodule", ignore_submodules),
     )
     Application.get_controller().controller_init()
 
@@ -84,15 +84,14 @@
         all_builds = find_templates_build(Application.data.compose_config)
         core_builds = find_templates_build(Application.data.base_services)
         overriding_builds = find_templates_override(
             Application.data.compose_config, core_builds
         )
 
         for image_tag, build in all_builds.items():
-
             services = build["services"]
             if not any(x in Application.data.active_services for x in services):
                 continue
 
             if image_tag not in dimages:
                 if image_tag in core_builds:
                     log.warning(
@@ -213,15 +212,14 @@
 def print_obsolete(
     image: str,
     date1: str,
     date2: str,
     service: Optional[str],
     from_img: Optional[str] = None,
 ) -> None:
-
     if service:
         if from_img:
             log.warning(
                 """Obsolete image {}: built on {} FROM {} that changed on {}
 Update it with: {command}""",
                 image,
                 date1,
@@ -252,24 +250,23 @@
         except ValueError:
             return False
 
 
 def build_is_obsolete(
     image_creation: datetime, path: Optional[Path]
 ) -> Tuple[Optional[str], Optional[str]]:
-
     if not path:  # pragma: no cover
         return None, None
 
     # compare dates between git and docker
-    btempl = Application.gits.get("build-templates")
+    do = Application.gits.get("do")
     vanilla = Application.gits.get("main")
 
-    if btempl and btempl.working_dir and is_relative_to(path, str(btempl.working_dir)):
-        git_repo = btempl
+    if do and do.working_dir and is_relative_to(path, str(do.working_dir)):
+        git_repo = do
     elif (
         vanilla
         and vanilla.working_dir
         and is_relative_to(path, str(vanilla.working_dir))
     ):
         git_repo = vanilla
     else:  # pragma: no cover
```

### Comparing `rapydo-2.4/controller/commands/compose/logs.py` & `rapydo-3.0/controller/commands/compose/logs.py`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/commands/compose/remove.py` & `rapydo-3.0/controller/commands/compose/remove.py`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/commands/compose/scale.py` & `rapydo-3.0/controller/commands/compose/scale.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from controller.deploy.docker import Docker
 
 
 @Application.app.command(help="Scale the number of containers for a service")
 def scale(
     scaling: str = typer.Argument(..., help="scale SERVICE to NUM_REPLICA")
 ) -> None:
-
     Application.print_command(Application.serialize_parameter("", scaling))
 
     Application.get_controller().controller_init()
 
     options = scaling.split("=")
     if len(options) != 2:
         scale_var = f"DEFAULT_SCALE_{scaling.upper()}"
```

### Comparing `rapydo-2.4/controller/commands/compose/stop.py` & `rapydo-3.0/controller/commands/compose/stop.py`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/commands/create.py` & `rapydo-3.0/controller/commands/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
     add_optionals: bool = typer.Option(
         False,
         "--add-optionals",
         help="Include all optionals files (html templates and customizers)",
         show_default=False,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--auth", auth),
         Application.serialize_parameter("--frontend", frontend),
         Application.serialize_parameter("--extend", extend, IF=extend),
         Application.serialize_parameter("--service", services),
         Application.serialize_parameter("--origin-url", origin_url, IF=origin_url),
         Application.serialize_parameter("--env", envs),
@@ -155,15 +154,14 @@
     envs: Optional[List[str]] = None,
     auto: bool = False,
     force: bool = False,
     force_current: bool = False,
     add_optionals: bool = False,
     path: Optional[Path] = None,
 ) -> None:
-
     project_scaffold = Project()
     enable_postgres = auth == "postgres" or "postgres" in services
     enable_neo4j = auth == "neo4j" or "neo4j" in services
     enable_rabbit = "rabbit" in services
     enable_redis = "redis" in services
     enable_celery = "celery" in services
     enable_flower = "flower" in services
@@ -188,15 +186,14 @@
                 "Use --current to force the creation here",
                 ", ".join(dirs[0:3]),  # add first 3 files/folders found
             )
 
     celery_broker = None  # Keep default value == REDIS
     celery_backend = None  # Keep default value == REDIS
     if enable_celery:
-
         if enable_rabbit:
             celery_broker = "RABBIT"
         else:
             celery_broker = "REDIS"
             enable_redis = True
 
         if enable_redis:
@@ -244,15 +241,14 @@
     if path:
         if path not in files:
             print_and_exit("Invalid path, cannot upgrade {}", path)
         else:
             files = [path]
 
     for p in files:
-
         template = templating.get_template(
             p.name,
             {
                 "version": __version__,
                 "project": project_name,
                 "auth_service": auth,
                 "enable_postgres": enable_postgres,
@@ -303,15 +299,14 @@
                 log.info("Project file already exists: {}", p)
             else:
                 # print(f"Missing file: {p}")
                 print_and_exit("File is missing: {}", p)
 
 
 def parse_env_variables(envs: Optional[List[str]]) -> Dict[str, str]:
-
     if not envs:
         return {}
 
     env_variables: Dict[str, str] = {}
     for env in envs:
         e = env.split("=")
         if len(e) != 2:
```

### Comparing `rapydo-2.4/controller/commands/dump.py` & `rapydo-3.0/controller/commands/dump.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Dump the current configuration into a docker compose YAML file
 """
+
 from controller import COMPOSE_FILE, log
 from controller.app import Application, Configuration
 from controller.deploy.docker import Docker
 
 
 @Application.app.command(help="Dump current config into docker compose YAML")
 def dump() -> None:
-
     Application.print_command()
     Application.get_controller().controller_init()
 
     docker = Docker()
     docker.compose.dump_config(
         Application.data.services, v1_compatibility=not Configuration.swarm_mode
     )
```

### Comparing `rapydo-2.4/controller/commands/init.py` & `rapydo-3.0/controller/commands/init.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Initialize the current RAPyDo project
 """
+
 from pathlib import Path
 
 import typer
 
 from controller import DATA_DIR, log, print_and_exit
 from controller.app import Application, Configuration
 from controller.deploy.docker import Docker
@@ -22,15 +23,14 @@
     ),
     submodules_path: Path = typer.Option(
         None,
         "--submodules-path",
         help="Link all submodules in an existing folder instead of download them",
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter(
             "--force", create_projectrc, IF=create_projectrc
         ),
         Application.serialize_parameter(
             "--submodules-path", submodules_path, IF=submodules_path
         ),
```

### Comparing `rapydo-2.4/controller/commands/install.py` & `rapydo-3.0/controller/commands/install.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Install the specified version of RAPyDO or docker, compose, buildx
 """
+
 import typer
 
 from controller import SUBMODULES_DIR, log, print_and_exit
 from controller.app import Application, Configuration
 from controller.packages import Packages
 from controller.utilities import git
 
@@ -15,15 +16,14 @@
     editable: bool = typer.Option(
         True,
         "--no-editable",
         help="Disable editable mode",
         show_default=False,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--no-editable", not editable, IF=not editable),
         Application.serialize_parameter("", version),
     )
 
     if version == "docker":
         Packages.install_docker()
@@ -46,20 +46,18 @@
     if editable:
         install_controller_from_folder(version)
     else:
         install_controller_from_git(version)
 
 
 def install_controller_from_folder(version: str) -> None:
-
     do_path = SUBMODULES_DIR.joinpath("do")
     try:
         Application.git_submodules()
     except SystemExit:
-
         log.info(
             """You asked to install rapydo {ver} in editable mode, but {p} is missing.
 
 You can force the installation by disabling the editable mode:
 
 rapydo install {ver} --no-editable
 
@@ -89,14 +87,13 @@
         print_and_exit("Invalid version")
 
     Packages.install(do_path, editable=True)
     log.info("Controller version {} installed from local folder", version)
 
 
 def install_controller_from_git(version: str) -> None:
-
     controller = f"git+https://github.com/rapydo/do.git@{version}"
 
     log.info("You asked to install rapydo {} from git", version)
 
     Packages.install(controller, editable=False)
     log.info("Controller version {} installed from git", version)
```

### Comparing `rapydo-2.4/controller/commands/interfaces.py` & `rapydo-3.0/controller/commands/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import typer
 
 from controller import log, print_and_exit
 from controller.app import Application
 
 
 class ServiceTypes(str, Enum):
-
     # New values
     swaggerui = "swaggerui"
     adminer = "adminer"
     flower = "flower"
 
     # Deprecated since 1.2
     sqlalchemy = "sqlalchemy"
@@ -38,20 +37,19 @@
     port: Optional[int] = typer.Option(
         None,
         "--port",
         "-p",
         help="port to be associated to the current service interface",
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--detach", detach, IF=detach),
         Application.serialize_parameter("--port", port, IF=port),
         Application.serialize_parameter("", service),
     )
     # Deprecated since 1.2
     if service.value == "sqlalchemy":
         log.warning("Deprecated interface sqlalchemy, use adminer instead")
         return None
 
     # Deprecated since 2.1
-    print_and_exit("Interfaces command is replaced by rapydo run {}", service)
+    print_and_exit("Interfaces command is replaced by rapydo run {}", service.value)
```

### Comparing `rapydo-2.4/controller/commands/list.py` & `rapydo-3.0/controller/commands/list.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,19 +45,21 @@
         headers = ["Name", "Image", "Status", "Path"]
 
         docker = Docker()
         services_status = docker.get_services_status(Configuration.project)
         for name, service in Application.data.compose_config.items():
             if name in Application.data.active_services:
                 image = service.image
+                if image is None:  # pragma: no cover
+                    image = "N/A"
                 build = service.build
 
                 status = services_status.get(name, "N/A")
 
-                if build:
+                if build and build.context:
                     build_path = str(build.context.relative_to(os.getcwd()))
                 else:
                     build_path = ""
 
                 table.append([name, image, status, build_path])
 
     if element_type == ElementTypes.submodules:
```

### Comparing `rapydo-2.4/controller/commands/password.py` & `rapydo-3.0/controller/commands/password.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Manage services passwords
 """
+
 import re
 from datetime import date, datetime, timedelta
 from enum import Enum
 from typing import Dict, List, Optional, Tuple, cast
 
 import typer
 from zxcvbn import zxcvbn  # type: ignore
@@ -12,31 +13,27 @@
 from controller import PLACEHOLDER, PROJECTRC, REGISTRY, log, print_and_exit
 from controller.app import Application, Configuration
 from controller.commands import PASSWORD_MODULES
 from controller.deploy.docker import Docker
 from controller.templating import Templating, get_strong_password
 from controller.utilities.tables import print_table
 
-# make this configurable
-PASSWORD_EXPIRATION = 90
-
 UPDATE_LABEL = "updated on"
 
 
 # Enum() expects a string, tuple, list or dict literal as the second argument
 # https://github.com/python/mypy/issues/5317
 SupportedServices = Enum(  # type: ignore
     "SupportedServices", {name: name for name in sorted(PASSWORD_MODULES.keys())}
 )
 
 
 # Note: can't directly extract yaml with comments because it is not supported
 # https://github.com/yaml/pyyaml/issues/90
 def parse_projectrc() -> Dict[str, datetime]:
-
     if not PROJECTRC.exists():
         return {}
 
     updates: Dict[str, datetime] = {}
     with open(PROJECTRC) as f:
         lines = f.readlines()
 
@@ -69,15 +66,14 @@
 
     return updates
 
 
 def get_projectrc_variables_indentation(projectrc: List[str]) -> int:
     env_indentation = 0
     for line in projectrc:
-
         # save the indentation level of the env block
         # it will be used to determine the variables indentation
         # if no further lines will be found
         if line.strip().startswith("env:"):
             env_indentation = line.index("env:")
             continue
 
@@ -100,15 +96,14 @@
     # Add 1 indentation level
     return int(3 * env_indentation / 2)
 
 
 # Note: can't directly use utilities in app.py because in this case we want to
 # maintain all values (not only templated variables) and we also want to keep comments
 def update_projectrc(variables: Dict[str, str]) -> None:
-
     today = date.today().strftime("%Y-%m-%d")
     annotation = f"# {UPDATE_LABEL} {today}"
     with open(PROJECTRC) as f:
         lines = f.readlines()
         append_additional_lines: List[str] = []
 
         blanks = get_projectrc_variables_indentation(lines)
@@ -150,14 +145,20 @@
 
 
 def get_expired_passwords() -> List[Tuple[str, datetime]]:
     expired_passwords: List[Tuple[str, datetime]] = []
 
     last_updates = parse_projectrc()
     now = datetime.now()
+    PASSWORD_EXPIRATION = int(
+        Application.env.get("PASSWORD_EXPIRATION_WARNING") or "180"
+    )
+
+    if PASSWORD_EXPIRATION == 0:
+        return expired_passwords
 
     for s in PASSWORD_MODULES:
         # This should never happens and can't be (easily) tested
         if s not in Application.data.base_services:  # pragma: no cover
             print_and_exit("Command misconfiguration, unknown {} service", s)
 
         if s != REGISTRY and s not in Application.data.active_services:
@@ -168,15 +169,14 @@
 
         module = PASSWORD_MODULES.get(s)
 
         if not module:  # pragma: no cover
             print_and_exit(f"{s} misconfiguration, module not found")
 
         for variable in module.PASSWORD_VARIABLES:
-
             if variable in last_updates:
                 change_date = last_updates.get(variable, datetime.fromtimestamp(0))
                 expiration_date = change_date + timedelta(days=PASSWORD_EXPIRATION)
                 if now > expiration_date:
                     expired_passwords.append(
                         (
                             variable,
@@ -204,27 +204,25 @@
     new_password: str = typer.Option(
         None,
         "--password",
         help="Force the given password",
         show_default=False,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--show", show, IF=show),
         Application.serialize_parameter("--random", random, IF=random),
         Application.serialize_parameter("--password", new_password, IF=new_password),
         Application.serialize_parameter("", service),
     )
 
     Application.get_controller().controller_init()
 
     # No service specified, only a summary will be reported
     if not service:
-
         if random:
             print_and_exit("--random flag is not supported without a service")
 
         if new_password:
             print_and_exit("--password option is not supported without a service")
 
         MIN_PASSWORD_SCORE = int(
@@ -247,32 +245,39 @@
                 continue
 
             module = PASSWORD_MODULES.get(s)
 
             if not module:  # pragma: no cover
                 print_and_exit(f"{s} misconfiguration, module not found")
 
+            PASSWORD_EXPIRATION = int(
+                Application.env.get("PASSWORD_EXPIRATION_WARNING") or "180"
+            )
             for variable in module.PASSWORD_VARIABLES:
-
                 password = Application.env.get(variable)
 
                 if password == PLACEHOLDER:
                     score = None
                 else:
                     result = zxcvbn(password)
                     score = result["score"]
 
-                if variable in last_updates:
-                    change_date = last_updates.get(variable, datetime.fromtimestamp(0))
-                    expiration_date = change_date + timedelta(days=PASSWORD_EXPIRATION)
-                    expired = now > expiration_date
-                    last_change = change_date.strftime("%Y-%m-%d")
-                else:
+                if variable not in last_updates:
                     expired = True
                     last_change = "N/A"
+                else:
+                    change_date = last_updates.get(variable, datetime.fromtimestamp(0))
+                    last_change = change_date.strftime("%Y-%m-%d")
+                    if PASSWORD_EXPIRATION == 0:
+                        expired = False
+                    else:
+                        expiration_date = change_date + timedelta(
+                            days=PASSWORD_EXPIRATION
+                        )
+                        expired = now > expiration_date
 
                 pass_line: List[str] = []
 
                 pass_line.append(s)
                 pass_line.append(variable)
 
                 if expired:
@@ -296,15 +301,14 @@
         if show:
             headers.append("PASSWORD")
 
         print_table(headers, table, table_title="Current passwords for active services")
 
     # In this case a service is asked to be updated
     else:
-
         module = PASSWORD_MODULES.get(service.value)
 
         if not module:  # pragma: no cover
             print_and_exit(f"{service.value} misconfiguration, module not found")
 
         if random:
             new_password = get_strong_password()
@@ -354,15 +358,14 @@
 
                 docker.client.container.remove(REGISTRY, force=True)
 
                 docker.compose.create_volatile_container(
                     REGISTRY, detach=True, publish=[(port, port)]
                 )
             elif Configuration.swarm_mode:
-
                 docker.compose.dump_config(Application.data.services)
                 docker.swarm.deploy()
 
             else:
                 docker.compose.start_containers(Application.data.services)
         else:
             log.info("{} was not running, restart is not needed", service.value)
```

### Comparing `rapydo-2.4/controller/commands/password_modules/backend.py` & `rapydo-3.0/controller/commands/password_modules/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 SERVICE_NAME = __name__
 PASSWORD_VARIABLES = ["AUTH_DEFAULT_PASSWORD"]
 IS_RUNNING_NEEDED = True
 
 
 def password(container: Tuple[str, str], old_password: str, new_password: str) -> None:
-
     docker = Docker()
     # restapi init need the env variable to be updated but can't be done after
     # the restart because it often fails because unable to re-connect to
     # services in a short time and some long sleep would be needed
     # => applied a workaround to be able to execute it before the restart
     docker = Docker()
     docker.exec_command(
```

### Comparing `rapydo-2.4/controller/commands/password_modules/neo4j.py` & `rapydo-3.0/controller/commands/password_modules/neo4j.py`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/commands/password_modules/postgres.py` & `rapydo-3.0/controller/commands/password_modules/postgres.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 SERVICE_NAME = __name__
 PASSWORD_VARIABLES = ["ALCHEMY_PASSWORD"]
 IS_RUNNING_NEEDED = True
 
 
 def password(container: Tuple[str, str], old_password: str, new_password: str) -> None:
-
     docker = Docker()
     # Interactively:
     # \password username
     # Non interactively:
     # https://ubiq.co/database-blog/how-to-change-user-password-in-postgresql
     user = Application.env.get("ALCHEMY_USER")
     db = Application.env.get("ALCHEMY_DB")
```

### Comparing `rapydo-2.4/controller/commands/password_modules/rabbit.py` & `rapydo-3.0/controller/commands/password_modules/rabbit.py`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/commands/pull.py` & `rapydo-3.0/controller/commands/pull.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Pull available images from the Docker Hub
 """
+
 from typing import List, Set
 
 import typer
 from glom import glom
 
 from controller import log
 from controller.app import Application, Configuration
@@ -27,15 +28,14 @@
     quiet: bool = typer.Option(
         False,
         "--quiet",
         help="Pull without printing progress information",
         show_default=False,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--all", include_all, IF=include_all),
         Application.serialize_parameter("--quiet", quiet, IF=quiet),
         Application.serialize_parameter("", services),
     )
 
     Application.get_controller().controller_init(services)
```

### Comparing `rapydo-2.4/controller/commands/reload.py` & `rapydo-3.0/controller/commands/reload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Reload services
 """
+
 from typing import List
 
 import typer
 from python_on_whales.utils import DockerException
 
 from controller import log, print_and_exit
 from controller.app import Application, Configuration
@@ -15,28 +16,26 @@
 def reload(
     services: List[str] = typer.Argument(
         None,
         help="Services to be reloaded",
         shell_complete=Application.autocomplete_service,
     ),
 ) -> None:
-
     Application.print_command(Application.serialize_parameter("", services))
 
     Application.get_controller().controller_init(services)
 
     docker = Docker()
     running_services = docker.get_running_services()
 
     if "frontend" in services and len(services) > 1:
         print_and_exit("Can't reload frontend and other services at once")
 
     reloaded = 0
     for service in Application.data.services:
-
         # Special case: frontend in production mode
         if Configuration.production and service == "frontend":
             # Only consider it if explicitly requested in input
             if "frontend" not in services:
                 log.debug("Can't reload the frontend if not explicitly requested")
             else:
                 log.info("Reloading frontend...")
```

### Comparing `rapydo-2.4/controller/commands/restart.py` & `rapydo-3.0/controller/commands/restart.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 [DEPRECATED] Restart modified running containers
 """
+
 import typer
 
 from controller import RED, print_and_exit
 from controller.app import Application
 
 
 @Application.app.command(help="[DEPRECATED] Restart modified running containers")
@@ -13,15 +14,14 @@
         False,
         "--force",
         "-f",
         help="Force services restart",
         show_default=False,
     ),
 ) -> None:
-
     # Deprecated since 2.2
 
     print_and_exit(
         "This command is no longer available "
         "\nIf you want to reload your services, use {} "
         "\nIf you want to recreated your containers, use {}",
         RED("rapydo reload"),
```

### Comparing `rapydo-2.4/controller/commands/restore.py` & `rapydo-3.0/controller/commands/restore.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Restore a backup of one service
 """
+
 import time
 from enum import Enum
 from typing import List, Optional
 
 import typer
 
 from controller import BACKUP_DIR, log, print_and_exit
@@ -44,15 +45,14 @@
     restart: List[str] = typer.Option(
         [],
         "--restart",
         help="Service to be restarted once completed the restore (multiple allowed)",
         shell_complete=Application.autocomplete_service,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--force", force, IF=force),
         Application.serialize_parameter("--restart", restart, IF=restart),
         Application.serialize_parameter("", service.value),
         Application.serialize_parameter("", backup_file),
     )
     Application.get_controller().controller_init()
```

### Comparing `rapydo-2.4/controller/commands/restore_modules/neo4j.py` & `rapydo-3.0/controller/commands/restore_modules/neo4j.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 SERVICE_NAME = __name__
 EXPECTED_EXT = ".dump"
 
 
 def restore(
     container: Optional[Tuple[str, str]], backup_file: str, force: bool
 ) -> None:
-
     if container and not force:
         print_and_exit(
             "Neo4j is running and the restore will temporary stop it. "
             "If you want to continue add --force flag"
         )
 
     docker = Docker()
```

### Comparing `rapydo-2.4/controller/commands/restore_modules/postgres.py` & `rapydo-3.0/controller/commands/restore_modules/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 SERVICE_NAME = __name__
 EXPECTED_EXT = ".sql.gz"
 
 
 def restore(
     container: Optional[Tuple[str, str]], backup_file: str, force: bool
 ) -> None:
-
     if not container:
         print_and_exit(
             "The restore procedure requires {} running, please start your stack",
             SERVICE_NAME,
         )
 
     docker = Docker()
```

### Comparing `rapydo-2.4/controller/commands/restore_modules/rabbit.py` & `rapydo-3.0/controller/commands/restore_modules/redis.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,31 +6,28 @@
 SERVICE_NAME = __name__
 EXPECTED_EXT = ".tar.gz"
 
 
 def restore(
     container: Optional[Tuple[str, str]], backup_file: str, force: bool
 ) -> None:
-
     if container and not force:
         print_and_exit(
-            "RabbitMQ is running and the restore will temporary stop it. "
+            "Redis is running and the restore will temporary stop it. "
             "If you want to continue add --force flag"
         )
 
     docker = Docker()
 
     if container:
         docker.remove(SERVICE_NAME)
 
     backup_path = f"/backup/{SERVICE_NAME}/{backup_file}"
-
-    command = f"tar -xf {backup_path} -C /var/lib/rabbitmq/"
-
     log.info("Starting restore on {}...", SERVICE_NAME)
 
+    command = f"tar -xf {backup_path} -C /data/"
     docker.compose.create_volatile_container(SERVICE_NAME, command=command)
 
     log.info("Restore from data{} completed", backup_path)
 
     if container:
         docker.start(SERVICE_NAME)
```

### Comparing `rapydo-2.4/controller/commands/restore_modules/redis.py` & `rapydo-3.0/controller/commands/restore_modules/rabbit.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 SERVICE_NAME = __name__
 EXPECTED_EXT = ".tar.gz"
 
 
 def restore(
     container: Optional[Tuple[str, str]], backup_file: str, force: bool
 ) -> None:
-
     if container and not force:
         print_and_exit(
-            "Redis is running and the restore will temporary stop it. "
+            "RabbitMQ is running and the restore will temporary stop it. "
             "If you want to continue add --force flag"
         )
 
     docker = Docker()
 
     if container:
         docker.remove(SERVICE_NAME)
 
     backup_path = f"/backup/{SERVICE_NAME}/{backup_file}"
+
+    command = f"tar -xf {backup_path} -C /var/lib/rabbitmq/"
+
     log.info("Starting restore on {}...", SERVICE_NAME)
 
-    command = f"tar -xf {backup_path} -C /data/"
     docker.compose.create_volatile_container(SERVICE_NAME, command=command)
 
     log.info("Restore from data{} completed", backup_path)
 
     if container:
         docker.start(SERVICE_NAME)
```

### Comparing `rapydo-2.4/controller/commands/run.py` & `rapydo-3.0/controller/commands/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Start a single container
 """
+
 import os
 from typing import List, Optional, Union
 
 import typer
 
 from controller import REGISTRY, log, print_and_exit
 from controller.app import Application, Configuration
@@ -18,27 +19,32 @@
     service: str, change_first_port: Optional[int]
 ) -> Optional[List[Union[PortMapping, PortRangeMapping]]]:
     service_config = Application.data.compose_config.get(service, None)
     if not service_config:
         print_and_exit("Services misconfiguration, can't find {}", service)
 
     ports: List[Union[PortMapping, PortRangeMapping]] = []
-    for p in service_config.ports:
-        port = change_first_port or p.published
-        target = p.target
-
-        # Remove it, because this option is to be applied only to the first port
-        change_first_port = None
-
-        ports.append(
-            (
-                port,
-                target,
+    if service_config.ports:
+        for p in service_config.ports:
+            port = change_first_port or p.published
+            target = p.target
+            if port is None or target is None:
+                log.warning(
+                    "Found null port on {}; port: {}, target: {}", service, port, target
+                )
+                continue
+            # Remove it, because this option is to be applied only to the first port
+            change_first_port = None
+
+            ports.append(
+                (
+                    port,
+                    target,
+                )
             )
-        )
 
     return ports
 
 
 # This command replaces volatile, interfaces and registry
 @Application.app.command(help="Start a single container")
 def run(
@@ -81,15 +87,14 @@
     detach: Optional[bool] = typer.Option(
         None,
         "--detach",
         help="Start the container in detach mode (default for non-interfaces)",
         show_default=False,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--pull", pull, IF=pull),
         Application.serialize_parameter("--debug", debug, IF=debug),
         Application.serialize_parameter("--command", command, IF=command),
         Application.serialize_parameter("--user", user, IF=user),
         Application.serialize_parameter("--port", first_port, IF=first_port),
         Application.serialize_parameter("", service),
@@ -107,15 +112,14 @@
         print_and_exit("Can't start the registry in compose mode")
 
     docker = Docker()
     if Configuration.swarm_mode:
         if service != REGISTRY:
             docker.registry.ping()
         else:
-
             if docker.registry.ping(do_exit=False):
                 registry = docker.registry.get_host()
                 print_and_exit("The registry is already running at {}", registry)
 
             if docker.client.container.exists("registry"):
                 log.debug("The registry container is already existing, removing")
                 docker.client.container.remove("registry", force=True)
@@ -165,15 +169,15 @@
     # This is equivalent to the old registry command
     if service == REGISTRY:
         # @ symbol in secrets is not working
         # https://github.com/bitnami/charts/issues/1954
         # Other symbols like # and " also lead to configuration errors
         os.environ["REGISTRY_HTTP_SECRET"] = password(
             param_not_used="",
-            length=96
+            length=96,
             # , symbols="%*,-.=?[]^_~"
         )
 
     publish_ports = get_publish_ports(service, first_port)
 
     if detach is None:
         if service == "swaggerui" or service == "adminer":
```

### Comparing `rapydo-2.4/controller/commands/shell.py` & `rapydo-3.0/controller/commands/shell.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Open a shell or execute a command onto a container
 """
+
 from typing import Optional
 
 import typer
 
 from controller import log, print_and_exit
 from controller.app import Application
 from controller.deploy.docker import Docker
@@ -49,15 +50,14 @@
     broadcast: bool = typer.Option(
         False,
         "--broadcast",
         help="Execute the command on all the replicas",
         show_default=False,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--user", user, IF=user),
         Application.serialize_parameter(
             "--default", default_command, IF=default_command
         ),
         Application.serialize_parameter("", service),
         Application.serialize_parameter("", command),
```

### Comparing `rapydo-2.4/controller/commands/ssl.py` & `rapydo-3.0/controller/commands/ssl.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Issue a SSL certificate with Let's Encrypt
 """
+
 from pathlib import Path
 from typing import Optional
 
 import typer
 
 from controller import RED, log, print_and_exit
 from controller.app import Application, Configuration
@@ -74,15 +75,14 @@
     verify_available_images(
         [service],
         Application.data.compose_config,
         Application.data.base_services,
     )
 
     if chain_file is not None and key_file is not None:
-
         log.info("Unable to automatically perform the requested operation")
         log.info("You can execute the following commands by your-self:")
 
         c = f"{Configuration.project}_{service}_1"
         letsencrypt_path = "/etc/letsencrypt/real"
         print("")
         print(f"docker cp {chain_file} {c}:{letsencrypt_path}/fullchain1.pem")
```

### Comparing `rapydo-2.4/controller/commands/start.py` & `rapydo-3.0/controller/commands/start.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Start services for the current configuration
 """
+
 import time
 from typing import List
 
 import typer
 from python_on_whales.exceptions import DockerException
 
 from controller import log
@@ -39,15 +40,14 @@
         False,
         "--force",
         "-f",
         help="Force containers restart",
         show_default=False,
     ),
 ) -> None:
-
     Application.print_command(Application.serialize_parameter("", services))
 
     Application.get_controller().controller_init(services)
 
     docker = Docker()
     if Configuration.swarm_mode:
         docker.registry.ping()
```

### Comparing `rapydo-2.4/controller/commands/status.py` & `rapydo-3.0/controller/commands/status.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Show current services status
 """
+
 from typing import List
 
 import typer
 
 from controller.app import Application
 from controller.deploy.docker import Docker
 
@@ -13,14 +14,13 @@
 def status(
     services: List[str] = typer.Argument(
         None,
         help="Services to be inspected",
         shell_complete=Application.autocomplete_service,
     ),
 ) -> None:
-
     Application.print_command(Application.serialize_parameter("", services))
 
     Application.get_controller().controller_init(services)
 
     docker = Docker()
     docker.status(Application.data.services)
```

### Comparing `rapydo-2.4/controller/commands/swarm/images.py` & `rapydo-3.0/controller/commands/swarm/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         "--rm",
         "--remove",
         help="Remove the specified image(s)",
         show_default=False,
         shell_complete=Application.autocomplete_submodule,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--remove", remove_images, IF=remove_images),
     )
 
     Application.get_controller().controller_init()
 
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
@@ -46,23 +45,21 @@
     # Retrieve a sorted, json list of repositories available in the registry
     r = docker.registry.send_request(f"{host}/v2/_catalog")
 
     catalog = r.json()
 
     images: List[Tuple[str, str, str, int, Optional[datetime]]] = []
     for repository in catalog.get("repositories", {}):
-
         # Fetch the tags under the repository identified by <name>
         r = docker.registry.send_request(f"{host}/v2/{repository}/tags/list")
         # tags can be None if all the tags of a repository have deleted
         # this or ensure that every None will be converted in an empty dictionary
         tags = r.json().get("tags") or {}
 
         for tag in tags:
-
             # Fetch the manifest identified by name and reference
             r = docker.registry.send_request(f"{host}/v2/{repository}/manifests/{tag}")
             manifest = r.json()
             size = 0
             for layer in manifest.get("layers", []):
                 size += layer.get("size", 0)
 
@@ -86,20 +83,18 @@
                     created = datetime.strptime(creation_date, "%Y-%m-%dT%H:%M:%S")
 
             images.append((_id, cast(str, repository), cast(str, tag), size, created))
 
     if not images:
         log.warning("This registry contains no images")
     else:
-
         log.info("This registry contains {} image(s):", len(images))
         images_to_be_removed: List[Tuple[str, str, str]] = []
         table: List[List[str]] = []
         for img in images:
-
             digest = img[0]
             # to be replaced with removeprefix starting from py39
             if digest.startswith("sha256:"):
                 digest = digest[7:]
             _id = digest[0:12]
 
             repository = img[1]
```

### Comparing `rapydo-2.4/controller/commands/swarm/join.py` & `rapydo-3.0/controller/commands/swarm/join.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,24 +17,24 @@
     Application.get_controller().controller_init()
 
     docker = Docker()
 
     manager_address = "N/A"
     # Search for the manager address
     for node in docker.client.node.list():
-
         role = node.spec.role
         state = node.status.state
         availability = node.spec.availability
 
         if (
             role == "manager"
             and state == "ready"
             and availability == "active"
             and node.manager_status
+            and node.manager_status.addr
         ):
             manager_address = node.manager_status.addr
 
     if manager:
         log.info("To add a manager to this swarm, run the following command:")
         token = docker.swarm.get_token("manager")
     else:
```

### Comparing `rapydo-2.4/controller/commands/swarm/logs.py` & `rapydo-3.0/controller/commands/swarm/logs.py`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/commands/swarm/remove.py` & `rapydo-3.0/controller/commands/swarm/remove.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 def remove(
     services: List[str] = typer.Argument(
         None,
         help="Services to be removed",
         shell_complete=Application.autocomplete_service,
     ),
 ) -> None:
-
     Application.print_command(Application.serialize_parameter("", services))
 
     remove_extras: List[str] = []
     for extra in (
         REGISTRY,
         "adminer",
         "swaggerui",
@@ -73,15 +72,14 @@
         # This is needed because docker stack remove does not support a --wait flag
         # To make the remove command sync and chainable with a start command
         engine = Application.env.get("DEPLOY_ENGINE", "swarm")
         network_name = f"{Configuration.project}_{engine}_default"
         wait_network_removal(docker, network_name)
         log.info("Stack removed")
     else:
-
         if not docker.swarm.stack_is_running():
             print_and_exit(
                 "Stack {} is not running, deploy it with {command}",
                 Configuration.project,
                 command=RED("rapydo start"),
             )
```

### Comparing `rapydo-2.4/controller/commands/swarm/scale.py` & `rapydo-3.0/controller/commands/swarm/scale.py`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/commands/tuning.py` & `rapydo-3.0/controller/commands/tuning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Show tuning suggestions for a service
 """
+
 import os
 from enum import Enum
 
 import typer
 
 from controller import log, print_and_exit
 from controller.app import Application
```

### Comparing `rapydo-2.4/controller/commands/tuning_modules/neo4j.py` & `rapydo-3.0/controller/commands/tuning_modules/neo4j.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from controller.deploy.builds import verify_available_images
 from controller.deploy.docker import Docker
 
 SERVICE_NAME = __name__
 
 
 def tuning(ram: int, cpu: int) -> None:
-
     verify_available_images(
         [SERVICE_NAME],
         Application.data.compose_config,
         Application.data.base_services,
     )
 
     docker = Docker()
```

### Comparing `rapydo-2.4/controller/commands/tuning_modules/postgres.py` & `rapydo-3.0/controller/commands/tuning_modules/postgres.py`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/commands/update.py` & `rapydo-3.0/controller/commands/update.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Update the current project
 """
+
 from typing import List
 
 import typer
 
 from controller import log
 from controller.app import Application
 from controller.utilities import services
@@ -17,15 +18,14 @@
         "--ignore-submodule",
         "-i",
         help="Ignore a submodule",
         show_default=False,
         shell_complete=Application.autocomplete_submodule,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--ignore-submodule", ignore_submodules),
     )
 
     Application.get_controller().controller_init()
 
     Application.git_update(ignore_submodules)
```

### Comparing `rapydo-2.4/controller/commands/upgrade.py` & `rapydo-3.0/controller/commands/upgrade.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Upgrade a project file by re-applying the templates
 """
+
 from pathlib import Path
 
 import typer
 from glom import glom
 
 from controller import EXTENDED_PROJECT_DISABLED
 from controller.app import Application, Configuration
@@ -17,15 +18,14 @@
     path: Path = typer.Option(
         ...,
         "--path",
         help="path of file to be upgraded",
         show_default=False,
     ),
 ) -> None:
-
     Application.print_command(
         Application.serialize_parameter("--path", path, IF=path),
     )
 
     Application.get_controller().controller_init()
 
     frontend = glom(
```

### Comparing `rapydo-2.4/controller/commands/version.py` & `rapydo-3.0/controller/commands/version.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Show RAPyDo and project version details
 """
+
 from packaging.version import Version
 
 from controller import RED, __version__, colors
 from controller.app import Application, Configuration
 
 
 @Application.app.command(help="Show rapydo and project version details")
 def version() -> None:
-
     Application.print_command()
 
     Application.get_controller().controller_init()
 
     # Check if rapydo version is compatible with version required by the project
     if __version__ == Configuration.rapydo_version:
         c = colors.GREEN  # Light Green
```

### Comparing `rapydo-2.4/controller/commands/volatile.py` & `rapydo-3.0/controller/commands/volatile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 [DEPRECATED] Run a single container in debug mode
 """
+
 import typer
 
 from controller import print_and_exit
 from controller.app import Application
 
 
 # Deprecated since 2.1
```

### Comparing `rapydo-2.4/controller/confs/angular.yml` & `rapydo-3.0/controller/confs/angular.yml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 services:
   proxy:
     volumes:
       - ${DATA_DIR}/${COMPOSE_PROJECT_NAME}/frontend:/app
 
   frontend:
     build:
-      context: ${SUBMODULE_DIR}/build-templates/${FRONTEND_BUILD_MODE}
+      context: ${SUBMODULE_DIR}/do/controller/builds/${FRONTEND_BUILD_MODE}
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/${FRONTEND_BUILD_MODE}:${RAPYDO_VERSION}
     healthcheck:
       test: "wget -t 1 --quiet --no-check-certificate http://localhost:8080 -O - > /dev/null"
@@ -34,14 +34,15 @@
       RAPYDO_VERSION: ${RAPYDO_VERSION}
       PROJECT_NAME: ${COMPOSE_PROJECT_NAME}
       PROJECT_TITLE: "${PROJECT_TITLE}"
       PROJECT_DESCRIPTION: "${PROJECT_DESCRIPTION}"
       PROJECT_KEYWORDS: "${PROJECT_KEYWORDS}"
       ENABLE_ANGULAR_SSR: ${ENABLE_ANGULAR_SSR}
       ENABLE_YARN_PNP: ${ENABLE_YARN_PNP}
+      ENABLE_ANGULAR_MULTI_LANGUAGE: ${ENABLE_ANGULAR_MULTI_LANGUAGE}
       FORCE_SSR_SERVER_MODE: ${FORCE_SSR_SERVER_MODE}
       SPINNER_TYPE: ${SPINNER_TYPE}
       SHOW_LOGIN: ${SHOW_LOGIN}
       ENABLE_FOOTER: ${ENABLE_FOOTER}
       ALLOW_PASSWORD_RESET: ${ALLOW_PASSWORD_RESET}
       ALLOW_REGISTRATION: ${ALLOW_REGISTRATION}
       ALLOW_TERMS_OF_USE: ${ALLOW_TERMS_OF_USE}
@@ -56,15 +57,14 @@
       FRONTEND_URL: ${FRONTEND_URL}
       BASE_HREF: ${PROJECT_DOMAIN}
       FRONTEND_PREFIX: ${FRONTEND_PREFIX}
       # Prevent: error YN0028: The lockfile would have been created by this install,
       #                        which is explicitly forbidden.
       YARN_ENABLE_IMMUTABLE_INSTALLS: "false"
       SENTRY_URL: ${SENTRY_URL}
-      GA_TRACKING_CODE: ${GA_TRACKING_CODE}
 
       CYPRESS_AUTH_DEFAULT_USERNAME: ${AUTH_DEFAULT_USERNAME}
       CYPRESS_AUTH_DEFAULT_PASSWORD: ${AUTH_DEFAULT_PASSWORD}
       CYPRESS_AUTH_FORCE_FIRST_PASSWORD_CHANGE: ${AUTH_FORCE_FIRST_PASSWORD_CHANGE}
       CYPRESS_SHOW_LOGIN: ${SHOW_LOGIN}
       CYPRESS_ALLOW_PASSWORD_RESET: ${ALLOW_PASSWORD_RESET}
       CYPRESS_ALLOW_REGISTRATION: ${ALLOW_REGISTRATION}
@@ -73,14 +73,15 @@
       CYPRESS_AUTH_ROLES: ${AUTH_ROLES}
       CYPRESS_AUTH_MIN_PASSWORD_LENGTH: ${AUTH_MIN_PASSWORD_LENGTH}
       CYPRESS_AUTH_MAX_PASSWORD_VALIDITY: ${AUTH_MAX_PASSWORD_VALIDITY}
       CYPRESS_AUTH_DISABLE_UNUSED_CREDENTIALS_AFTER: ${AUTH_DISABLE_UNUSED_CREDENTIALS_AFTER}
       CYPRESS_AUTH_SECOND_FACTOR_AUTHENTICATION: ${AUTH_SECOND_FACTOR_AUTHENTICATION}
       CYPRESS_AUTH_MAX_LOGIN_ATTEMPTS: ${AUTH_MAX_LOGIN_ATTEMPTS}
       CYPRESS_AUTH_LOGIN_BAN_TIME: ${AUTH_LOGIN_BAN_TIME}
+      CYPRESS_CACHE_FOLDER: "/tmp"
 
       CYPRESS_BACKEND_HOST: ${FLASK_HOST}
       CYPRESS_API_URL: http://${FLASK_HOST}:${BACKEND_PORT}/
       # FROM ENV, USED BY CYPRESS TO RECORD RESULTS:
       GITHUB_ACTIONS:
       GITHUB_RUN_ID:
       CYPRESS_RECORD_KEY:
@@ -119,16 +120,17 @@
       - ${SUBMODULE_DIR}/rapydo-angular/tsconfig.server.json:/app/tsconfig.server.json
       - ${SUBMODULE_DIR}/rapydo-angular/tsconfig.spec.json:/app/tsconfig.spec.json
 
       - ${SUBMODULE_DIR}/rapydo-angular/src:/app/app/rapydo
       - ${PROJECT_DIR}/frontend:/app/app/custom
 
       - ${SUBMODULE_DIR}/rapydo-angular/cypress.config.ts:/app/cypress.config.ts
-      - ${SUBMODULE_DIR}/rapydo-angular/cypress/tsconfig.json:/app/cypress/tsconfig.json
       - ${SUBMODULE_DIR}/rapydo-angular/cypress/coverage.webpack.js:/app/cypress/coverage.webpack.js
-      - ${SUBMODULE_DIR}/rapydo-angular/cypress/support:/app/cypress/support
-      - ${SUBMODULE_DIR}/rapydo-angular/cypress/plugins:/app/cypress/plugins
-      - ${SUBMODULE_DIR}/rapydo-angular/cypress/fixtures:/app/cypress/fixtures
-      - ${SUBMODULE_DIR}/rapydo-angular/cypress/e2e:/app/cypress/e2e/rapydo
-      - ${PROJECT_DIR}/frontend/e2e:/app/cypress/e2e/custom
+      - ${SUBMODULE_DIR}/rapydo-angular/cypress/support:/e2e/support
+      - ${SUBMODULE_DIR}/rapydo-angular/cypress/plugins:/e2e/plugins
+      - ${SUBMODULE_DIR}/rapydo-angular/cypress/fixtures:/e2e/fixtures
+      - ${SUBMODULE_DIR}/rapydo-angular/cypress/tsconfig.json:/e2e/tsconfig.json
+      - ${SUBMODULE_DIR}/rapydo-angular/cypress/e2e:/e2e/rapydo
+      - ${DATA_DIR}/${COMPOSE_PROJECT_NAME}/frontend/node_modules:/e2e/node_modules
+      - ${PROJECT_DIR}/frontend/e2e:/e2e/custom
 
       - ${DATA_DIR}/logs:/logs
```

### Comparing `rapydo-2.4/controller/confs/backend.yml` & `rapydo-3.0/controller/confs/backend.yml`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # SERVICES
 # #####################
 
 services:
   backend:
     restart: always
     build:
-      context: ${SUBMODULE_DIR}/build-templates/${BACKEND_BUILD_MODE}
+      context: ${SUBMODULE_DIR}/do/controller/builds/${BACKEND_BUILD_MODE}
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/${BACKEND_BUILD_MODE}:${RAPYDO_VERSION}
     healthcheck:
       test: ${HEALTHCHECK_BACKEND_CMD}
@@ -64,15 +64,15 @@
       PYTHONUNBUFFERED: 1
 
       PYTHONMALLOC: ${PYTHONMALLOC}
       PYTHONASYNCIODEBUG: ${PYTHONASYNCIODEBUG}
       PYTHONFAULTHANDLER: ${PYTHONFAULTHANDLER}
 
       FLASK_APP: ${PYTHON_PATH}/restapi/${PYTHON_MAIN_FILE}.py
-      FLASK_ENV: ${FLASK_ENV}
+      FLASK_DEBUG: ${FLASK_DEBUG}
       API_AUTOSTART: ${API_AUTOSTART}
       # used by gunicorn
       APP_MODULE: "restapi.${PYTHON_MAIN_FILE}:app"
       GUNICORN_WORKERS: ${GUNICORN_WORKERS}
       GUNICORN_WORKERS_PER_CORE: ${GUNICORN_WORKERS_PER_CORE}
       GUNICORN_MAX_NUM_WORKERS: ${GUNICORN_MAX_NUM_WORKERS}
       PROJECT_NAME: ${COMPOSE_PROJECT_NAME}
@@ -119,14 +119,15 @@
       ALCHEMY_HOST: ${ALCHEMY_HOST}
       ALCHEMY_PORT: ${ALCHEMY_PORT}
       ALCHEMY_USER: "${ALCHEMY_USER}"
       ALCHEMY_PASSWORD: "${ALCHEMY_PASSWORD}"
       ALCHEMY_DB: ${ALCHEMY_DB}
       ALCHEMY_POOLSIZE: ${ALCHEMY_POOLSIZE}
       ALCHEMY_DBTYPE: ${ALCHEMY_DBTYPE}
+      ALEMBIC_CONFIG: "${COMPOSE_PROJECT_NAME}/migrations/alembic.ini"
       ALEMBIC_AUTO_MIGRATE: ${ALEMBIC_AUTO_MIGRATE}
 
       NEO4J_ENABLE: ${ACTIVATE_NEO4J}
       NEO4J_ENABLE_CONNECTOR: ${NEO4J_ENABLE_CONNECTOR}
       NEO4J_EXPIRATION_TIME: ${NEO4J_EXPIRATION_TIME}
       NEO4J_VERIFICATION_TIME: ${NEO4J_VERIFICATION_TIME}
       NEO4J_HOST: ${NEO4J_HOST}
@@ -177,22 +178,27 @@
 
       SMTP_ENABLE: ${ACTIVATE_SMTP}
       SMTP_ENABLE_CONNECTOR: ${SMTP_ENABLE_CONNECTOR}
       SMTP_EXPIRATION_TIME: ${SMTP_EXPIRATION_TIME}
       SMTP_VERIFICATION_TIME: ${SMTP_VERIFICATION_TIME}
       SMTP_ADMIN: "${SMTP_ADMIN}"
       SMTP_NOREPLY: "${SMTP_NOREPLY}"
+      SMTP_REPLYTO: "${SMTP_REPLYTO}"
       SMTP_HOST: "${SMTP_HOST}"
       SMTP_PORT: "${SMTP_PORT}"
       SMTP_USERNAME: "${SMTP_USERNAME}"
       SMTP_PASSWORD: "${SMTP_PASSWORD}"
 
       SENTRY_URL: "${SENTRY_URL}"
       MAX_LOGS_LENGTH: ${MAX_LOGS_LENGTH}
 
+      # Temporary added to silence SQLAlchemy 2.0 uber warning
+      SQLALCHEMY_SILENCE_UBER_WARNING: "1"
+      # Added to raise sqlalchemy RemovedIn20Warning deprecation warnings
+      SQLALCHEMY_WARN_20: "1"
     volumes:
       # configuration files
       - ${SUBMODULE_DIR}/do/controller/confs/projects_defaults.yaml:/code/confs/projects_defaults.yaml
       - ${PROJECT_DIR}/project_configuration.yaml:/code/confs/project_configuration.yaml
       - secrets:${APP_SECRETS}
       - ssl_certs:/etc/letsencrypt
       - data_imports:${DATA_IMPORT_FOLDER}
@@ -219,15 +225,15 @@
       default:
         aliases:
           - ${FLASK_HOST}
 
   proxy:
     restart: always
     build:
-      context: ${SUBMODULE_DIR}/build-templates/proxy
+      context: ${SUBMODULE_DIR}/do/controller/builds/proxy
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/proxy:${RAPYDO_VERSION}
     hostname: proxy
     logging:
@@ -284,20 +290,19 @@
       CSP_FRAME_SRC: "${SET_CSP_FRAME_SRC}"
       SSL_VERIFY_CLIENT: "${SSL_VERIFY_CLIENT}"
       SSL_FORCE_SELF_SIGNED: "${SSL_FORCE_SELF_SIGNED}"
       MAX_REQUESTS_PER_SECOND_AUTH: ${SET_MAX_REQUESTS_PER_SECOND_AUTH}
       MAX_REQUESTS_BURST_AUTH: ${SET_MAX_REQUESTS_BURST_AUTH}
       MAX_REQUESTS_PER_SECOND_API: ${SET_MAX_REQUESTS_PER_SECOND_API}
       MAX_REQUESTS_BURST_API: ${SET_MAX_REQUESTS_BURST_API}
-      GA_TRACKING_CODE: "${GA_TRACKING_CODE}"
 
   maintenance:
     # restart: always
     build:
-      context: ${SUBMODULE_DIR}/build-templates/proxy
+      context: ${SUBMODULE_DIR}/do/controller/builds/proxy
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/proxy:${RAPYDO_VERSION}
     entrypoint: docker-entrypoint-maintenanance
     hostname: proxy
@@ -321,15 +326,15 @@
 
   ###################
   ###  DATABASES  ###
   ###################
   postgres:
     restart: always
     build:
-      context: ${SUBMODULE_DIR}/build-templates/postgres
+      context: ${SUBMODULE_DIR}/do/controller/builds/postgres
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/postgres:${RAPYDO_VERSION}
     command: postgres -c max_connections=${POSTGRES_MAX_CONNECTIONS} -c shared_buffers=${POSTGRES_SHARED_BUFFERS} -c wal_buffers=${POSTGRES_WAL_BUFFERS} -c effective_cache_size=${POSTGRES_EFFECTIVE_CACHE_SIZE} -c work_mem=${POSTGRES_WORK_MEM} -c maintenance_work_mem=${POSTGRES_MAINTENANCE_WORK_MEM} -c effective_io_concurrency=${POSTGRES_EFFECTIVE_IO_CONCURRENCY} -c max_worker_processes=${POSTGRES_MAX_WORKER_PROCESSES} -c max_parallel_workers=${POSTGRES_MAX_WORKER_PROCESSES}
     healthcheck:
@@ -357,15 +362,15 @@
       default:
         aliases:
           - ${ALCHEMY_HOST}
 
   neo4j:
     restart: always
     build:
-      context: ${SUBMODULE_DIR}/build-templates/neo4j
+      context: ${SUBMODULE_DIR}/do/controller/builds/neo4j
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/neo4j:${RAPYDO_VERSION}
     healthcheck:
       # test: ["CMD", "cypher-shell", "'match (n) WITH n LIMIT 1 return count(n)'"]
@@ -441,15 +446,15 @@
   #########################
   ###  QUEUE MANAGEMENT ###
   #########################
 
   celery:
     restart: always
     build:
-      context: ${SUBMODULE_DIR}/build-templates/${BACKEND_BUILD_MODE}
+      context: ${SUBMODULE_DIR}/do/controller/builds/${BACKEND_BUILD_MODE}
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/${BACKEND_BUILD_MODE}:${RAPYDO_VERSION}
     entrypoint: docker-entrypoint-celery
     command: celery --app restapi.connectors.celery.worker.celery_app worker --concurrency=1 --pool=${CELERY_POOL_MODE} -Ofair -Q celery -n ${COMPOSE_PROJECT_NAME}-%h
@@ -545,14 +550,15 @@
 
       SMTP_ENABLE: ${ACTIVATE_SMTP}
       SMTP_ENABLE_CONNECTOR: ${SMTP_ENABLE_CONNECTOR}
       SMTP_EXPIRATION_TIME: ${SMTP_EXPIRATION_TIME}
       SMTP_VERIFICATION_TIME: ${SMTP_VERIFICATION_TIME}
       SMTP_ADMIN: "${SMTP_ADMIN}"
       SMTP_NOREPLY: "${SMTP_NOREPLY}"
+      SMTP_REPLYTO: "${SMTP_REPLYTO}"
       SMTP_HOST: "${SMTP_HOST}"
       SMTP_PORT: "${SMTP_PORT}"
       SMTP_USERNAME: "${SMTP_USERNAME}"
       SMTP_PASSWORD: "${SMTP_PASSWORD}"
     volumes:
       # configuration files
       - ${SUBMODULE_DIR}/do/controller/confs/projects_defaults.yaml:/code/confs/projects_defaults.yaml
@@ -571,15 +577,15 @@
       - ${DATA_DIR}/uploads:/uploads
     networks:
       default:
 
   celerybeat:
     restart: always
     build:
-      context: ${SUBMODULE_DIR}/build-templates/${BACKEND_BUILD_MODE}
+      context: ${SUBMODULE_DIR}/do/controller/builds/${BACKEND_BUILD_MODE}
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/${BACKEND_BUILD_MODE}:${RAPYDO_VERSION}
     hostname: celery-beat
     entrypoint: docker-entrypoint-celery
@@ -633,14 +639,15 @@
       REDIS_VERIFICATION_TIME: ${REDIS_VERIFICATION_TIME}
       REDIS_HOST: ${REDIS_HOST}
       REDIS_PORT: ${REDIS_PORT}
       REDIS_PASSWORD: "${REDIS_PASSWORD}"
 
       SMTP_ADMIN: "${SMTP_ADMIN}"
       SMTP_NOREPLY: "${SMTP_NOREPLY}"
+      SMTP_REPLYTO: "${SMTP_REPLYTO}"
       SMTP_HOST: "${SMTP_HOST}"
       SMTP_PORT: "${SMTP_PORT}"
       SMTP_USERNAME: "${SMTP_USERNAME}"
       SMTP_PASSWORD: "${SMTP_PASSWORD}"
     volumes:
       # configuration files
       - ${SUBMODULE_DIR}/do/controller/confs/projects_defaults.yaml:/code/confs/projects_defaults.yaml
@@ -657,15 +664,15 @@
       - ${DATA_DIR}/logs:/logs
     networks:
       default:
 
   rabbit:
     restart: always
     build:
-      context: ${SUBMODULE_DIR}/build-templates/rabbitmq
+      context: ${SUBMODULE_DIR}/do/controller/builds/rabbitmq
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/rabbitmq:${RAPYDO_VERSION}
     healthcheck:
       test: "rabbitmq-diagnostics status"
@@ -700,15 +707,15 @@
       default:
         aliases:
           - ${RABBITMQ_HOST}
 
   redis:
     restart: always
     build:
-      context: ${SUBMODULE_DIR}/build-templates/redis
+      context: ${SUBMODULE_DIR}/do/controller/builds/redis
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/redis:${RAPYDO_VERSION}
     command: redis-server --appendonly yes --requirepass ${REDIS_PASSWORD}
     healthcheck:
@@ -736,15 +743,15 @@
   ##########################
   ### SERVICE INTERFACES ###
   ##########################
 
   flower:
     restart: always
     build:
-      context: ${SUBMODULE_DIR}/build-templates/${BACKEND_BUILD_MODE}
+      context: ${SUBMODULE_DIR}/do/controller/builds/${BACKEND_BUILD_MODE}
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/${BACKEND_BUILD_MODE}:${RAPYDO_VERSION}
     hostname: flower
 
@@ -829,15 +836,15 @@
       FLOWER_USER: "${FLOWER_USER}"
       FLOWER_PASSWORD: "${FLOWER_PASSWORD}"
       FLOWER_DBDIR: ${FLOWER_DBDIR}
       FLOWER_PROTOCOL: ${FLOWER_PROTOCOL}
 
   swaggerui:
     build:
-      context: ${SUBMODULE_DIR}/build-templates/swaggerui
+      context: ${SUBMODULE_DIR}/do/controller/builds/swaggerui
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/swaggerui:${RAPYDO_VERSION}
     logging:
       driver: ${DOCKER_LOGGING_DRIVER}
@@ -852,15 +859,15 @@
     volumes:
       - ssl_certs:/etc/letsencrypt
     ports:
       - 7777:8080
 
   adminer:
     build:
-      context: ${SUBMODULE_DIR}/build-templates/adminer
+      context: ${SUBMODULE_DIR}/do/controller/builds/adminer
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
         CURRENT_UID: ${CURRENT_UID}
         CURRENT_GID: ${CURRENT_GID}
     image: rapydo/adminer:${RAPYDO_VERSION}
     logging:
       driver: ${DOCKER_LOGGING_DRIVER}
@@ -880,15 +887,15 @@
       - 7777:80
 
   ###################
   ### FTP SERVER  ###
   ###################
   ftp:
     restart: always
-    build: ${SUBMODULE_DIR}/build-templates/ftp
+    build: ${SUBMODULE_DIR}/do/controller/builds/ftp
     image: rapydo/ftp:${RAPYDO_VERSION}
     volumes:
       - pureftpd:/etc/pure-ftpd/passwd
       - ssl_certs:/etc/letsencrypt
     # /etc/ssl/private/ A directory containing a single pure-ftpd.pem file
     # with the server's SSL certificates for TLS support. Optional TLS is
     # automatically enabled when the container finds this file on startup.
@@ -931,15 +938,15 @@
 
   #############################
   ### LOCAL DOCKER REGISTRY ###
   #############################
 
   registry:
     restart: always
-    build: ${SUBMODULE_DIR}/build-templates/registry
+    build: ${SUBMODULE_DIR}/do/controller/builds/registry
     image: rapydo/registry:${RAPYDO_VERSION}
     hostname: registry
     # make it common to all projects
     container_name: registry
     healthcheck:
       test: "wget -t 1 --quiet --no-check-certificate http://localhost:5001/debug/health -O - > /dev/null"
       interval: ${HEALTHCHECK_INTERVAL}
@@ -976,15 +983,15 @@
 
   ##################
   ###  FAIL2BAN  ###
   ##################
 
   fail2ban:
     restart: always
-    build: ${SUBMODULE_DIR}/build-templates/fail2ban
+    build: ${SUBMODULE_DIR}/do/controller/builds/fail2ban
     image: rapydo/fail2ban:${RAPYDO_VERSION}
     # This works for compose but not for swarm.
     # In swarm mode this flag is replaced with an external network
     network_mode: "host"
     hostname: fail2ban
     cap_add:
       - NET_ADMIN
@@ -1022,15 +1029,15 @@
 
   ################
   ###   MYPY   ###
   ################
 
   mypy:
     build:
-      context: ${SUBMODULE_DIR}/build-templates/mypy
+      context: ${SUBMODULE_DIR}/do/controller/builds/mypy
       args:
         RAPYDO_VERSION: ${RAPYDO_VERSION}
     image: rapydo/mypy:${RAPYDO_VERSION}
     command: mypy --version
     working_dir: /code/${COMPOSE_PROJECT_NAME}
     environment:
       ACTIVATE: ${ACTIVATE_MYPY}
```

### Comparing `rapydo-2.4/controller/confs/projects_defaults.yaml` & `rapydo-3.0/controller/confs/projects_defaults.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 variables:
   submodules:
     http-api:
       online_url: https://github.com/rapydo/http-api.git
-    build-templates:
-      online_url: https://github.com/rapydo/build-templates.git
     rapydo-angular:
       online_url: https://github.com/rapydo/rapydo-angular.git
       _if: $$angular
     do:
       online_url: https://github.com/rapydo/do.git
 
   roles:
@@ -20,15 +18,14 @@
   roles_descriptions:
     admin_root: System Administrator
     staff_user: Project Administrator
     group_coordinator: Group Coordinator
     normal_user: Normal User
 
   env:
-    BACKEND_BUILD_MODE: backend
     FRONTEND_FRAMEWORK: nofrontend
     FRONTEND_BUILD_MODE: angular # or angular-test
     NETWORK_MTU: 1500
     HEALTHCHECK_INTERVAL: "1m"
     # Healtcheck in development is not possibile because the server is not automatically executed
     HEALTHCHECK_BACKEND_CMD: "exit 0" # changed in prod mode to enable a true check
 
@@ -63,22 +60,21 @@
     MYPY_ADD_LIBS: ""
 
     MAX_LOGS_LENGTH: 200
 
     APP_MODE: development
     FLASK_HOST: apiserver.dockerized.io
     FLASK_DEFAULT_PORT: 8080 # used for Flask biding (into the container)
-    FLASK_ENV: development
+    FLASK_DEBUG: "1"
     API_AUTOSTART: 0 # used in some tests to auto-start the backend
     BACKEND_PORT: 8080 # used for port mapping (outside the container)
     BACKEND_API_PORT: 8080 # used to reach the backend from outer network (in production should much with proxy ssl port)
     BACKEND_URL: ""
     PYTHON_MAIN_FILE: __main__
-    # Path to dist-packages in backend/celery containers
-    PYTHON_PATH: /usr/local/lib/python3.10/dist-packages
+    BACKEND_PYTHON_VERSION: "v3.11"
 
     PYTHONMALLOC: ""
     PYTHONASYNCIODEBUG: 0
     PYTHONFAULTHANDLER: 0
 
     BACKEND_PREFIX: ""
     APP_SECRETS: /secrets
@@ -145,15 +141,15 @@
     ALCHEMY_HOST: sql.dockerized.io
     ALCHEMY_PORT: 5432
     ALCHEMY_DBTYPE: "postgresql"
     ALCHEMY_USER: "sqluser" # This default is invalidated in production mode
     ALCHEMY_PASSWORD: "D3vMode!" # This default is invalidated in production mode
     ALCHEMY_DB: SQL_API
     ALCHEMY_DBS: SQL_API
-    ALCHEMY_POOLSIZE: 30 # or 20 # (default is 5)
+    ALCHEMY_POOLSIZE: 30 # default is 5
 
     # Have a look at this website for a quick tuning:
     # https://pgtune.leopard.in.ua
     POSTGRES_MAX_CONNECTIONS: 50 # default increased to 250 in production mode
     # Something like 25% of available RAM
     POSTGRES_SHARED_BUFFERS: 256MB # default increased to 1GB in production mode
     # 16MB is the default, but if you have a lot of concurrent
@@ -315,14 +311,15 @@
 
     # Smtp
     SMTP_ENABLE_CONNECTOR: 1
     SMTP_EXPIRATION_TIME: 7200
     SMTP_VERIFICATION_TIME: 900
     SMTP_ADMIN:
     SMTP_NOREPLY:
+    SMTP_REPLYTO:
     SMTP_HOST:
     SMTP_PORT: 25
     SMTP_USERNAME:
     SMTP_PASSWORD:
 
     # These two variables should be merged with the variables above
     # i.e. if smtp server is enabled these should be the default values
@@ -339,19 +336,19 @@
     FRONTEND_URL: ""
     FRONTEND_PREFIX: /
     ALLOW_PASSWORD_RESET: 0
     ALLOW_REGISTRATION: 0
     ALLOW_TERMS_OF_USE: 0
     REGISTRATION_NOTIFICATIONS: 1
     SENTRY_URL:
-    GA_TRACKING_CODE:
     SHOW_LOGIN: 1
     ENABLE_FOOTER: 1
     ENABLE_ANGULAR_SSR: 1
     ENABLE_YARN_PNP: 0
+    ENABLE_ANGULAR_MULTI_LANGUAGE: 0
     FORCE_SSR_SERVER_MODE: 0
     SPINNER_TYPE: "ball-scale-multiple"
 
     ACTIVATE_AUTH: 1
     AUTH_SERVICE: NO_AUTHENTICATION
     AUTH_DEFAULT_USERNAME: "user@nomail.org"
     AUTH_DEFAULT_PASSWORD: "D3vMode!" # This default is invalidated in production mode
@@ -367,21 +364,23 @@
     AUTH_TOTP_VALIDITY_WINDOW: 1 # int value
     AUTH_JWT_TOKEN_TTL: 2592000 # 1 month in seconds
     AUTH_TOKEN_SAVE_FREQUENCY: 60 # tokens are saved every this amount of seconds
     AUTH_TOKEN_IP_GRACE_PERIOD: 1800 # period before starting to evaluate IP address on token validation
     ALLOW_ACCESS_TOKEN_PARAMETER: 0
     DEFAULT_DHLEN: 2048
 
+    PASSWORD_EXPIRATION_WARNING: 180
+
     FORCE_PRODUCTION_TESTS: 0 # Very dangerous, do not touch it!
 
 project:
   title: "REST HTTP-API server with Python, Flask and Docker"
   description: "No description yet"
   keywords: ""
-  rapydo: 2.4
+  rapydo: "3.0"
   version: v0.1
 
 tags:
   specifications: OpenAPI 2.0 Specification in JSON format
   status: Verify the status of the server
   authentication: Manage authentication and active tokens
   profile: Manage your own profile
```

### Comparing `rapydo-2.4/controller/confs/projects_prod_defaults.yaml` & `rapydo-3.0/controller/confs/projects_prod_defaults.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   env:
     LOG_LEVEL: INFO # log level for backend and celery
     MIN_PASSWORD_SCORE: 4
     DOCKER_LOGGING_DRIVER: "syslog"
 
     ACTIVATE_PROXY: 1
     APP_MODE: production
-    FLASK_ENV: production
+    FLASK_DEBUG: "0"
     # in development mode this is mapped on port 81
     PROXY_DEV_PORT: 80
     # used to reach the backend from outer network
     # in production it match the with proxy ssl port (${PROXY_PROD_PORT})
     BACKEND_API_PORT: 443
     ACTIVATE_FAIL2BAN: 1
```

### Comparing `rapydo-2.4/controller/confs/swarm_angular_prod_options.yml` & `rapydo-3.0/controller/confs/swarm_angular_prod_options.yml`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/confs/swarm_options.yml` & `rapydo-3.0/controller/confs/swarm_options.yml`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,15 @@
       mode: global
       # placement:
       #   constraints:
       #     - "node.role==manager"
 
     # network_mode does not work in swarm mode
     # This external network is a workaround to let the container access the host network
+    network_mode: ""
     networks:
       - outside
 
 networks:
   outside:
     name: "host"
     external: true
```

### Comparing `rapydo-2.4/controller/confs/volumes_nfs.yml` & `rapydo-3.0/controller/confs/volumes_nfs.yml`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/deploy/builds.py` & `rapydo-3.0/controller/deploy/builds.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     path: Optional[Path]
 
 
 BuildInfo = Dict[str, TemplateInfo]
 
 
 def name_priority(name1: str, name2: str) -> str:
-
     # Prevents warning: Cannot determine build priority with custom services
     if name1 in Application.data.custom_services:
         return name2
 
     if name2 in Application.data.custom_services:
         return name1
 
@@ -57,19 +56,17 @@
     except NoSuchImage:
         return datetime.fromtimestamp(0)
 
 
 def find_templates_build(
     base_services: ComposeServices, include_image: bool = False
 ) -> BuildInfo:
-
     templates: BuildInfo = {}
 
     for template_name, base_service in base_services.items():
-
         template_build = base_service.build
 
         if not template_build and not include_image:
             continue
 
         template_image = base_service.image
 
@@ -90,15 +87,14 @@
             )
         templates[template_image]["services"].append(template_name)
 
     return templates
 
 
 def get_dockerfile_base_image(path: Path, templates: BuildInfo) -> str:
-
     dockerfile = path.joinpath("Dockerfile")
 
     if not dockerfile.exists():
         print_and_exit("Build path not found: {}", dockerfile)
 
     with open(dockerfile) as f:
         for line in reversed(f.readlines()):
@@ -122,36 +118,37 @@
 
     print_and_exit("Invalid Dockerfile, no base image found in {}", dockerfile)
 
 
 def find_templates_override(
     services: ComposeServices, templates: BuildInfo
 ) -> Dict[str, str]:
-
     builds: Dict[str, str] = {}
 
     for service in services.values():
-
-        if service.build is not None and service.image not in templates:
-
+        if (
+            service.build is not None
+            and service.build.context is not None
+            and service.image not in templates
+        ):
             baseimage = get_dockerfile_base_image(service.build.context, templates)
-
             if not baseimage.startswith("rapydo/"):
                 continue
 
             vanilla_img = service.image
-            template_img = baseimage
-            log.debug("{} extends {}", vanilla_img, template_img)
-            builds[vanilla_img] = template_img
+            if vanilla_img is None:  # pragma: no cover
+                continue
+
+            log.debug("{} extends {}", vanilla_img, baseimage)
+            builds[vanilla_img] = baseimage
 
     return builds
 
 
 def get_non_redundant_services(templates: BuildInfo, targets: List[str]) -> Set[str]:
-
     # Removed redundant services
     services_normalization_mapping: Dict[str, str] = {}
 
     for s in templates.values():
         for s1 in s["services"]:
             services_normalization_mapping[s1] = s["service"]
 
@@ -166,15 +163,14 @@
 
 def verify_available_images(
     services: List[str],
     compose_config: ComposeServices,
     base_services: ComposeServices,
     is_run_command: bool = False,
 ) -> None:
-
     docker = Docker()
     # All template builds (core only)
     templates = find_templates_build(base_services, include_image=True)
     clean_core_services = get_non_redundant_services(templates, services)
 
     for service in sorted(clean_core_services):
         for image, data in templates.items():
```

### Comparing `rapydo-2.4/controller/deploy/compose_v2.py` & `rapydo-3.0/controller/deploy/compose_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 
     def dump_config(
         self,
         services: List[str],
         set_registry: bool = True,
         v1_compatibility: bool = False,
     ) -> None:
-
         compose_config = self.get_config_json()
 
         clean_config: Dict[str, Any] = {
             "version": compose_config.get("version", COMPOSE_FILE_VERSION),
             "networks": {},
             "volumes": {},
             "services": {},
@@ -83,14 +82,21 @@
         for key, value in compose_config.get("services", {}).items():
             if key not in services:
                 continue
 
             if Configuration.swarm_mode and set_registry and key != REGISTRY:
                 value["image"] = f"{registry}/{value['image']}"
 
+            for non_null_key in (
+                "command",
+                "entrypoint",
+            ):
+                if non_null_key in value and value[non_null_key] is None:
+                    value.pop(non_null_key)
+
             if "healthcheck" in value and "test" in value["healthcheck"]:
                 # healtcheck commands can contain env variables double-escaped ($$)
                 # When dumped to docker-compose.yml the double escape is removed
                 # and when started the single escaped variable is not resolved
                 # and breaks the command. Let's double all the $ to restore the
                 # expected behavior and counteract the consumed $
                 value["healthcheck"]["test"] = [
@@ -125,15 +131,14 @@
 
             for k in value.get("volumes", []):
                 source = k.get("source", "")
                 volume_type = k.get("type", "")
                 if source and volume_type == "volume":
                     volumes.add(source.split(":")[0])
                 elif source and volume_type == "bind":
-
                     # Remove unsupported option: 'create_host_path'
                     if v1_compatibility:
                         k.get("bind", {}).pop("create_host_path", None)
 
                     binds.add(Path(source.split(":")[0]))
 
             # Remove replicas if both replicas and global mode are set
@@ -177,15 +182,14 @@
 
     def start_containers(
         self,
         services: List[str],
         force: bool = False,
         scales: Optional[Dict[str, int]] = None,
     ) -> None:
-
         if scales:
             # Based on rapydo scale implementation services is always a 1-length list
             service = services[0]
             nreplicas = scales.get(service, 0)
             services_list = f"{service}={nreplicas}"
 
             log.info("Scaling services: {}...", services_list)
@@ -213,15 +217,14 @@
         service: str,
         command: Optional[str] = None,
         publish: Optional[List[Union[PortMapping, PortRangeMapping]]] = None,
         # used by interfaces
         detach: bool = False,
         user: Optional[str] = None,
     ) -> bool:
-
         compose_engine_forced = False
         if Configuration.swarm_mode:
             # import here to prevent circular imports
             from controller.app import Application
 
             if not Configuration.FORCE_COMPOSE_ENGINE:
                 compose_engine_forced = True
@@ -268,15 +271,14 @@
 
             return True
         except DockerException as e:
             log.critical(e)
             return False
 
     def get_running_services(self) -> Set[str]:
-
         prefix = f"{Configuration.project}{COMPOSE_SEP}"
         containers = set()
         try:
             for container in self.docker.compose.ps():
                 name = container.name
                 if not name.startswith(prefix):
                     continue
@@ -296,24 +298,23 @@
         # `docker compose ps`
         # that fails with a "not found" and it seems to be a bug of compose-cli.
         # In case it is a feature a specific exception would be helpful here
         except DockerException:
             return containers
 
     def get_services_status(self, prefix: str) -> Dict[str, str]:
-
         prefix += COMPOSE_SEP
         services_status: Dict[str, str] = dict()
         try:
             for container in self.docker.compose.ps():
                 name = container.name
                 if not name.startswith(prefix):
                     continue
 
-                status = container.state.status
+                status = container.state.status or "N/A"
 
                 # to be replaced with removeprefix
                 name = name[len(prefix) :]
                 # Remove the _instancenumber (i.e. _1 or _n in case of scaled services)
                 name = name[0 : name.index(COMPOSE_SEP)]
                 services_status[name] = status
             return services_status
@@ -327,27 +328,26 @@
 
     def status(self, services: List[str]) -> None:
         print("")
 
         prefix = f"{Configuration.project}{COMPOSE_SEP}"
         table: List[List[str]] = []
         for container in self.docker.compose.ps():
-
             name = container.name
             if not name.startswith(prefix):
                 continue
             # to be replaced with removeprefix
             name = name[len(prefix) :]
             if COMPOSE_SEP in name:
                 name = name[0 : name.index(COMPOSE_SEP)]
 
             if name not in services:
                 continue
 
-            status = container.state.status
+            status = container.state.status or "N/A"
             if status == "shutdown" or status == "complete":
                 OPEN_COLOR = "[bold blue]"
                 CLOSE_COLOR = "[/bold blue]"
             elif status == "running":
                 OPEN_COLOR = "[bold green]"
                 CLOSE_COLOR = "[/bold green]"
             elif status == "starting" or status == "ready":
@@ -357,41 +357,47 @@
                 OPEN_COLOR = "[bold red]"
                 CLOSE_COLOR = "[/bold red]"
             else:
                 OPEN_COLOR = ""
                 CLOSE_COLOR = ""
 
             ports_list = []
-            for container_port, host_port in container.network_settings.ports.items():
-                if host_port:
-                    container_port = container_port.split("/")[0]
-                    ports_list.append(f"{container_port}->{host_port[0]['HostPort']}")
+            if container.network_settings.ports:
+                for (
+                    container_port,
+                    host_port,
+                ) in container.network_settings.ports.items():
+                    if host_port:
+                        container_port = container_port.split("/")[0]
+                        ports_list.append(
+                            f"{container_port}->{host_port[0]['HostPort']}"
+                        )
 
+            container_image = container.config.image or "N/A"
             table.append(
                 [
                     container.id[0:12],
                     f"{OPEN_COLOR}{container.name}{CLOSE_COLOR}",
                     status,
                     container.created.strftime("%d-%m-%Y %H:%M:%S"),
-                    container.config.image,
+                    container_image,
                     ",".join(ports_list),
                 ],
             )
 
         if not table:
             log.info("No container is running")
         else:
             print_table(
                 ["ID", "NAME", "STATUS", "CREATED", "IMAGE", "PORTS"],
                 table,
                 table_title="List of containers",
             )
 
     def logs(self, services: List[str], follow: bool = False, tail: int = 500) -> None:
-
         if len(services) > 1:
             timestamps = False
             log_prefix = True
         elif services[0] in "frontend":
             timestamps = True
             log_prefix = False
         else:
```

### Comparing `rapydo-2.4/controller/deploy/docker.py` & `rapydo-3.0/controller/deploy/docker.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 COMPOSE_SEP = "-"
 
 
 class Docker:
     def __init__(
         self, compose_files: Optional[List[Path]] = None, verify_swarm: bool = True
     ) -> None:
-
         if not compose_files:
             # Not all commands initialize Application.data
             # e.g. init does not
             if hasattr(Application, "data"):
                 compose_files = Application.data.files
 
         if compose_files:
@@ -81,15 +80,14 @@
         if node.status.addr == manager_address:
             return self.client
 
         return DockerClient(host=self.get_engine(node.status.addr))
 
     @classmethod
     def get_engine(cls, engine: Optional[str]) -> Optional[str]:
-
         if not engine:
             return None
 
         if engine == MAIN_NODE:
             return None
 
         if "@" not in engine:
@@ -113,15 +111,14 @@
     def get_running_services(self) -> Set[str]:
         if Configuration.swarm_mode:
             return self.swarm.get_running_services()
         else:
             return self.compose.get_running_services()
 
     def get_containers(self, service: str) -> Dict[int, Tuple[str, str]]:
-
         containers: Dict[int, Tuple[str, str]] = {}
         service_name = self.get_service(service)
 
         if Configuration.swarm_mode:
             try:
                 for task in self.client.service.ps(service_name):
                     if task.status.state not in ("running", "starting", "ready"):
@@ -157,15 +154,14 @@
                 containers.setdefault(slot, (c.name, MAIN_NODE))
         return containers
 
     def get_container_name(self, service_name: str, slot: int = 1) -> str:
         return f"{service_name}{COMPOSE_SEP}{slot}"
 
     def get_container(self, service: str, slot: int = 1) -> Optional[Tuple[str, str]]:
-
         if Configuration.swarm_mode:
             tasks = self.get_containers(service)
             # the 0 index is found in case of containers in global mode, like the proxy
             return tasks.get(slot) or tasks.get(0)
 
         service_name = self.get_service(service)
         c = self.get_container_name(service_name, slot=slot)
@@ -198,15 +194,14 @@
         # Dict[int, Tuple[str, str]] == return of get_containers
         containers: Union[str, Tuple[str, str], Dict[int, Tuple[str, str]]],
         user: Optional[str],
         command: Optional[str] = None,
         # this basically force tty=False
         force_output_return: bool = False,
     ) -> Optional[Union[str, Iterable[Tuple[str, bytes]]]]:
-
         if isinstance(containers, str):
             containers = (
                 containers,
                 MAIN_NODE,
             )
 
         if isinstance(containers, tuple):
@@ -216,15 +211,14 @@
 
         broadcast = len(containers_list) > 1
 
         # Important security note: never log the command command because it can
         # contain sensitive data, for example when used from change password command
         tty = not force_output_return and sys.stdout.isatty()
         for container in containers_list:
-
             try:
                 client = self.connect_engine(container[1])
                 if client.client_config.host:
                     log.info(
                         "Executing command on {}:{}",
                         client.client_config.host,
                         container[0],
@@ -259,15 +253,14 @@
 
                         if isinstance(line, bytes):
                             line = line.decode("UTF-8")
 
                         print(line.strip())
 
             except DockerException as e:
-
                 m = re.search(r"It returned with code (\d+)\n", str(e))
                 if not m:
                     log.debug("Catched exception does not contains any valid exit code")
                     raise e
 
                 exit_code = m.group(1)
```

### Comparing `rapydo-2.4/controller/deploy/registry.py` & `rapydo-3.0/controller/deploy/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     def get_host() -> str:
         registry_host = Application.env["REGISTRY_HOST"]
         registry_port = Application.env["REGISTRY_PORT"]
 
         return f"{registry_host}:{registry_port}"
 
     def ping(self, do_exit: bool = True) -> bool:
-
         registry_host = Application.env["REGISTRY_HOST"]
         registry_port = int(Application.env.get("REGISTRY_PORT", "5000") or "5000")
 
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
             sock.settimeout(1)
             try:
                 result = sock.connect_ex((registry_host, registry_port))
@@ -49,74 +48,72 @@
 
             return False
 
     @staticmethod
     def send_request(
         url: str, check_status: bool = True, method: str = "GET", version: str = "2"
     ) -> Response:
-
         if version == "2":
             headers = {"Accept": "application/vnd.docker.distribution.manifest.v2+json"}
         else:
             headers = {}
         if method == "DELETE":
             expected_status = 202
             method_ref = requests.delete
 
         else:
             expected_status = 200
             method_ref = requests.get
 
+        user = str(Application.env["REGISTRY_USERNAME"])
+        password = str(Application.env["REGISTRY_PASSWORD"])
+        if not user or not password:  # pragma: no cover
+            print_and_exit("Invalid registry username or password")
+
         r = method_ref(
             url,
             verify=False,
-            auth=HTTPBasicAuth(
-                Application.env["REGISTRY_USERNAME"],
-                Application.env["REGISTRY_PASSWORD"],
-            ),
+            auth=HTTPBasicAuth(user, password),
             headers=headers,
         )
 
         if check_status and r.status_code != expected_status:
             print_and_exit(
                 "The registry responded with an unexpected status {} ({} {})",
                 str(r.status_code),
                 method,
                 url,
             )
 
         return r
 
     def verify_image(self, image: str) -> bool:
-
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
         registry = self.get_host()
         host = f"https://{registry}"
         repository, tag = image.split(":")
         r = self.send_request(
             f"{host}/v2/{repository}/manifests/{tag}", check_status=False
         )
 
         if r.status_code == 401:  # pragma: no cover
             print_and_exit("Access denied to {} registry", host)
 
         return r.status_code == 200
 
     def login(self) -> None:
-
         registry = self.get_host()
         try:
             self.docker.login(
                 server=registry,
                 username=cast(str, Application.env["REGISTRY_USERNAME"]),
                 password=cast(str, Application.env["REGISTRY_PASSWORD"]),
             )
         except DockerException as e:
             if "docker login --username" in str(e):
-
                 settings = f"""
 {{
   "insecure-registries" : ["{registry}"]
 }}
 """
 
                 print_and_exit(
```

### Comparing `rapydo-2.4/controller/deploy/swarm.py` & `rapydo-3.0/controller/deploy/swarm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Integration with Docker swarm
 """
+
 from typing import Dict, List, Optional, Set, Union
 
 from glom import glom
 from python_on_whales import Service
 from python_on_whales.exceptions import NoSuchService, NotASwarmManager
 
 from controller import COMPOSE_FILE, RED, colors, log, print_and_exit
@@ -12,39 +13,36 @@
 from controller.deploy.docker import Docker
 from controller.utilities import system
 from controller.utilities.tables import print_table
 
 
 class Swarm:
     def __init__(self, docker: Docker, check_initialization: bool = True):
-
         self.docker_wrapper = docker
         self.docker = self.docker_wrapper.client
 
         if check_initialization and not self.get_token():
             print_and_exit(
                 "Swarm is not initialized, please execute {command}",
                 command=RED("rapydo init"),
             )
 
     def init(self) -> None:
-
         manager_address = str(
             Application.env.get("SWARM_MANAGER_ADDRESS")
             or system.get_local_ip(Configuration.production)
         )
 
         log.info("Initializing Swarm with manager IP {}", manager_address)
         self.docker.swarm.init(advertise_address=manager_address)
 
     def get_token(self, node_type: str = "manager") -> Optional[str]:
         try:
             return str(self.docker.swarm.join_token(node_type))
         except NotASwarmManager:
-
             return None
 
     @staticmethod
     def get_replicas(service: Service) -> int:
         if not service.spec.mode or "Global" in service.spec.mode:
             return 1
 
@@ -54,51 +52,54 @@
         stack = Configuration.project
         for s in self.docker.stack.list():
             if s.name == stack:
                 return True
         return False
 
     def get_running_services(self) -> Set[str]:
-
         prefix = f"{Configuration.project}_"
         containers = set()
         for service in self.docker.service.list():
             name = service.spec.name
+            if name is None:  # pragma: no cover
+                log.warning("Got null name for {}", service)
+                continue
             if not name.startswith(prefix):
                 continue
 
             for task in self.docker.service.ps(name):
                 status = task.status.state
                 if status != "running" and status != "starting" and status != "ready":
                     continue
 
                 # to be replaced with removeprefix
                 name = name[len(prefix) :]
                 containers.add(name)
         return containers
 
     def get_services_status(self, prefix: str) -> Dict[str, str]:
-
         prefix += "_"
         services_status: Dict[str, str] = dict()
         for service in self.docker.service.list():
             name = service.spec.name
+            if name is None:  # pragma: no cover
+                log.warning("Got null name for {}", service)
+                continue
             if not name.startswith(prefix):
                 continue
 
             for task in self.docker.service.ps(name):
-                status = task.status.state
+                status = task.status.state or "N/A"
 
                 # to be replaced with removeprefix
                 name = name[len(prefix) :]
                 services_status[name] = status
         return services_status
 
     def deploy(self) -> None:
-
         self.docker.stack.deploy(
             name=Configuration.project,
             compose_files=COMPOSE_FILE,
             resolve_image="always",
             prune=True,
             with_registry_auth=True,
         )
@@ -112,73 +113,88 @@
             scales: Dict[Union[str, Service], int] = {}
             scales[service_name] = 1
             self.docker.service.scale(scales, detach=True)
         else:
             self.docker.service.update(service_name, force=True, detach=True)
 
     def status(self, services: List[str]) -> None:
-
         nodes: Dict[str, str] = {}
         nodes_table: List[List[str]] = []
         headers = ["Role", "State", "Name", "IP", "CPUs", "RAM", "LABELS", "Version"]
         for node in self.docker.node.list():
-            nodes[node.id] = node.description.hostname
-
-            state = f"{node.status.state.title()}+{node.spec.availability.title()}"
-            cpu = str(round(node.description.resources.nano_cpus / 1000000000))
-            ram = system.bytes_to_str(node.description.resources.memory_bytes)
+            node_hostname = node.description.hostname or "N/A"
+            node_addr = node.status.addr or "N/A"
+            nodes[node.id] = node_hostname
+
+            state = cpu = ram = ""
+            if node.status.state and node.spec.availability:
+                state = f"{node.status.state.title()}+{node.spec.availability.title()}"
+            if node.description.resources and node.description.resources.nano_cpus:
+                cpu = str(round(node.description.resources.nano_cpus / 1000000000))
+            if node.description.resources and node.description.resources.memory_bytes:
+                ram = system.bytes_to_str(node.description.resources.memory_bytes)
 
             if state == "Ready+Active":
                 p = "[bold green]"
                 s = "[/bold green]"
             else:
                 p = "[bold red]"
                 s = "[/bold red]"
 
+            node_role = "N/A"
+            if node.spec.role:
+                node_role = node.spec.role.title()
+
+            node_labels = ""
+            if node.spec.labels:
+                node_labels = ",".join(node.spec.labels)
+
+            engine_version = "N/A"
+            if node.description.engine and node.description.engine.engine_version:
+                engine_version = f"v{node.description.engine.engine_version}"
+
             nodes_table.append(
                 [
-                    p + (node.spec.role.title()) + s,
+                    p + (node_role) + s,
                     p + (state) + s,
-                    p + (node.description.hostname) + s,
-                    p + (node.status.addr) + s,
+                    p + (node_hostname) + s,
+                    p + (node_addr) + s,
                     p + (cpu) + s,
                     p + (ram) + s,
-                    p + (",".join(node.spec.labels)) + s,
-                    p + (f"v{node.description.engine.engine_version}") + s,
+                    p + (node_labels) + s,
+                    p + (engine_version) + s,
                 ]
             )
 
         print_table(headers, nodes_table, table_title="Cluster status")
         stack_services = self.docker.service.list()
 
         print("")
 
         if not stack_services:
             log.info("No service is running")
             return
 
         prefix = f"{Configuration.project}_"
         for service in stack_services:
-
-            service_name = service.spec.name
+            service_name = service.spec.name or "N/A"
 
             tmp_service_name = service_name
             if tmp_service_name.startswith(prefix):
                 # to be replaced with removeprefix
                 tmp_service_name = tmp_service_name[len(prefix) :]
             if tmp_service_name not in services:
                 continue
 
             print(f"{colors.RESET}Inspecting {service_name}...", end="\r")
 
             tasks_lines: List[str] = []
 
             running_tasks = 0
             for task in self.docker.service.ps(service_name):
-
                 if task.status.state == "shutdown" or task.status.state == "complete":
                     COLOR = colors.BLUE
                 elif task.status.state == "running":
                     COLOR = colors.GREEN
                     running_tasks += 1
                 elif task.status.state == "starting" or task.status.state == "ready":
                     COLOR = colors.YELLOW
@@ -194,15 +210,17 @@
                     slot = " \\_ [H]"
                     container_name = f"{service_name}.{task.node_id}.{task.id}"
 
                 node_name = nodes.get(task.node_id, "")
                 status = f"{COLOR}{task.status.state:8}{colors.RESET}"
                 errors = f"err={task.status.err}" if task.status.err else ""
                 labels = ",".join(task.labels)
-                ts = task.status.timestamp.strftime("%d-%m-%Y %H:%M:%S")
+                ts = "N/A"
+                if task.status.timestamp:
+                    ts = task.status.timestamp.strftime("%d-%m-%Y %H:%M:%S")
 
                 tasks_lines.append(
                     "\t".join(
                         (
                             slot,
                             status,
                             ts,
@@ -230,30 +248,35 @@
                 ports_list = [
                     f"{p.published_port}->{p.target_port}"
                     for p in service.endpoint.ports
                 ]
             else:
                 ports_list = []
 
-            image = service.spec.task_template.container_spec.image.split("@")[0]
+            image = "N/A"
+            if (
+                service.spec.task_template
+                and service.spec.task_template.container_spec
+                and service.spec.task_template.container_spec.image
+            ):
+                image = service.spec.task_template.container_spec.image.split("@")[0]
             ports = ",".join(ports_list)
             print(
                 f"{COLOR}{service_name:23}{colors.RESET} [{replicas}] {image}\t{ports}"
             )
 
             for line in tasks_lines:
                 print(line)
 
             print("")
 
     def remove(self) -> None:
         self.docker.stack.remove(Configuration.project)
 
     def logs(self, service: str, follow: bool, tail: int, timestamps: bool) -> None:
-
         if service not in Application.data.active_services:
             print_and_exit("No such service: {}", service)
 
         service_name = self.docker_wrapper.get_service(service)
 
         try:
             # lines: Iterable[Tuple[str, bytes]] due to stream=True
@@ -295,34 +318,36 @@
         for service in Application.data.active_services:
             config = Application.data.compose_config[service]
 
             # frontend container has no deploy options
             if not config.deploy:
                 continue
 
-            if config.deploy.resources.reservations:
+            if config.deploy.resources and config.deploy.resources.reservations:
                 # int() are needed because python on whales 0.25 extended type of
                 # cpus and replicas to Union[float, str] according to compose-cli typing
 
-                cpus = int(config.deploy.resources.reservations.cpus) or 0
-                memory = config.deploy.resources.reservations.memory
+                cpus = int(config.deploy.resources.reservations.cpus or 0)
+                memory = config.deploy.resources.reservations.memory or 0
 
                 # the proxy container is now defined as global and without any replicas
                 # => replicas is None => defaulted to 1
                 replicas = int(config.deploy.replicas or 1)
 
                 total_cpus += replicas * cpus
                 total_memory += replicas * memory
 
         nodes_cpus = 0.0
         nodes_memory = 0.0
         for node in self.docker.node.list():
-
-            nodes_cpus += round(node.description.resources.nano_cpus / 1000000000)
-            nodes_memory += node.description.resources.memory_bytes
+            if node.description.resources:
+                nodes_cpus += round(
+                    (node.description.resources.nano_cpus or 0) / 1000000000
+                )
+                nodes_memory += node.description.resources.memory_bytes or 0
 
         if total_cpus > nodes_cpus:
             log.critical(
                 "Your deployment requires {} cpus but your nodes only have {}",
                 total_cpus,
                 nodes_cpus,
             )
```

### Comparing `rapydo-2.4/controller/packages.py` & `rapydo-3.0/controller/packages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Utilities to work with python packages and binaries
 """
+
 # WARNING: to not import this package at startup,
 # but only into functions otherwise pip will go crazy
 # (we cannot understand why, but it does!)
 
 import hashlib
 import os
 import re
@@ -23,42 +24,46 @@
 )
 from python_on_whales import docker
 from sultan.api import Sultan  # type: ignore
 
 from controller import RED, log, print_and_exit
 
 # https://get.docker.com
-EXPECTED_DOCKER_SCRIPT_MD5 = "f0914813fcbbe35f1358a994cff812d3"
+EXPECTED_DOCKER_SCRIPT_MD5 = "21991ad5158db696823e3fd54eab00da"
 
 # https://github.com/docker/compose/releases
-COMPOSE_VERSION = "v2.9.0"
-EXPECTED_COMPOSE_LINUX_BIN_MD5 = "d098bb8304809a1335e0cf2c18d424db"
-EXPECTED_COMPOSE_MACOS_BIN_MD5 = "e7ce20441172f1e9f2c17688fe7e76a5"
+COMPOSE_VERSION = "v2.24.6"
+EXPECTED_COMPOSE_LINUX_BIN_MD5 = "593fb55fe05a76d5c5efb383e91ba129"
+EXPECTED_COMPOSE_MACOS_BIN_MD5 = "e9b48a919560f33710530ef6f18e26a1"
 EXPECTED_COMPOSE_WIN_BIN_MD5 = "not-implemented"
 
 # https://github.com/docker/buildx/releases
-BUILDX_VERSION = "v0.9.1"
-EXPECTED_BUILDX_LINUX_BIN_MD5 = "1f4ac4fbe0780d478caf7ac1806f186a"
-EXPECTED_BUILDX_MACOS_BIN_MD5 = "b259567a4cf3bb99bfbfe0e02baf2c76"
+BUILDX_VERSION = "v0.13.1"
+EXPECTED_BUILDX_LINUX_BIN_MD5 = "c7145e327f600f8e960f74f336926ecd"
+EXPECTED_BUILDX_MACOS_BIN_MD5 = "71a155d9a6f20510e2b7df0298e6291b"
 EXPECTED_BUILDX_WIN_BIN_MD5 = "not-implemented"
 
+DEFAULT_PIP_BIN = "pip3"
+ALTERNATIVE_PIP_BIN = "pip"
+
 
 class ExecutionException(Exception):
     pass
 
 
 class Packages:
     @staticmethod
-    def install(package: Union[str, Path], editable: bool) -> None:
+    def install(
+        package: Union[str, Path], editable: bool, pip_bin: str = DEFAULT_PIP_BIN
+    ) -> None:
         """
         Install a python package in editable or normal mode
         """
 
         try:
-
             options = ["install", "--upgrade"]
 
             home = Path.home()
 
             if editable:
                 if sys.platform != "darwin" and sys.platform != "win32":
                     options.append("--prefix")
@@ -66,20 +71,22 @@
                 options.append("--editable")
             else:
                 options.append("--user")
 
             # Note: package is a Path if editable, str otherwise
             options.append(str(package))
 
-            output = Packages.execute_command("pip3", options)
+            output = Packages.execute_command(pip_bin, options)
 
             for r in output.split("\n"):
                 print(r)
 
         except Exception as e:  # pragma: no cover
+            if pip_bin == DEFAULT_PIP_BIN:
+                return Packages.install(package, editable, pip_bin=ALTERNATIVE_PIP_BIN)
             print_and_exit(str(e))
 
     @staticmethod
     def check_program(
         program: str,
         min_version: Optional[str] = None,
         max_version: Optional[str] = None,
@@ -87,15 +94,14 @@
     ) -> str:
         """
         Verify if a binary exists and (optionally) its version
         """
 
         found_version = Packages.get_bin_version(program)
         if found_version is None:
-
             hints = ""
             if program == "docker":  # pragma: no cover
                 install_cmd = RED("rapydo install docker")
                 hints = "\n\nTo install docker visit: https://get.docker.com"
                 hints += f"or execute {install_cmd}"
 
             print_and_exit(
@@ -140,22 +146,27 @@
         """
         if exec_cmd == "docker":
             return "docker.exe"
         return exec_cmd
 
     @classmethod
     def get_bin_version(
-        cls, exec_cmd: str, option: List[str] = ["--version"], clean_output: bool = True
+        cls,
+        exec_cmd: str,
+        option: Optional[List[str]] = None,
+        clean_output: bool = True,
     ) -> Optional[str]:
         """
         Retrieve the version of a binary
         """
 
-        try:
+        if option is None:
+            option = ["--version"]
 
+        try:
             if os.name == "nt":  # pragma: no cover
                 exec_cmd = cls.convert_bin_to_win32(exec_cmd)
 
             output = Packages.execute_command(exec_cmd, option)
 
             if clean_output:
                 # then last element on spaces
@@ -174,33 +185,44 @@
             # That's all... this magic receipt is able to extract
             # version information from most of outputs, e.g.
             # Python 3.8.2
             # Docker version 19.03.8, build afacb8b7f0
             # git version 2.25.1
             # rapydo version 0.7.x
             return output
-            # Note that in may other cases it fails...
+            # Note that in many other cases it fails...
             # but we are interested in a very small list of programs, so it's ok
             # echo --version -> --version
             # ls --version -> ls
             # pip3 --version -> a path
         except ExecutionException as e:
             log.error(e)
 
         return None
 
     @staticmethod
-    def get_installation_path(package: str = "rapydo") -> Optional[Path]:
+    def get_installation_path(
+        package: str = "rapydo", pip_bin: str = DEFAULT_PIP_BIN
+    ) -> Optional[Path]:
         """
         Retrieve the controller installation path, if installed in editable mode
         """
-        for r in Packages.execute_command("pip3", ["list", "--editable"]).split("\n"):
-            if r.startswith(f"{package} "):
-                tokens = re.split(r"\s+", r)
-                return Path(str(tokens[2]))
+        try:
+            for r in Packages.execute_command(pip_bin, ["list", "--editable"]).split(
+                "\n"
+            ):
+                if r.startswith(f"{package} "):
+                    tokens = re.split(r"\s+", r)
+                    return Path(str(tokens[2]))
+        except Exception as e:  # pragma: no cover
+            if pip_bin == DEFAULT_PIP_BIN:
+                return Packages.get_installation_path(
+                    package, pip_bin=ALTERNATIVE_PIP_BIN
+                )
+            print_and_exit(str(e))
 
         return None
 
     @staticmethod
     def download(url: str, expected_checksum: str) -> Path:
         try:
             r = requests.get(url, timeout=10)
@@ -316,23 +338,22 @@
 
         v = docker.buildx.version()
         log.info("Docker buildx installed version: {}", v)
 
     @staticmethod
     def execute_command(command: str, parameters: List[str]) -> str:
         try:
-
             # Pattern in plumbum library for executing a shell command
             local_command = local[command]
             log.info("Executing command {} {}", command, " ".join(parameters))
             return str(local_command(parameters))
-        except CommandNotFound:
-            raise ExecutionException(f"Command not found: {command}")
+        except CommandNotFound as e:
+            raise ExecutionException(f"Command not found: {command}") from e
 
-        except ProcessExecutionError:
+        except ProcessExecutionError as e:
             raise ExecutionException(
                 f"Cannot execute command: {command} {' '.join(parameters)}"
-            )
+            ) from e
 
         # raised on Windows
-        except OSError:  # pragma: no cover
-            raise ExecutionException(f"Cannot execute: {command}")
+        except OSError as e:  # pragma: no cover
+            raise ExecutionException(f"Cannot execute: {command}: {e}") from e
```

### Comparing `rapydo-2.4/controller/project.py` & `rapydo-3.0/controller/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Utilities to handle projects' structure
 """
+
 import os
 import re
 from pathlib import Path
 from typing import List, Optional
 
 from controller import (
     BACKUP_DIR,
@@ -45,15 +46,14 @@
 
     def p_path(self, *args: str) -> Path:
         return PROJECT_DIR.joinpath(self.project, *args)
 
     def load_project_scaffold(
         self, project: str, auth: Optional[str], services: Optional[List[str]] = None
     ) -> bool:
-
         if services is None:
             services = []
 
         self.project = project
         self.expected_folders.extend(self.expected_main_folders)
         self.expected_folders.append(self.p_path("confs"))
         self.expected_folders.append(self.p_path("builds"))
@@ -96,15 +96,14 @@
         self.expected_files.append(Path(".flake8"))
         self.expected_files.append(Path(".prettierignore"))
 
         self.fixed_files.append(Path(".gitattributes"))
         self.fixed_files.append(Path("pyproject.toml"))
 
         if auth or services:
-
             models = self.p_path("backend", "models")
             if auth == "sqlalchemy" or "postgres" in services:
                 self.expected_files.append(models.joinpath("sqlalchemy.py"))
             if auth == "neo4j" or "neo4j" in services:
                 self.expected_files.append(models.joinpath("neo4j.py"))
 
         self.optionals_folders.append(self.p_path("backend", "models", "emails"))
@@ -144,14 +143,16 @@
         # Removed since 0.9
         self.obsolete_files.append(self.p_path("backend", "initialization"))
         self.obsolete_files.append(self.p_path("frontend", "assets", "favicon.ico"))
         # Removed since 1.2
         self.obsolete_files.append(Path(".pre-commit-config.yaml"))
         # Removed since 2.3
         self.obsolete_files.append(Path(".isort.cfg"))
+        # Removed since 3.0
+        self.obsolete_files.append(SUBMODULES_DIR.joinpath("build-templates"))
         return True
 
     def load_frontend_scaffold(self, frontend: Optional[str]) -> bool:
         self.frontend = frontend
 
         if self.frontend is None or self.frontend == NO_FRONTEND:
             log.debug("No frontend framework enabled")
@@ -183,14 +184,15 @@
                     self.p_path("frontend", "styles", "variables.scss"),
                     self.p_path("frontend", "app", "customization.ts"),
                     self.p_path("frontend", "app", "custom.module.ts"),
                     self.p_path("frontend", "app", "custom.navbar.ts"),
                     self.p_path("frontend", "app", "custom.footer.ts"),
                     self.p_path("frontend", "app", "custom.profile.ts"),
                     self.p_path("frontend", "app", "custom.navbar.links.html"),
+                    self.p_path("frontend", "app", "custom.navbar.controls.html"),
                     self.p_path("frontend", "app", "custom.navbar.brand.html"),
                     self.p_path("frontend", "app", "custom.footer.html"),
                     self.p_path("frontend", "app", "custom.profile.html"),
                     self.p_path("frontend", "app", "types.ts"),
                 ]
             )
             self.raw_files.extend(
@@ -262,24 +264,21 @@
                 ]
             )
 
         return True
 
     @staticmethod
     def get_project(project: Optional[str], ignore_multiples: bool = False) -> str:
-
         projects = os.listdir(PROJECT_DIR)
 
         if project is None:
-
             if len(projects) == 0:
                 print_and_exit("No project found (is {} folder empty?)", PROJECT_DIR)
 
             if len(projects) > 1:
-
                 # It is used by the preliminary get used to load the commands
                 # In case of multiple projects without a proper definition in
                 # projectrc, the custom commands will not be loaded
                 if ignore_multiples:
                     return ""
 
                 print_and_exit(
@@ -309,15 +308,14 @@
 
     @staticmethod
     def check_invalid_characters(project: str) -> None:
         if len(project) <= 1:
             print_and_exit("Wrong project name, expected at least two characters")
 
         if not re.match("^[a-z][a-z0-9]+$", project):
-
             # First character is expected to be a-z
             tmp_str = re.sub("[a-z]", "", project[0])
             # Other characters are expected to be a-z 0-9
             tmp_str += re.sub("[a-z0-9]", "", project[1:])
             invalid_list = list(set(tmp_str))
             invalid_list.sort()
             invalid_chars = "".join(str(e) for e in invalid_list)
@@ -367,24 +365,22 @@
             return f"""You are not in a git repository
 \nPlease note that this command only works from inside a rapydo-like repository
 Verify that you are in the right folder, now you are in: {Path.cwd()}
                 """
 
         for fpath in self.expected_main_folders:
             if not folder.joinpath(fpath).is_dir():
-
                 return f"""Folder not found: {fpath}
 \nPlease note that this command only works from inside a rapydo-like repository
 Verify that you are in the right folder, now you are in: {Path.cwd()}
                     """
 
         return None
 
     def inspect_project_folder(self) -> None:
-
         for fpath in self.expected_folders:
             if not fpath.is_dir():
                 print_and_exit(
                     "Project {} is invalid: required folder not found {}",
                     self.project,
                     fpath,
                 )
@@ -415,15 +411,14 @@
         "click",
         "collections",
         "datetime",
         "dateutil",
         "email",
         "errno",
         "flask",
-        "flask_sqlalchemy",
         "authlib",
         "functools",
         "glob",
         "hashlib",
         "hmac",
         "inspect",
         "io",
```

### Comparing `rapydo-2.4/controller/templates/android-chrome-192x192.png` & `rapydo-3.0/controller/templates/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/apple-touch-icon.png` & `rapydo-3.0/controller/templates/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/blocked_credentials.html.j2` & `rapydo-3.0/controller/templates/blocked_credentials.html.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/codeql-analysis.yml.j2` & `rapydo-3.0/controller/templates/codeql-analysis.yml.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/component_template.html.j2` & `rapydo-3.0/controller/templates/component_template.html.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/component_template.ts.j2` & `rapydo-3.0/controller/templates/component_template.ts.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/component_test_template.spec.ts.j2` & `rapydo-3.0/controller/templates/component_test_template.spec.ts.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/custom.module.ts.j2` & `rapydo-3.0/controller/templates/custom.module.ts.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/custom.navbar.links.html.j2` & `rapydo-3.0/controller/templates/custom.navbar.links.html.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/custom.navbar.ts.j2` & `rapydo-3.0/controller/templates/custom.navbar.ts.j2`

 * *Files 9% similar despite different names*

```diff
@@ -36,7 +36,23 @@
   constructor() {
     var t = environment.projectTitle;
     t = t.replace(/^'/, "");
     t = t.replace(/'$/, "");
     this.project = t;
   }
 }
+
+@Component({
+  selector: "customcontrols",
+  templateUrl: "custom.navbar.controls.html",
+  changeDetection: ChangeDetectionStrategy.OnPush,
+})
+export class CustomControlsComponent {
+  @Input() user: User;
+  @Output() onClick: EventEmitter<null> = new EventEmitter<null>();
+
+  constructor() {}
+
+  public collapse() {
+    this.onClick.emit();
+  }
+}
```

### Comparing `rapydo-2.4/controller/templates/customization.py.j2` & `rapydo-3.0/controller/templates/customization.py.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/customization.ts.j2` & `rapydo-3.0/controller/templates/customization.ts.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/cypress_template.spec.ts.j2` & `rapydo-3.0/controller/templates/cypress_template.spec.ts.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/endpoint_template.py.j2` & `rapydo-3.0/controller/templates/endpoint_template.py.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/endpoint_test_template.py.j2` & `rapydo-3.0/controller/templates/endpoint_test_template.py.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/favicon-16x16.png` & `rapydo-3.0/controller/templates/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/favicon-32x32.png` & `rapydo-3.0/controller/templates/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/favicon.ico` & `rapydo-3.0/controller/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/github_actions-backend.yml.j2` & `rapydo-3.0/controller/templates/github_actions-backend.yml.j2`

 * *Files 12% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 
 jobs:
   Development-mode:
     runs-on: ubuntu-latest
     timeout-minutes: 45
 
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - uses: rapydo/actions/install@v2
         with:
           project: ${PROJECT}
+          extra_options: "-e FRONTEND_FRAMEWORK=nofrontend"
           # swarm: 1
 
       - name: Run Pytest
         run: |
 
           rapydo pull --quiet
           # If a custom build is added
@@ -66,27 +67,27 @@
         run: rapydo logs
 
   Production-mode:
     runs-on: ubuntu-latest
     timeout-minutes: 45
 
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - uses: rapydo/actions/install@v2
         with:
           project: ${PROJECT}
           # swarm: 1
 
       - name: Production mode
         run: |
-          rapydo --testing --prod init --force
+          rapydo --testing --prod -e FRONTEND_FRAMEWORK=nofrontend init --force
           # rapydo run registry
           rapydo pull --quiet
 
           # If a custom build is added
           # rapydo build
 
           rapydo ssl --volatile
```

### Comparing `rapydo-2.4/controller/templates/github_actions-cypress.yml.j2` & `rapydo-3.0/controller/templates/github_actions-cypress.yml.j2`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 jobs:
   Cypress:
     runs-on: ubuntu-latest
     timeout-minutes: 60
 
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - uses: rapydo/actions/install@v2
         with:
           project: ${PROJECT}
           # swarm: 1
```

### Comparing `rapydo-2.4/controller/templates/github_actions-frontend.yml.j2` & `rapydo-3.0/controller/templates/github_actions-frontend.yml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 jobs:
   Development-mode:
     runs-on: ubuntu-latest
     timeout-minutes: 25
 
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - uses: rapydo/actions/install@v2
         with:
           project: ${PROJECT}
           # swarm: 1
@@ -50,16 +50,16 @@
           codecov_token: {% raw -%}${{ secrets.CODECOV_TOKEN }}{% endraw %}
 
   Production-mode:
     runs-on: ubuntu-latest
     timeout-minutes: 25
 
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - uses: rapydo/actions/install@v2
         with:
           project: ${PROJECT}
           # swarm: 1
```

### Comparing `rapydo-2.4/controller/templates/gitignore.j2` & `rapydo-3.0/controller/templates/gitignore.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/initialization.py.j2` & `rapydo-3.0/controller/templates/initialization.py.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/mstile-150x150.png` & `rapydo-3.0/controller/templates/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/neo4j.py.j2` & `rapydo-3.0/controller/templates/neo4j.py.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/project_configuration.yaml.j2` & `rapydo-3.0/controller/templates/project_configuration.yaml.j2`

 * *Files 4% similar despite different names*

```diff
@@ -21,23 +21,21 @@
   # roles_descriptions:
   #   normal_user: User Custom Description
   #   staff_user: Staff Custom Description
   #   group_coordinator: Group Coordinator Custom Description
   #   admin_root: Administrator Custom Description
   #   extra_role: Custom Role Description
 
-  submodules:
-    http-api:
-      # branch: "http-api-branch"
-    build-templates:
-      # branch: "build-templates-branch"
-    rapydo-angular:
-      # branch: "rapydo-angular-branch"
-    do:
-      # branch: "do-branch"
+  # submodules:
+  #   http-api:
+  #     branch: "http-api-branch"
+  #   rapydo-angular:
+  #     branch: "rapydo-angular-branch"
+  #   do:
+  #     branch: "do-branch"
   env:
 
     {% if auth_service == "NO_AUTHENTICATION" -%}
     ACTIVATE_AUTH: 0
     {% else -%}
     AUTH_SERVICE: {{ auth_service }}
     {% endif -%}
```

### Comparing `rapydo-2.4/controller/templates/projectrc.j2` & `rapydo-3.0/controller/templates/projectrc.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/pyproject.toml.j2` & `rapydo-3.0/controller/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/safari-pinned-tab.svg` & `rapydo-3.0/controller/templates/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/semgrep-analysis.yml.j2` & `rapydo-3.0/controller/templates/semgrep-analysis.yml.j2`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 jobs:
   semgrep:
     name: Scan
     runs-on: ubuntu-latest
     container:
       image: returntocorp/semgrep
     # Skip any PR created by dependabot to avoid permission issues
-    if: (github.actor != 'dependabot[bot]')
+    if: (github.actor != 'renovate[bot]')
     steps:
       # Fetch project source
       - uses: actions/checkout@v3
 
       # Scan code using project's configuration on https://semgrep.dev/manage
       - run: semgrep ci --sarif --output=semgrep.sarif
         name: Run semgrep
```

### Comparing `rapydo-2.4/controller/templates/service_template.ts.j2` & `rapydo-3.0/controller/templates/service_template.ts.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/sink.html.j2` & `rapydo-3.0/controller/templates/sink.html.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templates/sink.ts.j2` & `rapydo-3.0/controller/templates/sink.ts.j2`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 import { FormlyService } from "@rapydo/services/formly";
 import { ApiService } from "@rapydo/services/api";
 import { NotificationService } from "@rapydo/services/notification";
 import { environment } from "@rapydo/../environments/environment";
 import { Schema, SchemaType } from "@rapydo/types";
 
-import * as moment from "moment";
-
 // === @swimlane/ngx-datatable/src/types/column-mode.type
 enum ColumnMode {
   standard = "standard",
   flex = "flex",
   force = "force",
 }
```

### Comparing `rapydo-2.4/controller/templates/task_template.py.j2` & `rapydo-3.0/controller/templates/task_template.py.j2`

 * *Files identical despite different names*

### Comparing `rapydo-2.4/controller/templating.py` & `rapydo-3.0/controller/templating.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Utilities to work with jinja2 templates
 """
+
 import filecmp
 import os
 import random
 import string
 from pathlib import Path
 from typing import Dict, List, Optional, TypedDict
 
@@ -73,15 +74,14 @@
         log.warning("Generated password is not strong enough, sampling again")
         return get_strong_password()
     return p
 
 
 class Templating:
     def __init__(self) -> None:
-
         self.template_dir = Path(__file__).resolve().parent.joinpath(TEMPLATE_DIR)
 
         if not self.template_dir.is_dir():
             print_and_exit("Template folder not found: {}", self.template_dir)
 
         log.debug("Template folder: {}", self.template_dir)
         loader = FileSystemLoader([TEMPLATE_DIR, self.template_dir])
@@ -93,15 +93,14 @@
             keep_trailing_newline=True,
         )
         self.env.filters["password"] = password
         self.env.filters["username"] = username
 
     @staticmethod
     def get_template_name(filename: str) -> str:
-
         if filename.startswith("."):
             filename = filename[1:]
 
         return f"{filename}.j2"
 
     def get_template(self, filename: str, data: TemplateDataType) -> str:
         try:
@@ -112,15 +111,14 @@
             return content
         except TemplateNotFound as e:
             print_and_exit("Template {} not found in: {}", str(e), self.template_dir)
         except UndefinedError as e:  # pragma: no cover
             print_and_exit(str(e))
 
     def save_template(self, filename: Path, content: str, force: bool = False) -> None:
-
         if filename.exists():
             if force:
                 self.make_backup(filename)
             # It is always verified before calling save_template from app, create & add
             else:  # pragma: no cover
                 print_and_exit("File {} already exists", filename)
 
@@ -130,12 +128,11 @@
     @staticmethod
     def make_backup(filename: Path) -> None:
         backup_filename = f"{filename}.bak"
         os.rename(filename, backup_filename)
         log.info("A backup of {} is saved as {}", filename, backup_filename)
 
     def file_changed(self, filename: str) -> bool:
-
         template = self.get_template_name(filename)
         return not filecmp.cmp(
             filename, os.path.join(self.template_dir, template), shallow=True
         )
```

### Comparing `rapydo-2.4/controller/utilities/configuration.py` & `rapydo-3.0/controller/utilities/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,33 @@
-import re
+import sys
 from copy import deepcopy
 from enum import Enum, IntEnum
 from pathlib import Path
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Iterator,
-    List,
-    Optional,
-    Tuple,
-    TypedDict,
-    Union,
-    cast,
-)
+from typing import Dict, List, Optional, Tuple, TypedDict, Union, cast
 
 import yaml
 from glom import glom
-from pydantic import (
-    BaseModel,
-    ConstrainedInt,
-    ConstrainedStr,
-    Extra,
-    PositiveInt,
-    PydanticValueError,
-    ValidationError,
-)
+from pydantic import BaseModel, ConfigDict, Field, PositiveInt, ValidationError
 
 from controller import (
     COMPOSE_FILE_VERSION,
     CONFS_DIR,
     PLACEHOLDER,
     EnvType,
     log,
     print_and_exit,
 )
 
+# py38
+if sys.version_info.major == 3 and sys.version_info.minor == 8:
+    from typing_extensions import Annotated
+else:
+    from typing import Annotated  # type: ignore
+
+
 PROJECTS_DEFAULTS_FILE = Path("projects_defaults.yaml")
 PROJECTS_PROD_DEFAULTS_FILE = Path("projects_prod_defaults.yaml")
 PROJECT_CONF_FILENAME = Path("project_configuration.yaml")
 
 
 class Project(TypedDict):
     title: str
@@ -67,20 +55,14 @@
 # But should be total=True in case of projects_defaults
 class Configuration(TypedDict, total=False):
     project: Project
     tags: Dict[str, str]
     variables: Variables
 
 
-class BACKEND_BUILD_MODE_VALUES(Enum):
-    backend = "backend"
-    backend_legacy38 = "backend-legacy38"
-    backend_legacy39 = "backend-legacy39"
-
-
 class FRONTEND_FRAMEWORK_VALUES(Enum):
     nofrontend = "nofrontend"
     angular = "angular"
 
 
 class FRONTEND_BUILD_MODE_VALUES(Enum):
     angular = "angular"
@@ -103,17 +85,18 @@
 
 class APP_MODE_VALUES(Enum):
     development = "development"
     production = "production"
     test = "test"
 
 
-class FLASK_ENV_VALUES(Enum):
-    development = "development"
-    production = "production"
+class BACKEND_PYTHON_VERSION_VALUES(Enum):
+    py311 = "v3.11"
+    py310 = "v3.10"
+    py39 = "v3.9"
 
 
 class PYTHONMALLOC_VALUES(Enum):
     empty = ""
     debug = "debug"
     malloc = "malloc"
     pymalloc = "pymalloc"
@@ -220,116 +203,52 @@
     false = "false"
 
 
 class PLACEHOLDER_VALUE(Enum):
     PLACEHOLDER_VALUE = PLACEHOLDER
 
 
-# Conflicts between pydantic and mypy
-# https://stackoverflow.com/questions/66924001/conflict-between-pydantic-constr-and-mypy-checking
-class Port(ConstrainedInt):
-    gt = 0
-    le = 65535
-
-
-class NullablePort(ConstrainedInt):
-    ge = 0
-    le = 65535
-
-
-class PasswordScore(ConstrainedInt):
-    ge = 0
-    le = 4
-
-
-class GzipCompressionLevel(ConstrainedInt):
-    ge = 1
-    le = 9
-
-
-class NonNegativeInt(ConstrainedInt):
-    ge = 0
-
-
-class AssignedCPU(ConstrainedStr):
-    regex = re.compile(r"^[0-9]+\.[0-9]+$")
-
-
-class AssignedMemory(ConstrainedStr):
-    regex = re.compile(r"^[0-9]+(M|G)$")
-
-
-class PostgresMem(ConstrainedStr):
-    regex = re.compile(r"^[0-9]+(KB|MB|GB)$")
-
-
-class Neo4jMem(ConstrainedStr):
-    regex = re.compile(r"^[0-9]+(K|M|G|k|m|g)$")
-
-
-class HealthcheckInterval(ConstrainedStr):
-    regex = re.compile(r"^[0-9]+(s|m|h)$")
-
-
-class Version(ConstrainedStr):
-    regex = re.compile(r"^[0-9]+(\.[0-9]+)+$")
+Port = Annotated[int, Field(gt=0, le=65535)]
+NullablePort = Annotated[int, Field(ge=0, le=65535)]
+PasswordScore = Annotated[int, Field(ge=0, le=4)]
+GzipCompressionLevel = Annotated[int, Field(ge=1, le=9)]
+NonNegativeInt = Annotated[int, Field(ge=0)]
+AssignedCPU = Annotated[str, Field(pattern=r"^[0-9]+\.[0-9]+$")]
+AssignedMemory = Annotated[str, Field(pattern=r"^[0-9]+(M|G)$")]
+PostgresMem = Annotated[str, Field(pattern=r"^[0-9]+(KB|MB|GB)$")]
+Neo4jMem = Annotated[str, Field(pattern="^[0-9]+(K|M|G|k|m|g)$")]
+HealthcheckInterval = Annotated[str, Field(pattern=r"^[0-9]+(s|m|h)$")]
+Version = Annotated[str, Field(pattern=r"^[0-9]+(\.[0-9]+)+$")]
 
 
 # most of bool variables were deprecated since 1.0
 # Backend and Frontend use different booleans due to Py vs Js
 # 0/1 is a much more portable value to prevent true|True|"true"
 # This fixes troubles in setting boolean values only used by Angular
 # (expected true|false) or used by Pyton (expected True|False)
 class zero_or_one(IntEnum):
     ZERO = 0
     ONE = 1
 
 
-class InvalidNeo4jFlag(PydanticValueError):
-    msg_template = "Invalid Neo4j flag, expected values are: true or false"
-
-
-class Neo4jFlag:
-    @classmethod
-    def __modify_schema__(cls, field_schema: Dict[str, Any]) -> None:
-        field_schema.update(type="boolean")
-
-    @classmethod
-    def __get_validators__(cls) -> Iterator[Callable[["Neo4jFlag", Any], bool]]:
-        yield cls.validate
-
-    def validate(cls, value: Any) -> bool:
-        if isinstance(value, bool):
-            return value
-
-        if value == "true":
-            return True
-
-        if value == "false":
-            return False
-
-        raise InvalidNeo4jFlag()
-
-
 class ProjectModel(BaseModel):
     title: str
     description: str
     keywords: str
     rapydo: Version
     version: str
 
 
 class SubmoduleModel(BaseModel):
     online_url: str
-    branch: Optional[str]
+    branch: Optional[str] = None
     _if: str
 
 
 class BaseEnvModel(BaseModel):
-    BACKEND_BUILD_MODE: BACKEND_BUILD_MODE_VALUES
     FRONTEND_FRAMEWORK: FRONTEND_FRAMEWORK_VALUES
     FRONTEND_BUILD_MODE: FRONTEND_BUILD_MODE_VALUES
     NETWORK_MTU: PositiveInt
     DOCKER_LOGGING_DRIVER: DOCKER_LOGGING_DRIVERS
     HEALTHCHECK_INTERVAL: HealthcheckInterval
     HEALTHCHECK_BACKEND_CMD: str
     LOG_LEVEL: LOG_LEVEL_VALUES
@@ -355,21 +274,21 @@
     MYPY_DISALLOW_UNTYPED_DEFS: zero_or_one
     MYPY_IGNORE_LIBS: str
     MYPY_ADD_LIBS: str
     MAX_LOGS_LENGTH: PositiveInt
     APP_MODE: APP_MODE_VALUES
     FLASK_HOST: str
     FLASK_DEFAULT_PORT: Port
-    FLASK_ENV: FLASK_ENV_VALUES
+    FLASK_DEBUG: zero_or_one
     API_AUTOSTART: zero_or_one
     BACKEND_PORT: Port
     BACKEND_API_PORT: Port
     BACKEND_URL: str
+    BACKEND_PYTHON_VERSION: BACKEND_PYTHON_VERSION_VALUES
     PYTHON_MAIN_FILE: str
-    PYTHON_PATH: Path
     PYTHONASYNCIODEBUG: zero_or_one
     PYTHONFAULTHANDLER: zero_or_one
     PYTHONMALLOC: PYTHONMALLOC_VALUES
     BACKEND_PREFIX: str
     APP_SECRETS: Path
     DATA_PATH: Path
     DATA_IMPORT_FOLDER: Path
@@ -381,28 +300,28 @@
     GZIP_COMPRESSION_THRESHOLD: PositiveInt
     GZIP_COMPRESSION_LEVEL: GzipCompressionLevel
     ALEMBIC_AUTO_MIGRATE: zero_or_one
     PROXY_HOST: str
     PROXY_DEV_PORT: Port
     PROXY_PROD_PORT: Port
     PROXIED_CONNECTION: zero_or_one
-    DOMAIN_ALIASES: Optional[str]
-    SET_UNSAFE_EVAL: Optional[str]
-    SET_UNSAFE_INLINE: Optional[str]
-    SET_STYLE_UNSAFE_INLINE: Optional[str]
-    SET_CSP_SCRIPT_SRC: Optional[str]
-    SET_CSP_IMG_SRC: Optional[str]
-    SET_CSP_FONT_SRC: Optional[str]
-    SET_CSP_CONNECT_SRC: Optional[str]
-    SET_CSP_FRAME_SRC: Optional[str]
+    DOMAIN_ALIASES: Optional[str] = None
+    SET_UNSAFE_EVAL: Optional[str] = None
+    SET_UNSAFE_INLINE: Optional[str] = None
+    SET_STYLE_UNSAFE_INLINE: Optional[str] = None
+    SET_CSP_SCRIPT_SRC: Optional[str] = None
+    SET_CSP_IMG_SRC: Optional[str] = None
+    SET_CSP_FONT_SRC: Optional[str] = None
+    SET_CSP_CONNECT_SRC: Optional[str] = None
+    SET_CSP_FRAME_SRC: Optional[str] = None
     SET_MAX_REQUESTS_PER_SECOND_AUTH: PositiveInt
     SET_MAX_REQUESTS_BURST_AUTH: PositiveInt
     SET_MAX_REQUESTS_PER_SECOND_API: PositiveInt
     SET_MAX_REQUESTS_BURST_API: PositiveInt
-    CORS_ALLOWED_ORIGIN: Optional[str]
+    CORS_ALLOWED_ORIGIN: Optional[str] = None
     SSL_VERIFY_CLIENT: zero_or_one
     SSL_FORCE_SELF_SIGNED: zero_or_one
 
     ALCHEMY_ENABLE_CONNECTOR: zero_or_one
     ALCHEMY_EXPIRATION_TIME: PositiveInt
     ALCHEMY_VERIFICATION_TIME: PositiveInt
     ALCHEMY_HOST: str
@@ -426,36 +345,36 @@
     NEO4J_VERIFICATION_TIME: PositiveInt
     NEO4J_HOST: str
     NEO4J_BOLT_PORT: Port
     NEO4J_USER: str
     NEO4J_PASSWORD: str
     NEO4J_EXPOSED_WEB_INTERFACE_PORT: Port
     NEO4J_WEB_INTERFACE_PORT: Port
-    NEO4J_SSL_ENABLED: Neo4jFlag
+    NEO4J_SSL_ENABLED: bool
     NEO4J_BOLT_TLS_LEVEL: NEO4J_BOLT_TLS_LEVEL_VALUES
     # They are equal to placeholder in production mode when neo4j is not enabled
     NEO4J_HEAP_SIZE: Union[Neo4jMem, PLACEHOLDER_VALUE]
     NEO4J_PAGECACHE_SIZE: Union[Neo4jMem, PLACEHOLDER_VALUE]
-    NEO4J_ALLOW_UPGRADE: Neo4jFlag
-    NEO4J_RECOVERY_MODE: Neo4jFlag
+    NEO4J_ALLOW_UPGRADE: bool
+    NEO4J_RECOVERY_MODE: bool
     ELASTIC_HOST: str
     ELASTIC_PORT: Port
     RABBITMQ_ENABLE_CONNECTOR: zero_or_one
     RABBITMQ_EXPIRATION_TIME: PositiveInt
     RABBITMQ_VERIFICATION_TIME: PositiveInt
     RABBITMQ_HOST: str
     RABBITMQ_PORT: Port
     RABBITMQ_VHOST: str
     RABBITMQ_USER: str
     RABBITMQ_PASSWORD: str
     RABBITMQ_MANAGEMENT_PORT: Port
     RABBITMQ_ENABLE_SHOVEL_PLUGIN: zero_or_one
-    RABBITMQ_SSL_CERTFILE: Optional[Path]
-    RABBITMQ_SSL_KEYFILE: Optional[Path]
-    RABBITMQ_SSL_FAIL_IF_NO_PEER_CERT: Optional[true_or_false]
+    RABBITMQ_SSL_CERTFILE: Optional[Path] = None
+    RABBITMQ_SSL_KEYFILE: Optional[Path] = None
+    RABBITMQ_SSL_FAIL_IF_NO_PEER_CERT: Optional[true_or_false] = None
     RABBITMQ_SSL_ENABLED: zero_or_one
     REDIS_ENABLE_CONNECTOR: zero_or_one
     REDIS_EXPIRATION_TIME: PositiveInt
     REDIS_VERIFICATION_TIME: PositiveInt
     REDIS_HOST: str
     REDIS_PORT: Port
     REDIS_PASSWORD: str
@@ -463,15 +382,15 @@
     FTP_EXPIRATION_TIME: PositiveInt
     FTP_VERIFICATION_TIME: PositiveInt
     FTP_HOST: str
     FTP_PORT: Port
     FTP_USER: str
     FTP_PASSWORD: str
     FTP_SSL_ENABLED: zero_or_one
-    NFS_HOST: Optional[str]
+    NFS_HOST: Optional[str] = None
     NFS_EXPORTS_SECRETS: Path
     NFS_EXPORTS_RABBITDATA: Path
     NFS_EXPORTS_SQLDATA: Path
     NFS_EXPORTS_GRAPHDATA: Path
     NFS_EXPORTS_DATA_IMPORTS: Path
     NFS_EXPORTS_PUREFTPD: Path
     NFS_EXPORTS_SSL_CERTS: Path
@@ -483,15 +402,15 @@
     CELERY_BROKER: CELERY_BROKER_VALUES
     CELERY_BACKEND: CELERY_BACKEND_VALUES
     CELERY_POOL_MODE: CELERY_POOL_MODE_VALUES
     FLOWER_USER: str
     FLOWER_PASSWORD: str
     FLOWER_DBDIR: Path
     FLOWER_PORT: Port
-    FLOWER_SSL_OPTIONS: Optional[str]
+    FLOWER_SSL_OPTIONS: Optional[str] = None
     FLOWER_PROTOCOL: FLOWER_PROTOCOL_VALUES
     DEFAULT_SCALE_BACKEND: PositiveInt
     DEFAULT_SCALE_CELERY: PositiveInt
     DEFAULT_SCALE_CELERYBEAT: PositiveInt
     DEFAULT_SCALE_SWAGGERUI: PositiveInt
     ASSIGNED_CPU_BACKEND: AssignedCPU
     ASSIGNED_MEMORY_BACKEND: AssignedMemory
@@ -517,45 +436,46 @@
     ASSIGNED_MEMORY_ADMINER: AssignedMemory
     ASSIGNED_CPU_FTP: AssignedCPU
     ASSIGNED_MEMORY_FTP: AssignedMemory
     ASSIGNED_CPU_SMTP: AssignedCPU
     ASSIGNED_MEMORY_SMTP: AssignedMemory
     ASSIGNED_CPU_REGISTRY: AssignedCPU
     ASSIGNED_MEMORY_REGISTRY: AssignedMemory
-    REGISTRY_HOST: Optional[str]
+    REGISTRY_HOST: Optional[str] = None
     REGISTRY_PORT: Port
     REGISTRY_USERNAME: str
     REGISTRY_PASSWORD: str
-    REGISTRY_HTTP_SECRET: Optional[str]
+    REGISTRY_HTTP_SECRET: Optional[str] = None
     ACTIVATE_FAIL2BAN: zero_or_one
-    SWARM_MANAGER_ADDRESS: Optional[str]
+    SWARM_MANAGER_ADDRESS: Optional[str] = None
     # SYSLOG_ADDRESS: Optional[str]
     SMTP_ENABLE_CONNECTOR: zero_or_one
     SMTP_EXPIRATION_TIME: PositiveInt
     SMTP_VERIFICATION_TIME: PositiveInt
-    SMTP_ADMIN: Optional[str]
-    SMTP_NOREPLY: Optional[str]
-    SMTP_HOST: Optional[str]
+    SMTP_ADMIN: Optional[str] = None
+    SMTP_NOREPLY: Optional[str] = None
+    SMTP_REPLYTO: Optional[str] = None
+    SMTP_HOST: Optional[str] = None
     SMTP_PORT: NullablePort
-    SMTP_USERNAME: Optional[str]
-    SMTP_PASSWORD: Optional[str]
+    SMTP_USERNAME: Optional[str] = None
+    SMTP_PASSWORD: Optional[str] = None
     SMTP_SERVER_HOST: str
     SMTP_SERVER_PORT: Port
     FRONTEND_URL: str
     FRONTEND_PREFIX: str
     ALLOW_PASSWORD_RESET: zero_or_one
     ALLOW_REGISTRATION: zero_or_one
     ALLOW_TERMS_OF_USE: zero_or_one
     REGISTRATION_NOTIFICATIONS: zero_or_one
-    SENTRY_URL: Optional[str]
-    GA_TRACKING_CODE: Optional[str]
+    SENTRY_URL: Optional[str] = None
     SHOW_LOGIN: zero_or_one
     ENABLE_FOOTER: zero_or_one
     ENABLE_ANGULAR_SSR: zero_or_one
     ENABLE_YARN_PNP: zero_or_one
+    ENABLE_ANGULAR_MULTI_LANGUAGE: zero_or_one
     FORCE_SSR_SERVER_MODE: zero_or_one
     SPINNER_TYPE: SPINNER_TYPES
     ACTIVATE_AUTH: zero_or_one
     AUTH_SERVICE: AUTH_SERVICE_VALUES
     AUTH_DEFAULT_USERNAME: str
     AUTH_DEFAULT_PASSWORD: str
     AUTH_MIN_PASSWORD_LENGTH: NonNegativeInt
@@ -568,23 +488,24 @@
     AUTH_TOTP_VALIDITY_WINDOW: NonNegativeInt
     AUTH_JWT_TOKEN_TTL: PositiveInt
     AUTH_TOKEN_SAVE_FREQUENCY: NonNegativeInt
     AUTH_TOKEN_IP_GRACE_PERIOD: NonNegativeInt
     ALLOW_ACCESS_TOKEN_PARAMETER: zero_or_one
     DEFAULT_DHLEN: PositiveInt
 
+    PASSWORD_EXPIRATION_WARNING: NonNegativeInt
     FORCE_PRODUCTION_TESTS: zero_or_one
 
 
-class CoreEnvModel(BaseEnvModel, extra=Extra.forbid):
-    pass
+class CoreEnvModel(BaseEnvModel):
+    model_config = ConfigDict(extra="forbid")
 
 
-class CustomEnvModel(BaseEnvModel, extra=Extra.ignore):
-    pass
+class CustomEnvModel(BaseEnvModel):
+    model_config = ConfigDict(extra="ignore")
 
 
 class CoreVariablesModel(BaseModel):
     submodules: Dict[str, SubmoduleModel]
     roles: Dict[str, str]
     env: CoreEnvModel
 
@@ -630,15 +551,14 @@
         raise AttributeError("Missing project configuration")
 
     variables = ["title", "description", "version", "rapydo"]
 
     for key in variables:
         # Can't be tested because it is included in default configuration
         if project.get(key) is None:  # pragma: no cover
-
             print_and_exit(
                 "Project not configured, missing key '{}' in file {}/{}",
                 key,
                 base_project_path,
                 PROJECT_CONF_FILENAME,
             )
 
@@ -711,15 +631,14 @@
     if base is None:
         base = {}
 
     if custom is None:
         return base
 
     for key, elements in custom.items():
-
         if key not in base:
             # TypedDict key must be a string literal;
             base[key] = custom[key]  # type: ignore
             continue
 
         if elements is None:  # pragma: no cover
             # TypedDict key must be a string literal;
@@ -770,23 +689,20 @@
             # import codecs
             # error, _ = codecs.getdecoder("unicode_escape")(str(error))
 
             print_and_exit("Failed to read [{}]: {}", file, str(e))
 
 
 def read_composer_yamls(config_files: List[Path]) -> Tuple[List[Path], List[Path]]:
-
     base_files: List[Path] = []
     all_files: List[Path] = []
 
     # YAML CHECK UP
     for path in config_files:
-
         try:
-
             # This is to verify that mandatory files exist and yml syntax is valid
             conf = load_yaml_file(file=path, is_optional=False)
 
             if conf.get("version") != COMPOSE_FILE_VERSION:  # pragma: no cover
                 log.warning(
                     "Compose file version in {} is {}, expected {}",
                     path,
@@ -798,15 +714,14 @@
                 all_files.append(path)
 
                 # Base files are those loaded from CONFS_DIR
                 if CONFS_DIR in path.parents:
                     base_files.append(path)
 
         except KeyError as e:  # pragma: no cover
-
             print_and_exit("Error reading {}: {}", path, str(e))
 
     return all_files, base_files
 
 
 def validate_configuration(conf: Configuration, core: bool) -> None:
     if conf:
```

### Comparing `rapydo-2.4/controller/utilities/git.py` & `rapydo-3.0/controller/utilities/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,27 +37,25 @@
         url: str = gitobj.remotes.origin.url
         return url
     except AttributeError:  # pragma: no cover
         return None
 
 
 def get_active_branch(gitobj: Optional[Repo]) -> Optional[str]:
-
     if not gitobj:
         log.error("git object is None, cannot retrieve active branch")
         return None
     try:
         return gitobj.active_branch.name
     except AttributeError as e:  # pragma: no cover
         log.warning(e)
         return None
 
 
 def switch_branch(gitobj: Optional[Repo], branch_name: str) -> bool:
-
     if not gitobj:
         log.error("git object is None, cannot switch the active branch")
         return False
 
     current_branch = gitobj.active_branch.name
 
     path: str = "N/A"
@@ -89,15 +87,14 @@
     log.info("Switched {} branch from {} to {}", path, current_branch, branch_name)
     return True
 
 
 def clone(
     url: str, path: Path, branch: str, do: bool = False, check: bool = True
 ) -> Repo:
-
     local_path = SUBMODULES_DIR.joinpath(path)
 
     if local_path.exists():
         log.debug("Path {} already exists", local_path)
         gitobj = Repo(local_path)
     elif do:
         gitobj = Repo.clone_from(url=url, to_path=local_path)
@@ -117,21 +114,19 @@
     if check:
         compare_repository(gitobj, branch, online_url=url)
 
     return gitobj
 
 
 def compare_repository(gitobj: Repo, branch: str, online_url: str) -> bool:
-
     # origin = gitobj.remote()
     # url = list(origin.urls).pop(0)
     url = gitobj.remotes.origin.url
 
     if online_url != url:  # pragma: no cover
-
         local_url = urlparse(url)
         expected_url = urlparse(online_url)
 
         # Remove username in the URL, if any
         # i.e. youruser@github.com became github.com
         local_netloc = local_url.netloc.split("@").pop()
         expected_netloc = local_url.netloc.split("@").pop()
@@ -175,15 +170,14 @@
 
     return aware_utc_dt
 
 
 def check_file_younger_than(
     gitobj: Repo, filename: Path, timestamp: Union[str, float]
 ) -> Tuple[bool, float, datetime]:
-
     try:
         commits = gitobj.blame(rev="HEAD", file=str(filename))
     except GitCommandError:
         log.debug("Can't retrieve a commit history for {}", filename)
         return False, 0, datetime.fromtimestamp(0)
 
     # added a default date to prevent errors in case of new files with no blame commits
@@ -214,15 +208,14 @@
     return {
         "changed": [d.a_path for d in diff if d.a_path],
         "untracked": gitobj.untracked_files,
     }
 
 
 def print_diff(gitobj: Repo, unstaged: Dict[str, List[str]]) -> bool:
-
     changed = len(unstaged["changed"]) > 0
     untracked = len(unstaged["untracked"]) > 0
     if not changed and not untracked:
         return False
 
     if not gitobj.working_dir:  # pragma: no cover
         return False
@@ -255,15 +248,14 @@
         log.critical("Unable to update {} repo, you have unstaged files", path)
         print_diff(gitobj, unstaged)
 
     return updatable
 
 
 def update(path: str, gitobj: Repo) -> None:
-
     if not gitobj.active_branch:  # pragma: no cover
         log.error("Can't update {}, no active branch found", path)
         return None
 
     for remote in gitobj.remotes:
         if remote.name == "origin":
             try:
@@ -299,33 +291,30 @@
             except GitCommandError as e:  # pragma: no cover
                 log.error("Unable to update {} repo\n{}", path, e)
             except TypeError as e:  # pragma: no cover
                 print_and_exit("Unable to update {} repo, {}", path, str(e))
 
 
 def check_unstaged(path: str, gitobj: Repo) -> None:
-
     unstaged = get_unstaged_files(gitobj)
     if len(unstaged["changed"]) > 0 or len(unstaged["untracked"]) > 0:
         log.warning("You have unstaged files on {}", path)
     print_diff(gitobj, unstaged)
 
 
 def fetch(path: str, gitobj: Repo) -> None:
-
     for remote in gitobj.remotes:
         if remote.name == "origin":
             try:
                 remote.fetch()
             except GitCommandError as e:  # pragma: no cover
                 print_and_exit(str(e))
 
 
 def check_updates(path: str, gitobj: Repo) -> None:
-
     fetch(path, gitobj)
 
     branch = get_active_branch(gitobj)
     if branch is None:  # pragma: no cover
         log.warning("Is {} repo detached? Unable to verify updates", path)
         return None
 
@@ -339,15 +328,14 @@
     except GitCommandError:  # pragma: no cover
         log.info(
             "Remote branch {} not found for {} repo. Is it a local branch?",
             branch,
             path,
         )
     else:
-
         if not commits_behind_list:
             log.debug("{} repo is updated", path)
         else:  # pragma: no cover
             log.warning("{} repo should be updated!", path)
             for c in commits_behind_list:
                 message = str(c.message).strip().replace("\n", "")
 
@@ -365,15 +353,14 @@
     try:
         commits_ahead_list = list(commits_ahead)
     except GitCommandError:  # pragma: no cover
         log.info(
             "Remote branch {} not found for {}. Is it a local branch?", branch, path
         )
     else:
-
         if len(commits_ahead_list) > 0:
             log.warning("You have commits not pushed on {} repo", path)
         else:
             log.debug("You pushed all commits on {} repo", path)
         for c in commits_ahead_list:
             message = str(c.message).strip().replace("\n", "")
```

### Comparing `rapydo-2.4/controller/utilities/services.py` & `rapydo-3.0/controller/utilities/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,30 +5,28 @@
 from controller.project import ANGULAR
 
 
 def get_services(
     services: Optional[Union[str, Iterable[str]]],
     default: List[str],
 ) -> List[str]:
-
     return_list: List[str] = []
     if not services:
         return_list = sorted(default)
     elif isinstance(services, str):
         warnings.warn("Deprecated use of -s option")
         return_list = sorted(services.split(","))
     else:
         return_list = sorted(services)
 
     excluded_services_list: List[str] = [
         s[1:] for s in return_list if s.startswith("_")
     ]
 
     if excluded_services_list:
-
         # Filter out _ services from return_list
         return_list = [s for s in return_list if not s.startswith("_")]
 
         for service in excluded_services_list:
             if service not in return_list:
                 print_and_exit("No such service: {}", service)
 
@@ -36,15 +34,14 @@
 
     return return_list
 
 
 def walk_services(
     actives: List[str], dependecies: Dict[str, List[str]], index: int = 0
 ) -> List[str]:
-
     if index >= len(actives):
         return actives
 
     next_active = actives[index]
 
     for service in dependecies.get(next_active, []):
         # Not easy to test, since we have few services with dependencies
@@ -62,18 +59,24 @@
     which is equal to services 'activated' + 'depends_on'.
     """
 
     dependencies: Dict[str, List[str]] = {}
     base_actives: List[str] = []
 
     for name, service in services.items():
-
         dependencies[name] = list(service.depends_on.keys())
 
-        if service.environment and service.environment.get("ACTIVATE", "0") == "1":
+        if service.environment is None:  # pragma: no cover
+            continue
+
+        if isinstance(service.environment, list):  # pragma: no cover
+            log.error("Unsupported service environment format as list")
+            continue
+
+        if service.environment.get("ACTIVATE", "0") == "1":
             base_actives.append(name)
 
     log.debug("Base active services: {}", ", ".join(base_actives))
     # log.debug("Services dependencies: {}", ", ".join(dependencies))
     active_services = walk_services(base_actives, dependencies)
     return active_services
 
@@ -90,14 +93,15 @@
     "NEO4J_HEAP_SIZE": "neo4j",
     "NEO4J_PAGECACHE_SIZE": "neo4j",
     "AUTH_DEFAULT_PASSWORD": "backend",
     "AUTH_DEFAULT_USERNAME": "backend",
     "SMTP_PORT": "backend",
     "SMTP_ADMIN": "backend",
     "SMTP_NOREPLY": "backend",
+    "SMTP_REPLYTO": "backend",
     "SMTP_HOST": "backend",
     "SMTP_USERNAME": "backend",
     "SMTP_PASSWORD": "backend",
     "FTP_PASSWORD": "ftp",
     "FTP_USER": "ftp",
 }
 
@@ -129,15 +133,14 @@
     if key == "CYPRESS_AUTH_DEFAULT_PASSWORD":
         return "AUTH_DEFAULT_PASSWORD"
 
     return key
 
 
 def get_celerybeat_scheduler(env: Dict[str, EnvType]) -> str:
-
     if env.get("ACTIVATE_CELERYBEAT", "0") == "0":
         return "Unknown"
 
     celery_backend = env.get("CELERY_BACKEND")
 
     if celery_backend is None:
         return "Unknown"
@@ -169,15 +172,14 @@
                 "Some special characters, including {}, are not allowed "
                 "because make some clients to fail to connect",
                 " ".join(invalid_characters),
             )
 
 
 def get_default_user(service: str) -> Optional[str]:
-
     if service in ["backend", "celery", "flower", "celerybeat"]:
         return "developer"
 
     if service in ["frontend"]:
         from controller.app import Configuration
 
         if Configuration.frontend == ANGULAR:
@@ -195,15 +197,14 @@
     if service == "redis":
         return "redis"
 
     return None
 
 
 def get_default_command(service: str) -> str:
-
     if service == "backend":
         return "restapi launch"
 
     if service == "bot":
         return "restapi bot"
 
     if service == "neo4j":
```

### Comparing `rapydo-2.4/controller/utilities/system.py` & `rapydo-3.0/controller/utilities/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     # Can fail on Windows
     except AttributeError as e:  # pragma: no cover
         log.debug(e)
         return 0
 
 
 def bytes_to_str(value: float) -> str:
-
     if value >= GB:
         value /= GB
         unit = "GB"
     elif value >= MB:
         value /= MB
         unit = "MB"
     elif value >= KB:
@@ -53,15 +52,14 @@
         unit = ""
 
     return f"{int(round(value, 0))}{unit}"
 
 
 # This is no longer needed
 def str_to_bytes(text: str) -> float:
-
     text = text.upper()
 
     value: str = text
     unit: int = 1
 
     if text.endswith("G"):
         value = text[:-1]
```

### Comparing `rapydo-2.4/docs/conf.py` & `rapydo-3.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
 sys.path.insert(0, os.path.abspath(".."))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "RAPyDo Controller"
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

### Comparing `rapydo-2.4/pyproject.toml` & `rapydo-3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rapydo"
-version = "2.4"
+version = "3.0"
 description = "Manage and deploy projects based on RAPyDo framework"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 dynamic = ["dependencies", "optional-dependencies"]
 readme = "README.rst"
 keywords = ["http", "api", "rest", "docker", "docker-compose", "docker-swarm", "rapydo"]
 classifiers=[
@@ -12,14 +12,15 @@
     "Intended Audience :: Developers",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = {dev = {file = ["requirements.dev.txt"]}, types = {file = ["requirements.types.txt"]}}
 
 [project.urls]
```

### Comparing `rapydo-2.4/rapydo.egg-info/SOURCES.txt` & `rapydo-3.0/rapydo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
 README.rst
 pyproject.toml
+requirements.dev.txt
+requirements.txt
+requirements.types.txt
 controller/__init__.py
 controller/__main__.py
 controller/app.py
 controller/packages.py
 controller/project.py
 controller/py.typed
 controller/templating.py
+controller/builds/backend/gunicorn_conf.py
+controller/builds/backend-legacy310/gunicorn_conf.py
+controller/builds/backend-legacy39/gunicorn_conf.py
 controller/commands/__init__.py
 controller/commands/add.py
 controller/commands/backup.py
 controller/commands/build.py
 controller/commands/check.py
 controller/commands/create.py
 controller/commands/dump.py
@@ -27,15 +33,14 @@
 controller/commands/restart.py
 controller/commands/restore.py
 controller/commands/run.py
 controller/commands/shell.py
 controller/commands/ssl.py
 controller/commands/start.py
 controller/commands/status.py
-controller/commands/test.py
 controller/commands/tuning.py
 controller/commands/update.py
 controller/commands/upgrade.py
 controller/commands/version.py
 controller/commands/volatile.py
 controller/commands/backup_modules/__init__.py
 controller/commands/backup_modules/neo4j.py
@@ -100,14 +105,15 @@
 controller/templates/component_template.html.j2
 controller/templates/component_template.ts.j2
 controller/templates/component_test_template.spec.ts.j2
 controller/templates/custom.footer.html.j2
 controller/templates/custom.footer.ts.j2
 controller/templates/custom.module.ts.j2
 controller/templates/custom.navbar.brand.html.j2
+controller/templates/custom.navbar.controls.html.j2
 controller/templates/custom.navbar.links.html.j2
 controller/templates/custom.navbar.ts.j2
 controller/templates/custom.profile.html.j2
 controller/templates/custom.profile.ts.j2
 controller/templates/customization.py.j2
 controller/templates/customization.ts.j2
 controller/templates/cypress_template.spec.ts.j2
@@ -156,8 +162,9 @@
 controller/utilities/tables.py
 docs/conf.py
 rapydo.egg-info/PKG-INFO
 rapydo.egg-info/SOURCES.txt
 rapydo.egg-info/dependency_links.txt
 rapydo.egg-info/entry_points.txt
 rapydo.egg-info/requires.txt
-rapydo.egg-info/top_level.txt
+rapydo.egg-info/top_level.txt
+stubs/glom/__init__.pyi
```

### Comparing `rapydo-2.4/rapydo.egg-info/requires.txt` & `rapydo-3.0/rapydo.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-python-on-whales==0.54.0
+python-on-whales==0.70.1
 python-dateutil
 pytz
 loguru
 jinja2
 sultan==0.9.1
 plumbum
 glom
-GitPython==3.1.29
-PyYAML==6.0
-pip==22.3.1
-setuptools==65.6.3
-wheel==0.38.4
-requests==2.28.1
-typer[all]==0.7.0
-click==8.1.3
+GitPython==3.1.43
+PyYAML==6.0.1
+pydantic==2.7.0
+pip==24.0
+setuptools==69.2.0
+wheel==0.43.0
+requests==2.31.0
+typer[all]==0.9.0
+click==8.1.7
 zxcvbn
 packaging
 
 [dev]
-pytest==7.2.0
-pytest-cov==4.0.0
-pytest-timeout==2.1.0
-pytest-sugar==0.9.6
-freezegun==1.2.2
+pytest==8.1.1
+pytest-cov==5.0.0
+pytest-sugar==1.0.0
+pytest-timeout==2.3.1
+freezegun==1.4.0
 Faker
 
 [types]
 rapydo[dev]
-mypy==0.991
-lxml==4.9.1
+mypy==1.9.0
+lxml==5.2.1
 html5lib==1.1
-types-PyYAML==6.0.12.2
-types-python-dateutil==2.8.19.4
-types-pytz==2022.6.0.1
-types-requests==2.28.11.5
+types-PyYAML==6.0.12.20240311
+types-python-dateutil==2.9.0.20240316
+types-pytz==2024.1.0.20240203
+types-requests==2.31.0.20240406
 types-freezegun==1.1.10
```

