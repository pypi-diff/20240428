# Comparing `tmp/libretranslate-1.5.6.tar.gz` & `tmp/libretranslate-1.5.7.tar.gz`

## Comparing `libretranslate-1.5.6.tar` & `libretranslate-1.5.7.tar`

### file list

```diff
@@ -1,158 +1,211 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 libretranslate-1.5.6/.dockerignore
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 libretranslate-1.5.6/.editorconfig
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 libretranslate-1.5.6/.gitattributes
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 libretranslate-1.5.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 libretranslate-1.5.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 libretranslate-1.5.6/TRADEMARK.md
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 libretranslate-1.5.6/VERSION
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 libretranslate-1.5.6/babel.cfg
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 libretranslate-1.5.6/docker-compose.cuda.yml
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 libretranslate-1.5.6/docker-compose.yml
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 libretranslate-1.5.6/k8s.yaml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 libretranslate-1.5.6/main.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 libretranslate-1.5.6/manage.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 libretranslate-1.5.6/run.bat
--rwxr-xr-x   0        0        0     2191 2020-02-02 00:00:00.000000 libretranslate-1.5.6/run.sh
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 libretranslate-1.5.6/wsgi.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 libretranslate-1.5.6/.github/FUNDING.yml
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 libretranslate-1.5.6/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 libretranslate-1.5.6/.github/dependabot.yaml
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 libretranslate-1.5.6/.github/workflows/issue-triage.yml
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 libretranslate-1.5.6/.github/workflows/publish-docker.yml
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 libretranslate-1.5.6/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 libretranslate-1.5.6/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 libretranslate-1.5.6/docker/Dockerfile
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 libretranslate-1.5.6/docker/arm.Dockerfile
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 libretranslate-1.5.6/docker/cuda.Dockerfile
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/__init__.py
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/api_keys.py
--rw-r--r--   0        0        0    38856 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/app.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/default_values.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/detect.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/flood.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/init.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/language.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales.py
--rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/main.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/manage.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/no_limiter.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/remove_translated_files.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/scheduler.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/secret.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/security.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/storage.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/suggestions.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/.gitignore
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ar/meta.json
--rw-r--r--   0        0        0    19137 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ar/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/az/meta.json
--rw-r--r--   0        0        0    17098 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/az/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/bg/meta.json
--rw-r--r--   0        0        0    20573 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/bg/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    15380 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ca/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/cs/meta.json
--rw-r--r--   0        0        0    17894 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/cs/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/da/meta.json
--rw-r--r--   0        0        0    17615 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/da/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/de/meta.json
--rw-r--r--   0        0        0    18080 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/el/meta.json
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/el/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/eo/meta.json
--rw-r--r--   0        0        0    17483 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/eo/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/es/meta.json
--rw-r--r--   0        0        0    17970 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/et/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/eu/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    13827 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ext/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/fa/meta.json
--rw-r--r--   0        0        0    19492 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/fa/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/fi/meta.json
--rw-r--r--   0        0        0    17560 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/fi/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/fr/meta.json
--rw-r--r--   0        0        0    18111 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ga/meta.json
--rw-r--r--   0        0        0    18547 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ga/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    17678 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/gl/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/he/meta.json
--rw-r--r--   0        0        0    18218 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/he/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/hi/meta.json
--rw-r--r--   0        0        0    22067 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/hi/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/hu/meta.json
--rw-r--r--   0        0        0    17905 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/hu/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/id/meta.json
--rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/id/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/it/meta.json
--rw-r--r--   0        0        0    17736 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/it/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ja/meta.json
--rw-r--r--   0        0        0    19021 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/kab/meta.json
--rw-r--r--   0        0        0    17588 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/kab/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ko/meta.json
--rw-r--r--   0        0        0    17946 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ko/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    17485 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/nb_NO/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/nl/meta.json
--rw-r--r--   0        0        0    17553 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/nl/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    17799 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/oc/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    13957 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/pa/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/pl/meta.json
--rw-r--r--   0        0        0    17749 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/pl/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/pt/meta.json
--rw-r--r--   0        0        0    17852 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/pt/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    17868 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    17809 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ro/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ru/meta.json
--rw-r--r--   0        0        0    21031 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ru/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    14423 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/si/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/sk/meta.json
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/sk/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    13826 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/sq/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    17521 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/sr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/sv/meta.json
--rw-r--r--   0        0        0    17670 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/sv/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/tr/meta.json
--rw-r--r--   0        0        0    17785 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/tr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/ug/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/uk/meta.json
--rw-r--r--   0        0        0    24485 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/uk/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/vi/meta.json
--rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/vi/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    14158 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/zgh/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/zh/meta.json
--rw-r--r--   0        0        0    17207 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/zh/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    17053 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/locales/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0   268350 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/favicon.ico
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/icon.svg
--rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/css/main.css
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/css/material-icons.css
--rw-r--r--   0        0        0   141841 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/css/materialize.min.css
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/css/prism.min.css
--rw-r--r--   0        0        0   143258 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/fonts/MaterialIcons-Regular.eot
--rw-r--r--   0        0        0   128180 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/fonts/MaterialIcons-Regular.ttf
--rw-r--r--   0        0        0    57620 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/fonts/MaterialIcons-Regular.woff
--rw-r--r--   0        0        0    44300 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/fonts/MaterialIcons-Regular.woff2
--rw-r--r--   0        0        0   181109 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/js/materialize.min.js
--rw-r--r--   0        0        0    16284 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/js/prism.min.js
--rw-r--r--   0        0        0    94151 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/static/js/vue@2.js
--rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/templates/app.js.template
--rw-r--r--   0        0        0    16194 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/templates/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/tests/__init__.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/tests/test_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/tests/test_api/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/tests/test_api/conftest.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/tests/test_api/test_api_detect_language.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/tests/test_api/test_api_frontend_settings.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/tests/test_api/test_api_get_languages.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/tests/test_api/test_api_spec.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 libretranslate-1.5.6/libretranslate/tests/test_api/test_api_translate.py
--rwxr-xr-x   0        0        0     1135 2020-02-02 00:00:00.000000 libretranslate-1.5.6/scripts/compile_locales.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 libretranslate-1.5.6/scripts/gunicorn_conf.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 libretranslate-1.5.6/scripts/healthcheck.py
--rwxr-xr-x   0        0        0      744 2020-02-02 00:00:00.000000 libretranslate-1.5.6/scripts/install_models.py
--rwxr-xr-x   0        0        0     1312 2020-02-02 00:00:00.000000 libretranslate-1.5.6/scripts/suggestions-to-jsonl.py
--rwxr-xr-x   0        0        0     4715 2020-02-02 00:00:00.000000 libretranslate-1.5.6/scripts/update_locales.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 libretranslate-1.5.6/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 libretranslate-1.5.6/LICENSE
--rw-r--r--   0        0        0    34254 2020-02-02 00:00:00.000000 libretranslate-1.5.6/README.md
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 libretranslate-1.5.6/pyproject.toml
--rw-r--r--   0        0        0    76261 2020-02-02 00:00:00.000000 libretranslate-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 libretranslate-1.5.7/.dockerignore
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 libretranslate-1.5.7/.editorconfig
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 libretranslate-1.5.7/.gitattributes
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 libretranslate-1.5.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 libretranslate-1.5.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 libretranslate-1.5.7/TRADEMARK.md
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 libretranslate-1.5.7/VERSION
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 libretranslate-1.5.7/babel.cfg
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 libretranslate-1.5.7/docker-compose.cuda.yml
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 libretranslate-1.5.7/docker-compose.yml
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 libretranslate-1.5.7/k8s.yaml
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 libretranslate-1.5.7/main.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 libretranslate-1.5.7/manage.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 libretranslate-1.5.7/run.bat
+-rwxr-xr-x   0        0        0     2191 2020-02-02 00:00:00.000000 libretranslate-1.5.7/run.sh
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 libretranslate-1.5.7/wsgi.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 libretranslate-1.5.7/.github/FUNDING.yml
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 libretranslate-1.5.7/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 libretranslate-1.5.7/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 libretranslate-1.5.7/.github/workflows/issue-triage.yml
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 libretranslate-1.5.7/.github/workflows/publish-docker.yml
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 libretranslate-1.5.7/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 libretranslate-1.5.7/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 libretranslate-1.5.7/docker/Dockerfile
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 libretranslate-1.5.7/docker/arm.Dockerfile
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 libretranslate-1.5.7/docker/cuda.Dockerfile
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/__init__.py
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/api_keys.py
+-rw-r--r--   0        0        0    38870 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/app.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/default_values.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/detect.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/flood.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/init.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/language.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales.py
+-rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/main.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/manage.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/no_limiter.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/remove_translated_files.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/scheduler.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/secret.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/security.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/storage.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/suggestions.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/.gitignore
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ar/meta.json
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    19137 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ar/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/az/meta.json
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/az/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17098 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/az/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/be/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    18948 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/be/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/bg/meta.json
+-rw-r--r--   0        0        0    12805 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    20573 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/bg/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    15461 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ca/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/cs/meta.json
+-rw-r--r--   0        0        0    10073 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17894 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/cs/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/da/meta.json
+-rw-r--r--   0        0        0     9736 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17569 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/da/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/de/meta.json
+-rw-r--r--   0        0        0    10275 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    18080 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/el/meta.json
+-rw-r--r--   0        0        0    12861 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/el/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/eo/meta.json
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/eo/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17483 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/eo/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/es/meta.json
+-rw-r--r--   0        0        0    10162 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17970 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/et/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/eu/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/eu/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ext/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    13827 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ext/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/fa/meta.json
+-rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    19470 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/fa/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/fi/meta.json
+-rw-r--r--   0        0        0     9764 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/fi/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17560 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/fi/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/fil/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    15079 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/fil/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/fr/meta.json
+-rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    18111 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ga/meta.json
+-rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ga/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    18547 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ga/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17678 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/gl/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/he/meta.json
+-rw-r--r--   0        0        0    10434 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/he/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    18218 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/he/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/hi/meta.json
+-rw-r--r--   0        0        0    14238 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/hi/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    22067 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/hi/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/hu/meta.json
+-rw-r--r--   0        0        0    10151 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    18002 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/hu/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/id/meta.json
+-rw-r--r--   0        0        0     9841 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/id/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/id/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/it/meta.json
+-rw-r--r--   0        0        0     9929 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17736 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/it/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ja/meta.json
+-rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    19021 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/kab/meta.json
+-rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/kab/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17588 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/kab/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ko/meta.json
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ko/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17946 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ko/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     9632 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/nb_NO/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17491 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/nb_NO/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/nl/meta.json
+-rw-r--r--   0        0        0     9721 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17553 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/nl/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/nn/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    14721 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/nn/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/oc/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17799 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/oc/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/pa/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    13957 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/pa/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/pl/meta.json
+-rw-r--r--   0        0        0     9911 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17749 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/pl/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/pt/meta.json
+-rw-r--r--   0        0        0    10045 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17852 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    10135 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17868 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    10077 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17809 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ro/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ru/meta.json
+-rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    21031 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ru/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/si/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    14423 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/si/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/sk/meta.json
+-rw-r--r--   0        0        0    10001 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/sk/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/sq/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    13826 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/sq/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     9805 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/sr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17521 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/sr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/sv/meta.json
+-rw-r--r--   0        0        0     9871 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17670 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/sv/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/tr/meta.json
+-rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17785 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/tr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ug/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/ug/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/uk/meta.json
+-rw-r--r--   0        0        0    13017 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    24485 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/uk/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/vi/meta.json
+-rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/vi/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/vi/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/zgh/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    14158 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/zgh/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/zh/meta.json
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/zh/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17207 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/zh/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    17052 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/locales/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0   268350 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/favicon.ico
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/icon.svg
+-rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/css/main.css
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/css/material-icons.css
+-rw-r--r--   0        0        0   141841 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/css/materialize.min.css
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/css/prism.min.css
+-rw-r--r--   0        0        0   143258 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/fonts/MaterialIcons-Regular.eot
+-rw-r--r--   0        0        0   128180 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/fonts/MaterialIcons-Regular.ttf
+-rw-r--r--   0        0        0    57620 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/fonts/MaterialIcons-Regular.woff
+-rw-r--r--   0        0        0    44300 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/fonts/MaterialIcons-Regular.woff2
+-rw-r--r--   0        0        0   181109 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/js/materialize.min.js
+-rw-r--r--   0        0        0    16284 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/js/prism.min.js
+-rw-r--r--   0        0        0    94151 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/static/js/vue@2.js
+-rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/templates/app.js.template
+-rw-r--r--   0        0        0    16194 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/templates/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/tests/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/tests/test_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/tests/test_api/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/tests/test_api/conftest.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/tests/test_api/test_api_detect_language.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/tests/test_api/test_api_frontend_settings.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/tests/test_api/test_api_get_languages.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/tests/test_api/test_api_spec.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 libretranslate-1.5.7/libretranslate/tests/test_api/test_api_translate.py
+-rwxr-xr-x   0        0        0     1135 2020-02-02 00:00:00.000000 libretranslate-1.5.7/scripts/compile_locales.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 libretranslate-1.5.7/scripts/gunicorn_conf.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 libretranslate-1.5.7/scripts/healthcheck.py
+-rwxr-xr-x   0        0        0      744 2020-02-02 00:00:00.000000 libretranslate-1.5.7/scripts/install_models.py
+-rwxr-xr-x   0        0        0     1312 2020-02-02 00:00:00.000000 libretranslate-1.5.7/scripts/suggestions-to-jsonl.py
+-rwxr-xr-x   0        0        0     4715 2020-02-02 00:00:00.000000 libretranslate-1.5.7/scripts/update_locales.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 libretranslate-1.5.7/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 libretranslate-1.5.7/LICENSE
+-rw-r--r--   0        0        0    34316 2020-02-02 00:00:00.000000 libretranslate-1.5.7/README.md
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 libretranslate-1.5.7/pyproject.toml
+-rw-r--r--   0        0        0    76323 2020-02-02 00:00:00.000000 libretranslate-1.5.7/PKG-INFO
```

