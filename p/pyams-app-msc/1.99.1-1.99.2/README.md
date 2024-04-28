# Comparing `tmp/pyams_app_msc-1.99.1.tar.gz` & `tmp/pyams_app_msc-1.99.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_app_msc-1.99.1.tar", last modified: Wed Apr 10 07:49:17 2024, max compression
+gzip compressed data, was "dist/pyams_app_msc-1.99.2.tar", last modified: Sun Apr 28 15:45:17 2024, max compression
```

## Comparing `pyams_app_msc-1.99.1.tar` & `pyams_app_msc-1.99.2.tar`

### file list

```diff
@@ -1,373 +1,386 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2004 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/docs/
--rwxrwxrwx   0 root         (0) root         (0)      467 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)      965 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/docs/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/docs/booking.puml
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/docs/classes.puml
--rw-rw-rw-   0 root         (0) root         (0)    16507 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/docs/es-mapping.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/assets/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/clock.png
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/email.png
--rw-rw-rw-   0 root         (0) root         (0)   207972 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-brands-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)   117372 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-brands-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)    68004 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-regular-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)    25452 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-regular-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)   419720 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-solid-900.ttf
--rw-rw-rw-   0 root         (0) root         (0)   156496 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-solid-900.woff2
--rw-rw-rw-   0 root         (0) root         (0)    10832 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-v4compatibility.ttf
--rw-rw-rw-   0 root         (0) root         (0)     4792 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/fa-v4compatibility.woff2
--rw-rw-rw-   0 root         (0) root         (0)     7604 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/form.png
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/layers-2x.png
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/layers.png
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/list-item.png
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/map.png
--rw-rw-rw-   0 root         (0) root         (0)     1466 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/marker-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/mobile-menu.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/phone.png
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/select2-spinner.gif
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/select2.png
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/select2x2.png
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/assets/social-icons.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/css/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/css/dev/
--rw-rw-rw-   0 root         (0) root         (0)   263831 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/dev/msc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/css/dist/
--rw-rw-rw-   0 root         (0) root         (0)   337917 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/dist/msc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/css/img/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/clock.png
--rw-rw-rw-   0 root         (0) root         (0)      880 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/download.svg
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/email.png
--rw-rw-rw-   0 root         (0) root         (0)     7604 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/form.png
--rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/link.svg
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/list-item.png
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/map.png
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/mobile-menu.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/phone.png
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/print.svg
--rw-rw-rw-   0 root         (0) root         (0)     4315 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/search.png
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/css/img/social-icons.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/js/dev/
--rw-rw-rw-   0 root         (0) root         (0)  2392493 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/mscapp.js
--rw-rw-rw-   0 root         (0) root         (0)  2948389 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/mscapp.js.map
--rw-rw-rw-   0 root         (0) root         (0)     4652 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js
--rw-rw-rw-   0 root         (0) root         (0)     4686 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    10624 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
--rw-rw-rw-   0 root         (0) root         (0)     6409 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)    19333 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js
--rw-rw-rw-   0 root         (0) root         (0)    29675 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   209738 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js
--rw-rw-rw-   0 root         (0) root         (0)   236865 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   182041 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js
--rw-rw-rw-   0 root         (0) root         (0)   230602 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map
--rw-rw-rw-   0 root         (0) root         (0)   181575 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js
--rw-rw-rw-   0 root         (0) root         (0)   230045 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map
--rw-rw-rw-   0 root         (0) root         (0)   174144 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js
--rw-rw-rw-   0 root         (0) root         (0)   220941 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map
--rw-rw-rw-   0 root         (0) root         (0)    21983 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
--rw-rw-rw-   0 root         (0) root         (0)    18395 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)    18911 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js
--rw-rw-rw-   0 root         (0) root         (0)    20127 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   450498 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js
--rw-rw-rw-   0 root         (0) root         (0)   569896 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    46418 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js
--rw-rw-rw-   0 root         (0) root         (0)    53162 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)   153997 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js
--rw-rw-rw-   0 root         (0) root         (0)   189149 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   114212 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js
--rw-rw-rw-   0 root         (0) root         (0)   139871 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/pkg/js/dist/
--rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/116.js
--rw-rw-rw-   0 root         (0) root         (0)     8340 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/137.js
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/178.js
--rw-rw-rw-   0 root         (0) root         (0)    67548 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/23.js
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/23.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)   148911 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/243.js
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/243.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    16009 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/274.js
--rw-rw-rw-   0 root         (0) root         (0)     3221 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/284.js
--rw-rw-rw-   0 root         (0) root         (0)    69465 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/458.js
--rw-rw-rw-   0 root         (0) root         (0)     3219 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/47.js
--rw-rw-rw-   0 root         (0) root         (0)   148911 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/481.js
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/481.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70252 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/528.js
--rw-rw-rw-   0 root         (0) root         (0)     1457 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/528.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70026 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/612.js
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/612.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    16008 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/623.js
--rw-rw-rw-   0 root         (0) root         (0)    61493 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/624.js
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/624.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)   105878 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/660.js
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/660.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/671.js
--rw-rw-rw-   0 root         (0) root         (0)    69464 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/686.js
--rw-rw-rw-   0 root         (0) root         (0)    61491 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/698.js
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/698.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70252 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/814.js
--rw-rw-rw-   0 root         (0) root         (0)     1457 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/814.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    18213 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/830.js
--rw-rw-rw-   0 root         (0) root         (0)     1859 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/854.js
--rw-rw-rw-   0 root         (0) root         (0)     1858 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/860.js
--rw-rw-rw-   0 root         (0) root         (0)    18213 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/882.js
--rw-rw-rw-   0 root         (0) root         (0)   937336 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/mscapp.js
--rw-rw-rw-   0 root         (0) root         (0)     1770 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/pkg/js/dist/mscapp.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3871 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/
--rw-rw-rw-   0 root         (0) root         (0)     1188 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1605 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1268 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/
--rw-rw-rw-   0 root         (0) root         (0)     1027 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2428 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1257 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1828 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/doctests/
--rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/
--rw-rw-rw-   0 root         (0) root         (0)    12350 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4204 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/container.py
--rw-rw-rw-   0 root         (0) root         (0)     9596 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4366 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/reminder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6130 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/templates/booking-ok.pt
--rw-rw-rw-   0 root         (0) root         (0)     3861 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    34191 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15231 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/home.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1094 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/reminder.py
--rw-rw-rw-   0 root         (0) root         (0)     8133 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     2300 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3080 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt
--rw-rw-rw-   0 root         (0) root         (0)    38087 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/
--rw-rw-rw-   0 root         (0) root         (0)     1816 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2258 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/oauth/
--rw-rw-rw-   0 root         (0) root         (0)     2036 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/oauth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/oauth/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3332 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/oauth/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/
--rw-rw-rw-   0 root         (0) root         (0)     3511 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5672 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    12615 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8006 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15941 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2395 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/
--rw-rw-rw-   0 root         (0) root         (0)     3428 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4090 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2631 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7142 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/password.py
--rw-rw-rw-   0 root         (0) root         (0)    11384 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/register.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      642 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/password-final.pt
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt
--rw-rw-rw-   0 root         (0) root         (0)     6337 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    11638 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/
--rw-rw-rw-   0 root         (0) root         (0)    20552 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   167336 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0 root         (0) root         (0)   167000 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf
--rw-rw-rw-   0 root         (0) root         (0)   168644 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/
--rw-rw-rw-   0 root         (0) root         (0)    17171 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/api/
--rw-rw-rw-   0 root         (0) root         (0)     2850 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/api/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7788 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4826 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/zmi/lookup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/generations/
--rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8628 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/include.py
--rw-rw-rw-   0 root         (0) root         (0)     2375 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    61512 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo
--rw-rw-rw-   0 root         (0) root         (0)   105688 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po
--rw-rw-rw-   0 root         (0) root         (0)    74943 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/locales/pyams_app_msc.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/reference/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/reference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/reference/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/reference/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1218 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/reference/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/root/
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/root/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/root/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/root/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1750 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/root/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/
--rw-rw-rw-   0 root         (0) root         (0)     4447 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/api/
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1862 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/index.py
--rw-rw-rw-   0 root         (0) root         (0)     4591 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2381 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2027 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/page.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4485 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3476 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt
--rw-rw-rw-   0 root         (0) root         (0)     2050 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/search.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/security.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3704 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     6790 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8269 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3360 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/
--rw-rw-rw-   0 root         (0) root         (0)     8288 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2950 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/price.py
--rw-rw-rw-   0 root         (0) root         (0)     1906 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4330 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/audience.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    12262 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/audience.py
--rw-rw-rw-   0 root         (0) root         (0)     4080 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     2938 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/price.py
--rw-rw-rw-   0 root         (0) root         (0)     2494 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/room.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/page.py
--rw-rw-rw-   0 root         (0) root         (0)     4262 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/price.py
--rw-rw-rw-   0 root         (0) root         (0)     4216 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/room.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/session.py
--rw-rw-rw-   0 root         (0) root         (0)     5536 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    12429 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9666 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/audience.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5472 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     3713 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/planning.py
--rw-rw-rw-   0 root         (0) root         (0)     3108 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/presentation.py
--rw-rw-rw-   0 root         (0) root         (0)     9318 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/price.py
--rw-rw-rw-   0 root         (0) root         (0)     1554 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/restrictions.py
--rw-rw-rw-   0 root         (0) root         (0)     9175 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/room.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     2927 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/session.py
--rw-rw-rw-   0 root         (0) root         (0)     3243 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/types.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1726 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/form.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/layer.py
--rw-rw-rw-   0 root         (0) root         (0)     5255 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/
--rw-rw-rw-   0 root         (0) root         (0)    11860 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_form.js
--rw-rw-rw-   0 root         (0) root         (0)     5731 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_gis.js
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_i18n.js
--rw-rw-rw-   0 root         (0) root         (0)     1460 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_search.js
--rw-rw-rw-   0 root         (0) root         (0)     9714 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_utils.js
--rw-rw-rw-   0 root         (0) root         (0)     4237 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/app.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      170 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/i18n/fr.js
--rw-rw-rw-   0 root         (0) root         (0)      210 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/mscapp.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_breadcrumbs.scss
--rw-rw-rw-   0 root         (0) root         (0)      320 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_carousel.scss
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_content.scss
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_footer.scss
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)     3047 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_layout.scss
--rw-rw-rw-   0 root         (0) root         (0)      275 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_list.scss
--rw-rw-rw-   0 root         (0) root         (0)     4416 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_misc.scss
--rw-rw-rw-   0 root         (0) root         (0)      960 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_search.scss
--rw-rw-rw-   0 root         (0) root         (0)     4329 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/msc.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      788 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/skin/templates/select-admin-theater.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/tests/
--rw-rw-rw-   0 root         (0) root         (0)      802 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    20672 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/resources/js/msc.js
--rw-rw-rw-   0 root         (0) root         (0)     8006 2024-04-10 07:48:50.000000 pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/resources/js/msc.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2004 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12885 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:49:12.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      677 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-10 07:49:17.000000 pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1664 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/docs/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/docs/booking.puml
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/docs/classes.puml
+-rw-rw-rw-   0 root         (0) root         (0)    16507 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/docs/es-mapping.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/assets/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/clock.png
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/email.png
+-rw-rw-rw-   0 root         (0) root         (0)   207972 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-brands-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   117372 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-brands-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    68004 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-regular-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    25452 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-regular-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)   419720 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-solid-900.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   156496 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-solid-900.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    10832 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-v4compatibility.ttf
+-rw-rw-rw-   0 root         (0) root         (0)     4792 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-v4compatibility.woff2
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/form.png
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/layers-2x.png
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/layers.png
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/list-item.png
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/map.png
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/marker-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/mobile-menu.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/phone.png
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/select2-spinner.gif
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/select2.png
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/select2x2.png
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/social-icons.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/css/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/css/dev/
+-rw-rw-rw-   0 root         (0) root         (0)   263831 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/dev/msc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/css/dist/
+-rw-rw-rw-   0 root         (0) root         (0)   337917 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/dist/msc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/css/img/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/clock.png
+-rw-rw-rw-   0 root         (0) root         (0)      880 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/download.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/email.png
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/form.png
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/link.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/list-item.png
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/map.png
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/mobile-menu.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/phone.png
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/print.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/search.png
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/social-icons.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/js/dev/
+-rw-rw-rw-   0 root         (0) root         (0)  2392493 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/mscapp.js
+-rw-rw-rw-   0 root         (0) root         (0)  2948389 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/mscapp.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     4652 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    10624 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
+-rw-rw-rw-   0 root         (0) root         (0)     6409 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    19333 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    29675 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   209738 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   236865 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   182041 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js
+-rw-rw-rw-   0 root         (0) root         (0)   230602 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   181575 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js
+-rw-rw-rw-   0 root         (0) root         (0)   230045 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   174144 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js
+-rw-rw-rw-   0 root         (0) root         (0)   220941 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    21983 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
+-rw-rw-rw-   0 root         (0) root         (0)    18395 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    18911 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   450498 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   569896 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    46418 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js
+-rw-rw-rw-   0 root         (0) root         (0)    53162 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   153997 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   189149 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   114212 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   139871 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/js/dist/
+-rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/116.js
+-rw-rw-rw-   0 root         (0) root         (0)     8340 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/137.js
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/178.js
+-rw-rw-rw-   0 root         (0) root         (0)    67548 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/23.js
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/23.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)   148911 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/243.js
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/243.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    16009 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/274.js
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/284.js
+-rw-rw-rw-   0 root         (0) root         (0)    69465 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/458.js
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/47.js
+-rw-rw-rw-   0 root         (0) root         (0)   148911 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/481.js
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/481.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70252 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/528.js
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/528.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70026 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/612.js
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/612.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    16008 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/623.js
+-rw-rw-rw-   0 root         (0) root         (0)    61493 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/624.js
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/624.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)   105878 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/660.js
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/660.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/671.js
+-rw-rw-rw-   0 root         (0) root         (0)    69464 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/686.js
+-rw-rw-rw-   0 root         (0) root         (0)    61491 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/698.js
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/698.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70252 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/814.js
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/814.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    18213 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/830.js
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/854.js
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/860.js
+-rw-rw-rw-   0 root         (0) root         (0)    18213 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/882.js
+-rw-rw-rw-   0 root         (0) root         (0)   937336 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/mscapp.js
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/mscapp.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3871 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2428 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/zmi/container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/
+-rw-rw-rw-   0 root         (0) root         (0)    12350 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     9708 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4366 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/reminder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6130 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/templates/booking-ok.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3861 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    36201 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15231 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/home.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/reminder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8133 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3121 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt
+-rw-rw-rw-   0 root         (0) root         (0)    38087 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/oauth/
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/oauth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/oauth/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3332 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/oauth/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/
+-rw-rw-rw-   0 root         (0) root         (0)     3511 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5672 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    12100 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8006 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16194 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/
+-rw-rw-rw-   0 root         (0) root         (0)     3975 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7142 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/password.py
+-rw-rw-rw-   0 root         (0) root         (0)    11384 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/register.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      642 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/password-final.pt
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt
+-rw-rw-rw-   0 root         (0) root         (0)     6337 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12105 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/
+-rw-rw-rw-   0 root         (0) root         (0)    20552 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   167336 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   167000 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   168644 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/
+-rw-rw-rw-   0 root         (0) root         (0)    17688 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/api/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7788 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4826 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/zmi/lookup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8674 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     2375 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    62537 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo
+-rw-rw-rw-   0 root         (0) root         (0)   107792 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po
+-rw-rw-rw-   0 root         (0) root         (0)    76407 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/locales/pyams_app_msc.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3216 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/root/
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/root/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/root/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/root/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/root/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     4591 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2381 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/page.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4485 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2050 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/security.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     6790 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8269 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6079 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/
+-rw-rw-rw-   0 root         (0) root         (0)     8410 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4330 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/audience.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    12262 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/audience.py
+-rw-rw-rw-   0 root         (0) root         (0)     4080 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/room.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/page.py
+-rw-rw-rw-   0 root         (0) root         (0)     4262 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     4216 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/room.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12679 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9666 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/audience.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     5472 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3642 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/planning.py
+-rw-rw-rw-   0 root         (0) root         (0)     3108 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/presentation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9318 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9175 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/room.py
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     3618 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4526 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5255 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/
+-rw-rw-rw-   0 root         (0) root         (0)    11860 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_form.js
+-rw-rw-rw-   0 root         (0) root         (0)     5731 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_gis.js
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_i18n.js
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_search.js
+-rw-rw-rw-   0 root         (0) root         (0)     9714 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     4237 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/app.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/i18n/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/mscapp.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_breadcrumbs.scss
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_carousel.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_content.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_footer.scss
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_layout.scss
+-rw-rw-rw-   0 root         (0) root         (0)      275 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_list.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4416 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_misc.scss
+-rw-rw-rw-   0 root         (0) root         (0)      960 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_search.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4329 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/msc.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      788 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/templates/select-admin-theater.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/img/
+-rw-rw-rw-   0 root         (0) root         (0)     4680 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/img/pass-culture.webp
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    21353 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/js/msc.js
+-rw-rw-rw-   0 root         (0) root         (0)     8471 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/js/msc.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13305 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:45:11.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      677 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/top_level.txt
```

### Comparing `pyams_app_msc-1.99.1/LICENSE` & `pyams_app_msc-1.99.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/PKG-INFO` & `pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams_app_msc
-Version: 1.99.1
+Name: pyams-app-msc
+Version: 1.99.2
 Summary: PyAMS application for cinema reservation management
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -44,14 +44,43 @@
 PyAMS MSC application is a french web application ("Ma Séance Cinéma") which is used to manage sessions
 and bookings in movies theaters.
 
 
 Changelog
 =========
 
