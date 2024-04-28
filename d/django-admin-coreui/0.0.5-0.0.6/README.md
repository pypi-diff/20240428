# Comparing `tmp/django-admin-coreui-0.0.5.tar.gz` & `tmp/django-admin-coreui-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-coreui-0.0.5.tar", last modified: Sun Apr 28 06:50:29 2024, max compression
+gzip compressed data, was "django-admin-coreui-0.0.6.tar", last modified: Sun Apr 28 06:56:06 2024, max compression
```

## Comparing `django-admin-coreui-0.0.5.tar` & `django-admin-coreui-0.0.6.tar`

### file list

```diff
@@ -1,1425 +1,1425 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.228272 django-admin-coreui-0.0.5/
--rw-rw-rw-   0        0        0     1113 2022-12-05 15:06:59.000000 django-admin-coreui-0.0.5/LICENSE.md
--rw-rw-rw-   0        0        0      148 2024-04-28 06:49:04.000000 django-admin-coreui-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     7415 2024-04-28 06:50:29.228199 django-admin-coreui-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6323 2024-04-28 06:13:31.000000 django-admin-coreui-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.247408 django-admin-coreui-0.0.5/admin_coreui/
--rw-rw-rw-   0        0        0        0 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/__init__.py
--rw-rw-rw-   0        0        0       66 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/admin.py
--rw-rw-rw-   0        0        0      174 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/apps.py
--rw-rw-rw-   0        0        0     2623 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/forms.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.249502 django-admin-coreui-0.0.5/admin_coreui/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/models.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.204025 django-admin-coreui-0.0.5/admin_coreui/static/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.252500 django-admin-coreui-0.0.5/admin_coreui/static/assets/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.254498 django-admin-coreui-0.0.5/admin_coreui/static/assets/brand/
--rw-rw-rw-   0        0        0     3305 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/brand/coreui.svg
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.258497 django-admin-coreui-0.0.5/admin_coreui/static/assets/css/
--rw-rw-rw-   0        0        0    10376 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/css/forms.css
--rw-rw-rw-   0        0        0    12542 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/css/widgets.css
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.304175 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/
--rw-rw-rw-   0        0        0    13344 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/android-icon-144x144.png
--rw-rw-rw-   0        0        0    17566 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/android-icon-192x192.png
--rw-rw-rw-   0        0        0     2495 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/android-icon-36x36.png
--rw-rw-rw-   0        0        0     3537 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/android-icon-48x48.png
--rw-rw-rw-   0        0        0     5297 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/android-icon-72x72.png
--rw-rw-rw-   0        0        0     7298 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/android-icon-96x96.png
--rw-rw-rw-   0        0        0     9891 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-114x114.png
--rw-rw-rw-   0        0        0    10620 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-120x120.png
--rw-rw-rw-   0        0        0    13344 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-144x144.png
--rw-rw-rw-   0        0        0    14451 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-152x152.png
--rw-rw-rw-   0        0        0    17458 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-180x180.png
--rw-rw-rw-   0        0        0     4120 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-57x57.png
--rw-rw-rw-   0        0        0     4034 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-60x60.png
--rw-rw-rw-   0        0        0     5297 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-72x72.png
--rw-rw-rw-   0        0        0     5539 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-76x76.png
--rw-rw-rw-   0        0        0    18140 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-precomposed.png
--rw-rw-rw-   0        0        0    18140 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon.png
--rw-rw-rw-   0        0        0      282 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/browserconfig.xml
--rw-rw-rw-   0        0        0     1201 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/favicon-16x16.png
--rw-rw-rw-   0        0        0     2196 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/favicon-32x32.png
--rw-rw-rw-   0        0        0     7298 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/favicon-96x96.png
--rw-rw-rw-   0        0        0     1150 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/favicon.ico
--rw-rw-rw-   0        0        0      849 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/manifest.json
--rw-rw-rw-   0        0        0    13344 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/ms-icon-144x144.png
--rw-rw-rw-   0        0        0    14113 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/ms-icon-150x150.png
--rw-rw-rw-   0        0        0    37803 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/ms-icon-310x310.png
--rw-rw-rw-   0        0        0     5120 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/ms-icon-70x70.png
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:27.539293 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/
--rw-rw-rw-   0        0        0      696 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/3d.svg
--rw-rw-rw-   0        0        0      626 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/4k.svg
--rw-rw-rw-   0        0        0      375 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/account-logout.svg
--rw-rw-rw-   0        0        0      486 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/action-redo.svg
--rw-rw-rw-   0        0        0      755 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/action-undo.svg
--rw-rw-rw-   0        0        0     1226 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/address-book.svg
--rw-rw-rw-   0        0        0     1023 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/airplane-mode-off.svg
--rw-rw-rw-   0        0        0      906 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/airplane-mode.svg
--rw-rw-rw-   0        0        0      479 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/airplay.svg
--rw-rw-rw-   0        0        0      725 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/alarm.svg
--rw-rw-rw-   0        0        0     1089 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/album.svg
--rw-rw-rw-   0        0        0      416 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/align-center.svg
--rw-rw-rw-   0        0        0      432 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/align-left.svg
--rw-rw-rw-   0        0        0      435 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/align-right.svg
--rw-rw-rw-   0        0        0     1309 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/american-football.svg
--rw-rw-rw-   0        0        0     1634 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/android.svg
--rw-rw-rw-   0        0        0      475 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/angular.svg
--rw-rw-rw-   0        0        0     1702 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/aperture.svg
--rw-rw-rw-   0        0        0     1534 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/apple.svg
--rw-rw-rw-   0        0        0     1983 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/applications-settings.svg
--rw-rw-rw-   0        0        0     2289 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/applications.svg
--rw-rw-rw-   0        0        0      287 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-bottom.svg
--rw-rw-rw-   0        0        0      662 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-circle-bottom.svg
--rw-rw-rw-   0        0        0      660 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-circle-left.svg
--rw-rw-rw-   0        0        0      664 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-circle-right.svg
--rw-rw-rw-   0        0        0      656 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-circle-top.svg
--rw-rw-rw-   0        0        0      282 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-left.svg
--rw-rw-rw-   0        0        0      286 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-right.svg
--rw-rw-rw-   0        0        0      336 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-thick-bottom.svg
--rw-rw-rw-   0        0        0      383 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-thick-from-bottom.svg
--rw-rw-rw-   0        0        0      376 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-thick-from-left.svg
--rw-rw-rw-   0        0        0      390 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-thick-from-right.svg
--rw-rw-rw-   0        0        0      387 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-thick-from-top.svg
--rw-rw-rw-   0        0        0      335 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-thick-left.svg
--rw-rw-rw-   0        0        0      339 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-thick-right.svg
--rw-rw-rw-   0        0        0      376 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-thick-to-bottom.svg
--rw-rw-rw-   0        0        0      382 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-thick-to-left.svg
--rw-rw-rw-   0        0        0      372 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-thick-to-right.svg
--rw-rw-rw-   0        0        0      372 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-thick-to-top.svg
--rw-rw-rw-   0        0        0      341 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-thick-top.svg
--rw-rw-rw-   0        0        0      284 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-top.svg
--rw-rw-rw-   0        0        0     1506 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/assistive-listening-system.svg
--rw-rw-rw-   0        0        0      755 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/asterisk-circle.svg
--rw-rw-rw-   0        0        0      405 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/asterisk.svg
--rw-rw-rw-   0        0        0     1064 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/at.svg
--rw-rw-rw-   0        0        0      763 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/audio-description.svg
--rw-rw-rw-   0        0        0      460 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/audio-spectrum.svg
--rw-rw-rw-   0        0        0     1428 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/audio.svg
--rw-rw-rw-   0        0        0      716 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/av-timer.svg
--rw-rw-rw-   0        0        0      915 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/badge.svg
--rw-rw-rw-   0        0        0     1373 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/balance-scale.svg
--rw-rw-rw-   0        0        0      764 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/ban.svg
--rw-rw-rw-   0        0        0      646 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bank.svg
--rw-rw-rw-   0        0        0      688 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bar-chart.svg
--rw-rw-rw-   0        0        0      659 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/barcode.svg
--rw-rw-rw-   0        0        0     1488 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/baseball.svg
--rw-rw-rw-   0        0        0      602 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/basket.svg
--rw-rw-rw-   0        0        0     1561 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/basketball.svg
--rw-rw-rw-   0        0        0     1341 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bath.svg
--rw-rw-rw-   0        0        0      530 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/battery-0.svg
--rw-rw-rw-   0        0        0      684 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/battery-3.svg
--rw-rw-rw-   0        0        0      790 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/battery-5.svg
--rw-rw-rw-   0        0        0      647 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/battery-alert.svg
--rw-rw-rw-   0        0        0      611 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/battery-slash.svg
--rw-rw-rw-   0        0        0     1061 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/beach-access.svg
--rw-rw-rw-   0        0        0      702 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/beaker.svg
--rw-rw-rw-   0        0        0      522 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bed.svg
--rw-rw-rw-   0        0        0      878 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bell.svg
--rw-rw-rw-   0        0        0     1172 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bike.svg
--rw-rw-rw-   0        0        0     1676 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/birthday-cake.svg
--rw-rw-rw-   0        0        0      793 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/blind.svg
--rw-rw-rw-   0        0        0      398 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bluetooth.svg
--rw-rw-rw-   0        0        0     3490 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/blur-circular.svg
--rw-rw-rw-   0        0        0     1893 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/blur-linear.svg
--rw-rw-rw-   0        0        0     2628 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/blur.svg
--rw-rw-rw-   0        0        0      724 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/boat-alt.svg
--rw-rw-rw-   0        0        0      633 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bold.svg
--rw-rw-rw-   0        0        0      327 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bolt.svg
--rw-rw-rw-   0        0        0      692 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/book.svg
--rw-rw-rw-   0        0        0      302 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bookmark.svg
--rw-rw-rw-   0        0        0      931 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bootstrap.svg
--rw-rw-rw-   0        0        0      485 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-all.svg
--rw-rw-rw-   0        0        0     1714 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-bottom.svg
--rw-rw-rw-   0        0        0     2042 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-clear.svg
--rw-rw-rw-   0        0        0     1689 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-horizontal.svg
--rw-rw-rw-   0        0        0     1377 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-inner.svg
--rw-rw-rw-   0        0        0     1722 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-left.svg
--rw-rw-rw-   0        0        0      934 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-outer.svg
--rw-rw-rw-   0        0        0     1713 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-right.svg
--rw-rw-rw-   0        0        0      881 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-style.svg
--rw-rw-rw-   0        0        0     1717 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-top.svg
--rw-rw-rw-   0        0        0     1691 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-vertical.svg
--rw-rw-rw-   0        0        0     1751 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bowling.svg
--rw-rw-rw-   0        0        0     5934 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/braille.svg
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.452977 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/
--rw-rw-rw-   0        0        0     1245 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/500px.svg
--rw-rw-rw-   0        0        0      775 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/accessible-icon.svg
--rw-rw-rw-   0        0        0      852 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/accusoft.svg
--rw-rw-rw-   0        0        0     1391 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/acquisitions-incorporated.svg
--rw-rw-rw-   0        0        0      267 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/adn.svg
--rw-rw-rw-   0        0        0      187 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/adobe.svg
--rw-rw-rw-   0        0        0     1306 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/adversal.svg
--rw-rw-rw-   0        0        0      404 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/affiliatetheme.svg
--rw-rw-rw-   0        0        0      849 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/airbnb.svg
--rw-rw-rw-   0        0        0      907 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/algolia.svg
--rw-rw-rw-   0        0        0      745 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/alipay.svg
--rw-rw-rw-   0        0        0     3466 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/amazon-pay.svg
--rw-rw-rw-   0        0        0      720 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/amazon.svg
--rw-rw-rw-   0        0        0      605 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/amilia.svg
--rw-rw-rw-   0        0        0      907 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/android.svg
--rw-rw-rw-   0        0        0     1382 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/angellist.svg
--rw-rw-rw-   0        0        0     1951 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/angrycreative.svg
--rw-rw-rw-   0        0        0      239 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/angular.svg
--rw-rw-rw-   0        0        0      726 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/app-store-ios.svg
--rw-rw-rw-   0        0        0      858 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/app-store.svg
--rw-rw-rw-   0        0        0     1729 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/apper.svg
--rw-rw-rw-   0        0        0     1190 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/apple-pay.svg
--rw-rw-rw-   0        0        0      515 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/apple.svg
--rw-rw-rw-   0        0        0      273 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/artstation.svg
--rw-rw-rw-   0        0        0      764 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/asymmetrik.svg
--rw-rw-rw-   0        0        0      366 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/atlassian.svg
--rw-rw-rw-   0        0        0      574 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/audible.svg
--rw-rw-rw-   0        0        0      279 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/autoprefixer.svg
--rw-rw-rw-   0        0        0      571 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/avianex.svg
--rw-rw-rw-   0        0        0     2177 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/aviato.svg
--rw-rw-rw-   0        0        0     2310 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/aws.svg
--rw-rw-rw-   0        0        0      192 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/bandcamp.svg
--rw-rw-rw-   0        0        0     2573 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/battle-net.svg
--rw-rw-rw-   0        0        0      783 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/behance-square.svg
--rw-rw-rw-   0        0        0      684 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/behance.svg
--rw-rw-rw-   0        0        0      485 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/bimobject.svg
--rw-rw-rw-   0        0        0      306 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/bitbucket.svg
--rw-rw-rw-   0        0        0     1165 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/bitcoin.svg
--rw-rw-rw-   0        0        0      759 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/bity.svg
--rw-rw-rw-   0        0        0      177 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/black-tie.svg
--rw-rw-rw-   0        0        0      676 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/blackberry.svg
--rw-rw-rw-   0        0        0      900 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/blogger-b.svg
--rw-rw-rw-   0        0        0     1199 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/blogger.svg
--rw-rw-rw-   0        0        0      371 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/bluetooth-b.svg
--rw-rw-rw-   0        0        0      370 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/bluetooth.svg
--rw-rw-rw-   0        0        0      606 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/bootstrap.svg
--rw-rw-rw-   0        0        0   442536 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/brands-symbol-defs.svg
--rw-rw-rw-   0        0        0      758 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/btc.svg
--rw-rw-rw-   0        0        0      719 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/buffer.svg
--rw-rw-rw-   0        0        0      474 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/buromobelexperte.svg
--rw-rw-rw-   0        0        0      297 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/buysellads.svg
--rw-rw-rw-   0        0        0      866 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/canadian-maple-leaf.svg
--rw-rw-rw-   0        0        0     3428 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-amazon-pay.svg
--rw-rw-rw-   0        0        0     3197 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-amex.svg
--rw-rw-rw-   0        0        0     1285 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-apple-pay.svg
--rw-rw-rw-   0        0        0      600 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-diners-club.svg
--rw-rw-rw-   0        0        0     1237 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-discover.svg
--rw-rw-rw-   0        0        0      779 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-jcb.svg
--rw-rw-rw-   0        0        0     3020 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-mastercard.svg
--rw-rw-rw-   0        0        0     1762 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-paypal.svg
--rw-rw-rw-   0        0        0     1288 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-stripe.svg
--rw-rw-rw-   0        0        0      934 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-visa.svg
--rw-rw-rw-   0        0        0      455 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/centercode.svg
--rw-rw-rw-   0        0        0      913 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/centos.svg
--rw-rw-rw-   0        0        0      577 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/chrome.svg
--rw-rw-rw-   0        0        0      474 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/chromecast.svg
--rw-rw-rw-   0        0        0      631 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cloudscale.svg
--rw-rw-rw-   0        0        0      294 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cloudsmith.svg
--rw-rw-rw-   0        0        0     1362 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cloudversify.svg
--rw-rw-rw-   0        0        0      745 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/codepen.svg
--rw-rw-rw-   0        0        0      537 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/codiepie.svg
--rw-rw-rw-   0        0        0      592 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/confluence.svg
--rw-rw-rw-   0        0        0     3122 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/connectdevelop.svg
--rw-rw-rw-   0        0        0      552 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/contao.svg
--rw-rw-rw-   0        0        0     1431 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cpanel.svg
--rw-rw-rw-   0        0        0      579 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-by.svg
--rw-rw-rw-   0        0        0      824 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-nc-eu.svg
--rw-rw-rw-   0        0        0      582 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-nc-jp.svg
--rw-rw-rw-   0        0        0      742 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-nc.svg
--rw-rw-rw-   0        0        0      386 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-nd.svg
--rw-rw-rw-   0        0        0      618 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-pd-alt.svg
--rw-rw-rw-   0        0        0      658 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-pd.svg
--rw-rw-rw-   0        0        0      648 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-remix.svg
--rw-rw-rw-   0        0        0      586 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-sa.svg
--rw-rw-rw-   0        0        0     1171 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-sampling-plus.svg
--rw-rw-rw-   0        0        0     1235 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-sampling.svg
--rw-rw-rw-   0        0        0      625 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-share.svg
--rw-rw-rw-   0        0        0      664 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-zero.svg
--rw-rw-rw-   0        0        0      962 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons.svg
--rw-rw-rw-   0        0        0     7133 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/critical-role.svg
--rw-rw-rw-   0        0        0      317 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/css3-alt.svg
--rw-rw-rw-   0        0        0      207 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/css3.svg
--rw-rw-rw-   0        0        0      330 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cuttlefish.svg
--rw-rw-rw-   0        0        0     3996 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/d-and-d-beyond.svg
--rw-rw-rw-   0        0        0     4519 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/d-and-d.svg
--rw-rw-rw-   0        0        0      320 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/dashcube.svg
--rw-rw-rw-   0        0        0      546 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/delicious.svg
--rw-rw-rw-   0        0        0      844 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/deploydog.svg
--rw-rw-rw-   0        0        0      687 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/deskpro.svg
--rw-rw-rw-   0        0        0      765 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/dev.svg
--rw-rw-rw-   0        0        0      252 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/deviantart.svg
--rw-rw-rw-   0        0        0      839 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/dhl.svg
--rw-rw-rw-   0        0        0      486 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/diaspora.svg
--rw-rw-rw-   0        0        0      384 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/digg.svg
--rw-rw-rw-   0        0        0      376 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/digital-ocean.svg
--rw-rw-rw-   0        0        0     1218 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/discord.svg
--rw-rw-rw-   0        0        0      343 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/discourse.svg
--rw-rw-rw-   0        0        0      267 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/dochub.svg
--rw-rw-rw-   0        0        0      663 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/docker.svg
--rw-rw-rw-   0        0        0      779 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/draft2digital.svg
--rw-rw-rw-   0        0        0      921 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/dribbble-square.svg
--rw-rw-rw-   0        0        0     1131 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/dribbble.svg
--rw-rw-rw-   0        0        0      310 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/dropbox.svg
--rw-rw-rw-   0        0        0      771 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/drupal.svg
--rw-rw-rw-   0        0        0      260 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/dyalog.svg
--rw-rw-rw-   0        0        0     1927 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/earlybirds.svg
--rw-rw-rw-   0        0        0     1097 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ebay.svg
--rw-rw-rw-   0        0        0      615 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/edge.svg
--rw-rw-rw-   0        0        0      326 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/elementor.svg
--rw-rw-rw-   0        0        0      428 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ello.svg
--rw-rw-rw-   0        0        0     1933 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ember.svg
--rw-rw-rw-   0        0        0     1847 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/empire.svg
--rw-rw-rw-   0        0        0      366 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/envira.svg
--rw-rw-rw-   0        0        0      432 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/erlang.svg
--rw-rw-rw-   0        0        0      175 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ethereum.svg
--rw-rw-rw-   0        0        0      662 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/etsy.svg
--rw-rw-rw-   0        0        0     1009 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/evernote.svg
--rw-rw-rw-   0        0        0      962 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/expeditedssl.svg
--rw-rw-rw-   0        0        0      252 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/facebook-f.svg
--rw-rw-rw-   0        0        0      554 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/facebook-messenger.svg
--rw-rw-rw-   0        0        0      338 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/facebook-square.svg
--rw-rw-rw-   0        0        0      344 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/facebook.svg
--rw-rw-rw-   0        0        0     1139 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fantasy-flight-games.svg
--rw-rw-rw-   0        0        0      819 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fedex.svg
--rw-rw-rw-   0        0        0     2243 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fedora.svg
--rw-rw-rw-   0        0        0      263 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/figma.svg
--rw-rw-rw-   0        0        0     2632 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/firefox.svg
--rw-rw-rw-   0        0        0     1530 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/first-order-alt.svg
--rw-rw-rw-   0        0        0     1242 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/first-order.svg
--rw-rw-rw-   0        0        0      267 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/firstdraft.svg
--rw-rw-rw-   0        0        0      379 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/flickr.svg
--rw-rw-rw-   0        0        0      156 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/flipboard.svg
--rw-rw-rw-   0        0        0      740 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fly.svg
--rw-rw-rw-   0        0        0      814 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/font-awesome-alt.svg
--rw-rw-rw-   0        0        0      657 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/font-awesome-flag.svg
--rw-rw-rw-   0        0        0     2994 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/font-awesome-logo-full.svg
--rw-rw-rw-   0        0        0      699 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/font-awesome.svg
--rw-rw-rw-   0        0        0      614 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fonticons-fi.svg
--rw-rw-rw-   0        0        0      640 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fonticons.svg
--rw-rw-rw-   0        0        0     3691 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fort-awesome-alt.svg
--rw-rw-rw-   0        0        0     1019 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fort-awesome.svg
--rw-rw-rw-   0        0        0      617 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/forumbee.svg
--rw-rw-rw-   0        0        0      623 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/foursquare.svg
--rw-rw-rw-   0        0        0     1312 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/free-code-camp.svg
--rw-rw-rw-   0        0        0      596 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/freebsd.svg
--rw-rw-rw-   0        0        0      339 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fulcrum.svg
--rw-rw-rw-   0        0        0     1603 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/galactic-republic.svg
--rw-rw-rw-   0        0        0     2684 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/galactic-senate.svg
--rw-rw-rw-   0        0        0      424 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/get-pocket.svg
--rw-rw-rw-   0        0        0      410 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/gg-circle.svg
--rw-rw-rw-   0        0        0      341 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/gg.svg
--rw-rw-rw-   0        0        0      538 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/git-alt.svg
--rw-rw-rw-   0        0        0     1216 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/git-square.svg
--rw-rw-rw-   0        0        0     1099 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/git.svg
--rw-rw-rw-   0        0        0      880 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/github-alt.svg
--rw-rw-rw-   0        0        0     1494 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/github-square.svg
--rw-rw-rw-   0        0        0     1384 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/github.svg
--rw-rw-rw-   0        0        0     1354 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/gitkraken.svg
--rw-rw-rw-   0        0        0      354 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/gitlab.svg
--rw-rw-rw-   0        0        0      194 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/gitter.svg
--rw-rw-rw-   0        0        0      758 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/glide-g.svg
--rw-rw-rw-   0        0        0      855 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/glide.svg
--rw-rw-rw-   0        0        0      440 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/gofore.svg
--rw-rw-rw-   0        0        0      723 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/goodreads-g.svg
--rw-rw-rw-   0        0        0      811 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/goodreads.svg
--rw-rw-rw-   0        0        0      217 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/google-drive.svg
--rw-rw-rw-   0        0        0      326 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/google-play.svg
--rw-rw-rw-   0        0        0      557 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/google-plus-g.svg
--rw-rw-rw-   0        0        0      498 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/google-plus-square.svg
--rw-rw-rw-   0        0        0      501 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/google-plus.svg
--rw-rw-rw-   0        0        0      598 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/google-wallet.svg
--rw-rw-rw-   0        0        0      327 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/google.svg
--rw-rw-rw-   0        0        0      333 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/gratipay.svg
--rw-rw-rw-   0        0        0     1628 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/grav.svg
--rw-rw-rw-   0        0        0      690 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/gripfire.svg
--rw-rw-rw-   0        0        0     5490 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/grunt.svg
--rw-rw-rw-   0        0        0     2601 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/gulp.svg
--rw-rw-rw-   0        0        0      346 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hacker-news-square.svg
--rw-rw-rw-   0        0        0      260 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hacker-news.svg
--rw-rw-rw-   0        0        0      843 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hackerrank.svg
--rw-rw-rw-   0        0        0     1445 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hips.svg
--rw-rw-rw-   0        0        0     1062 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hire-a-helper.svg
--rw-rw-rw-   0        0        0     1486 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hooli.svg
--rw-rw-rw-   0        0        0     1094 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hornbill.svg
--rw-rw-rw-   0        0        0      350 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hotjar.svg
--rw-rw-rw-   0        0        0      142 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/houzz.svg
--rw-rw-rw-   0        0        0      279 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/html5.svg
--rw-rw-rw-   0        0        0      832 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hubspot.svg
--rw-rw-rw-   0        0        0      753 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/imdb.svg
--rw-rw-rw-   0        0        0     1002 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/instagram.svg
--rw-rw-rw-   0        0        0      662 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/intercom.svg
--rw-rw-rw-   0        0        0      937 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/internet-explorer.svg
--rw-rw-rw-   0        0        0      683 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/invision.svg
--rw-rw-rw-   0        0        0      703 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ioxhost.svg
--rw-rw-rw-   0        0        0     1265 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/itch-io.svg
--rw-rw-rw-   0        0        0      662 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/itunes-note.svg
--rw-rw-rw-   0        0        0      952 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/itunes.svg
--rw-rw-rw-   0        0        0     1182 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/java.svg
--rw-rw-rw-   0        0        0      736 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/jedi-order.svg
--rw-rw-rw-   0        0        0     4341 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/jenkins.svg
--rw-rw-rw-   0        0        0      299 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/jira.svg
--rw-rw-rw-   0        0        0      877 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/joget.svg
--rw-rw-rw-   0        0        0     1145 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/joomla.svg
--rw-rw-rw-   0        0        0      697 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/js-square.svg
--rw-rw-rw-   0        0        0      611 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/js.svg
--rw-rw-rw-   0        0        0     1903 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/jsfiddle.svg
--rw-rw-rw-   0        0        0      318 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/kaggle.svg
--rw-rw-rw-   0        0        0     1916 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/keybase.svg
--rw-rw-rw-   0        0        0     1519 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/keycdn.svg
--rw-rw-rw-   0        0        0      372 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/kickstarter-k.svg
--rw-rw-rw-   0        0        0      469 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/kickstarter.svg
--rw-rw-rw-   0        0        0      330 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/korvue.svg
--rw-rw-rw-   0        0        0     1122 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/laravel.svg
--rw-rw-rw-   0        0        0      737 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/lastfm-square.svg
--rw-rw-rw-   0        0        0      649 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/lastfm.svg
--rw-rw-rw-   0        0        0     1163 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/leanpub.svg
--rw-rw-rw-   0        0        0     1840 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/less.svg
--rw-rw-rw-   0        0        0     1205 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/line.svg
--rw-rw-rw-   0        0        0      380 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/linkedin-in.svg
--rw-rw-rw-   0        0        0      504 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/linkedin.svg
--rw-rw-rw-   0        0        0     1337 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/linode.svg
--rw-rw-rw-   0        0        0     3568 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/linux.svg
--rw-rw-rw-   0        0        0      675 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/lyft.svg
--rw-rw-rw-   0        0        0      279 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/magento.svg
--rw-rw-rw-   0        0        0     3137 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/mailchimp.svg
--rw-rw-rw-   0        0        0     5988 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/mandalorian.svg
--rw-rw-rw-   0        0        0      359 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/markdown.svg
--rw-rw-rw-   0        0        0      695 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/mastodon.svg
--rw-rw-rw-   0        0        0      300 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/maxcdn.svg
--rw-rw-rw-   0        0        0      896 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/medapps.svg
--rw-rw-rw-   0        0        0      413 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/medium-m.svg
--rw-rw-rw-   0        0        0      416 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/medium.svg
--rw-rw-rw-   0        0        0      836 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/medrt.svg
--rw-rw-rw-   0        0        0     2132 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/meetup.svg
--rw-rw-rw-   0        0        0      429 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/megaport.svg
--rw-rw-rw-   0        0        0      736 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/mendeley.svg
--rw-rw-rw-   0        0        0      187 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/microsoft.svg
--rw-rw-rw-   0        0        0      224 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/mix.svg
--rw-rw-rw-   0        0        0     1375 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/mixcloud.svg
--rw-rw-rw-   0        0        0      437 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/mizuni.svg
--rw-rw-rw-   0        0        0      248 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/modx.svg
--rw-rw-rw-   0        0        0      294 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/monero.svg
--rw-rw-rw-   0        0        0      980 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/napster.svg
--rw-rw-rw-   0        0        0      439 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/neos.svg
--rw-rw-rw-   0        0        0      554 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/nimblr.svg
--rw-rw-rw-   0        0        0     1164 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/node-js.svg
--rw-rw-rw-   0        0        0     3117 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/node.svg
--rw-rw-rw-   0        0        0      254 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/npm.svg
--rw-rw-rw-   0        0        0     1026 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ns8.svg
--rw-rw-rw-   0        0        0     1498 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/nutritionix.svg
--rw-rw-rw-   0        0        0      768 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/odnoklassniki-square.svg
--rw-rw-rw-   0        0        0      663 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/odnoklassniki.svg
--rw-rw-rw-   0        0        0    11219 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/old-republic.svg
--rw-rw-rw-   0        0        0      426 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/opencart.svg
--rw-rw-rw-   0        0        0      334 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/openid.svg
--rw-rw-rw-   0        0        0      494 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/opera.svg
--rw-rw-rw-   0        0        0     4751 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/optin-monster.svg
--rw-rw-rw-   0        0        0      955 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/osi.svg
--rw-rw-rw-   0        0        0      804 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/page4.svg
--rw-rw-rw-   0        0        0      564 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pagelines.svg
--rw-rw-rw-   0        0        0      842 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/palfed.svg
--rw-rw-rw-   0        0        0      237 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/patreon.svg
--rw-rw-rw-   0        0        0      633 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/paypal.svg
--rw-rw-rw-   0        0        0     1202 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/penny-arcade.svg
--rw-rw-rw-   0        0        0      608 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/periscope.svg
--rw-rw-rw-   0        0        0     1028 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/phabricator.svg
--rw-rw-rw-   0        0        0     2492 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/phoenix-framework.svg
--rw-rw-rw-   0        0        0     1597 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/phoenix-squadron.svg
--rw-rw-rw-   0        0        0      852 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/php.svg
--rw-rw-rw-   0        0        0     1672 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pied-piper-alt.svg
--rw-rw-rw-   0        0        0      620 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pied-piper-hat.svg
--rw-rw-rw-   0        0        0      742 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pied-piper-pp.svg
--rw-rw-rw-   0        0        0      363 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pied-piper.svg
--rw-rw-rw-   0        0        0      575 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pinterest-p.svg
--rw-rw-rw-   0        0        0      709 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pinterest-square.svg
--rw-rw-rw-   0        0        0      746 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pinterest.svg
--rw-rw-rw-   0        0        0      674 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/playstation.svg
--rw-rw-rw-   0        0        0      328 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/product-hunt.svg
--rw-rw-rw-   0        0        0      543 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pushed.svg
--rw-rw-rw-   0        0        0      844 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/python.svg
--rw-rw-rw-   0        0        0      647 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/qq.svg
--rw-rw-rw-   0        0        0      410 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/quinscape.svg
--rw-rw-rw-   0        0        0      572 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/quora.svg
--rw-rw-rw-   0        0        0      625 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/r-project.svg
--rw-rw-rw-   0        0        0     3819 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/raspberry-pi.svg
--rw-rw-rw-   0        0        0     1302 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ravelry.svg
--rw-rw-rw-   0        0        0     2908 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/react.svg
--rw-rw-rw-   0        0        0     5488 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/reacteurope.svg
--rw-rw-rw-   0        0        0     1063 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/readme.svg
--rw-rw-rw-   0        0        0      631 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/rebel.svg
--rw-rw-rw-   0        0        0      489 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/red-river.svg
--rw-rw-rw-   0        0        0      926 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/reddit-alien.svg
--rw-rw-rw-   0        0        0     1037 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/reddit-square.svg
--rw-rw-rw-   0        0        0      988 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/reddit.svg
--rw-rw-rw-   0        0        0      643 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/redhat.svg
--rw-rw-rw-   0        0        0      412 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/renren.svg
--rw-rw-rw-   0        0        0     1297 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/replyd.svg
--rw-rw-rw-   0        0        0      812 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/researchgate.svg
--rw-rw-rw-   0        0        0      553 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/resolving.svg
--rw-rw-rw-   0        0        0      443 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/rev.svg
--rw-rw-rw-   0        0        0      938 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/rocketchat.svg
--rw-rw-rw-   0        0        0      343 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/rockrms.svg
--rw-rw-rw-   0        0        0     1346 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/safari.svg
--rw-rw-rw-   0        0        0     4278 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/salesforce.svg
--rw-rw-rw-   0        0        0     3087 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sass.svg
--rw-rw-rw-   0        0        0      864 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/schlix.svg
--rw-rw-rw-   0        0        0      737 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/scribd.svg
--rw-rw-rw-   0        0        0      757 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/searchengin.svg
--rw-rw-rw-   0        0        0      830 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sellcast.svg
--rw-rw-rw-   0        0        0     1210 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sellsy.svg
--rw-rw-rw-   0        0        0      250 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/servicestack.svg
--rw-rw-rw-   0        0        0     1588 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/shirtsinbulk.svg
--rw-rw-rw-   0        0        0      591 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/shopware.svg
--rw-rw-rw-   0        0        0      533 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/simplybuilt.svg
--rw-rw-rw-   0        0        0      357 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sistrix.svg
--rw-rw-rw-   0        0        0      826 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sith.svg
--rw-rw-rw-   0        0        0      410 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sketch.svg
--rw-rw-rw-   0        0        0      739 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/skyatlas.svg
--rw-rw-rw-   0        0        0      785 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/skype.svg
--rw-rw-rw-   0        0        0      771 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/slack-hash.svg
--rw-rw-rw-   0        0        0     1069 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/slack.svg
--rw-rw-rw-   0        0        0      862 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/slideshare.svg
--rw-rw-rw-   0        0        0     1482 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/snapchat-ghost.svg
--rw-rw-rw-   0        0        0     1090 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/snapchat-square.svg
--rw-rw-rw-   0        0        0     1055 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/snapchat.svg
--rw-rw-rw-   0        0        0     2188 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/soundcloud.svg
--rw-rw-rw-   0        0        0      334 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sourcetree.svg
--rw-rw-rw-   0        0        0      635 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/speakap.svg
--rw-rw-rw-   0        0        0      440 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/speaker-deck.svg
--rw-rw-rw-   0        0        0      869 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/spotify.svg
--rw-rw-rw-   0        0        0     1185 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/squarespace.svg
--rw-rw-rw-   0        0        0      300 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/stack-exchange.svg
--rw-rw-rw-   0        0        0      299 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/stack-overflow.svg
--rw-rw-rw-   0        0        0      786 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/stackpath.svg
--rw-rw-rw-   0        0        0      795 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/staylinked.svg
--rw-rw-rw-   0        0        0      829 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/steam-square.svg
--rw-rw-rw-   0        0        0      694 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/steam-symbol.svg
--rw-rw-rw-   0        0        0      812 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/steam.svg
--rw-rw-rw-   0        0        0     1635 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sticker-mule.svg
--rw-rw-rw-   0        0        0      184 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/strava.svg
--rw-rw-rw-   0        0        0      383 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/stripe-s.svg
--rw-rw-rw-   0        0        0     1199 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/stripe.svg
--rw-rw-rw-   0        0        0      567 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/studiovinari.svg
--rw-rw-rw-   0        0        0      587 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/stumbleupon-circle.svg
--rw-rw-rw-   0        0        0      498 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/stumbleupon.svg
--rw-rw-rw-   0        0        0      400 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/superpowers.svg
--rw-rw-rw-   0        0        0     1712 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/supple.svg
--rw-rw-rw-   0        0        0     1289 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/suse.svg
--rw-rw-rw-   0        0        0     1183 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/symfony.svg
--rw-rw-rw-   0        0        0     1075 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/teamspeak.svg
--rw-rw-rw-   0        0        0      320 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/telegram-plane.svg
--rw-rw-rw-   0        0        0      376 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/telegram.svg
--rw-rw-rw-   0        0        0      496 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/tencent-weibo.svg
--rw-rw-rw-   0        0        0     6169 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/the-red-yeti.svg
--rw-rw-rw-   0        0        0      756 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/themeco.svg
--rw-rw-rw-   0        0        0     3279 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/themeisle.svg
--rw-rw-rw-   0        0        0      211 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/think-peaks.svg
--rw-rw-rw-   0        0        0     1378 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/trade-federation.svg
--rw-rw-rw-   0        0        0      484 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/trello.svg
--rw-rw-rw-   0        0        0     2012 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/tripadvisor.svg
--rw-rw-rw-   0        0        0      557 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/tumblr-square.svg
--rw-rw-rw-   0        0        0      445 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/tumblr.svg
--rw-rw-rw-   0        0        0      261 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/twitch.svg
--rw-rw-rw-   0        0        0      671 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/twitter-square.svg
--rw-rw-rw-   0        0        0      871 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/twitter.svg
--rw-rw-rw-   0        0        0      402 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/typo3.svg
--rw-rw-rw-   0        0        0      460 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/uber.svg
--rw-rw-rw-   0        0        0      949 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ubuntu.svg
--rw-rw-rw-   0        0        0      235 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/uikit.svg
--rw-rw-rw-   0        0        0     1048 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/uniregistry.svg
--rw-rw-rw-   0        0        0     1122 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/untappd.svg
--rw-rw-rw-   0        0        0      747 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ups.svg
--rw-rw-rw-   0        0        0      761 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/usb.svg
--rw-rw-rw-   0        0        0      569 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/usps.svg
--rw-rw-rw-   0        0        0     3256 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ussunnah.svg
--rw-rw-rw-   0        0        0      765 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vaadin.svg
--rw-rw-rw-   0        0        0      236 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/viacoin.svg
--rw-rw-rw-   0        0        0      885 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/viadeo-square.svg
--rw-rw-rw-   0        0        0      817 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/viadeo.svg
--rw-rw-rw-   0        0        0     1457 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/viber.svg
--rw-rw-rw-   0        0        0      552 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vimeo-square.svg
--rw-rw-rw-   0        0        0      461 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vimeo-v.svg
--rw-rw-rw-   0        0        0      575 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vimeo.svg
--rw-rw-rw-   0        0        0      501 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vine.svg
--rw-rw-rw-   0        0        0      689 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vk.svg
--rw-rw-rw-   0        0        0      851 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vnv.svg
--rw-rw-rw-   0        0        0      200 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vuejs.svg
--rw-rw-rw-   0        0        0     1053 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/waze.svg
--rw-rw-rw-   0        0        0     1008 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/weebly.svg
--rw-rw-rw-   0        0        0     1000 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/weibo.svg
--rw-rw-rw-   0        0        0      948 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/weixin.svg
--rw-rw-rw-   0        0        0     1028 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/whatsapp-square.svg
--rw-rw-rw-   0        0        0      966 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/whatsapp.svg
--rw-rw-rw-   0        0        0     1258 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/whmcs.svg
--rw-rw-rw-   0        0        0      777 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wikipedia-w.svg
--rw-rw-rw-   0        0        0      215 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/windows.svg
--rw-rw-rw-   0        0        0     1228 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wix.svg
--rw-rw-rw-   0        0        0     8139 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wizards-of-the-coast.svg
--rw-rw-rw-   0        0        0     2472 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wolf-pack-battalion.svg
--rw-rw-rw-   0        0        0      963 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wordpress-simple.svg
--rw-rw-rw-   0        0        0     1104 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wordpress.svg
--rw-rw-rw-   0        0        0      578 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wpbeginner.svg
--rw-rw-rw-   0        0        0      517 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wpexplorer.svg
--rw-rw-rw-   0        0        0      590 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wpforms.svg
--rw-rw-rw-   0        0        0     1212 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wpressr.svg
--rw-rw-rw-   0        0        0      971 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/xbox.svg
--rw-rw-rw-   0        0        0      550 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/xing-square.svg
--rw-rw-rw-   0        0        0      459 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/xing.svg
--rw-rw-rw-   0        0        0      209 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/y-combinator.svg
--rw-rw-rw-   0        0        0      363 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/yahoo.svg
--rw-rw-rw-   0        0        0      695 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/yammer.svg
--rw-rw-rw-   0        0        0      156 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/yandex-international.svg
--rw-rw-rw-   0        0        0      282 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/yandex.svg
--rw-rw-rw-   0        0        0     1412 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/yarn.svg
--rw-rw-rw-   0        0        0      837 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/yelp.svg
--rw-rw-rw-   0        0        0      520 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/yoast.svg
--rw-rw-rw-   0        0        0      526 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/youtube-square.svg
--rw-rw-rw-   0        0        0      550 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/youtube.svg
--rw-rw-rw-   0        0        0     1544 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/zhihu.svg
--rw-rw-rw-   0        0        0      601 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/briefcase.svg
--rw-rw-rw-   0        0        0      999 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brightness.svg
--rw-rw-rw-   0        0        0      449 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/british-pound.svg
--rw-rw-rw-   0        0        0      458 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/browser.svg
--rw-rw-rw-   0        0        0      773 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brush-alt.svg
--rw-rw-rw-   0        0        0     1163 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brush.svg
--rw-rw-rw-   0        0        0     1279 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bug.svg
--rw-rw-rw-   0        0        0      723 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/building.svg
--rw-rw-rw-   0        0        0      469 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bullhorn.svg
--rw-rw-rw-   0        0        0     1307 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/burger.svg
--rw-rw-rw-   0        0        0     1101 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bus-alt.svg
--rw-rw-rw-   0        0        0      839 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/calculator.svg
--rw-rw-rw-   0        0        0      597 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/calendar-check.svg
--rw-rw-rw-   0        0        0     1097 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/calendar.svg
--rw-rw-rw-   0        0        0      862 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/camera-control.svg
--rw-rw-rw-   0        0        0     1018 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/camera-roll.svg
--rw-rw-rw-   0        0        0      867 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/camera.svg
--rw-rw-rw-   0        0        0     1198 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/car-alt.svg
--rw-rw-rw-   0        0        0      278 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/caret-bottom.svg
--rw-rw-rw-   0        0        0      279 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/caret-left.svg
--rw-rw-rw-   0        0        0      270 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/caret-right.svg
--rw-rw-rw-   0        0        0      278 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/caret-top.svg
--rw-rw-rw-   0        0        0      818 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cart.svg
--rw-rw-rw-   0        0        0     1317 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/casino.svg
--rw-rw-rw-   0        0        0      632 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cast.svg
--rw-rw-rw-   0        0        0     1061 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cat.svg
--rw-rw-rw-   0        0        0      928 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/center-focus.svg
--rw-rw-rw-   0        0        0      385 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chart-line.svg
--rw-rw-rw-   0        0        0      966 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chart-pie.svg
--rw-rw-rw-   0        0        0      843 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chart.svg
--rw-rw-rw-   0        0        0     1513 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chat-bubble.svg
--rw-rw-rw-   0        0        0      463 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/check.svg
--rw-rw-rw-   0        0        0      436 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-bottom.svg
--rw-rw-rw-   0        0        0      647 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-circle-down-alt.svg
--rw-rw-rw-   0        0        0      650 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-circle-left-alt.svg
--rw-rw-rw-   0        0        0      651 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-circle-right-alt.svg
--rw-rw-rw-   0        0        0      656 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-circle-up-alt.svg
--rw-rw-rw-   0        0        0      666 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-double-down.svg
--rw-rw-rw-   0        0        0      600 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-double-left.svg
--rw-rw-rw-   0        0        0      641 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-double-right.svg
--rw-rw-rw-   0        0        0      395 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-double-up-alt.svg
--rw-rw-rw-   0        0        0      674 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-double-up.svg
--rw-rw-rw-   0        0        0      402 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-left.svg
--rw-rw-rw-   0        0        0      396 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-right.svg
--rw-rw-rw-   0        0        0      408 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-top.svg
--rw-rw-rw-   0        0        0     1154 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/child-friendly.svg
--rw-rw-rw-   0        0        0     1187 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/child.svg
--rw-rw-rw-   0        0        0      550 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/circle.svg
--rw-rw-rw-   0        0        0      328 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/clear-all.svg
--rw-rw-rw-   0        0        0      577 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/clipboard.svg
--rw-rw-rw-   0        0        0      488 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/clock.svg
--rw-rw-rw-   0        0        0      607 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/clone.svg
--rw-rw-rw-   0        0        0     1287 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/closed-captioning.svg
--rw-rw-rw-   0        0        0      645 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cloud-download.svg
--rw-rw-rw-   0        0        0      933 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cloud-upload.svg
--rw-rw-rw-   0        0        0      819 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cloud.svg
--rw-rw-rw-   0        0        0     1035 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cloudy.svg
--rw-rw-rw-   0        0        0      439 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/code.svg
--rw-rw-rw-   0        0        0      946 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/codepen.svg
--rw-rw-rw-   0        0        0      605 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/coffee.svg
--rw-rw-rw-   0        0        0      869 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/color-border.svg
--rw-rw-rw-   0        0        0     1349 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/color-fill.svg
--rw-rw-rw-   0        0        0     2109 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/color-palette.svg
--rw-rw-rw-   0        0        0      452 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/columns.svg
--rw-rw-rw-   0        0        0      941 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/comment-bubble.svg
--rw-rw-rw-   0        0        0      397 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/comment-square.svg
--rw-rw-rw-   0        0        0      875 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/compass.svg
--rw-rw-rw-   0        0        0      386 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/compress.svg
--rw-rw-rw-   0        0        0      842 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/contact.svg
--rw-rw-rw-   0        0        0     1026 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/contrast.svg
--rw-rw-rw-   0        0        0      383 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/copy.svg
--rw-rw-rw-   0        0        0      936 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/copyright.svg
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.454979 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/coreui/
--rw-rw-rw-   0        0        0   387926 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/coreui/free-symbol-defs.svg
--rw-rw-rw-   0        0        0      846 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/couch.svg
--rw-rw-rw-   0        0        0      521 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/credit-card.svg
--rw-rw-rw-   0        0        0      663 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/crop-rotate.svg
--rw-rw-rw-   0        0        0      603 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/crop.svg
--rw-rw-rw-   0        0        0      855 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cursor-move.svg
--rw-rw-rw-   0        0        0      407 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cursor.svg
--rw-rw-rw-   0        0        0      929 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cut.svg
--rw-rw-rw-   0        0        0      356 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/data-transfer-down.svg
--rw-rw-rw-   0        0        0      349 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/data-transfer-up.svg
--rw-rw-rw-   0        0        0     1418 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/deaf.svg
--rw-rw-rw-   0        0        0      622 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/delete.svg
--rw-rw-rw-   0        0        0      420 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/description.svg
--rw-rw-rw-   0        0        0      633 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/devices.svg
--rw-rw-rw-   0        0        0     2975 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/dialpad.svg
--rw-rw-rw-   0        0        0      411 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/dinner.svg
--rw-rw-rw-   0        0        0      924 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/dog.svg
--rw-rw-rw-   0        0        0      657 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/dollar.svg
--rw-rw-rw-   0        0        0      321 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/door.svg
--rw-rw-rw-   0        0        0      383 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/double-quote-sans-left.svg
--rw-rw-rw-   0        0        0      377 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/double-quote-sans-right.svg
--rw-rw-rw-   0        0        0      367 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/drink-alcohol.svg
--rw-rw-rw-   0        0        0      525 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/drink.svg
--rw-rw-rw-   0        0        0      751 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/drop.svg
--rw-rw-rw-   0        0        0      770 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/drop1.svg
--rw-rw-rw-   0        0        0      359 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/elevator.svg
--rw-rw-rw-   0        0        0      297 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/energy.svg
--rw-rw-rw-   0        0        0      455 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/envelope-closed.svg
--rw-rw-rw-   0        0        0      577 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/envelope-letter.svg
--rw-rw-rw-   0        0        0      503 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/envelope-open.svg
--rw-rw-rw-   0        0        0     1148 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/equalizer.svg
--rw-rw-rw-   0        0        0      523 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/ethernet.svg
--rw-rw-rw-   0        0        0      602 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/euro.svg
--rw-rw-rw-   0        0        0      526 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/excerpt.svg
--rw-rw-rw-   0        0        0      532 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/exit-to-app.svg
--rw-rw-rw-   0        0        0      388 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/expand-down.svg
--rw-rw-rw-   0        0        0      382 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/expand-left.svg
--rw-rw-rw-   0        0        0      396 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/expand-right.svg
--rw-rw-rw-   0        0        0      388 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/expand-up.svg
--rw-rw-rw-   0        0        0      577 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/exposure.svg
--rw-rw-rw-   0        0        0      355 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/external-link.svg
--rw-rw-rw-   0        0        0      924 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/eye.svg
--rw-rw-rw-   0        0        0     1052 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/eyedropper.svg
--rw-rw-rw-   0        0        0      934 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/face-dead.svg
--rw-rw-rw-   0        0        0      880 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/face.svg
--rw-rw-rw-   0        0        0      678 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/facebook.svg
--rw-rw-rw-   0        0        0      729 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fastfood.svg
--rw-rw-rw-   0        0        0      899 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fax.svg
--rw-rw-rw-   0        0        0      606 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/featured-playlist.svg
--rw-rw-rw-   0        0        0      305 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/file.svg
--rw-rw-rw-   0        0        0      532 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/filter-frames.svg
--rw-rw-rw-   0        0        0      809 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/filter-photo.svg
--rw-rw-rw-   0        0        0      331 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/filter.svg
--rw-rw-rw-   0        0        0      731 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/find-in-page.svg
--rw-rw-rw-   0        0        0     2035 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fingerprint.svg
--rw-rw-rw-   0        0        0     1623 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fire.svg
--rw-rw-rw-   0        0        0      312 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/flag-alt.svg
--rw-rw-rw-   0        0        0     1190 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/flight-takeoff.svg
--rw-rw-rw-   0        0        0     1606 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/flip-to-back.svg
--rw-rw-rw-   0        0        0     1088 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/flip-to-front.svg
--rw-rw-rw-   0        0        0      926 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/flip.svg
--rw-rw-rw-   0        0        0     2522 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/flower.svg
--rw-rw-rw-   0        0        0      719 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/folder-open.svg
--rw-rw-rw-   0        0        0      499 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/folder.svg
--rw-rw-rw-   0        0        0      367 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/font.svg
--rw-rw-rw-   0        0        0     1357 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/football.svg
--rw-rw-rw-   0        0        0     1163 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fork.svg
--rw-rw-rw-   0        0        0      582 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fridge.svg
--rw-rw-rw-   0        0        0      810 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/frown.svg
--rw-rw-rw-   0        0        0      370 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fullscreen-exit.svg
--rw-rw-rw-   0        0        0      357 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fullscreen.svg
--rw-rw-rw-   0        0        0      313 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/functions-alt.svg
--rw-rw-rw-   0        0        0      896 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/functions.svg
--rw-rw-rw-   0        0        0     1230 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/gamepad.svg
--rw-rw-rw-   0        0        0     1067 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/garage.svg
--rw-rw-rw-   0        0        0      504 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/gem.svg
--rw-rw-rw-   0        0        0      445 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/gif.svg
--rw-rw-rw-   0        0        0      934 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/gift.svg
--rw-rw-rw-   0        0        0     1125 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/git.svg
--rw-rw-rw-   0        0        0     2036 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/github-circle.svg
--rw-rw-rw-   0        0        0     1908 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/github.svg
--rw-rw-rw-   0        0        0     1192 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/gitlab.svg
--rw-rw-rw-   0        0        0     1249 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/globe-alt.svg
--rw-rw-rw-   0        0        0     1061 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/golf-alt.svg
--rw-rw-rw-   0        0        0     1034 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/golf.svg
--rw-rw-rw-   0        0        0      948 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/gradient.svg
--rw-rw-rw-   0        0        0     2581 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/grain.svg
--rw-rw-rw-   0        0        0     1510 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/graph.svg
--rw-rw-rw-   0        0        0      726 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/grid-slash.svg
--rw-rw-rw-   0        0        0      651 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/grid.svg
--rw-rw-rw-   0        0        0      809 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hand-point-down.svg
--rw-rw-rw-   0        0        0      841 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hand-point-left.svg
--rw-rw-rw-   0        0        0      824 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hand-point-right.svg
--rw-rw-rw-   0        0        0      811 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hand-point-up.svg
--rw-rw-rw-   0        0        0      693 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hd.svg
--rw-rw-rw-   0        0        0      582 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hdr.svg
--rw-rw-rw-   0        0        0      389 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/header.svg
--rw-rw-rw-   0        0        0      730 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/headphones.svg
--rw-rw-rw-   0        0        0     1751 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/healing.svg
--rw-rw-rw-   0        0        0      909 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/heart.svg
--rw-rw-rw-   0        0        0      849 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/highlighter.svg
--rw-rw-rw-   0        0        0      520 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/highligt.svg
--rw-rw-rw-   0        0        0      643 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/history.svg
--rw-rw-rw-   0        0        0      533 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/home.svg
--rw-rw-rw-   0        0        0      603 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hospital.svg
--rw-rw-rw-   0        0        0     1763 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hot-tub.svg
--rw-rw-rw-   0        0        0      561 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/house.svg
--rw-rw-rw-   0        0        0      593 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/https.svg
--rw-rw-rw-   0        0        0      511 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/image-broken.svg
--rw-rw-rw-   0        0        0      487 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/image-plus.svg
--rw-rw-rw-   0        0        0      397 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/image1.svg
--rw-rw-rw-   0        0        0      322 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/inbox.svg
--rw-rw-rw-   0        0        0      541 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/indent-decrease.svg
--rw-rw-rw-   0        0        0      538 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/indent-increase.svg
--rw-rw-rw-   0        0        0      794 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/industry-slash.svg
--rw-rw-rw-   0        0        0      794 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/industry.svg
--rw-rw-rw-   0        0        0      877 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/infinity.svg
--rw-rw-rw-   0        0        0      880 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/info.svg
--rw-rw-rw-   0        0        0      447 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/input-hdmi.svg
--rw-rw-rw-   0        0        0      362 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/input-power.svg
--rw-rw-rw-   0        0        0      536 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/input.svg
--rw-rw-rw-   0        0        0     1012 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/instagram.svg
--rw-rw-rw-   0        0        0      568 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/institution.svg
--rw-rw-rw-   0        0        0      351 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/italic.svg
--rw-rw-rw-   0        0        0      423 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/justify-center.svg
--rw-rw-rw-   0        0        0      422 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/justify-left.svg
--rw-rw-rw-   0        0        0      423 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/justify-right.svg
--rw-rw-rw-   0        0        0     1151 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/keyboard.svg
--rw-rw-rw-   0        0        0      838 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/lan.svg
--rw-rw-rw-   0        0        0      998 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/language.svg
--rw-rw-rw-   0        0        0      450 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/laptop.svg
--rw-rw-rw-   0        0        0      895 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/layers.svg
--rw-rw-rw-   0        0        0      884 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/leaf.svg
--rw-rw-rw-   0        0        0     1769 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/lemon.svg
--rw-rw-rw-   0        0        0      301 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/level-down.svg
--rw-rw-rw-   0        0        0      298 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/level-up.svg
--rw-rw-rw-   0        0        0      699 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/library-add.svg
--rw-rw-rw-   0        0        0      578 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/library.svg
--rw-rw-rw-   0        0        0     1247 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/life-ring.svg
--rw-rw-rw-   0        0        0      825 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/lightbulb.svg
--rw-rw-rw-   0        0        0      557 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/line-spacing.svg
--rw-rw-rw-   0        0        0     1961 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/line-style.svg
--rw-rw-rw-   0        0        0      442 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/line-weight.svg
--rw-rw-rw-   0        0        0      573 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/link-alt.svg
--rw-rw-rw-   0        0        0      977 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/link-broken.svg
--rw-rw-rw-   0        0        0      842 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/link.svg
--rw-rw-rw-   0        0        0      988 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/linkedin.svg
--rw-rw-rw-   0        0        0      369 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/list-filter.svg
--rw-rw-rw-   0        0        0      704 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/list-high-priority.svg
--rw-rw-rw-   0        0        0      700 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/list-low-priority.svg
--rw-rw-rw-   0        0        0      589 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/list-numbered.svg
--rw-rw-rw-   0        0        0      701 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/list-rich.svg
--rw-rw-rw-   0        0        0     1040 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/list.svg
--rw-rw-rw-   0        0        0      902 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/location-pin.svg
--rw-rw-rw-   0        0        0      461 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/lock-locked.svg
--rw-rw-rw-   0        0        0      503 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/lock-unlocked.svg
--rw-rw-rw-   0        0        0     1802 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/locomotive.svg
--rw-rw-rw-   0        0        0      653 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/loop-1.svg
--rw-rw-rw-   0        0        0      693 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/loop-circular.svg
--rw-rw-rw-   0        0        0      554 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/loop.svg
--rw-rw-rw-   0        0        0     1171 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/low-vision.svg
--rw-rw-rw-   0        0        0      851 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/magnifying-glass.svg
--rw-rw-rw-   0        0        0      657 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/map.svg
--rw-rw-rw-   0        0        0      699 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-eject.svg
--rw-rw-rw-   0        0        0      598 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-pause.svg
--rw-rw-rw-   0        0        0      506 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-play.svg
--rw-rw-rw-   0        0        0      421 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-record.svg
--rw-rw-rw-   0        0        0      728 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-skip-backward.svg
--rw-rw-rw-   0        0        0      711 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-skip-forward.svg
--rw-rw-rw-   0        0        0      633 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-step-backward.svg
--rw-rw-rw-   0        0        0      557 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-step-forward.svg
--rw-rw-rw-   0        0        0      393 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-stop.svg
--rw-rw-rw-   0        0        0      352 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/medical-cross.svg
--rw-rw-rw-   0        0        0      685 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/meh.svg
--rw-rw-rw-   0        0        0      478 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/memory.svg
--rw-rw-rw-   0        0        0      313 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/menu.svg
--rw-rw-rw-   0        0        0      600 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/microphone.svg
--rw-rw-rw-   0        0        0      218 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/minus.svg
--rw-rw-rw-   0        0        0      437 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mobile-landscape.svg
--rw-rw-rw-   0        0        0      502 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mobile.svg
--rw-rw-rw-   0        0        0      660 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/money.svg
--rw-rw-rw-   0        0        0      507 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/monitor.svg
--rw-rw-rw-   0        0        0      745 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mood-bad.svg
--rw-rw-rw-   0        0        0      742 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mood-good.svg
--rw-rw-rw-   0        0        0      783 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mood-very-bad.svg
--rw-rw-rw-   0        0        0      832 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mood-very-good.svg
--rw-rw-rw-   0        0        0     1209 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/moon.svg
--rw-rw-rw-   0        0        0      739 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mouse.svg
--rw-rw-rw-   0        0        0     1948 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mouth-slash.svg
--rw-rw-rw-   0        0        0      539 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/move.svg
--rw-rw-rw-   0        0        0      680 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/movie.svg
--rw-rw-rw-   0        0        0      840 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mug-tea.svg
--rw-rw-rw-   0        0        0      725 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mug.svg
--rw-rw-rw-   0        0        0      553 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/music-note.svg
--rw-rw-rw-   0        0        0      753 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/newspaper.svg
--rw-rw-rw-   0        0        0      389 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/notes.svg
--rw-rw-rw-   0        0        0      601 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/object-group.svg
--rw-rw-rw-   0        0        0      703 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/object-ungroup.svg
--rw-rw-rw-   0        0        0     2037 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/opacity.svg
--rw-rw-rw-   0        0        0      870 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/options-horizontal.svg
--rw-rw-rw-   0        0        0      864 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/options.svg
--rw-rw-rw-   0        0        0     1203 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/paint-bucket.svg
--rw-rw-rw-   0        0        0      678 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/paint.svg
--rw-rw-rw-   0        0        0      507 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/paper-plane.svg
--rw-rw-rw-   0        0        0      945 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/paperclip.svg
--rw-rw-rw-   0        0        0      355 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/paragraph.svg
--rw-rw-rw-   0        0        0     3241 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/paw.svg
--rw-rw-rw-   0        0        0     1072 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pen-alt.svg
--rw-rw-rw-   0        0        0     1159 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pen-nib.svg
--rw-rw-rw-   0        0        0      749 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pencil.svg
--rw-rw-rw-   0        0        0     1520 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/people.svg
--rw-rw-rw-   0        0        0      698 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/phone.svg
--rw-rw-rw-   0        0        0     1266 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pin.svg
--rw-rw-rw-   0        0        0     1457 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pizza.svg
--rw-rw-rw-   0        0        0      389 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/playlist-add.svg
--rw-rw-rw-   0        0        0      266 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/plus.svg
--rw-rw-rw-   0        0        0      498 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/polymer.svg
--rw-rw-rw-   0        0        0     2383 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pool.svg
--rw-rw-rw-   0        0        0      509 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/power-standby.svg
--rw-rw-rw-   0        0        0      734 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pregnant.svg
--rw-rw-rw-   0        0        0      615 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/print.svg
--rw-rw-rw-   0        0        0     1426 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/puzzle.svg
--rw-rw-rw-   0        0        0      999 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/qr-code.svg
--rw-rw-rw-   0        0        0     1127 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/rain.svg
--rw-rw-rw-   0        0        0     3362 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/react.svg
--rw-rw-rw-   0        0        0      395 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/rectangle.svg
--rw-rw-rw-   0        0        0     1682 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/reddit.svg
--rw-rw-rw-   0        0        0      895 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/registered.svg
--rw-rw-rw-   0        0        0      464 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/reload.svg
--rw-rw-rw-   0        0        0      426 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/resize-both.svg
--rw-rw-rw-   0        0        0      398 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/resize-height.svg
--rw-rw-rw-   0        0        0      392 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/resize-width.svg
--rw-rw-rw-   0        0        0      618 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/restaurant.svg
--rw-rw-rw-   0        0        0      389 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/room.svg
--rw-rw-rw-   0        0        0      894 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/rowing.svg
--rw-rw-rw-   0        0        0      958 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/rss.svg
--rw-rw-rw-   0        0        0     1038 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/running.svg
--rw-rw-rw-   0        0        0      605 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/satelite.svg
--rw-rw-rw-   0        0        0      848 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/save.svg
--rw-rw-rw-   0        0        0      422 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/school.svg
--rw-rw-rw-   0        0        0      457 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/screen-desktop.svg
--rw-rw-rw-   0        0        0      509 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/screen-smartphone.svg
--rw-rw-rw-   0        0        0      756 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/scrubber.svg
--rw-rw-rw-   0        0        0     2637 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/settings.svg
--rw-rw-rw-   0        0        0      759 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/share-all.svg
--rw-rw-rw-   0        0        0     1248 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/share-alt.svg
--rw-rw-rw-   0        0        0      783 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/share-boxed.svg
--rw-rw-rw-   0        0        0      666 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/share.svg
--rw-rw-rw-   0        0        0      952 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/shield-alt.svg
--rw-rw-rw-   0        0        0      336 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/short-text.svg
--rw-rw-rw-   0        0        0     1423 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/shower.svg
--rw-rw-rw-   0        0        0     1927 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sign-language.svg
--rw-rw-rw-   0        0        0      275 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/signal-cellular-0.svg
--rw-rw-rw-   0        0        0      401 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/signal-cellular-3.svg
--rw-rw-rw-   0        0        0      447 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/signal-cellular-4.svg
--rw-rw-rw-   0        0        0      574 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sim.svg
--rw-rw-rw-   0        0        0     1156 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sitemap.svg
--rw-rw-rw-   0        0        0     2021 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/skype.svg
--rw-rw-rw-   0        0        0      948 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/smile-plus.svg
--rw-rw-rw-   0        0        0      943 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/smile.svg
--rw-rw-rw-   0        0        0     1284 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/smoke-free.svg
--rw-rw-rw-   0        0        0     1199 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/smoking-room.svg
--rw-rw-rw-   0        0        0      727 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/snowflake.svg
--rw-rw-rw-   0        0        0      537 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sort-alpha-down.svg
--rw-rw-rw-   0        0        0      531 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sort-alpha-up.svg
--rw-rw-rw-   0        0        0      521 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sort-ascending.svg
--rw-rw-rw-   0        0        0      523 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sort-descending.svg
--rw-rw-rw-   0        0        0      914 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sort-numeric-down.svg
--rw-rw-rw-   0        0        0      905 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sort-numeric-up.svg
--rw-rw-rw-   0        0        0      924 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/spa.svg
--rw-rw-rw-   0        0        0      236 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/space-bar.svg
--rw-rw-rw-   0        0        0      864 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/speaker.svg
--rw-rw-rw-   0        0        0      582 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/speech.svg
--rw-rw-rw-   0        0        0     1007 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/speedometer.svg
--rw-rw-rw-   0        0        0     1513 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/spotify.svg
--rw-rw-rw-   0        0        0      891 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/spreadsheet.svg
--rw-rw-rw-   0        0        0      402 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/square.svg
--rw-rw-rw-   0        0        0      632 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/stackoverflow.svg
--rw-rw-rw-   0        0        0      763 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/star-half.svg
--rw-rw-rw-   0        0        0     1385 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/star.svg
--rw-rw-rw-   0        0        0      444 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/storage.svg
--rw-rw-rw-   0        0        0      324 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/stream.svg
--rw-rw-rw-   0        0        0      929 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sun.svg
--rw-rw-rw-   0        0        0      427 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/swap-horizontal.svg
--rw-rw-rw-   0        0        0      420 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/swap-vertical.svg
--rw-rw-rw-   0        0        0     3156 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/swimming.svg
--rw-rw-rw-   0        0        0      672 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sync.svg
--rw-rw-rw-   0        0        0      486 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/tablet.svg
--rw-rw-rw-   0        0        0      980 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/tag.svg
--rw-rw-rw-   0        0        0     1467 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/tags.svg
--rw-rw-rw-   0        0        0      519 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/task.svg
--rw-rw-rw-   0        0        0      654 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/taxi.svg
--rw-rw-rw-   0        0        0     1168 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/tennis-ball.svg
--rw-rw-rw-   0        0        0     1726 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/tennis.svg
--rw-rw-rw-   0        0        0      560 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/terminal.svg
--rw-rw-rw-   0        0        0      394 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/terrain.svg
--rw-rw-rw-   0        0        0      633 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/text-shapes.svg
--rw-rw-rw-   0        0        0      392 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/text-size.svg
--rw-rw-rw-   0        0        0      347 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/text-square.svg
--rw-rw-rw-   0        0        0      910 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/text-strike.svg
--rw-rw-rw-   0        0        0      283 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/text.svg
--rw-rw-rw-   0        0        0     1339 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/thumb-down.svg
--rw-rw-rw-   0        0        0     1305 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/thumb-up.svg
--rw-rw-rw-   0        0        0      630 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/toggle-off.svg
--rw-rw-rw-   0        0        0      676 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/toilet.svg
--rw-rw-rw-   0        0        0     1064 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/touch-app.svg
--rw-rw-rw-   0        0        0      396 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/trademark.svg
--rw-rw-rw-   0        0        0      417 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/transfer.svg
--rw-rw-rw-   0        0        0      861 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/translate.svg
--rw-rw-rw-   0        0        0      684 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/trash.svg
--rw-rw-rw-   0        0        0      490 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/triangle.svg
--rw-rw-rw-   0        0        0     1125 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/truck.svg
--rw-rw-rw-   0        0        0      511 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/tv.svg
--rw-rw-rw-   0        0        0     1289 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/twitter.svg
--rw-rw-rw-   0        0        0      531 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/underline.svg
--rw-rw-rw-   0        0        0     1157 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/user-female.svg
--rw-rw-rw-   0        0        0      850 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/user-follow.svg
--rw-rw-rw-   0        0        0      970 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/user-unfollow.svg
--rw-rw-rw-   0        0        0      897 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/user.svg
--rw-rw-rw-   0        0        0     1691 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/vector.svg
--rw-rw-rw-   0        0        0      360 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/vertical-align-bottom.svg
--rw-rw-rw-   0        0        0      444 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/vertical-align-bottom1.svg
--rw-rw-rw-   0        0        0      480 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/vertical-align-center.svg
--rw-rw-rw-   0        0        0      593 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/vertical-align-center1.svg
--rw-rw-rw-   0        0        0      351 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/vertical-align-top.svg
--rw-rw-rw-   0        0        0      423 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/vertical-align-top1.svg
--rw-rw-rw-   0        0        0      343 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/video.svg
--rw-rw-rw-   0        0        0      278 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/view-column.svg
--rw-rw-rw-   0        0        0      366 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/view-module.svg
--rw-rw-rw-   0        0        0      321 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/view-quilt.svg
--rw-rw-rw-   0        0        0      264 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/view-stream.svg
--rw-rw-rw-   0        0        0     1333 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/voice-over-record.svg
--rw-rw-rw-   0        0        0      647 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/volume-high.svg
--rw-rw-rw-   0        0        0      468 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/volume-low.svg
--rw-rw-rw-   0        0        0      491 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/volume-off.svg
--rw-rw-rw-   0        0        0      396 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/vue.svg
--rw-rw-rw-   0        0        0      647 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/walk.svg
--rw-rw-rw-   0        0        0      691 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wallet.svg
--rw-rw-rw-   0        0        0      610 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wallpaper.svg
--rw-rw-rw-   0        0        0      386 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/warning.svg
--rw-rw-rw-   0        0        0      770 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/watch.svg
--rw-rw-rw-   0        0        0     1318 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wc.svg
--rw-rw-rw-   0        0        0      674 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/weightlifitng.svg
--rw-rw-rw-   0        0        0      884 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wheelchair.svg
--rw-rw-rw-   0        0        0      512 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wifi-signal-0.svg
--rw-rw-rw-   0        0        0      681 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wifi-signal-1.svg
--rw-rw-rw-   0        0        0      765 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wifi-signal-2.svg
--rw-rw-rw-   0        0        0      781 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wifi-signal-4.svg
--rw-rw-rw-   0        0        0      753 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wifi-signal-off.svg
--rw-rw-rw-   0        0        0      454 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/window-maximize.svg
--rw-rw-rw-   0        0        0      222 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/window-minimize.svg
--rw-rw-rw-   0        0        0      650 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/window-restore.svg
--rw-rw-rw-   0        0        0      406 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/window.svg
--rw-rw-rw-   0        0        0      515 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wrap-text.svg
--rw-rw-rw-   0        0        0      687 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/x-circle.svg
--rw-rw-rw-   0        0        0      322 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/x.svg
--rw-rw-rw-   0        0        0      367 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/yen.svg
--rw-rw-rw-   0        0        0      939 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/zoom-in.svg
--rw-rw-rw-   0        0        0      892 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/zoom-out.svg
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.472775 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.488292 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/
--rw-rw-rw-   0        0        0    13887 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/1.jpg
--rw-rw-rw-   0        0        0    12870 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/2.jpg
--rw-rw-rw-   0        0        0    13528 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/3.jpg
--rw-rw-rw-   0        0        0    13725 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/4.jpg
--rw-rw-rw-   0        0        0    12666 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/5.jpg
--rw-rw-rw-   0        0        0    11918 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/6.jpg
--rw-rw-rw-   0        0        0    14285 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/7.jpg
--rw-rw-rw-   0        0        0    15146 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/8.jpg
--rw-rw-rw-   0        0        0    12451 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/9.jpg
--rw-rw-rw-   0        0        0   362060 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/background-pro-yellow.jpg
--rw-rw-rw-   0        0        0   319788 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/background-pro.jpg
--rw-rw-rw-   0        0        0   290033 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/full.jpg
--rw-rw-rw-   0        0        0     1095 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/icon-calendar.svg
--rw-rw-rw-   0        0        0      686 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/icon-clock.svg
--rw-rw-rw-   0        0        0      658 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/icon-unknown-alt.svg
--rw-rw-rw-   0        0        0      658 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/icon-unknown.svg
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.489364 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/icons/
--rw-rw-rw-   0        0        0     1040 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/icons/add.svg
--rw-rw-rw-   0        0        0      461 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/search.svg
--rw-rw-rw-   0        0        0     3325 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/img/selector-icons.svg
--rw-rw-rw-   0        0        0   435188 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/package-lock.json
--rw-rw-rw-   0        0        0     5309 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/assets/package.json
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.513704 django-admin-coreui-0.0.5/admin_coreui/static/css/
--rw-rw-rw-   0        0        0     1324 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/ads.css
--rw-rw-rw-   0        0        0    16388 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/ads.css.map
--rw-rw-rw-   0        0        0     1099 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/ads.min.css
--rw-rw-rw-   0        0        0    15001 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/ads.min.css.map
--rw-rw-rw-   0        0        0     1924 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/examples.css
--rw-rw-rw-   0        0        0     9564 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/examples.css.map
--rw-rw-rw-   0        0        0     1437 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/examples.min.css
--rw-rw-rw-   0        0        0     9482 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/examples.min.css.map
--rw-rw-rw-   0        0        0    22248 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/icons.css
--rw-rw-rw-   0        0        0   361904 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/style.css
--rw-rw-rw-   0        0        0   833191 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/style.css.map
--rw-rw-rw-   0        0        0   293400 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/style.min.css
--rw-rw-rw-   0        0        0   728464 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/style.min.css.map
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.518195 django-admin-coreui-0.0.5/admin_coreui/static/css/vendors/
--rw-rw-rw-   0        0        0      136 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/vendors/simplebar.css
--rw-rw-rw-   0        0        0      264 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/css/vendors/simplebar.css.map
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.549994 django-admin-coreui-0.0.5/admin_coreui/static/js/
--rw-rw-rw-   0        0        0     4721 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/charts.js
--rw-rw-rw-   0        0        0     9093 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/charts.js.map
--rw-rw-rw-   0        0        0     2325 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/color-modes.js
--rw-rw-rw-   0        0        0     4760 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/color-modes.js.map
--rw-rw-rw-   0        0        0     1027 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/colors.js
--rw-rw-rw-   0        0        0     1819 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/colors.js.map
--rw-rw-rw-   0        0        0      671 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/config.js
--rw-rw-rw-   0        0        0     1309 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/config.js.map
--rw-rw-rw-   0        0        0     8323 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/main.js
--rw-rw-rw-   0        0        0    17712 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/main.js.map
--rw-rw-rw-   0        0        0      541 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/popovers.js
--rw-rw-rw-   0        0        0      860 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/popovers.js.map
--rw-rw-rw-   0        0        0      660 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/toasts.js
--rw-rw-rw-   0        0        0     1192 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/toasts.js.map
--rw-rw-rw-   0        0        0      541 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/tooltips.js
--rw-rw-rw-   0        0        0      858 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/tooltips.js.map
--rw-rw-rw-   0        0        0    14513 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/widgets.js
--rw-rw-rw-   0        0        0    27525 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/js/widgets.js.map
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.213512 django-admin-coreui-0.0.5/admin_coreui/static/vendors/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.210507 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.205987 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/chartjs/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.553993 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/chartjs/css/
--rw-rw-rw-   0        0        0     1931 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/chartjs/css/coreui-chartjs.css
--rw-rw-rw-   0        0        0     8155 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/chartjs/css/coreui-chartjs.css.map
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.556991 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/chartjs/js/
--rw-rw-rw-   0        0        0     4690 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/chartjs/js/coreui-chartjs.js
--rw-rw-rw-   0        0        0     9081 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/chartjs/js/coreui-chartjs.js.map
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.206988 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/coreui/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.560588 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/coreui/js/
--rw-rw-rw-   0        0        0    88068 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/coreui/js/coreui.bundle.min.js
--rw-rw-rw-   0        0        0   362032 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/coreui/js/coreui.bundle.min.js.map
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.209506 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.572768 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/
--rw-rw-rw-   0        0        0    31612 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/brand.min.css
--rw-rw-rw-   0        0        0    15076 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/brand.min.css.map
--rw-rw-rw-   0        0        0    10975 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/flag.min.css
--rw-rw-rw-   0        0        0     4360 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/flag.min.css.map
--rw-rw-rw-   0        0        0    22248 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/free.min.css
--rw-rw-rw-   0        0        0    10703 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/free.min.css.map
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.593443 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/
--rw-rw-rw-   0        0        0   522960 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.eot
--rw-rw-rw-   0        0        0  3405774 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.svg
--rw-rw-rw-   0        0        0   522752 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.ttf
--rw-rw-rw-   0        0        0   378328 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.woff
--rw-rw-rw-   0        0        0   146944 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.eot
--rw-rw-rw-   0        0        0   561928 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.svg
--rw-rw-rw-   0        0        0   146740 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.ttf
--rw-rw-rw-   0        0        0    78996 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.woff
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:28.606531 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/
--rw-rw-rw-   0        0        0  1456471 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/brand.svg
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.018097 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/
--rw-rw-rw-   0        0        0    69248 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ad.svg
--rw-rw-rw-   0        0        0      321 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ae.svg
--rw-rw-rw-   0        0        0    52644 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-af.svg
--rw-rw-rw-   0        0        0      617 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ag.svg
--rw-rw-rw-   0        0        0     9013 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-al.svg
--rw-rw-rw-   0        0        0      279 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-am.svg
--rw-rw-rw-   0        0        0     2556 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ao.svg
--rw-rw-rw-   0        0        0    11535 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ar.svg
--rw-rw-rw-   0        0        0      229 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-at.svg
--rw-rw-rw-   0        0        0     2078 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-au.svg
--rw-rw-rw-   0        0        0      620 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-az.svg
--rw-rw-rw-   0        0        0     1197 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ba.svg
--rw-rw-rw-   0        0        0     1068 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bb.svg
--rw-rw-rw-   0        0        0      232 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bd.svg
--rw-rw-rw-   0        0        0      281 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-be.svg
--rw-rw-rw-   0        0        0      390 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bf.svg
--rw-rw-rw-   0        0        0      277 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bg.svg
--rw-rw-rw-   0        0        0      280 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bh.svg
--rw-rw-rw-   0        0        0     1669 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bi.svg
--rw-rw-rw-   0        0        0      278 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bj.svg
--rw-rw-rw-   0        0        0    26617 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bn.svg
--rw-rw-rw-   0        0        0      291 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bo.svg
--rw-rw-rw-   0        0        0     8293 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-br.svg
--rw-rw-rw-   0        0        0      273 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bs.svg
--rw-rw-rw-   0        0        0    41412 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bt.svg
--rw-rw-rw-   0        0        0      278 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bw.svg
--rw-rw-rw-   0        0        0     8608 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-by.svg
--rw-rw-rw-   0        0        0   107351 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bz.svg
--rw-rw-rw-   0        0        0     1034 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ca.svg
--rw-rw-rw-   0        0        0      405 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cd.svg
--rw-rw-rw-   0        0        0      532 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cf.svg
--rw-rw-rw-   0        0        0      284 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cg.svg
--rw-rw-rw-   0        0        0      297 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ch.svg
--rw-rw-rw-   0        0        0      276 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ci.svg
--rw-rw-rw-   0        0        0     5532 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ck.svg
--rw-rw-rw-   0        0        0      445 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cl.svg
--rw-rw-rw-   0        0        0      412 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cm.svg
--rw-rw-rw-   0        0        0      529 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cn.svg
--rw-rw-rw-   0        0        0      280 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-co.svg
--rw-rw-rw-   0        0        0      276 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cr.svg
--rw-rw-rw-   0        0        0      438 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cu.svg
--rw-rw-rw-   0        0        0     1529 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cv.svg
--rw-rw-rw-   0        0        0    13897 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cy.svg
--rw-rw-rw-   0        0        0      276 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cz.svg
--rw-rw-rw-   0        0        0      274 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-de.svg
--rw-rw-rw-   0        0        0      451 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-dj.svg
--rw-rw-rw-   0        0        0      293 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-dk.svg
--rw-rw-rw-   0        0        0    15792 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-dm.svg
--rw-rw-rw-   0        0        0   179774 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-do.svg
--rw-rw-rw-   0        0        0      879 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-dz.svg
--rw-rw-rw-   0        0        0   295696 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ec.svg
--rw-rw-rw-   0        0        0      284 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ee.svg
--rw-rw-rw-   0        0        0    25811 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-eg.svg
--rw-rw-rw-   0        0        0     4464 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-er.svg
--rw-rw-rw-   0        0        0   142496 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-es.svg
--rw-rw-rw-   0        0        0     1145 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-et.svg
--rw-rw-rw-   0        0        0      289 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-fi.svg
--rw-rw-rw-   0        0        0   109829 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-fj.svg
--rw-rw-rw-   0        0        0      678 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-fm.svg
--rw-rw-rw-   0        0        0      271 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-fr.svg
--rw-rw-rw-   0        0        0      273 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ga.svg
--rw-rw-rw-   0        0        0      771 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gb.svg
--rw-rw-rw-   0        0        0     1527 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gd.svg
--rw-rw-rw-   0        0        0     1396 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ge.svg
--rw-rw-rw-   0        0        0      367 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gh.svg
--rw-rw-rw-   0        0        0      348 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gm.svg
--rw-rw-rw-   0        0        0     9364 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gn.svg
--rw-rw-rw-   0        0        0     9364 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gq.svg
--rw-rw-rw-   0        0        0      365 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gr.svg
--rw-rw-rw-   0        0        0    99692 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gt.svg
--rw-rw-rw-   0        0        0      441 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gw.svg
--rw-rw-rw-   0        0        0      395 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gy.svg
--rw-rw-rw-   0        0        0     3046 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hk.svg
--rw-rw-rw-   0        0        0      854 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hn.svg
--rw-rw-rw-   0        0        0   119564 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hr.svg
--rw-rw-rw-   0        0        0    40443 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ht.svg
--rw-rw-rw-   0        0        0      275 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hu.svg
--rw-rw-rw-   0        0        0      225 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-id.svg
--rw-rw-rw-   0        0        0      281 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ie.svg
--rw-rw-rw-   0        0        0      446 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-il.svg
--rw-rw-rw-   0        0        0     3887 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-in.svg
--rw-rw-rw-   0        0        0     3580 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-iq.svg
--rw-rw-rw-   0        0        0     5234 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ir.svg
--rw-rw-rw-   0        0        0      308 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-is.svg
--rw-rw-rw-   0        0        0      281 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-it.svg
--rw-rw-rw-   0        0        0      536 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-jm.svg
--rw-rw-rw-   0        0        0      521 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-jo.svg
--rw-rw-rw-   0        0        0      230 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-jp.svg
--rw-rw-rw-   0        0        0     1932 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ke.svg
--rw-rw-rw-   0        0        0    10437 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kg.svg
--rw-rw-rw-   0        0        0    20460 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kh.svg
--rw-rw-rw-   0        0        0     4811 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ki.svg
--rw-rw-rw-   0        0        0      976 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-km.svg
--rw-rw-rw-   0        0        0     1116 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kn.svg
--rw-rw-rw-   0        0        0      495 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kp.svg
--rw-rw-rw-   0        0        0     1765 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kr.svg
--rw-rw-rw-   0        0        0      327 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kw.svg
--rw-rw-rw-   0        0        0    31510 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kz.svg
--rw-rw-rw-   0        0        0      283 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-la.svg
--rw-rw-rw-   0        0        0     9268 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lb.svg
--rw-rw-rw-   0        0        0      360 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lc.svg
--rw-rw-rw-   0        0        0    17635 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-li.svg
--rw-rw-rw-   0        0        0    32573 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lk.svg
--rw-rw-rw-   0        0        0      715 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lr.svg
--rw-rw-rw-   0        0        0     3276 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ls.svg
--rw-rw-rw-   0        0        0      278 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lt.svg
--rw-rw-rw-   0        0        0      274 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lu.svg
--rw-rw-rw-   0        0        0      223 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lv.svg
--rw-rw-rw-   0        0        0      582 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ly.svg
--rw-rw-rw-   0        0        0      660 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ma.svg
--rw-rw-rw-   0        0        0      225 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mc.svg
--rw-rw-rw-   0        0        0    30845 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-md.svg
--rw-rw-rw-   0        0        0    98104 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-me.svg
--rw-rw-rw-   0        0        0      285 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mg.svg
--rw-rw-rw-   0        0        0     1118 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mh.svg
--rw-rw-rw-   0        0        0      471 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mk.svg
--rw-rw-rw-   0        0        0      284 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ml.svg
--rw-rw-rw-   0        0        0      447 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mm.svg
--rw-rw-rw-   0        0        0     1557 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mn.svg
--rw-rw-rw-   0        0        0      801 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mr.svg
--rw-rw-rw-   0        0        0    16379 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mt.svg
--rw-rw-rw-   0        0        0      331 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mu.svg
--rw-rw-rw-   0        0        0      352 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mv.svg
--rw-rw-rw-   0        0        0     5294 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mw.svg
--rw-rw-rw-   0        0        0   217014 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mx.svg
--rw-rw-rw-   0        0        0     1116 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-my.svg
--rw-rw-rw-   0        0        0     3135 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mz.svg
--rw-rw-rw-   0        0        0     1282 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-na.svg
--rw-rw-rw-   0        0        0      351 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ne.svg
--rw-rw-rw-   0        0        0      226 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ng.svg
--rw-rw-rw-   0        0        0    19703 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ni.svg
--rw-rw-rw-   0        0        0      278 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nl.svg
--rw-rw-rw-   0        0        0      424 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-no.svg
--rw-rw-rw-   0        0        0     1411 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-np.svg
--rw-rw-rw-   0        0        0      547 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nr.svg
--rw-rw-rw-   0        0        0     1690 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nu.svg
--rw-rw-rw-   0        0        0     2386 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nz.svg
--rw-rw-rw-   0        0        0    24184 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-om.svg
--rw-rw-rw-   0        0        0      604 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pa.svg
--rw-rw-rw-   0        0        0      226 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pe.svg
--rw-rw-rw-   0        0        0     3218 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pg.svg
--rw-rw-rw-   0        0        0     2008 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ph.svg
--rw-rw-rw-   0        0        0      441 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pk.svg
--rw-rw-rw-   0        0        0      229 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pl.svg
--rw-rw-rw-   0        0        0    45475 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pt.svg
--rw-rw-rw-   0        0        0      239 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pw.svg
--rw-rw-rw-   0        0        0    39303 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-py.svg
--rw-rw-rw-   0        0        0      460 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-qa.svg
--rw-rw-rw-   0        0        0      284 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ro.svg
--rw-rw-rw-   0        0        0   814059 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-rs.svg
--rw-rw-rw-   0        0        0      283 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ru.svg
--rw-rw-rw-   0        0        0     1242 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-rw.svg
--rw-rw-rw-   0        0        0    17152 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sa.svg
--rw-rw-rw-   0        0        0     1200 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sb.svg
--rw-rw-rw-   0        0        0      378 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sc.svg
--rw-rw-rw-   0        0        0      325 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sd.svg
--rw-rw-rw-   0        0        0      292 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-se.svg
--rw-rw-rw-   0        0        0     1193 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sg.svg
--rw-rw-rw-   0        0        0     1928 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-si.svg
--rw-rw-rw-   0        0        0     2466 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sk.svg
--rw-rw-rw-   0        0        0      290 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sl.svg
--rw-rw-rw-   0        0        0   164720 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sm.svg
--rw-rw-rw-   0        0        0      450 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sn.svg
--rw-rw-rw-   0        0        0      327 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-so.svg
--rw-rw-rw-   0        0        0      373 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sr.svg
--rw-rw-rw-   0        0        0      475 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ss.svg
--rw-rw-rw-   0        0        0      566 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-st.svg
--rw-rw-rw-   0        0        0   199390 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sv.svg
--rw-rw-rw-   0        0        0      563 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sy.svg
--rw-rw-rw-   0        0        0     8156 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sz.svg
--rw-rw-rw-   0        0        0      284 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-td.svg
--rw-rw-rw-   0        0        0      464 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tg.svg
--rw-rw-rw-   0        0        0      288 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-th.svg
--rw-rw-rw-   0        0        0     2147 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tj.svg
--rw-rw-rw-   0        0        0      435 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tl.svg
--rw-rw-rw-   0        0        0    66310 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tm.svg
--rw-rw-rw-   0        0        0      440 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tn.svg
--rw-rw-rw-   0        0        0      353 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-to.svg
--rw-rw-rw-   0        0        0      385 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tr.svg
--rw-rw-rw-   0        0        0      305 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tt.svg
--rw-rw-rw-   0        0        0     2111 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tv.svg
--rw-rw-rw-   0        0        0     1213 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tw.svg
--rw-rw-rw-   0        0        0      747 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tz.svg
--rw-rw-rw-   0        0        0      228 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ua.svg
--rw-rw-rw-   0        0        0     4062 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ug.svg
--rw-rw-rw-   0        0        0     6292 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-us.svg
--rw-rw-rw-   0        0        0     6541 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-uy.svg
--rw-rw-rw-   0        0        0     1842 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-uz.svg
--rw-rw-rw-   0        0        0    83348 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-va.svg
--rw-rw-rw-   0        0        0      444 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-vc.svg
--rw-rw-rw-   0        0        0     1266 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ve.svg
--rw-rw-rw-   0        0        0    70173 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-vg.svg
--rw-rw-rw-   0        0        0      339 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-vn.svg
--rw-rw-rw-   0        0        0      545 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ws.svg
--rw-rw-rw-   0        0        0     6467 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-xk.svg
--rw-rw-rw-   0        0        0      271 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ye.svg
--rw-rw-rw-   0        0        0      942 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-za.svg
--rw-rw-rw-   0        0        0     7357 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-zm.svg
--rw-rw-rw-   0        0        0     3010 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-zw.svg
--rw-rw-rw-   0        0        0  3544097 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag.svg
--rw-rw-rw-   0        0        0   421016 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/free.svg
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.211516 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/utils/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.021112 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/utils/js/
--rw-rw-rw-   0        0        0     8100 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/utils/js/index.js
--rw-rw-rw-   0        0        0     5763 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/utils/js/index.js.map
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.212514 django-admin-coreui-0.0.5/admin_coreui/static/vendors/chart.js/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.024104 django-admin-coreui-0.0.5/admin_coreui/static/vendors/chart.js/js/
--rw-rw-rw-   0        0        0   205228 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/chart.js/js/chart.umd.js
--rw-rw-rw-   0        0        0   953847 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/chart.js/js/chart.umd.js.map
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.214515 django-admin-coreui-0.0.5/admin_coreui/static/vendors/simplebar/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.027129 django-admin-coreui-0.0.5/admin_coreui/static/vendors/simplebar/css/
--rw-rw-rw-   0        0        0     4467 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/simplebar/css/simplebar.css
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.028640 django-admin-coreui-0.0.5/admin_coreui/static/vendors/simplebar/js/
--rw-rw-rw-   0        0        0    27067 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/static/vendors/simplebar/js/simplebar.min.js
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.043203 django-admin-coreui-0.0.5/admin_coreui/templates/
--rw-rw-rw-   0        0        0     1007 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/404.html
--rw-rw-rw-   0        0        0     1026 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/500.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.056299 django-admin-coreui-0.0.5/admin_coreui/templates/accounts/
--rw-rw-rw-   0        0        0     1292 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/accounts/change-password.html
--rw-rw-rw-   0        0        0     2303 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/accounts/login.html
--rw-rw-rw-   0        0        0      646 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/accounts/password-change-done.html
--rw-rw-rw-   0        0        0      702 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/accounts/password-reset-complete.html
--rw-rw-rw-   0        0        0     1314 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/accounts/password-reset-confirm.html
--rw-rw-rw-   0        0        0      726 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/accounts/password-reset-done.html
--rw-rw-rw-   0        0        0     1314 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/accounts/password-reset.html
--rw-rw-rw-   0        0        0     1318 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/accounts/register.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.090259 django-admin-coreui-0.0.5/admin_coreui/templates/admin/
--rw-rw-rw-   0        0        0        0 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/.gitkeep
--rw-rw-rw-   0        0        0     1743 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/actions.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:26.216515 django-admin-coreui-0.0.5/admin_coreui/templates/admin/auth/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.096268 django-admin-coreui-0.0.5/admin_coreui/templates/admin/auth/user/
--rw-rw-rw-   0        0        0      471 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/auth/user/add_form.html
--rw-rw-rw-   0        0        0     5363 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/auth/user/change_password.html
--rw-rw-rw-   0        0        0     6511 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/change_form.html
--rw-rw-rw-   0        0        0      696 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/change_form_object_tools.html
--rw-rw-rw-   0        0        0     5953 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/change_list.html
--rw-rw-rw-   0        0        0      479 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/change_list_object_tools.html
--rw-rw-rw-   0        0        0     3257 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/change_list_results.html
--rw-rw-rw-   0        0        0     7313 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/delete_confirmation.html
--rw-rw-rw-   0        0        0     7632 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/delete_selected_confirmation.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.102325 django-admin-coreui-0.0.5/admin_coreui/templates/admin/edit_inline/
--rw-rw-rw-   0        0        0     3893 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/edit_inline/stacked.html
--rw-rw-rw-   0        0        0     7834 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/edit_inline/tabular.html
--rw-rw-rw-   0        0        0      643 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/filter.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.108832 django-admin-coreui-0.0.5/admin_coreui/templates/admin/includes/
--rw-rw-rw-   0        0        0     2608 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/includes/fieldset.html
--rw-rw-rw-   0        0        0      339 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/includes/object_delete_summary.html
--rw-rw-rw-   0        0        0    45052 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/index.html
--rw-rw-rw-   0        0        0     3270 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/invalid_setup.html
--rw-rw-rw-   0        0        0     4103 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/login.html
--rw-rw-rw-   0        0        0     4402 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/object_history.html
--rw-rw-rw-   0        0        0     2318 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/pagination.html
--rw-rw-rw-   0        0        0     2641 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/search_form.html
--rw-rw-rw-   0        0        0     1616 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/admin/submit_line.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.138570 django-admin-coreui-0.0.5/admin_coreui/templates/base/
--rw-rw-rw-   0        0        0    11990 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/accordion.html
--rw-rw-rw-   0        0        0     4567 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/breadcrumb.html
--rw-rw-rw-   0        0        0    82746 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/cards.html
--rw-rw-rw-   0        0        0    28776 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/carousel.html
--rw-rw-rw-   0        0        0     9271 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/collapse.html
--rw-rw-rw-   0        0        0    34134 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/list-group.html
--rw-rw-rw-   0        0        0    52908 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/navs-tabs.html
--rw-rw-rw-   0        0        0    19133 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/pagination.html
--rw-rw-rw-   0        0        0    13926 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/placeholders.html
--rw-rw-rw-   0        0        0     9313 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/popovers.html
--rw-rw-rw-   0        0        0    18116 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/progress.html
--rw-rw-rw-   0        0        0    23874 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/spinners.html
--rw-rw-rw-   0        0        0    56754 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/tables.html
--rw-rw-rw-   0        0        0     7546 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/base/tooltips.html
--rw-rw-rw-   0        0        0     1886 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/blank.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.144130 django-admin-coreui-0.0.5/admin_coreui/templates/buttons/
--rw-rw-rw-   0        0        0    30739 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/buttons/button-group.html
--rw-rw-rw-   0        0        0    43034 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/buttons/buttons.html
--rw-rw-rw-   0        0        0    69301 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/buttons/dropdowns.html
--rw-rw-rw-   0        0        0    14383 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/charts.html
--rw-rw-rw-   0        0        0     3142 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/colors.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.156692 django-admin-coreui-0.0.5/admin_coreui/templates/forms/
--rw-rw-rw-   0        0        0    35183 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/forms/checks-radios.html
--rw-rw-rw-   0        0        0    14654 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/forms/floating-labels.html
--rw-rw-rw-   0        0        0    19111 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/forms/form-control.html
--rw-rw-rw-   0        0        0    32078 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/forms/input-group.html
--rw-rw-rw-   0        0        0    30767 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/forms/layout.html
--rw-rw-rw-   0        0        0     7863 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/forms/range.html
--rw-rw-rw-   0        0        0    10096 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/forms/select.html
--rw-rw-rw-   0        0        0    26760 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/forms/validation.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.163214 django-admin-coreui-0.0.5/admin_coreui/templates/icons/
--rw-rw-rw-   0        0        0   136182 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/icons/coreui-icons-brand.html
--rw-rw-rw-   0        0        0    31442 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/icons/coreui-icons-flag.html
--rw-rw-rw-   0        0        0    92991 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/icons/coreui-icons-free.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.171535 django-admin-coreui-0.0.5/admin_coreui/templates/includes/
--rw-rw-rw-   0        0        0     3049 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/includes/head.html
--rw-rw-rw-   0        0        0    17068 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/includes/navbar.html
--rw-rw-rw-   0        0        0     1873 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/includes/scripts.html
--rw-rw-rw-   0        0        0    23256 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/includes/sidebar.html
--rw-rw-rw-   0        0        0      824 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/includes/topbar.html
--rw-rw-rw-   0        0        0    47374 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/index.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.174495 django-admin-coreui-0.0.5/admin_coreui/templates/layouts/
--rw-rw-rw-   0        0        0      667 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/layouts/base-fullscreen.html
--rw-rw-rw-   0        0        0      956 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/layouts/base.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.180789 django-admin-coreui-0.0.5/admin_coreui/templates/notifications/
--rw-rw-rw-   0        0        0    10717 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/notifications/alerts.html
--rw-rw-rw-   0        0        0     8451 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/notifications/badge.html
--rw-rw-rw-   0        0        0    57472 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/notifications/modals.html
--rw-rw-rw-   0        0        0    17214 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/notifications/toasts.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.188428 django-admin-coreui-0.0.5/admin_coreui/templates/registration/
--rw-rw-rw-   0        0        0        0 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/registration/.gitkeep
--rw-rw-rw-   0        0        0     1690 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/registration/logged_out.html
--rw-rw-rw-   0        0        0     2672 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/registration/password_change_done.html
--rw-rw-rw-   0        0        0     3948 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/registration/password_change_form.html
--rw-rw-rw-   0        0        0     7832 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/typography.html
--rw-rw-rw-   0        0        0   107237 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templates/widgets.html
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.193386 django-admin-coreui-0.0.5/admin_coreui/templatetags/
--rw-rw-rw-   0        0        0        0 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templatetags/__init__.py
--rw-rw-rw-   0        0        0     2551 2024-04-28 06:32:23.000000 django-admin-coreui-0.0.5/admin_coreui/templatetags/admin_coreui.py
--rw-rw-rw-   0        0        0      237 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/templatetags/replace_value.py
--rw-rw-rw-   0        0        0       63 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/tests.py
--rw-rw-rw-   0        0        0     3485 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/urls.py
--rw-rw-rw-   0        0        0    16587 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.5/admin_coreui/utils.py
--rw-rw-rw-   0        0        0     5779 2024-04-28 06:32:23.000000 django-admin-coreui-0.0.5/admin_coreui/views.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:50:29.225720 django-admin-coreui-0.0.5/django_admin_coreui.egg-info/
--rw-rw-rw-   0        0        0     7415 2024-04-28 06:50:25.000000 django-admin-coreui-0.0.5/django_admin_coreui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    70589 2024-04-28 06:50:26.000000 django-admin-coreui-0.0.5/django_admin_coreui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 06:50:25.000000 django-admin-coreui-0.0.5/django_admin_coreui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-28 06:12:07.000000 django-admin-coreui-0.0.5/django_admin_coreui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2024-04-28 06:50:25.000000 django-admin-coreui-0.0.5/django_admin_coreui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 06:50:29.229205 django-admin-coreui-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1340 2024-04-28 06:49:10.000000 django-admin-coreui-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.767359 django-admin-coreui-0.0.6/
+-rw-rw-rw-   0        0        0     1113 2022-12-05 15:06:59.000000 django-admin-coreui-0.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0      148 2024-04-28 06:49:04.000000 django-admin-coreui-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     7415 2024-04-28 06:56:06.765848 django-admin-coreui-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6323 2024-04-28 06:13:31.000000 django-admin-coreui-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.829903 django-admin-coreui-0.0.6/admin_coreui/
+-rw-rw-rw-   0        0        0        0 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/admin.py
+-rw-rw-rw-   0        0        0      186 2024-04-28 06:54:17.000000 django-admin-coreui-0.0.6/admin_coreui/apps.py
+-rw-rw-rw-   0        0        0     2623 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/forms.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.831918 django-admin-coreui-0.0.6/admin_coreui/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/models.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.664955 django-admin-coreui-0.0.6/admin_coreui/static/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.835915 django-admin-coreui-0.0.6/admin_coreui/static/assets/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.837498 django-admin-coreui-0.0.6/admin_coreui/static/assets/brand/
+-rw-rw-rw-   0        0        0     3305 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/brand/coreui.svg
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.840452 django-admin-coreui-0.0.6/admin_coreui/static/assets/css/
+-rw-rw-rw-   0        0        0    10376 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/css/forms.css
+-rw-rw-rw-   0        0        0    12542 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/css/widgets.css
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.895626 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/
+-rw-rw-rw-   0        0        0    13344 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/android-icon-144x144.png
+-rw-rw-rw-   0        0        0    17566 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/android-icon-192x192.png
+-rw-rw-rw-   0        0        0     2495 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/android-icon-36x36.png
+-rw-rw-rw-   0        0        0     3537 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/android-icon-48x48.png
+-rw-rw-rw-   0        0        0     5297 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/android-icon-72x72.png
+-rw-rw-rw-   0        0        0     7298 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/android-icon-96x96.png
+-rw-rw-rw-   0        0        0     9891 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-114x114.png
+-rw-rw-rw-   0        0        0    10620 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-120x120.png
+-rw-rw-rw-   0        0        0    13344 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-144x144.png
+-rw-rw-rw-   0        0        0    14451 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-152x152.png
+-rw-rw-rw-   0        0        0    17458 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-180x180.png
+-rw-rw-rw-   0        0        0     4120 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-57x57.png
+-rw-rw-rw-   0        0        0     4034 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-60x60.png
+-rw-rw-rw-   0        0        0     5297 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-72x72.png
+-rw-rw-rw-   0        0        0     5539 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-76x76.png
+-rw-rw-rw-   0        0        0    18140 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-precomposed.png
+-rw-rw-rw-   0        0        0    18140 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon.png
+-rw-rw-rw-   0        0        0      282 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/browserconfig.xml
+-rw-rw-rw-   0        0        0     1201 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/favicon-16x16.png
+-rw-rw-rw-   0        0        0     2196 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/favicon-32x32.png
+-rw-rw-rw-   0        0        0     7298 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/favicon-96x96.png
+-rw-rw-rw-   0        0        0     1150 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/favicon.ico
+-rw-rw-rw-   0        0        0      849 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/manifest.json
+-rw-rw-rw-   0        0        0    13344 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/ms-icon-144x144.png
+-rw-rw-rw-   0        0        0    14113 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/ms-icon-150x150.png
+-rw-rw-rw-   0        0        0    37803 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/ms-icon-310x310.png
+-rw-rw-rw-   0        0        0     5120 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/ms-icon-70x70.png
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:05.053968 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/
+-rw-rw-rw-   0        0        0      696 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/3d.svg
+-rw-rw-rw-   0        0        0      626 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/4k.svg
+-rw-rw-rw-   0        0        0      375 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/account-logout.svg
+-rw-rw-rw-   0        0        0      486 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/action-redo.svg
+-rw-rw-rw-   0        0        0      755 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/action-undo.svg
+-rw-rw-rw-   0        0        0     1226 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/address-book.svg
+-rw-rw-rw-   0        0        0     1023 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/airplane-mode-off.svg
+-rw-rw-rw-   0        0        0      906 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/airplane-mode.svg
+-rw-rw-rw-   0        0        0      479 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/airplay.svg
+-rw-rw-rw-   0        0        0      725 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/alarm.svg
+-rw-rw-rw-   0        0        0     1089 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/album.svg
+-rw-rw-rw-   0        0        0      416 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/align-center.svg
+-rw-rw-rw-   0        0        0      432 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/align-left.svg
+-rw-rw-rw-   0        0        0      435 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/align-right.svg
+-rw-rw-rw-   0        0        0     1309 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/american-football.svg
+-rw-rw-rw-   0        0        0     1634 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/android.svg
+-rw-rw-rw-   0        0        0      475 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/angular.svg
+-rw-rw-rw-   0        0        0     1702 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/aperture.svg
+-rw-rw-rw-   0        0        0     1534 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/apple.svg
+-rw-rw-rw-   0        0        0     1983 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/applications-settings.svg
+-rw-rw-rw-   0        0        0     2289 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/applications.svg
+-rw-rw-rw-   0        0        0      287 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-bottom.svg
+-rw-rw-rw-   0        0        0      662 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-circle-bottom.svg
+-rw-rw-rw-   0        0        0      660 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-circle-left.svg
+-rw-rw-rw-   0        0        0      664 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-circle-right.svg
+-rw-rw-rw-   0        0        0      656 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-circle-top.svg
+-rw-rw-rw-   0        0        0      282 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-left.svg
+-rw-rw-rw-   0        0        0      286 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-right.svg
+-rw-rw-rw-   0        0        0      336 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-thick-bottom.svg
+-rw-rw-rw-   0        0        0      383 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-thick-from-bottom.svg
+-rw-rw-rw-   0        0        0      376 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-thick-from-left.svg
+-rw-rw-rw-   0        0        0      390 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-thick-from-right.svg
+-rw-rw-rw-   0        0        0      387 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-thick-from-top.svg
+-rw-rw-rw-   0        0        0      335 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-thick-left.svg
+-rw-rw-rw-   0        0        0      339 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-thick-right.svg
+-rw-rw-rw-   0        0        0      376 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-thick-to-bottom.svg
+-rw-rw-rw-   0        0        0      382 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-thick-to-left.svg
+-rw-rw-rw-   0        0        0      372 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-thick-to-right.svg
+-rw-rw-rw-   0        0        0      372 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-thick-to-top.svg
+-rw-rw-rw-   0        0        0      341 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-thick-top.svg
+-rw-rw-rw-   0        0        0      284 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-top.svg
+-rw-rw-rw-   0        0        0     1506 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/assistive-listening-system.svg
+-rw-rw-rw-   0        0        0      755 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/asterisk-circle.svg
+-rw-rw-rw-   0        0        0      405 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/asterisk.svg
+-rw-rw-rw-   0        0        0     1064 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/at.svg
+-rw-rw-rw-   0        0        0      763 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/audio-description.svg
+-rw-rw-rw-   0        0        0      460 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/audio-spectrum.svg
+-rw-rw-rw-   0        0        0     1428 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/audio.svg
+-rw-rw-rw-   0        0        0      716 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/av-timer.svg
+-rw-rw-rw-   0        0        0      915 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/badge.svg
+-rw-rw-rw-   0        0        0     1373 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/balance-scale.svg
+-rw-rw-rw-   0        0        0      764 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/ban.svg
+-rw-rw-rw-   0        0        0      646 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bank.svg
+-rw-rw-rw-   0        0        0      688 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bar-chart.svg
+-rw-rw-rw-   0        0        0      659 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/barcode.svg
+-rw-rw-rw-   0        0        0     1488 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/baseball.svg
+-rw-rw-rw-   0        0        0      602 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/basket.svg
+-rw-rw-rw-   0        0        0     1561 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/basketball.svg
+-rw-rw-rw-   0        0        0     1341 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bath.svg
+-rw-rw-rw-   0        0        0      530 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/battery-0.svg
+-rw-rw-rw-   0        0        0      684 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/battery-3.svg
+-rw-rw-rw-   0        0        0      790 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/battery-5.svg
+-rw-rw-rw-   0        0        0      647 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/battery-alert.svg
+-rw-rw-rw-   0        0        0      611 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/battery-slash.svg
+-rw-rw-rw-   0        0        0     1061 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/beach-access.svg
+-rw-rw-rw-   0        0        0      702 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/beaker.svg
+-rw-rw-rw-   0        0        0      522 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bed.svg
+-rw-rw-rw-   0        0        0      878 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bell.svg
+-rw-rw-rw-   0        0        0     1172 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bike.svg
+-rw-rw-rw-   0        0        0     1676 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/birthday-cake.svg
+-rw-rw-rw-   0        0        0      793 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/blind.svg
+-rw-rw-rw-   0        0        0      398 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bluetooth.svg
+-rw-rw-rw-   0        0        0     3490 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/blur-circular.svg
+-rw-rw-rw-   0        0        0     1893 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/blur-linear.svg
+-rw-rw-rw-   0        0        0     2628 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/blur.svg
+-rw-rw-rw-   0        0        0      724 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/boat-alt.svg
+-rw-rw-rw-   0        0        0      633 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bold.svg
+-rw-rw-rw-   0        0        0      327 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bolt.svg
+-rw-rw-rw-   0        0        0      692 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/book.svg
+-rw-rw-rw-   0        0        0      302 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bookmark.svg
+-rw-rw-rw-   0        0        0      931 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bootstrap.svg
+-rw-rw-rw-   0        0        0      485 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-all.svg
+-rw-rw-rw-   0        0        0     1714 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-bottom.svg
+-rw-rw-rw-   0        0        0     2042 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-clear.svg
+-rw-rw-rw-   0        0        0     1689 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-horizontal.svg
+-rw-rw-rw-   0        0        0     1377 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-inner.svg
+-rw-rw-rw-   0        0        0     1722 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-left.svg
+-rw-rw-rw-   0        0        0      934 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-outer.svg
+-rw-rw-rw-   0        0        0     1713 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-right.svg
+-rw-rw-rw-   0        0        0      881 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-style.svg
+-rw-rw-rw-   0        0        0     1717 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-top.svg
+-rw-rw-rw-   0        0        0     1691 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-vertical.svg
+-rw-rw-rw-   0        0        0     1751 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bowling.svg
+-rw-rw-rw-   0        0        0     5934 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/braille.svg
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:05.943874 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/
+-rw-rw-rw-   0        0        0     1245 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/500px.svg
+-rw-rw-rw-   0        0        0      775 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/accessible-icon.svg
+-rw-rw-rw-   0        0        0      852 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/accusoft.svg
+-rw-rw-rw-   0        0        0     1391 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/acquisitions-incorporated.svg
+-rw-rw-rw-   0        0        0      267 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/adn.svg
+-rw-rw-rw-   0        0        0      187 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/adobe.svg
+-rw-rw-rw-   0        0        0     1306 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/adversal.svg
+-rw-rw-rw-   0        0        0      404 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/affiliatetheme.svg
+-rw-rw-rw-   0        0        0      849 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/airbnb.svg
+-rw-rw-rw-   0        0        0      907 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/algolia.svg
+-rw-rw-rw-   0        0        0      745 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/alipay.svg
+-rw-rw-rw-   0        0        0     3466 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/amazon-pay.svg
+-rw-rw-rw-   0        0        0      720 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/amazon.svg
+-rw-rw-rw-   0        0        0      605 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/amilia.svg
+-rw-rw-rw-   0        0        0      907 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/android.svg
+-rw-rw-rw-   0        0        0     1382 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/angellist.svg
+-rw-rw-rw-   0        0        0     1951 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/angrycreative.svg
+-rw-rw-rw-   0        0        0      239 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/angular.svg
+-rw-rw-rw-   0        0        0      726 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/app-store-ios.svg
+-rw-rw-rw-   0        0        0      858 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/app-store.svg
+-rw-rw-rw-   0        0        0     1729 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/apper.svg
+-rw-rw-rw-   0        0        0     1190 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/apple-pay.svg
+-rw-rw-rw-   0        0        0      515 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/apple.svg
+-rw-rw-rw-   0        0        0      273 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/artstation.svg
+-rw-rw-rw-   0        0        0      764 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/asymmetrik.svg
+-rw-rw-rw-   0        0        0      366 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/atlassian.svg
+-rw-rw-rw-   0        0        0      574 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/audible.svg
+-rw-rw-rw-   0        0        0      279 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/autoprefixer.svg
+-rw-rw-rw-   0        0        0      571 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/avianex.svg
+-rw-rw-rw-   0        0        0     2177 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/aviato.svg
+-rw-rw-rw-   0        0        0     2310 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/aws.svg
+-rw-rw-rw-   0        0        0      192 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/bandcamp.svg
+-rw-rw-rw-   0        0        0     2573 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/battle-net.svg
+-rw-rw-rw-   0        0        0      783 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/behance-square.svg
+-rw-rw-rw-   0        0        0      684 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/behance.svg
+-rw-rw-rw-   0        0        0      485 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/bimobject.svg
+-rw-rw-rw-   0        0        0      306 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/bitbucket.svg
+-rw-rw-rw-   0        0        0     1165 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/bitcoin.svg
+-rw-rw-rw-   0        0        0      759 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/bity.svg
+-rw-rw-rw-   0        0        0      177 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/black-tie.svg
+-rw-rw-rw-   0        0        0      676 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/blackberry.svg
+-rw-rw-rw-   0        0        0      900 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/blogger-b.svg
+-rw-rw-rw-   0        0        0     1199 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/blogger.svg
+-rw-rw-rw-   0        0        0      371 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/bluetooth-b.svg
+-rw-rw-rw-   0        0        0      370 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/bluetooth.svg
+-rw-rw-rw-   0        0        0      606 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/bootstrap.svg
+-rw-rw-rw-   0        0        0   442536 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/brands-symbol-defs.svg
+-rw-rw-rw-   0        0        0      758 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/btc.svg
+-rw-rw-rw-   0        0        0      719 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/buffer.svg
+-rw-rw-rw-   0        0        0      474 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/buromobelexperte.svg
+-rw-rw-rw-   0        0        0      297 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/buysellads.svg
+-rw-rw-rw-   0        0        0      866 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/canadian-maple-leaf.svg
+-rw-rw-rw-   0        0        0     3428 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-amazon-pay.svg
+-rw-rw-rw-   0        0        0     3197 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-amex.svg
+-rw-rw-rw-   0        0        0     1285 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-apple-pay.svg
+-rw-rw-rw-   0        0        0      600 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-diners-club.svg
+-rw-rw-rw-   0        0        0     1237 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-discover.svg
+-rw-rw-rw-   0        0        0      779 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-jcb.svg
+-rw-rw-rw-   0        0        0     3020 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-mastercard.svg
+-rw-rw-rw-   0        0        0     1762 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-paypal.svg
+-rw-rw-rw-   0        0        0     1288 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-stripe.svg
+-rw-rw-rw-   0        0        0      934 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-visa.svg
+-rw-rw-rw-   0        0        0      455 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/centercode.svg
+-rw-rw-rw-   0        0        0      913 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/centos.svg
+-rw-rw-rw-   0        0        0      577 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/chrome.svg
+-rw-rw-rw-   0        0        0      474 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/chromecast.svg
+-rw-rw-rw-   0        0        0      631 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cloudscale.svg
+-rw-rw-rw-   0        0        0      294 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cloudsmith.svg
+-rw-rw-rw-   0        0        0     1362 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cloudversify.svg
+-rw-rw-rw-   0        0        0      745 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/codepen.svg
+-rw-rw-rw-   0        0        0      537 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/codiepie.svg
+-rw-rw-rw-   0        0        0      592 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/confluence.svg
+-rw-rw-rw-   0        0        0     3122 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/connectdevelop.svg
+-rw-rw-rw-   0        0        0      552 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/contao.svg
+-rw-rw-rw-   0        0        0     1431 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cpanel.svg
+-rw-rw-rw-   0        0        0      579 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-by.svg
+-rw-rw-rw-   0        0        0      824 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-nc-eu.svg
+-rw-rw-rw-   0        0        0      582 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-nc-jp.svg
+-rw-rw-rw-   0        0        0      742 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-nc.svg
+-rw-rw-rw-   0        0        0      386 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-nd.svg
+-rw-rw-rw-   0        0        0      618 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-pd-alt.svg
+-rw-rw-rw-   0        0        0      658 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-pd.svg
+-rw-rw-rw-   0        0        0      648 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-remix.svg
+-rw-rw-rw-   0        0        0      586 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-sa.svg
+-rw-rw-rw-   0        0        0     1171 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-sampling-plus.svg
+-rw-rw-rw-   0        0        0     1235 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-sampling.svg
+-rw-rw-rw-   0        0        0      625 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-share.svg
+-rw-rw-rw-   0        0        0      664 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-zero.svg
+-rw-rw-rw-   0        0        0      962 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons.svg
+-rw-rw-rw-   0        0        0     7133 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/critical-role.svg
+-rw-rw-rw-   0        0        0      317 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/css3-alt.svg
+-rw-rw-rw-   0        0        0      207 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/css3.svg
+-rw-rw-rw-   0        0        0      330 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cuttlefish.svg
+-rw-rw-rw-   0        0        0     3996 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/d-and-d-beyond.svg
+-rw-rw-rw-   0        0        0     4519 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/d-and-d.svg
+-rw-rw-rw-   0        0        0      320 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/dashcube.svg
+-rw-rw-rw-   0        0        0      546 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/delicious.svg
+-rw-rw-rw-   0        0        0      844 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/deploydog.svg
+-rw-rw-rw-   0        0        0      687 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/deskpro.svg
+-rw-rw-rw-   0        0        0      765 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/dev.svg
+-rw-rw-rw-   0        0        0      252 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/deviantart.svg
+-rw-rw-rw-   0        0        0      839 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/dhl.svg
+-rw-rw-rw-   0        0        0      486 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/diaspora.svg
+-rw-rw-rw-   0        0        0      384 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/digg.svg
+-rw-rw-rw-   0        0        0      376 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/digital-ocean.svg
+-rw-rw-rw-   0        0        0     1218 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/discord.svg
+-rw-rw-rw-   0        0        0      343 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/discourse.svg
+-rw-rw-rw-   0        0        0      267 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/dochub.svg
+-rw-rw-rw-   0        0        0      663 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/docker.svg
+-rw-rw-rw-   0        0        0      779 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/draft2digital.svg
+-rw-rw-rw-   0        0        0      921 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/dribbble-square.svg
+-rw-rw-rw-   0        0        0     1131 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/dribbble.svg
+-rw-rw-rw-   0        0        0      310 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/dropbox.svg
+-rw-rw-rw-   0        0        0      771 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/drupal.svg
+-rw-rw-rw-   0        0        0      260 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/dyalog.svg
+-rw-rw-rw-   0        0        0     1927 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/earlybirds.svg
+-rw-rw-rw-   0        0        0     1097 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ebay.svg
+-rw-rw-rw-   0        0        0      615 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/edge.svg
+-rw-rw-rw-   0        0        0      326 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/elementor.svg
+-rw-rw-rw-   0        0        0      428 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ello.svg
+-rw-rw-rw-   0        0        0     1933 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ember.svg
+-rw-rw-rw-   0        0        0     1847 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/empire.svg
+-rw-rw-rw-   0        0        0      366 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/envira.svg
+-rw-rw-rw-   0        0        0      432 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/erlang.svg
+-rw-rw-rw-   0        0        0      175 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ethereum.svg
+-rw-rw-rw-   0        0        0      662 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/etsy.svg
+-rw-rw-rw-   0        0        0     1009 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/evernote.svg
+-rw-rw-rw-   0        0        0      962 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/expeditedssl.svg
+-rw-rw-rw-   0        0        0      252 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/facebook-f.svg
+-rw-rw-rw-   0        0        0      554 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/facebook-messenger.svg
+-rw-rw-rw-   0        0        0      338 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/facebook-square.svg
+-rw-rw-rw-   0        0        0      344 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/facebook.svg
+-rw-rw-rw-   0        0        0     1139 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fantasy-flight-games.svg
+-rw-rw-rw-   0        0        0      819 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fedex.svg
+-rw-rw-rw-   0        0        0     2243 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fedora.svg
+-rw-rw-rw-   0        0        0      263 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/figma.svg
+-rw-rw-rw-   0        0        0     2632 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/firefox.svg
+-rw-rw-rw-   0        0        0     1530 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/first-order-alt.svg
+-rw-rw-rw-   0        0        0     1242 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/first-order.svg
+-rw-rw-rw-   0        0        0      267 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/firstdraft.svg
+-rw-rw-rw-   0        0        0      379 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/flickr.svg
+-rw-rw-rw-   0        0        0      156 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/flipboard.svg
+-rw-rw-rw-   0        0        0      740 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fly.svg
+-rw-rw-rw-   0        0        0      814 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/font-awesome-alt.svg
+-rw-rw-rw-   0        0        0      657 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/font-awesome-flag.svg
+-rw-rw-rw-   0        0        0     2994 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/font-awesome-logo-full.svg
+-rw-rw-rw-   0        0        0      699 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/font-awesome.svg
+-rw-rw-rw-   0        0        0      614 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fonticons-fi.svg
+-rw-rw-rw-   0        0        0      640 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fonticons.svg
+-rw-rw-rw-   0        0        0     3691 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fort-awesome-alt.svg
+-rw-rw-rw-   0        0        0     1019 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fort-awesome.svg
+-rw-rw-rw-   0        0        0      617 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/forumbee.svg
+-rw-rw-rw-   0        0        0      623 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/foursquare.svg
+-rw-rw-rw-   0        0        0     1312 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/free-code-camp.svg
+-rw-rw-rw-   0        0        0      596 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/freebsd.svg
+-rw-rw-rw-   0        0        0      339 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fulcrum.svg
+-rw-rw-rw-   0        0        0     1603 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/galactic-republic.svg
+-rw-rw-rw-   0        0        0     2684 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/galactic-senate.svg
+-rw-rw-rw-   0        0        0      424 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/get-pocket.svg
+-rw-rw-rw-   0        0        0      410 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/gg-circle.svg
+-rw-rw-rw-   0        0        0      341 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/gg.svg
+-rw-rw-rw-   0        0        0      538 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/git-alt.svg
+-rw-rw-rw-   0        0        0     1216 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/git-square.svg
+-rw-rw-rw-   0        0        0     1099 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/git.svg
+-rw-rw-rw-   0        0        0      880 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/github-alt.svg
+-rw-rw-rw-   0        0        0     1494 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/github-square.svg
+-rw-rw-rw-   0        0        0     1384 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/github.svg
+-rw-rw-rw-   0        0        0     1354 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/gitkraken.svg
+-rw-rw-rw-   0        0        0      354 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/gitlab.svg
+-rw-rw-rw-   0        0        0      194 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/gitter.svg
+-rw-rw-rw-   0        0        0      758 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/glide-g.svg
+-rw-rw-rw-   0        0        0      855 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/glide.svg
+-rw-rw-rw-   0        0        0      440 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/gofore.svg
+-rw-rw-rw-   0        0        0      723 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/goodreads-g.svg
+-rw-rw-rw-   0        0        0      811 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/goodreads.svg
+-rw-rw-rw-   0        0        0      217 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/google-drive.svg
+-rw-rw-rw-   0        0        0      326 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/google-play.svg
+-rw-rw-rw-   0        0        0      557 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/google-plus-g.svg
+-rw-rw-rw-   0        0        0      498 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/google-plus-square.svg
+-rw-rw-rw-   0        0        0      501 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/google-plus.svg
+-rw-rw-rw-   0        0        0      598 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/google-wallet.svg
+-rw-rw-rw-   0        0        0      327 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/google.svg
+-rw-rw-rw-   0        0        0      333 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/gratipay.svg
+-rw-rw-rw-   0        0        0     1628 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/grav.svg
+-rw-rw-rw-   0        0        0      690 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/gripfire.svg
+-rw-rw-rw-   0        0        0     5490 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/grunt.svg
+-rw-rw-rw-   0        0        0     2601 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/gulp.svg
+-rw-rw-rw-   0        0        0      346 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hacker-news-square.svg
+-rw-rw-rw-   0        0        0      260 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hacker-news.svg
+-rw-rw-rw-   0        0        0      843 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hackerrank.svg
+-rw-rw-rw-   0        0        0     1445 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hips.svg
+-rw-rw-rw-   0        0        0     1062 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hire-a-helper.svg
+-rw-rw-rw-   0        0        0     1486 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hooli.svg
+-rw-rw-rw-   0        0        0     1094 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hornbill.svg
+-rw-rw-rw-   0        0        0      350 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hotjar.svg
+-rw-rw-rw-   0        0        0      142 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/houzz.svg
+-rw-rw-rw-   0        0        0      279 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/html5.svg
+-rw-rw-rw-   0        0        0      832 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hubspot.svg
+-rw-rw-rw-   0        0        0      753 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/imdb.svg
+-rw-rw-rw-   0        0        0     1002 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/instagram.svg
+-rw-rw-rw-   0        0        0      662 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/intercom.svg
+-rw-rw-rw-   0        0        0      937 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/internet-explorer.svg
+-rw-rw-rw-   0        0        0      683 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/invision.svg
+-rw-rw-rw-   0        0        0      703 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ioxhost.svg
+-rw-rw-rw-   0        0        0     1265 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/itch-io.svg
+-rw-rw-rw-   0        0        0      662 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/itunes-note.svg
+-rw-rw-rw-   0        0        0      952 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/itunes.svg
+-rw-rw-rw-   0        0        0     1182 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/java.svg
+-rw-rw-rw-   0        0        0      736 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/jedi-order.svg
+-rw-rw-rw-   0        0        0     4341 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/jenkins.svg
+-rw-rw-rw-   0        0        0      299 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/jira.svg
+-rw-rw-rw-   0        0        0      877 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/joget.svg
+-rw-rw-rw-   0        0        0     1145 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/joomla.svg
+-rw-rw-rw-   0        0        0      697 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/js-square.svg
+-rw-rw-rw-   0        0        0      611 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/js.svg
+-rw-rw-rw-   0        0        0     1903 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/jsfiddle.svg
+-rw-rw-rw-   0        0        0      318 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/kaggle.svg
+-rw-rw-rw-   0        0        0     1916 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/keybase.svg
+-rw-rw-rw-   0        0        0     1519 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/keycdn.svg
+-rw-rw-rw-   0        0        0      372 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/kickstarter-k.svg
+-rw-rw-rw-   0        0        0      469 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/kickstarter.svg
+-rw-rw-rw-   0        0        0      330 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/korvue.svg
+-rw-rw-rw-   0        0        0     1122 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/laravel.svg
+-rw-rw-rw-   0        0        0      737 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/lastfm-square.svg
+-rw-rw-rw-   0        0        0      649 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/lastfm.svg
+-rw-rw-rw-   0        0        0     1163 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/leanpub.svg
+-rw-rw-rw-   0        0        0     1840 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/less.svg
+-rw-rw-rw-   0        0        0     1205 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/line.svg
+-rw-rw-rw-   0        0        0      380 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/linkedin-in.svg
+-rw-rw-rw-   0        0        0      504 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/linkedin.svg
+-rw-rw-rw-   0        0        0     1337 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/linode.svg
+-rw-rw-rw-   0        0        0     3568 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/linux.svg
+-rw-rw-rw-   0        0        0      675 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/lyft.svg
+-rw-rw-rw-   0        0        0      279 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/magento.svg
+-rw-rw-rw-   0        0        0     3137 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/mailchimp.svg
+-rw-rw-rw-   0        0        0     5988 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/mandalorian.svg
+-rw-rw-rw-   0        0        0      359 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/markdown.svg
+-rw-rw-rw-   0        0        0      695 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/mastodon.svg
+-rw-rw-rw-   0        0        0      300 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/maxcdn.svg
+-rw-rw-rw-   0        0        0      896 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/medapps.svg
+-rw-rw-rw-   0        0        0      413 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/medium-m.svg
+-rw-rw-rw-   0        0        0      416 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/medium.svg
+-rw-rw-rw-   0        0        0      836 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/medrt.svg
+-rw-rw-rw-   0        0        0     2132 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/meetup.svg
+-rw-rw-rw-   0        0        0      429 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/megaport.svg
+-rw-rw-rw-   0        0        0      736 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/mendeley.svg
+-rw-rw-rw-   0        0        0      187 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/microsoft.svg
+-rw-rw-rw-   0        0        0      224 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/mix.svg
+-rw-rw-rw-   0        0        0     1375 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/mixcloud.svg
+-rw-rw-rw-   0        0        0      437 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/mizuni.svg
+-rw-rw-rw-   0        0        0      248 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/modx.svg
+-rw-rw-rw-   0        0        0      294 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/monero.svg
+-rw-rw-rw-   0        0        0      980 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/napster.svg
+-rw-rw-rw-   0        0        0      439 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/neos.svg
+-rw-rw-rw-   0        0        0      554 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/nimblr.svg
+-rw-rw-rw-   0        0        0     1164 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/node-js.svg
+-rw-rw-rw-   0        0        0     3117 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/node.svg
+-rw-rw-rw-   0        0        0      254 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/npm.svg
+-rw-rw-rw-   0        0        0     1026 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ns8.svg
+-rw-rw-rw-   0        0        0     1498 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/nutritionix.svg
+-rw-rw-rw-   0        0        0      768 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/odnoklassniki-square.svg
+-rw-rw-rw-   0        0        0      663 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/odnoklassniki.svg
+-rw-rw-rw-   0        0        0    11219 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/old-republic.svg
+-rw-rw-rw-   0        0        0      426 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/opencart.svg
+-rw-rw-rw-   0        0        0      334 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/openid.svg
+-rw-rw-rw-   0        0        0      494 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/opera.svg
+-rw-rw-rw-   0        0        0     4751 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/optin-monster.svg
+-rw-rw-rw-   0        0        0      955 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/osi.svg
+-rw-rw-rw-   0        0        0      804 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/page4.svg
+-rw-rw-rw-   0        0        0      564 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pagelines.svg
+-rw-rw-rw-   0        0        0      842 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/palfed.svg
+-rw-rw-rw-   0        0        0      237 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/patreon.svg
+-rw-rw-rw-   0        0        0      633 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/paypal.svg
+-rw-rw-rw-   0        0        0     1202 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/penny-arcade.svg
+-rw-rw-rw-   0        0        0      608 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/periscope.svg
+-rw-rw-rw-   0        0        0     1028 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/phabricator.svg
+-rw-rw-rw-   0        0        0     2492 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/phoenix-framework.svg
+-rw-rw-rw-   0        0        0     1597 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/phoenix-squadron.svg
+-rw-rw-rw-   0        0        0      852 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/php.svg
+-rw-rw-rw-   0        0        0     1672 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pied-piper-alt.svg
+-rw-rw-rw-   0        0        0      620 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pied-piper-hat.svg
+-rw-rw-rw-   0        0        0      742 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pied-piper-pp.svg
+-rw-rw-rw-   0        0        0      363 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pied-piper.svg
+-rw-rw-rw-   0        0        0      575 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pinterest-p.svg
+-rw-rw-rw-   0        0        0      709 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pinterest-square.svg
+-rw-rw-rw-   0        0        0      746 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pinterest.svg
+-rw-rw-rw-   0        0        0      674 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/playstation.svg
+-rw-rw-rw-   0        0        0      328 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/product-hunt.svg
+-rw-rw-rw-   0        0        0      543 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pushed.svg
+-rw-rw-rw-   0        0        0      844 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/python.svg
+-rw-rw-rw-   0        0        0      647 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/qq.svg
+-rw-rw-rw-   0        0        0      410 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/quinscape.svg
+-rw-rw-rw-   0        0        0      572 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/quora.svg
+-rw-rw-rw-   0        0        0      625 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/r-project.svg
+-rw-rw-rw-   0        0        0     3819 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/raspberry-pi.svg
+-rw-rw-rw-   0        0        0     1302 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ravelry.svg
+-rw-rw-rw-   0        0        0     2908 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/react.svg
+-rw-rw-rw-   0        0        0     5488 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/reacteurope.svg
+-rw-rw-rw-   0        0        0     1063 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/readme.svg
+-rw-rw-rw-   0        0        0      631 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/rebel.svg
+-rw-rw-rw-   0        0        0      489 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/red-river.svg
+-rw-rw-rw-   0        0        0      926 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/reddit-alien.svg
+-rw-rw-rw-   0        0        0     1037 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/reddit-square.svg
+-rw-rw-rw-   0        0        0      988 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/reddit.svg
+-rw-rw-rw-   0        0        0      643 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/redhat.svg
+-rw-rw-rw-   0        0        0      412 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/renren.svg
+-rw-rw-rw-   0        0        0     1297 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/replyd.svg
+-rw-rw-rw-   0        0        0      812 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/researchgate.svg
+-rw-rw-rw-   0        0        0      553 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/resolving.svg
+-rw-rw-rw-   0        0        0      443 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/rev.svg
+-rw-rw-rw-   0        0        0      938 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/rocketchat.svg
+-rw-rw-rw-   0        0        0      343 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/rockrms.svg
+-rw-rw-rw-   0        0        0     1346 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/safari.svg
+-rw-rw-rw-   0        0        0     4278 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/salesforce.svg
+-rw-rw-rw-   0        0        0     3087 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sass.svg
+-rw-rw-rw-   0        0        0      864 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/schlix.svg
+-rw-rw-rw-   0        0        0      737 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/scribd.svg
+-rw-rw-rw-   0        0        0      757 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/searchengin.svg
+-rw-rw-rw-   0        0        0      830 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sellcast.svg
+-rw-rw-rw-   0        0        0     1210 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sellsy.svg
+-rw-rw-rw-   0        0        0      250 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/servicestack.svg
+-rw-rw-rw-   0        0        0     1588 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/shirtsinbulk.svg
+-rw-rw-rw-   0        0        0      591 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/shopware.svg
+-rw-rw-rw-   0        0        0      533 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/simplybuilt.svg
+-rw-rw-rw-   0        0        0      357 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sistrix.svg
+-rw-rw-rw-   0        0        0      826 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sith.svg
+-rw-rw-rw-   0        0        0      410 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sketch.svg
+-rw-rw-rw-   0        0        0      739 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/skyatlas.svg
+-rw-rw-rw-   0        0        0      785 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/skype.svg
+-rw-rw-rw-   0        0        0      771 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/slack-hash.svg
+-rw-rw-rw-   0        0        0     1069 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/slack.svg
+-rw-rw-rw-   0        0        0      862 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/slideshare.svg
+-rw-rw-rw-   0        0        0     1482 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/snapchat-ghost.svg
+-rw-rw-rw-   0        0        0     1090 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/snapchat-square.svg
+-rw-rw-rw-   0        0        0     1055 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/snapchat.svg
+-rw-rw-rw-   0        0        0     2188 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/soundcloud.svg
+-rw-rw-rw-   0        0        0      334 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sourcetree.svg
+-rw-rw-rw-   0        0        0      635 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/speakap.svg
+-rw-rw-rw-   0        0        0      440 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/speaker-deck.svg
+-rw-rw-rw-   0        0        0      869 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/spotify.svg
+-rw-rw-rw-   0        0        0     1185 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/squarespace.svg
+-rw-rw-rw-   0        0        0      300 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/stack-exchange.svg
+-rw-rw-rw-   0        0        0      299 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/stack-overflow.svg
+-rw-rw-rw-   0        0        0      786 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/stackpath.svg
+-rw-rw-rw-   0        0        0      795 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/staylinked.svg
+-rw-rw-rw-   0        0        0      829 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/steam-square.svg
+-rw-rw-rw-   0        0        0      694 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/steam-symbol.svg
+-rw-rw-rw-   0        0        0      812 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/steam.svg
+-rw-rw-rw-   0        0        0     1635 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sticker-mule.svg
+-rw-rw-rw-   0        0        0      184 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/strava.svg
+-rw-rw-rw-   0        0        0      383 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/stripe-s.svg
+-rw-rw-rw-   0        0        0     1199 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/stripe.svg
+-rw-rw-rw-   0        0        0      567 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/studiovinari.svg
+-rw-rw-rw-   0        0        0      587 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/stumbleupon-circle.svg
+-rw-rw-rw-   0        0        0      498 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/stumbleupon.svg
+-rw-rw-rw-   0        0        0      400 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/superpowers.svg
+-rw-rw-rw-   0        0        0     1712 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/supple.svg
+-rw-rw-rw-   0        0        0     1289 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/suse.svg
+-rw-rw-rw-   0        0        0     1183 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/symfony.svg
+-rw-rw-rw-   0        0        0     1075 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/teamspeak.svg
+-rw-rw-rw-   0        0        0      320 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/telegram-plane.svg
+-rw-rw-rw-   0        0        0      376 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/telegram.svg
+-rw-rw-rw-   0        0        0      496 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/tencent-weibo.svg
+-rw-rw-rw-   0        0        0     6169 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/the-red-yeti.svg
+-rw-rw-rw-   0        0        0      756 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/themeco.svg
+-rw-rw-rw-   0        0        0     3279 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/themeisle.svg
+-rw-rw-rw-   0        0        0      211 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/think-peaks.svg
+-rw-rw-rw-   0        0        0     1378 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/trade-federation.svg
+-rw-rw-rw-   0        0        0      484 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/trello.svg
+-rw-rw-rw-   0        0        0     2012 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/tripadvisor.svg
+-rw-rw-rw-   0        0        0      557 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/tumblr-square.svg
+-rw-rw-rw-   0        0        0      445 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/tumblr.svg
+-rw-rw-rw-   0        0        0      261 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/twitch.svg
+-rw-rw-rw-   0        0        0      671 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/twitter-square.svg
+-rw-rw-rw-   0        0        0      871 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/twitter.svg
+-rw-rw-rw-   0        0        0      402 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/typo3.svg
+-rw-rw-rw-   0        0        0      460 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/uber.svg
+-rw-rw-rw-   0        0        0      949 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ubuntu.svg
+-rw-rw-rw-   0        0        0      235 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/uikit.svg
+-rw-rw-rw-   0        0        0     1048 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/uniregistry.svg
+-rw-rw-rw-   0        0        0     1122 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/untappd.svg
+-rw-rw-rw-   0        0        0      747 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ups.svg
+-rw-rw-rw-   0        0        0      761 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/usb.svg
+-rw-rw-rw-   0        0        0      569 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/usps.svg
+-rw-rw-rw-   0        0        0     3256 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ussunnah.svg
+-rw-rw-rw-   0        0        0      765 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vaadin.svg
+-rw-rw-rw-   0        0        0      236 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/viacoin.svg
+-rw-rw-rw-   0        0        0      885 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/viadeo-square.svg
+-rw-rw-rw-   0        0        0      817 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/viadeo.svg
+-rw-rw-rw-   0        0        0     1457 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/viber.svg
+-rw-rw-rw-   0        0        0      552 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vimeo-square.svg
+-rw-rw-rw-   0        0        0      461 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vimeo-v.svg
+-rw-rw-rw-   0        0        0      575 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vimeo.svg
+-rw-rw-rw-   0        0        0      501 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vine.svg
+-rw-rw-rw-   0        0        0      689 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vk.svg
+-rw-rw-rw-   0        0        0      851 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vnv.svg
+-rw-rw-rw-   0        0        0      200 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vuejs.svg
+-rw-rw-rw-   0        0        0     1053 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/waze.svg
+-rw-rw-rw-   0        0        0     1008 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/weebly.svg
+-rw-rw-rw-   0        0        0     1000 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/weibo.svg
+-rw-rw-rw-   0        0        0      948 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/weixin.svg
+-rw-rw-rw-   0        0        0     1028 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/whatsapp-square.svg
+-rw-rw-rw-   0        0        0      966 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/whatsapp.svg
+-rw-rw-rw-   0        0        0     1258 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/whmcs.svg
+-rw-rw-rw-   0        0        0      777 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wikipedia-w.svg
+-rw-rw-rw-   0        0        0      215 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/windows.svg
+-rw-rw-rw-   0        0        0     1228 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wix.svg
+-rw-rw-rw-   0        0        0     8139 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wizards-of-the-coast.svg
+-rw-rw-rw-   0        0        0     2472 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wolf-pack-battalion.svg
+-rw-rw-rw-   0        0        0      963 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wordpress-simple.svg
+-rw-rw-rw-   0        0        0     1104 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wordpress.svg
+-rw-rw-rw-   0        0        0      578 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wpbeginner.svg
+-rw-rw-rw-   0        0        0      517 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wpexplorer.svg
+-rw-rw-rw-   0        0        0      590 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wpforms.svg
+-rw-rw-rw-   0        0        0     1212 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wpressr.svg
+-rw-rw-rw-   0        0        0      971 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/xbox.svg
+-rw-rw-rw-   0        0        0      550 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/xing-square.svg
+-rw-rw-rw-   0        0        0      459 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/xing.svg
+-rw-rw-rw-   0        0        0      209 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/y-combinator.svg
+-rw-rw-rw-   0        0        0      363 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/yahoo.svg
+-rw-rw-rw-   0        0        0      695 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/yammer.svg
+-rw-rw-rw-   0        0        0      156 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/yandex-international.svg
+-rw-rw-rw-   0        0        0      282 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/yandex.svg
+-rw-rw-rw-   0        0        0     1412 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/yarn.svg
+-rw-rw-rw-   0        0        0      837 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/yelp.svg
+-rw-rw-rw-   0        0        0      520 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/yoast.svg
+-rw-rw-rw-   0        0        0      526 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/youtube-square.svg
+-rw-rw-rw-   0        0        0      550 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/youtube.svg
+-rw-rw-rw-   0        0        0     1544 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/zhihu.svg
+-rw-rw-rw-   0        0        0      601 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/briefcase.svg
+-rw-rw-rw-   0        0        0      999 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brightness.svg
+-rw-rw-rw-   0        0        0      449 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/british-pound.svg
+-rw-rw-rw-   0        0        0      458 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/browser.svg
+-rw-rw-rw-   0        0        0      773 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brush-alt.svg
+-rw-rw-rw-   0        0        0     1163 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brush.svg
+-rw-rw-rw-   0        0        0     1279 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bug.svg
+-rw-rw-rw-   0        0        0      723 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/building.svg
+-rw-rw-rw-   0        0        0      469 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bullhorn.svg
+-rw-rw-rw-   0        0        0     1307 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/burger.svg
+-rw-rw-rw-   0        0        0     1101 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bus-alt.svg
+-rw-rw-rw-   0        0        0      839 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/calculator.svg
+-rw-rw-rw-   0        0        0      597 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/calendar-check.svg
+-rw-rw-rw-   0        0        0     1097 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/calendar.svg
+-rw-rw-rw-   0        0        0      862 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/camera-control.svg
+-rw-rw-rw-   0        0        0     1018 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/camera-roll.svg
+-rw-rw-rw-   0        0        0      867 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/camera.svg
+-rw-rw-rw-   0        0        0     1198 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/car-alt.svg
+-rw-rw-rw-   0        0        0      278 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/caret-bottom.svg
+-rw-rw-rw-   0        0        0      279 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/caret-left.svg
+-rw-rw-rw-   0        0        0      270 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/caret-right.svg
+-rw-rw-rw-   0        0        0      278 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/caret-top.svg
+-rw-rw-rw-   0        0        0      818 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cart.svg
+-rw-rw-rw-   0        0        0     1317 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/casino.svg
+-rw-rw-rw-   0        0        0      632 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cast.svg
+-rw-rw-rw-   0        0        0     1061 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cat.svg
+-rw-rw-rw-   0        0        0      928 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/center-focus.svg
+-rw-rw-rw-   0        0        0      385 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chart-line.svg
+-rw-rw-rw-   0        0        0      966 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chart-pie.svg
+-rw-rw-rw-   0        0        0      843 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chart.svg
+-rw-rw-rw-   0        0        0     1513 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chat-bubble.svg
+-rw-rw-rw-   0        0        0      463 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/check.svg
+-rw-rw-rw-   0        0        0      436 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-bottom.svg
+-rw-rw-rw-   0        0        0      647 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-circle-down-alt.svg
+-rw-rw-rw-   0        0        0      650 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-circle-left-alt.svg
+-rw-rw-rw-   0        0        0      651 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-circle-right-alt.svg
+-rw-rw-rw-   0        0        0      656 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-circle-up-alt.svg
+-rw-rw-rw-   0        0        0      666 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-double-down.svg
+-rw-rw-rw-   0        0        0      600 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-double-left.svg
+-rw-rw-rw-   0        0        0      641 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-double-right.svg
+-rw-rw-rw-   0        0        0      395 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-double-up-alt.svg
+-rw-rw-rw-   0        0        0      674 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-double-up.svg
+-rw-rw-rw-   0        0        0      402 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-left.svg
+-rw-rw-rw-   0        0        0      396 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-right.svg
+-rw-rw-rw-   0        0        0      408 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-top.svg
+-rw-rw-rw-   0        0        0     1154 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/child-friendly.svg
+-rw-rw-rw-   0        0        0     1187 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/child.svg
+-rw-rw-rw-   0        0        0      550 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/circle.svg
+-rw-rw-rw-   0        0        0      328 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/clear-all.svg
+-rw-rw-rw-   0        0        0      577 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/clipboard.svg
+-rw-rw-rw-   0        0        0      488 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/clock.svg
+-rw-rw-rw-   0        0        0      607 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/clone.svg
+-rw-rw-rw-   0        0        0     1287 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/closed-captioning.svg
+-rw-rw-rw-   0        0        0      645 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cloud-download.svg
+-rw-rw-rw-   0        0        0      933 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cloud-upload.svg
+-rw-rw-rw-   0        0        0      819 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cloud.svg
+-rw-rw-rw-   0        0        0     1035 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cloudy.svg
+-rw-rw-rw-   0        0        0      439 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/code.svg
+-rw-rw-rw-   0        0        0      946 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/codepen.svg
+-rw-rw-rw-   0        0        0      605 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/coffee.svg
+-rw-rw-rw-   0        0        0      869 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/color-border.svg
+-rw-rw-rw-   0        0        0     1349 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/color-fill.svg
+-rw-rw-rw-   0        0        0     2109 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/color-palette.svg
+-rw-rw-rw-   0        0        0      452 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/columns.svg
+-rw-rw-rw-   0        0        0      941 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/comment-bubble.svg
+-rw-rw-rw-   0        0        0      397 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/comment-square.svg
+-rw-rw-rw-   0        0        0      875 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/compass.svg
+-rw-rw-rw-   0        0        0      386 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/compress.svg
+-rw-rw-rw-   0        0        0      842 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/contact.svg
+-rw-rw-rw-   0        0        0     1026 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/contrast.svg
+-rw-rw-rw-   0        0        0      383 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/copy.svg
+-rw-rw-rw-   0        0        0      936 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/copyright.svg
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:05.944841 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/coreui/
+-rw-rw-rw-   0        0        0   387926 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/coreui/free-symbol-defs.svg
+-rw-rw-rw-   0        0        0      846 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/couch.svg
+-rw-rw-rw-   0        0        0      521 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/credit-card.svg
+-rw-rw-rw-   0        0        0      663 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/crop-rotate.svg
+-rw-rw-rw-   0        0        0      603 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/crop.svg
+-rw-rw-rw-   0        0        0      855 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cursor-move.svg
+-rw-rw-rw-   0        0        0      407 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cursor.svg
+-rw-rw-rw-   0        0        0      929 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cut.svg
+-rw-rw-rw-   0        0        0      356 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/data-transfer-down.svg
+-rw-rw-rw-   0        0        0      349 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/data-transfer-up.svg
+-rw-rw-rw-   0        0        0     1418 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/deaf.svg
+-rw-rw-rw-   0        0        0      622 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/delete.svg
+-rw-rw-rw-   0        0        0      420 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/description.svg
+-rw-rw-rw-   0        0        0      633 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/devices.svg
+-rw-rw-rw-   0        0        0     2975 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/dialpad.svg
+-rw-rw-rw-   0        0        0      411 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/dinner.svg
+-rw-rw-rw-   0        0        0      924 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/dog.svg
+-rw-rw-rw-   0        0        0      657 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/dollar.svg
+-rw-rw-rw-   0        0        0      321 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/door.svg
+-rw-rw-rw-   0        0        0      383 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/double-quote-sans-left.svg
+-rw-rw-rw-   0        0        0      377 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/double-quote-sans-right.svg
+-rw-rw-rw-   0        0        0      367 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/drink-alcohol.svg
+-rw-rw-rw-   0        0        0      525 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/drink.svg
+-rw-rw-rw-   0        0        0      751 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/drop.svg
+-rw-rw-rw-   0        0        0      770 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/drop1.svg
+-rw-rw-rw-   0        0        0      359 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/elevator.svg
+-rw-rw-rw-   0        0        0      297 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/energy.svg
+-rw-rw-rw-   0        0        0      455 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/envelope-closed.svg
+-rw-rw-rw-   0        0        0      577 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/envelope-letter.svg
+-rw-rw-rw-   0        0        0      503 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/envelope-open.svg
+-rw-rw-rw-   0        0        0     1148 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/equalizer.svg
+-rw-rw-rw-   0        0        0      523 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/ethernet.svg
+-rw-rw-rw-   0        0        0      602 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/euro.svg
+-rw-rw-rw-   0        0        0      526 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/excerpt.svg
+-rw-rw-rw-   0        0        0      532 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/exit-to-app.svg
+-rw-rw-rw-   0        0        0      388 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/expand-down.svg
+-rw-rw-rw-   0        0        0      382 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/expand-left.svg
+-rw-rw-rw-   0        0        0      396 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/expand-right.svg
+-rw-rw-rw-   0        0        0      388 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/expand-up.svg
+-rw-rw-rw-   0        0        0      577 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/exposure.svg
+-rw-rw-rw-   0        0        0      355 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/external-link.svg
+-rw-rw-rw-   0        0        0      924 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/eye.svg
+-rw-rw-rw-   0        0        0     1052 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/eyedropper.svg
+-rw-rw-rw-   0        0        0      934 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/face-dead.svg
+-rw-rw-rw-   0        0        0      880 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/face.svg
+-rw-rw-rw-   0        0        0      678 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/facebook.svg
+-rw-rw-rw-   0        0        0      729 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fastfood.svg
+-rw-rw-rw-   0        0        0      899 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fax.svg
+-rw-rw-rw-   0        0        0      606 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/featured-playlist.svg
+-rw-rw-rw-   0        0        0      305 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/file.svg
+-rw-rw-rw-   0        0        0      532 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/filter-frames.svg
+-rw-rw-rw-   0        0        0      809 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/filter-photo.svg
+-rw-rw-rw-   0        0        0      331 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/filter.svg
+-rw-rw-rw-   0        0        0      731 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/find-in-page.svg
+-rw-rw-rw-   0        0        0     2035 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fingerprint.svg
+-rw-rw-rw-   0        0        0     1623 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fire.svg
+-rw-rw-rw-   0        0        0      312 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/flag-alt.svg
+-rw-rw-rw-   0        0        0     1190 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/flight-takeoff.svg
+-rw-rw-rw-   0        0        0     1606 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/flip-to-back.svg
+-rw-rw-rw-   0        0        0     1088 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/flip-to-front.svg
+-rw-rw-rw-   0        0        0      926 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/flip.svg
+-rw-rw-rw-   0        0        0     2522 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/flower.svg
+-rw-rw-rw-   0        0        0      719 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/folder-open.svg
+-rw-rw-rw-   0        0        0      499 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/folder.svg
+-rw-rw-rw-   0        0        0      367 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/font.svg
+-rw-rw-rw-   0        0        0     1357 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/football.svg
+-rw-rw-rw-   0        0        0     1163 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fork.svg
+-rw-rw-rw-   0        0        0      582 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fridge.svg
+-rw-rw-rw-   0        0        0      810 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/frown.svg
+-rw-rw-rw-   0        0        0      370 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fullscreen-exit.svg
+-rw-rw-rw-   0        0        0      357 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fullscreen.svg
+-rw-rw-rw-   0        0        0      313 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/functions-alt.svg
+-rw-rw-rw-   0        0        0      896 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/functions.svg
+-rw-rw-rw-   0        0        0     1230 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/gamepad.svg
+-rw-rw-rw-   0        0        0     1067 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/garage.svg
+-rw-rw-rw-   0        0        0      504 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/gem.svg
+-rw-rw-rw-   0        0        0      445 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/gif.svg
+-rw-rw-rw-   0        0        0      934 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/gift.svg
+-rw-rw-rw-   0        0        0     1125 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/git.svg
+-rw-rw-rw-   0        0        0     2036 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/github-circle.svg
+-rw-rw-rw-   0        0        0     1908 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/github.svg
+-rw-rw-rw-   0        0        0     1192 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/gitlab.svg
+-rw-rw-rw-   0        0        0     1249 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/globe-alt.svg
+-rw-rw-rw-   0        0        0     1061 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/golf-alt.svg
+-rw-rw-rw-   0        0        0     1034 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/golf.svg
+-rw-rw-rw-   0        0        0      948 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/gradient.svg
+-rw-rw-rw-   0        0        0     2581 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/grain.svg
+-rw-rw-rw-   0        0        0     1510 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/graph.svg
+-rw-rw-rw-   0        0        0      726 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/grid-slash.svg
+-rw-rw-rw-   0        0        0      651 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/grid.svg
+-rw-rw-rw-   0        0        0      809 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hand-point-down.svg
+-rw-rw-rw-   0        0        0      841 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hand-point-left.svg
+-rw-rw-rw-   0        0        0      824 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hand-point-right.svg
+-rw-rw-rw-   0        0        0      811 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hand-point-up.svg
+-rw-rw-rw-   0        0        0      693 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hd.svg
+-rw-rw-rw-   0        0        0      582 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hdr.svg
+-rw-rw-rw-   0        0        0      389 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/header.svg
+-rw-rw-rw-   0        0        0      730 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/headphones.svg
+-rw-rw-rw-   0        0        0     1751 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/healing.svg
+-rw-rw-rw-   0        0        0      909 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/heart.svg
+-rw-rw-rw-   0        0        0      849 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/highlighter.svg
+-rw-rw-rw-   0        0        0      520 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/highligt.svg
+-rw-rw-rw-   0        0        0      643 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/history.svg
+-rw-rw-rw-   0        0        0      533 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/home.svg
+-rw-rw-rw-   0        0        0      603 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hospital.svg
+-rw-rw-rw-   0        0        0     1763 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hot-tub.svg
+-rw-rw-rw-   0        0        0      561 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/house.svg
+-rw-rw-rw-   0        0        0      593 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/https.svg
+-rw-rw-rw-   0        0        0      511 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/image-broken.svg
+-rw-rw-rw-   0        0        0      487 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/image-plus.svg
+-rw-rw-rw-   0        0        0      397 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/image1.svg
+-rw-rw-rw-   0        0        0      322 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/inbox.svg
+-rw-rw-rw-   0        0        0      541 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/indent-decrease.svg
+-rw-rw-rw-   0        0        0      538 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/indent-increase.svg
+-rw-rw-rw-   0        0        0      794 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/industry-slash.svg
+-rw-rw-rw-   0        0        0      794 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/industry.svg
+-rw-rw-rw-   0        0        0      877 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/infinity.svg
+-rw-rw-rw-   0        0        0      880 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/info.svg
+-rw-rw-rw-   0        0        0      447 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/input-hdmi.svg
+-rw-rw-rw-   0        0        0      362 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/input-power.svg
+-rw-rw-rw-   0        0        0      536 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/input.svg
+-rw-rw-rw-   0        0        0     1012 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/instagram.svg
+-rw-rw-rw-   0        0        0      568 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/institution.svg
+-rw-rw-rw-   0        0        0      351 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/italic.svg
+-rw-rw-rw-   0        0        0      423 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/justify-center.svg
+-rw-rw-rw-   0        0        0      422 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/justify-left.svg
+-rw-rw-rw-   0        0        0      423 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/justify-right.svg
+-rw-rw-rw-   0        0        0     1151 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/keyboard.svg
+-rw-rw-rw-   0        0        0      838 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/lan.svg
+-rw-rw-rw-   0        0        0      998 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/language.svg
+-rw-rw-rw-   0        0        0      450 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/laptop.svg
+-rw-rw-rw-   0        0        0      895 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/layers.svg
+-rw-rw-rw-   0        0        0      884 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/leaf.svg
+-rw-rw-rw-   0        0        0     1769 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/lemon.svg
+-rw-rw-rw-   0        0        0      301 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/level-down.svg
+-rw-rw-rw-   0        0        0      298 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/level-up.svg
+-rw-rw-rw-   0        0        0      699 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/library-add.svg
+-rw-rw-rw-   0        0        0      578 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/library.svg
+-rw-rw-rw-   0        0        0     1247 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/life-ring.svg
+-rw-rw-rw-   0        0        0      825 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/lightbulb.svg
+-rw-rw-rw-   0        0        0      557 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/line-spacing.svg
+-rw-rw-rw-   0        0        0     1961 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/line-style.svg
+-rw-rw-rw-   0        0        0      442 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/line-weight.svg
+-rw-rw-rw-   0        0        0      573 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/link-alt.svg
+-rw-rw-rw-   0        0        0      977 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/link-broken.svg
+-rw-rw-rw-   0        0        0      842 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/link.svg
+-rw-rw-rw-   0        0        0      988 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/linkedin.svg
+-rw-rw-rw-   0        0        0      369 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/list-filter.svg
+-rw-rw-rw-   0        0        0      704 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/list-high-priority.svg
+-rw-rw-rw-   0        0        0      700 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/list-low-priority.svg
+-rw-rw-rw-   0        0        0      589 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/list-numbered.svg
+-rw-rw-rw-   0        0        0      701 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/list-rich.svg
+-rw-rw-rw-   0        0        0     1040 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/list.svg
+-rw-rw-rw-   0        0        0      902 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/location-pin.svg
+-rw-rw-rw-   0        0        0      461 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/lock-locked.svg
+-rw-rw-rw-   0        0        0      503 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/lock-unlocked.svg
+-rw-rw-rw-   0        0        0     1802 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/locomotive.svg
+-rw-rw-rw-   0        0        0      653 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/loop-1.svg
+-rw-rw-rw-   0        0        0      693 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/loop-circular.svg
+-rw-rw-rw-   0        0        0      554 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/loop.svg
+-rw-rw-rw-   0        0        0     1171 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/low-vision.svg
+-rw-rw-rw-   0        0        0      851 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/magnifying-glass.svg
+-rw-rw-rw-   0        0        0      657 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/map.svg
+-rw-rw-rw-   0        0        0      699 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-eject.svg
+-rw-rw-rw-   0        0        0      598 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-pause.svg
+-rw-rw-rw-   0        0        0      506 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-play.svg
+-rw-rw-rw-   0        0        0      421 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-record.svg
+-rw-rw-rw-   0        0        0      728 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-skip-backward.svg
+-rw-rw-rw-   0        0        0      711 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-skip-forward.svg
+-rw-rw-rw-   0        0        0      633 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-step-backward.svg
+-rw-rw-rw-   0        0        0      557 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-step-forward.svg
+-rw-rw-rw-   0        0        0      393 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-stop.svg
+-rw-rw-rw-   0        0        0      352 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/medical-cross.svg
+-rw-rw-rw-   0        0        0      685 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/meh.svg
+-rw-rw-rw-   0        0        0      478 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/memory.svg
+-rw-rw-rw-   0        0        0      313 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/menu.svg
+-rw-rw-rw-   0        0        0      600 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/microphone.svg
+-rw-rw-rw-   0        0        0      218 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/minus.svg
+-rw-rw-rw-   0        0        0      437 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mobile-landscape.svg
+-rw-rw-rw-   0        0        0      502 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mobile.svg
+-rw-rw-rw-   0        0        0      660 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/money.svg
+-rw-rw-rw-   0        0        0      507 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/monitor.svg
+-rw-rw-rw-   0        0        0      745 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mood-bad.svg
+-rw-rw-rw-   0        0        0      742 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mood-good.svg
+-rw-rw-rw-   0        0        0      783 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mood-very-bad.svg
+-rw-rw-rw-   0        0        0      832 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mood-very-good.svg
+-rw-rw-rw-   0        0        0     1209 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/moon.svg
+-rw-rw-rw-   0        0        0      739 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mouse.svg
+-rw-rw-rw-   0        0        0     1948 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mouth-slash.svg
+-rw-rw-rw-   0        0        0      539 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/move.svg
+-rw-rw-rw-   0        0        0      680 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/movie.svg
+-rw-rw-rw-   0        0        0      840 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mug-tea.svg
+-rw-rw-rw-   0        0        0      725 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mug.svg
+-rw-rw-rw-   0        0        0      553 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/music-note.svg
+-rw-rw-rw-   0        0        0      753 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/newspaper.svg
+-rw-rw-rw-   0        0        0      389 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/notes.svg
+-rw-rw-rw-   0        0        0      601 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/object-group.svg
+-rw-rw-rw-   0        0        0      703 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/object-ungroup.svg
+-rw-rw-rw-   0        0        0     2037 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/opacity.svg
+-rw-rw-rw-   0        0        0      870 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/options-horizontal.svg
+-rw-rw-rw-   0        0        0      864 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/options.svg
+-rw-rw-rw-   0        0        0     1203 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/paint-bucket.svg
+-rw-rw-rw-   0        0        0      678 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/paint.svg
+-rw-rw-rw-   0        0        0      507 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/paper-plane.svg
+-rw-rw-rw-   0        0        0      945 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/paperclip.svg
+-rw-rw-rw-   0        0        0      355 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/paragraph.svg
+-rw-rw-rw-   0        0        0     3241 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/paw.svg
+-rw-rw-rw-   0        0        0     1072 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pen-alt.svg
+-rw-rw-rw-   0        0        0     1159 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pen-nib.svg
+-rw-rw-rw-   0        0        0      749 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pencil.svg
+-rw-rw-rw-   0        0        0     1520 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/people.svg
+-rw-rw-rw-   0        0        0      698 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/phone.svg
+-rw-rw-rw-   0        0        0     1266 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pin.svg
+-rw-rw-rw-   0        0        0     1457 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pizza.svg
+-rw-rw-rw-   0        0        0      389 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/playlist-add.svg
+-rw-rw-rw-   0        0        0      266 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/plus.svg
+-rw-rw-rw-   0        0        0      498 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/polymer.svg
+-rw-rw-rw-   0        0        0     2383 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pool.svg
+-rw-rw-rw-   0        0        0      509 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/power-standby.svg
+-rw-rw-rw-   0        0        0      734 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pregnant.svg
+-rw-rw-rw-   0        0        0      615 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/print.svg
+-rw-rw-rw-   0        0        0     1426 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/puzzle.svg
+-rw-rw-rw-   0        0        0      999 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/qr-code.svg
+-rw-rw-rw-   0        0        0     1127 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/rain.svg
+-rw-rw-rw-   0        0        0     3362 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/react.svg
+-rw-rw-rw-   0        0        0      395 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/rectangle.svg
+-rw-rw-rw-   0        0        0     1682 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/reddit.svg
+-rw-rw-rw-   0        0        0      895 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/registered.svg
+-rw-rw-rw-   0        0        0      464 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/reload.svg
+-rw-rw-rw-   0        0        0      426 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/resize-both.svg
+-rw-rw-rw-   0        0        0      398 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/resize-height.svg
+-rw-rw-rw-   0        0        0      392 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/resize-width.svg
+-rw-rw-rw-   0        0        0      618 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/restaurant.svg
+-rw-rw-rw-   0        0        0      389 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/room.svg
+-rw-rw-rw-   0        0        0      894 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/rowing.svg
+-rw-rw-rw-   0        0        0      958 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/rss.svg
+-rw-rw-rw-   0        0        0     1038 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/running.svg
+-rw-rw-rw-   0        0        0      605 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/satelite.svg
+-rw-rw-rw-   0        0        0      848 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/save.svg
+-rw-rw-rw-   0        0        0      422 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/school.svg
+-rw-rw-rw-   0        0        0      457 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/screen-desktop.svg
+-rw-rw-rw-   0        0        0      509 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/screen-smartphone.svg
+-rw-rw-rw-   0        0        0      756 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/scrubber.svg
+-rw-rw-rw-   0        0        0     2637 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/settings.svg
+-rw-rw-rw-   0        0        0      759 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/share-all.svg
+-rw-rw-rw-   0        0        0     1248 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/share-alt.svg
+-rw-rw-rw-   0        0        0      783 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/share-boxed.svg
+-rw-rw-rw-   0        0        0      666 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/share.svg
+-rw-rw-rw-   0        0        0      952 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/shield-alt.svg
+-rw-rw-rw-   0        0        0      336 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/short-text.svg
+-rw-rw-rw-   0        0        0     1423 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/shower.svg
+-rw-rw-rw-   0        0        0     1927 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sign-language.svg
+-rw-rw-rw-   0        0        0      275 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/signal-cellular-0.svg
+-rw-rw-rw-   0        0        0      401 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/signal-cellular-3.svg
+-rw-rw-rw-   0        0        0      447 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/signal-cellular-4.svg
+-rw-rw-rw-   0        0        0      574 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sim.svg
+-rw-rw-rw-   0        0        0     1156 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sitemap.svg
+-rw-rw-rw-   0        0        0     2021 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/skype.svg
+-rw-rw-rw-   0        0        0      948 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/smile-plus.svg
+-rw-rw-rw-   0        0        0      943 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/smile.svg
+-rw-rw-rw-   0        0        0     1284 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/smoke-free.svg
+-rw-rw-rw-   0        0        0     1199 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/smoking-room.svg
+-rw-rw-rw-   0        0        0      727 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/snowflake.svg
+-rw-rw-rw-   0        0        0      537 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sort-alpha-down.svg
+-rw-rw-rw-   0        0        0      531 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sort-alpha-up.svg
+-rw-rw-rw-   0        0        0      521 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sort-ascending.svg
+-rw-rw-rw-   0        0        0      523 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sort-descending.svg
+-rw-rw-rw-   0        0        0      914 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sort-numeric-down.svg
+-rw-rw-rw-   0        0        0      905 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sort-numeric-up.svg
+-rw-rw-rw-   0        0        0      924 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/spa.svg
+-rw-rw-rw-   0        0        0      236 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/space-bar.svg
+-rw-rw-rw-   0        0        0      864 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/speaker.svg
+-rw-rw-rw-   0        0        0      582 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/speech.svg
+-rw-rw-rw-   0        0        0     1007 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/speedometer.svg
+-rw-rw-rw-   0        0        0     1513 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/spotify.svg
+-rw-rw-rw-   0        0        0      891 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/spreadsheet.svg
+-rw-rw-rw-   0        0        0      402 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/square.svg
+-rw-rw-rw-   0        0        0      632 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/stackoverflow.svg
+-rw-rw-rw-   0        0        0      763 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/star-half.svg
+-rw-rw-rw-   0        0        0     1385 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/star.svg
+-rw-rw-rw-   0        0        0      444 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/storage.svg
+-rw-rw-rw-   0        0        0      324 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/stream.svg
+-rw-rw-rw-   0        0        0      929 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sun.svg
+-rw-rw-rw-   0        0        0      427 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/swap-horizontal.svg
+-rw-rw-rw-   0        0        0      420 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/swap-vertical.svg
+-rw-rw-rw-   0        0        0     3156 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/swimming.svg
+-rw-rw-rw-   0        0        0      672 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sync.svg
+-rw-rw-rw-   0        0        0      486 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/tablet.svg
+-rw-rw-rw-   0        0        0      980 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/tag.svg
+-rw-rw-rw-   0        0        0     1467 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/tags.svg
+-rw-rw-rw-   0        0        0      519 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/task.svg
+-rw-rw-rw-   0        0        0      654 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/taxi.svg
+-rw-rw-rw-   0        0        0     1168 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/tennis-ball.svg
+-rw-rw-rw-   0        0        0     1726 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/tennis.svg
+-rw-rw-rw-   0        0        0      560 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/terminal.svg
+-rw-rw-rw-   0        0        0      394 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/terrain.svg
+-rw-rw-rw-   0        0        0      633 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/text-shapes.svg
+-rw-rw-rw-   0        0        0      392 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/text-size.svg
+-rw-rw-rw-   0        0        0      347 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/text-square.svg
+-rw-rw-rw-   0        0        0      910 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/text-strike.svg
+-rw-rw-rw-   0        0        0      283 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/text.svg
+-rw-rw-rw-   0        0        0     1339 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/thumb-down.svg
+-rw-rw-rw-   0        0        0     1305 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/thumb-up.svg
+-rw-rw-rw-   0        0        0      630 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/toggle-off.svg
+-rw-rw-rw-   0        0        0      676 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/toilet.svg
+-rw-rw-rw-   0        0        0     1064 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/touch-app.svg
+-rw-rw-rw-   0        0        0      396 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/trademark.svg
+-rw-rw-rw-   0        0        0      417 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/transfer.svg
+-rw-rw-rw-   0        0        0      861 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/translate.svg
+-rw-rw-rw-   0        0        0      684 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/trash.svg
+-rw-rw-rw-   0        0        0      490 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/triangle.svg
+-rw-rw-rw-   0        0        0     1125 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/truck.svg
+-rw-rw-rw-   0        0        0      511 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/tv.svg
+-rw-rw-rw-   0        0        0     1289 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/twitter.svg
+-rw-rw-rw-   0        0        0      531 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/underline.svg
+-rw-rw-rw-   0        0        0     1157 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/user-female.svg
+-rw-rw-rw-   0        0        0      850 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/user-follow.svg
+-rw-rw-rw-   0        0        0      970 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/user-unfollow.svg
+-rw-rw-rw-   0        0        0      897 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/user.svg
+-rw-rw-rw-   0        0        0     1691 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/vector.svg
+-rw-rw-rw-   0        0        0      360 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/vertical-align-bottom.svg
+-rw-rw-rw-   0        0        0      444 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/vertical-align-bottom1.svg
+-rw-rw-rw-   0        0        0      480 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/vertical-align-center.svg
+-rw-rw-rw-   0        0        0      593 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/vertical-align-center1.svg
+-rw-rw-rw-   0        0        0      351 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/vertical-align-top.svg
+-rw-rw-rw-   0        0        0      423 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/vertical-align-top1.svg
+-rw-rw-rw-   0        0        0      343 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/video.svg
+-rw-rw-rw-   0        0        0      278 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/view-column.svg
+-rw-rw-rw-   0        0        0      366 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/view-module.svg
+-rw-rw-rw-   0        0        0      321 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/view-quilt.svg
+-rw-rw-rw-   0        0        0      264 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/view-stream.svg
+-rw-rw-rw-   0        0        0     1333 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/voice-over-record.svg
+-rw-rw-rw-   0        0        0      647 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/volume-high.svg
+-rw-rw-rw-   0        0        0      468 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/volume-low.svg
+-rw-rw-rw-   0        0        0      491 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/volume-off.svg
+-rw-rw-rw-   0        0        0      396 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/vue.svg
+-rw-rw-rw-   0        0        0      647 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/walk.svg
+-rw-rw-rw-   0        0        0      691 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wallet.svg
+-rw-rw-rw-   0        0        0      610 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wallpaper.svg
+-rw-rw-rw-   0        0        0      386 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/warning.svg
+-rw-rw-rw-   0        0        0      770 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/watch.svg
+-rw-rw-rw-   0        0        0     1318 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wc.svg
+-rw-rw-rw-   0        0        0      674 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/weightlifitng.svg
+-rw-rw-rw-   0        0        0      884 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wheelchair.svg
+-rw-rw-rw-   0        0        0      512 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wifi-signal-0.svg
+-rw-rw-rw-   0        0        0      681 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wifi-signal-1.svg
+-rw-rw-rw-   0        0        0      765 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wifi-signal-2.svg
+-rw-rw-rw-   0        0        0      781 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wifi-signal-4.svg
+-rw-rw-rw-   0        0        0      753 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wifi-signal-off.svg
+-rw-rw-rw-   0        0        0      454 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/window-maximize.svg
+-rw-rw-rw-   0        0        0      222 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/window-minimize.svg
+-rw-rw-rw-   0        0        0      650 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/window-restore.svg
+-rw-rw-rw-   0        0        0      406 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/window.svg
+-rw-rw-rw-   0        0        0      515 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wrap-text.svg
+-rw-rw-rw-   0        0        0      687 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/x-circle.svg
+-rw-rw-rw-   0        0        0      322 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/x.svg
+-rw-rw-rw-   0        0        0      367 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/yen.svg
+-rw-rw-rw-   0        0        0      939 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/zoom-in.svg
+-rw-rw-rw-   0        0        0      892 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/zoom-out.svg
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:05.961583 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:05.977642 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/
+-rw-rw-rw-   0        0        0    13887 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/1.jpg
+-rw-rw-rw-   0        0        0    12870 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/2.jpg
+-rw-rw-rw-   0        0        0    13528 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/3.jpg
+-rw-rw-rw-   0        0        0    13725 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/4.jpg
+-rw-rw-rw-   0        0        0    12666 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/5.jpg
+-rw-rw-rw-   0        0        0    11918 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/6.jpg
+-rw-rw-rw-   0        0        0    14285 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/7.jpg
+-rw-rw-rw-   0        0        0    15146 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/8.jpg
+-rw-rw-rw-   0        0        0    12451 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/9.jpg
+-rw-rw-rw-   0        0        0   362060 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/background-pro-yellow.jpg
+-rw-rw-rw-   0        0        0   319788 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/background-pro.jpg
+-rw-rw-rw-   0        0        0   290033 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/full.jpg
+-rw-rw-rw-   0        0        0     1095 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/icon-calendar.svg
+-rw-rw-rw-   0        0        0      686 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/icon-clock.svg
+-rw-rw-rw-   0        0        0      658 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/icon-unknown-alt.svg
+-rw-rw-rw-   0        0        0      658 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/icon-unknown.svg
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:05.979649 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/icons/
+-rw-rw-rw-   0        0        0     1040 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/icons/add.svg
+-rw-rw-rw-   0        0        0      461 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/search.svg
+-rw-rw-rw-   0        0        0     3325 2024-04-28 06:02:42.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/img/selector-icons.svg
+-rw-rw-rw-   0        0        0   435188 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/package-lock.json
+-rw-rw-rw-   0        0        0     5309 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/assets/package.json
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.003299 django-admin-coreui-0.0.6/admin_coreui/static/css/
+-rw-rw-rw-   0        0        0     1324 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/ads.css
+-rw-rw-rw-   0        0        0    16388 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/ads.css.map
+-rw-rw-rw-   0        0        0     1099 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/ads.min.css
+-rw-rw-rw-   0        0        0    15001 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/ads.min.css.map
+-rw-rw-rw-   0        0        0     1924 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/examples.css
+-rw-rw-rw-   0        0        0     9564 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/examples.css.map
+-rw-rw-rw-   0        0        0     1437 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/examples.min.css
+-rw-rw-rw-   0        0        0     9482 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/examples.min.css.map
+-rw-rw-rw-   0        0        0    22248 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/icons.css
+-rw-rw-rw-   0        0        0   361904 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/style.css
+-rw-rw-rw-   0        0        0   833191 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/style.css.map
+-rw-rw-rw-   0        0        0   293400 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/style.min.css
+-rw-rw-rw-   0        0        0   728464 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/style.min.css.map
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.007307 django-admin-coreui-0.0.6/admin_coreui/static/css/vendors/
+-rw-rw-rw-   0        0        0      136 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/vendors/simplebar.css
+-rw-rw-rw-   0        0        0      264 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/css/vendors/simplebar.css.map
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.039404 django-admin-coreui-0.0.6/admin_coreui/static/js/
+-rw-rw-rw-   0        0        0     4721 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/charts.js
+-rw-rw-rw-   0        0        0     9093 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/charts.js.map
+-rw-rw-rw-   0        0        0     2325 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/color-modes.js
+-rw-rw-rw-   0        0        0     4760 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/color-modes.js.map
+-rw-rw-rw-   0        0        0     1027 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/colors.js
+-rw-rw-rw-   0        0        0     1819 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/colors.js.map
+-rw-rw-rw-   0        0        0      671 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/config.js
+-rw-rw-rw-   0        0        0     1309 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/config.js.map
+-rw-rw-rw-   0        0        0     8323 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/main.js
+-rw-rw-rw-   0        0        0    17712 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/main.js.map
+-rw-rw-rw-   0        0        0      541 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/popovers.js
+-rw-rw-rw-   0        0        0      860 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/popovers.js.map
+-rw-rw-rw-   0        0        0      660 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/toasts.js
+-rw-rw-rw-   0        0        0     1192 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/toasts.js.map
+-rw-rw-rw-   0        0        0      541 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/tooltips.js
+-rw-rw-rw-   0        0        0      858 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/tooltips.js.map
+-rw-rw-rw-   0        0        0    14513 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/widgets.js
+-rw-rw-rw-   0        0        0    27525 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/js/widgets.js.map
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.674531 django-admin-coreui-0.0.6/admin_coreui/static/vendors/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.672554 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.667576 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/chartjs/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.042443 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/chartjs/css/
+-rw-rw-rw-   0        0        0     1931 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/chartjs/css/coreui-chartjs.css
+-rw-rw-rw-   0        0        0     8155 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/chartjs/css/coreui-chartjs.css.map
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.045407 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/chartjs/js/
+-rw-rw-rw-   0        0        0     4690 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/chartjs/js/coreui-chartjs.js
+-rw-rw-rw-   0        0        0     9081 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/chartjs/js/coreui-chartjs.js.map
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.668549 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/coreui/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.048925 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/coreui/js/
+-rw-rw-rw-   0        0        0    88068 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/coreui/js/coreui.bundle.min.js
+-rw-rw-rw-   0        0        0   362032 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/coreui/js/coreui.bundle.min.js.map
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.670533 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.176452 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/
+-rw-rw-rw-   0        0        0    31612 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/brand.min.css
+-rw-rw-rw-   0        0        0    15076 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/brand.min.css.map
+-rw-rw-rw-   0        0        0    10975 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/flag.min.css
+-rw-rw-rw-   0        0        0     4360 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/flag.min.css.map
+-rw-rw-rw-   0        0        0    22248 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/free.min.css
+-rw-rw-rw-   0        0        0    10703 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/free.min.css.map
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.197282 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/
+-rw-rw-rw-   0        0        0   522960 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.eot
+-rw-rw-rw-   0        0        0  3405774 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.svg
+-rw-rw-rw-   0        0        0   522752 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.ttf
+-rw-rw-rw-   0        0        0   378328 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.woff
+-rw-rw-rw-   0        0        0   146944 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.eot
+-rw-rw-rw-   0        0        0   561928 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.svg
+-rw-rw-rw-   0        0        0   146740 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.ttf
+-rw-rw-rw-   0        0        0    78996 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.woff
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.211146 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/
+-rw-rw-rw-   0        0        0  1456471 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/brand.svg
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.565294 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/
+-rw-rw-rw-   0        0        0    69248 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ad.svg
+-rw-rw-rw-   0        0        0      321 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ae.svg
+-rw-rw-rw-   0        0        0    52644 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-af.svg
+-rw-rw-rw-   0        0        0      617 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ag.svg
+-rw-rw-rw-   0        0        0     9013 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-al.svg
+-rw-rw-rw-   0        0        0      279 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-am.svg
+-rw-rw-rw-   0        0        0     2556 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ao.svg
+-rw-rw-rw-   0        0        0    11535 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ar.svg
+-rw-rw-rw-   0        0        0      229 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-at.svg
+-rw-rw-rw-   0        0        0     2078 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-au.svg
+-rw-rw-rw-   0        0        0      620 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-az.svg
+-rw-rw-rw-   0        0        0     1197 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ba.svg
+-rw-rw-rw-   0        0        0     1068 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bb.svg
+-rw-rw-rw-   0        0        0      232 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bd.svg
+-rw-rw-rw-   0        0        0      281 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-be.svg
+-rw-rw-rw-   0        0        0      390 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bf.svg
+-rw-rw-rw-   0        0        0      277 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bg.svg
+-rw-rw-rw-   0        0        0      280 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bh.svg
+-rw-rw-rw-   0        0        0     1669 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bi.svg
+-rw-rw-rw-   0        0        0      278 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bj.svg
+-rw-rw-rw-   0        0        0    26617 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bn.svg
+-rw-rw-rw-   0        0        0      291 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bo.svg
+-rw-rw-rw-   0        0        0     8293 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-br.svg
+-rw-rw-rw-   0        0        0      273 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bs.svg
+-rw-rw-rw-   0        0        0    41412 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bt.svg
+-rw-rw-rw-   0        0        0      278 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bw.svg
+-rw-rw-rw-   0        0        0     8608 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-by.svg
+-rw-rw-rw-   0        0        0   107351 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bz.svg
+-rw-rw-rw-   0        0        0     1034 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ca.svg
+-rw-rw-rw-   0        0        0      405 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cd.svg
+-rw-rw-rw-   0        0        0      532 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cf.svg
+-rw-rw-rw-   0        0        0      284 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cg.svg
+-rw-rw-rw-   0        0        0      297 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ch.svg
+-rw-rw-rw-   0        0        0      276 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ci.svg
+-rw-rw-rw-   0        0        0     5532 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ck.svg
+-rw-rw-rw-   0        0        0      445 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cl.svg
+-rw-rw-rw-   0        0        0      412 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cm.svg
+-rw-rw-rw-   0        0        0      529 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cn.svg
+-rw-rw-rw-   0        0        0      280 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-co.svg
+-rw-rw-rw-   0        0        0      276 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cr.svg
+-rw-rw-rw-   0        0        0      438 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cu.svg
+-rw-rw-rw-   0        0        0     1529 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cv.svg
+-rw-rw-rw-   0        0        0    13897 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cy.svg
+-rw-rw-rw-   0        0        0      276 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cz.svg
+-rw-rw-rw-   0        0        0      274 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-de.svg
+-rw-rw-rw-   0        0        0      451 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-dj.svg
+-rw-rw-rw-   0        0        0      293 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-dk.svg
+-rw-rw-rw-   0        0        0    15792 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-dm.svg
+-rw-rw-rw-   0        0        0   179774 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-do.svg
+-rw-rw-rw-   0        0        0      879 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-dz.svg
+-rw-rw-rw-   0        0        0   295696 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ec.svg
+-rw-rw-rw-   0        0        0      284 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ee.svg
+-rw-rw-rw-   0        0        0    25811 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-eg.svg
+-rw-rw-rw-   0        0        0     4464 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-er.svg
+-rw-rw-rw-   0        0        0   142496 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-es.svg
+-rw-rw-rw-   0        0        0     1145 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-et.svg
+-rw-rw-rw-   0        0        0      289 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-fi.svg
+-rw-rw-rw-   0        0        0   109829 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-fj.svg
+-rw-rw-rw-   0        0        0      678 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-fm.svg
+-rw-rw-rw-   0        0        0      271 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-fr.svg
+-rw-rw-rw-   0        0        0      273 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ga.svg
+-rw-rw-rw-   0        0        0      771 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gb.svg
+-rw-rw-rw-   0        0        0     1527 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gd.svg
+-rw-rw-rw-   0        0        0     1396 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ge.svg
+-rw-rw-rw-   0        0        0      367 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gh.svg
+-rw-rw-rw-   0        0        0      348 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gm.svg
+-rw-rw-rw-   0        0        0     9364 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gn.svg
+-rw-rw-rw-   0        0        0     9364 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gq.svg
+-rw-rw-rw-   0        0        0      365 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gr.svg
+-rw-rw-rw-   0        0        0    99692 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gt.svg
+-rw-rw-rw-   0        0        0      441 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gw.svg
+-rw-rw-rw-   0        0        0      395 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gy.svg
+-rw-rw-rw-   0        0        0     3046 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hk.svg
+-rw-rw-rw-   0        0        0      854 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hn.svg
+-rw-rw-rw-   0        0        0   119564 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hr.svg
+-rw-rw-rw-   0        0        0    40443 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ht.svg
+-rw-rw-rw-   0        0        0      275 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hu.svg
+-rw-rw-rw-   0        0        0      225 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-id.svg
+-rw-rw-rw-   0        0        0      281 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ie.svg
+-rw-rw-rw-   0        0        0      446 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-il.svg
+-rw-rw-rw-   0        0        0     3887 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-in.svg
+-rw-rw-rw-   0        0        0     3580 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-iq.svg
+-rw-rw-rw-   0        0        0     5234 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ir.svg
+-rw-rw-rw-   0        0        0      308 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-is.svg
+-rw-rw-rw-   0        0        0      281 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-it.svg
+-rw-rw-rw-   0        0        0      536 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-jm.svg
+-rw-rw-rw-   0        0        0      521 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-jo.svg
+-rw-rw-rw-   0        0        0      230 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-jp.svg
+-rw-rw-rw-   0        0        0     1932 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ke.svg
+-rw-rw-rw-   0        0        0    10437 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kg.svg
+-rw-rw-rw-   0        0        0    20460 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kh.svg
+-rw-rw-rw-   0        0        0     4811 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ki.svg
+-rw-rw-rw-   0        0        0      976 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-km.svg
+-rw-rw-rw-   0        0        0     1116 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kn.svg
+-rw-rw-rw-   0        0        0      495 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kp.svg
+-rw-rw-rw-   0        0        0     1765 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kr.svg
+-rw-rw-rw-   0        0        0      327 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kw.svg
+-rw-rw-rw-   0        0        0    31510 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kz.svg
+-rw-rw-rw-   0        0        0      283 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-la.svg
+-rw-rw-rw-   0        0        0     9268 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lb.svg
+-rw-rw-rw-   0        0        0      360 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lc.svg
+-rw-rw-rw-   0        0        0    17635 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-li.svg
+-rw-rw-rw-   0        0        0    32573 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lk.svg
+-rw-rw-rw-   0        0        0      715 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lr.svg
+-rw-rw-rw-   0        0        0     3276 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ls.svg
+-rw-rw-rw-   0        0        0      278 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lt.svg
+-rw-rw-rw-   0        0        0      274 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lu.svg
+-rw-rw-rw-   0        0        0      223 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lv.svg
+-rw-rw-rw-   0        0        0      582 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ly.svg
+-rw-rw-rw-   0        0        0      660 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ma.svg
+-rw-rw-rw-   0        0        0      225 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mc.svg
+-rw-rw-rw-   0        0        0    30845 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-md.svg
+-rw-rw-rw-   0        0        0    98104 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-me.svg
+-rw-rw-rw-   0        0        0      285 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mg.svg
+-rw-rw-rw-   0        0        0     1118 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mh.svg
+-rw-rw-rw-   0        0        0      471 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mk.svg
+-rw-rw-rw-   0        0        0      284 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ml.svg
+-rw-rw-rw-   0        0        0      447 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mm.svg
+-rw-rw-rw-   0        0        0     1557 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mn.svg
+-rw-rw-rw-   0        0        0      801 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mr.svg
+-rw-rw-rw-   0        0        0    16379 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mt.svg
+-rw-rw-rw-   0        0        0      331 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mu.svg
+-rw-rw-rw-   0        0        0      352 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mv.svg
+-rw-rw-rw-   0        0        0     5294 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mw.svg
+-rw-rw-rw-   0        0        0   217014 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mx.svg
+-rw-rw-rw-   0        0        0     1116 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-my.svg
+-rw-rw-rw-   0        0        0     3135 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mz.svg
+-rw-rw-rw-   0        0        0     1282 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-na.svg
+-rw-rw-rw-   0        0        0      351 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ne.svg
+-rw-rw-rw-   0        0        0      226 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ng.svg
+-rw-rw-rw-   0        0        0    19703 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ni.svg
+-rw-rw-rw-   0        0        0      278 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nl.svg
+-rw-rw-rw-   0        0        0      424 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-no.svg
+-rw-rw-rw-   0        0        0     1411 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-np.svg
+-rw-rw-rw-   0        0        0      547 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nr.svg
+-rw-rw-rw-   0        0        0     1690 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nu.svg
+-rw-rw-rw-   0        0        0     2386 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nz.svg
+-rw-rw-rw-   0        0        0    24184 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-om.svg
+-rw-rw-rw-   0        0        0      604 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pa.svg
+-rw-rw-rw-   0        0        0      226 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pe.svg
+-rw-rw-rw-   0        0        0     3218 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pg.svg
+-rw-rw-rw-   0        0        0     2008 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ph.svg
+-rw-rw-rw-   0        0        0      441 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pk.svg
+-rw-rw-rw-   0        0        0      229 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pl.svg
+-rw-rw-rw-   0        0        0    45475 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pt.svg
+-rw-rw-rw-   0        0        0      239 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pw.svg
+-rw-rw-rw-   0        0        0    39303 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-py.svg
+-rw-rw-rw-   0        0        0      460 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-qa.svg
+-rw-rw-rw-   0        0        0      284 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ro.svg
+-rw-rw-rw-   0        0        0   814059 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-rs.svg
+-rw-rw-rw-   0        0        0      283 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ru.svg
+-rw-rw-rw-   0        0        0     1242 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-rw.svg
+-rw-rw-rw-   0        0        0    17152 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sa.svg
+-rw-rw-rw-   0        0        0     1200 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sb.svg
+-rw-rw-rw-   0        0        0      378 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sc.svg
+-rw-rw-rw-   0        0        0      325 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sd.svg
+-rw-rw-rw-   0        0        0      292 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-se.svg
+-rw-rw-rw-   0        0        0     1193 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sg.svg
+-rw-rw-rw-   0        0        0     1928 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-si.svg
+-rw-rw-rw-   0        0        0     2466 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sk.svg
+-rw-rw-rw-   0        0        0      290 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sl.svg
+-rw-rw-rw-   0        0        0   164720 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sm.svg
+-rw-rw-rw-   0        0        0      450 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sn.svg
+-rw-rw-rw-   0        0        0      327 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-so.svg
+-rw-rw-rw-   0        0        0      373 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sr.svg
+-rw-rw-rw-   0        0        0      475 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ss.svg
+-rw-rw-rw-   0        0        0      566 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-st.svg
+-rw-rw-rw-   0        0        0   199390 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sv.svg
+-rw-rw-rw-   0        0        0      563 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sy.svg
+-rw-rw-rw-   0        0        0     8156 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sz.svg
+-rw-rw-rw-   0        0        0      284 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-td.svg
+-rw-rw-rw-   0        0        0      464 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tg.svg
+-rw-rw-rw-   0        0        0      288 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-th.svg
+-rw-rw-rw-   0        0        0     2147 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tj.svg
+-rw-rw-rw-   0        0        0      435 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tl.svg
+-rw-rw-rw-   0        0        0    66310 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tm.svg
+-rw-rw-rw-   0        0        0      440 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tn.svg
+-rw-rw-rw-   0        0        0      353 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-to.svg
+-rw-rw-rw-   0        0        0      385 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tr.svg
+-rw-rw-rw-   0        0        0      305 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tt.svg
+-rw-rw-rw-   0        0        0     2111 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tv.svg
+-rw-rw-rw-   0        0        0     1213 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tw.svg
+-rw-rw-rw-   0        0        0      747 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tz.svg
+-rw-rw-rw-   0        0        0      228 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ua.svg
+-rw-rw-rw-   0        0        0     4062 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ug.svg
+-rw-rw-rw-   0        0        0     6292 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-us.svg
+-rw-rw-rw-   0        0        0     6541 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-uy.svg
+-rw-rw-rw-   0        0        0     1842 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-uz.svg
+-rw-rw-rw-   0        0        0    83348 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-va.svg
+-rw-rw-rw-   0        0        0      444 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-vc.svg
+-rw-rw-rw-   0        0        0     1266 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ve.svg
+-rw-rw-rw-   0        0        0    70173 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-vg.svg
+-rw-rw-rw-   0        0        0      339 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-vn.svg
+-rw-rw-rw-   0        0        0      545 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ws.svg
+-rw-rw-rw-   0        0        0     6467 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-xk.svg
+-rw-rw-rw-   0        0        0      271 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ye.svg
+-rw-rw-rw-   0        0        0      942 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-za.svg
+-rw-rw-rw-   0        0        0     7357 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-zm.svg
+-rw-rw-rw-   0        0        0     3010 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-zw.svg
+-rw-rw-rw-   0        0        0  3544097 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag.svg
+-rw-rw-rw-   0        0        0   421016 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/free.svg
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.672554 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/utils/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.568826 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/utils/js/
+-rw-rw-rw-   0        0        0     8100 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/utils/js/index.js
+-rw-rw-rw-   0        0        0     5763 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/utils/js/index.js.map
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.673533 django-admin-coreui-0.0.6/admin_coreui/static/vendors/chart.js/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.572820 django-admin-coreui-0.0.6/admin_coreui/static/vendors/chart.js/js/
+-rw-rw-rw-   0        0        0   205228 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/chart.js/js/chart.umd.js
+-rw-rw-rw-   0        0        0   953847 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/chart.js/js/chart.umd.js.map
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.675540 django-admin-coreui-0.0.6/admin_coreui/static/vendors/simplebar/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.574819 django-admin-coreui-0.0.6/admin_coreui/static/vendors/simplebar/css/
+-rw-rw-rw-   0        0        0     4467 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/simplebar/css/simplebar.css
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.575821 django-admin-coreui-0.0.6/admin_coreui/static/vendors/simplebar/js/
+-rw-rw-rw-   0        0        0    27067 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/static/vendors/simplebar/js/simplebar.min.js
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.590300 django-admin-coreui-0.0.6/admin_coreui/templates/
+-rw-rw-rw-   0        0        0     1007 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/404.html
+-rw-rw-rw-   0        0        0     1026 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/500.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.604705 django-admin-coreui-0.0.6/admin_coreui/templates/accounts/
+-rw-rw-rw-   0        0        0     1292 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/accounts/change-password.html
+-rw-rw-rw-   0        0        0     2303 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/accounts/login.html
+-rw-rw-rw-   0        0        0      646 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/accounts/password-change-done.html
+-rw-rw-rw-   0        0        0      702 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/accounts/password-reset-complete.html
+-rw-rw-rw-   0        0        0     1314 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/accounts/password-reset-confirm.html
+-rw-rw-rw-   0        0        0      726 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/accounts/password-reset-done.html
+-rw-rw-rw-   0        0        0     1314 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/accounts/password-reset.html
+-rw-rw-rw-   0        0        0     1318 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/accounts/register.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.637359 django-admin-coreui-0.0.6/admin_coreui/templates/admin/
+-rw-rw-rw-   0        0        0        0 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/.gitkeep
+-rw-rw-rw-   0        0        0     1743 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/actions.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:03.678060 django-admin-coreui-0.0.6/admin_coreui/templates/admin/auth/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.640901 django-admin-coreui-0.0.6/admin_coreui/templates/admin/auth/user/
+-rw-rw-rw-   0        0        0      471 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/auth/user/add_form.html
+-rw-rw-rw-   0        0        0     5363 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/auth/user/change_password.html
+-rw-rw-rw-   0        0        0     6511 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/change_form.html
+-rw-rw-rw-   0        0        0      696 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/change_form_object_tools.html
+-rw-rw-rw-   0        0        0     5953 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/change_list.html
+-rw-rw-rw-   0        0        0      479 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/change_list_object_tools.html
+-rw-rw-rw-   0        0        0     3257 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/change_list_results.html
+-rw-rw-rw-   0        0        0     7313 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/delete_confirmation.html
+-rw-rw-rw-   0        0        0     7632 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/delete_selected_confirmation.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.644901 django-admin-coreui-0.0.6/admin_coreui/templates/admin/edit_inline/
+-rw-rw-rw-   0        0        0     3893 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/edit_inline/stacked.html
+-rw-rw-rw-   0        0        0     7834 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/edit_inline/tabular.html
+-rw-rw-rw-   0        0        0      643 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/filter.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.648426 django-admin-coreui-0.0.6/admin_coreui/templates/admin/includes/
+-rw-rw-rw-   0        0        0     2608 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/includes/fieldset.html
+-rw-rw-rw-   0        0        0      339 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/includes/object_delete_summary.html
+-rw-rw-rw-   0        0        0    45052 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/index.html
+-rw-rw-rw-   0        0        0     3270 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/invalid_setup.html
+-rw-rw-rw-   0        0        0     4103 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/login.html
+-rw-rw-rw-   0        0        0     4402 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/object_history.html
+-rw-rw-rw-   0        0        0     2318 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/pagination.html
+-rw-rw-rw-   0        0        0     2641 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/search_form.html
+-rw-rw-rw-   0        0        0     1616 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/admin/submit_line.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.674429 django-admin-coreui-0.0.6/admin_coreui/templates/base/
+-rw-rw-rw-   0        0        0    11990 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/accordion.html
+-rw-rw-rw-   0        0        0     4567 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/breadcrumb.html
+-rw-rw-rw-   0        0        0    82746 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/cards.html
+-rw-rw-rw-   0        0        0    28776 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/carousel.html
+-rw-rw-rw-   0        0        0     9271 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/collapse.html
+-rw-rw-rw-   0        0        0    34134 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/list-group.html
+-rw-rw-rw-   0        0        0    52908 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/navs-tabs.html
+-rw-rw-rw-   0        0        0    19133 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/pagination.html
+-rw-rw-rw-   0        0        0    13926 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/placeholders.html
+-rw-rw-rw-   0        0        0     9313 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/popovers.html
+-rw-rw-rw-   0        0        0    18116 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/progress.html
+-rw-rw-rw-   0        0        0    23874 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/spinners.html
+-rw-rw-rw-   0        0        0    56754 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/tables.html
+-rw-rw-rw-   0        0        0     7546 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/base/tooltips.html
+-rw-rw-rw-   0        0        0     1886 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/blank.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.678943 django-admin-coreui-0.0.6/admin_coreui/templates/buttons/
+-rw-rw-rw-   0        0        0    30739 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/buttons/button-group.html
+-rw-rw-rw-   0        0        0    43034 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/buttons/buttons.html
+-rw-rw-rw-   0        0        0    69301 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/buttons/dropdowns.html
+-rw-rw-rw-   0        0        0    14383 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/charts.html
+-rw-rw-rw-   0        0        0     3142 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/colors.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.694061 django-admin-coreui-0.0.6/admin_coreui/templates/forms/
+-rw-rw-rw-   0        0        0    35183 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/forms/checks-radios.html
+-rw-rw-rw-   0        0        0    14654 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/forms/floating-labels.html
+-rw-rw-rw-   0        0        0    19111 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/forms/form-control.html
+-rw-rw-rw-   0        0        0    32078 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/forms/input-group.html
+-rw-rw-rw-   0        0        0    30767 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/forms/layout.html
+-rw-rw-rw-   0        0        0     7863 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/forms/range.html
+-rw-rw-rw-   0        0        0    10096 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/forms/select.html
+-rw-rw-rw-   0        0        0    26760 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/forms/validation.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.700551 django-admin-coreui-0.0.6/admin_coreui/templates/icons/
+-rw-rw-rw-   0        0        0   136182 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/icons/coreui-icons-brand.html
+-rw-rw-rw-   0        0        0    31442 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/icons/coreui-icons-flag.html
+-rw-rw-rw-   0        0        0    92991 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/icons/coreui-icons-free.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.708097 django-admin-coreui-0.0.6/admin_coreui/templates/includes/
+-rw-rw-rw-   0        0        0     3049 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/includes/head.html
+-rw-rw-rw-   0        0        0    17068 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/includes/navbar.html
+-rw-rw-rw-   0        0        0     1873 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/includes/scripts.html
+-rw-rw-rw-   0        0        0    23256 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/includes/sidebar.html
+-rw-rw-rw-   0        0        0      824 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/includes/topbar.html
+-rw-rw-rw-   0        0        0    47374 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/index.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.712111 django-admin-coreui-0.0.6/admin_coreui/templates/layouts/
+-rw-rw-rw-   0        0        0      667 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/layouts/base-fullscreen.html
+-rw-rw-rw-   0        0        0      956 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/layouts/base.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.719599 django-admin-coreui-0.0.6/admin_coreui/templates/notifications/
+-rw-rw-rw-   0        0        0    10717 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/notifications/alerts.html
+-rw-rw-rw-   0        0        0     8451 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/notifications/badge.html
+-rw-rw-rw-   0        0        0    57472 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/notifications/modals.html
+-rw-rw-rw-   0        0        0    17214 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/notifications/toasts.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.725597 django-admin-coreui-0.0.6/admin_coreui/templates/registration/
+-rw-rw-rw-   0        0        0        0 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/registration/.gitkeep
+-rw-rw-rw-   0        0        0     1690 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/registration/logged_out.html
+-rw-rw-rw-   0        0        0     2672 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/registration/password_change_done.html
+-rw-rw-rw-   0        0        0     3948 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/registration/password_change_form.html
+-rw-rw-rw-   0        0        0     7832 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/typography.html
+-rw-rw-rw-   0        0        0   107237 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templates/widgets.html
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.731158 django-admin-coreui-0.0.6/admin_coreui/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     2551 2024-04-28 06:32:23.000000 django-admin-coreui-0.0.6/admin_coreui/templatetags/admin_coreui.py
+-rw-rw-rw-   0        0        0      237 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/templatetags/replace_value.py
+-rw-rw-rw-   0        0        0       63 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/tests.py
+-rw-rw-rw-   0        0        0     3485 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/urls.py
+-rw-rw-rw-   0        0        0    16587 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.6/admin_coreui/utils.py
+-rw-rw-rw-   0        0        0     5779 2024-04-28 06:32:23.000000 django-admin-coreui-0.0.6/admin_coreui/views.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:56:06.763846 django-admin-coreui-0.0.6/django_admin_coreui.egg-info/
+-rw-rw-rw-   0        0        0     7415 2024-04-28 06:56:02.000000 django-admin-coreui-0.0.6/django_admin_coreui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    70589 2024-04-28 06:56:03.000000 django-admin-coreui-0.0.6/django_admin_coreui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 06:56:02.000000 django-admin-coreui-0.0.6/django_admin_coreui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-28 06:12:07.000000 django-admin-coreui-0.0.6/django_admin_coreui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2024-04-28 06:56:03.000000 django-admin-coreui-0.0.6/django_admin_coreui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 06:56:06.767359 django-admin-coreui-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2024-04-28 06:54:21.000000 django-admin-coreui-0.0.6/setup.py
```

### Comparing `django-admin-coreui-0.0.5/LICENSE.md` & `django-admin-coreui-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/PKG-INFO` & `django-admin-coreui-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-coreui
-Version: 0.0.5
+Version: 0.0.6
 Summary: Modern template for Django admin interface
 Home-page: https://appseed.us/product/coreui/django/
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `django-admin-coreui-0.0.5/README.md` & `django-admin-coreui-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/forms.py` & `django-admin-coreui-0.0.6/admin_coreui/forms.py`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/brand/coreui.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/brand/coreui.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/css/forms.css` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/css/forms.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/css/widgets.css` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/css/widgets.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/android-icon-144x144.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/android-icon-192x192.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/android-icon-36x36.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/android-icon-48x48.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/android-icon-72x72.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/android-icon-96x96.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-114x114.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-120x120.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-144x144.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-152x152.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-180x180.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-57x57.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-60x60.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-72x72.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-76x76.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon-precomposed.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/apple-icon.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/apple-icon.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/favicon-16x16.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/favicon-32x32.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/favicon-96x96.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/favicon.ico` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/manifest.json` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/manifest.json`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/ms-icon-144x144.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/ms-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/ms-icon-150x150.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/ms-icon-310x310.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/favicon/ms-icon-70x70.png` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/favicon/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/3d.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/3d.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/4k.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/4k.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/action-undo.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/action-undo.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/address-book.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/address-book.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/airplane-mode-off.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/airplane-mode-off.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/airplane-mode.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/airplane-mode.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/alarm.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/alarm.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/album.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/album.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/american-football.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/american-football.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/android.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/android.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/aperture.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/aperture.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/apple.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/apple.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/applications-settings.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/applications-settings.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/applications.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/applications.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-circle-bottom.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-circle-bottom.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-circle-left.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-circle-left.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-circle-right.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-circle-right.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/arrow-circle-top.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/arrow-circle-top.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/assistive-listening-system.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/assistive-listening-system.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/asterisk-circle.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/asterisk-circle.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/at.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/at.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/audio-description.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/audio-description.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/audio.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/audio.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/av-timer.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/av-timer.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/badge.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/badge.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/balance-scale.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/balance-scale.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/ban.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/ban.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bank.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bank.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bar-chart.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bar-chart.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/barcode.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/barcode.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/baseball.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/baseball.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/basket.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/basket.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/basketball.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/basketball.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bath.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bath.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/battery-0.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/battery-0.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/battery-3.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/battery-3.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/battery-5.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/battery-5.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/battery-alert.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/battery-alert.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/battery-slash.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/battery-slash.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/beach-access.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/beach-access.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/beaker.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/beaker.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bed.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bed.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bell.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bell.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bike.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bike.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/birthday-cake.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/birthday-cake.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/blind.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/blind.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/blur-circular.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/blur-circular.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/blur-linear.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/blur-linear.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/blur.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/blur.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/boat-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/boat-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bold.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bold.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/book.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/book.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bootstrap.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bootstrap.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-bottom.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-bottom.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-clear.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-clear.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-horizontal.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-horizontal.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-inner.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-inner.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-left.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-left.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-outer.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-outer.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-right.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-right.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-style.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-style.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-top.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-top.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/border-vertical.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/border-vertical.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bowling.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bowling.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/braille.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/braille.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/500px.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/500px.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/accessible-icon.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/accessible-icon.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/accusoft.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/accusoft.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/acquisitions-incorporated.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/acquisitions-incorporated.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/adversal.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/adversal.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/airbnb.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/airbnb.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/algolia.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/algolia.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/alipay.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/alipay.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/amazon-pay.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/amazon-pay.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/amazon.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/amazon.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/amilia.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/amilia.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/android.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/android.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/angellist.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/angellist.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/angrycreative.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/angrycreative.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/app-store-ios.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/app-store-ios.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/app-store.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/app-store.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/apper.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/apper.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/apple-pay.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/apple-pay.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/apple.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/apple.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/asymmetrik.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/asymmetrik.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/audible.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/audible.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/avianex.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/avianex.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/aviato.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/aviato.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/aws.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/aws.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/battle-net.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/battle-net.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/behance-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/behance-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/behance.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/behance.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/bitcoin.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/bitcoin.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/bity.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/bity.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/blackberry.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/blackberry.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/blogger-b.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/blogger-b.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/blogger.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/blogger.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/bootstrap.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/bootstrap.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/brands-symbol-defs.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/brands-symbol-defs.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/btc.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/btc.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/buffer.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/buffer.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/canadian-maple-leaf.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/canadian-maple-leaf.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-amazon-pay.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-amazon-pay.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-amex.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-amex.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-apple-pay.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-apple-pay.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-diners-club.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-diners-club.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-discover.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-discover.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-jcb.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-jcb.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-mastercard.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-mastercard.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-paypal.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-paypal.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-stripe.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-stripe.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cc-visa.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cc-visa.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/centos.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/centos.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/chrome.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/chrome.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cloudscale.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cloudscale.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cloudversify.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cloudversify.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/codepen.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/codepen.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/codiepie.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/codiepie.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/confluence.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/confluence.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/connectdevelop.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/connectdevelop.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/contao.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/contao.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/cpanel.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/cpanel.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-by.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-by.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-nc-eu.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-nc-eu.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-nc-jp.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-nc-jp.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-nc.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-nc.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-pd-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-pd-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-pd.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-pd.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-remix.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-remix.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-sa.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-sa.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-sampling-plus.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-sampling-plus.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-sampling.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-sampling.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-share.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-share.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons-zero.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons-zero.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/creative-commons.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/creative-commons.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/critical-role.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/critical-role.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/d-and-d-beyond.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/d-and-d-beyond.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/d-and-d.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/d-and-d.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/delicious.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/delicious.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/deploydog.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/deploydog.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/deskpro.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/deskpro.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/dev.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/dev.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/dhl.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/dhl.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/discord.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/discord.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/docker.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/docker.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/draft2digital.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/draft2digital.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/dribbble-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/dribbble-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/dribbble.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/dribbble.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/drupal.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/drupal.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/earlybirds.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/earlybirds.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ebay.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ebay.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/edge.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/edge.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ember.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ember.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/empire.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/empire.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/etsy.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/etsy.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/evernote.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/evernote.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/expeditedssl.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/expeditedssl.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/facebook-messenger.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/facebook-messenger.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fantasy-flight-games.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fantasy-flight-games.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fedex.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fedex.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fedora.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fedora.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/firefox.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/firefox.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/first-order-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/first-order-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/first-order.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/first-order.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fly.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fly.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/font-awesome-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/font-awesome-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/font-awesome-flag.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/font-awesome-flag.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/font-awesome-logo-full.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/font-awesome-logo-full.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/font-awesome.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/font-awesome.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fonticons-fi.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fonticons-fi.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fonticons.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fonticons.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fort-awesome-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fort-awesome-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/fort-awesome.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/fort-awesome.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/forumbee.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/forumbee.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/foursquare.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/foursquare.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/free-code-camp.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/free-code-camp.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/freebsd.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/freebsd.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/galactic-republic.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/galactic-republic.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/galactic-senate.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/galactic-senate.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/git-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/git-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/git-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/git-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/git.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/git.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/github-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/github-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/github-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/github-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/github.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/github.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/gitkraken.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/gitkraken.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/glide-g.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/glide-g.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/glide.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/glide.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/goodreads-g.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/goodreads-g.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/goodreads.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/goodreads.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/google-plus-g.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/google-plus-g.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/google-wallet.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/google-wallet.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/grav.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/grav.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/gripfire.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/gripfire.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/grunt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/grunt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/gulp.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/gulp.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hackerrank.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hackerrank.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hips.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hips.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hire-a-helper.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hire-a-helper.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hooli.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hooli.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hornbill.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hornbill.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/hubspot.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/hubspot.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/imdb.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/imdb.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/instagram.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/instagram.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/intercom.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/intercom.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/internet-explorer.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/internet-explorer.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/invision.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/invision.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ioxhost.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ioxhost.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/itch-io.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/itch-io.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/itunes-note.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/itunes-note.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/itunes.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/itunes.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/java.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/java.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/jedi-order.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/jedi-order.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/jenkins.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/jenkins.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/joget.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/joget.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/joomla.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/joomla.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/js-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/js-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/js.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/js.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/jsfiddle.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/jsfiddle.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/keybase.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/keybase.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/keycdn.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/keycdn.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/laravel.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/laravel.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/lastfm-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/lastfm-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/lastfm.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/lastfm.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/leanpub.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/leanpub.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/less.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/less.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/line.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/line.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/linode.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/linode.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/linux.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/linux.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/lyft.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/lyft.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/mailchimp.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/mailchimp.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/mandalorian.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/mandalorian.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/mastodon.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/mastodon.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/medapps.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/medapps.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/medrt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/medrt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/meetup.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/meetup.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/mendeley.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/mendeley.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/mixcloud.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/mixcloud.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/napster.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/napster.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/nimblr.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/nimblr.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/node-js.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/node-js.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/node.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/node.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ns8.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ns8.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/nutritionix.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/nutritionix.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/odnoklassniki-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/odnoklassniki-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/odnoklassniki.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/odnoklassniki.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/old-republic.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/old-republic.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/optin-monster.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/optin-monster.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/osi.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/osi.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/page4.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/page4.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pagelines.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pagelines.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/palfed.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/palfed.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/paypal.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/paypal.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/penny-arcade.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/penny-arcade.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/periscope.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/periscope.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/phabricator.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/phabricator.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/phoenix-framework.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/phoenix-framework.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/phoenix-squadron.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/phoenix-squadron.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/php.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/php.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pied-piper-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pied-piper-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pied-piper-hat.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pied-piper-hat.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pied-piper-pp.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pied-piper-pp.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pinterest-p.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pinterest-p.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pinterest-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pinterest-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pinterest.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pinterest.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/playstation.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/playstation.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/pushed.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/pushed.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/python.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/python.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/qq.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/qq.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/quora.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/quora.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/r-project.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/r-project.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/raspberry-pi.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/raspberry-pi.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ravelry.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ravelry.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/react.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/react.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/reacteurope.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/reacteurope.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/readme.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/readme.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/rebel.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/rebel.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/reddit-alien.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/reddit-alien.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/reddit-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/reddit-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/reddit.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/reddit.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/redhat.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/redhat.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/replyd.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/replyd.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/researchgate.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/researchgate.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/resolving.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/resolving.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/rocketchat.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/rocketchat.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/safari.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/safari.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/salesforce.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/salesforce.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sass.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sass.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/schlix.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/schlix.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/scribd.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/scribd.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/searchengin.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/searchengin.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sellcast.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sellcast.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sellsy.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sellsy.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/shirtsinbulk.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/shirtsinbulk.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/shopware.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/shopware.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/simplybuilt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/simplybuilt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sith.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sith.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/skyatlas.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/skyatlas.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/skype.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/skype.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/slack-hash.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/slack-hash.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/slack.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/slack.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/slideshare.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/slideshare.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/snapchat-ghost.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/snapchat-ghost.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/snapchat-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/snapchat-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/snapchat.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/snapchat.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/soundcloud.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/soundcloud.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/speakap.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/speakap.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/spotify.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/spotify.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/squarespace.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/squarespace.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/stackpath.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/stackpath.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/staylinked.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/staylinked.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/steam-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/steam-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/steam-symbol.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/steam-symbol.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/steam.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/steam.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/sticker-mule.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/sticker-mule.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/stripe.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/stripe.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/studiovinari.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/studiovinari.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/stumbleupon-circle.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/stumbleupon-circle.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/supple.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/supple.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/suse.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/suse.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/symfony.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/symfony.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/teamspeak.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/teamspeak.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/the-red-yeti.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/the-red-yeti.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/themeco.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/themeco.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/themeisle.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/themeisle.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/trade-federation.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/trade-federation.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/tripadvisor.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/tripadvisor.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/tumblr-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/tumblr-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/twitter-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/twitter-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/twitter.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/twitter.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ubuntu.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ubuntu.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/uniregistry.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/uniregistry.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/untappd.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/untappd.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ups.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ups.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/usb.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/usb.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/usps.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/usps.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/ussunnah.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/ussunnah.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vaadin.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vaadin.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/viadeo-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/viadeo-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/viadeo.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/viadeo.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/viber.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/viber.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vimeo-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vimeo-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vimeo.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vimeo.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vk.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vk.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/vnv.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/vnv.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/waze.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/waze.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/weebly.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/weebly.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/weibo.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/weibo.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/weixin.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/weixin.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/whatsapp-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/whatsapp-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/whatsapp.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/whatsapp.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/whmcs.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/whmcs.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wikipedia-w.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wikipedia-w.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wix.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wix.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wizards-of-the-coast.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wizards-of-the-coast.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wolf-pack-battalion.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wolf-pack-battalion.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wordpress-simple.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wordpress-simple.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wordpress.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wordpress.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wpbeginner.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wpbeginner.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wpexplorer.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wpexplorer.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wpforms.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wpforms.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/wpressr.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/wpressr.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/xbox.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/xbox.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/xing-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/xing-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/yammer.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/yammer.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/yarn.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/yarn.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/yelp.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/yelp.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/yoast.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/yoast.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/youtube-square.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/youtube-square.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/youtube.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/youtube.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brands/zhihu.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brands/zhihu.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/briefcase.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/briefcase.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brightness.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brightness.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brush-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brush-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/brush.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/brush.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bug.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bug.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/building.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/building.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/burger.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/burger.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/bus-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/bus-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/calculator.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/calculator.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/calendar-check.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/calendar-check.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/calendar.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/calendar.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/camera-control.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/camera-control.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/camera-roll.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/camera-roll.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/camera.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/camera.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/car-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/car-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cart.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cart.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/casino.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/casino.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cast.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cast.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cat.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cat.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/center-focus.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/center-focus.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chart-pie.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chart-pie.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chart.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chart.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chat-bubble.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chat-bubble.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-circle-down-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-circle-down-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-circle-left-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-circle-left-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-circle-right-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-circle-right-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-circle-up-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-circle-up-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-double-down.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-double-down.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-double-left.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-double-left.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-double-right.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-double-right.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/chevron-double-up.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/chevron-double-up.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/child-friendly.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/child-friendly.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/child.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/child.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/circle.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/circle.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/clipboard.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/clipboard.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/clone.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/clone.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/closed-captioning.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/closed-captioning.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cloud-download.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cloud-download.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cloud-upload.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cloud-upload.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cloud.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cloud.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cloudy.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cloudy.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/codepen.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/codepen.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/coffee.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/coffee.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/color-border.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/color-border.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/color-fill.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/color-fill.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/color-palette.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/color-palette.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/comment-bubble.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/comment-bubble.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/compass.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/compass.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/contact.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/contact.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/contrast.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/contrast.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/copyright.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/copyright.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/coreui/free-symbol-defs.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/coreui/free-symbol-defs.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/couch.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/couch.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/credit-card.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/credit-card.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/crop-rotate.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/crop-rotate.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/crop.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/crop.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cursor-move.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cursor-move.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/cut.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/cut.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/deaf.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/deaf.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/delete.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/devices.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/devices.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/dialpad.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/dialpad.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/dog.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/dog.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/dollar.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/dollar.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/drink.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/drink.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/drop.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/drop.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/drop1.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/drop1.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/envelope-letter.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/envelope-letter.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/equalizer.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/equalizer.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/ethernet.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/ethernet.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/euro.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/euro.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/excerpt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/excerpt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/exit-to-app.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/exit-to-app.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/exposure.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/exposure.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/eye.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/eye.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/eyedropper.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/eyedropper.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/face-dead.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/face-dead.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/face.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/face.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/facebook.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/facebook.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fastfood.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fastfood.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fax.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fax.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/featured-playlist.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/featured-playlist.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/filter-frames.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/filter-frames.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/filter-photo.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/filter-photo.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/find-in-page.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/find-in-page.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fingerprint.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fire.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fire.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/flight-takeoff.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/flight-takeoff.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/flip-to-back.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/flip-to-back.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/flip-to-front.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/flip-to-front.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/flip.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/flip.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/flower.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/flower.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/folder-open.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/folder-open.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/football.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/football.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fork.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fork.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/fridge.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/fridge.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/frown.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/frown.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/functions.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/functions.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/gamepad.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/gamepad.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/garage.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/garage.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/gift.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/gift.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/git.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/git.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/github-circle.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/github-circle.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/github.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/gitlab.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/gitlab.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/globe-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/globe-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/golf-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/golf-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/golf.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/golf.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/gradient.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/gradient.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/grain.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/grain.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/graph.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/graph.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/grid-slash.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/grid-slash.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/grid.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/grid.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hand-point-down.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hand-point-down.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hand-point-left.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hand-point-left.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hand-point-right.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hand-point-right.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hand-point-up.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hand-point-up.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hd.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hd.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hdr.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hdr.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/headphones.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/headphones.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/healing.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/healing.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/heart.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/heart.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/highlighter.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/highlighter.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/highligt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/highligt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/history.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/history.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/home.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/home.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hospital.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hospital.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/hot-tub.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/hot-tub.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/house.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/house.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/https.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/https.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/indent-decrease.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/indent-decrease.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/indent-increase.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/indent-increase.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/industry-slash.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/industry-slash.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/industry.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/industry.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/infinity.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/infinity.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/info.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/info.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/input.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/input.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/instagram.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/instagram.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/institution.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/institution.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/keyboard.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/keyboard.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/lan.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/lan.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/language.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/language.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/layers.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/layers.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/leaf.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/leaf.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/lemon.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/lemon.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/library-add.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/library-add.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/library.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/library.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/life-ring.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/life-ring.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/lightbulb.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/lightbulb.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/line-spacing.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/line-spacing.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/line-style.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/line-style.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/link-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/link-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/link-broken.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/link-broken.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/link.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/link.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/linkedin.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/linkedin.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/list-high-priority.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/list-high-priority.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/list-low-priority.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/list-low-priority.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/list-numbered.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/list-numbered.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/list-rich.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/list-rich.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/list.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/list.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/location-pin.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/location-pin.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/locomotive.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/locomotive.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/loop-1.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/loop-1.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/loop-circular.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/loop-circular.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/loop.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/loop.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/low-vision.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/low-vision.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/magnifying-glass.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/magnifying-glass.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/map.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/map.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-eject.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-eject.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-pause.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-pause.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-skip-backward.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-skip-backward.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-skip-forward.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-skip-forward.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-step-backward.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-step-backward.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/media-step-forward.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/media-step-forward.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/meh.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/meh.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/microphone.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/microphone.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/money.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/money.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mood-bad.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mood-bad.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mood-good.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mood-good.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mood-very-bad.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mood-very-bad.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mood-very-good.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mood-very-good.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/moon.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/moon.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mouse.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mouse.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mouth-slash.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mouth-slash.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/move.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/move.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/movie.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/movie.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mug-tea.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mug-tea.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/mug.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/mug.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/music-note.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/music-note.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/newspaper.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/newspaper.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/object-group.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/object-group.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/object-ungroup.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/object-ungroup.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/opacity.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/opacity.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/options-horizontal.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/options-horizontal.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/options.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/options.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/paint-bucket.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/paint-bucket.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/paint.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/paint.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/paperclip.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/paperclip.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/paw.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/paw.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pen-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pen-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pen-nib.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pen-nib.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pencil.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pencil.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/people.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/people.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/phone.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/phone.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pin.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pin.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pizza.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pizza.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pool.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pool.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/pregnant.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/pregnant.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/print.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/print.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/puzzle.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/puzzle.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/qr-code.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/qr-code.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/rain.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/rain.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/react.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/react.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/reddit.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/reddit.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/registered.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/registered.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/restaurant.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/restaurant.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/rowing.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/rowing.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/rss.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/rss.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/running.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/running.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/satelite.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/satelite.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/save.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/save.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/scrubber.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/scrubber.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/settings.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/share-all.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/share-all.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/share-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/share-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/share-boxed.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/share-boxed.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/share.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/share.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/shield-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/shield-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/shower.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/shower.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sign-language.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sign-language.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sim.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sim.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sitemap.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sitemap.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/skype.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/skype.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/smile-plus.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/smile-plus.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/smile.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/smile.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/smoke-free.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/smoke-free.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/smoking-room.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/smoking-room.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/snowflake.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/snowflake.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sort-alpha-down.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sort-alpha-down.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sort-alpha-up.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sort-alpha-up.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sort-ascending.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sort-ascending.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sort-descending.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sort-descending.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sort-numeric-down.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sort-numeric-down.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sort-numeric-up.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sort-numeric-up.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/spa.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/spa.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/speaker.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/speaker.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/speech.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/speech.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/speedometer.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/speedometer.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/spotify.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/spotify.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/spreadsheet.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/spreadsheet.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/stackoverflow.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/stackoverflow.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/star-half.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/star-half.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/star.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/star.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sun.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sun.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/swimming.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/swimming.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/sync.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/sync.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/tag.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/tag.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/tags.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/tags.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/task.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/task.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/taxi.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/taxi.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/tennis-ball.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/tennis-ball.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/tennis.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/tennis.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/terminal.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/terminal.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/text-shapes.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/text-shapes.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/text-strike.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/text-strike.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/thumb-down.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/thumb-down.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/thumb-up.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/thumb-up.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/toggle-off.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/toggle-off.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/toilet.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/toilet.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/touch-app.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/touch-app.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/translate.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/translate.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/trash.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/trash.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/truck.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/truck.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/twitter.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/twitter.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/underline.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/underline.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/user-female.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/user-female.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/user-follow.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/user-follow.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/user-unfollow.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/user-unfollow.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/user.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/user.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/vector.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/vector.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/vertical-align-center1.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/vertical-align-center1.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/voice-over-record.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/voice-over-record.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/volume-high.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/volume-high.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/walk.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/walk.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wallet.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wallet.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wallpaper.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wallpaper.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/watch.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/watch.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wc.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wc.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/weightlifitng.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/weightlifitng.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wheelchair.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wheelchair.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wifi-signal-0.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wifi-signal-0.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wifi-signal-1.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wifi-signal-1.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wifi-signal-2.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wifi-signal-2.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wifi-signal-4.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wifi-signal-4.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wifi-signal-off.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wifi-signal-off.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/window-restore.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/window-restore.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/wrap-text.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/wrap-text.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/x-circle.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/x-circle.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/zoom-in.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/zoom-in.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/icons/zoom-out.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/icons/zoom-out.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/1.jpg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/1.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/2.jpg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/2.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/3.jpg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/3.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/4.jpg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/4.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/5.jpg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/5.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/6.jpg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/6.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/7.jpg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/7.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/8.jpg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/8.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/avatars/9.jpg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/avatars/9.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/background-pro-yellow.jpg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/background-pro-yellow.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/background-pro.jpg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/background-pro.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/full.jpg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/full.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/icon-calendar.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/icon-calendar.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/icon-clock.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/icon-clock.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/icon-unknown-alt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/icon-unknown-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/icon-unknown.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/icon-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/icons/add.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/icons/add.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/img/selector-icons.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/img/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/package-lock.json` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/package-lock.json`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/assets/package.json` & `django-admin-coreui-0.0.6/admin_coreui/static/assets/package.json`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/ads.css` & `django-admin-coreui-0.0.6/admin_coreui/static/css/ads.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/ads.css.map` & `django-admin-coreui-0.0.6/admin_coreui/static/css/ads.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/ads.min.css` & `django-admin-coreui-0.0.6/admin_coreui/static/css/ads.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/ads.min.css.map` & `django-admin-coreui-0.0.6/admin_coreui/static/css/ads.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/examples.css` & `django-admin-coreui-0.0.6/admin_coreui/static/css/examples.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/examples.css.map` & `django-admin-coreui-0.0.6/admin_coreui/static/css/examples.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/examples.min.css` & `django-admin-coreui-0.0.6/admin_coreui/static/css/examples.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/examples.min.css.map` & `django-admin-coreui-0.0.6/admin_coreui/static/css/examples.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/icons.css` & `django-admin-coreui-0.0.6/admin_coreui/static/css/icons.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/style.css` & `django-admin-coreui-0.0.6/admin_coreui/static/css/style.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/style.css.map` & `django-admin-coreui-0.0.6/admin_coreui/static/css/style.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/style.min.css` & `django-admin-coreui-0.0.6/admin_coreui/static/css/style.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/css/style.min.css.map` & `django-admin-coreui-0.0.6/admin_coreui/static/css/style.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/charts.js` & `django-admin-coreui-0.0.6/admin_coreui/static/js/charts.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/charts.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/js/charts.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/color-modes.js` & `django-admin-coreui-0.0.6/admin_coreui/static/js/color-modes.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/color-modes.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/js/color-modes.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/colors.js` & `django-admin-coreui-0.0.6/admin_coreui/static/js/colors.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/colors.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/js/colors.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/config.js` & `django-admin-coreui-0.0.6/admin_coreui/static/js/config.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/config.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/js/config.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/main.js` & `django-admin-coreui-0.0.6/admin_coreui/static/js/main.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/main.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/js/main.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/popovers.js` & `django-admin-coreui-0.0.6/admin_coreui/static/js/popovers.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/popovers.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/js/popovers.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/toasts.js` & `django-admin-coreui-0.0.6/admin_coreui/static/js/toasts.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/toasts.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/js/toasts.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/tooltips.js` & `django-admin-coreui-0.0.6/admin_coreui/static/js/tooltips.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/tooltips.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/js/tooltips.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/widgets.js` & `django-admin-coreui-0.0.6/admin_coreui/static/js/widgets.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/js/widgets.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/js/widgets.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/chartjs/css/coreui-chartjs.css` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/chartjs/css/coreui-chartjs.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/chartjs/css/coreui-chartjs.css.map` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/chartjs/css/coreui-chartjs.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/chartjs/js/coreui-chartjs.js` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/chartjs/js/coreui-chartjs.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/chartjs/js/coreui-chartjs.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/chartjs/js/coreui-chartjs.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/coreui/js/coreui.bundle.min.js` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/coreui/js/coreui.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/coreui/js/coreui.bundle.min.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/coreui/js/coreui.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/brand.min.css` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/brand.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/brand.min.css.map` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/brand.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/flag.min.css` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/flag.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/flag.min.css.map` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/flag.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/free.min.css` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/free.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/css/free.min.css.map` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/css/free.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.eot` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.eot`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.ttf` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.woff` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Brand.woff`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.eot` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.eot`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.ttf` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.woff` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/fonts/CoreUI-Icons-Free.woff`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/brand.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/brand.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ad.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ad.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-af.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-af.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ag.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ag.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-al.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-al.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ao.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ao.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ar.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ar.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-au.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-au.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-az.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-az.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ba.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ba.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bb.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bb.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bi.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bi.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bn.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bn.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-br.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-br.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-by.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-by.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bz.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-bz.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ca.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ca.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cf.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cf.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ck.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ck.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cn.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cn.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cv.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cv.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cy.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-cy.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-dm.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-dm.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-do.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-do.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-dz.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-dz.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ec.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ec.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-eg.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-eg.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-er.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-er.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-es.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-es.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-et.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-et.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-fj.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-fj.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-fm.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-fm.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gb.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gb.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gd.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gd.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ge.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ge.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gn.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gn.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gq.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gq.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-gt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hk.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hk.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hn.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hn.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hr.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-hr.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ht.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ht.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-in.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-in.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-iq.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-iq.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ir.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ir.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-jm.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-jm.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-jo.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-jo.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ke.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ke.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kg.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kg.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kh.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kh.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ki.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ki.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-km.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-km.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kn.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kn.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kr.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kr.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kz.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-kz.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lb.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lb.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-li.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-li.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lk.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lk.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lr.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-lr.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ls.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ls.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ly.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ly.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ma.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ma.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-md.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-md.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-me.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-me.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mh.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mh.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mn.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mn.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mr.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mr.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mw.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mw.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mx.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mx.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-my.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-my.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mz.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-mz.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-na.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-na.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ni.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ni.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-np.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-np.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nr.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nr.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nu.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nu.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nz.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-nz.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-om.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-om.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pa.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pa.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pg.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pg.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ph.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ph.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pt.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-pt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-py.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-py.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-rs.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-rs.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-rw.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-rw.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sa.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sa.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sb.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sb.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sg.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sg.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-si.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-si.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sk.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sk.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sm.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sm.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-st.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-st.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sv.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sv.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sy.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sy.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sz.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-sz.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tj.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tj.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tm.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tm.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tv.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tv.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tw.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tw.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tz.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-tz.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ug.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ug.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-us.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-us.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-uy.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-uy.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-uz.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-uz.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-va.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-va.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ve.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ve.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-vg.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-vg.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ws.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-ws.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-xk.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-xk.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-za.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-za.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-zm.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-zm.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-zw.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag/cif-zw.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/flag.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/flag.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/icons/svg/free.svg` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/icons/svg/free.svg`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/utils/js/index.js` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/utils/js/index.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/@coreui/utils/js/index.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/@coreui/utils/js/index.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/chart.js/js/chart.umd.js` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/chart.js/js/chart.umd.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/chart.js/js/chart.umd.js.map` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/chart.js/js/chart.umd.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/simplebar/css/simplebar.css` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/simplebar/css/simplebar.css`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/static/vendors/simplebar/js/simplebar.min.js` & `django-admin-coreui-0.0.6/admin_coreui/static/vendors/simplebar/js/simplebar.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/404.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/404.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/500.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/500.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/accounts/change-password.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/accounts/change-password.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/accounts/login.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/accounts/login.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/accounts/password-change-done.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/accounts/password-change-done.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/accounts/password-reset-complete.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/accounts/password-reset-complete.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/accounts/password-reset-confirm.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/accounts/password-reset-confirm.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/accounts/password-reset-done.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/accounts/password-reset-done.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/accounts/password-reset.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/accounts/password-reset.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/accounts/register.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/accounts/register.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/actions.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/auth/user/change_password.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/change_form.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/change_form_object_tools.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/change_list.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/change_list_results.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/delete_confirmation.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/delete_selected_confirmation.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/edit_inline/stacked.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/edit_inline/tabular.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/filter.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/includes/fieldset.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/index.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/invalid_setup.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/invalid_setup.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/login.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/object_history.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/pagination.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/search_form.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/admin/submit_line.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/accordion.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/accordion.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/breadcrumb.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/cards.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/cards.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/carousel.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/carousel.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/collapse.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/collapse.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/list-group.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/list-group.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/navs-tabs.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/navs-tabs.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/pagination.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/pagination.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/placeholders.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/placeholders.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/popovers.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/popovers.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/progress.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/progress.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/spinners.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/spinners.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/tables.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/tables.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/base/tooltips.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/base/tooltips.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/blank.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/blank.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/buttons/button-group.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/buttons/button-group.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/buttons/buttons.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/buttons/buttons.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/buttons/dropdowns.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/buttons/dropdowns.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/charts.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/charts.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/colors.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/colors.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/forms/checks-radios.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/forms/checks-radios.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/forms/floating-labels.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/forms/floating-labels.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/forms/form-control.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/forms/form-control.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/forms/input-group.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/forms/input-group.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/forms/layout.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/forms/layout.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/forms/range.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/forms/range.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/forms/select.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/forms/select.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/forms/validation.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/forms/validation.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/icons/coreui-icons-brand.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/icons/coreui-icons-brand.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/icons/coreui-icons-flag.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/icons/coreui-icons-flag.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/icons/coreui-icons-free.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/icons/coreui-icons-free.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/includes/head.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/includes/head.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/includes/navbar.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/includes/navbar.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/includes/scripts.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/includes/scripts.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/includes/sidebar.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/includes/sidebar.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/includes/topbar.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/includes/topbar.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/index.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/layouts/base-fullscreen.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/layouts/base-fullscreen.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/layouts/base.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/notifications/alerts.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/notifications/alerts.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/notifications/badge.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/notifications/badge.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/notifications/modals.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/notifications/modals.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/notifications/toasts.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/notifications/toasts.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/registration/logged_out.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/registration/password_change_done.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/registration/password_change_form.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/typography.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/typography.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templates/widgets.html` & `django-admin-coreui-0.0.6/admin_coreui/templates/widgets.html`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/templatetags/admin_coreui.py` & `django-admin-coreui-0.0.6/admin_coreui/templatetags/admin_coreui.py`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/urls.py` & `django-admin-coreui-0.0.6/admin_coreui/urls.py`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/utils.py` & `django-admin-coreui-0.0.6/admin_coreui/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/admin_coreui/views.py` & `django-admin-coreui-0.0.6/admin_coreui/views.py`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/django_admin_coreui.egg-info/PKG-INFO` & `django-admin-coreui-0.0.6/django_admin_coreui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-coreui
-Version: 0.0.5
+Version: 0.0.6
 Summary: Modern template for Django admin interface
 Home-page: https://appseed.us/product/coreui/django/
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `django-admin-coreui-0.0.5/django_admin_coreui.egg-info/SOURCES.txt` & `django-admin-coreui-0.0.6/django_admin_coreui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.5/setup.py` & `django-admin-coreui-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
 name='django-admin-coreui',
-version='0.0.5',
+version='0.0.6',
 zip_safe=False,
 packages=find_packages(),
 include_package_data=True,
 description='Modern template for Django admin interface',
 long_description=README,
 long_description_content_type="text/markdown",
 url='https://appseed.us/product/coreui/django/',
```