### Comparing `libretranslate-1.5.6/.pre-commit-config.yaml` & `libretranslate-1.5.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/CONTRIBUTING.md` & `libretranslate-1.5.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/TRADEMARK.md` & `libretranslate-1.5.7/TRADEMARK.md`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/docker-compose.yml` & `libretranslate-1.5.7/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/k8s.yaml` & `libretranslate-1.5.7/k8s.yaml`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/run.bat` & `libretranslate-1.5.7/run.bat`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/run.sh` & `libretranslate-1.5.7/run.sh`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/.github/ISSUE_TEMPLATE.md` & `libretranslate-1.5.7/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/.github/workflows/issue-triage.yml` & `libretranslate-1.5.7/.github/workflows/issue-triage.yml`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/.github/workflows/publish-docker.yml` & `libretranslate-1.5.7/.github/workflows/publish-docker.yml`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/.github/workflows/publish-package.yml` & `libretranslate-1.5.7/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/.github/workflows/run-tests.yml` & `libretranslate-1.5.7/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/docker/Dockerfile` & `libretranslate-1.5.7/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/docker/arm.Dockerfile` & `libretranslate-1.5.7/docker/arm.Dockerfile`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/docker/cuda.Dockerfile` & `libretranslate-1.5.7/docker/cuda.Dockerfile`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/api_keys.py` & `libretranslate-1.5.7/libretranslate/api_keys.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/app.py` & `libretranslate-1.5.7/libretranslate/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -854,15 +854,15 @@
         tags:
           - translate
         parameters:
           - in: formData
             name: q
             schema:
               type: string
-              example: Hello world!
+              example: What language is this?
             required: true
             description: Text to detect
           - in: formData
             name: api_key
             schema:
               type: string
               example: xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
@@ -875,19 +875,19 @@
               id: detections
               type: array
               items:
                 type: object
                 properties:
                   confidence:
                     type: number
-                    format: float
+                    format: integer
                     minimum: 0
-                    maximum: 1
+                    maximum: 100
                     description: Confidence value
-                    example: 0.6
+                    example: 100
                   language:
                     type: string
                     description: Language code
                     example: en
           400:
             description: Invalid request
             schema:
```

### Comparing `libretranslate-1.5.6/libretranslate/default_values.py` & `libretranslate-1.5.7/libretranslate/default_values.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/detect.py` & `libretranslate-1.5.7/libretranslate/detect.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/flood.py` & `libretranslate-1.5.7/libretranslate/flood.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/init.py` & `libretranslate-1.5.7/libretranslate/init.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/language.py` & `libretranslate-1.5.7/libretranslate/language.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales.py` & `libretranslate-1.5.7/libretranslate/locales.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/main.py` & `libretranslate-1.5.7/libretranslate/main.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/manage.py` & `libretranslate-1.5.7/libretranslate/manage.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/remove_translated_files.py` & `libretranslate-1.5.7/libretranslate/remove_translated_files.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/scheduler.py` & `libretranslate-1.5.7/libretranslate/scheduler.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/secret.py` & `libretranslate-1.5.7/libretranslate/secret.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/storage.py` & `libretranslate-1.5.7/libretranslate/storage.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/suggestions.py` & `libretranslate-1.5.7/libretranslate/suggestions.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/ar/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/az/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/az/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/bg/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/ca/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/ca/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: LibreTranslate 1.3.12\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2023-10-09 15:17-0400\n"
-"PO-Revision-Date: 2024-01-27 09:01+0000\n"
-"Last-Translator: victor dargallo <victordargallo@disroot.org>\n"
+"PO-Revision-Date: 2024-03-07 08:01+0000\n"
+"Last-Translator: d <dmanye@gmail.com>\n"
 "Language-Team: Catalan <https://hosted.weblate.org/projects/libretranslate/"
 "app/ca/>\n"
 "Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: libretranslate/app.py:79
 msgid "Invalid JSON format"
 msgstr "Format JSON invàlid"
 
 #: libretranslate/app.py:149 libretranslate/templates/app.js.template:459
@@ -347,35 +347,35 @@
 
 #: libretranslate/locales/.swag.py:27
 msgid "frontend"
 msgstr ""
 
 #: libretranslate/locales/.swag.py:28
 msgid "Submit a suggestion to improve a translation"
-msgstr ""
+msgstr "Envia un suggeriment per millorar una traducció"
 
 #: libretranslate/locales/.swag.py:29
 msgid "Success"
 msgstr ""
 
 #: libretranslate/locales/.swag.py:30
 msgid "Not authorized"
 msgstr ""
 
 #: libretranslate/locales/.swag.py:31
 msgid "Original text"
-msgstr ""
+msgstr "Text original"
 
 #: libretranslate/locales/.swag.py:32
 msgid "Suggested translation"
-msgstr ""
+msgstr "Traducció suggerida"
 
 #: libretranslate/locales/.swag.py:33
 msgid "Language of original text"
-msgstr ""
+msgstr "Idioma del text original"
 
 #: libretranslate/locales/.swag.py:34
 msgid "Language of suggested translation"
 msgstr ""
 
 #: libretranslate/locales/.swag.py:35
 msgid "feedback"
```

### Comparing `libretranslate-1.5.6/libretranslate/locales/cs/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/da/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/da/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,59 +5,58 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: LibreTranslate 1.3.9\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2023-10-09 15:17-0400\n"
-"PO-Revision-Date: 2024-01-15 00:06+0000\n"
-"Last-Translator: symegac <97731141+symegac@users.noreply.github.com>\n"
+"PO-Revision-Date: 2024-03-25 12:01+0000\n"
+"Last-Translator: cat <158170307+cultcats@users.noreply.github.com>\n"
 "Language-Team: Danish <https://hosted.weblate.org/projects/libretranslate/"
 "app/da/>\n"
 "Language: da\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: libretranslate/app.py:79
 msgid "Invalid JSON format"
 msgstr "Ugyldig JSON format"
 
 #: libretranslate/app.py:149 libretranslate/templates/app.js.template:459
 msgid "Auto Detect"