+1.99.2
+------
+ - updated menus order
+ - added paragraphs factory settings support to movie theater
+ - updated booking recipient label
+ - added structure type attribute to user profile
+ - disable autocomplete on user profile creation form
+ - added structures types references table
+ - renamed MSC skin
+ - updated movie theater breadcrumbs
+ - added marker interface to user dashboard views
+ - updated translations
+ - updated session seats
+ - updated session label adapter
+ - added button in booking add form to automatically redirect to validation form after creation
+ - updated AJAX finder URL to only get activities declared inside movie theater
+ - removed unused fields from address
+ - added tooltips on calendar events
+ - added permission and role to manage references tables
+ - allow theater manager to assign role to other managers
+ - include TMDB images as gallery paragraph instead of global gallery
+ - removed gallery support on catalog entries
+ - disabled paragraphs associations menu
+ - updated illustrations adapters
+ - updated activity types forms (fixes issue #6)
+ - added condition on bookings button display
+ - added missing picture to Git
+ - updated theater planning menu position
+
 1.99.1
 ------
  - added edit forms content getters
  - added custom catalog entry roles adapters
  - removed roles restrictions menu entries from theater navigation menu
  - removed source folder from movie theater activity types properties (issue #6)
  - changed reminder delay unit from hours to days (issue #4]
```

### Comparing `pyams_app_msc-1.99.1/docs/README.rst` & `pyams_app_msc-1.99.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/docs/classes.puml` & `pyams_app_msc-1.99.2/docs/classes.puml`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/docs/es-mapping.json` & `pyams_app_msc-1.99.2/docs/es-mapping.json`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/clock.png` & `pyams_app_msc-1.99.2/pkg/assets/clock.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/email.png` & `pyams_app_msc-1.99.2/pkg/assets/email.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/fa-brands-400.ttf` & `pyams_app_msc-1.99.2/pkg/assets/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/fa-brands-400.woff2` & `pyams_app_msc-1.99.2/pkg/assets/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/fa-regular-400.ttf` & `pyams_app_msc-1.99.2/pkg/assets/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/fa-regular-400.woff2` & `pyams_app_msc-1.99.2/pkg/assets/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/fa-solid-900.ttf` & `pyams_app_msc-1.99.2/pkg/assets/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/fa-solid-900.woff2` & `pyams_app_msc-1.99.2/pkg/assets/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/fa-v4compatibility.ttf` & `pyams_app_msc-1.99.2/pkg/assets/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/fa-v4compatibility.woff2` & `pyams_app_msc-1.99.2/pkg/assets/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/form.png` & `pyams_app_msc-1.99.2/pkg/assets/form.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/layers-2x.png` & `pyams_app_msc-1.99.2/pkg/assets/layers-2x.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/layers.png` & `pyams_app_msc-1.99.2/pkg/assets/layers.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/list-item.png` & `pyams_app_msc-1.99.2/pkg/assets/list-item.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/map.png` & `pyams_app_msc-1.99.2/pkg/assets/map.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/marker-icon.png` & `pyams_app_msc-1.99.2/pkg/assets/marker-icon.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/mobile-menu.png` & `pyams_app_msc-1.99.2/pkg/assets/mobile-menu.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/phone.png` & `pyams_app_msc-1.99.2/pkg/assets/phone.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/select2-spinner.gif` & `pyams_app_msc-1.99.2/pkg/assets/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/select2.png` & `pyams_app_msc-1.99.2/pkg/assets/select2.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/select2x2.png` & `pyams_app_msc-1.99.2/pkg/assets/select2x2.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/assets/social-icons.png` & `pyams_app_msc-1.99.2/pkg/assets/social-icons.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/css/dev/msc.css` & `pyams_app_msc-1.99.2/pkg/css/dev/msc.css`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/css/dist/msc.css` & `pyams_app_msc-1.99.2/pkg/css/dist/msc.css`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/css/img/clock.png` & `pyams_app_msc-1.99.2/pkg/css/img/clock.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/css/img/download.svg` & `pyams_app_msc-1.99.2/pkg/css/img/download.svg`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/css/img/email.png` & `pyams_app_msc-1.99.2/pkg/css/img/email.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/css/img/form.png` & `pyams_app_msc-1.99.2/pkg/css/img/form.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/css/img/list-item.png` & `pyams_app_msc-1.99.2/pkg/css/img/list-item.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/css/img/map.png` & `pyams_app_msc-1.99.2/pkg/css/img/map.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/css/img/mobile-menu.png` & `pyams_app_msc-1.99.2/pkg/css/img/mobile-menu.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/css/img/phone.png` & `pyams_app_msc-1.99.2/pkg/css/img/phone.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/css/img/search.png` & `pyams_app_msc-1.99.2/pkg/css/img/search.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/css/img/social-icons.png` & `pyams_app_msc-1.99.2/pkg/css/img/social-icons.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/mscapp.js` & `pyams_app_msc-1.99.2/pkg/js/dev/mscapp.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/mscapp.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/mscapp.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js` & `pyams_app_msc-1.99.2/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js` & `pyams_app_msc-1.99.2/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js` & `pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js` & `pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map` & `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/116.js` & `pyams_app_msc-1.99.2/pkg/js/dist/116.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/137.js` & `pyams_app_msc-1.99.2/pkg/js/dist/137.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/23.js` & `pyams_app_msc-1.99.2/pkg/js/dist/23.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/23.js.LICENSE.txt` & `pyams_app_msc-1.99.2/pkg/js/dist/23.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/243.js` & `pyams_app_msc-1.99.2/pkg/js/dist/243.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/274.js` & `pyams_app_msc-1.99.2/pkg/js/dist/274.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/284.js` & `pyams_app_msc-1.99.2/pkg/js/dist/284.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/458.js` & `pyams_app_msc-1.99.2/pkg/js/dist/458.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/47.js` & `pyams_app_msc-1.99.2/pkg/js/dist/47.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/481.js` & `pyams_app_msc-1.99.2/pkg/js/dist/481.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/528.js` & `pyams_app_msc-1.99.2/pkg/js/dist/528.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/528.js.LICENSE.txt` & `pyams_app_msc-1.99.2/pkg/js/dist/528.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/612.js` & `pyams_app_msc-1.99.2/pkg/js/dist/612.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/612.js.LICENSE.txt` & `pyams_app_msc-1.99.2/pkg/js/dist/612.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/623.js` & `pyams_app_msc-1.99.2/pkg/js/dist/623.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/624.js` & `pyams_app_msc-1.99.2/pkg/js/dist/624.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/660.js` & `pyams_app_msc-1.99.2/pkg/js/dist/660.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/686.js` & `pyams_app_msc-1.99.2/pkg/js/dist/686.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/698.js` & `pyams_app_msc-1.99.2/pkg/js/dist/698.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/814.js` & `pyams_app_msc-1.99.2/pkg/js/dist/814.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/814.js.LICENSE.txt` & `pyams_app_msc-1.99.2/pkg/js/dist/814.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/830.js` & `pyams_app_msc-1.99.2/pkg/js/dist/830.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/854.js` & `pyams_app_msc-1.99.2/pkg/js/dist/854.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/860.js` & `pyams_app_msc-1.99.2/pkg/js/dist/860.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/882.js` & `pyams_app_msc-1.99.2/pkg/js/dist/882.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/mscapp.js` & `pyams_app_msc-1.99.2/pkg/js/dist/mscapp.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/pkg/js/dist/mscapp.js.LICENSE.txt` & `pyams_app_msc-1.99.2/pkg/js/dist/mscapp.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/setup.py` & `pyams_app_msc-1.99.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.99.1'
+version = '1.99.2'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 data_dir = 'pkg'
 data_files = [(d, [os.path.join(d, f) for f in files])
               for d, folders, files in os.walk(data_dir)]
 
 tests_require = [
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,12 @@
 __docformat__ = 'restructuredtext'
 
 
 @factory_config(IAddress)
 class Address(Persistent):
     """Address persistent class"""
 
-    apartment = FieldProperty(IAddress['apartment'])
-    entry = FieldProperty(IAddress['entry'])
     street = FieldProperty(IAddress['street'])
     locality = FieldProperty(IAddress['locality'])
     postal_code = FieldProperty(IAddress['postal_code'])
     city = FieldProperty(IAddress['city'])
     comments = FieldProperty(IAddress['comments'])
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/interfaces.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,22 +21,14 @@
 
 from pyams_app_msc import _
 
 
 class IAddress(Interface):
     """Address interface"""
 
-    apartment = TextLine(title=_("Apartment"),
-                         description=_("Floor, corridor..."),
-                         required=False)
-
-    entry = TextLine(title=_("Entry"),
-                     description=_("Entry, building, residence..."),
-                     required=False)
-
     street = TextLine(title=_("Number and street"),
                       description=_("Entry number and street name"),
                       required=False)
 
     locality = TextLine(title=_("Locality"),
                         required=False)
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/address/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/admininfo/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/banking/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/contact/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/schema.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/component/duration/zmi/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/container.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/container.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from ZODB.interfaces import IConnection
 
 from pyams_app_msc.feature.booking import BOOKING_STATUS
 from pyams_app_msc.feature.booking.interfaces import BOOKING_CONTAINER_KEY, IBookingContainer, \
     IBookingTarget, OCCUPIED_BOOKING_STATUS, REQUESTED_BOOKING_STATUS
 from pyams_app_msc.feature.planning.interfaces import ISession
 from pyams_app_msc.feature.planning.session import Session
+from pyams_app_msc.feature.profile.interfaces import SEATS_DISPLAY_MODE
 from pyams_catalog.utils import index_object
 from pyams_utils.adapter import ContextAdapter, adapter_config, get_annotation_adapter
 from pyams_utils.factory import factory_config
 from pyams_utils.interfaces import ICacheKeyValue
 from pyams_utils.traversing import get_parent
 from pyams_utils.zodb import volatile_property
 
@@ -77,14 +78,27 @@
         ))
 
     @property
     def free_seats(self):
         """Free seats getter"""
         return (self.session.capacity or 0) - self.get_confirmed_seats()
 
+    def get_seats(self, display_mode):
+        """Get total number of seats according to given display mode"""
+        if display_mode == SEATS_DISPLAY_MODE.TOTAL.value:
+            return (f'{self.get_confirmed_seats()} / '
+                    f'{self.get_requested_seats()} / '
+                    f'{self.session.capacity}')
+        if display_mode == SEATS_DISPLAY_MODE.WAITING.value:
+            return (f'{self.get_confirmed_seats()} / '
+                    f'{self.get_waiting_seats()} / '
+                    f'{self.session.capacity}')
+        return (f'{self.get_confirmed_seats()} / '
+                f'{self.session.capacity}')
+
 
 @adapter_config(required=IBookingTarget,
                 provides=IBookingContainer)
 def session_booking_container(context):
     """Session booking container adapter"""
     return get_annotation_adapter(context, BOOKING_CONTAINER_KEY, IBookingContainer,
                                   name='++booking++')
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,14 +260,17 @@
     def get_confirmed_seats(self):
         """Get number of confirmed reserved seats"""
 
     free_seats = Int(title=_("Free seats"),
                      description=_("Number of free seats for this session"),
                      readonly=True)
 
+    def get_seats(self, display_mode):
+        """Get total number of seats according to given display mode"""
+
 
 class IBookingTarget(IAttributeAnnotatable):
     """Booking target marker interface"""
 
 
 class IBookingReminderTask(ITask):
     """Booking reminder task interface"""
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/reminder.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/reminder.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/task.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 
 from pyams_app_msc.feature.booking import get_booking_message_values
 from pyams_app_msc.feature.booking.interfaces import BOOKING_STATUS, BOOKING_STATUS_VOCABULARY, IBookingContainer, \
     IBookingInfo, IBookingTarget
 from pyams_app_msc.feature.booking.zmi.interfaces import IBookingContainerTable, IBookingContainerView, IBookingForm
 from pyams_app_msc.feature.messaging import IMessagingSettings
 from pyams_app_msc.feature.planning.interfaces import ISession
-from pyams_app_msc.feature.profile import IUserProfile, USER_PROFILE_KEY
+from pyams_app_msc.feature.profile import IOperatorProfile, IUserProfile, USER_PROFILE_KEY
+from pyams_app_msc.feature.profile.interfaces import SEATS_DISPLAY_MODE
 from pyams_app_msc.feature.profile.zmi.widget import PrincipalSelectFieldWidget
 from pyams_app_msc.interfaces import MANAGE_BOOKING_PERMISSION, VIEW_BOOKING_PERMISSION
 from pyams_app_msc.shared.theater import IMovieTheater, IMovieTheaterSettings
 from pyams_app_msc.shared.theater.api.interfaces import MSC_PRICE_API_PATH, MSC_PRICE_API_ROUTE
 from pyams_app_msc.shared.theater.interfaces.mail import IMailTemplates
 from pyams_app_msc.zmi import msc
 from pyams_content.feature.history import IHistoryContainer
@@ -68,15 +69,15 @@
 from pyams_utils.traversing import get_parent
 from pyams_utils.url import absolute_url
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.form import AdminModalAddForm, AdminModalDisplayForm, AdminModalEditForm, \
     FormGroupChecker, SimpleAddFormRenderer, SimpleEditFormRenderer
 from pyams_zmi.helper.container import delete_container_element
 from pyams_zmi.interfaces import IAdminLayer, IObjectLabel, TITLE_SPAN_BREAK
-from pyams_zmi.interfaces.form import IFormTitle, IModalDisplayFormButtons, check_submit_button
+from pyams_zmi.interfaces.form import IFormTitle, IModalAddFormButtons, IModalDisplayFormButtons, check_submit_button
 from pyams_zmi.interfaces.table import ITableElementEditor, ITableWithActions
 from pyams_zmi.interfaces.viewlet import IToolbarViewletManager
 from pyams_zmi.table import I18nColumnMixin, IconColumn, InnerTableAdminView, NameColumn, Table, TableElementEditor, \
     TrashColumn
 from pyams_zmi.utils import get_object_hint, get_object_label
 
 __docformat__ = 'restructuredtext'
@@ -281,15 +282,26 @@
 @pagelet_config(name='bookings.html',
                 context=IBookingTarget, layer=IPyAMSLayer,
                 permission=VIEW_BOOKING_PERMISSION)
 @implementer(IBookingContainerView)
 class BookingContainerModalView(AdminModalDisplayForm):
     """Booking target container modal view"""
 
-    subtitle = _("Session bookings")
+    @property
+    def subtitle(self):
+        """Subtitle getter"""
+        translate = self.request.localizer.translate
+        subtitle = translate(_("Session bookings"))
+        profile = IOperatorProfile(self.request)
+        if profile.session_seats_display_mode != SEATS_DISPLAY_MODE.NONE.value:
+            container = IBookingContainer(self.context)
+            if container is not None:
+                subtitle += translate(_(" (Seats: {})")).format(container.get_seats(profile.session_seats_display_mode))
+        return subtitle
+
     modal_class = 'modal-xl'
 
 
 @adapter_config(required=(IBookingTarget, IAdminLayer, IBookingContainerView),
                 provides=IFormTitle)
 def booking_target_edit_form_title(context, request, form):
     """Booking target edit form title"""
@@ -311,15 +323,16 @@
 def get_booking_label(context, request, view):
     """Booking label getter"""
     recipient = get_principal(request, context.recipient)
     result = recipient.title
     profile_info = IUserProfile(recipient, None)
     if (profile_info is None) or not profile_info.establishment:
         return result
-    return f'{result} ({profile_info.establishment})'
+    return (f'{result} ({profile_info.get_structure_type()} - '
+            f'{profile_info.establishment}, {profile_info.establishment_address.city})')
 
 
 @viewlet_config(name='add-booking.action',
                 context=IBookingTarget, layer=IAdminLayer,
                 view=IBookingContainerTable,
                 manager=IToolbarViewletManager, weigth=20,
                 permission=MANAGE_BOOKING_PERMISSION)
@@ -335,28 +348,38 @@
             return None
         return ContextAddAction.__new__(cls)
 
     def get_href(self):
         return absolute_url(self.context, self.request, f'++booking++/{self.href}')
 
 
+class IBookingAddFormButtons(IModalAddFormButtons):
+    """Booking add form buttons"""
+
+    validate = SubmitButton(name='validate',
+                            title=_("Add and accept"),
+                            condition=check_submit_button)
+
+
 @ajax_form_config(name='add-booking.html',
                   context=IBookingContainer, layer=IPyAMSLayer,
                   permission=MANAGE_BOOKING_PERMISSION)
 class BookingAddForm(AdminModalAddForm):
     """Booking add form"""
 
     subtitle = _("New booking")
     legend = _("New booking properties")
 
     fields = Fields(IBookingInfo).select('recipient', 'status',
                                          'nb_participants', 'nb_accompanists',
                                          'nb_groups', 'price', 'accompanying_ratio',
                                          'cultural_pass', 'comments', 'notepad')
     fields['recipient'].widget_factory = PrincipalSelectFieldWidget
+    buttons = Buttons(IBookingAddFormButtons).select('add', 'validate', 'close')
+
     content_factory = IBookingInfo
 
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         status = self.widgets.get('status')
         if status is not None:
             status.mode = DISPLAY_MODE
@@ -376,14 +399,20 @@
                                                        MSC_PRICE_API_PATH).format(
                         theater_name=theater.__name__),
                 'ams-select2-helper-argument': 'price_id',
                 'ams-select2-helper-callback': 'MyAMS.msc.booking.priceChanged'
             }
             alsoProvides(price, IObjectData)
 
+    def update_actions(self):
+        super().update_actions()
+        validate  =self.actions.get('validate')
+        if validate is not None:
+            validate.add_class('btn-info')
+
     def update_content(self, obj, data):
         form_data = data.get(self, data)
         if form_data.get('notepad'):
             history = IHistoryContainer(obj, None)
             if history is not None:
                 history.add_history(obj,
                                     comment=form_data.get('notepad'),
@@ -391,14 +420,22 @@
         changes = super().update_content(obj, data)
         obj.creator = self.request.principal.id
         return changes
 
     def add(self, obj):
         IBookingContainer(self.context).append(obj)
 
+    @handler(IBookingAddFormButtons['add'])
+    def handle_add(self, action):
+        return super().handle_add(self, action)
+
+    @handler(IBookingAddFormButtons['validate'])
+    def handle_validate(self, action):
+        return self.handle_add(self, action)
+
 
 @adapter_config(required=(IBookingContainer, IAdminLayer, BookingAddForm),
                 provides=IFormTitle)
 def booking_add_form_title(context, request, form):
     """Booking add form title"""
     session = get_parent(context, ISession)
     return booking_target_edit_form_title(session, request, form)
@@ -419,14 +456,28 @@
                 'options': {
                     'room_id': ISession(self.context).room
                 }
             })
         return result
 
 
+@adapter_config(name='validate',
+                required=(IBookingContainer, IAdminLayer, BookingAddForm),
+                provides=IAJAXFormRenderer)
+class BookingAddFormValidateRenderer(BookingAddFormRenderer):
+    """Booking add form validate button renderer"""
+
+    def render(self, changes):
+        result = super().render(changes)
+        if changes:
+            result['status'] = 'modal'
+            result['location'] = absolute_url(changes, self.request, 'booking-accept.html')
+        return result
+
+
 @adapter_config(required=(IBookingInfo, IAdminLayer, IBookingContainerTable),
                 provides=ITableElementEditor)
 class BookingInfoEditor(TableElementEditor):
     """Booking info editor"""
 
 
 @adapter_config(required=(IBookingInfo, IAdminLayer, IBookingForm),
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/dashboard.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/home.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/home.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/reminder.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/reminder.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/search.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/task.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 					 tal:define="items view.get_bookings(session);
 								 (has_bookings, bookings) tales:boolean_iter(items)">
 					<tal:loop repeat="booking bookings">
 						<div class="card-title"
 							 tal:define="(principal, profile) booking.get_recipient()">
 							<a class="text-dark"
 							   href="${tales:absolute_url(booking, 'properties.html')}" data-toggle="modal">
-								${profile.establishment} (${profile.establishment_address.city}) - <strong>${principal.title}</strong>
+								${profile.establishment}
+								(${profile.get_structure_type()}, ${profile.establishment_address.city}) - <strong>${principal.title}</strong>
 							</a>
 							<tal:if condition="booking.cultural_pass">
 								<img title="Cultural pass" alt="" i18n:attributes="title"
 									 class="position-absolute mx-3 mt-n2 hint"
 									 src="/--static--/msc/img/pass-culture.webp"
 									 width="32" height="32" />
 							</tal:if><br />
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/booking/zmi/workflow.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/messaging/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/oauth/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/oauth/skin/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/oauth/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/session.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from pyams_utils.date import SH_TIME_FORMAT, format_date, format_time
 from pyams_utils.factory import factory_config, get_interface_base_name
 from pyams_utils.interfaces import ICacheKeyValue, MISSING_INFO
 from pyams_utils.timezone import tztime
 from pyams_utils.traversing import get_parent
 from pyams_utils.url import absolute_url
 from pyams_workflow.interfaces import IWorkflowVersions
-from pyams_zmi.interfaces import IObjectLabel
+from pyams_zmi.interfaces import IObjectLabel, SMALL_TITLE_SPAN_BREAK
 from pyams_zmi.utils import get_object_label
 
 __docformat__ = 'restructuredtext'
 
 from pyams_app_msc import _
 
 
@@ -147,16 +147,20 @@
 @adapter_config(required=(ISession, IPyAMSLayer, Interface),
                 provides=IObjectLabel)
 def get_session_label(context, request, view, formatter='html'):
     """Session label getter"""
     translate = request.localizer.translate
     target = context.get_target()
     rooms = getVocabularyRegistry().get(context, ROOMS_VOCABULARY)
-    return ('<small>{}</small><br />{}' if formatter == 'html' else '{} - {}').format(
-        get_object_label(target, request, view),
+    if IMovieTheater.providedBy(target):
+        label = translate(_("Out of catalog activity"))
+    else:
+        label = get_object_label(target, request, view)
+    return (SMALL_TITLE_SPAN_BREAK if formatter == 'html' else '{} - {}').format(
+        label,
         translate(_("{room} - {date} from {start_time} to {end_time}")).format(
             room=rooms.by_value.get(context.room).title,
             date=format_date(context.start_date),
             start_time=format_time(context.start_date, SH_TIME_FORMAT),
             end_time=format_time(context.end_date, SH_TIME_FORMAT)
         ))
 
@@ -229,28 +233,15 @@
         if not self.context.bookable:
             return value
         profile = IOperatorProfile(self.request)
         if profile.session_seats_display_mode == SEATS_DISPLAY_MODE.NONE.value:
             return f'{value} \n'
         else:
             container = IBookingContainer(self.context)
-            if profile.session_seats_display_mode == SEATS_DISPLAY_MODE.TOTAL.value:
-                return (f'{value} \n'
-                        f'({container.get_confirmed_seats()} / '
-                        f'{container.get_requested_seats()} / '
-                        f'{self.context.capacity})')
-            if profile.session_seats_display_mode == SEATS_DISPLAY_MODE.WAITING.value:
-                return (f'{value} \n'
-                        f'({container.get_confirmed_seats()} / '
-                        f'{container.get_waiting_seats()} / '
-                        f'{self.context.capacity})')
-            return (f'{value} \n'
-                    f'({container.get_confirmed_seats()} / '
-                    f'{self.context.capacity})')
-
+            return f'{value} \n({container.get_seats(profile.session_seats_display_mode)})'
 
     def convert_content(self, **params):
         result = super().convert_content(**params)
         context = self.context
         request = self.request
         result['id'] = ICacheKeyValue(context)
         result['href'] = absolute_url(context, request)
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/session.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from pyramid.view import view_config
 from zope.copy import copy
 from zope.interface import Invalid
 from zope.lifecycleevent import ObjectModifiedEvent
 
 from pyams_app_msc.feature.booking import IBookingContainer
 from pyams_app_msc.feature.planning.interfaces import IPlanning, IPlanningTarget, ISession, IWfPlanningTarget
-from pyams_app_msc.interfaces import MANAGE_PLANNING_PERMISSION, VIEW_PLANNING_PERMISSION
+from pyams_app_msc.interfaces import MANAGE_PLANNING_PERMISSION, VIEW_BOOKING_PERMISSION, VIEW_PLANNING_PERMISSION
 from pyams_app_msc.shared.catalog.interfaces import ICatalogEntryInfo, IWfCatalogEntry
 from pyams_app_msc.shared.theater.interfaces import IMovieTheater, IMovieTheaterSettings
 from pyams_app_msc.shared.theater.interfaces.room import ICinemaRoomContainer
 from pyams_content_api.feature.json.interfaces import IJSONExporter
 from pyams_form.ajax import ajax_form_config
 from pyams_form.button import Buttons, handler
 from pyams_form.field import Fields
@@ -153,24 +153,30 @@
                     'event': exporter.to_json(with_edit_info=True,
                                               edit_context=IPlanning(self.context))
                 }
             }]
         }
 
 
+def can_view_bookings(form):
+    """Check if session bookings can be viewed"""
+    return form.request.has_permission(VIEW_BOOKING_PERMISSION, context=form.context)
+
+    
 def can_delete_session(form):
     """Check if session can be deleted or modified"""
     return form.request.has_permission(MANAGE_PLANNING_PERMISSION, context=form.context)
 
 
 class ISessionPropertiesEditFormButtons(IModalEditFormButtons):
     """Session properties edit form buttons"""
 
     bookings = ActionButton(name='bookings',
-                            title=_("Bookings"))
+                            title=_("Bookings"),
+                            condition=can_view_bookings)
 
     delete = SubmitButton(name='delete',
                           title=_("Delete"),
                           condition=can_delete_session)
 
 
 @ajax_form_config(name='properties.html',
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,43 +18,57 @@
 from pyramid.interfaces import IRequest
 from pyramid.security import ALL_PERMISSIONS, Allow
 from zope.container.contained import Contained
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_app_msc.feature.profile.interfaces import IOperatorProfile, IUserProfile, OPERATOR_PROFILE_KEY, \
     USER_PROFILE_KEY
+from pyams_app_msc.reference.structure import IStructureTypeTable
+from pyams_i18n.interfaces import II18n
 from pyams_security.interfaces.base import IPrincipalInfo
 from pyams_security.interfaces.names import ADMIN_USER_ID
 from pyams_utils.adapter import adapter_config, get_annotation_adapter
 from pyams_utils.factory import factory_config
 
 __docformat__ = 'restructuredtext'
 
+from pyams_utils.interfaces import MISSING_INFO
+
+from pyams_utils.registry import get_utility
+
 
 @factory_config(IUserProfile)
 class UserProfile(Persistent, Contained):
     """User profile persistent class"""
 
     principal_id = None
 
     active = FieldProperty(IUserProfile['active'])
     firstname = FieldProperty(IUserProfile['firstname'])
     lastname = FieldProperty(IUserProfile['lastname'])
     email = FieldProperty(IUserProfile['email'])
     phone_number = FieldProperty(IUserProfile['phone_number'])
     establishment = FieldProperty(IUserProfile['establishment'])
+    structure_type = FieldProperty(IUserProfile['structure_type'])
     establishment_address = FieldProperty(IUserProfile['establishment_address'])
     local_theaters = FieldProperty(IUserProfile['local_theaters'])
 
     def __acl__(self):
         return [
             (Allow, ADMIN_USER_ID, ALL_PERMISSIONS),
             (Allow, self.principal_id, ALL_PERMISSIONS)
         ]
 
+    def get_structure_type(self):
+        structures = get_utility(IStructureTypeTable)
+        structure_type = structures.get(self.structure_type)
+        if structure_type is None:
+            return MISSING_INFO
+        return II18n(structure_type).query_attribute('title')
+
 
 @adapter_config(required=IPrincipalInfo,
                 provides=IUserProfile)
 def principal_user_profile(principal):
     """Principal user profile factory"""
 
     def user_profile_callback(profile):
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/interfaces.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from zope.interface import Attribute, Interface, implementer
 from zope.interface.interfaces import IObjectEvent, ObjectEvent
 from zope.schema import Bool, Choice, List, Object, TextLine
 from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
 from pyams_app_msc.component.address.interfaces import IAddress
+from pyams_app_msc.reference.structure import STRUCTURE_TYPES_VOCABULARY
 from pyams_app_msc.shared.theater.interfaces import MSC_THEATERS_VOCABULARY
 from pyams_scheduler.interfaces import ITask
 from pyams_utils.schema import MailAddressField
 
 __docformat__ = 'restructuredtext'
 
 from pyams_app_msc import _
@@ -34,14 +35,18 @@
 
 USER_PROFILE_KEY = 'msc.profile'
 
 
 class IUserProfile(Interface):
     """User profile interface"""
 
+    principal_id = TextLine(title="Principal ID",
+                            description=_("Principal ID"),
+                            required=True)
+
     active = Bool(title=_("Active user?"),
                   description=_("Inactive users can't login anymore to website"),
                   required=True,
                   default=True)
 
     firstname = TextLine(title=_("First name"),
                          required=True)
@@ -54,22 +59,30 @@
 
     phone_number = TextLine(title=_("Phone number"),
                             required=True)
 
     establishment = TextLine(title=_("Establishment of affiliation"),
                              required=True)
 
+    structure_type = Choice(title=_("Structure type"),
+                            description=_("Select structure type matching this establishment"),
+                            vocabulary=STRUCTURE_TYPES_VOCABULARY,
+                            required=True)
+
     establishment_address = Object(title=_("Establishment address"),
                                    schema=IAddress,
                                    required=False)
 
     local_theaters = List(title=_("Preferred local theaters"),
                           value_type=Choice(vocabulary=MSC_THEATERS_VOCABULARY),
                           required=True)
 
+    def get_structure_type(self):
+        """Structure type label getter"""
+
 
 class SEATS_DISPLAY_MODE(Enum):
     """Session seats display mode"""
     NONE = 'none'
     TOTAL = 'total'
     WAITING = 'waiting'
     CONFIRMED = 'confirmed'
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/password.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/password.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/register.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/register.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/task.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from pyams_app_msc.feature.profile import IOperatorProfile, IUserProfile, USER_PROFILE_KEY
 from pyams_app_msc.interfaces import MANAGE_BOOKING_PERMISSION
 from pyams_form.ajax import ajax_form_config
 from pyams_form.button import Buttons, handler
 from pyams_form.field import Fields
 from pyams_form.group import Group
-from pyams_form.interfaces import DISPLAY_MODE
+from pyams_form.interfaces import DISPLAY_MODE, HIDDEN_MODE
 from pyams_form.interfaces.form import IDataExtractedEvent, IFormContent, IGroup
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_mail.interfaces import IPrincipalMailInfo
 from pyams_security.interfaces import ISecurityManager
 from pyams_security.interfaces.base import IPrincipalInfo
 from pyams_security.interfaces.plugin import ILocalUser, LOCKED_ACCOUNT_PASSWORD
 from pyams_security.utility import get_principal
@@ -57,16 +57,17 @@
                   layer=IPyAMSLayer,
                   permission=MANAGE_BOOKING_PERMISSION)
 class UserProfileAddForm(AdminModalAddForm):
     """User profile add form"""
 
     title = _("User add form")
     legend = _("User account settings")
+    autocomplete = 'off'
 
-    fields = Fields(IUserProfile).omit('active')
+    fields = Fields(IUserProfile).omit('active', 'principal_id')
     content_factory = IUserProfile
 
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         email = self.widgets.get('email')
         if email is not None:
             email.object_data = {
@@ -78,14 +79,18 @@
             alsoProvides(email, IObjectData)
         phone_number = self.widgets.get('phone_number')
         if phone_number is not None:
             phone_number.object_data = {
                 'input-mask': '[+9{3}] [9]9 99 99 99 99'
             }
             alsoProvides(phone_number, IObjectData)
+        structure_type = self.widgets.get('structure_type')
+        if structure_type is not None:
+            structure_type.prompt = True
+            structure_type.prompt_message = _("Select structure type...")
 
     def add(self, obj):
         login_config = ILoginConfiguration(self.request.root)
         sm = get_utility(ISecurityManager)
         users_folder = sm.get(login_config.users_folder)
         if users_folder is not None:
             local_user = create_object(ILocalUser)
@@ -164,14 +169,17 @@
     def buttons(self):
         if self.mode == DISPLAY_MODE:
             return Buttons(IModalDisplayFormButtons)
         return Buttons(IUserProfileEditFormButtons).select('disable', 'enable', 'apply', 'close')
 
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
+        principal_id = self.widgets.get('principal_id')
+        if principal_id is not None:
+            principal_id.mode = HIDDEN_MODE
         phone_number = self.widgets.get('phone_number')
         if phone_number is not None:
             phone_number.object_data = {
                 'input-mask': '[+9{3}] [9]9 99 99 99 99'
             }
             alsoProvides(phone_number, IObjectData)
         email = self.widgets.get('email')
@@ -193,15 +201,15 @@
         disable = self.actions.get('disable')
         if disable is not None:
             disable.add_class('btn-danger mr-auto')
             disable.hint = translate(_("Disabled profiles can't be used for website login anymore but can "
                                        "still be assigned new bookings"))
         enable = self.actions.get('enable')
         if enable is not None:
-            enable.add_class('btn-info mr-auto')
+            enable.add_class('btn-danger mr-auto')
 
     @handler(IUserProfileEditFormButtons['disable'])
     def handle_disable(self, action):
         """Handle disable button"""
         principal_info = self.form_content
         IUserProfile(principal_info).active = False
         sm = get_utility(ISecurityManager)
@@ -248,15 +256,15 @@
 
 
 @adapter_config(required=(Interface, IAdminLayer, UserProfileEditForm),
                 provides=IFormContent)
 def user_profile_edit_form_content(context, request, view):
     """User profile edit form content getter"""
     principal = None
-    principal_id = request.params.get('principal_id')
+    principal_id = request.params.get('principal_id') or request.params.get(f'{view.prefix}widgets.principal_id')
     if principal_id:
         principal = get_principal(request, principal_id)
     else:
         email = request.params.get(f'{view.prefix}widgets.email')
         if email:
             login_config = ILoginConfiguration(request.root)
             sm = get_utility(ISecurityManager)
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/profile/zmi/widget.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from pyramid.httpexceptions import HTTPOk
 from zope.container.contained import Contained
 from zope.lifecycleevent.interfaces import IObjectAddedEvent
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_app_msc.feature.tmdb.interfaces import ITMDBConfiguration, ITMDBService, ITMDBServiceClientTarget, \
     TMDB_CONFIGURATION_KEY
-from pyams_content.component.gallery.interfaces import IGallery, IGalleryFile
+from pyams_content.component.gallery.interfaces import GALLERY_PARAGRAPH_TYPE, IGalleryFile, IGalleryParagraph
 from pyams_content.component.illustration.interfaces import IIllustration
 from pyams_content.component.paragraph.interfaces import IParagraphContainer
 from pyams_content.component.video import external_video_settings
 from pyams_content.component.video.interfaces import IExternalVideoParagraph
 from pyams_i18n.interfaces import II18n, INegotiator
 from pyams_site.interfaces import ISiteRoot
 from pyams_utils.adapter import adapter_config, get_annotation_adapter
@@ -317,42 +317,49 @@
                 catalog_info.director = info.get('directors')
                 catalog_info.composer = info.get('composers')
                 catalog_info.actors = info.get('actors')
                 catalog_info.duration = info.get('duration')
                 catalog_info.synopsis = info.get('overview')
             # set gallery images
             if configuration.download_pictures or configuration.download_posters:
-                gallery_file_factory = get_object_factory(IGalleryFile)
-                if gallery_file_factory is not None:
-                    gallery = IGallery(activity, None)
-                    for picture in self.get_movie_pictures(movie_id, negotiator.server_language):
-                        image_type = picture.get('image_type')
-                        if (image_type == 'backdrop') and not configuration.download_pictures:
-                            continue
-                        if (image_type == 'poster') and not configuration.download_posters:
-                            continue
-                        gallery_file = gallery_file_factory()
-                        gallery.append(gallery_file)
-                        gallery_file.visible = False
-                        if image_type == 'poster':
-                            gallery_file.data = self.get_image(configuration,
-                                                               image_id=picture.get('image_id'),
-                                                               size=configuration.posters_size)
+                paragraphs = IParagraphContainer(activity, None)
+                if paragraphs is not None:
+                    gallery_file_factory = get_object_factory(IGalleryFile)
+                    if gallery_file_factory is not None:
+                        galleries = list(paragraphs.get_paragraphs(GALLERY_PARAGRAPH_TYPE))
+                        if galleries:
+                            gallery = galleries[0]
                         else:
-                            gallery_file.data = self.get_image(configuration,
-                                                               image_id=picture.get('image_id'),
-                                                               size=configuration.pictures_size)
+                            gallery = create_object(IGalleryParagraph)
+                            paragraphs.append(gallery)
+                        for picture in self.get_movie_pictures(movie_id, negotiator.server_language):
+                            image_type = picture.get('image_type')
+                            if (image_type == 'backdrop') and not configuration.download_pictures:
+                                continue
+                            if (image_type == 'poster') and not configuration.download_posters:
+                                continue
+                            gallery_file = gallery_file_factory()
+                            gallery.append(gallery_file)
+                            gallery_file.visible = False
+                            if image_type == 'poster':
+                                gallery_file.data = self.get_image(configuration,
+                                                                   image_id=picture.get('image_id'),
+                                                                   size=configuration.posters_size)
+                            else:
+                                gallery_file.data = self.get_image(configuration,
+                                                                   image_id=picture.get('image_id'),
+                                                                   size=configuration.pictures_size)
             # set videos
             if configuration.download_videos:
                 paragraphs = IParagraphContainer(activity, None)
                 if paragraphs is not None:
-                    factory = get_object_factory(IExternalVideoParagraph)
-                    if factory is not None:
+                    video_factory = get_object_factory(IExternalVideoParagraph)
+                    if video_factory is not None:
                         for video in self.get_movie_videos(movie_id, configuration.language):
-                            paragraph = factory()
+                            paragraph = video_factory()
                             paragraph.visible = False
                             paragraph.title = {
                                 negotiator.server_language: video.get('title')
                             }
                             paragraph.description = {
                                 negotiator.server_language: video.get('type')
                             }
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/api/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/api/schema.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/api/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/feature/tmdb/zmi/lookup.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/zmi/lookup.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/generations/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/generations/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,28 +17,31 @@
 __docformat__ = 'restructuredtext'
 
 from importlib import import_module
 
 from pyams_app_msc.feature.booking.interfaces import IBookingInfo
 from pyams_app_msc.feature.planning.interfaces import ISession
 from pyams_app_msc.interfaces import MSC_CONTRIBUTOR_ROLE, MSC_MANAGER_ROLE, MSC_OPERATOR_ROLE, MSC_READER_ROLE
+from pyams_app_msc.reference.structure import IStructureTypeTable
 from pyams_app_msc.shared.catalog.interfaces import ICatalogEntryInfo
 from pyams_catalog.generations import check_required_indexes
 from pyams_catalog.index import DatetimeIndexWithInterface, FieldIndexWithInterface, KeywordIndexWithInterface
 from pyams_catalog.interfaces import MINUTE_RESOLUTION
 from pyams_content.generations import check_required_tables, check_required_tools
 from pyams_security.index import PrincipalsRoleIndex
 from pyams_site.generations import check_required_utilities
 from pyams_site.interfaces import ISiteGenerations
 from pyams_utils.registry import utility_config
 
 
 REQUIRED_UTILITIES = ()
 
-REQUIRED_TABLES = ()
+REQUIRED_TABLES = (
+    (IStructureTypeTable, 'structures-types'),
+)
 
 REQUIRED_TOOLS = (
 )
 
 REQUIRED_INDEXES = (
     ('role:msc:manager', PrincipalsRoleIndex, {
         'role_id': MSC_MANAGER_ROLE
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/include.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/include.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,16 @@
             VIEW_PLANNING_PERMISSION, VIEW_BOOKING_PERMISSION,
             MANAGE_BOOKING_PERMISSION, VIEW_SYSTEM_PERMISSION,
             MANAGE_ROLES_PERMISSION
         },
         'managers': {
             ADMIN_USER_ID,
             ROLE_ID.format(SYSTEM_ADMIN_ROLE),
-            ROLE_ID.format(MSC_SITES_MANAGER_ROLE)
+            ROLE_ID.format(MSC_SITES_MANAGER_ROLE),
+            ROLE_ID.format(MSC_MANAGER_ROLE)
         },
         'set_as_operator': False
     })
     config.register_role({
         'id': MSC_OPERATOR_ROLE,
         'title': _("MSC: Theater operator"),
         'permissions': {
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo` & `pyams_app_msc-1.99.2/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -14,14 +14,17 @@
 
 msgid "   - Free accompanists"
 msgstr "   - Accompagnateurs non payants"
 
 msgid "   - Paying accompanists"
 msgstr "   - Accompagnateurs payants"
 
+msgid " (Seats: {})"
+msgstr " (places : {})"
+
 msgid " {date} from {start_time} to {end_time}"
 msgstr "{date}, de {start_time} à {end_time}"
 
 msgid "#Quotation:"
 msgstr "N° de devis :"
 
 msgid "${groups}: ${participants} participants, ${accompanists} accompanists"
@@ -127,50 +130,59 @@
 
 msgid "Activity information"
 msgstr "Détails spécifiques de l'activité"
 
 msgid "Activity type"
 msgstr "Type d'activité"
 
+msgid "Activity type properties"
+msgstr "Propriétés du type d'activités"
+
 msgid "Activity types"
 msgstr "Types d'activités"
 
 msgid "Actors count"
 msgstr "Nombre d'acteurs"
 
 msgid "Actors:"
 msgstr "Acteurs :"
 
 msgid "Add activity type"
 msgstr "Ajouter un type d'activité"
 
+msgid "Add and accept"
+msgstr "Ajouter et accepter"
+
 msgid "Add audience"
 msgstr "Ajouter un public"
 
 msgid "Add booking"
 msgstr "Ajouter une réservation"
 
 msgid "Add booking archiver task..."
 msgstr "Archivage des réservations"
 
 msgid "Add booking for this session"
 msgstr "Confirmer la demande de réservation"
 
 msgid "Add catalog entry"
-msgstr "Ajouter une entrée au catalogue"
+msgstr "Ajouter une activité au catalogue"
 
 msgid "Add movie theater"
 msgstr "Ajouter un cinéma"
 
 msgid "Add price"
 msgstr "Ajouter un tarif"
 
 msgid "Add room"
 msgstr "Ajouter une salle"
 
+msgid "Add structure type"
+msgstr "Ajouter un type de structure"
+
 msgid "Add theater"
 msgstr "Ajouter un cinéma"
 
 msgid "Additional comments"
 msgstr "Commentaires complémentaires"
 
 msgid "Address"
@@ -192,17 +204,14 @@
 msgstr "Un tarif inactif ne peut pas être affecté à de nouvelles réservations"
 
 msgid "An inactive room can't be selected to assign new activities"
 msgstr ""
 "Une salle active ne peut pas être sélectionnée pour lui affecter de "
 "nouvelles activités"
 
-msgid "Apartment"
-msgstr "Appartement"
-
 msgid "Apply"
 msgstr "Enregistrer"
 
 msgid "Archived"
 msgstr "Archivée"
 
 msgid "Archived booking"
@@ -373,30 +382,30 @@
 msgid "Cancelled booking"
 msgstr "Réservation annulée"
 
 msgid "Capacity"
 msgstr "Capacité"
 
 msgid "Catalog entries with next planned sessions"
-msgstr "Entrées du catalogue avec les prochaines séances"
+msgstr "Activités au catalogue avec les prochaines séances"
 
 msgid "Catalog entry"
-msgstr "Entrée du catalogue"
+msgstr "Activité au catalogue"
 
 msgid "Catalog layout"
 msgstr "Mise en page"
 
 msgid "Catalog management"
 msgstr "Gérer le catalogue"
 
 msgid "Catalog presentation"
-msgstr "Entrées du catalogue"
+msgstr "Activités au catalogue"
 
 msgid "Catalog template configuration"
-msgstr "Modèle de présentation des entrées du catalogue"
+msgstr "Modèle de présentation des activités inscrites au catalogue"
 
 msgid "Change booking session"
 msgstr "Changement d'événement"
 
 msgid "Change password"
 msgstr "Changer de mot de passe"
 
@@ -684,23 +693,17 @@
 
 msgid "Enter login or email address"
 msgstr "Votre code utilisateur est votre adresse de messagerie"
 
 msgid "Enter text for TMDB movie search"
 msgstr "Indiquez un titre pour rechercher dans TMDB..."
 
-msgid "Entry"
-msgstr "Entrée"
-
 msgid "Entry number and street name"
 msgstr "Numéro de l'adresse et nom de la rue"
 
-msgid "Entry, building, residence..."
-msgstr "Entrée, bâtiment, résidence..."
-
 msgid "Establishment"
 msgstr "Établissement"
 
 msgid "Establishment address"
 msgstr "Adresse de l'établissement ou de la structure"
 
 msgid "Establishment of affiliation"
@@ -708,17 +711,14 @@
 
 msgid "First name"
 msgstr "Prénom"
 
 msgid "First time available for sessions planning"
 msgstr "Heure à partir de laquelle des événements peuvent être programmés"
 
-msgid "Floor, corridor..."
-msgstr "Niveau, couloir..."
-
 msgid "Forbidden cancellation"
 msgstr "Annulation impossible"
 
 msgid "Free seats"
 msgstr "Places disponibles"
 
 msgid "Full name"
@@ -824,16 +824,16 @@
 
 msgid "If 'yes', this session is 'temporary' and not confirmed yet!"
 msgstr ""
 "Si 'oui', cet événement est encore temporaire, en attente de confirmation..."
 
 msgid "If no label is set, activity label will be used"
 msgstr ""
-"Ce libellé sera affiché en lieu et place du titre de l'activité, s'il y en a "
-"une"
+"Ce libellé sera affiché s'il n'y a pas d'activité associée à cet événement, "
+"ou à la place du libellé de l'activité si vous en avez sélectionné une"
 
 msgid "Images URL"
 msgstr "URL des images"
 
 msgid "Inactive users can't login anymore to website"
 msgstr ""
 "Un profil désactivé ne peut plus être utilisé pour se connecter au site"
@@ -1109,14 +1109,17 @@
 
 msgid "Name of workflow utility used to manage tool contents"
 msgstr "Type de workflow appliqué à la gestion du catalogue des activités"
 
 msgid "Name used as messages sender name"
 msgstr "Nom utilisé comme expéditeur des messages"
 
+msgid "New activity type"
+msgstr "Nouveau type d'activité"
+
 msgid "New booking"
 msgstr "Nouvelle réservation"
 
 msgid "New booking properties"
 msgstr "Propriétés de la nouvelle réservation"
 
 msgid "New catalog entry properties"
@@ -1142,14 +1145,20 @@
 
 msgid "New session"
 msgstr "Nouvel événement"
 
 msgid "New session properties"
 msgstr "Propriétés de l'événement"
 
+msgid "New structure type"
+msgstr "Nouveau type de structure"
+
+msgid "New structure type properties"
+msgstr "Propriétés du nouveau type de structure"
+
 msgid "New theater properties"
 msgstr "Propriétés du nouveau cinéma"
 
 msgid "Next page"
 msgstr "Page suivante"
 
 msgid "No session selected, booking was not changed."
@@ -1210,15 +1219,15 @@
 
 msgid "Object:"
 msgstr "Objet :"
 
 msgid "Only external bookable sessions are visible to public for booking"
 msgstr ""
 "Seuls les événements ouverts aux réservations externes peuvent faire l'objet "
-"de demandes de réservations par les clients du site"
+"de demandes de réservations par les partenaires du cinéma"
 
 msgid "Only internal bookable sessions are visible to operators for booking"
 msgstr ""
 "Seuls les événements ouverts aux réservations internes peuvent être réservés "
 "par les opérateurs du cinéma"
 
 msgid "Open for external booking"
@@ -1371,15 +1380,15 @@
 msgid "Proposed version: ${version}"
 msgstr "Version proposée : ${version}"
 
 msgid "Proxy information"
 msgstr "Serveur proxy"
 
 msgid "PyAMS MSC skin"
-msgstr "Thème commun \"Ma sortie cinéma\""
+msgstr "Thème commun \"Ma Séance Ciné\""
 
 msgid "QUOTATION"
 msgstr "DEVIS"
 
 msgid "Quotation"
 msgstr "Devis"
 
@@ -1506,14 +1515,20 @@
 
 msgid "Search results"
 msgstr "Résultats de la recherche"
 
 msgid "Seats"
 msgstr "Places"
 
+msgid "Select structure type matching this establishment"
+msgstr "Sélectionner le type de structure correspondant à cet établissement"
+
+msgid "Select structure type..."
+msgstr "Sélectionner un type de structure..."
+
 msgid "Select the session for which this booking is applied"
 msgstr "Nouvel événement auquel doit s'appliquer la réservation"
 
 msgid "Selected audiences"
 msgstr "Publics concernés"
 
 msgid "Selected mailer"
@@ -1607,14 +1622,32 @@
 
 msgid "Start date and time of the session"
 msgstr "Date et heure de début de la séance"
 
 msgid "Status"
 msgstr "Statut"
 
+msgid "Structure type"
+msgstr "Type de structure"
+
+msgid "Structure type properties"
+msgstr "Propriétés du type de structure"
+
+msgid "Structure type: {}"
+msgstr "Type de structure : {}"
+
+msgid "Structures types"
+msgstr "Types de structures"
+
+msgid "Structures types list"
+msgstr "Liste des types de structures"
+
+msgid "Structures types table"
+msgstr "Table des types de structures"
+
 msgid "Subject of notification message sent to the recipient"
 msgstr "Sujet du message adressé au bénéficiaire"
 
 msgid "Subject of reminder message sent to the recipient"
 msgstr "Sujet du message de rappel adressé au bénéficiaire"
 
 msgid "Subject of update message sent to the recipient"
@@ -1650,14 +1683,17 @@
 
 msgid "TMDB service properties"
 msgstr "Propriétés du service"
 
 msgid "TV"
 msgstr "VF"
 
+msgid "Table contents"
+msgstr "Contenu"
+
 msgid ""
 "Target room doesn't have enough capacity for confirmed seats of this session!"
 msgstr ""
 "La salle sélectionnée ne dispose pas d'une capacité suffisante pour "
 "accueillir les réservations confirmées à cet événement !"
 
 msgid "Temporary session"
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po` & `pyams_app_msc-1.99.2/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # PyAMS application for cinema reservation management
 #
 # This file is distributed under the same license as the PACKAGE package.
 # Thierry Florac <tflorac@ulthar.net>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: PyAMS MSC application 1.0.0\n"
-"POT-Creation-Date: 2024-03-24 03:43+0100\n"
+"POT-Creation-Date: 2024-04-27 14:19+0200\n"
 "Last-Translator: Thierry Florac <tflorac@ulthar.net>\n"
 "Language-Team: FRENCH <FR@li.org>\n"
 "Language: French\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 3.10.dev0\n"
@@ -56,34 +56,72 @@
 msgid "MSC: Sites manager"
 msgstr "MSC : Administrateur délégué"
 
 #: src/pyams_app_msc/include.py:120
 msgid "MSC: Theater manager"
 msgstr "MSC : Administrateur d'un cinéma"
 
-#: src/pyams_app_msc/include.py:139
+#: src/pyams_app_msc/include.py:140
 msgid "MSC: Theater operator"
 msgstr "MSC : Opérateur d'un cinéma"
 
-#: src/pyams_app_msc/include.py:157
+#: src/pyams_app_msc/include.py:158
 msgid "MSC: Contributor"
 msgstr "MSC : Contributeur d'un cinéma"
 
-#: src/pyams_app_msc/include.py:174
+#: src/pyams_app_msc/include.py:175
 msgid "MSC: Theater consultant"
 msgstr "MSC : Invité d'un cinéma"
 
-#: src/pyams_app_msc/include.py:189
+#: src/pyams_app_msc/include.py:190
 msgid "MSC: Theater client"
 msgstr "MSC : Client d'un cinéma"
 
-#: src/pyams_app_msc/include.py:201
+#: src/pyams_app_msc/include.py:202
 msgid "MSC: Reservation owner"
 msgstr "MSC : Propriétaire d'une réservation"
 
+#: src/pyams_app_msc/reference/structure/zmi/table.py:38
+#: src/pyams_app_msc/reference/structure/zmi/table.py:79
+msgid "Structures types"
+msgstr "Types de structures"
+
+#: src/pyams_app_msc/reference/structure/zmi/table.py:56
+msgid "Table contents"
+msgstr "Contenu"
+
+#: src/pyams_app_msc/reference/structure/zmi/table.py:82
+msgid "Structures types list"
+msgstr "Liste des types de structures"
+
+#: src/pyams_app_msc/reference/structure/zmi/table.py:90
+msgid "Structures types table"
+msgstr "Table des types de structures"
+
+#: src/pyams_app_msc/reference/structure/zmi/__init__.py:56
+msgid "Add structure type"
+msgstr "Ajouter un type de structure"
+
+#: src/pyams_app_msc/reference/structure/zmi/__init__.py:66
+msgid "New structure type"
+msgstr "Nouveau type de structure"
+
+#: src/pyams_app_msc/reference/structure/zmi/__init__.py:67
+msgid "New structure type properties"
+msgstr "Propriétés du nouveau type de structure"
+
+#: src/pyams_app_msc/reference/structure/zmi/__init__.py:118
+#, python-format
+msgid "Structure type: {}"
+msgstr "Type de structure : {}"
+
+#: src/pyams_app_msc/reference/structure/zmi/__init__.py:121
+msgid "Structure type properties"
+msgstr "Propriétés du type de structure"
+
 #: src/pyams_app_msc/feature/tmdb/interfaces.py:41
 msgid "Enable TMDB configuration"
 msgstr "Activer le service TMDB"
 
 #: src/pyams_app_msc/feature/tmdb/interfaces.py:45
 msgid "Service URL"
 msgstr "URL du service"
@@ -298,74 +336,86 @@
 msgid "TMDB service configuration"
 msgstr "Configuration du service TMDB"
 
 #: src/pyams_app_msc/feature/tmdb/zmi/__init__.py:64
 msgid "TMDB service properties"
 msgstr "Propriétés du service"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:41
+#: src/pyams_app_msc/feature/profile/interfaces.py:43
+msgid "Principal ID"
+msgstr ""
+
+#: src/pyams_app_msc/feature/profile/interfaces.py:46
 msgid "Active user?"
 msgstr "Profil actif ?"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:42
+#: src/pyams_app_msc/feature/profile/interfaces.py:47
 msgid "Inactive users can't login anymore to website"
 msgstr ""
 "Un profil désactivé ne peut plus être utilisé pour se connecter au site"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:46
+#: src/pyams_app_msc/feature/profile/interfaces.py:51
 msgid "First name"
 msgstr "Prénom"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:49
+#: src/pyams_app_msc/feature/profile/interfaces.py:54
 msgid "Last name"
 msgstr "Nom"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:52
+#: src/pyams_app_msc/feature/profile/interfaces.py:57
 msgid "Mail address"
 msgstr "Addresse de messagerie"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:55
+#: src/pyams_app_msc/feature/profile/interfaces.py:60
 #: src/pyams_app_msc/component/contact/interfaces.py:38
 #: src/pyams_app_msc/shared/theater/interfaces/__init__.py:92
 msgid "Phone number"
 msgstr "Téléphone"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:58
+#: src/pyams_app_msc/feature/profile/interfaces.py:63
 msgid "Establishment of affiliation"
 msgstr "Établissement ou structure"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:61
+#: src/pyams_app_msc/feature/profile/interfaces.py:66
+msgid "Structure type"
+msgstr "Type de structure"
+
+#: src/pyams_app_msc/feature/profile/interfaces.py:67
+msgid "Select structure type matching this establishment"
+msgstr "Sélectionner le type de structure correspondant à cet établissement"
+
+#: src/pyams_app_msc/feature/profile/interfaces.py:71
 msgid "Establishment address"
 msgstr "Adresse de l'établissement ou de la structure"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:65
+#: src/pyams_app_msc/feature/profile/interfaces.py:75
 msgid "Preferred local theaters"
 msgstr "Cinémas de rattachement"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:79
+#: src/pyams_app_msc/feature/profile/interfaces.py:89
 msgid "Not displayed"
 msgstr "Non affichées"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:80
+#: src/pyams_app_msc/feature/profile/interfaces.py:90
 msgid "Display confirmed/requested/capacity seats"
 msgstr "Afficher les places acceptées / demandées / en jauge"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:81
+#: src/pyams_app_msc/feature/profile/interfaces.py:91
 msgid "Display confirmed/waiting/capacity seats"
 msgstr "Afficher les places acceptées / en attente / en jauge"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:82
+#: src/pyams_app_msc/feature/profile/interfaces.py:92
 msgid "Display confirmed/capacity seats"
 msgstr "Afficher les places acceptées / en jauge"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:98
+#: src/pyams_app_msc/feature/profile/interfaces.py:108
 msgid "Session seats display mode"
 msgstr "Affichage des places dans l'agenda"
 
-#: src/pyams_app_msc/feature/profile/interfaces.py:99
+#: src/pyams_app_msc/feature/profile/interfaces.py:109
 msgid ""
 "You can choose how session seats are displayed in movie theater planning view"
 msgstr ""
 "Vous pouvez choisir la façon dont les places sont affichées dans le planning "
 "des activités"
 
 #: src/pyams_app_msc/feature/profile/task.py:56
@@ -373,57 +423,61 @@
 msgstr "Suppression de profil utilisateur"
 
 #: src/pyams_app_msc/feature/profile/zmi/__init__.py:62
 msgid "User add form"
 msgstr "Création d'un compte utilisateur"
 
 #: src/pyams_app_msc/feature/profile/zmi/__init__.py:63
-#: src/pyams_app_msc/feature/profile/zmi/__init__.py:159
+#: src/pyams_app_msc/feature/profile/zmi/__init__.py:164
 msgid "User account settings"
 msgstr "Propriétés du profil utilisateur"
 
-#: src/pyams_app_msc/feature/profile/zmi/__init__.py:119
+#: src/pyams_app_msc/feature/profile/zmi/__init__.py:89
+msgid "Select structure type..."
+msgstr "Sélectionner un type de structure..."
+
+#: src/pyams_app_msc/feature/profile/zmi/__init__.py:124
 #: src/pyams_app_msc/feature/profile/skin/register.py:175
 msgid "This email address is already registered!"
 msgstr "Cette adresse de messagerie est déjà enregistrée !"
 
-#: src/pyams_app_msc/feature/profile/zmi/__init__.py:131
+#: src/pyams_app_msc/feature/profile/zmi/__init__.py:136
 msgid ""
 "This form allows you to register a new user account.\n"
 "If this user want to login, he will have to use the \"Forgotten password\" "
 "feature to get a new activation link to set his password."
 msgstr ""
 "Ce formulaire vous permet de renseigner les paramètres d'inscription d'un "
 "utilisateur.\n"
 "À l'issue de cette inscription, si cet utilisateur souhaite se connecter, il "
 "devra utiliser la fonction \"Mot de passe oublié\" accessible depuis l'écran "
 "de connexion pour obtenir sur son adresse de messagerie un lien d'activation "
 "lui permettant de définir son mot de passe."
 
-#: src/pyams_app_msc/feature/profile/zmi/__init__.py:144
+#: src/pyams_app_msc/feature/profile/zmi/__init__.py:149
 msgid "Disable profile"
 msgstr "Désactiver le profil"
 
-#: src/pyams_app_msc/feature/profile/zmi/__init__.py:148
+#: src/pyams_app_msc/feature/profile/zmi/__init__.py:153
 msgid "Enable profile"
 msgstr "Activer le profil"
 
-#: src/pyams_app_msc/feature/profile/zmi/__init__.py:158
+#: src/pyams_app_msc/feature/profile/zmi/__init__.py:163
 msgid "User edit form"
 msgstr "Modification d'un compte utilisateur"
 
-#: src/pyams_app_msc/feature/profile/zmi/__init__.py:196
+#: src/pyams_app_msc/feature/profile/zmi/__init__.py:204
 msgid ""
 "Disabled profiles can't be used for website login anymore but can still be "
 "assigned new bookings"
 msgstr ""
 "Un profil utilisateur désactivé ne peut plus être utilisé pour se connecter "
 "sur le site, mais peut toujours être bénéficiaire de nouvelles réservations"
 
-#: src/pyams_app_msc/feature/profile/zmi/__init__.py:284
+#: src/pyams_app_msc/feature/profile/zmi/__init__.py:292
 msgid "Operator profile"
 msgstr "Mon profil opérateur"
 
 #: src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt:53
 msgid "Edit user profile"
 msgstr "Modifier le profil utilisateur"
 
@@ -659,21 +713,26 @@
 msgid "Messaging service settings"
 msgstr "Paramètres de la messagerie"
 
 #: src/pyams_app_msc/feature/messaging/zmi/__init__.py:54
 msgid "Messaging properties"
 msgstr "Propriétés de la messagerie"
 
-#: src/pyams_app_msc/feature/planning/session.py:156
+#: src/pyams_app_msc/feature/planning/session.py:155
+#: src/pyams_app_msc/feature/planning/zmi/session.py:236
+msgid "Out of catalog activity"
+msgstr "(activité hors-catalogue)"
+
+#: src/pyams_app_msc/feature/planning/session.py:160
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:180
 #, python-format
 msgid "{room} - {date} from {start_time} to {end_time}"
 msgstr "{room} - {date}, de {start_time} à {end_time}"
 
-#: src/pyams_app_msc/feature/planning/session.py:184
+#: src/pyams_app_msc/feature/planning/session.py:188
 #, python-format
 msgid " {date} from {start_time} to {end_time}"
 msgstr "{date}, de {start_time} à {end_time}"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:44
 msgid "Original version"
 msgstr "Version originale"
@@ -701,16 +760,16 @@
 #: src/pyams_app_msc/feature/planning/interfaces.py:68
 msgid "Label"
 msgstr "Libellé"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:69
 msgid "If no label is set, activity label will be used"
 msgstr ""
-"Ce libellé sera affiché en lieu et place du titre de l'activité, s'il y en a "
-"une"
+"Ce libellé sera affiché s'il n'y a pas d'activité associée à cet événement, "
+"ou à la place du libellé de l'activité si vous en avez sélectionné une"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:75
 msgid "Session start date"
 msgstr "Début de la séance"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:76
 msgid "Start date and time of the session"
@@ -796,15 +855,15 @@
 msgid "Open for external booking"
 msgstr "Ouverte aux réservations externes"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:124
 msgid "Only external bookable sessions are visible to public for booking"
 msgstr ""
 "Seuls les événements ouverts aux réservations externes peuvent faire l'objet "
-"de demandes de réservations par les clients du site"
+"de demandes de réservations par les partenaires du cinéma"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:128
 msgid "Movie theater comments"
 msgstr "Commentaires du cinéma"
 
 #: src/pyams_app_msc/feature/planning/interfaces.py:129
 msgid "These comments will be displayed to the users on booking form"
@@ -844,67 +903,63 @@
 msgid "New session"
 msgstr "Nouvel événement"
 
 #: src/pyams_app_msc/feature/planning/zmi/session.py:62
 msgid "New session properties"
 msgstr "Propriétés de l'événement"
 
-#: src/pyams_app_msc/feature/planning/zmi/session.py:169
+#: src/pyams_app_msc/feature/planning/zmi/session.py:174
 msgid "Bookings"
 msgstr "Réservations"
 
-#: src/pyams_app_msc/feature/planning/zmi/session.py:172
+#: src/pyams_app_msc/feature/planning/zmi/session.py:178
 msgid "Delete"
 msgstr "Supprimer l'événement"
 
-#: src/pyams_app_msc/feature/planning/zmi/session.py:182
+#: src/pyams_app_msc/feature/planning/zmi/session.py:188
 msgid "Session planning"
 msgstr "Programmation d'un événement"
 
-#: src/pyams_app_msc/feature/planning/zmi/session.py:183
+#: src/pyams_app_msc/feature/planning/zmi/session.py:189
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:468
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:665
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:715
 msgid "Session properties"
 msgstr "Propriétés de l'événement"
 
-#: src/pyams_app_msc/feature/planning/zmi/session.py:230
-msgid "Out of catalog activity"
-msgstr "(activité hors-catalogue)"
-
-#: src/pyams_app_msc/feature/planning/zmi/session.py:252
+#: src/pyams_app_msc/feature/planning/zmi/session.py:258
 msgid "You can't define a session gauge higher than the room's capacity!"
 msgstr ""
 "Vous ne pouvez pas définir une jauge supérieure à la capacité de la salle !"
 
-#: src/pyams_app_msc/feature/planning/zmi/session.py:257
+#: src/pyams_app_msc/feature/planning/zmi/session.py:263
 msgid "The number of validated seats is already higher than this gauge!"
 msgstr ""
 "Vous ne pouvez pas abaisser la jauge à un nombre de places inférieur au "
 "nombre de places déjà validées !"
 
-#: src/pyams_app_msc/feature/planning/zmi/session.py:344
+#: src/pyams_app_msc/feature/planning/zmi/session.py:350
 msgid "Unknown room!"
 msgstr "La salle indiquée est inconnue !"
 
-#: src/pyams_app_msc/feature/planning/zmi/session.py:351
+#: src/pyams_app_msc/feature/planning/zmi/session.py:357
 msgid ""
 "Target room doesn't have enough capacity for confirmed seats of this session!"
 msgstr ""
 "La salle sélectionnée ne dispose pas d'une capacité suffisante pour "
 "accueillir les réservations confirmées à cet événement !"
 
-#: src/pyams_app_msc/feature/planning/zmi/session.py:379
+#: src/pyams_app_msc/feature/planning/zmi/session.py:385
 msgid "Bad parameters"
 msgstr "Paramètres incorrects."
 
-#: src/pyams_app_msc/feature/planning/zmi/session.py:390
+#: src/pyams_app_msc/feature/planning/zmi/session.py:396
 msgid "Session updated"
 msgstr "Séance modifiée"
 
-#: src/pyams_app_msc/feature/planning/zmi/session.py:391
+#: src/pyams_app_msc/feature/planning/zmi/session.py:397
 msgid "Session capacity has been reduced due to lower room capacity!"
 msgstr ""
 "La jauge de l'événement a été réduite du fait de la capacité insuffisante de "
 "cette salle !"
 
 #: src/pyams_app_msc/feature/planning/zmi/__init__.py:64
 msgid "Planning"
@@ -1078,15 +1133,15 @@
 
 #: src/pyams_app_msc/feature/quotation/__init__.py:443
 #, python-format
 msgid "Quotation: {}"
 msgstr "Devis : {}"
 
 #: src/pyams_app_msc/feature/booking/reminder.py:50
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:769
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:819
 #: src/pyams_app_msc/shared/theater/zmi/mail.py:142
 msgid "Booking reminder"
 msgstr "Rappel de réservation"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:75
 msgid "Waiting"
 msgstr "En attente"
@@ -1105,37 +1160,37 @@
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:79
 msgid "Accepted"
 msgstr "Acceptée"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:109
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:232
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:125
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:126
 msgid "Creator"
 msgstr "Créateur"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:110
 msgid "Name of the principal who created the booking"
 msgstr "Nom du mandataire ayant effectué la demande de réservation"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:113
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:248
 #: src/pyams_app_msc/feature/booking/zmi/search.py:71
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:139
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:140
 msgid "Recipient"
 msgstr "Bénéficiaire"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:114
 msgid "Name of the principal for which the booking is done"
 msgstr "Nom du mandataire bénéficiaire de la réservation"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:120
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:292
 #: src/pyams_app_msc/feature/booking/zmi/search.py:74
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:182
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:183
 msgid "Status"
 msgstr "Statut"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:125
 msgid "Participants"
 msgstr "Participants"
 
@@ -1179,27 +1234,27 @@
 msgstr ""
 "Vous pouvez indiquer ici le nombre de participants par accompagnateur qui "
 "bénéficient d'une entrée non payante, ou 0 pour que tous les accompagnateurs "
 "aient à régler leur entrée"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:156
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:262
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:168
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:169
 #: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:46
 msgid "Cultural pass"
 msgstr "Pass Culture"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:157
 msgid "Check this option if payment is done using cultural pass"
 msgstr ""
 "Sélectionnez cette option lorsque le paiement est fait via un Pass Culture"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:161
 #: src/pyams_app_msc/feature/booking/skin/__init__.py:53
-#: src/pyams_app_msc/component/address/interfaces.py:49
+#: src/pyams_app_msc/component/address/interfaces.py:41
 #: src/pyams_app_msc/shared/theater/interfaces/audience.py:50
 #: src/pyams_app_msc/shared/theater/interfaces/price.py:58
 msgid "Comments"
 msgstr "Commentaire"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:162
 msgid "These comments where added by booking recipient"
@@ -1233,15 +1288,15 @@
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:192
 msgid "This message is added to quotation as an information message"
 msgstr "Ce message d'information est associé au devis envoyé au client"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:195
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:310
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:213
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:214
 msgid "Quotation"
 msgstr "Devis"
 
 #: src/pyams_app_msc/feature/booking/interfaces.py:196
 msgid "This quotation was attached to booking confirmation"
 msgstr "Ceci est le document au format PDF contenant le devis"
 
@@ -1396,21 +1451,21 @@
 msgstr "Nouvel événement auquel doit s'appliquer la réservation"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:217
 msgid "Change session"
 msgstr "Changer d'événement"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:221
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:460
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:510
 msgid "Cancel"
 msgstr "Annuler"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:234
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:367
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:473
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:523
 #, python-format
 msgid "Booking: {}"
 msgstr "Réservation : {}"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:237
 msgid "Change booking session"
 msgstr "Changement d'événement"
@@ -1428,15 +1483,15 @@
 msgid "There are only {} free seats left in this session!"
 msgstr ""
 "<strong>ATTENTION :</strong> il ne reste que {} places libres sur cet "
 "événement !"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:370
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:489
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:477
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:527
 msgid "Booking properties"
 msgstr "Propriétés de la réservation"
 
 #. Default: Cancel booking
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:622
 msgid "cancel-booking-menu"
 msgstr "Annuler"
@@ -1459,15 +1514,15 @@
 msgstr "Refuser la réservation"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:669
 msgid "Booking refused"
 msgstr "Réservation refusée"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:682
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:447
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:497
 msgid "Quotation preview"
 msgstr "Prévisualiser le devis"
 
 #. Default: Optional booking
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:701
 msgid "option-booking-menu"
 msgstr "Accepter (sous réserve)"
@@ -1502,15 +1557,15 @@
 msgstr "Accepter la réservation"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:780
 msgid "Booking accepted"
 msgstr "Réservation acceptée"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:826
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:653
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:703
 msgid "You must set a price to accept a booking!"
 msgstr "Vous devez spécifier un tarif pour pouvoir accepter une réservation !"
 
 #: src/pyams_app_msc/feature/booking/zmi/workflow.py:908
 msgid ""
 "**WARNING**<br />The session capacity is too low to accept this booking!"
 msgstr ""
@@ -1551,15 +1606,15 @@
 msgstr "Salle"
 
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:216
 msgid "Date"
 msgstr "Date"
 
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:276
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:198
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:199
 msgid "Seats"
 msgstr "Places"
 
 #: src/pyams_app_msc/feature/booking/zmi/dashboard.py:331
 msgid "Last update"
 msgstr "Dernière modification"
 
@@ -1619,85 +1674,94 @@
 msgid "Today program"
 msgstr "Programme du jour"
 
 #: src/pyams_app_msc/feature/booking/zmi/home.py:67
 msgid "Sessions planned for today"
 msgstr "Séances programmées aujourd'hui"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:153
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:154
 msgid "Establishment"
 msgstr "Établissement"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:240
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:241
 msgid "Archived booking"
 msgstr "Réservation archivée"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:276
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:277
 msgid "Current session bookings"
 msgstr "Réservations sur l'événement"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:288
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:293
 msgid "Session bookings"
 msgstr "Gestion des réservations"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:302
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:298
+#, python-format
+msgid " (Seats: {})"
+msgstr " (places : {})"
+
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:314
 #, python-format
 msgid "{}: {}"
 msgstr "{}: {}"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:329
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:341
 msgid "Add booking"
 msgstr "Ajouter une réservation"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:348
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:358
+msgid "Add and accept"
+msgstr "Ajouter et accepter"
+
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:368
 msgid "New booking"
 msgstr "Nouvelle réservation"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:349
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:369
 msgid "New booking properties"
 msgstr "Propriétés de la nouvelle réservation"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:450
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:500
 msgid "Reset quotation"
 msgstr "Ré-éditer le devis"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:456
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:506
 msgid "Apply"
 msgstr "Enregistrer"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:624
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:674
 msgid "This booking is archived and can't be modified anymore!"
 msgstr "Cette réservation est archivée et ne peut plus être modifiée !"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:693
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:743
 msgid "Booking quotation"
 msgstr "Devis de la réservation"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:711
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:761
 msgid "Booking update"
 msgstr "Réservation modifiée"
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:746
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:796
 msgid ""
 "Update message can be sent to booking recipient when a booking is modified "
 "after being validated."
 msgstr ""
 "Ce nouveau message sera adressé au bénéficiaire (avec le devis actualisé) "
 "pour indiquer que cette réservation qui a déjà été acceptée a été modifiée."
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:807
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:857
 #, python-format
 msgid ""
 "Reminder message will be sent to booking recipient {} hours before session "
 "begin date..."
 msgstr ""
 "Le message de rappel sera envoyé au bénéficiaire {} heures avant le début de "
 "l'événement."
 
-#: src/pyams_app_msc/feature/booking/zmi/__init__.py:822
+#: src/pyams_app_msc/feature/booking/zmi/__init__.py:872
 msgid "Quotation has been reset!"
 msgstr "Le devis a été re-généré !"
 
 #: src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:52
 msgid "${groups}: ${participants} participants, ${accompanists} accompanists"
 msgstr ""
 "${groups} : ${participants} participants, ${accompanists} accompagnateurs"
@@ -1801,50 +1865,34 @@
 "Banking account information must contain bank code, counter code, account "
 "number and account key"
 msgstr ""
 "Le relevé d'identité bancaire doit contenir le code banque, le code guichet, "
 "le numéro de compte et la clé du RIB"
 
 #: src/pyams_app_msc/component/address/interfaces.py:28
-msgid "Apartment"
-msgstr "Appartement"
-
-#: src/pyams_app_msc/component/address/interfaces.py:29
-msgid "Floor, corridor..."
-msgstr "Niveau, couloir..."
-
-#: src/pyams_app_msc/component/address/interfaces.py:32
-msgid "Entry"
-msgstr "Entrée"
-
-#: src/pyams_app_msc/component/address/interfaces.py:33
-msgid "Entry, building, residence..."
-msgstr "Entrée, bâtiment, résidence..."
-
-#: src/pyams_app_msc/component/address/interfaces.py:36
 msgid "Number and street"
 msgstr "Numéro et rue"
 
-#: src/pyams_app_msc/component/address/interfaces.py:37
+#: src/pyams_app_msc/component/address/interfaces.py:29
 msgid "Entry number and street name"
 msgstr "Numéro de l'adresse et nom de la rue"
 
-#: src/pyams_app_msc/component/address/interfaces.py:40
+#: src/pyams_app_msc/component/address/interfaces.py:32
 msgid "Locality"
 msgstr "Localité"
 
-#: src/pyams_app_msc/component/address/interfaces.py:43
+#: src/pyams_app_msc/component/address/interfaces.py:35
 msgid "Postal code"
 msgstr "Code postal"
 
-#: src/pyams_app_msc/component/address/interfaces.py:46
+#: src/pyams_app_msc/component/address/interfaces.py:38
 msgid "City"
 msgstr "Ville"
 
-#: src/pyams_app_msc/component/address/interfaces.py:50
+#: src/pyams_app_msc/component/address/interfaces.py:42
 msgid "Optional observations which can be added to describe the location"
 msgstr ""
 "Observations complémentaires qui peuvent être ajoutées pour décrire "
 "l'emplacement"
 
 #: src/pyams_app_msc/component/contact/interfaces.py:30
 msgid "Full name"
@@ -1986,40 +2034,48 @@
 #: src/pyams_app_msc/shared/theater/zmi/room.py:249
 #, python-format
 msgid "Cinema room: {}"
 msgstr "Salle : {}"
 
 #: src/pyams_app_msc/shared/theater/zmi/presentation.py:44
 msgid "Catalog presentation"
-msgstr "Entrées du catalogue"
+msgstr "Activités au catalogue"
 
 #: src/pyams_app_msc/shared/theater/zmi/presentation.py:55
 msgid "Catalog template configuration"
-msgstr "Modèle de présentation des entrées du catalogue"
+msgstr "Modèle de présentation des activités inscrites au catalogue"
 
 #: src/pyams_app_msc/shared/theater/zmi/presentation.py:67
 msgid "Catalog layout"
 msgstr "Mise en page"
 
-#: src/pyams_app_msc/shared/theater/zmi/types.py:43
+#: src/pyams_app_msc/shared/theater/zmi/types.py:46
 msgid "Activity types"
 msgstr "Types d'activités"
 
-#: src/pyams_app_msc/shared/theater/zmi/types.py:53
+#: src/pyams_app_msc/shared/theater/zmi/types.py:56
 msgid "Add activity type"
 msgstr "Ajouter un type d'activité"
 
-#: src/pyams_app_msc/shared/theater/zmi/types.py:73
+#: src/pyams_app_msc/shared/theater/zmi/types.py:65
+msgid "New activity type"
+msgstr "Nouveau type d'activité"
+
+#: src/pyams_app_msc/shared/theater/zmi/types.py:79
 msgid "Activities types"
 msgstr "Types d'activités"
 
-#: src/pyams_app_msc/shared/theater/zmi/types.py:74
+#: src/pyams_app_msc/shared/theater/zmi/types.py:80
 msgid "Movie theater activities types list"
 msgstr "Liste des types d'activités"
 
+#: src/pyams_app_msc/shared/theater/zmi/types.py:93
+msgid "Activity type properties"
+msgstr "Propriétés du type d'activités"
+
 #: src/pyams_app_msc/shared/theater/zmi/viewlet.py:39
 msgid "My theaters"
 msgstr "Mes cinémas"
 
 #: src/pyams_app_msc/shared/theater/zmi/search.py:39
 msgid "Between all catalog contents"
 msgstr "Parmi tout le catalogue du cinéma"
@@ -2071,87 +2127,87 @@
 msgstr "Propriétés du public"
 
 #: src/pyams_app_msc/shared/theater/zmi/audience.py:251
 #, python-format
 msgid "Cinema audience: {}"
 msgstr "Public : {}"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:72
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:73
 msgid "Add movie theater"
 msgstr "Ajouter un cinéma"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:85
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:86
 msgid "Add theater"
 msgstr "Ajouter un cinéma"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:86
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:87
 msgid "New theater properties"
 msgstr "Propriétés du nouveau cinéma"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:106
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:107
 msgid "Movie theater name is required!"
 msgstr "Le nom du cinéma est obligatoire !"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:110
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:111
 msgid "A movie theater is already registered with this name!"
 msgstr "Un autre cinéma est déjà inscrit avec ce nom !"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:161
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:168
 msgid "Theater management"
 msgstr "Gérer le cinéma"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:172
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:179
 msgid "Properties"
 msgstr "Propriétés"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:183
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:190
 msgid "Movie theater properties"
 msgstr "Propriétés du cinéma"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:184
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:191
 msgid "Main theater properties"
 msgstr "Propriétés principales"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:197
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:204
 msgid "Contacts"
 msgstr "Contacts"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:231
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:238
 msgid "Settings"
 msgstr "Paramètres"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:241
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:248
 msgid "Movie theater settings"
 msgstr "Paramètres du cinéma"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:242
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:249
 msgid "Main theater settings"
 msgstr "Paramètres principaux"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:262
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:269
 msgid "Booking settings"
 msgstr "Gestion des réservations"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:275
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:282
 msgid "Booking cancel mode"
 msgstr "Gestion des annulations"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:289
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:296
 msgid "Cancel max delay must be set in \"max delay\" mode!"
 msgstr ""
 "Le délai maximum après la réservation doit être indiqué pour utiliser ce "
 "mode d'annulation !"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:292
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:299
 msgid "Cancel notice period must be set in \"notice period\" mode!"
 msgstr ""
 "Le préavis minimum avant l'événement doit être indiqué pour utiliser ce mode "
 "d'annulation !"
 
-#: src/pyams_app_msc/shared/theater/zmi/__init__.py:301
+#: src/pyams_app_msc/shared/theater/zmi/__init__.py:308
 msgid "Quotations settings"
 msgstr "Gestion des devis"
 
 #: src/pyams_app_msc/shared/theater/zmi/price.py:60
 #: src/pyams_app_msc/shared/theater/zmi/price.py:159
 msgid "Cinema prices"
 msgstr "Gestion des tarifs"
@@ -2766,15 +2822,15 @@
 
 #: src/pyams_app_msc/shared/catalog/interfaces.py:79
 msgid "Synopsis"
 msgstr "Synopsis"
 
 #: src/pyams_app_msc/shared/catalog/interfaces.py:94
 msgid "Catalog entry"
-msgstr "Entrée du catalogue"
+msgstr "Activité au catalogue"
 
 #: src/pyams_app_msc/shared/catalog/interfaces.py:100
 msgid "Title"
 msgstr "Titre"
 
 #: src/pyams_app_msc/shared/catalog/interfaces.py:101
 msgid ""
@@ -2796,29 +2852,29 @@
 msgid "TMDB movie ID"
 msgstr "ID TMDB du film"
 
 #: src/pyams_app_msc/shared/catalog/interfaces.py:114
 msgid "Movie ID in TMDB database"
 msgstr "Identifiant du film dans la base TMDB"
 
-#: src/pyams_app_msc/shared/catalog/zmi/dashboard.py:51
+#: src/pyams_app_msc/shared/catalog/zmi/dashboard.py:53
 msgid "Catalog management"
 msgstr "Gérer le catalogue"
 
-#: src/pyams_app_msc/shared/catalog/zmi/dashboard.py:58
+#: src/pyams_app_msc/shared/catalog/zmi/dashboard.py:69
 msgid "Activities catalog"
 msgstr "Gérer le catalogue"
 
 #: src/pyams_app_msc/shared/catalog/zmi/__init__.py:60
 msgid "Enter text for TMDB movie search"
 msgstr "Indiquez un titre pour rechercher dans TMDB..."
 
 #: src/pyams_app_msc/shared/catalog/zmi/__init__.py:93
 msgid "Add catalog entry"
-msgstr "Ajouter une entrée au catalogue"
+msgstr "Ajouter une activité au catalogue"
 
 #: src/pyams_app_msc/shared/catalog/zmi/__init__.py:102
 msgid "New catalog entry properties"
 msgstr "Propriétés de la nouvelle activité"
 
 #: src/pyams_app_msc/shared/catalog/zmi/__init__.py:173
 msgid "Activity details"
@@ -2854,29 +2910,29 @@
 
 #: src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py:40
 msgid "If 'no', number of free seats is not displayed"
 msgstr "Si 'non', le nombre de places libres ne sera pas affiché"
 
 #: src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py:65
 msgid "Catalog entries with next planned sessions"
-msgstr "Entrées du catalogue avec les prochaines séances"
+msgstr "Activités au catalogue avec les prochaines séances"
 
-#: src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:62
+#: src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:61
 msgid "${seats} seats"
 msgstr "${seats} places"
 
-#: src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:71
+#: src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:70
 msgid "Pagination"
 msgstr "Pagination"
 
-#: src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:79
+#: src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:78
 msgid "Previous page"
 msgstr "Page précédente"
 
-#: src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:86
+#: src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:85
 msgid "Next page"
 msgstr "Page suivante"
 
 #: src/pyams_app_msc/shared/catalog/skin/__init__.py:60
 msgid "(unknown)"
 msgstr "(inconnue)"
 
@@ -2940,15 +2996,15 @@
 
 #: src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt:113
 msgid "Synopsis:"
 msgstr "Synopsis :"
 
 #: src/pyams_app_msc/skin/__init__.py:52
 msgid "PyAMS MSC skin"
-msgstr "Thème commun \"Ma sortie cinéma\""
+msgstr "Thème commun \"Ma Séance Ciné\""
 
 #: src/pyams_app_msc/skin/login.py:99
 msgid "User profile is disabled!"
 msgstr "Ce profil utilisateur est désactivé !"
 
 #: src/pyams_app_msc/root/interfaces.py:31
 msgid "Sites managers"
@@ -2957,14 +3013,26 @@
 #: src/pyams_app_msc/root/interfaces.py:32
 msgid ""
 "These principals are allowed to create and manage sites and movie theaters"
 msgstr ""
 "Ces mandataires peuvent procéder à la création d'un nouveau cinéma et nommer "
 "ses gestionnaires"
 
+#~ msgid "Apartment"
+#~ msgstr "Appartement"
+
+#~ msgid "Floor, corridor..."
+#~ msgstr "Niveau, couloir..."
+
+#~ msgid "Entry"
+#~ msgstr "Entrée"
+
+#~ msgid "Entry, building, residence..."
+#~ msgstr "Entrée, bâtiment, résidence..."
+
 #~ msgid "Display all booked seats"
 #~ msgstr "Afficher les places libres"
 
 #~ msgid "Preferred audiences"
 #~ msgstr "Publics privilégiés"
 
 #~ msgid "Movie theater comment"
@@ -2984,17 +3052,14 @@
 
 #~ msgid "Add new catalog entry"
 #~ msgstr "Ajout d'une entrée du catalogue"
 
 #~ msgid "#Quotation: <b>{}</b>"
 #~ msgstr "N° de devis : <b>{}</b>"
 
-#~ msgid "Date: {}"
-#~ msgstr "Date : {}"
-
 #~ msgid "Accepted booking \"in option\""
 #~ msgstr "Réservation en attente de confirmation"
 
 #~ msgid "You can't create a new session starting before current date!"
 #~ msgstr ""
 #~ "Vous ne pouvez pas créer une nouvelle séance dont l'heure de début est "
 #~ "antérieure à l'heure actuelle !"
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/locales/pyams_app_msc.pot` & `pyams_app_msc-1.99.2/src/pyams_app_msc/locales/pyams_app_msc.pot`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2024-03-24 03:43+0100\n"
+"POT-Creation-Date: 2024-04-27 14:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -56,34 +56,72 @@
 msgid "MSC: Sites manager"
 msgstr ""
 
 #: ./src/pyams_app_msc/include.py:120
 msgid "MSC: Theater manager"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:139
+#: ./src/pyams_app_msc/include.py:140
 msgid "MSC: Theater operator"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:157
+#: ./src/pyams_app_msc/include.py:158
 msgid "MSC: Contributor"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:174
+#: ./src/pyams_app_msc/include.py:175
 msgid "MSC: Theater consultant"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:189
+#: ./src/pyams_app_msc/include.py:190
 msgid "MSC: Theater client"
 msgstr ""
 
-#: ./src/pyams_app_msc/include.py:201
+#: ./src/pyams_app_msc/include.py:202
 msgid "MSC: Reservation owner"
 msgstr ""
 
+#: ./src/pyams_app_msc/reference/structure/zmi/table.py:38
+#: ./src/pyams_app_msc/reference/structure/zmi/table.py:79
+msgid "Structures types"
+msgstr ""
+
+#: ./src/pyams_app_msc/reference/structure/zmi/table.py:56
+msgid "Table contents"
+msgstr ""
+
+#: ./src/pyams_app_msc/reference/structure/zmi/table.py:82
+msgid "Structures types list"
+msgstr ""
+
+#: ./src/pyams_app_msc/reference/structure/zmi/table.py:90
+msgid "Structures types table"
+msgstr ""
+
+#: ./src/pyams_app_msc/reference/structure/zmi/__init__.py:56
+msgid "Add structure type"
+msgstr ""
+
+#: ./src/pyams_app_msc/reference/structure/zmi/__init__.py:66
+msgid "New structure type"
+msgstr ""
+
+#: ./src/pyams_app_msc/reference/structure/zmi/__init__.py:67
+msgid "New structure type properties"
+msgstr ""
+
+#: ./src/pyams_app_msc/reference/structure/zmi/__init__.py:118
+#, python-format
+msgid "Structure type: {}"
+msgstr ""
+
+#: ./src/pyams_app_msc/reference/structure/zmi/__init__.py:121
+msgid "Structure type properties"
+msgstr ""
+
 #: ./src/pyams_app_msc/feature/tmdb/interfaces.py:41
 msgid "Enable TMDB configuration"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/tmdb/interfaces.py:45
 msgid "Service URL"
 msgstr ""
@@ -272,120 +310,136 @@
 msgid "TMDB service configuration"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/tmdb/zmi/__init__.py:64
 msgid "TMDB service properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:41
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:43
+msgid "Principal ID"
+msgstr ""
+
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:46
 msgid "Active user?"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:42
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:47
 msgid "Inactive users can't login anymore to website"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:46
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:51
 msgid "First name"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:49
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:54
 msgid "Last name"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:52
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:57
 msgid "Mail address"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:55
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:60
 #: ./src/pyams_app_msc/component/contact/interfaces.py:38
 #: ./src/pyams_app_msc/shared/theater/interfaces/__init__.py:92
 msgid "Phone number"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:58
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:63
 msgid "Establishment of affiliation"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:61
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:66
+msgid "Structure type"
+msgstr ""
+
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:67
+msgid "Select structure type matching this establishment"
+msgstr ""
+
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:71
 msgid "Establishment address"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:65
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:75
 msgid "Preferred local theaters"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:79
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:89
 msgid "Not displayed"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:80
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:90
 msgid "Display confirmed/requested/capacity seats"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:81
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:91
 msgid "Display confirmed/waiting/capacity seats"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:82
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:92
 msgid "Display confirmed/capacity seats"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:98
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:108
 msgid "Session seats display mode"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/interfaces.py:99
+#: ./src/pyams_app_msc/feature/profile/interfaces.py:109
 msgid ""
 "You can choose how session seats are displayed in movie theater planning view"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/profile/task.py:56
 msgid "User profile cleaner"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:62
 msgid "User add form"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:63
-#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:159
+#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:164
 msgid "User account settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:119
+#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:89
+msgid "Select structure type..."
+msgstr ""
+
+#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:124
 #: ./src/pyams_app_msc/feature/profile/skin/register.py:175
 msgid "This email address is already registered!"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:131
+#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:136
 msgid ""
 "This form allows you to register a new user account.\n"
 "If this user want to login, he will have to use the \"Forgotten password\" feature to get a new activation link to set his password."
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:144
+#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:149
 msgid "Disable profile"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:148
+#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:153
 msgid "Enable profile"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:158
+#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:163
 msgid "User edit form"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:196
+#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:204
 msgid ""
 "Disabled profiles can't be used for website login anymore but can still be "
 "assigned new bookings"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:284
+#: ./src/pyams_app_msc/feature/profile/zmi/__init__.py:292
 msgid "Operator profile"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt:53
 msgid "Edit user profile"
 msgstr ""
 
@@ -596,21 +650,26 @@
 msgid "Messaging service settings"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/messaging/zmi/__init__.py:54
 msgid "Messaging properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/session.py:156
+#: ./src/pyams_app_msc/feature/planning/session.py:155
+#: ./src/pyams_app_msc/feature/planning/zmi/session.py:236
+msgid "Out of catalog activity"
+msgstr ""
+
+#: ./src/pyams_app_msc/feature/planning/session.py:160
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:180
 #, python-format
 msgid "{room} - {date} from {start_time} to {end_time}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/session.py:184
+#: ./src/pyams_app_msc/feature/planning/session.py:188
 #, python-format
 msgid " {date} from {start_time} to {end_time}"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/interfaces.py:44
 msgid "Original version"
 msgstr ""
@@ -769,62 +828,58 @@
 msgid "New session"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/zmi/session.py:62
 msgid "New session properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/session.py:169
+#: ./src/pyams_app_msc/feature/planning/zmi/session.py:174
 msgid "Bookings"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/session.py:172
+#: ./src/pyams_app_msc/feature/planning/zmi/session.py:178
 msgid "Delete"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/session.py:182
+#: ./src/pyams_app_msc/feature/planning/zmi/session.py:188
 msgid "Session planning"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/session.py:183
+#: ./src/pyams_app_msc/feature/planning/zmi/session.py:189
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:468
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:665
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:715
 msgid "Session properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/session.py:230
-msgid "Out of catalog activity"
-msgstr ""
-
-#: ./src/pyams_app_msc/feature/planning/zmi/session.py:252
+#: ./src/pyams_app_msc/feature/planning/zmi/session.py:258
 msgid "You can't define a session gauge higher than the room's capacity!"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/session.py:257
+#: ./src/pyams_app_msc/feature/planning/zmi/session.py:263
 msgid "The number of validated seats is already higher than this gauge!"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/session.py:344
+#: ./src/pyams_app_msc/feature/planning/zmi/session.py:350
 msgid "Unknown room!"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/session.py:351
+#: ./src/pyams_app_msc/feature/planning/zmi/session.py:357
 msgid ""
 "Target room doesn't have enough capacity for confirmed seats of this session!"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/session.py:379
+#: ./src/pyams_app_msc/feature/planning/zmi/session.py:385
 msgid "Bad parameters"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/session.py:390
+#: ./src/pyams_app_msc/feature/planning/zmi/session.py:396
 msgid "Session updated"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/planning/zmi/session.py:391
+#: ./src/pyams_app_msc/feature/planning/zmi/session.py:397
 msgid "Session capacity has been reduced due to lower room capacity!"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/planning/zmi/__init__.py:64
 msgid "Planning"
 msgstr ""
 
@@ -996,15 +1051,15 @@
 
 #: ./src/pyams_app_msc/feature/quotation/__init__.py:443
 #, python-format
 msgid "Quotation: {}"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/reminder.py:50
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:769
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:819
 #: ./src/pyams_app_msc/shared/theater/zmi/mail.py:142
 msgid "Booking reminder"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:75
 msgid "Waiting"
 msgstr ""
@@ -1023,37 +1078,37 @@
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:79
 msgid "Accepted"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:109
 #: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:232
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:125
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:126
 msgid "Creator"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:110
 msgid "Name of the principal who created the booking"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:113
 #: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:248
 #: ./src/pyams_app_msc/feature/booking/zmi/search.py:71
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:139
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:140
 msgid "Recipient"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:114
 msgid "Name of the principal for which the booking is done"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:120
 #: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:292
 #: ./src/pyams_app_msc/feature/booking/zmi/search.py:74
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:182
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:183
 msgid "Status"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:125
 msgid "Participants"
 msgstr ""
 
@@ -1094,26 +1149,26 @@
 msgid ""
 "You can set an integer number which will define the count of participants for"
 " which one accompanying person will have free access"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:156
 #: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:262
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:168
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:169
 #: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:46
 msgid "Cultural pass"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:157
 msgid "Check this option if payment is done using cultural pass"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:161
 #: ./src/pyams_app_msc/feature/booking/skin/__init__.py:53
-#: ./src/pyams_app_msc/component/address/interfaces.py:49
+#: ./src/pyams_app_msc/component/address/interfaces.py:41
 #: ./src/pyams_app_msc/shared/theater/interfaces/audience.py:50
 #: ./src/pyams_app_msc/shared/theater/interfaces/price.py:58
 msgid "Comments"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:162
 msgid "These comments where added by booking recipient"
@@ -1145,15 +1200,15 @@
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:192
 msgid "This message is added to quotation as an information message"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:195
 #: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:310
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:213
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:214
 msgid "Quotation"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/interfaces.py:196
 msgid "This quotation was attached to booking confirmation"
 msgstr ""
 
@@ -1288,21 +1343,21 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:217
 msgid "Change session"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:221
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:460
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:510
 msgid "Cancel"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:234
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:367
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:473
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:523
 #, python-format
 msgid "Booking: {}"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:237
 msgid "Change booking session"
 msgstr ""
@@ -1318,15 +1373,15 @@
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:303
 #, python-format
 msgid "There are only {} free seats left in this session!"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:370
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:489
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:477
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:527
 msgid "Booking properties"
 msgstr ""
 
 #. Default: Cancel booking
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:622
 msgid "cancel-booking-menu"
 msgstr ""
@@ -1349,15 +1404,15 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:669
 msgid "Booking refused"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:682
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:447
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:497
 msgid "Quotation preview"
 msgstr ""
 
 #. Default: Optional booking
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:701
 msgid "option-booking-menu"
 msgstr ""
@@ -1392,15 +1447,15 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:780
 msgid "Booking accepted"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:826
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:653
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:703
 msgid "You must set a price to accept a booking!"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/workflow.py:908
 msgid ""
 "**WARNING**<br />The session capacity is too low to accept this booking!"
 msgstr ""
@@ -1437,15 +1492,15 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:216
 msgid "Date"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:276
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:198
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:199
 msgid "Seats"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/dashboard.py:331
 msgid "Last update"
 msgstr ""
 
@@ -1505,81 +1560,90 @@
 msgid "Today program"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/home.py:67
 msgid "Sessions planned for today"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:153
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:154
 msgid "Establishment"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:240
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:241
 msgid "Archived booking"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:276
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:277
 msgid "Current session bookings"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:288
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:293
 msgid "Session bookings"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:302
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:298
+#, python-format
+msgid " (Seats: {})"
+msgstr ""
+
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:314
 #, python-format
 msgid "{}: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:329
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:341
 msgid "Add booking"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:348
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:358
+msgid "Add and accept"
+msgstr ""
+
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:368
 msgid "New booking"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:349
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:369
 msgid "New booking properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:450
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:500
 msgid "Reset quotation"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:456
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:506
 msgid "Apply"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:624
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:674
 msgid "This booking is archived and can't be modified anymore!"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:693
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:743
 msgid "Booking quotation"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:711
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:761
 msgid "Booking update"
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:746
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:796
 msgid ""
 "Update message can be sent to booking recipient when a booking is modified "
 "after being validated."
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:807
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:857
 #, python-format
 msgid ""
 "Reminder message will be sent to booking recipient {} hours before session "
 "begin date..."
 msgstr ""
 
-#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:822
+#: ./src/pyams_app_msc/feature/booking/zmi/__init__.py:872
 msgid "Quotation has been reset!"
 msgstr ""
 
 #: ./src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt:52
 msgid "${groups}: ${participants} participants, ${accompanists} accompanists"
 msgstr ""
 
@@ -1672,50 +1736,34 @@
 #: ./src/pyams_app_msc/component/banking/interfaces.py:68
 msgid ""
 "Banking account information must contain bank code, counter code, account "
 "number and account key"
 msgstr ""
 
 #: ./src/pyams_app_msc/component/address/interfaces.py:28
-msgid "Apartment"
-msgstr ""
-
-#: ./src/pyams_app_msc/component/address/interfaces.py:29
-msgid "Floor, corridor..."
-msgstr ""
-
-#: ./src/pyams_app_msc/component/address/interfaces.py:32
-msgid "Entry"
-msgstr ""
-
-#: ./src/pyams_app_msc/component/address/interfaces.py:33
-msgid "Entry, building, residence..."
-msgstr ""
-
-#: ./src/pyams_app_msc/component/address/interfaces.py:36
 msgid "Number and street"
 msgstr ""
 
-#: ./src/pyams_app_msc/component/address/interfaces.py:37
+#: ./src/pyams_app_msc/component/address/interfaces.py:29
 msgid "Entry number and street name"
 msgstr ""
 
-#: ./src/pyams_app_msc/component/address/interfaces.py:40
+#: ./src/pyams_app_msc/component/address/interfaces.py:32
 msgid "Locality"
 msgstr ""
 
-#: ./src/pyams_app_msc/component/address/interfaces.py:43
+#: ./src/pyams_app_msc/component/address/interfaces.py:35
 msgid "Postal code"
 msgstr ""
 
-#: ./src/pyams_app_msc/component/address/interfaces.py:46
+#: ./src/pyams_app_msc/component/address/interfaces.py:38
 msgid "City"
 msgstr ""
 
-#: ./src/pyams_app_msc/component/address/interfaces.py:50
+#: ./src/pyams_app_msc/component/address/interfaces.py:42
 msgid "Optional observations which can be added to describe the location"
 msgstr ""
 
 #: ./src/pyams_app_msc/component/contact/interfaces.py:30
 msgid "Full name"
 msgstr ""
 
@@ -1852,30 +1900,38 @@
 msgid "Catalog template configuration"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/presentation.py:67
 msgid "Catalog layout"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/types.py:43
+#: ./src/pyams_app_msc/shared/theater/zmi/types.py:46
 msgid "Activity types"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/types.py:53
+#: ./src/pyams_app_msc/shared/theater/zmi/types.py:56
 msgid "Add activity type"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/types.py:73
+#: ./src/pyams_app_msc/shared/theater/zmi/types.py:65
+msgid "New activity type"
+msgstr ""
+
+#: ./src/pyams_app_msc/shared/theater/zmi/types.py:79
 msgid "Activities types"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/types.py:74
+#: ./src/pyams_app_msc/shared/theater/zmi/types.py:80
 msgid "Movie theater activities types list"
 msgstr ""
 
+#: ./src/pyams_app_msc/shared/theater/zmi/types.py:93
+msgid "Activity type properties"
+msgstr ""
+
 #: ./src/pyams_app_msc/shared/theater/zmi/viewlet.py:39
 msgid "My theaters"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/search.py:39
 msgid "Between all catalog contents"
 msgstr ""
@@ -1927,83 +1983,83 @@
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/audience.py:251
 #, python-format
 msgid "Cinema audience: {}"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:72
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:73
 msgid "Add movie theater"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:85
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:86
 msgid "Add theater"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:86
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:87
 msgid "New theater properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:106
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:107
 msgid "Movie theater name is required!"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:110
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:111
 msgid "A movie theater is already registered with this name!"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:161
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:168
 msgid "Theater management"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:172
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:179
 msgid "Properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:183
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:190
 msgid "Movie theater properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:184
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:191
 msgid "Main theater properties"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:197
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:204
 msgid "Contacts"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:231
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:238
 msgid "Settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:241
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:248
 msgid "Movie theater settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:242
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:249
 msgid "Main theater settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:262
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:269
 msgid "Booking settings"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:275
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:282
 msgid "Booking cancel mode"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:289
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:296
 msgid "Cancel max delay must be set in \"max delay\" mode!"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:292
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:299
 msgid "Cancel notice period must be set in \"notice period\" mode!"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:301
+#: ./src/pyams_app_msc/shared/theater/zmi/__init__.py:308
 msgid "Quotations settings"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/theater/zmi/price.py:60
 #: ./src/pyams_app_msc/shared/theater/zmi/price.py:159
 msgid "Cinema prices"
 msgstr ""
@@ -2569,19 +2625,19 @@
 msgid "TMDB movie ID"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/catalog/interfaces.py:114
 msgid "Movie ID in TMDB database"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/zmi/dashboard.py:51
+#: ./src/pyams_app_msc/shared/catalog/zmi/dashboard.py:53
 msgid "Catalog management"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/zmi/dashboard.py:58
+#: ./src/pyams_app_msc/shared/catalog/zmi/dashboard.py:69
 msgid "Activities catalog"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/catalog/zmi/__init__.py:60
 msgid "Enter text for TMDB movie search"
 msgstr ""
 
@@ -2629,27 +2685,27 @@
 msgid "If 'no', number of free seats is not displayed"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py:65
 msgid "Catalog entries with next planned sessions"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:62
+#: ./src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:61
 msgid "${seats} seats"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:71
+#: ./src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:70
 msgid "Pagination"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:79
+#: ./src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:78
 msgid "Previous page"
 msgstr ""
 
-#: ./src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:86
+#: ./src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt:85
 msgid "Next page"
 msgstr ""
 
 #: ./src/pyams_app_msc/shared/catalog/skin/__init__.py:60
 msgid "(unknown)"
 msgstr ""
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/reference/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/reference/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/reference/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/reference/zmi/viewlet.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/reference/zmi/viewlet.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 """
 
 __docformat__ = 'restructuredtext'
 
 from zope.interface import Interface
 
-from pyams_content.interfaces import MANAGE_SITE_ROOT_PERMISSION
+from pyams_content.interfaces import MANAGE_REFERENCE_TABLE_PERMISSION
 from pyams_content.reference.zmi.viewlet import ReferencesTablesMenu
 from pyams_content.zmi.viewlet.toplinks import TopTabsViewletManager
 from pyams_viewlet.manager import viewletmanager_config
 from pyams_zmi.interfaces import IAdminLayer
 
 
 @viewletmanager_config(name='reference-tables.menu',
                        context=Interface, layer=IAdminLayer,
                        manager=TopTabsViewletManager, weight=40)
 class MSCReferencesTablesMenu(ReferencesTablesMenu):
     """MSC reference tables menu"""
 
-    menus_permissions = {MANAGE_SITE_ROOT_PERMISSION}
+    menus_permissions = {MANAGE_REFERENCE_TABLE_PERMISSION}
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/root/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/root/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/root/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/root/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/root/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/root/zmi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,30 +14,40 @@
 
 """
 
 __docformat__ = 'restructuredtext'
 
 from pyams_app_msc.interfaces import VIEW_THEATER_PERMISSION
 from pyams_app_msc.shared.theater import IMovieTheater
-from pyams_content.interfaces import MANAGE_SITE_TREE_PERMISSION
+from pyams_content.interfaces import MANAGE_REFERENCE_TABLE_PERMISSION, MANAGE_SITE_TREE_PERMISSION
+from pyams_content.reference import IReferenceTable
 from pyams_viewlet.manager import viewletmanager_config
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.interfaces.viewlet import INavigationViewletManager, ISiteManagementMenu
 from pyams_zmi.zmi.viewlet.menu import SiteManagementMenu
 
 
 @viewletmanager_config(name='site-manager.menu',
                        layer=IAdminLayer,
                        manager=INavigationViewletManager, weight=200,
                        provides=ISiteManagementMenu,
                        permission=MANAGE_SITE_TREE_PERMISSION)
 class MSCSiteManagementMenu(SiteManagementMenu):
-    """MSC Site management menu"""
+    """MSC site management menu"""
+
+
+@viewletmanager_config(name='site-manager.menu',
+                       context=IReferenceTable, layer=IAdminLayer,
+                       manager=INavigationViewletManager, weight=200,
+                       provides=ISiteManagementMenu,
+                       permission=MANAGE_REFERENCE_TABLE_PERMISSION)
+class MSCReferenceTableManagementMenu(SiteManagementMenu):
+    """MSC reference table site management menu"""
 
 
 @viewletmanager_config(name='site-manager.menu',
                        context=IMovieTheater, layer=IAdminLayer,
                        manager=INavigationViewletManager, weight=200,
                        provides=ISiteManagementMenu,
                        permission=VIEW_THEATER_PERMISSION)
 class MSCMovieTheaterSiteManagementMenu(SiteManagementMenu):
-    """MSC movie theater Site management menu"""
+    """MSC movie theater site management menu"""
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from zope.container.contained import Contained
 from zope.interface import implementer
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_app_msc.feature.tmdb.interfaces import ITMDBServiceClientTarget
 from pyams_app_msc.shared.catalog.interfaces import CATALOG_ENTRY_CONTENT_NAME, CATALOG_ENTRY_CONTENT_TYPE, \
     CATALOG_ENTRY_INFORMATION_KEY, ICatalogEntry, ICatalogEntryInfo, IWfCatalogEntry
-from pyams_content.component.gallery.interfaces import IGalleryTarget
 from pyams_content.component.illustration.interfaces import IIllustrationTarget, ILinkIllustrationTarget
 from pyams_content.component.paragraph.interfaces import IParagraphContainerTarget
 from pyams_content.component.thesaurus.interfaces import ITagsTarget, IThemesTarget
 from pyams_content.feature.preview.interfaces import IPreviewTarget
 from pyams_content.feature.review.interfaces import IReviewTarget
 from pyams_content.shared.common import SharedContent, WfSharedContent
 from pyams_content.shared.common.interfaces import ISharedContent, IWfSharedContent
@@ -39,15 +38,15 @@
 from pyams_utils.factory import factory_config
 from pyams_utils.traversing import get_parent
 
 
 @factory_config(IWfCatalogEntry)
 @factory_config(IWfSharedContent, name=CATALOG_ENTRY_CONTENT_TYPE)
 @implementer(ITMDBServiceClientTarget,
-             IIllustrationTarget, ILinkIllustrationTarget, IGalleryTarget,
+             IIllustrationTarget, ILinkIllustrationTarget,
              IParagraphContainerTarget, ITagsTarget, IThemesTarget,
              IPortalContext, IReviewTarget, IPreviewTarget)
 class WfCatalogEntry(WfSharedContent, WfTypedSharedContentMixin):
     """Catalog entry"""
 
     content_type = CATALOG_ENTRY_CONTENT_TYPE
     content_name = CATALOG_ENTRY_CONTENT_NAME
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/api/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/index.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/index.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/manager.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/page.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/page.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 		<span class="position-absolute underline"></span>
 	</h3>
 	<div class="row row-cols-1 row-cols-sm-2 row-cols-md-3"
 		 tal:define="global count 0;">
 		<div class="col my-3 d-flex flex-column"
 			 tal:repeat="item results">
 			<tal:var define="global count count + 1;
-							 target view.get_url(item);
-							 illustration tales:pyams_illustration(item);">
+							 target view.get_url(item);">
 				<div class="position-relative"
-					 tal:define="illustration tales:pyams_illustration(item)"
+					 tal:define="illustration tales:pyams_navigation_illustration(item)"
 					 tal:condition="illustration">
 					<a href="${target}">
 						${structure:tales:pyams_card_datatype(item)}
 						<tal:if define="image i18n:illustration.data;
 										alt_title i18n:illustration.alt_title;"
 								condition="image">
 							${structure:tales:picture(image,
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/search.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/security.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/security.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/skin/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/catalog/zmi/workflow.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/common/zmi/viewlet.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/site/zmi/viewlet.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from pyams_app_msc.shared.theater.interfaces import IMovieTheater, IMovieTheaterRoles, IMovieTheaterSettings, \
     MOVIE_THEATER_ROLES, MOVIE_THEATER_SETTINGS_KEY, MSC_THEATERS_VOCABULARY
 from pyams_app_msc.shared.theater.interfaces.audience import ICinemaAudienceContainerTarget
 from pyams_app_msc.shared.theater.interfaces.mail import IMailTemplatesTarget
 from pyams_app_msc.shared.theater.interfaces.price import ICinemaPriceContainerTarget
 from pyams_app_msc.shared.theater.interfaces.room import ICinemaRoomContainer, ICinemaRoomContainerTarget
 from pyams_content.component.illustration.interfaces import IIllustrationTarget, ILinkIllustrationTarget
+from pyams_content.component.paragraph.interfaces import IParagraphFactorySettingsTarget
 from pyams_content.feature.preview.interfaces import IPreviewTarget
 from pyams_content.interfaces import IObjectType
 from pyams_content.shared.common.interfaces import CONTENT_MANAGER_ROLES, ISharedContent
 from pyams_content.shared.common.manager import BaseSharedTool
 from pyams_content.shared.common.types import TypedSharedToolMixin
 from pyams_file.property import FileProperty
 from pyams_i18n.interfaces import II18n
@@ -54,15 +55,15 @@
 
 from pyams_app_msc import _
 
 
 @factory_config(IMovieTheater)
 @implementer(IDefaultProtectionPolicy, IIllustrationTarget, ILinkIllustrationTarget,
              ICinemaRoomContainerTarget, ICinemaPriceContainerTarget, ICinemaAudienceContainerTarget,
-             ICatalogManagerTarget, IMailTemplatesTarget,
+             ICatalogManagerTarget, IMailTemplatesTarget, IParagraphFactorySettingsTarget,
              IPortalContext, IPortalHeaderContext, IPortalFooterContext, IPreviewTarget)
 class Theater(OrderedContainer, BaseSharedTool, TypedSharedToolMixin,
               ProtectedObjectMixin, UserSkinnableContentMixin):
     """Main theater persistent class"""
 
     title = FieldProperty(IMovieTheater['title'])
     short_name = FieldProperty(IMovieTheater['short_name'])
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/price.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/api/schema.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/audience.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/audience.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/mail.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/price.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/interfaces/room.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/mail.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/page.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/page.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/price.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/room.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/session.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/settings.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/settings.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """PyAMS_*** module
 
 """
 
 from pyramid.events import subscriber
 from zope.interface import Interface, Invalid
 
+from pyams_app_msc.shared.catalog import IWfCatalogEntry
 from pyams_app_msc.shared.theater import IMovieTheater, IMovieTheaterSettings
 from pyams_app_msc.shared.theater.interfaces import BOOKING_CANCEL_MODE
 from pyams_content.interfaces import IBaseContent, MANAGE_SITE_TREE_PERMISSION
 from pyams_content.root.zmi.sites import SiteRootSitesTable
 from pyams_content.zmi.properties import PropertiesEditForm
 from pyams_form.ajax import AJAXFormRenderer, ajax_form_config
 from pyams_form.field import Fields
@@ -146,17 +147,23 @@
 class MovieTheaterBreadcrumbs(BreadcrumbItem):
     """Movie theater breadcrumb item"""
 
     @property
     def label(self):
         return II18n(self.context).query_attribute('short_name', request=self.request)
 
-    view_name = 'admin'
     css_class = 'breadcrumb-item persistent strong'
 
+    @property
+    def view_name(self):
+        """Movie theater breadcrumb view getter"""
+        if IWfCatalogEntry.providedBy(self.request.context):
+            return 'admin#dashboard.html'
+        return 'admin'
+
 
 @adapter_config(required=(IMovieTheater, IAdminLayer, Interface, ISiteManagementMenu),
                 provides=IMenuHeader)
 def movie_theater_management_menu_header(context, request, view, manager):
     """Movie theater management menu header adapter"""
     return _("Theater management")
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/audience.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/interfaces.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/mail.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/planning.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/planning.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,41 +16,38 @@
 
 __docformat__ = 'restructuredtext'
 
 from datetime import datetime
 
 from hypatia.catalog import CatalogQuery
 from hypatia.interfaces import ICatalog
-from hypatia.query import And, Eq, Le, Ge
-from pyramid.httpexceptions import HTTPNotFound, HTTPBadRequest
+from hypatia.query import And, Eq, Ge, Le
+from pyramid.httpexceptions import HTTPBadRequest, HTTPNotFound
 from pyramid.view import view_config
 
+from pyams_app_msc.feature.booking.zmi.interfaces import IBookingManagementMenu
 from pyams_app_msc.feature.planning import IPlanning
 from pyams_app_msc.feature.planning.interfaces import ISession
 from pyams_app_msc.feature.planning.zmi import PlanningMenu, PlanningView
 from pyams_app_msc.interfaces import VIEW_CATALOG_PERMISSION
 from pyams_app_msc.shared.theater import ICinemaRoomContainer, IMovieTheater
 from pyams_catalog.query import CatalogResultSet
 from pyams_content_api.feature.json import IJSONExporter
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_pagelet.pagelet import pagelet_config
 from pyams_security.interfaces.base import USE_INTERNAL_API_PERMISSION
 from pyams_utils.factory import get_interface_base_name
 from pyams_utils.registry import get_utility
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.interfaces import IAdminLayer
-from pyams_zmi.interfaces.viewlet import IContentManagementMenu
-from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
-
-from pyams_app_msc import _
 
 
 @viewlet_config(name='planning.menu',
                 context=IMovieTheater, layer=IAdminLayer,
-                manager=IContentManagementMenu, weight=7,
+                manager=IBookingManagementMenu, weight=7,
                 permission=VIEW_CATALOG_PERMISSION)
 class MovieTheaterPlanningMenu(PlanningMenu):
     """Movie theater planning menu"""
 
 
 @pagelet_config(name='planning.html',
                 context=IMovieTheater, layer=IPyAMSLayer,
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/presentation.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/presentation.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/price.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/restrictions.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/restrictions.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/room.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/search.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/session.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,34 +12,46 @@
 
 """PyAMS_*** module
 
 """
 
 __docformat__ = 'restructuredtext'
 
+from pyramid.view import view_config
 from zope.interface import alsoProvides
 
 from pyams_app_msc.feature.planning.interfaces import IMovieTheaterSession, IPlanning, ISession
 from pyams_app_msc.feature.planning.zmi.session import SessionAddForm
 from pyams_app_msc.interfaces import MANAGE_CATALOG_PERMISSION
 from pyams_app_msc.shared.catalog.interfaces import CATALOG_ENTRY_CONTENT_TYPE
 from pyams_app_msc.shared.theater.interfaces import IMovieTheater
 from pyams_app_msc.zmi import msc
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
 from pyams_layer.interfaces import IPyAMSLayer
+from pyams_security.interfaces.base import USE_INTERNAL_API_PERMISSION
+from pyams_sequence.api.rest import find_references
 from pyams_sequence.reference import get_reference_target
 from pyams_utils.fanstatic import get_resource_path
 from pyams_utils.interfaces.data import IObjectData
 from pyams_utils.interfaces.form import NO_VALUE_STRING
-
+from pyams_utils.url import absolute_url
 
 IMovieTheaterSession['activity'].content_type = CATALOG_ENTRY_CONTENT_TYPE
 
 
+@view_config(name='find-references.json',
+             context=IMovieTheater, request_type=IPyAMSLayer,
+             permission=USE_INTERNAL_API_PERMISSION,
+             renderer='json', xhr=True)
+def find_theater_references(request):
+    """Returns list of references matching given query inside theater context"""
+    return find_references(request, parent=request.context, validate=False)
+
+
 @ajax_form_config(name='add-session.html',
                   context=IMovieTheater, layer=IPyAMSLayer,
                   permission=MANAGE_CATALOG_PERMISSION)
 class MovieTheaterSessionAddForm(SessionAddForm):
     """Movie theater session add form"""
 
     @property
@@ -53,14 +65,15 @@
 
     planning_target = None
 
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         activity = self.widgets.get('activity')
         if activity is not None:
+            activity.ajax_url = absolute_url(self.context, self.request, 'find-references.json')
             activity.object_data = {
                 'ams-modules': {
                     'msc': {
                         'src': get_resource_path(msc)
                     }
                 },
                 'ams-change-handler': 'MyAMS.msc.session.changeActivity'
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/types.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,34 +12,37 @@
 
 """PyAMS_*** module
 
 """
 
 from pyams_app_msc.shared.theater import IMovieTheater
 from pyams_content.interfaces import MANAGE_TOOL_PERMISSION
-from pyams_content.shared.common.interfaces.types import IDataType
-from pyams_content.shared.common.zmi.types import DataTypeAddForm, DataTypeEditForm, DataTypesAddAction, \
-    ISharedToolTypesTable
+from pyams_content.shared.common.interfaces.types import IDataType, ITypedSharedTool
+from pyams_content.shared.common.zmi.types import DataTypeAddForm, DataTypeEditForm, DataTypePictogramsGroup, \
+    DataTypesAddAction
 from pyams_content.shared.common.zmi.types.container import SharedToolTypesMenu, SharedToolTypesView
+from pyams_content.shared.common.zmi.types.interfaces import ISharedToolTypesTable
 from pyams_form.ajax import ajax_form_config
+from pyams_form.interfaces.form import IGroup
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_pagelet.pagelet import pagelet_config
+from pyams_utils.adapter import adapter_config
 from pyams_utils.traversing import get_parent
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.interfaces.viewlet import IPropertiesMenu, IToolbarViewletManager
 
 __docformat__ = 'restructuredtext'
 
 from pyams_app_msc import _
 
 
 @viewlet_config(name='data-types.menu',
                 context=IMovieTheater, layer=IAdminLayer,
-                manager=IPropertiesMenu, weight=400,
+                manager=IPropertiesMenu, weight=405,
                 permission=MANAGE_TOOL_PERMISSION)
 class MovieTheaterSharedToolTypesMenu(SharedToolTypesMenu):
     """Shared tool data types menu"""
 
     label = _("Activity types")
 
 
@@ -55,17 +58,20 @@
 
 @ajax_form_config(name='add-data-type.html',
                   context=IMovieTheater, layer=IPyAMSLayer,
                   permission=MANAGE_TOOL_PERMISSION)
 class MovieTheaterDataTypeAddForm(DataTypeAddForm):
     """Movie theater data type add form"""
 
+    subtitle = _("New activity type")
+
     @property
     def fields(self):
-        return super().fields.omit('source_folder')
+        return super().fields.omit('source_folder', 'navigation_label', 'backoffice_label',
+                                   'color', 'pictogram')
 
 
 @pagelet_config(name='data-types.html',
                 context=IMovieTheater, layer=IPyAMSLayer,
                 permission=MANAGE_TOOL_PERMISSION)
 class MovieTheaterSharedToolTypesView(SharedToolTypesView):
     """Movie theater data types view"""
@@ -77,13 +83,37 @@
 @ajax_form_config(name='properties.html',
                   context=IDataType, layer=IPyAMSLayer,
                   permission=MANAGE_TOOL_PERMISSION)
 class MovieTheaterDataTypeEditForm(DataTypeEditForm):
     """Movie theater data type properties edit form"""
 
     @property
+    def legend(self):
+        manager = get_parent(self.context, IMovieTheater)
+        if manager is not None:
+            return _("Activity type properties")
+        return super().legend
+
+    @property
     def fields(self):
         fields = super().fields
         manager = get_parent(self.context, IMovieTheater)
         if manager is not None:
-            fields = fields.omit('source_folder')
+            fields = fields.omit('source_folder', 'navigation_label', 'backoffice_label',
+                                 'color', 'pictogram')
         return fields
+
+
+@adapter_config(name='add-data-type-pictograms.group',
+                required=(ITypedSharedTool, IAdminLayer, DataTypeAddForm),
+                provides=IGroup)
+@adapter_config(name='edit-data-type-pictograms.group',
+                required=(IDataType, IAdminLayer, DataTypeEditForm),
+                provides=IGroup)
+class MovieTheaterDataTypePictogramsGroup(DataTypePictogramsGroup):
+    """Movie theater data type pictograms group"""
+
+    def __new__(cls, context, request, view):
+        manager = get_parent(context, IMovieTheater)
+        if manager is not None:
+            return None
+        return DataTypePictogramsGroup.__new__(cls)
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/shared/theater/zmi/viewlet.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/form.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/form.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/layer.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/layer.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/login.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/login.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_form.js` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_form.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_gis.js` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_gis.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_search.js` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_search.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/_utils.js` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_utils.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/js/app.js` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/app.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_content.scss` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_content.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_footer.scss` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_footer.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_forms.scss` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_forms.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_layout.scss` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_layout.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_misc.scss` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_misc.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/_variables.scss` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_variables.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/resources/src/sass/msc.scss` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/msc.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/skin/templates/select-admin-theater.pt` & `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/templates/select-admin-theater.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/tests/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/tests/test_utilsdocs.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/tests/test_utilsdocstrings.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/__init__.py` & `pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/resources/js/msc.js` & `pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/js/msc.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -174,14 +174,19 @@
 
         renderedEvent: (info) => {
             const elt = $(info.el);
             elt.data('msc-event', info.event)
                 .contextMenu({
                     menuSelector: '#eventMenu'
                 });
+            const title = info.event.title.split('\n');
+            elt.tooltip({
+                title: `<strong>${title[0]}</strong><br />Places: ${title[1].replace(/\(/, '').replace(/\)/, '') || ''}`,
+                html: true
+            });
         },
 
         /**
          * Transpose plannings
          */
         transpose: (source) => {
             const wrapper = $('.calendar-wrapper');
@@ -239,14 +244,15 @@
          */
         setDates: (dateInfo) => {
 
             function clearUpdates() {
                 msc.calendar.updating.splice(0, msc.calendar.updating.length);
             }
 
+            $('.tooltip').tooltip('hide');
             if (!msc.calendar.synchronized) {
                 return;
             }
             const updating = msc.calendar.updating;
             if (updating.indexOf(dateInfo.view.calendar) > -1) {
                 return;
             }
@@ -271,27 +277,29 @@
         /**
          * Add new event to calendar
          */
         addEvent: (info) => {
             const source = info.jsEvent.target,
                 calendar = $(source).parents('.calendar'),
                 room = calendar.data('msc-room');
+            $('.tooltip').tooltip('hide');
             if (calendar.data('msc-editable') !== 'True') {
                 return;
             }
             MyAMS.require('modal').then(() => {
                 MyAMS.modal.open('add-session.html', {
                     start: info.dateStr,
                     room: room
                 });
             });
         },
 
         cloneEvent: (menu, source) => {
             return () => {
+                $('.tooltip').tooltip('hide');
                 MyAMS.require('ajax').then(() => {
                     const event = source.data('msc-event');
                     MyAMS.ajax.post(`${event.extendedProps.href}/clone-event.json`).then((result) => {
                         if (result.status === 'success') {
                             MyAMS.msc.calendar.refresh(result.event.room);
                         }
                     });
@@ -302,24 +310,26 @@
         /**
          * Update calendar after event creation
          */
         addEventCallback: (form, options) => {
             const
                 event = options.event,
                 roomName = event.room;
+            $('.tooltip').tooltip('hide');
             MyAMS.msc.calendar.refresh(roomName);
         },
 
         /**
          * Show event properties on click
          */
         showEvent: (info) => {
             const
                 event = info.event,
                 visible = event.extendedProps?.visible;
+            $('.tooltip').tooltip('hide');
             if (visible) {
                 const href = event.extendedProps?.href;
                 if (href) {
                     MyAMS.require('modal').then(() => {
                         MyAMS.modal.open(`${href}/properties.html`);
                     });
                 }
@@ -330,14 +340,15 @@
          * Update calendars after event update
          */
         editEventCallback: (form, options) => {
             const
                 event = options.event,
                 eventRoomName = event.room.toString(),
                 calendars = $('.calendar');
+            $('.tooltip').tooltip('hide');
             calendars.each((idx, elt) => {
                 const
                     calendar = $(elt),
                     calendarRoomName = calendar.data('msc-room').toString(),
                     plugin = calendar.data('msc-calendar');
                 if (calendarRoomName === eventRoomName) {
                     plugin.refetchEvents();
@@ -350,14 +361,15 @@
             });
         },
 
         /**
          * Change event by drag & drop on same calendar
          */
         dropEvent: (info) => {
+            $('.tooltip').tooltip('hide');
             return new Promise((resolve, reject) => {
                 const
                     event = info.event,
                     href = event.extendedProps?.href;
                 if (href) {
                     MyAMS.require('ajax').then(() => {
                         MyAMS.ajax.post(`${href}/update-event.json`, {
@@ -378,14 +390,15 @@
             });
         },
 
         /**
          * Update event duration by drag & drop
          */
         resizeEvent: (info) => {
+            $('.tooltip').tooltip('hide');
             return new Promise((resolve, reject) => {
                 const
                     event = info.event,
                     href = event.extendedProps?.href;
                 if (href) {
                     MyAMS.require('ajax').then(() => {
                         MyAMS.ajax.post(`${href}/update-event.json`, {
@@ -406,14 +419,15 @@
             });
         },
 
         /**
          * Drag event to another calendar
          */
         receiveEvent: (info) => {
+            $('.tooltip').tooltip('hide');
             return new Promise((resolve, reject) => {
                 const
                     event = info.event,
                     href = event.extendedProps?.href;
                 if (href) {
                     const target = $(info.view.calendar.el),
                         targetPlugin = target.data('msc-calendar'),
@@ -454,14 +468,15 @@
         /**
          * Delete event callback
          */
         deleteEventCallback: (form, options) => {
             const calendar = $(`.calendar[data-msc-room="${options.room}"]`),
                 plugin = calendar.data('msc-calendar'),
                 event = plugin.getEventById(options.event_id);
+            $('.tooltip').tooltip('hide');
             if (event) {
                 event.remove();
             }
         },
 
         /**
          * Manage event booking
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc/zmi/resources/js/msc.min.js` & `pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/js/msc.min.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -64,16 +64,21 @@
             }
         },
         setEventClassNames: e => {
             let t = "";
             return e.event.extendedProps.temporary && (t = "font-italic"), e.event.extendedProps.borderWidth && (t += " border-" + e.event.extendedProps.borderWidth), e.event.extendedProps.borderStyle && (t += " border-" + e.event.extendedProps.borderStyle), t
         },
         renderedEvent: e => {
-            $(e.el).data("msc-event", e.event).contextMenu({
-                menuSelector: "#eventMenu"
+            var t = $(e.el),
+                e = (t.data("msc-event", e.event).contextMenu({
+                    menuSelector: "#eventMenu"
+                }), e.event.title.split("\n"));
+            t.tooltip({
+                title: `<strong>${e[0]}</strong><br />Places: ` + (e[1].replace(/\(/, "").replace(/\)/, "") || ""),
+                html: !0
             })
         },
         transpose: e => {
             var t = $(".calendar-wrapper"),
                 e = (t.toggleClass("transposed"), $(".calendar").each((e, t) => {
                     $(t).data("msc-calendar").render()
                 }), e.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), t.hasClass("transposed"));
@@ -91,15 +96,15 @@
                     msc.calendar.synchronized = !0
                 }
             }
             e.button("toggle").toggleClass("btn-light").toggleClass("btn-link").toggleClass("btn-secondary").toggleClass("border-secondary"), localStorage.setItem("msc.synchronized", e.hasClass("btn-secondary"))
         },
         updating: [],
         setDates: a => {
-            if (msc.calendar.synchronized) {
+            if ($(".tooltip").tooltip("hide"), msc.calendar.synchronized) {
                 const n = msc.calendar.updating;
                 if (!(-1 < n.indexOf(a.view.calendar))) {
                     n.push(a.view.calendar);
                     var e = $(".calendar");
                     try {
                         e.each((e, t) => {
                             t = $(t).data("msc-calendar");
@@ -113,110 +118,111 @@
                 }
             }
         },
         addEvent: e => {
             const t = e.jsEvent.target,
                 a = $(t).parents(".calendar"),
                 n = a.data("msc-room");
-            "True" === a.data("msc-editable") && MyAMS.require("modal").then(() => {
+            $(".tooltip").tooltip("hide"), "True" === a.data("msc-editable") && MyAMS.require("modal").then(() => {
                 MyAMS.modal.open("add-session.html", {
                     start: e.dateStr,
                     room: n
                 })
             })
         },
         cloneEvent: (e, t) => () => {
-            MyAMS.require("ajax").then(() => {
+            $(".tooltip").tooltip("hide"), MyAMS.require("ajax").then(() => {
                 var e = t.data("msc-event");
                 MyAMS.ajax.post(e.extendedProps.href + "/clone-event.json").then(e => {
                     "success" === e.status && MyAMS.msc.calendar.refresh(e.event.room)
                 })
             })
         },
         addEventCallback: (e, t) => {
             t = t.event.room;
-            MyAMS.msc.calendar.refresh(t)
+            $(".tooltip").tooltip("hide"), MyAMS.msc.calendar.refresh(t)
         },
         showEvent: e => {
-            e = e.event;
-            if (e.extendedProps?.visible) {
-                const t = e.extendedProps?.href;
-                t && MyAMS.require("modal").then(() => {
-                    MyAMS.modal.open(t + "/properties.html")
+            var e = e.event,
+                t = e.extendedProps?.visible;
+            if ($(".tooltip").tooltip("hide"), t) {
+                const a = e.extendedProps?.href;
+                a && MyAMS.require("modal").then(() => {
+                    MyAMS.modal.open(a + "/properties.html")
                 })
             }
         },
         editEventCallback: (e, t) => {
             const n = t.event,
                 r = n.room.toString(),
                 a = $(".calendar");
-            a.each((e, t) => {
+            $(".tooltip").tooltip("hide"), a.each((e, t) => {
                 var t = $(t),
                     a = t.data("msc-room").toString(),
                     t = t.data("msc-calendar");
                 a === r ? t.refetchEvents() : (a = t.getEventById(n.id)) && a.remove()
             })
         },
-        dropEvent: r => new Promise((t, e) => {
+        dropEvent: r => ($(".tooltip").tooltip("hide"), new Promise((t, e) => {
             const a = r.event,
                 n = a.extendedProps?.href;
             n ? MyAMS.require("ajax").then(() => {
                 MyAMS.ajax.post(n + "/update-event.json", {
                     room: a.extendedProps.room.toString(),
                     start: a.startStr,
                     end: a.endStr
                 }).then(e => {
                     t(e)
                 }, () => {
                     r.revert(), e()
                 })
             }) : (r.revert(), e())
-        }),
-        resizeEvent: r => new Promise((t, e) => {
+        })),
+        resizeEvent: r => ($(".tooltip").tooltip("hide"), new Promise((t, e) => {
             const a = r.event,
                 n = a.extendedProps?.href;
             n ? MyAMS.require("ajax").then(() => {
                 MyAMS.ajax.post(n + "/update-event.json", {
                     room: a.extendedProps.room.toString(),
                     start: a.startStr,
                     end: a.endStr
                 }).then(e => {
                     t(e)
                 }, () => {
                     r.revert(), e()
                 })
             }) : (r.revert(), e())
-        }),
-        receiveEvent: l => new Promise((t, e) => {
-            const a = l.event,
+        })),
+        receiveEvent: i => ($(".tooltip").tooltip("hide"), new Promise((t, e) => {
+            const a = i.event,
                 n = a.extendedProps?.href;
             if (n) {
-                const r = $(l.view.calendar.el),
+                const r = $(i.view.calendar.el),
                     s = r.data("msc-calendar"),
                     o = r.data("msc-room"),
                     d = a.extendedProps?.room,
-                    c = $(`.calendar[data-msc-room="${d}"]`).data("msc-calendar");
+                    l = $(`.calendar[data-msc-room="${d}"]`).data("msc-calendar");
                 MyAMS.require("ajax").then(() => {
                     MyAMS.ajax.post(n + "/update-event.json", {
                         room: o.toString(),
                         start: a.startStr,
                         end: a.endStr
                     }).then(e => {
-                        l.revert(), c.refetchEvents(), s.refetchEvents(), e.messagebox ? MyAMS.require("alert").then(() => {
+                        i.revert(), l.refetchEvents(), s.refetchEvents(), e.messagebox ? MyAMS.require("alert").then(() => {
                             MyAMS.alert.messageBox(e.messagebox), t(e)
                         }) : t(e)
                     }, () => {
-                        l.revert(), c.refetchEvents(), s.refetchEvents(), e()
+                        i.revert(), l.refetchEvents(), s.refetchEvents(), e()
                     })
                 })
-            } else l.revert(), e()
-        }),
+            } else i.revert(), e()
+        })),
         deleteEventCallback: (e, t) => {
             t = $(`.calendar[data-msc-room="${t.room}"]`).data("msc-calendar").getEventById(t.event_id);
-            t && t.remove()
+            $(".tooltip").tooltip("hide"), t && t.remove()
         },
         manageEventBookings: (e, t) => () => {
             const e = t.data("msc-event");
             MyAMS.require("modal").then(() => {
                 MyAMS.modal.open(e.extendedProps.href + "/bookings.html")
             })
         }
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/SOURCES.txt` & `pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -131,14 +131,17 @@
 src/pyams_app_msc/component/contact/interfaces.py
 src/pyams_app_msc/component/contact/zmi/__init__.py
 src/pyams_app_msc/component/duration/__init__.py
 src/pyams_app_msc/component/duration/interfaces.py
 src/pyams_app_msc/component/duration/schema.py
 src/pyams_app_msc/component/duration/zmi/__init__.py
 src/pyams_app_msc/component/duration/zmi/interfaces.py
+src/pyams_app_msc/component/paragraph/__init__.py
+src/pyams_app_msc/component/paragraph/zmi/__init__.py
+src/pyams_app_msc/component/paragraph/zmi/container.py
 src/pyams_app_msc/doctests/README.rst
 src/pyams_app_msc/feature/__init__.py
 src/pyams_app_msc/feature/booking/__init__.py
 src/pyams_app_msc/feature/booking/container.py
 src/pyams_app_msc/feature/booking/interfaces.py
 src/pyams_app_msc/feature/booking/reminder.py
 src/pyams_app_msc/feature/booking/task.py
@@ -189,14 +192,18 @@
 src/pyams_app_msc/feature/tmdb/zmi/__init__.py
 src/pyams_app_msc/feature/tmdb/zmi/lookup.py
 src/pyams_app_msc/generations/__init__.py
 src/pyams_app_msc/locales/pyams_app_msc.pot
 src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo
 src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po
 src/pyams_app_msc/reference/__init__.py
+src/pyams_app_msc/reference/structure/__init__.py
+src/pyams_app_msc/reference/structure/interfaces.py
+src/pyams_app_msc/reference/structure/zmi/__init__.py
+src/pyams_app_msc/reference/structure/zmi/table.py
 src/pyams_app_msc/reference/zmi/__init__.py
 src/pyams_app_msc/reference/zmi/viewlet.py
 src/pyams_app_msc/root/__init__.py
 src/pyams_app_msc/root/interfaces.py
 src/pyams_app_msc/root/zmi/__init__.py
 src/pyams_app_msc/shared/__init__.py
 src/pyams_app_msc/shared/catalog/__init__.py
@@ -278,9 +285,10 @@
 src/pyams_app_msc/skin/resources/src/sass/_variables.scss
 src/pyams_app_msc/skin/resources/src/sass/msc.scss
 src/pyams_app_msc/skin/templates/select-admin-theater.pt
 src/pyams_app_msc/tests/__init__.py
 src/pyams_app_msc/tests/test_utilsdocs.py
 src/pyams_app_msc/tests/test_utilsdocstrings.py
 src/pyams_app_msc/zmi/__init__.py
+src/pyams_app_msc/zmi/resources/img/pass-culture.webp
 src/pyams_app_msc/zmi/resources/js/msc.js
 src/pyams_app_msc/zmi/resources/js/msc.min.js
```

### Comparing `pyams_app_msc-1.99.1/src/pyams_app_msc.egg-info/requires.txt` & `pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/requires.txt`

 * *Files identical despite different names*