-msgstr "Autodetektor"
+msgstr "Auto detektor"
 
 #: libretranslate/app.py:232
 msgid "Unauthorized"
 msgstr "Uautoriseret"
 
 #: libretranslate/app.py:250
-#, fuzzy
 msgid "Too many request limits violations"
-msgstr "For mange anmodninger begrænser overtrædelser"
+msgstr "For mange overtrædelser af anmodningsbegrænsninger"
 
 #: libretranslate/app.py:257
 msgid "Invalid API key"
 msgstr "Ugyldig API-nøgle"
 
 #: libretranslate/app.py:276
 msgid "Please contact the server operator to get an API key"
-msgstr "Kontakt serveroperatøren for at få en API-nøgle"
+msgstr "Kontakt venligst serveroperatøren for at få en API-nøgle"
 
 #: libretranslate/app.py:278
 #, python-format
 msgid "Visit %(url)s to get an API key"
-msgstr "Besøg %(url)s at få en API-nøgle"
+msgstr "Besøg %(url)s for at få en API-nøgle"
 
 #: libretranslate/app.py:318
 msgid "Slowdown:"
-msgstr "Langlægning:"
+msgstr "Nedbremsning:"
 
 #: libretranslate/app.py:525 libretranslate/app.py:527
 #: libretranslate/app.py:529 libretranslate/app.py:741
 #: libretranslate/app.py:743 libretranslate/app.py:745
 #: libretranslate/app.py:896 libretranslate/app.py:1053
 #: libretranslate/app.py:1055 libretranslate/app.py:1057
 #: libretranslate/app.py:1059
@@ -95,27 +94,27 @@
 #: libretranslate/app.py:647
 #, python-format
 msgid "Cannot translate text: %(text)s"
 msgstr "Kan ikke oversætte tekst: %(text)s"
 
 #: libretranslate/app.py:734 libretranslate/app.py:788
 msgid "Files translation are disabled on this server."
-msgstr "Filer oversættelse er deaktiveret på denne server."
+msgstr "File oversættelse er deaktiveret på denne server."
 
 #: libretranslate/app.py:748
 msgid "Invalid request: empty file"
-msgstr "Ugyldig anmodning: tomt fil"
+msgstr "Ugyldig anmodning: tom fil"
 
 #: libretranslate/app.py:751
 msgid "Invalid request: file format not supported"
-msgstr "Ugyldig anmodning: filformat ikke understøttet"
+msgstr "Ugyldig anmodning: filformat understøttes ikke"
 
 #: libretranslate/app.py:796
 msgid "Invalid filename"
-msgstr "Ugyldig filnavn"
+msgstr "Ugyldigt filnavn"
 
 #: libretranslate/app.py:1038
 msgid "Suggestions are disabled on this server."
 msgstr "Forslag er deaktiveret på denne server."
 
 #: libretranslate/locales/.langs.py:1
 msgid "English"
@@ -139,15 +138,15 @@
 
 #: libretranslate/locales/.langs.py:6
 msgid "Danish"
 msgstr "Dansk"
 
 #: libretranslate/locales/.langs.py:7
 msgid "Dutch"
-msgstr "Hollandske"
+msgstr "Hollandsk"
 
 #: libretranslate/locales/.langs.py:8
 msgid "Esperanto"
 msgstr "Esperanto"
 
 #: libretranslate/locales/.langs.py:9
 msgid "Finnish"
@@ -243,15 +242,15 @@
 
 #: libretranslate/locales/.swag.py:2
 msgid "List of languages"
 msgstr "Liste over sprog"
 
 #: libretranslate/locales/.swag.py:3
 msgid "translate"
-msgstr "oversætter"
+msgstr "oversæt"
 
 #: libretranslate/locales/.swag.py:4
 msgid "Translate text from a language to another"
 msgstr "Oversæt tekst fra et sprog til et andet"
 
 #: libretranslate/locales/.swag.py:5 libretranslate/templates/index.html:222
 msgid "Translated text"
@@ -275,23 +274,23 @@
 
 #: libretranslate/locales/.swag.py:10
 msgid "Hello world!"
 msgstr "Hej verden!"
 
 #: libretranslate/locales/.swag.py:11
 msgid "Text(s) to translate"
-msgstr "Tekst(er) at oversætte"
+msgstr "Tekst(er) til oversættelse"
 
 #: libretranslate/locales/.swag.py:12
 msgid "Source language code"
 msgstr "Kildesprogkode"
 
 #: libretranslate/locales/.swag.py:13
 msgid "Target language code"
-msgstr "Målsprogkoder"
+msgstr "Målsprogkode"
 
 #: libretranslate/locales/.swag.py:14
 msgid "text"
 msgstr "tekst"
 
 #: libretranslate/locales/.swag.py:15
 msgid "html"
@@ -300,15 +299,15 @@
 #: libretranslate/locales/.swag.py:16
 msgid ""
 "Format of source text:\n"
 " * `text` - Plain text\n"
 " * `html` - HTML markup\n"
 msgstr ""
 "Format af kildetekst:\n"
-"* 'tekst' - almindeligt tekst\n"
+"* 'tekst' - almindelig tekst\n"
 "* `html' - HTML-markup\n"
 
 #: libretranslate/locales/.swag.py:17
 msgid "API key"
 msgstr "API-nøgle"
 
 #: libretranslate/locales/.swag.py:18
@@ -321,51 +320,51 @@
 
 #: libretranslate/locales/.swag.py:20
 msgid "File to translate"
 msgstr "Fil at oversætte"
 
 #: libretranslate/locales/.swag.py:21
 msgid "Detect the language of a single text"
-msgstr "Angiv sproget for en enkelt tekst"
+msgstr "Registrer sproget i en enkelt tekst"
 
 #: libretranslate/locales/.swag.py:22
 msgid "Detections"
 msgstr "Registreringer"
 
 #: libretranslate/locales/.swag.py:23
 msgid "Detection error"
 msgstr "Registreringsfejl"
 
 #: libretranslate/locales/.swag.py:24
 msgid "Text to detect"
-msgstr "Tekst at opdage"
+msgstr "Tekst at finde"
 
 #: libretranslate/locales/.swag.py:25
 msgid "Retrieve frontend specific settings"
-msgstr "Hent frontend specifikke indstillinger"
+msgstr "Hent frontend-specifikke indstillinger"
 
 #: libretranslate/locales/.swag.py:26
 msgid "frontend settings"
 msgstr "frontend indstillinger"
 
 #: libretranslate/locales/.swag.py:27
 msgid "frontend"
-msgstr "frontend"
+msgstr "grænseflade"
 
 #: libretranslate/locales/.swag.py:28
 msgid "Submit a suggestion to improve a translation"
-msgstr "Indsend et forslag til at forbedre en oversættelse"
+msgstr "Indsend et forslag til forbedring af en oversættelse"
 
 #: libretranslate/locales/.swag.py:29
 msgid "Success"
 msgstr "Succes"
 
 #: libretranslate/locales/.swag.py:30
 msgid "Not authorized"
-msgstr "Ikke godkendt"
+msgstr "Ikke autoriseret"
 
 #: libretranslate/locales/.swag.py:31
 msgid "Original text"
 msgstr "Original tekst"
 
 #: libretranslate/locales/.swag.py:32
 msgid "Suggested translation"
@@ -373,75 +372,75 @@
 
 #: libretranslate/locales/.swag.py:33
 msgid "Language of original text"
 msgstr "Originaltekstens sprog"
 
 #: libretranslate/locales/.swag.py:34
 msgid "Language of suggested translation"
-msgstr "Foreslået oversættelses sprog"
+msgstr "Sprog i foreslået oversættelse"
 
 #: libretranslate/locales/.swag.py:35
 msgid "feedback"
-msgstr "tilbagemelding"
+msgstr "feedback"
 
 #: libretranslate/locales/.swag.py:36
 msgid "Language code"
 msgstr "Sprogkode"
 
 #: libretranslate/locales/.swag.py:37
 msgid "Human-readable language name (in English)"
 msgstr "Menneskeligt læseligt sprognavn (på engelsk)"
 
 #: libretranslate/locales/.swag.py:38
 msgid "Supported target language codes"
-msgstr "Understøttede sprogkoder"
+msgstr "Understøttede målsprogkoder"
 
 #: libretranslate/locales/.swag.py:39
 msgid "Translated text(s)"
-msgstr "Oversat tekst(r)"
+msgstr "Oversat tekst(er)"
 
 #: libretranslate/locales/.swag.py:40
 msgid "Error message"
 msgstr "Fejlmeddelelse"
 
 #: libretranslate/locales/.swag.py:41
 msgid "Reason for slow down"
-msgstr "Reason for langsom ned"
+msgstr "Årsag til nedbremsning"
 
 #: libretranslate/locales/.swag.py:42
 msgid "Translated file url"
-msgstr "Oversætt fil url"
+msgstr "Oversat fil-url"
 
 #: libretranslate/locales/.swag.py:43
 msgid "Confidence value"
-msgstr "Konsekvensværdi"
+msgstr "Konfidensværdi"
 
 #: libretranslate/locales/.swag.py:44
 msgid "Character input limit for this language (-1 indicates no limit)"
-msgstr "Karakterindgangsgrænse for dette sprog (-1 angiver ingen grænse)"
+msgstr "Grænse for tegninput for dette sprog (-1 angiver ingen grænse)"
 
 #: libretranslate/locales/.swag.py:45
 msgid "Frontend translation timeout"
-msgstr "Frontend oversættelsestidspunktout"
+msgstr "Timeout for frontend-oversættelse"
 
 #: libretranslate/locales/.swag.py:46
 msgid "Whether the API key database is enabled."
 msgstr "Om API-nøgledatabasen er aktiveret."
 
 #: libretranslate/locales/.swag.py:47
 msgid "Whether an API key is required."
-msgstr "Om en API-nøgle kræves."
+msgstr "Om en API-nøgle er påkrævet."
 
 #: libretranslate/locales/.swag.py:48
 msgid "Whether submitting suggestions is enabled."
 msgstr "Om indsendelse af forslag er aktiveret."
 
 #: libretranslate/locales/.swag.py:49
 msgid "Supported files format"
-msgstr "Understøttet filformat"
+msgstr "Understøttede filformater"
 
 #: libretranslate/locales/.swag.py:50
 msgid "Whether submission was successful"
 msgstr "Om indsendelse var vellykket"
 
 #: libretranslate/templates/app.js.template:31
 #: libretranslate/templates/app.js.template:286
@@ -472,16 +471,16 @@
 msgstr "Kopieret"
 
 #: libretranslate/templates/app.js.template:331
 msgid ""
 "Thanks for your correction. Note the suggestion will not take effect "
 "right away."
 msgstr ""
-"Tak for din korrektion. Bemærk, at forslaget ikke vil tage virkning med "
-"det samme."
+"Tak for din rettelse. Bemærk, at forslaget ikke vil træde i kraft med det "
+"samme."
 
 #: libretranslate/templates/app.js.template:455
 msgid "No languages available. Did you install the models correctly?"
 msgstr "Ingen tilgængelige sprog. Har du installeret modellerne korrekt?"
 
 #: libretranslate/templates/app.js.template:522
 #, python-format
@@ -495,85 +494,85 @@
 #: libretranslate/templates/app.js.template:522
 msgid "contact the server operator."
 msgstr "kontakt serveroperatøren."
 
 #: libretranslate/templates/index.html:9 libretranslate/templates/index.html:27
 #: libretranslate/templates/index.html:336
 msgid "Free and Open Source Machine Translation API"
-msgstr "Gratis og Open Source Machine Oversættelse API"
+msgstr "Gratis og Open Source Maskinoversættelses-API"
 
 #: libretranslate/templates/index.html:10
 #: libretranslate/templates/index.html:31
 msgid ""
 "Free and Open Source Machine Translation API. Self-hosted, offline "
 "capable and easy to setup. Run your own API server in just a few minutes."
 msgstr ""
-"Gratis og Open Source Machine Oversættelse API. Self-hosted, offline i "
-"stand og let at konfigurere. Kør din egen API-server på blot et par "
+"Gratis og Open Source Maskinoversættelses-API. Selv-hosted, kan bruges "
+"offline og er let at opsætte. Kør din egen API-server på blot et par "
 "minutter."
 
 #: libretranslate/templates/index.html:11
 msgid "translation"
-msgstr "oversættelse af oversættelse"
+msgstr "oversættelse"
 
 #: libretranslate/templates/index.html:11
 msgid "api"
 msgstr "api"
 
 #: libretranslate/templates/index.html:65
 msgid "API Docs"
 msgstr "API Docs"
 
 #: libretranslate/templates/index.html:67
 msgid "Get API Key"
-msgstr "Få API Nøglenøgle"
+msgstr "Få API-nøgle"
 
 #: libretranslate/templates/index.html:69
 msgid "GitHub"
 msgstr "GitHub"
 
 #: libretranslate/templates/index.html:71
 msgid "Set API Key"
-msgstr "Indstil API Nøglenøgle"
+msgstr "Indstil API-nøgle"
 
 #: libretranslate/templates/index.html:73
 msgid "Change language"
 msgstr "Skift sprog"
 
 #: libretranslate/templates/index.html:79
 msgid "Edit"
-msgstr "Rediger redigering"
+msgstr "Rediger"
 
 #: libretranslate/templates/index.html:81
 msgid "Toggle dark/light mode"
-msgstr "Skift mørke/lysetilstand"
+msgstr "Skift mellem mørk/lys tilstand"
 
 #: libretranslate/templates/index.html:157
 msgid "Dismiss"
-msgstr "Begrænsninger"
+msgstr "Afvis"
 
 #: libretranslate/templates/index.html:171
 msgid "Translation API"
 msgstr "Oversættelses-API"
 
 #: libretranslate/templates/index.html:175
 msgid "Translate Text"
-msgstr "Oversæt tekst"
+msgstr "Oversæt Tekst"
 
 #: libretranslate/templates/index.html:179
 msgid "Translate Files"
-msgstr "Oversæt filer"
+msgstr "Oversæt Filer"
 
 #: libretranslate/templates/index.html:185
 msgid "Translate from"
 msgstr "Oversæt fra"
 
 #: libretranslate/templates/index.html:195
 msgid "Swap source and target languages"
-msgstr "Skift kilde- og målsprog"
+msgstr "Byt om på kilde- og målsprog"
 
 #: libretranslate/templates/index.html:198
 msgid "Translate into"
 msgstr "Oversæt til"
 
 #: libretranslate/templates/index.html:210
 msgid "Text to translate"
@@ -585,15 +584,15 @@
 
 #: libretranslate/templates/index.html:226
 msgid "Suggest translation"
 msgstr "Foreslå oversættelse"
 
 #: libretranslate/templates/index.html:230
 msgid "Cancel"
-msgstr "Annuller"
+msgstr "annullere"
 
 #: libretranslate/templates/index.html:233
 msgid "Send"
 msgstr "Send"
 
 #: libretranslate/templates/index.html:249
 msgid "Supported file formats:"
@@ -610,31 +609,31 @@
 #: libretranslate/templates/index.html:275
 msgid "Translate"
 msgstr "Oversæt"
 
 #: libretranslate/templates/index.html:276
 #: libretranslate/templates/index.html:320
 msgid "Download"
-msgstr "Download"
+msgstr "Hent"
 
 #: libretranslate/templates/index.html:295
 msgid "Request"
-msgstr "Anmod om forespørgsel"
+msgstr "Anmod"
 
 #: libretranslate/templates/index.html:300
 msgid "Response"
 msgstr "Svar"
 
 #: libretranslate/templates/index.html:315
 msgid "Open Source Machine Translation API"
-msgstr "Maskinoversættelses-API med åben kildekode"
+msgstr "Open Source Maskinoversættelses-API"
 
 #: libretranslate/templates/index.html:316
 msgid "Self-Hosted. Offline Capable. Easy to Setup."
-msgstr "Self-Hosted. Offline Capable. Nem at konfigurere."
+msgstr "Selv-Hosted. Kan bruges offline. Nem at opsætte."
 
 #: libretranslate/templates/index.html:335
 msgid "LibreTranslate"
 msgstr "LibreTranslate"
 
 #: libretranslate/templates/index.html:337
 msgid "License:"
@@ -643,31 +642,31 @@
 #: libretranslate/templates/index.html:340
 #, python-format
 msgid ""
 "This public API should be used for testing, personal or infrequent use. "
 "If you're going to run an application in production, please "
 "%(host_server)s or %(get_api_key)s."
 msgstr ""
-"Denne offentlige API skal bruges til test, personlig eller sjælden brug. "
-"Hvis du vil køre en ansøgning i produktionen, bedes du venligst "
-"%(host_server)s eller %(get_api_key)s."
+"Denne offentlige API bør bruges til test, personlig eller sjælden brug. Hvis "
+"du har tænkt dig at køre en applikation i produktion, venligst %(host_server)"
+"s eller %(get_api_key)s."
 
 #: libretranslate/templates/index.html:340
 msgid "host your own server"
 msgstr "host din egen server"
 
 #: libretranslate/templates/index.html:340
 msgid "get an API key"
 msgstr "få en API-nøgle"
 
 #: libretranslate/templates/index.html:348
 #, python-format
 msgid "Made with %(heart)s by %(contributors)s and powered by %(engine)s"
-msgstr "Lavet med %(heart)s af by %(contributors)s og drevet af %(engine)s"
+msgstr "Lavet med %(heart)s af %(contributors)s og drevet af %(engine)s"
 
 #: libretranslate/templates/index.html:348
 #, python-format
 msgid "%(libretranslate)s Contributors"
-msgstr "%(libretranslate)s-bidragsydere"
+msgstr "%(libretranslate)s Bidragsydere"
 
 #~ msgid "multipart/form-data"
 #~ msgstr "multipart/form-data"
```

### Comparing `libretranslate-1.5.6/libretranslate/locales/de/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/el/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/eo/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/eo/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/es/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/et/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/eu/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/eu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/ext/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/ext/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/fa/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/fa/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: LibreTranslate 1.3.9\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2023-10-09 15:17-0400\n"
-"PO-Revision-Date: 2023-12-26 21:08+0000\n"
-"Last-Translator: Moji Norouzi zadeh <mnz1988@aol.com>\n"
+"PO-Revision-Date: 2024-04-07 09:57+0000\n"
+"Last-Translator: Ilya <ilyagvc2@gmail.com>\n"
 "Language-Team: Persian <https://hosted.weblate.org/projects/libretranslate/"
 "app/fa/>\n"
 "Language: fa\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: libretranslate/app.py:79
 msgid "Invalid JSON format"
 msgstr "فرمت JSON نامعتبر است"
 
 #: libretranslate/app.py:149 libretranslate/templates/app.js.template:459
@@ -58,22 +58,21 @@
 #: libretranslate/app.py:529 libretranslate/app.py:741
 #: libretranslate/app.py:743 libretranslate/app.py:745
 #: libretranslate/app.py:896 libretranslate/app.py:1053
 #: libretranslate/app.py:1055 libretranslate/app.py:1057
 #: libretranslate/app.py:1059
 #, python-format
 msgid "Invalid request: missing %(name)s parameter"
-msgstr "درخواست نامعتبر است: پارامتر %(name)s وجود ندارد"
+msgstr "درخواست نامعتبر: پارامتر %(name)s وجود ندارد"
 
 #: libretranslate/app.py:544 libretranslate/app.py:553
 #, python-format
 msgid "Invalid request: request (%(size)s) exceeds text limit (%(limit)s)"
 msgstr ""
-"درخواست نامعتبر است: درخواست (%(size)s) از محدودیت متنی (%(limit)s) فراتر"
-" رفت"
+"درخواست نامعتبر: درخواست (%(size)s) از محدودیت متنی (%(limit)s) فراتر رفت"
 
 #: libretranslate/app.py:583 libretranslate/app.py:588
 #: libretranslate/app.py:758 libretranslate/app.py:763
 #, python-format
 msgid "%(lang)s is not supported"
 msgstr "%(lang)s پشتیبانی نمی‌شود"
 
@@ -84,16 +83,16 @@
 
 #: libretranslate/app.py:602 libretranslate/app.py:626
 #, python-format
 msgid ""
 "%(tname)s (%(tcode)s) is not available as a target language from "
 "%(sname)s (%(scode)s)"
 msgstr ""
-"(%(tcode)s) (%(tname)s) از (%(scode)s) (%(sname)s)به‌عنوان یک زبان هدف در"
-" دسترس نیست"
+"(%(tcode)s) (%(tname)s) از (%(scode)s) (%(sname)s) به عنوان یک زبان هدف در "
+"دسترس نیست"
 
 #: libretranslate/app.py:647
 #, python-format
 msgid "Cannot translate text: %(text)s"
 msgstr "متن قابل ترجمه نیست: %(text)s"
 
 #: libretranslate/app.py:734 libretranslate/app.py:788
@@ -130,15 +129,15 @@
 
 #: libretranslate/locales/.langs.py:4
 msgid "Chinese"
 msgstr "چینی"
 
 #: libretranslate/locales/.langs.py:5
 msgid "Czech"
-msgstr "چکی"
+msgstr "(کشور) چک"
 
 #: libretranslate/locales/.langs.py:6
 msgid "Danish"
 msgstr "دانمارکی"
 
 #: libretranslate/locales/.langs.py:7
 msgid "Dutch"
@@ -194,15 +193,15 @@
 
 #: libretranslate/locales/.langs.py:20
 msgid "Korean"
 msgstr "کره‌ای"
 
 #: libretranslate/locales/.langs.py:21
 msgid "Persian"
-msgstr "فارسی"
+msgstr "پارسی"
 
 #: libretranslate/locales/.langs.py:22
 msgid "Polish"
 msgstr "لهستانی"
 
 #: libretranslate/locales/.langs.py:23
 msgid "Portuguese"
@@ -300,15 +299,15 @@
 msgid ""
 "Format of source text:\n"
 " * `text` - Plain text\n"
 " * `html` - HTML markup\n"
 msgstr ""
 "فرمت متن منبع:\n"
 "* text - متن ساده\n"
-"* html - کدهای اچ تی ام ال\n"
+"* html - حالت های html\n"
 
 #: libretranslate/locales/.swag.py:17
 msgid "API key"
 msgstr "کلید API"
 
 #: libretranslate/locales/.swag.py:18
 msgid "Translate file from a language to another"
@@ -336,31 +335,31 @@
 
 #: libretranslate/locales/.swag.py:24
 msgid "Text to detect"
 msgstr "متن برای شناسایی"
 
 #: libretranslate/locales/.swag.py:25
 msgid "Retrieve frontend specific settings"
-msgstr "بازیابی تنظیمات ویژه نما"
+msgstr "بازیابی تنظیمات ظاهری ویژه"
 
 #: libretranslate/locales/.swag.py:26
 msgid "frontend settings"
-msgstr "تنظیمات صفحه نما"
+msgstr "تنظیمات ظاهری"
 
 #: libretranslate/locales/.swag.py:27
 msgid "frontend"
-msgstr "صفحه نما"
+msgstr "نما ظاهری"
 
 #: libretranslate/locales/.swag.py:28
 msgid "Submit a suggestion to improve a translation"
 msgstr "پیشنهادی برای بهبود ترجمه ثبت نمایید"
 
 #: libretranslate/locales/.swag.py:29
 msgid "Success"
-msgstr "موفقیت‌آمیز بود"
+msgstr "موفقیت‌آمیز"
 
 #: libretranslate/locales/.swag.py:30
 msgid "Not authorized"
 msgstr "مجاز نیست"
 
 #: libretranslate/locales/.swag.py:31
 msgid "Original text"
@@ -412,19 +411,19 @@
 
 #: libretranslate/locales/.swag.py:43
 msgid "Confidence value"
 msgstr "ضریب اطمینان"
 
 #: libretranslate/locales/.swag.py:44
 msgid "Character input limit for this language (-1 indicates no limit)"
-msgstr "محدودیت کاراکتر برای این زبان (-1 یعنی بدون محدودیتت)"
+msgstr "محدودیت کاراکتر برای این زبان (-1 یعنی بدون محدودیت)"
 
 #: libretranslate/locales/.swag.py:45
 msgid "Frontend translation timeout"
-msgstr "محدودیت زمانی ترجمه برای صفحه نما"
+msgstr "محدودیت زمانی ترجمه برای نمای ظاهری"
 
 #: libretranslate/locales/.swag.py:46
 msgid "Whether the API key database is enabled."
 msgstr "اینکه (آیا) پایگاه داده مربوط به کلید API فعال است."
 
 #: libretranslate/locales/.swag.py:47
 msgid "Whether an API key is required."
@@ -432,15 +431,15 @@
 
 #: libretranslate/locales/.swag.py:48
 msgid "Whether submitting suggestions is enabled."
 msgstr "اینکه (آیا) ارسال پیشنهادات ممکن است."
 
 #: libretranslate/locales/.swag.py:49
 msgid "Supported files format"
-msgstr "قالب فایل‌های پشتیبانی شده"
+msgstr "فرمت فایل‌های پشتیبانی شده"
 
 #: libretranslate/locales/.swag.py:50
 msgid "Whether submission was successful"
 msgstr "اینکه (آیا) ارسال موفقیت‌آمیز بود"
 
 #: libretranslate/templates/app.js.template:31
 #: libretranslate/templates/app.js.template:286
@@ -487,15 +486,15 @@
 msgid "Type in your API Key. If you need an API key, %(instructions)s"
 msgstr ""
 "کلید API خود را وارد نمایید. اگر به یک کلید API نیاز دارید، "
 "%(instructions)s"
 
 #: libretranslate/templates/app.js.template:522
 msgid "press the \"Get API Key\" link."
-msgstr "بر روی \"دریافت کلید API\" کلیک کنید."
+msgstr "بر روی لینک \"دریافت کلید API\" کلیک کنید."
 
 #: libretranslate/templates/app.js.template:522
 msgid "contact the server operator."
 msgstr "با اپراتور سرور تماس بگیرید."
 
 #: libretranslate/templates/index.html:9 libretranslate/templates/index.html:27
 #: libretranslate/templates/index.html:336
@@ -525,15 +524,15 @@
 
 #: libretranslate/templates/index.html:67
 msgid "Get API Key"
 msgstr "دریافت کلید API"
 
 #: libretranslate/templates/index.html:69
 msgid "GitHub"
-msgstr "گیتهاب"
+msgstr "گیت‌هاب"
 
 #: libretranslate/templates/index.html:71
 msgid "Set API Key"
 msgstr "تنظیم کلید API"
 
 #: libretranslate/templates/index.html:73
 msgid "Change language"
@@ -541,15 +540,15 @@
 
 #: libretranslate/templates/index.html:79
 msgid "Edit"
 msgstr "ویرایش"
 
 #: libretranslate/templates/index.html:81
 msgid "Toggle dark/light mode"
-msgstr "تغییر به حالت تیره / روشن"
+msgstr "تغییر به حالت تیره/روشن"
 
 #: libretranslate/templates/index.html:157
 msgid "Dismiss"
 msgstr "انصراف"
 
 #: libretranslate/templates/index.html:171
 msgid "Translation API"
@@ -643,21 +642,21 @@
 #: libretranslate/templates/index.html:340
 #, python-format
 msgid ""
 "This public API should be used for testing, personal or infrequent use. "
 "If you're going to run an application in production, please "
 "%(host_server)s or %(get_api_key)s."
 msgstr ""
-"این API عمومی باید برای آزمایش، کاربری شخصی یا اختصاصی است. اگر قرار است "
+"این API عمومی باید برای آزمایش، استفاده شخصی یا اختصاصی است. اگر قرار است "
 "برنامه‌ای که برای محصول است با آن اجرا کنید، لطفا %(host_server)s یا "
 "%(get_api_key)s."
 
 #: libretranslate/templates/index.html:340
 msgid "host your own server"
-msgstr "سرور خود را میزبانی کنید"
+msgstr "در سرور خود میزبانی کنید"
 
 #: libretranslate/templates/index.html:340
 msgid "get an API key"
 msgstr "یک کلید API بگیرید"
 
 #: libretranslate/templates/index.html:348
 #, python-format
```

### Comparing `libretranslate-1.5.6/libretranslate/locales/fi/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/fi/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/fr/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/ga/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/ga/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/gl/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/he/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/he/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/hi/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/hi/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/hu/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/hu/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,36 +5,37 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: LibreTranslate 1.3.9\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2023-10-09 15:17-0400\n"
-"PO-Revision-Date: 2023-02-25 11:36+0000\n"
-"Last-Translator: ebela <bela@dandre.hu>\n"
+"PO-Revision-Date: 2024-04-18 08:04+0000\n"
+"Last-Translator: Netesfiu <r4verino@gmail.com>\n"
+"Language-Team: Hungarian <https://hosted.weblate.org/projects/libretranslate/"
+"app/hu/>\n"
 "Language: hu\n"
-"Language-Team: Hungarian "
-"<https://hosted.weblate.org/projects/libretranslate/app/hu/>\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 5.5-dev\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: libretranslate/app.py:79
 msgid "Invalid JSON format"
 msgstr "Érvénytelen JSON formátum"
 
 #: libretranslate/app.py:149 libretranslate/templates/app.js.template:459
 msgid "Auto Detect"
 msgstr "Automatikus felismerés"
 
 #: libretranslate/app.py:232
 msgid "Unauthorized"
-msgstr "Nem engedélyezett"
+msgstr "Nincs jogosultsága"
 
 #: libretranslate/app.py:250
 msgid "Too many request limits violations"
 msgstr "Túl sok kérelem korlátozza a jogsértéseket"
 
 #: libretranslate/app.py:257
 msgid "Invalid API key"
@@ -45,15 +46,15 @@
 msgstr ""
 "Kérjük, vegye fel a kapcsolatot a szerver-üzemeltetővel, hogy megkapja az"
 " API kulcsot"
 
 #: libretranslate/app.py:278
 #, python-format
 msgid "Visit %(url)s to get an API key"
-msgstr "Látogatás %(url)s API kulcsot kapni"
+msgstr "Látogasson el a(z) %(url)s címre, API kulcshoz"
 
 #: libretranslate/app.py:318
 msgid "Slowdown:"
 msgstr "Lassulás:"
 
 #: libretranslate/app.py:525 libretranslate/app.py:527
 #: libretranslate/app.py:529 libretranslate/app.py:741
@@ -65,22 +66,22 @@
 msgid "Invalid request: missing %(name)s parameter"
 msgstr "Érvénytelen kérés: hiányzik a(z) %(name)s paraméter"
 
 #: libretranslate/app.py:544 libretranslate/app.py:553
 #, python-format
 msgid "Invalid request: request (%(size)s) exceeds text limit (%(limit)s)"
 msgstr ""
-"Érvénytelen kérés: kérés (%(size)s) meghaladja a szövegkorlátot "
+"Érvénytelen kérés: a kérés mérete (%(size)s) meghaladja a szövegkorlátot "
 "(%(limit)s)"
 
 #: libretranslate/app.py:583 libretranslate/app.py:588
 #: libretranslate/app.py:758 libretranslate/app.py:763
 #, python-format
 msgid "%(lang)s is not supported"
-msgstr "%(lang)s nem támogatott"
+msgstr "%(lang)s nyelv nem támogatott"
 
 #: libretranslate/app.py:594
 #, python-format
 msgid "%(format)s format is not supported"
 msgstr "%(format)s formátum nem támogatott"
 
 #: libretranslate/app.py:602 libretranslate/app.py:626
@@ -95,15 +96,15 @@
 #: libretranslate/app.py:647
 #, python-format
 msgid "Cannot translate text: %(text)s"
 msgstr "Nem fordítható szöveg: %(text)s"
 
 #: libretranslate/app.py:734 libretranslate/app.py:788
 msgid "Files translation are disabled on this server."
-msgstr "Files fordítás letiltása ezen a szerveren."
+msgstr "Fájlok fordítása kikapcsolva ezen a szerveren."
 
 #: libretranslate/app.py:748
 msgid "Invalid request: empty file"
 msgstr "Érvénytelen kérés: üres fájl"
 
 #: libretranslate/app.py:751
 msgid "Invalid request: file format not supported"
@@ -111,15 +112,15 @@
 
 #: libretranslate/app.py:796
 msgid "Invalid filename"
 msgstr "Érvénytelen fájlnév"
 
 #: libretranslate/app.py:1038
 msgid "Suggestions are disabled on this server."
-msgstr "A javaslatok fogyatékkal élők ezen a szerveren."
+msgstr "A javaslatok kikapcsolva ezen a szerveren."
 
 #: libretranslate/locales/.langs.py:1
 msgid "English"
 msgstr "Angol"
 
 #: libretranslate/locales/.langs.py:2
 msgid "Arabic"
@@ -131,27 +132,27 @@
 
 #: libretranslate/locales/.langs.py:4
 msgid "Chinese"
 msgstr "Kínai"
 
 #: libretranslate/locales/.langs.py:5
 msgid "Czech"
-msgstr "Csehország"
+msgstr "Cseh"
 
 #: libretranslate/locales/.langs.py:6
 msgid "Danish"
 msgstr "Dán"
 
 #: libretranslate/locales/.langs.py:7
 msgid "Dutch"
-msgstr "Hollandia"
+msgstr "Holland"
 
 #: libretranslate/locales/.langs.py:8
 msgid "Esperanto"
-msgstr "Esperanto"
+msgstr "Eszperantó"
 
 #: libretranslate/locales/.langs.py:9
 msgid "Finnish"
 msgstr "Finn"
 
 #: libretranslate/locales/.langs.py:10
 msgid "French"
@@ -179,23 +180,23 @@
 
 #: libretranslate/locales/.langs.py:16
 msgid "Indonesian"
 msgstr "Indonéz"
 
 #: libretranslate/locales/.langs.py:17
 msgid "Irish"
-msgstr "Írország"
+msgstr "Ír"
 
 #: libretranslate/locales/.langs.py:18
 msgid "Italian"
 msgstr "Olasz"
 
 #: libretranslate/locales/.langs.py:19
 msgid "Japanese"
-msgstr "Japán japán"
+msgstr "Japán"
 
 #: libretranslate/locales/.langs.py:20
 msgid "Korean"
 msgstr "Koreai"
 
 #: libretranslate/locales/.langs.py:21
 msgid "Persian"
@@ -203,31 +204,31 @@
 
 #: libretranslate/locales/.langs.py:22
 msgid "Polish"
 msgstr "Lengyel"
 
 #: libretranslate/locales/.langs.py:23
 msgid "Portuguese"
-msgstr "Portugália"
+msgstr "Portugál"
 
 #: libretranslate/locales/.langs.py:24
 msgid "Russian"
 msgstr "Orosz"
 
 #: libretranslate/locales/.langs.py:25
 msgid "Slovak"
-msgstr "Szlovákia"
+msgstr "Szlovák"
 
 #: libretranslate/locales/.langs.py:26
 msgid "Spanish"
 msgstr "Spanyol"
 
 #: libretranslate/locales/.langs.py:27
 msgid "Swedish"
-msgstr "Svédország"
+msgstr "Svéd"
 
 #: libretranslate/locales/.langs.py:28
 msgid "Turkish"
 msgstr "Török"
 
 #: libretranslate/locales/.langs.py:29
 msgid "Ukranian"
@@ -235,15 +236,15 @@
 
 #: libretranslate/locales/.langs.py:30
 msgid "Vietnamese"
 msgstr "Vietnami"
 
 #: libretranslate/locales/.swag.py:1
 msgid "Retrieve list of supported languages"
-msgstr "A támogatott nyelvek újraindítása"
+msgstr "A támogatott nyelvek listájának lekérése"
 
 #: libretranslate/locales/.swag.py:2
 msgid "List of languages"
 msgstr "A nyelvek listája"
 
 #: libretranslate/locales/.swag.py:3
 msgid "translate"
@@ -263,19 +264,19 @@
 
 #: libretranslate/locales/.swag.py:7
 msgid "Translation error"
 msgstr "Fordítási hiba"
 
 #: libretranslate/locales/.swag.py:8
 msgid "Slow down"
-msgstr "Lassabb"
+msgstr "Lassabban"
 
 #: libretranslate/locales/.swag.py:9
 msgid "Banned"
-msgstr "Betiltott"
+msgstr "Tiltott"
 
 #: libretranslate/locales/.swag.py:10
 msgid "Hello world!"
 msgstr "Hello világ!"
 
 #: libretranslate/locales/.swag.py:11
 msgid "Text(s) to translate"
@@ -300,15 +301,15 @@
 #: libretranslate/locales/.swag.py:16
 msgid ""
 "Format of source text:\n"
 " * `text` - Plain text\n"
 " * `html` - HTML markup\n"
 msgstr ""
 "Formátum forrás szöveg:\n"
-"* `text' - Plain szöveg\n"
+"* `text' - egyszerű szöveg\n"
 "* `html' - HTML markup\n"
 
 #: libretranslate/locales/.swag.py:17
 msgid "API key"
 msgstr "API kulcs"
 
 #: libretranslate/locales/.swag.py:18
@@ -321,15 +322,15 @@
 
 #: libretranslate/locales/.swag.py:20
 msgid "File to translate"
 msgstr "Fájl fordítása"
 
 #: libretranslate/locales/.swag.py:21
 msgid "Detect the language of a single text"
-msgstr "Védje meg egyetlen szöveg nyelvét"
+msgstr "A szöveg nyelvének észlelése"
 
 #: libretranslate/locales/.swag.py:22
 msgid "Detections"
 msgstr "Észlelések"
 
 #: libretranslate/locales/.swag.py:23
 msgid "Detection error"
@@ -345,19 +346,19 @@
 
 #: libretranslate/locales/.swag.py:26
 msgid "frontend settings"
 msgstr "frontend beállítások"
 
 #: libretranslate/locales/.swag.py:27
 msgid "frontend"
-msgstr "fénykép"
+msgstr "frontend"
 
 #: libretranslate/locales/.swag.py:28
 msgid "Submit a suggestion to improve a translation"
-msgstr "Javaslatot nyújt be a fordítás javítására"
+msgstr "Küldjön javaslatot a fordítés javításához"
 
 #: libretranslate/locales/.swag.py:29
 msgid "Success"
 msgstr "Siker"
 
 #: libretranslate/locales/.swag.py:30
 msgid "Not authorized"
@@ -401,198 +402,200 @@
 
 #: libretranslate/locales/.swag.py:40
 msgid "Error message"
 msgstr "Hibaüzenet"
 
 #: libretranslate/locales/.swag.py:41
 msgid "Reason for slow down"
-msgstr "Oka lassú le"
+msgstr "A lelassulás oka"
 
 #: libretranslate/locales/.swag.py:42
 msgid "Translated file url"
 msgstr "Fordított fájl url"
 
 #: libretranslate/locales/.swag.py:43
 msgid "Confidence value"
-msgstr "Biztonsági érték"
+msgstr "Bizalmi érték"
 
 #: libretranslate/locales/.swag.py:44
 msgid "Character input limit for this language (-1 indicates no limit)"
 msgstr "Jellemző bemeneti határértéke ennek a nyelvnek (-1 nem jelzi a határt)"
 
 #: libretranslate/locales/.swag.py:45
 msgid "Frontend translation timeout"
-msgstr "Frontend fordítási idő"
+msgstr "Frontend fordítás időtúllépés"
 
 #: libretranslate/locales/.swag.py:46
 msgid "Whether the API key database is enabled."
-msgstr "Függetlenül attól, hogy az API kulcsfontosságú adatbázisa engedélyezett-e."
+msgstr "Függetlenül attól, hogy az API kulcs adatbázisa engedélyezett-e."
 
 #: libretranslate/locales/.swag.py:47
 msgid "Whether an API key is required."
-msgstr "Függetlenül attól, hogy egy API kulcsra van szükség."
+msgstr "Szükséges-e API kulcs."
 
 #: libretranslate/locales/.swag.py:48
 msgid "Whether submitting suggestions is enabled."
-msgstr "Akár javaslatok benyújtása engedélyezett."
+msgstr "Ha javaslatok benyújtásá engedélyezett."
 
 #: libretranslate/locales/.swag.py:49
 msgid "Supported files format"
 msgstr "Támogatott fájlformátum"
 
 #: libretranslate/locales/.swag.py:50
 msgid "Whether submission was successful"
-msgstr "Akár sikeres volt a benyújtás"
+msgstr "Amennyiben a beküldsé sikeres volt"
 
 #: libretranslate/templates/app.js.template:31
 #: libretranslate/templates/app.js.template:286
 #: libretranslate/templates/app.js.template:290
 msgid "Copy text"
-msgstr "Másolás szöveg"
+msgstr "Szöveg másolása"
 
 #: libretranslate/templates/app.js.template:80
 #: libretranslate/templates/app.js.template:86
 #: libretranslate/templates/app.js.template:91
 #: libretranslate/templates/app.js.template:273
 #: libretranslate/templates/app.js.template:343
 #: libretranslate/templates/app.js.template:431
 #: libretranslate/templates/app.js.template:479
 #, python-format
 msgid "Cannot load %(url)s"
-msgstr "Nem tölthet %(url)s"
+msgstr "Nem tölthető be a(z) %(url)s"
 
 #: libretranslate/templates/app.js.template:264
 #: libretranslate/templates/app.js.template:334
 #: libretranslate/templates/app.js.template:412
 #: libretranslate/templates/app.js.template:423
 msgid "Unknown error"
 msgstr "Ismeretlen hiba"
 
 #: libretranslate/templates/app.js.template:287
 msgid "Copied"
-msgstr "Második"
+msgstr "Másolva"
 
 #: libretranslate/templates/app.js.template:331
 msgid ""
 "Thanks for your correction. Note the suggestion will not take effect "
 "right away."
 msgstr ""
-"Köszönöm a korrekciót. Ne feledje, hogy a javaslat nem fog azonnal "
+"Köszönöm a korrekciót. Vegye figyelembe, hogy a javaslata nem fog azonnal "
 "hatályba lépni."
 
 #: libretranslate/templates/app.js.template:455
 msgid "No languages available. Did you install the models correctly?"
-msgstr "Nincsenek nyelvek. Helyesen telepítette a modelleket?"
+msgstr "Nincsenek elérhető nyelvek. Helyesen telepítette a modelleket?"
 
 #: libretranslate/templates/app.js.template:522
 #, python-format
 msgid "Type in your API Key. If you need an API key, %(instructions)s"
-msgstr "Típus az API kulcsodban. Ha szüksége van egy API kulcsra, %(instructions)s"
+msgstr ""
+"Írja be az API kulcsot. Ha szüksége van egy API kulcsra, %(instructions)s"
 
 #: libretranslate/templates/app.js.template:522
 msgid "press the \"Get API Key\" link."
 msgstr "nyomja meg a \"Get API Key\" linket."
 
 #: libretranslate/templates/app.js.template:522
 msgid "contact the server operator."
 msgstr "lépjen kapcsolatba a szerver-üzemeltetővel."
 
 #: libretranslate/templates/index.html:9 libretranslate/templates/index.html:27
 #: libretranslate/templates/index.html:336
 msgid "Free and Open Source Machine Translation API"
-msgstr "Ingyenes és nyílt forráskódú gép fordítás API"
+msgstr "Ingyenes és nyílt forráskódú gépi fordító API"
 
 #: libretranslate/templates/index.html:10
 #: libretranslate/templates/index.html:31
 msgid ""
 "Free and Open Source Machine Translation API. Self-hosted, offline "
 "capable and easy to setup. Run your own API server in just a few minutes."
 msgstr ""
-"Ingyenes és nyílt forráskódú gép fordítás API. Önálló, offline képes és "
-"könnyen telepíthető. Futtassa saját API szerverét néhány perc alatt."
+"Ingyenes és nyílt forráskódú gépi fordító  API. Helyileg telepített, offline "
+"működő és könnyen telepíthető. Futtassa saját API szerverét néhány perc "
+"alatt."
 
 #: libretranslate/templates/index.html:11
 msgid "translation"
 msgstr "fordítás"
 
 #: libretranslate/templates/index.html:11
 msgid "api"
 msgstr "api"
 
 #: libretranslate/templates/index.html:65
 msgid "API Docs"
-msgstr "API Docs"
+msgstr "API Dokumentáció"
 
 #: libretranslate/templates/index.html:67
 msgid "Get API Key"
-msgstr "Szerezd meg az API-t Key"
+msgstr "Szerezzen API kucsot"
 
 #: libretranslate/templates/index.html:69
 msgid "GitHub"
 msgstr "GitHub"
 
 #: libretranslate/templates/index.html:71
 msgid "Set API Key"
-msgstr "Állítsa be az API-t Key"
+msgstr "Állítsa be az API kulcsot"
 
 #: libretranslate/templates/index.html:73
 msgid "Change language"
-msgstr "Változási nyelv"
+msgstr "Nyelv módosítása"
 
 #: libretranslate/templates/index.html:79
 msgid "Edit"
 msgstr "Szerkesztés"
 
 #: libretranslate/templates/index.html:81
 msgid "Toggle dark/light mode"
-msgstr "Toggle sötét / fény mód"
+msgstr "Váltás sötét/világos módra"
 
 #: libretranslate/templates/index.html:157
 msgid "Dismiss"
-msgstr "Elbocsátások"
+msgstr "elvetés"
 
 #: libretranslate/templates/index.html:171
 msgid "Translation API"
-msgstr "Fordítás API"
+msgstr "Fordító API"
 
 #: libretranslate/templates/index.html:175
 msgid "Translate Text"
-msgstr "Fordító szöveg"
+msgstr "Szöveg Fordítása"
 
 #: libretranslate/templates/index.html:179
 msgid "Translate Files"
-msgstr "Fordító fájlok"
+msgstr "File-ok fordítása"
 
 #: libretranslate/templates/index.html:185
 msgid "Translate from"
-msgstr "Fordítsd le"
+msgstr "Fordítási ürlap"
 
 #: libretranslate/templates/index.html:195
 msgid "Swap source and target languages"
-msgstr "Swap forrás és célnyelvek"
+msgstr "Forrás és célnyelv felcserélése"
 
 #: libretranslate/templates/index.html:198
 msgid "Translate into"
-msgstr "Fordítsd le"
+msgstr "Fordítsd le ebbe"
 
 #: libretranslate/templates/index.html:210
 msgid "Text to translate"
-msgstr "Fordítás szövege"
+msgstr "Fordítandó szöveg"
 
 #: libretranslate/templates/index.html:213
 msgid "Delete text"
-msgstr "Törlés szöveg"
+msgstr "szöveg törlése"
 
 #: libretranslate/templates/index.html:226
 msgid "Suggest translation"
-msgstr "Legjobb fordítás"
+msgstr "Javasolj fordítást"
 
 #: libretranslate/templates/index.html:230
 msgid "Cancel"
-msgstr "Törlés"
+msgstr "mégse"
 
 #: libretranslate/templates/index.html:233
 msgid "Send"
 msgstr "Küldés"
 
 #: libretranslate/templates/index.html:249
 msgid "Supported file formats:"
@@ -600,15 +603,15 @@
 
 #: libretranslate/templates/index.html:253
 msgid "File"
 msgstr "File"
 
 #: libretranslate/templates/index.html:268
 msgid "Remove file"
-msgstr "Távolítsa el a fájlt"
+msgstr "File eltávolítása"
 
 #: libretranslate/templates/index.html:275
 msgid "Translate"
 msgstr "Fordítás"
 
 #: libretranslate/templates/index.html:276
 #: libretranslate/templates/index.html:320
@@ -625,49 +628,50 @@
 
 #: libretranslate/templates/index.html:315
 msgid "Open Source Machine Translation API"
 msgstr "Nyilt Forráskódú Gépi Fordító API"
 
 #: libretranslate/templates/index.html:316
 msgid "Self-Hosted. Offline Capable. Easy to Setup."
-msgstr "Önmagát választotta. Offline Képes. Könnyű a beállításhoz."
+msgstr "Helyben futtatható, offline működő. Könnyen beállítható."
 
 #: libretranslate/templates/index.html:335
 msgid "LibreTranslate"
 msgstr "LibreTranslate"
 
 #: libretranslate/templates/index.html:337
 msgid "License:"
-msgstr "Engedély:"
+msgstr "Licenc:"
 
 #: libretranslate/templates/index.html:340
 #, python-format
 msgid ""
 "This public API should be used for testing, personal or infrequent use. "
 "If you're going to run an application in production, please "
 "%(host_server)s or %(get_api_key)s."
 msgstr ""
-"Ezt a nyilvános API-t tesztelésre, személyes vagy alkalmankénti "
-"használatra használhatod. Amennyiben az alkalmazásod éles környezetben "
-"fogod használni úgy használd a %(host_server)s-t vagy %(get_api_key)s-t."
+"Ezt a nyilvános API-t tesztelésre, személyes vagy alkalmi használatra "
+"használandó. Amennyiben az alkalmazásod éles környezetben fogod használni "
+"úgy használd a %(host_server)s-t vagy %(get_api_key)s-t."
 
 #: libretranslate/templates/index.html:340
 msgid "host your own server"
-msgstr "fogadja el saját szerverét"
+msgstr "Hosztold a saját szervered"
 
 #: libretranslate/templates/index.html:340
 msgid "get an API key"
-msgstr "kap egy API kulcsot"
+msgstr "API kulcs szerzése"
 
 #: libretranslate/templates/index.html:348
 #, python-format
 msgid "Made with %(heart)s by %(contributors)s and powered by %(engine)s"
-msgstr "Made with %(heart)s által %(contributors)s és erőteljes %(engine)s"
+msgstr ""
+"%(heart)s-el készítve. Közreműködtek %(contributors)s működtetve ezzel: "
+"%(engine)s"
 
 #: libretranslate/templates/index.html:348
 #, python-format
 msgid "%(libretranslate)s Contributors"
 msgstr "%(libretranslate)s Közreműködők"
 
 #~ msgid "multipart/form-data"
 #~ msgstr "multipart/form-data"
-
```

### Comparing `libretranslate-1.5.6/libretranslate/locales/id/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/id/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/it/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/ja/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/kab/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/kab/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/ko/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/ko/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/nb_NO/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/nb_NO/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: LibreTranslate 1.3.9\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2023-01-06 17:52-0500\n"
-"PO-Revision-Date: 2023-06-03 02:40+0000\n"
-"Last-Translator: \"T. Alexander\" <theools@gmail.com>\n"
+"PO-Revision-Date: 2024-03-25 12:01+0000\n"
+"Last-Translator: Kaleido Scope <senpai@firemail.cc>\n"
 "Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/"
 "libretranslate/app/nb_NO/>\n"
 "Language: nb_NO\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.18-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 "Generated-By: Babel 2.11.0\n"
 
 #: libretranslate/app.py:60
 msgid "Invalid JSON format"
 msgstr "Ugyldig JSON-format"
 
 #: libretranslate/app.py:128 libretranslate/templates/app.js.template:427
@@ -32,15 +32,15 @@
 #: libretranslate/app.py:193
 msgid "Unauthorized"
 msgstr "Ikke godkjent"
 
 #: libretranslate/app.py:211
 #, fuzzy
 msgid "Too many request limits violations"
-msgstr "For mange forespørsler"
+msgstr "For mange brudd på forespørselsgrensene"
 
 #: libretranslate/app.py:220
 msgid "Invalid API key"
 msgstr "Ugyldig API-nøkkel"
 
 #: libretranslate/app.py:227
 msgid "Please contact the server operator to get an API key"
@@ -274,15 +274,15 @@
 
 #: libretranslate/locales/.swag.py:9
 msgid "Banned"
 msgstr "Bannlyst"
 
 #: libretranslate/locales/.swag.py:10
 msgid "Hello world!"
-msgstr "Hei verden."
+msgstr "Hei verden!"
 
 #: libretranslate/locales/.swag.py:11
 msgid "Text(s) to translate"
 msgstr "Tekst(er) å oversette"
 
 #: libretranslate/locales/.swag.py:12
 msgid "Source language code"
@@ -293,15 +293,14 @@
 msgstr "Målspråkkode"
 
 #: libretranslate/locales/.swag.py:14
 msgid "text"
 msgstr "tekst"
 
 #: libretranslate/locales/.swag.py:15
-#, fuzzy
 msgid "html"
 msgstr "HTML"
 
 #: libretranslate/locales/.swag.py:16
 msgid ""
 "Format of source text:\n"
 " * `text` - Plain text\n"
```

### Comparing `libretranslate-1.5.6/libretranslate/locales/nl/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/oc/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/oc/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/pa/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/pa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/pl/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/pt/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/pt_BR/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/ro/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/ru/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/si/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/si/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/sk/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/sq/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/sq/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/sr/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/sr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/sv/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/tr/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/ug/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/ug/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/uk/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/vi/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/vi/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/zgh/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/zgh/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/zh/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/zh/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/locales/zh_Hant/LC_MESSAGES/messages.po` & `libretranslate-1.5.7/libretranslate/locales/zh_Hant/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: LibreTranslate 1.3.9\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2023-01-06 17:52-0500\n"
-"PO-Revision-Date: 2023-05-18 17:53+0000\n"
+"PO-Revision-Date: 2024-04-23 20:07+0000\n"
 "Last-Translator: Peter Dave Hello <hsu@peterdavehello.org>\n"
 "Language-Team: Chinese (Traditional) <https://hosted.weblate.org/projects/"
 "libretranslate/app/zh_Hant/>\n"
 "Language: zh_Hant\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.18-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 "Generated-By: Babel 2.11.0\n"
 
 #: libretranslate/app.py:60
 msgid "Invalid JSON format"
 msgstr "無效的 JSON 格式"
 
 #: libretranslate/app.py:128 libretranslate/templates/app.js.template:427
```

### Comparing `libretranslate-1.5.6/libretranslate/static/favicon.ico` & `libretranslate-1.5.7/libretranslate/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/static/icon.svg` & `libretranslate-1.5.7/libretranslate/static/icon.svg`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/static/css/main.css` & `libretranslate-1.5.7/libretranslate/static/css/main.css`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/static/css/material-icons.css` & `libretranslate-1.5.7/libretranslate/static/css/material-icons.css`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/static/css/materialize.min.css` & `libretranslate-1.5.7/libretranslate/static/css/materialize.min.css`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/static/css/prism.min.css` & `libretranslate-1.5.7/libretranslate/static/css/prism.min.css`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/static/fonts/MaterialIcons-Regular.eot` & `libretranslate-1.5.7/libretranslate/static/fonts/MaterialIcons-Regular.eot`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/static/fonts/MaterialIcons-Regular.ttf` & `libretranslate-1.5.7/libretranslate/static/fonts/MaterialIcons-Regular.ttf`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/static/fonts/MaterialIcons-Regular.woff` & `libretranslate-1.5.7/libretranslate/static/fonts/MaterialIcons-Regular.woff`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/static/fonts/MaterialIcons-Regular.woff2` & `libretranslate-1.5.7/libretranslate/static/fonts/MaterialIcons-Regular.woff2`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/static/js/materialize.min.js` & `libretranslate-1.5.7/libretranslate/static/js/materialize.min.js`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/static/js/prism.min.js` & `libretranslate-1.5.7/libretranslate/static/js/prism.min.js`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/static/js/vue@2.js` & `libretranslate-1.5.7/libretranslate/static/js/vue@2.js`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/templates/app.js.template` & `libretranslate-1.5.7/libretranslate/templates/app.js.template`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/templates/index.html` & `libretranslate-1.5.7/libretranslate/templates/index.html`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/tests/test_api/test_api_detect_language.py` & `libretranslate-1.5.7/libretranslate/tests/test_api/test_api_detect_language.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/libretranslate/tests/test_api/test_api_translate.py` & `libretranslate-1.5.7/libretranslate/tests/test_api/test_api_translate.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/scripts/compile_locales.py` & `libretranslate-1.5.7/scripts/compile_locales.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/scripts/gunicorn_conf.py` & `libretranslate-1.5.7/scripts/gunicorn_conf.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/scripts/install_models.py` & `libretranslate-1.5.7/scripts/install_models.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/scripts/suggestions-to-jsonl.py` & `libretranslate-1.5.7/scripts/suggestions-to-jsonl.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/scripts/update_locales.py` & `libretranslate-1.5.7/scripts/update_locales.py`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/.gitignore` & `libretranslate-1.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/LICENSE` & `libretranslate-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `libretranslate-1.5.6/README.md` & `libretranslate-1.5.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
 ```javascript
 {
     "translatedText": "¡Hola!"
 }
 ```
 
+List of language codes: https://libretranslate.com/languages
+
 ### Auto Detect Language
 
 Request:
 
 ```javascript
 const res = await fetch("https://libretranslate.com/translate", {
   method: "POST",
```

### Comparing `libretranslate-1.5.6/pyproject.toml` & `libretranslate-1.5.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,16 @@
 [project.urls]
 Homepage = "https://libretranslate.com"
 Source = "https://github.com/LibreTranslate/LibreTranslate"
 Documentation = "https://github.com/LibreTranslate/LibreTranslate"
 Tracker = "https://github.com/LibreTranslate/LibreTranslate/issues"
 History = "https://github.com/LibreTranslate/LibreTranslate/releases"
 
+[tool.hatch.build]
+artifacts = ["*.mo"]
 
 # ENVIRONMENTS AND SCRIPTS
 [tool.hatch.envs.default]
 features = [
     "test",
 ]
 post-install-commands = [
```

### Comparing `libretranslate-1.5.6/PKG-INFO` & `libretranslate-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: libretranslate
-Version: 1.5.6
+Version: 1.5.7
 Summary: Free and Open Source Machine Translation API. Self-hosted, no limits, no ties to proprietary services.
 Project-URL: Homepage, https://libretranslate.com
 Project-URL: Source, https://github.com/LibreTranslate/LibreTranslate
 Project-URL: Documentation, https://github.com/LibreTranslate/LibreTranslate
 Project-URL: Tracker, https://github.com/LibreTranslate/LibreTranslate/issues
 Project-URL: History, https://github.com/LibreTranslate/LibreTranslate/releases
 Author: LibreTranslate Authors
@@ -749,14 +749,16 @@
 
 ```javascript
 {
     "translatedText": "¡Hola!"
 }
 ```
 
+List of language codes: https://libretranslate.com/languages
+
 ### Auto Detect Language
 
 Request:
 
 ```javascript
 const res = await fetch("https://libretranslate.com/translate", {
   method: "POST",
```

