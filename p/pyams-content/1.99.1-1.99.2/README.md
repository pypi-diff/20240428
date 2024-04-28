# Comparing `tmp/pyams_content-1.99.1.tar.gz` & `tmp/pyams_content-1.99.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_content-1.99.1.tar", last modified: Tue Apr  9 20:48:29 2024, max compression
+gzip compressed data, was "dist/pyams_content-1.99.2.tar", last modified: Sun Apr 28 15:31:16 2024, max compression
```

## Comparing `pyams_content-1.99.1.tar` & `pyams_content-1.99.2.tar`

### file list

```diff
@@ -1,659 +1,659 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-26 23:15:27.000000 pyams_content-1.99.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-26 23:15:27.000000 pyams_content-1.99.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2079 2024-04-09 20:48:29.000000 pyams_content-1.99.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/docs/
--rwxrwxrwx   0 root         (0) root         (0)      246 2024-04-09 20:44:10.000000 pyams_content-1.99.1/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-02-26 23:15:27.000000 pyams_content-1.99.1/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 20:48:29.000000 pyams_content-1.99.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3377 2024-04-09 20:44:10.000000 pyams_content-1.99.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/association/
--rw-rw-rw-   0 root         (0) root         (0)     3402 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4072 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/container.py
--rw-rw-rw-   0 root         (0) root         (0)     3230 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2091 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/association/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2162 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1514 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/skin/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/association/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/skin/templates/association-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1960 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/skin/templates/association-viewlet.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/association/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     5882 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8776 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2039 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/association/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/calendar/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/calendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/cards/
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/cards/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2619 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/cards/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/skin/templates/cards-masonry.pt
--rw-rw-rw-   0 root         (0) root         (0)     1773 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/skin/templates/cards.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/cards/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2094 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/cards/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/contact/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/component/contact/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/
--rw-rw-rw-   0 root         (0) root         (0)     7387 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4426 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     9775 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2467 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3254 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     2798 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/fields/
--rw-rw-rw-   0 root         (0) root         (0)      571 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3504 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5218 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/mail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2786 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/fields/handler/zmi/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/fields/skin/
--rw-rw-rw-   0 root         (0) root         (0)      576 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/skin/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/fields/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/skin/templates/form-submit.pt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/skin/templates/paragraph-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/fields/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2100 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/fields/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/file/
--rw-rw-rw-   0 root         (0) root         (0)     1583 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/file/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/frame/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/component/frame/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/frame/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/
--rw-rw-rw-   0 root         (0) root         (0)     6052 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4672 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/file.py
--rw-rw-rw-   0 root         (0) root         (0)     5094 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     1661 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4654 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2175 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt
--rw-rw-rw-   0 root         (0) root         (0)     2954 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1242 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/zmi/templates/gallery-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4053 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2120 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt
--rw-rw-rw-   0 root         (0) root         (0)     2891 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/gallery-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1185 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/gallery-random.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8399 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11894 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1995 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1498 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/
--rw-rw-rw-   0 root         (0) root         (0)     7780 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4725 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2005 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6710 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2989 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1390 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     2530 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1328 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/zmi/templates/illustration-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/
--rw-rw-rw-   0 root         (0) root         (0)     5098 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4472 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/illustration.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2087 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/illustration-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     2388 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/illustration-side.pt
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     5108 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5143 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/paragraph.py
--rw-rw-rw-   0 root         (0) root         (0)     1989 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/keynumber/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/keynumber/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/links/
--rw-rw-rw-   0 root         (0) root         (0)    10891 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/links/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4819 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/links/html.py
--rw-rw-rw-   0 root         (0) root         (0)     5037 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/links/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/links/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8653 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/links/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/links/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2658 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/links/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/map/
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/map/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/milestone/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/milestone/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/
--rw-rw-rw-   0 root         (0) root         (0)     6756 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5621 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/container.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     5077 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/interfaces/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     4693 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5340 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     7591 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4105 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      606 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/templates/navigation-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7323 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2456 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/interfaces/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      899 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/templates/html.pt
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/templates/raw-code.pt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/templates/raw.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    17744 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17906 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/helper.py
--rw-rw-rw-   0 root         (0) root         (0)     4263 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/html.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/templates/title-toolbar.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/pictogram/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/component/pictogram/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/
--rw-rw-rw-   0 root         (0) root         (0)     7603 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2699 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/skin/templates/tags.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    12144 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     6509 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/verbatim/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/component/verbatim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/
--rw-rw-rw-   0 root         (0) root         (0)     2307 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1971 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/provider/
--rw-rw-rw-   0 root         (0) root         (0)     2984 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/provider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3286 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/provider/dailymotion.py
--rw-rw-rw-   0 root         (0) root         (0)     9322 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/provider/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2895 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/provider/vimeo.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/provider/youtube.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2151 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/
--rw-rw-rw-   0 root         (0) root         (0)     2159 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1737 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/dailymotion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/templates/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/templates/custom-render.pt
--rw-rw-rw-   0 root         (0) root         (0)      450 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/templates/dailymotion-render.pt
--rw-rw-rw-   0 root         (0) root         (0)      542 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/templates/youtube-render.pt
--rw-rw-rw-   0 root         (0) root         (0)     1503 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/vimeo.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/youtube.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/skin/templates/video-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/component/video/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      574 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12014 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/component/video/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/doctests/
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/
--rw-rw-rw-   0 root         (0) root         (0)     3608 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2142 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1882 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/skin/templates/alerts.pt
--rw-rw-rw-   0 root         (0) root         (0)     1098 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/skin/templates/context-alerts.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2205 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/alert/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/audit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/feature/audit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/
--rw-rw-rw-   0 root         (0) root         (0)     2343 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6737 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1803 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/sitemap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      406 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/glossary-sitemap.pt
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/glossary.pt
--rw-rw-rw-   0 root         (0) root         (0)     1731 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-associations.pt
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-body.pt
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-footer.pt
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     3568 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/term.py
--rw-rw-rw-   0 root         (0) root         (0)     3180 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3093 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/glossary/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/history/
--rw-rw-rw-   0 root         (0) root         (0)     3000 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/history/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2286 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/history/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/history/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      574 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/history/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/history/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/history/zmi/templates/history.pt
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/history/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/html/
--rw-rw-rw-   0 root         (0) root         (0)     3125 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/html/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/
--rw-rw-rw-   0 root         (0) root         (0)     6800 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     3392 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3551 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2154 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1339 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3353 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1301 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7353 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/
--rw-rw-rw-   0 root         (0) root         (0)      570 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2670 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      738 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/qrcode/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/feature/qrcode/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/redirect/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/feature/redirect/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/renderer/
--rw-rw-rw-   0 root         (0) root         (0)     5451 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/renderer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/renderer/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/review/
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3253 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/chat.py
--rw-rw-rw-   0 root         (0) root         (0)     3206 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4664 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/review/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    11050 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/comment.pt
--rw-rw-rw-   0 root         (0) root         (0)     2784 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/comments.pt
--rw-rw-rw-   0 root         (0) root         (0)     1787 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/mail-notification.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/
--rw-rw-rw-   0 root         (0) root         (0)     3169 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7419 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3804 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/search/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     4825 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2527 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)    11035 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6230 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt
--rw-rw-rw-   0 root         (0) root         (0)     5146 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt
--rw-rw-rw-   0 root         (0) root         (0)     5176 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt
--rw-rw-rw-   0 root         (0) root         (0)     4985 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1187 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt
--rw-rw-rw-   0 root         (0) root         (0)     5184 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt
--rw-rw-rw-   0 root         (0) root         (0)     4002 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/zmi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1258 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      708 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     4276 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/search/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/search/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7625 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3101 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/search/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/zmi/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     3955 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/feature/search/zmi/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/share/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/feature/share/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/
--rw-rw-rw-   0 root         (0) root         (0)     4558 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      796 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/templates/
--rw-rw-rw-   0 root         (0) root         (0)      299 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/templates/humans.pt
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/templates/robots.pt
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/templates/root-sitemap.pt
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/feature/sitemap/templates/tool-sitemap.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/feature/toolbox/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/feature/toolbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/generations/
--rw-rw-rw-   0 root         (0) root         (0)    10545 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8956 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     4405 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)   124539 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo
--rw-rw-rw-   0 root         (0) root         (0)   223765 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po
--rw-rw-rw-   0 root         (0) root         (0)   161700 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/locales/pyams_content.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/
--rw-rw-rw-   0 root         (0) root         (0)     2851 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2917 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     6729 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3473 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/templates/pictogram-header.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/
--rw-rw-rw-   0 root         (0) root         (0)     2896 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2831 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/templates/
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/templates/selection-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     3174 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1938 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4333 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/reference/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/reference/zmi/viewlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/root/
--rw-rw-rw-   0 root         (0) root         (0)     4904 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/root/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6721 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/root/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4841 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/root/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/root/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3885 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/root/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25806 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/root/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)    13639 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/root/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     5338 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/root/zmi/sites.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/
--rw-rw-rw-   0 root         (0) root         (0)      561 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/
--rw-rw-rw-   0 root         (0) root         (0)     2969 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5270 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2824 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4288 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3268 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     9134 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/blog/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/blog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/calendar/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/calendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/
--rw-rw-rw-   0 root         (0) root         (0)    11763 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    15461 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/common/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5998 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/interfaces/types.py
--rw-rw-rw-   0 root         (0) root         (0)     3368 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2786 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2282 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/header.py
--rw-rw-rw-   0 root         (0) root         (0)     5197 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1762 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/specificities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2618 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/templates/specificities-default.pt
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/templates/title-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/title.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/specificities.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/title.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      658 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1386 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1435 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/specificities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      644 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/templates/specificities-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/templates/title-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     1369 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/title.py
--rw-rw-rw-   0 root         (0) root         (0)     9807 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/restrictions.py
--rw-rw-rw-   0 root         (0) root         (0)     3878 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/security.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2333 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/breadcrumb.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/oid.py
--rw-rw-rw-   0 root         (0) root         (0)     1765 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/specificities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      201 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/templates/breadcrumbs.pt
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/templates/card-datatype.pt
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/templates/publication-date.pt
--rw-rw-rw-   0 root         (0) root         (0)     1727 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/title.py
--rw-rw-rw-   0 root         (0) root         (0)     2556 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/types.py
--rw-rw-rw-   0 root         (0) root         (0)     4801 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/url.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/skin/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)    12425 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    23132 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14620 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/content.py
--rw-rw-rw-   0 root         (0) root         (0)    36824 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     3872 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4679 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    18561 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/owner.py
--rw-rw-rw-   0 root         (0) root         (0)     3030 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/portal.py
--rw-rw-rw-   0 root         (0) root         (0)     2899 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/reference.py
--rw-rw-rw-   0 root         (0) root         (0)    18640 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/restrictions.py
--rw-rw-rw-   0 root         (0) root         (0)    17565 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     8992 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/content-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/content-workflow.pt
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/owner-change.pt
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/quick-search.pt
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/sequence-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/
--rw-rw-rw-   0 root         (0) root         (0)     7226 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5005 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/container.py
--rw-rw-rw-   0 root         (0) root         (0)     2605 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/content.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)     3179 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29957 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/common/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/file/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/file/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/form/
--rw-rw-rw-   0 root         (0) root         (0)     2560 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/form/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/form/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/form/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/form/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2046 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/form/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/form/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2195 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/form/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/hub/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/hub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/logo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/shared/logo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/logo/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1149 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/logo/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/news/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/shared/news/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 20:47:51.000000 pyams_content-1.99.1/src/pyams_content/shared/resource/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/site/
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4564 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/container.py
--rw-rw-rw-   0 root         (0) root         (0)     5188 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     8784 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     7205 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/link.py
--rw-rw-rw-   0 root         (0) root         (0)     5429 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8526 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/folder.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    15922 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/link.py
--rw-rw-rw-   0 root         (0) root         (0)     8144 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5391 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/rename.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     5002 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/topic.py
--rw-rw-rw-   0 root         (0) root         (0)    21405 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)     1899 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/viewlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/templates/
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/topic/
--rw-rw-rw-   0 root         (0) root         (0)     2195 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/topic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/topic/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/topic/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/topic/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1737 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/topic/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/
--rw-rw-rw-   0 root         (0) root         (0)     8677 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     7663 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/query.py
--rw-rw-rw-   0 root         (0) root         (0)     5853 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1486 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     6223 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/merge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     4700 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5886 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6787 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt
--rw-rw-rw-   0 root         (0) root         (0)     2969 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt
--rw-rw-rw-   0 root         (0) root         (0)     2449 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt
--rw-rw-rw-   0 root         (0) root         (0)     2666 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/zmi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     6586 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/query.py
--rw-rw-rw-   0 root         (0) root         (0)     6661 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/reference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1398 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/skin/templates/preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     7845 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/shared/view/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4191 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/shared/view/zmi/references.py
--rw-rw-rw-   0 root         (0) root         (0)     6188 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/shared/view/zmi/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/skin/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2024-04-09 20:44:10.000000 pyams_content-1.99.1/src/pyams_content/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/tests/
--rw-rw-rw-   0 root         (0) root         (0)      802 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/workflow/
--rw-rw-rw-   0 root         (0) root         (0)    43555 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21211 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/basic.py
--rw-rw-rw-   0 root         (0) root         (0)     1227 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4984 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/notify.py
--rw-rw-rw-   0 root         (0) root         (0)     6272 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/workflow/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3222 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/zmi/publication.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/zmi/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/workflow/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/workflow/zmi/templates/publication-header.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      777 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7680 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     2383 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/html.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/properties.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    19424 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/content.js
--rw-rw-rw-   0 root         (0) root         (0)    10283 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/content.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/headers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/headers/langs/
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/headers/langs/fr.js
--rw-rw-rw-   0 root         (0) root         (0)     2115 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/internal-link/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js
--rw-rw-rw-   0 root         (0) root         (0)     5919 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/viewlet/toplinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/widget/
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/widget/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/widget/seo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content/zmi/widget/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1260 2024-02-26 23:15:27.000000 pyams_content-1.99.1/src/pyams_content/zmi/widget/templates/seo-textline-input.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2079 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24617 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:48:17.000000 pyams_content-1.99.1/src/pyams_content.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-09 20:48:29.000000 pyams_content-1.99.1/src/pyams_content.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-26 23:15:27.000000 pyams_content-1.99.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-26 23:15:27.000000 pyams_content-1.99.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2488 2024-04-28 15:31:16.000000 pyams_content-1.99.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      655 2024-04-28 15:24:34.000000 pyams_content-1.99.2/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-02-26 23:15:27.000000 pyams_content-1.99.2/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 15:31:16.000000 pyams_content-1.99.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3377 2024-04-28 15:24:34.000000 pyams_content-1.99.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/
+-rw-rw-rw-   0 root         (0) root         (0)      865 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/association/
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4072 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3230 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/association/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1514 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/skin/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/association/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/skin/templates/association-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1960 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/skin/templates/association-viewlet.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/association/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5882 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9011 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/association/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2039 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/calendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/cards/
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/cards/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/cards/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/skin/templates/cards-masonry.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1773 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/skin/templates/cards.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/cards/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/contact/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/component/contact/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/
+-rw-rw-rw-   0 root         (0) root         (0)     7387 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     9775 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3254 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2798 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/fields/
+-rw-rw-rw-   0 root         (0) root         (0)      571 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3504 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     5218 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/mail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/zmi/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/fields/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/skin/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/fields/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/skin/templates/form-submit.pt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/skin/templates/paragraph-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/fields/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/file/
+-rw-rw-rw-   0 root         (0) root         (0)     1583 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/file/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/frame/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/component/frame/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/frame/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4672 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5095 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1661 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2954 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/zmi/templates/gallery-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4053 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2891 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/gallery-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/gallery-random.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8399 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11894 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1995 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/
+-rw-rw-rw-   0 root         (0) root         (0)     7780 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2005 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6710 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2989 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1390 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/zmi/templates/illustration-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6234 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/illustration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/illustration-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/illustration-side.pt
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5108 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5143 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/paragraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     1989 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/keynumber/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/keynumber/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/links/
+-rw-rw-rw-   0 root         (0) root         (0)    10891 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/links/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4819 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/links/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     5037 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/links/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/links/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8653 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/links/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/links/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2658 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/links/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/map/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/map/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/milestone/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/milestone/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/
+-rw-rw-rw-   0 root         (0) root         (0)     6756 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5966 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     5173 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/interfaces/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     4693 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5340 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     7591 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/templates/navigation-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7323 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/interfaces/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      899 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/templates/html.pt
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/templates/raw-code.pt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/templates/raw.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    17744 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17906 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4263 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/templates/title-toolbar.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/pictogram/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/component/pictogram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/
+-rw-rw-rw-   0 root         (0) root         (0)     7603 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2699 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/skin/templates/tags.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12144 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     6509 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/verbatim/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/component/verbatim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/
+-rw-rw-rw-   0 root         (0) root         (0)     2307 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1971 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/provider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3286 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/provider/dailymotion.py
+-rw-rw-rw-   0 root         (0) root         (0)     9322 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/provider/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2895 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/provider/vimeo.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/provider/youtube.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2159 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/dailymotion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/templates/custom-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)      450 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/templates/dailymotion-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)      542 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/templates/youtube-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/vimeo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/youtube.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/templates/video-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12014 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/
+-rw-rw-rw-   0 root         (0) root         (0)     3608 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2142 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/skin/templates/alerts.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/skin/templates/context-alerts.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/audit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/feature/audit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6737 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1803 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/sitemap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/glossary-sitemap.pt
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/glossary.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-associations.pt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-body.pt
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-footer.pt
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3568 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     3180 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/history/
+-rw-rw-rw-   0 root         (0) root         (0)     3000 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/history/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2286 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/history/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/history/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/history/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/history/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/history/zmi/templates/history.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/history/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/html/
+-rw-rw-rw-   0 root         (0) root         (0)     3125 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/html/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/
+-rw-rw-rw-   0 root         (0) root         (0)     6800 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4435 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     3392 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3551 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3353 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      553 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7344 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/
+-rw-rw-rw-   0 root         (0) root         (0)      570 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2670 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      738 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/qrcode/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/feature/qrcode/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/redirect/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/feature/redirect/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/renderer/
+-rw-rw-rw-   0 root         (0) root         (0)     5451 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/renderer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/renderer/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/review/
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3253 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/chat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3206 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4664 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/review/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    11045 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/feature/review/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/comment.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2784 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/comments.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/mail-notification.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/
+-rw-rw-rw-   0 root         (0) root         (0)     3169 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7419 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3804 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/search/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     4861 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2527 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)    11035 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6230 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt
+-rw-rw-rw-   0 root         (0) root         (0)     5146 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt
+-rw-rw-rw-   0 root         (0) root         (0)     5176 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4985 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt
+-rw-rw-rw-   0 root         (0) root         (0)     5184 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4002 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/zmi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4276 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/search/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7625 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/search/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/zmi/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/zmi/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/share/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/feature/share/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/
+-rw-rw-rw-   0 root         (0) root         (0)     4558 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/templates/humans.pt
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/templates/robots.pt
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/templates/root-sitemap.pt
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/templates/tool-sitemap.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/toolbox/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/feature/toolbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/generations/
+-rw-rw-rw-   0 root         (0) root         (0)    10545 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9656 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     4659 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)   124893 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo
+-rw-rw-rw-   0 root         (0) root         (0)   224270 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po
+-rw-rw-rw-   0 root         (0) root         (0)   162061 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/locales/pyams_content.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     4561 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/reference/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/reference/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2917 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     6747 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3851 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/templates/pictogram-header.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/templates/selection-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3174 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4440 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/reference/zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/zmi/viewlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/root/
+-rw-rw-rw-   0 root         (0) root         (0)     4904 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/root/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6721 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/root/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4841 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/root/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/root/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3885 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/root/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25806 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/root/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13639 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/root/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     5338 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/root/zmi/sites.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/
+-rw-rw-rw-   0 root         (0) root         (0)      561 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5270 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2824 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4288 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3268 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     9134 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/blog/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/blog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/calendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/
+-rw-rw-rw-   0 root         (0) root         (0)    11763 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    15461 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/common/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5998 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/interfaces/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3368 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2282 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     5197 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/specificities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/templates/specificities-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/templates/title-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/title.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/specificities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/title.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1435 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/specificities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/templates/specificities-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/templates/title-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/title.py
+-rw-rw-rw-   0 root         (0) root         (0)     9807 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3877 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/shared/common/security.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2333 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/breadcrumb.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/oid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/specificities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/templates/breadcrumbs.pt
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/templates/card-datatype.pt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/templates/publication-date.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/title.py
+-rw-rw-rw-   0 root         (0) root         (0)     2556 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     4801 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    12425 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    23132 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14620 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/content.py
+-rw-rw-rw-   0 root         (0) root         (0)    36824 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3872 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4679 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    18561 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/owner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3030 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/portal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2899 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)    18640 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17565 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     8992 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/content-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/content-workflow.pt
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/owner-change.pt
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/quick-search.pt
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/sequence-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/
+-rw-rw-rw-   0 root         (0) root         (0)     7226 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5005 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     2605 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/content.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)     3179 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29957 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/file/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/file/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/form/
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/form/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/form/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/form/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/form/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/form/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/form/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/form/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/hub/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/hub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/logo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/shared/logo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/logo/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1149 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/logo/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/news/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/shared/news/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/shared/resource/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/site/
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     5188 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8784 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     7205 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     5429 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8526 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    15922 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     8144 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5391 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/rename.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/topic.py
+-rw-rw-rw-   0 root         (0) root         (0)    21405 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/viewlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/topic/
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/topic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/topic/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/topic/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/topic/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/topic/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/
+-rw-rw-rw-   0 root         (0) root         (0)     8677 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     7663 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     5853 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     6223 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/merge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     4700 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5886 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6787 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/zmi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     6586 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     6661 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/skin/templates/preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     7845 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4191 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/zmi/references.py
+-rw-rw-rw-   0 root         (0) root         (0)     6188 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/zmi/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/workflow/
+-rw-rw-rw-   0 root         (0) root         (0)    43555 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21211 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/basic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4984 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/notify.py
+-rw-rw-rw-   0 root         (0) root         (0)     6272 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/workflow/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/zmi/publication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/zmi/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/workflow/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/zmi/templates/publication-header.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      777 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7680 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2383 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/properties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    19424 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/content.js
+-rw-rw-rw-   0 root         (0) root         (0)    10283 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/content.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/headers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/headers/langs/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/headers/langs/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/internal-link/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/viewlet/toplinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/widget/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/widget/seo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/widget/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/widget/templates/seo-textline-input.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2488 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24617 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:31:04.000000 pyams_content-1.99.2/src/pyams_content.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/top_level.txt
```

### Comparing `pyams_content-1.99.1/LICENSE` & `pyams_content-1.99.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/PKG-INFO` & `pyams_content-1.99.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_content
-Version: 1.99.1
+Version: 1.99.2
 Summary: PyAMS content management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS CMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -48,14 +48,24 @@
 Please note that PyAMS_content only provide a basic Bootstrap based skin, so you will have to
 include other extension packages (like PyAMS_content_themes) to get more advanced graphical themes.
 
 
 Changelog
 =========
 
+1.99.2
+------
+ - added permission and role to manage references tables
+ - disable cache when using aggregated search results portlet renderer
+ - always open switcher in associations paragraph
+ - added method to paragraphs container to get iterator over paragraphs matching a given set of factories
+ - removed required flag on gallery files author
+ - updated menus order
+ - formatting and other minor updates
+
 1.99.1
 ------
  - added edit forms content getters
  - added alerts types
  - added vocabulary to handle shared contents which can be used by views and search folders
  - minor updates
```

### Comparing `pyams_content-1.99.1/docs/README.rst` & `pyams_content-1.99.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/setup.py` & `pyams_content-1.99.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.99.1'
+version = '1.99.2'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_security_views',
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
```

### Comparing `pyams_content-1.99.1/src/pyams_content/__init__.py` & `pyams_content-1.99.2/src/pyams_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/association/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/association/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/association/container.py` & `pyams_content-1.99.2/src/pyams_content/component/association/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/association/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/association/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/association/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/association/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/association/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/association/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/association/skin/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/association/skin/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/association/skin/templates/association-viewlet.pt` & `pyams_content-1.99.2/src/pyams_content/component/association/skin/templates/association-viewlet.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/association/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/association/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/association/zmi/container.py` & `pyams_content-1.99.2/src/pyams_content/component/association/zmi/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 This module provides a few components used for management of associations containers.
 """
 
 from pyramid.view import view_config
 from zope.interface import implementer
 
 from pyams_content.component.association import IAssociationContainer, IAssociationContainerTarget
-from pyams_content.component.association.interfaces import IAssociationInfo
+from pyams_content.component.association.interfaces import IAssociationInfo, IAssociationParagraph
 from pyams_content.component.association.zmi import IAssociationsTable
 from pyams_content.component.association.zmi.interfaces import IAssociationsContainerEditForm
 from pyams_content.component.paragraph.zmi.helper import get_json_paragraph_toolbar_refresh_event
 from pyams_content.shared.common.interfaces.types import ITypedSharedTool
 from pyams_content.shared.common.zmi.types import ISharedToolTypesTable
 from pyams_form.ajax import ajax_form_config
 from pyams_form.interfaces.form import IInnerSubForm
@@ -248,7 +248,14 @@
 
     legend = _("Links and external files")
 
     table_class = IAssociationsTable
     container_intf = IAssociationContainer
 
     weight = 20
+
+    @property
+    def state(self):
+        """Always open switcher in associations paragraphs"""
+        if IAssociationParagraph.providedBy(self.context):
+            return 'open'
+        return super().state
```

### Comparing `pyams_content-1.99.1/src/pyams_content/component/association/zmi/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/association/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/association/zmi/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/association/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/calendar/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/cards/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/cards/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/cards/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/cards/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/cards/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/cards/skin/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/cards/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/cards/skin/templates/cards-masonry.pt` & `pyams_content-1.99.2/src/pyams_content/component/cards/skin/templates/cards-masonry.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/cards/skin/templates/cards.pt` & `pyams_content-1.99.2/src/pyams_content/component/cards/skin/templates/cards.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/cards/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/cards/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/extfile/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/extfile/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/extfile/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/extfile/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/extfile/manager.py` & `pyams_content-1.99.2/src/pyams_content/component/extfile/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/manager.py` & `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt` & `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt` & `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/extfile/zmi/widget.py` & `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/fields/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/fields/handler/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/fields/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/fields/handler/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/fields/handler/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/fields/handler/mail.py` & `pyams_content-1.99.2/src/pyams_content/component/fields/handler/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/fields/handler/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/fields/handler/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/fields/handler/zmi/mail.py` & `pyams_content-1.99.2/src/pyams_content/component/fields/handler/zmi/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/fields/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/fields/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/fields/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/fields/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/fields/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/fields/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/fields/skin/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/fields/skin/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/fields/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/fields/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/fields/zmi/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/fields/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/file/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/file/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/frame/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/frame/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/file.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/file.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     description = I18nTextField(title=_("Associated text"),
                                 description=_("Media description can be displayed in "
                                               "front-office templates"),
                                 required=False)
 
     author = TextLine(title=_("Author"),
                       description=_("Name of media's author"),
-                      required=True)
+                      required=False)
 
     sound = AudioField(title=_("Audio data"),
                        description=_("Sound file associated with the current media"),
                        required=False)
 
     sound_title = I18nTextLineField(title=_("Sound title"),
                                     description=_("Title of associated sound file"),
```

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt` & `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt` & `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt` & `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/portlet/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/skin/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt` & `pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/gallery-default.pt` & `pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/gallery-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/skin/templates/gallery-random.pt` & `pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/gallery-random.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/file.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/file.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/helpers.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/helpers.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/interfaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,12 +35,12 @@
     medias_data = FileField(title=_("Images or videos data"),
                             description=_("You can upload a single file, or choose to upload "
                                           "a whole ZIP archive"),
                             required=True)
 
     author = TextLine(title=_("Author"),
                       description=_("Name of document's author"),
-                      required=True)
+                      required=False)
 
 
 class IGalleryMediaThumbnailView(Interface):
     """Gallery media thumbnail view marker interface"""
```

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt` & `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt` & `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt` & `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt` & `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt` & `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/portlet/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,93 +14,130 @@
 
 This module provides base illustrations adapters.
 """
 
 from zope.interface import Interface
 
 from pyams_content.component.illustration import IBaseIllustrationTarget, IIllustration, \
-    ILinkIllustration, ILinkIllustrationTarget
+    IIllustrationTargetBase, ILinkIllustration, ILinkIllustrationTarget
 from pyams_content.component.links import IInternalLink
 from pyams_content.interfaces import IBaseContent
 from pyams_content.shared.common import ISharedContent
-from pyams_content.skin.interfaces import IContentBannerIllustration, IContentNavigationIllustration
+from pyams_content.skin.interfaces import IContentBannerIllustration, IContentIllustration, \
+    IContentNavigationIllustration
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_portal.interfaces import HIDDEN_RENDERER_NAME
 from pyams_site.interfaces import ISiteRoot
 from pyams_utils.adapter import ContextRequestViewAdapter, adapter_config
 from pyams_utils.interfaces.tales import ITALESExtension
 
 
 #
 # Illustrations adapters
 #
 
-@adapter_config(required=(IInternalLink, IPyAMSLayer),
-                provides=IContentNavigationIllustration)
+@adapter_config(required=(IIllustrationTargetBase, IPyAMSLayer),
+                provides=IContentIllustration)
+def base_content_illustration(context, request):
+    """Base content illustration adapter"""
+    illustration = IIllustration(context, None)
+    if illustration and illustration.has_data():
+        return illustration
+    return None
+
+
+@adapter_config(name='pyams_illustration',
+                required=(Interface, Interface, Interface),
+                provides=ITALESExtension)
+class PyAMSIllustrationTALESExtension(ContextRequestViewAdapter):
+    """PyAMS illustration TALES extension"""
+
+    def render(self, context=None, name=''):
+        if context is None:
+            context = self.context
+        return self.request.registry.queryMultiAdapter((context, self.request),
+                                                       IContentIllustration,
+                                                       name=name)
+
+
+#
+# Navigation illustration adapters
+#
+
 @adapter_config(required=(IBaseIllustrationTarget, IPyAMSLayer),
                 provides=IContentNavigationIllustration)
-def base_content_navigation_illustration_factory(context, request):
+def base_content_navigation_illustration(context, request):
     """Default content navigation illustration adapter"""
     illustration = ILinkIllustration(context, None)
     if not (illustration and illustration.has_data()):
         illustration = IIllustration(context, None)
         if IIllustration.providedBy(illustration) and \
                 (illustration.renderer == HIDDEN_RENDERER_NAME):
             illustration = None
     if illustration and illustration.has_data():
         return illustration
-    if IInternalLink.providedBy(context):
-        target = context.get_target()
-        if target is not None:
-            illustration = request.registry.queryMultiAdapter((target, request),
-                                                              IContentNavigationIllustration)
-            if illustration and illustration.has_data():
-                return illustration
+    return None
+
+
+@adapter_config(required=(IInternalLink, IPyAMSLayer),
+                provides=IContentNavigationIllustration)
+def internal_link_navigation_illustration(context, request):
+    """Internal link navigation illustration adapter"""
+    target = context.get_target()
+    if target is not None:
+        illustration = request.registry.queryMultiAdapter((target, request),
+                                                          IContentNavigationIllustration)
+        if illustration and illustration.has_data():
+            return illustration
     return None
 
 
 @adapter_config(required=(ILinkIllustrationTarget, IPyAMSLayer),
                 provides=IContentNavigationIllustration)
-def link_content_navigation_illustration_factory(context, request):
+def link_content_navigation_illustration(context, request):
     """Content navigation illustration adapter for basic link illustration targets"""
     illustration = ILinkIllustration(context, None)
     if illustration and illustration.has_data():
         return illustration
 
 
 @adapter_config(required=(ISharedContent, IPyAMSLayer),
                 provides=IContentNavigationIllustration)
-def shared_content_illustration_factory(context, request):
+def shared_content_navigation_illustration(context, request):
     """Shared content illustration factory"""
     version = context.visible_version
     if version is not None:
         return request.registry.queryMultiAdapter((version, request),
                                                   IContentNavigationIllustration)
     return None
 
 
-@adapter_config(name='pyams_illustration',
+@adapter_config(name='pyams_navigation_illustration',
                 required=(Interface, Interface, Interface),
                 provides=ITALESExtension)
-class PyAMSIllustrationTALESExtension(ContextRequestViewAdapter):
+class PyAMSNavigationIllustrationTALESExtension(ContextRequestViewAdapter):
     """PyAMS navigation illustration TALES extension"""
 
     def render(self, context=None, name=''):
         if context is None:
             context = self.context
         return self.request.registry.queryMultiAdapter((context, self.request),
                                                        IContentNavigationIllustration,
                                                        name=name)
 
 
+#
+# Banner illustration adapters
+#
+
 @adapter_config(required=(ISiteRoot, IPyAMSLayer),
                 provides=IContentBannerIllustration)
 @adapter_config(context=(IBaseContent, IPyAMSLayer),
                 provides=IContentBannerIllustration)
-def base_content_banner_illustration_factory(context, request):
+def base_content_banner_illustration(context, request):
     """Base content banner illustration adapter"""
     illustration = IIllustration(context, None)
     if illustration and illustration.has_data() and (illustration.renderer != HIDDEN_RENDERER_NAME):
         return illustration
     return None
```

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/illustration.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/illustration.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/illustration-default.pt` & `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/illustration-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/illustration-side.pt` & `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/illustration-side.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt` & `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/thesaurus.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/illustration/zmi/thesaurus.py` & `pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/keynumber/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/keynumber/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/links/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/links/html.py` & `pyams_content-1.99.2/src/pyams_content/component/links/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/links/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/links/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/links/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/links/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/links/zmi/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/links/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/links/zmi/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/links/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/map/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/map/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/milestone/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/milestone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/container.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,24 @@
 __docformat__ = 'restructuredtext'
 
 
 @factory_config(IParagraphContainer)
 class ParagraphContainer(BTreeOrderedContainer):
     """Paragraph container persistent class"""
 
+    def get_paragraphs(self, factories):
+        """Get paragraphs matching given factories"""
+        if not isinstance(factories, (list, tuple, set)):
+            factories = {factories}
+        yield from (
+            paragraph
+            for paragraph in self.values()
+            if paragraph.factory_name in (factories or ())
+        )
+
     def get_visible_paragraphs(self, names=None, anchors_only=False, exclude_anchors=False,
                                factories=None, limit=None):
         """Visible paragraphs getter"""
         count = 0
         if names:
             for name in names:
                 paragraph = self.get(name)
```

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/html.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/interfaces/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/interfaces/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,17 @@
     """Paragraphs container"""
 
     contains(IBaseParagraph)
 
     def append(self, value):
         """Add given value to container"""
 
+    def get_paragraphs(self, factories):
+        """Get paragraphs matching given factories"""
+
     def get_visible_paragraphs(self, names=None, anchors_only=False, exclude_anchors=False,
                                factories=None, limit=None):
         """Get visible paragraphs matching given arguments"""
 
 
 CONTENT_PARAGRAPHS_VOCABULARY = 'pyams_content.paragraphs'
```

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/interfaces/html.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/interfaces/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/settings.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/settings.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/html.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/interfaces/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/interfaces/html.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/interfaces/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/skin/templates/html.pt` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/templates/html.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 __docformat__ = 'restructuredtext'
 
 from pyams_content import _
 
 
 @viewlet_config(name='paragraph-types.menu',
                 context=IParagraphFactorySettingsTarget, layer=IAdminLayer,
-                manager=IPropertiesMenu, weight=610,
+                manager=IPropertiesMenu, weight=400,
                 permission=MANAGE_TOOL_PERMISSION)
 class ParagraphFactorySettingsMenu(NavigationMenuItem):
     """Paragraph factory settings menu"""
 
     label = _("Paragraphs types")
     href = '#paragraph-types.html'
```

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/container.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/helper.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/helper.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/html.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/paragraph/zmi/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/thesaurus/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/thesaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/thesaurus/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/thesaurus/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/thesaurus/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/thesaurus/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/thesaurus/zmi/manager.py` & `pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/video/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/video/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/video/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/provider/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/video/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/provider/dailymotion.py` & `pyams_content-1.99.2/src/pyams_content/component/video/provider/dailymotion.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/provider/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/video/provider/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/provider/vimeo.py` & `pyams_content-1.99.2/src/pyams_content/component/video/provider/vimeo.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/provider/youtube.py` & `pyams_content-1.99.2/src/pyams_content/component/video/provider/youtube.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/video/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/skin/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/component/video/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/dailymotion.py` & `pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/dailymotion.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt` & `pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/vimeo.py` & `pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/vimeo.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/skin/provider/youtube.py` & `pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/youtube.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/skin/templates/video-default.pt` & `pyams_content-1.99.2/src/pyams_content/component/video/skin/templates/video-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/component/video/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/component/video/zmi/paragraph.py` & `pyams_content-1.99.2/src/pyams_content/component/video/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/doctests/README.rst` & `pyams_content-1.99.2/src/pyams_content/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/alert/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/alert/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/alert/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/alert/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/alert/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/alert/skin/templates/alerts.pt` & `pyams_content-1.99.2/src/pyams_content/feature/alert/skin/templates/alerts.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/alert/skin/templates/context-alerts.pt` & `pyams_content-1.99.2/src/pyams_content/feature/alert/skin/templates/context-alerts.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/alert/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/alert/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/glossary/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/glossary/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/glossary/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/glossary/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/sitemap.py` & `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/sitemap.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt` & `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/glossary.pt` & `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/glossary.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-associations.pt` & `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-associations.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt` & `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/glossary/skin/term.py` & `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/term.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/glossary/task.py` & `pyams_content-1.99.2/src/pyams_content/feature/glossary/task.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/glossary/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/glossary/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/history/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/history/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/history/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/history/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/history/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/history/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/history/zmi/viewlet.py` & `pyams_content-1.99.2/src/pyams_content/feature/history/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/html/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/html/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,16 +177,15 @@
 @adapter_config(required=(IMenu, IAdminLayer, IPropertiesEditForm),
                 provides=IFormTitle)
 def menu_edit_form_title(context, request, view):
     """Menu properties edit form title getter"""
     parent = get_parent(context, IMenusContainerTarget)
     hint = get_object_hint(parent, request, view)
     label = get_object_label(parent, request, view)
-    return TITLE_SPAN_BREAK.format(
-        hint, label)
+    return TITLE_SPAN_BREAK.format(hint, label)
 
 
 @adapter_config(required=(IMenu, IAdminLayer, MenuPropertiesEditForm),
                 provides=IAJAXFormRenderer)
 class MenuEditFormRenderer(ContextRequestViewAdapter):
     """Menu edit form renderer"""
```

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/container.py` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/navigation/zmi/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/preview/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/preview/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/preview/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/preview/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/preview/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt` & `pyams_content-1.99.2/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/renderer/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/renderer/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/renderer/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/review/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/review/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/review/chat.py` & `pyams_content-1.99.2/src/pyams_content/feature/review/chat.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/review/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/review/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/review/manager.py` & `pyams_content-1.99.2/src/pyams_content/feature/review/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/review/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/review/zmi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         return get_age(comment.creation_date)
 
 
 @view_config(name='add-review-comment.json',
              context=IReviewTarget, request_type=IPyAMSLayer,
              renderer='json', xhr=True,
              permission=COMMENT_CONTENT_PERMISSION)
-def review_comment_add_view(request):
+def add_review_comment(request):
     """Review comment add view"""
     translate = request.localizer.translate
     comment_body = request.params.get('comment')
     if not comment_body:
         return {
             'status': 'error',
             'message': translate(_("Message is mandatory!"))
```

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/comment.pt` & `pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/comment.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/comments.pt` & `pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/comments.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/review/zmi/templates/mail-notification.pt` & `pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/mail-notification.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/manager.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
             order_by = params.get('order_by', context.order_by)
             if (order_by == RELEVANCE_ORDER) and \
                     not self.has_user_query(request):
                 request.GET['order_by'] = order_by = VISIBLE_PUBLICATION_DATE_ORDER
             renderer_settings = IPortletRendererSettings(self)
             if IAggregatedPortletRenderer.providedBy(renderer_settings):
                 aggregates = renderer_settings.aggregates
+                ignore_cache = True
             else:
                 aggregates = {}
             yield from context.get_results(context, order_by,
                                            reverse=order_by != RELEVANCE_ORDER,
                                            limit=limit,
                                            start=int(start),
                                            length=int(length),
```

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/skin/zmi.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/zmi.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt` & `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/thesaurus.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/zmi/manager.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/zmi/reference.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/zmi/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/search/zmi/thesaurus.py` & `pyams_content-1.99.2/src/pyams_content/feature/search/zmi/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/sitemap/__init__.py` & `pyams_content-1.99.2/src/pyams_content/feature/sitemap/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/feature/sitemap/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/feature/sitemap/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/generations/__init__.py` & `pyams_content-1.99.2/src/pyams_content/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/include.py` & `pyams_content-1.99.2/src/pyams_content/include.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 from pyams_content.component.extfile.interfaces import IExtFileManagerTarget
 from pyams_content.component.thesaurus import ICollectionsManagerTarget, ITagsManagerTarget, \
     IThemesManagerTarget
 from pyams_content.feature.preview.interfaces import IPreviewTarget
 from pyams_content.interfaces import COMMENT_CONTENT_PERMISSION, CONTRIBUTOR_ROLE, \
     CREATE_CONTENT_PERMISSION, CREATE_VERSION_PERMISSION, GUEST_ROLE, MANAGER_ROLE, \
-    MANAGE_CONTENT_PERMISSION, MANAGE_SITE_PERMISSION, MANAGE_SITE_ROOT_PERMISSION, \
+    MANAGE_CONTENT_PERMISSION, MANAGE_REFERENCE_TABLE_PERMISSION, MANAGE_SITE_PERMISSION, MANAGE_SITE_ROOT_PERMISSION, \
     MANAGE_SITE_TREE_PERMISSION, MANAGE_TOOL_PERMISSION, OID_ACCESS_PATH, OID_ACCESS_ROUTE, OPERATOR_ROLE, OWNER_ROLE, \
-    PILOT_ROLE, PUBLISH_CONTENT_PERMISSION, READER_ROLE, WEBMASTER_ROLE
+    PILOT_ROLE, PUBLISH_CONTENT_PERMISSION, READER_ROLE, REFERENCE_MANAGER_ROLE, WEBMASTER_ROLE
 from pyams_layer.interfaces import MANAGE_SKIN_PERMISSION
 from pyams_security.interfaces.base import MANAGE_PERMISSION, MANAGE_ROLES_PERMISSION, \
     PUBLIC_PERMISSION, ROLE_ID, VIEW_PERMISSION, VIEW_SYSTEM_PERMISSION
 from pyams_security.interfaces.names import ADMIN_USER_ID, SYSTEM_ADMIN_ROLE
 from pyams_site.site import BaseSiteRoot
 from pyams_thesaurus.interfaces import ADMIN_THESAURUS_PERMISSION, CREATE_THESAURUS_PERMISSION, \
     MANAGE_THESAURUS_CONTENT_PERMISSION, MANAGE_THESAURUS_EXTRACT_PERMISSION
@@ -49,14 +49,18 @@
 
     # register permissions
     config.register_permission({
         'id': MANAGE_SITE_ROOT_PERMISSION,
         'title': _("Manage main site root properties")
     })
     config.register_permission({
+        'id': MANAGE_REFERENCE_TABLE_PERMISSION,
+        'title': _("Manage references table")
+    })
+    config.register_permission({
         'id': MANAGE_SITE_TREE_PERMISSION,
         'title': _("Manage first level site tree elements")
     })
     config.register_permission({
         'id': MANAGE_SITE_PERMISSION,
         'title': _("Manage site, blog or hub properties")
     })
@@ -84,42 +88,56 @@
         'id': PUBLISH_CONTENT_PERMISSION,
         'title': _("Publish or retire existing content")
     })
 
     # upgrade system manager roles
     config.upgrade_role(SYSTEM_ADMIN_ROLE,
                         permissions={
-                            COMMENT_CONTENT_PERMISSION, CREATE_CONTENT_PERMISSION,
+                            MANAGE_SITE_ROOT_PERMISSION, MANAGE_REFERENCE_TABLE_PERMISSION,
+                            MANAGE_SITE_TREE_PERMISSION, MANAGE_SITE_PERMISSION,
+                            MANAGE_TOOL_PERMISSION, CREATE_CONTENT_PERMISSION,
                             CREATE_VERSION_PERMISSION, MANAGE_CONTENT_PERMISSION,
-                            MANAGE_SITE_PERMISSION, MANAGE_SITE_ROOT_PERMISSION,
-                            MANAGE_SITE_TREE_PERMISSION, MANAGE_TOOL_PERMISSION,
-                            PUBLISH_CONTENT_PERMISSION
+                            COMMENT_CONTENT_PERMISSION, PUBLISH_CONTENT_PERMISSION
                         })
 
     # register new roles
     config.register_role({
         'id': WEBMASTER_ROLE,
         'title': _("Webmaster (role)"),
         'permissions': {
             PUBLIC_PERMISSION, VIEW_PERMISSION, MANAGE_PERMISSION,
             VIEW_SYSTEM_PERMISSION, MANAGE_ROLES_PERMISSION,
             CREATE_THESAURUS_PERMISSION, ADMIN_THESAURUS_PERMISSION,
             MANAGE_THESAURUS_CONTENT_PERMISSION, MANAGE_THESAURUS_EXTRACT_PERMISSION,
-            MANAGE_SITE_ROOT_PERMISSION, MANAGE_SITE_TREE_PERMISSION,
-            MANAGE_SITE_PERMISSION, MANAGE_TOOL_PERMISSION,
-            CREATE_CONTENT_PERMISSION, MANAGE_CONTENT_PERMISSION,
-            CREATE_VERSION_PERMISSION, MANAGE_SKIN_PERMISSION,
-            COMMENT_CONTENT_PERMISSION, PUBLISH_CONTENT_PERMISSION
+            MANAGE_SITE_ROOT_PERMISSION, MANAGE_REFERENCE_TABLE_PERMISSION,
+            MANAGE_SITE_TREE_PERMISSION, MANAGE_SITE_PERMISSION,
+            MANAGE_TOOL_PERMISSION, CREATE_CONTENT_PERMISSION,
+            CREATE_VERSION_PERMISSION, MANAGE_CONTENT_PERMISSION,
+            COMMENT_CONTENT_PERMISSION, PUBLISH_CONTENT_PERMISSION,
+            MANAGE_SKIN_PERMISSION
         },
         'managers': {
             ADMIN_USER_ID,
             ROLE_ID.format(SYSTEM_ADMIN_ROLE)
         }
     })
     config.register_role({
+        'id': REFERENCE_MANAGER_ROLE,
+        'title': _("References manager (role)"),
+        'permissions': {
+            PUBLIC_PERMISSION, VIEW_PERMISSION, VIEW_SYSTEM_PERMISSION,
+            MANAGE_REFERENCE_TABLE_PERMISSION
+        },
+        'managers': {
+            ADMIN_USER_ID,
+            ROLE_ID.format(SYSTEM_ADMIN_ROLE),
+            ROLE_ID.format(WEBMASTER_ROLE)
+        }
+    })
+    config.register_role({
         'id': PILOT_ROLE,
         'title': _("Pilot (role)"),
         'permissions': {
             PUBLIC_PERMISSION, VIEW_PERMISSION, MANAGE_PERMISSION,
             VIEW_SYSTEM_PERMISSION, MANAGE_ROLES_PERMISSION,
             MANAGE_SITE_PERMISSION, MANAGE_TOOL_PERMISSION,
             MANAGE_CONTENT_PERMISSION, COMMENT_CONTENT_PERMISSION,
```

### Comparing `pyams_content-1.99.1/src/pyams_content/interfaces/__init__.py` & `pyams_content-1.99.2/src/pyams_content/interfaces/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 #
 # Custom permissions
 #
 
 MANAGE_SITE_ROOT_PERMISSION = 'pyams.ManageSiteRoot'
 '''Permission required to manage main site root properties'''
 
+MANAGE_REFERENCE_TABLE_PERMISSION = 'pyams.ManageReferenceTable'
+'''Permission required to manage reference table properties'''
+
 MANAGE_SITE_TREE_PERMISSION = 'pyams.ManageSiteTree'
 '''Permission required to create first level site elements'''
 
 MANAGE_SITE_PERMISSION = 'pyams.ManageSite'
 '''Permission required to manager inner site or blog properties'''
 
 MANAGE_TOOL_PERMISSION = 'pyams.ManageTool'
@@ -63,14 +66,17 @@
 #
 # Custom roles
 #
 
 WEBMASTER_ROLE = 'pyams.Webmaster'
 '''Webmaster role has all permissions on all contents'''
 
+REFERENCE_MANAGER_ROLE = 'pyams.ReferenceManager'
+'''References manager role has permissions to handle references tables'''
+
 PILOT_ROLE = 'pyams.Pilot'
 '''Pilot role is allowed to manage tools configuration and permissions'''
 
 MANAGER_ROLE = 'pyams.Manager'
 '''Manager role is allowed to manage contents workflow'''
 
 OWNER_ROLE = 'pyams.Owner'
```

### Comparing `pyams_content-1.99.1/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo` & `pyams_content-1.99.2/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2092,14 +2092,17 @@
 
 msgid "Manage first level site tree elements"
 msgstr "Gérer les sites de premier niveau"
 
 msgid "Manage main site root properties"
 msgstr "Gérer les propriétés globales du site"
 
+msgid "Manage references table"
+msgstr "Gérer les tables de références"
+
 msgid "Manage shared tool properties"
 msgstr "Gérer les propriétés d'un outil partagé"
 
 msgid "Manage site, blog or hub properties"
 msgstr "Gérer les propriétés d'un site, d'un blog ou d'un hub"
 
 msgid "Manager (role)"
@@ -2868,14 +2871,17 @@
 "Référence des vues dont les résultats sont extraits ; vous pouvez combiner "
 "les résultats de plusieurs vues ensemble en indiquant la façon de mélanger "
 "leurs résultats"
 
 msgid "References"
 msgstr "Références"
 
+msgid "References manager (role)"
+msgstr "Gestionnaire de références (rôle)"
+
 msgid "References settings"
 msgstr "Paramétrage des références internes"
 
 msgid "References tables"
 msgstr "Références"
 
 msgid "Refuse publication"
@@ -3446,14 +3452,20 @@
 
 msgid "Table contents"
 msgstr "Contenu"
 
 msgid "Table management"
 msgstr "Gérer cette table"
 
+msgid "Table managers"
+msgstr "Gestionnaires"
+
+msgid "Table managers can handle all table contents"
+msgstr "Liste des gestionnaires autorisés à gérer le contenu de cette table"
+
 msgid "Tags"
 msgstr "Tags"
 
 msgid "Tags search target"
 msgstr "Cible de la recherche par tags"
 
 msgid "Tags settings"
```

### Comparing `pyams_content-1.99.1/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po` & `pyams_content-1.99.2/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,108 +1,116 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2024-03-24 02:24+0100\n"
+"POT-Creation-Date: 2024-04-24 23:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.14\n"
 
 #: src/pyams_content/include.py:53
 msgid "Manage main site root properties"
 msgstr "Gérer les propriétés globales du site"
 
 #: src/pyams_content/include.py:57
+msgid "Manage references table"
+msgstr "Gérer les tables de références"
+
+#: src/pyams_content/include.py:61
 msgid "Manage first level site tree elements"
 msgstr "Gérer les sites de premier niveau"
 
-#: src/pyams_content/include.py:61
+#: src/pyams_content/include.py:65
 msgid "Manage site, blog or hub properties"
 msgstr "Gérer les propriétés d'un site, d'un blog ou d'un hub"
 
-#: src/pyams_content/include.py:65
+#: src/pyams_content/include.py:69
 msgid "Manage shared tool properties"
 msgstr "Gérer les propriétés d'un outil partagé"
 
-#: src/pyams_content/include.py:69
+#: src/pyams_content/include.py:73
 msgid "Create new content"
 msgstr "Créer un nouveau contenu"
 
-#: src/pyams_content/include.py:73
+#: src/pyams_content/include.py:77
 msgid "Create new version of existing content"
 msgstr "Créer une nouvelle version d'un contenu"
 
-#: src/pyams_content/include.py:77
+#: src/pyams_content/include.py:81
 msgid "Manage content properties"
 msgstr "Gérer les propriétés d'un contenu"
 
-#: src/pyams_content/include.py:81
+#: src/pyams_content/include.py:85
 msgid "Comment existing content"
 msgstr "Commenter un contenu"
 
-#: src/pyams_content/include.py:85
+#: src/pyams_content/include.py:89
 msgid "Publish or retire existing content"
 msgstr "Publier ou retirer un contenu"
 
-#: src/pyams_content/include.py:101
+#: src/pyams_content/include.py:105
 msgid "Webmaster (role)"
 msgstr "Webmestre (rôle)"
 
-#: src/pyams_content/include.py:120
+#: src/pyams_content/include.py:125
+msgid "References manager (role)"
+msgstr "Gestionnaire de références (rôle)"
+
+#: src/pyams_content/include.py:138
 msgid "Pilot (role)"
 msgstr "Pilote (rôle)"
 
-#: src/pyams_content/include.py:136
+#: src/pyams_content/include.py:154
 msgid "Manager (role)"
 msgstr "Responsable (rôle)"
 
-#: src/pyams_content/include.py:152
+#: src/pyams_content/include.py:170
 msgid "Owner (role)"
 msgstr "Propriétaire (rôle)"
 
-#: src/pyams_content/include.py:162
+#: src/pyams_content/include.py:180
 msgid "Contributor (role)"
 msgstr "Contributeur (rôle)"
 
-#: src/pyams_content/include.py:179
+#: src/pyams_content/include.py:197
 msgid "Reader (role)"
 msgstr "Relecteur (rôle)"
 
-#: src/pyams_content/include.py:196
+#: src/pyams_content/include.py:214
 msgid "Operator (role)"
 msgstr "Opérateur (rôle)"
 
-#: src/pyams_content/include.py:207
+#: src/pyams_content/include.py:225
 msgid "Guest user (role)"
 msgstr "Invité (rôle)"
 
 #: src/pyams_content/zmi/dashboard.py:84
 msgid "Switch element visibility"
 msgstr "Cliquez pour rendre l'élément visible ou non"
 
 #: src/pyams_content/zmi/dashboard.py:85
 msgid "Visible element?"
 msgstr ""
 "Un élément peut ne pas être visible s'il n'a pas encore été publié ou si son "
 "niveau parent n'est pas publié"
 
 #: src/pyams_content/zmi/dashboard.py:112
-#: src/pyams_content/reference/zmi/table.py:99
+#: src/pyams_content/reference/zmi/table.py:98
 #: src/pyams_content/feature/navigation/portlet/interfaces.py:33
 #: src/pyams_content/feature/navigation/portlet/interfaces.py:47
 #: src/pyams_content/feature/search/portlet/interfaces.py:44
-#: src/pyams_content/interfaces/__init__.py:116
+#: src/pyams_content/interfaces/__init__.py:122
 #: src/pyams_content/component/paragraph/zmi/container.py:236
 #: src/pyams_content/component/paragraph/portlet/interfaces.py:33
 #: src/pyams_content/component/gallery/interfaces.py:118
 #: src/pyams_content/component/gallery/portlet/interfaces.py:33
 #: src/pyams_content/shared/site/zmi/folder.py:83
 #: src/pyams_content/shared/form/interfaces.py:49
 #: src/pyams_content/shared/view/portlet/interfaces.py:64
@@ -154,32 +162,40 @@
 msgid "Last update"
 msgstr "Dernière modification"
 
 #: src/pyams_content/zmi/viewlet/toplinks.py:37
 msgid "Shortcuts"
 msgstr "Contenus"
 
-#: src/pyams_content/reference/zmi/table.py:51
+#: src/pyams_content/reference/interfaces.py:48
+msgid "Table managers"
+msgstr "Gestionnaires"
+
+#: src/pyams_content/reference/interfaces.py:49
+msgid "Table managers can handle all table contents"
+msgstr "Liste des gestionnaires autorisés à gérer le contenu de cette table"
+
+#: src/pyams_content/reference/zmi/table.py:50
 #: src/pyams_content/shared/site/zmi/manager.py:167
 #: src/pyams_content/shared/site/zmi/folder.py:180
 #: src/pyams_content/shared/common/zmi/manager.py:82
 #: src/pyams_content/shared/common/zmi/__init__.py:305
 #: src/pyams_content/root/zmi/__init__.py:63
 msgid "Properties"
 msgstr "Propriétés"
 
-#: src/pyams_content/reference/zmi/table.py:62
+#: src/pyams_content/reference/zmi/table.py:61
 msgid "Pictograms table"
 msgstr "Table des pictogrammes"
 
-#: src/pyams_content/reference/zmi/table.py:63
+#: src/pyams_content/reference/zmi/table.py:62
 msgid "Edit table properties"
 msgstr "Propriétés de la table"
 
-#: src/pyams_content/reference/zmi/table.py:73
+#: src/pyams_content/reference/zmi/table.py:72
 msgid "Table management"
 msgstr "Gérer cette table"
 
 #: src/pyams_content/reference/zmi/__init__.py:33
 #: src/pyams_content/shared/view/zmi/references.py:50
 msgid "References"
 msgstr "Références"
@@ -821,15 +837,15 @@
 msgstr "Commentaire"
 
 #: src/pyams_content/feature/review/interfaces.py:73
 msgid "Reviewer comment?"
 msgstr "Commentaire d'un relecteur"
 
 #: src/pyams_content/feature/review/interfaces.py:77
-#: src/pyams_content/interfaces/__init__.py:128
+#: src/pyams_content/interfaces/__init__.py:134
 #: src/pyams_content/shared/common/zmi/search.py:225
 #: src/pyams_content/root/zmi/search.py:160
 msgid "Creation date"
 msgstr "Date de création"
 
 #: src/pyams_content/feature/review/interfaces.py:89
 msgid "Reviewers list"
@@ -938,16 +954,16 @@
 msgstr "Bonjour,"
 
 #: src/pyams_content/feature/review/zmi/templates/mail-notification.pt:31
 msgid ""
 "You have been requested by ${sender}, contributor of « ${service_name} » "
 "website, to make a review of a content."
 msgstr ""
-"Vous êtes sollicité par ${sender}, contributor du site internet « "
-"${service_name} », qui souhaite recueillir votre commentaire à propos d'un "
+"Vous êtes sollicité par ${sender}, contributor du site internet "
+"« ${service_name} », qui souhaite recueillir votre commentaire à propos d'un "
 "contenu."
 
 #: src/pyams_content/feature/review/zmi/templates/mail-notification.pt:36
 msgid "${sender} added the following message to his request:"
 msgstr "${sender} a accompagné sa demande de relecture du message suivant :"
 
 #: src/pyams_content/feature/review/zmi/templates/mail-notification.pt:41
@@ -1480,15 +1496,15 @@
 "display target in it's attachment context (if defined)"
 msgstr ""
 "Par défaut, les liens internes utilisent une URl \"relative\", qui tente "
 "d'afficher la cible du lien dans le contexte courant ; en utilisant une URL "
 "canonique, vous pouvez imposer l'affichage de ce contenu dans son contexte "
 "d'origine, s'il est défini"
 
-#: src/pyams_content/feature/search/portlet/__init__.py:113
+#: src/pyams_content/feature/search/portlet/__init__.py:114
 #: src/pyams_content/shared/common/zmi/owner.py:362
 #: src/pyams_content/shared/common/zmi/search.py:430
 msgid "Search results"
 msgstr "Résultats de la recherche"
 
 #: src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt:5
 msgid "First search results sample:"
@@ -1761,47 +1777,47 @@
 msgid "Preview"
 msgstr "Aperçu"
 
 #: src/pyams_content/feature/preview/zmi/__init__.py:75
 msgid "Open preview in new tab"
 msgstr "Ouvrir l'aperçu dans un nouvel onglet"
 
-#: src/pyams_content/interfaces/__init__.py:110
+#: src/pyams_content/interfaces/__init__.py:116
 msgid "Unique key"
 msgstr "Nom du contenu"
 
-#: src/pyams_content/interfaces/__init__.py:111
+#: src/pyams_content/interfaces/__init__.py:117
 msgid ""
 "WARNING: this key can't be modified after creation!!! Spaces, uppercase "
 "letters or accentuated characters will be replaced automatically."
 msgstr ""
 "ATTENTION : cette clé ne pourra pas être modifiée après sa création ! Les "
 "espaces, majuscules et caractères accentués seront remplacés "
 "automatiquement..."
 
-#: src/pyams_content/interfaces/__init__.py:117
+#: src/pyams_content/interfaces/__init__.py:123
 #: src/pyams_content/shared/site/zmi/folder.py:84
 msgid "Visible label used to display content"
 msgstr "Libellé principal du contenu"
 
-#: src/pyams_content/interfaces/__init__.py:120
+#: src/pyams_content/interfaces/__init__.py:126
 msgid "Short name"
 msgstr "Fil d'Ariane"
 
-#: src/pyams_content/interfaces/__init__.py:121
+#: src/pyams_content/interfaces/__init__.py:127
 msgid "Short name used in breadcrumbs"
 msgstr "Libellé court visible dans le fil d'Ariane"
 
-#: src/pyams_content/interfaces/__init__.py:132
+#: src/pyams_content/interfaces/__init__.py:138
 #: src/pyams_content/shared/common/zmi/search.py:228
 #: src/pyams_content/root/zmi/search.py:163
 msgid "Modification date"
 msgstr "Date de dernière modification"
 
-#: src/pyams_content/interfaces/__init__.py:144
+#: src/pyams_content/interfaces/__init__.py:150
 msgid "Object types"
 msgstr "Types de l'objet"
 
 #: src/pyams_content/component/illustration/interfaces.py:44
 #: src/pyams_content/component/illustration/interfaces.py:120
 #: src/pyams_content/component/gallery/interfaces.py:48
 msgid "Image or video data"
@@ -2318,42 +2334,42 @@
 "Un paragraphe verrouillé ne peut être supprimé que par un responsable des "
 "contenus ou un webmestre"
 
 #: src/pyams_content/component/paragraph/interfaces/__init__.py:65
 msgid "§ Title"
 msgstr "Titre §"
 
-#: src/pyams_content/component/paragraph/interfaces/__init__.py:112
+#: src/pyams_content/component/paragraph/interfaces/__init__.py:115
 msgid "Allowed paragraphs"
 msgstr "Types de blocs autorisés"
 
-#: src/pyams_content/component/paragraph/interfaces/__init__.py:113
+#: src/pyams_content/component/paragraph/interfaces/__init__.py:116
 msgid ""
 "List of paragraphs allowed for this content type; if selection is empty, all "
 "paragraphs types will be allowed"
 msgstr ""
 "Liste des types de blocs autorisés au sein de ce gabarit ; une sélection "
 "vide indique que tous les types de blocs seront utilisables"
 
-#: src/pyams_content/component/paragraph/interfaces/__init__.py:118
+#: src/pyams_content/component/paragraph/interfaces/__init__.py:121
 msgid "Default paragraphs types"
 msgstr "Types de blocs par défaut"
 
-#: src/pyams_content/component/paragraph/interfaces/__init__.py:119
+#: src/pyams_content/component/paragraph/interfaces/__init__.py:122
 msgid ""
 "Empty paragraphs of these types will be added automatically to new contents "
 "of this content type; if paragraphs are associated to content type, these "
 "will be used instead of these ones"
 msgstr ""
 "Des blocs vides des types sélectionnés seront créés automatiquement dans les "
 "nouveaux contenus de ce gabarit lors de leur création ; si des blocs de "
 "contenus sont associés au type de contenu sélectionné lors de la création "
 "d'un contenu, ceux-ci seront prioritaires par rapport à ceux sélectionnés ici"
 
-#: src/pyams_content/component/paragraph/interfaces/__init__.py:146
+#: src/pyams_content/component/paragraph/interfaces/__init__.py:149
 msgid "Renderer"
 msgstr "Mode de rendu"
 
 #: src/pyams_content/component/paragraph/portlet/interfaces.py:36
 msgid "Paragraphs source"
 msgstr "Source des blocs de contenu"
 
@@ -3767,16 +3783,16 @@
 msgstr "En-tête du formulaire"
 
 #: src/pyams_content/shared/common/types.py:234
 #, python-format
 msgid "-- missing value ({}) --"
 msgstr "-- valeur manquante ({}) --"
 
-#: src/pyams_content/shared/common/__init__.py:117
-#: src/pyams_content/shared/common/__init__.py:126
+#: src/pyams_content/shared/common/__init__.py:135
+#: src/pyams_content/shared/common/__init__.py:144
 #, python-format
 msgid "{date} by {principal}"
 msgstr "{date} par {principal}"
 
 #: src/pyams_content/shared/common/zmi/workflow.py:61
 msgid "Workflow action"
 msgstr "Action du workflow"
@@ -4966,70 +4982,70 @@
 #: src/pyams_content/shared/common/interfaces/__init__.py:256
 msgid ""
 "Guests are users which are allowed to view contents with restricted access"
 msgstr ""
 "Les invités sont autorisés à consulter les contenus sur lesquels des "
 "restrictions d'accès ont été appliquées"
 
-#: src/pyams_content/shared/common/interfaces/__init__.py:303
+#: src/pyams_content/shared/common/interfaces/__init__.py:306
 msgid "Principal ID"
 msgstr "Mandataire"
 
-#: src/pyams_content/shared/common/interfaces/__init__.py:333
+#: src/pyams_content/shared/common/interfaces/__init__.py:336
 msgid "Show workflow checks warning"
 msgstr "Activer le tunnel de publication"
 
-#: src/pyams_content/shared/common/interfaces/__init__.py:334
+#: src/pyams_content/shared/common/interfaces/__init__.py:337
 msgid ""
 "If 'yes', this contributor will have to confirm that contents have been "
 "checked before asking for publication"
 msgstr ""
 "Si 'oui', ce contributeur devra confirmer explicitement que ses contenus ont "
 "été prévisualisés et vérifiés avant de pouvoir demander leur publication"
 
-#: src/pyams_content/shared/common/interfaces/__init__.py:340
+#: src/pyams_content/shared/common/interfaces/__init__.py:343
 msgid "Substitute for"
 msgstr "Suppléant de"
 
-#: src/pyams_content/shared/common/interfaces/__init__.py:341
+#: src/pyams_content/shared/common/interfaces/__init__.py:344
 msgid "Contributor will have access to contents owned by these principals"
 msgstr ""
 "Le contributeur aura accès aux contenus dont ces mandataires sont "
 "propriétaires"
 
-#: src/pyams_content/shared/common/interfaces/__init__.py:363
+#: src/pyams_content/shared/common/interfaces/__init__.py:366
 msgid "Publication checks"
 msgstr "Activer le tunnel de publication"
 
-#: src/pyams_content/shared/common/interfaces/__init__.py:364
+#: src/pyams_content/shared/common/interfaces/__init__.py:367
 msgid ""
 "If 'yes', this manager will have to confirm that contents have been "
 "previewed and checked before publishing a content"
 msgstr ""
 "Si 'oui', ce responsable devra confirmer explicitement que les contenus qui "
 "lui ont été transmis ont été prévisualisés et vérifiés avant de pouvoir les "
 "publier"
 
-#: src/pyams_content/shared/common/interfaces/__init__.py:370
+#: src/pyams_content/shared/common/interfaces/__init__.py:373
 msgid "Restricted contents"
 msgstr "Activer des restrictions d'accès"
 
-#: src/pyams_content/shared/common/interfaces/__init__.py:371
+#: src/pyams_content/shared/common/interfaces/__init__.py:374
 msgid ""
 "If 'yes', this manager will get restricted access to manage contents based "
 "on selected settings"
 msgstr ""
 "Si 'oui', ce responsable ne pourra gérer que des contenus dont les "
 "propriétés correspondent à au moins l'un des paramètres indiqués ci-dessous"
 
-#: src/pyams_content/shared/common/interfaces/__init__.py:376
+#: src/pyams_content/shared/common/interfaces/__init__.py:379
 msgid "Selected owners"
 msgstr "Propriétaires"
 
-#: src/pyams_content/shared/common/interfaces/__init__.py:377
+#: src/pyams_content/shared/common/interfaces/__init__.py:380
 msgid "Manager will have access to contents owned by these principals"
 msgstr "Ce responsable aura accès aux contenus de ces propriétaires"
 
 #: src/pyams_content/shared/common/portlet/title.py:44
 msgid "Content title"
 msgstr "Titre du contenu"
 
@@ -5144,15 +5160,15 @@
 msgstr "Couleur de base associée à ce type d'alerte"
 
 #: src/pyams_content/shared/alert/interfaces.py:80
 msgid "Alert"
 msgstr "Alerte"
 
 #: src/pyams_content/shared/alert/interfaces.py:86
-#: src/pyams_content/shared/alert/zmi/types.py:223
+#: src/pyams_content/shared/alert/zmi/types.py:222
 msgid "Alert type"
 msgstr "Type d'alerte"
 
 #: src/pyams_content/shared/alert/interfaces.py:87
 msgid "Alert type can affect renderer alert style"
 msgstr ""
 "Le type d'alerte peut éventuellement, en fonction du thème graphique, "
@@ -5235,15 +5251,15 @@
 msgid "New alert type"
 msgstr "Nouveau type d'alerte"
 
 #: src/pyams_content/shared/alert/zmi/types.py:182
 msgid "New alert type properties"
 msgstr "Propriétés du nouveau type"
 
-#: src/pyams_content/shared/alert/zmi/types.py:238
+#: src/pyams_content/shared/alert/zmi/types.py:237
 msgid "Alert type properties"
 msgstr "Propriétés du type d'alerte"
 
 #: src/pyams_content/shared/alert/zmi/__init__.py:55
 msgid "Alert management"
 msgstr "Cette alerte"
```

### Comparing `pyams_content-1.99.1/src/pyams_content/locales/pyams_content.pot` & `pyams_content-1.99.2/src/pyams_content/locales/pyams_content.pot`

 * *Files 0% similar despite different names*

```diff
@@ -2,106 +2,114 @@
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2024-03-24 02:24+0100\n"
+"POT-Creation-Date: 2024-04-24 23:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.15.0\n"
 
 #: ./src/pyams_content/include.py:53
 msgid "Manage main site root properties"
 msgstr ""
 
 #: ./src/pyams_content/include.py:57
-msgid "Manage first level site tree elements"
+msgid "Manage references table"
 msgstr ""
 
 #: ./src/pyams_content/include.py:61
-msgid "Manage site, blog or hub properties"
+msgid "Manage first level site tree elements"
 msgstr ""
 
 #: ./src/pyams_content/include.py:65
-msgid "Manage shared tool properties"
+msgid "Manage site, blog or hub properties"
 msgstr ""
 
 #: ./src/pyams_content/include.py:69
-msgid "Create new content"
+msgid "Manage shared tool properties"
 msgstr ""
 
 #: ./src/pyams_content/include.py:73
-msgid "Create new version of existing content"
+msgid "Create new content"
 msgstr ""
 
 #: ./src/pyams_content/include.py:77
-msgid "Manage content properties"
+msgid "Create new version of existing content"
 msgstr ""
 
 #: ./src/pyams_content/include.py:81
-msgid "Comment existing content"
+msgid "Manage content properties"
 msgstr ""
 
 #: ./src/pyams_content/include.py:85
+msgid "Comment existing content"
+msgstr ""
+
+#: ./src/pyams_content/include.py:89
 msgid "Publish or retire existing content"
 msgstr ""
 
-#: ./src/pyams_content/include.py:101
+#: ./src/pyams_content/include.py:105
 msgid "Webmaster (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:120
+#: ./src/pyams_content/include.py:125
+msgid "References manager (role)"
+msgstr ""
+
+#: ./src/pyams_content/include.py:138
 msgid "Pilot (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:136
+#: ./src/pyams_content/include.py:154
 msgid "Manager (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:152
+#: ./src/pyams_content/include.py:170
 msgid "Owner (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:162
+#: ./src/pyams_content/include.py:180
 msgid "Contributor (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:179
+#: ./src/pyams_content/include.py:197
 msgid "Reader (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:196
+#: ./src/pyams_content/include.py:214
 msgid "Operator (role)"
 msgstr ""
 
-#: ./src/pyams_content/include.py:207
+#: ./src/pyams_content/include.py:225
 msgid "Guest user (role)"
 msgstr ""
 
 #: ./src/pyams_content/zmi/dashboard.py:84
 msgid "Switch element visibility"
 msgstr ""
 
 #: ./src/pyams_content/zmi/dashboard.py:85
 msgid "Visible element?"
 msgstr ""
 
 #: ./src/pyams_content/zmi/dashboard.py:112
-#: ./src/pyams_content/reference/zmi/table.py:99
+#: ./src/pyams_content/reference/zmi/table.py:98
 #: ./src/pyams_content/feature/navigation/portlet/interfaces.py:33
 #: ./src/pyams_content/feature/navigation/portlet/interfaces.py:47
 #: ./src/pyams_content/feature/search/portlet/interfaces.py:44
-#: ./src/pyams_content/interfaces/__init__.py:116
+#: ./src/pyams_content/interfaces/__init__.py:122
 #: ./src/pyams_content/component/paragraph/zmi/container.py:236
 #: ./src/pyams_content/component/paragraph/portlet/interfaces.py:33
 #: ./src/pyams_content/component/gallery/interfaces.py:118
 #: ./src/pyams_content/component/gallery/portlet/interfaces.py:33
 #: ./src/pyams_content/shared/site/zmi/folder.py:83
 #: ./src/pyams_content/shared/form/interfaces.py:49
 #: ./src/pyams_content/shared/view/portlet/interfaces.py:64
@@ -153,32 +161,40 @@
 msgid "Last update"
 msgstr ""
 
 #: ./src/pyams_content/zmi/viewlet/toplinks.py:37
 msgid "Shortcuts"
 msgstr ""
 
-#: ./src/pyams_content/reference/zmi/table.py:51
+#: ./src/pyams_content/reference/interfaces.py:48
+msgid "Table managers"
+msgstr ""
+
+#: ./src/pyams_content/reference/interfaces.py:49
+msgid "Table managers can handle all table contents"
+msgstr ""
+
+#: ./src/pyams_content/reference/zmi/table.py:50
 #: ./src/pyams_content/shared/site/zmi/manager.py:167
 #: ./src/pyams_content/shared/site/zmi/folder.py:180
 #: ./src/pyams_content/shared/common/zmi/manager.py:82
 #: ./src/pyams_content/shared/common/zmi/__init__.py:305
 #: ./src/pyams_content/root/zmi/__init__.py:63
 msgid "Properties"
 msgstr ""
 
-#: ./src/pyams_content/reference/zmi/table.py:62
+#: ./src/pyams_content/reference/zmi/table.py:61
 msgid "Pictograms table"
 msgstr ""
 
-#: ./src/pyams_content/reference/zmi/table.py:63
+#: ./src/pyams_content/reference/zmi/table.py:62
 msgid "Edit table properties"
 msgstr ""
 
-#: ./src/pyams_content/reference/zmi/table.py:73
+#: ./src/pyams_content/reference/zmi/table.py:72
 msgid "Table management"
 msgstr ""
 
 #: ./src/pyams_content/reference/zmi/__init__.py:33
 #: ./src/pyams_content/shared/view/zmi/references.py:50
 msgid "References"
 msgstr ""
@@ -802,15 +818,15 @@
 msgstr ""
 
 #: ./src/pyams_content/feature/review/interfaces.py:73
 msgid "Reviewer comment?"
 msgstr ""
 
 #: ./src/pyams_content/feature/review/interfaces.py:77
-#: ./src/pyams_content/interfaces/__init__.py:128
+#: ./src/pyams_content/interfaces/__init__.py:134
 #: ./src/pyams_content/shared/common/zmi/search.py:225
 #: ./src/pyams_content/root/zmi/search.py:160
 msgid "Creation date"
 msgstr ""
 
 #: ./src/pyams_content/feature/review/interfaces.py:89
 msgid "Reviewers list"
@@ -1398,15 +1414,15 @@
 #: ./src/pyams_content/shared/view/portlet/interfaces.py:112
 msgid ""
 "By default, internal links use a \"relative\" URL, which tries to display "
 "link target in the current context; by using a canonical URL, you can display"
 " target in it's attachment context (if defined)"
 msgstr ""
 
-#: ./src/pyams_content/feature/search/portlet/__init__.py:113
+#: ./src/pyams_content/feature/search/portlet/__init__.py:114
 #: ./src/pyams_content/shared/common/zmi/owner.py:362
 #: ./src/pyams_content/shared/common/zmi/search.py:430
 msgid "Search results"
 msgstr ""
 
 #: ./src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt:5
 msgid "First search results sample:"
@@ -1666,44 +1682,44 @@
 msgid "Preview"
 msgstr ""
 
 #: ./src/pyams_content/feature/preview/zmi/__init__.py:75
 msgid "Open preview in new tab"
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:110
+#: ./src/pyams_content/interfaces/__init__.py:116
 msgid "Unique key"
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:111
+#: ./src/pyams_content/interfaces/__init__.py:117
 msgid ""
 "WARNING: this key can't be modified after creation!!! Spaces, uppercase "
 "letters or accentuated characters will be replaced automatically."
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:117
+#: ./src/pyams_content/interfaces/__init__.py:123
 #: ./src/pyams_content/shared/site/zmi/folder.py:84
 msgid "Visible label used to display content"
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:120
+#: ./src/pyams_content/interfaces/__init__.py:126
 msgid "Short name"
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:121
+#: ./src/pyams_content/interfaces/__init__.py:127
 msgid "Short name used in breadcrumbs"
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:132
+#: ./src/pyams_content/interfaces/__init__.py:138
 #: ./src/pyams_content/shared/common/zmi/search.py:228
 #: ./src/pyams_content/root/zmi/search.py:163
 msgid "Modification date"
 msgstr ""
 
-#: ./src/pyams_content/interfaces/__init__.py:144
+#: ./src/pyams_content/interfaces/__init__.py:150
 msgid "Object types"
 msgstr ""
 
 #: ./src/pyams_content/component/illustration/interfaces.py:44
 #: ./src/pyams_content/component/illustration/interfaces.py:120
 #: ./src/pyams_content/component/gallery/interfaces.py:48
 msgid "Image or video data"
@@ -2189,36 +2205,36 @@
 "A locked paragraph can only be removed by a content manager or a webmaster"
 msgstr ""
 
 #: ./src/pyams_content/component/paragraph/interfaces/__init__.py:65
 msgid "§ Title"
 msgstr ""
 
-#: ./src/pyams_content/component/paragraph/interfaces/__init__.py:112
+#: ./src/pyams_content/component/paragraph/interfaces/__init__.py:115
 msgid "Allowed paragraphs"
 msgstr ""
 
-#: ./src/pyams_content/component/paragraph/interfaces/__init__.py:113
+#: ./src/pyams_content/component/paragraph/interfaces/__init__.py:116
 msgid ""
 "List of paragraphs allowed for this content type; if selection is empty, all "
 "paragraphs types will be allowed"
 msgstr ""
 
-#: ./src/pyams_content/component/paragraph/interfaces/__init__.py:118
+#: ./src/pyams_content/component/paragraph/interfaces/__init__.py:121
 msgid "Default paragraphs types"
 msgstr ""
 
-#: ./src/pyams_content/component/paragraph/interfaces/__init__.py:119
+#: ./src/pyams_content/component/paragraph/interfaces/__init__.py:122
 msgid ""
 "Empty paragraphs of these types will be added automatically to new contents "
 "of this content type; if paragraphs are associated to content type, these "
 "will be used instead of these ones"
 msgstr ""
 
-#: ./src/pyams_content/component/paragraph/interfaces/__init__.py:146
+#: ./src/pyams_content/component/paragraph/interfaces/__init__.py:149
 msgid "Renderer"
 msgstr ""
 
 #: ./src/pyams_content/component/paragraph/portlet/interfaces.py:36
 msgid "Paragraphs source"
 msgstr ""
 
@@ -3521,16 +3537,16 @@
 msgstr ""
 
 #: ./src/pyams_content/shared/common/types.py:234
 #, python-format
 msgid "-- missing value ({}) --"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/__init__.py:117
-#: ./src/pyams_content/shared/common/__init__.py:126
+#: ./src/pyams_content/shared/common/__init__.py:135
+#: ./src/pyams_content/shared/common/__init__.py:144
 #, python-format
 msgid "{date} by {principal}"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/zmi/workflow.py:61
 msgid "Workflow action"
 msgstr ""
@@ -4597,61 +4613,61 @@
 msgstr ""
 
 #: ./src/pyams_content/shared/common/interfaces/__init__.py:256
 msgid ""
 "Guests are users which are allowed to view contents with restricted access"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/interfaces/__init__.py:303
+#: ./src/pyams_content/shared/common/interfaces/__init__.py:306
 msgid "Principal ID"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/interfaces/__init__.py:333
+#: ./src/pyams_content/shared/common/interfaces/__init__.py:336
 msgid "Show workflow checks warning"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/interfaces/__init__.py:334
+#: ./src/pyams_content/shared/common/interfaces/__init__.py:337
 msgid ""
 "If 'yes', this contributor will have to confirm that contents have been "
 "checked before asking for publication"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/interfaces/__init__.py:340
+#: ./src/pyams_content/shared/common/interfaces/__init__.py:343
 msgid "Substitute for"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/interfaces/__init__.py:341
+#: ./src/pyams_content/shared/common/interfaces/__init__.py:344
 msgid "Contributor will have access to contents owned by these principals"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/interfaces/__init__.py:363
+#: ./src/pyams_content/shared/common/interfaces/__init__.py:366
 msgid "Publication checks"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/interfaces/__init__.py:364
+#: ./src/pyams_content/shared/common/interfaces/__init__.py:367
 msgid ""
 "If 'yes', this manager will have to confirm that contents have been previewed"
 " and checked before publishing a content"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/interfaces/__init__.py:370
+#: ./src/pyams_content/shared/common/interfaces/__init__.py:373
 msgid "Restricted contents"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/interfaces/__init__.py:371
+#: ./src/pyams_content/shared/common/interfaces/__init__.py:374
 msgid ""
 "If 'yes', this manager will get restricted access to manage contents based on"
 " selected settings"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/interfaces/__init__.py:376
+#: ./src/pyams_content/shared/common/interfaces/__init__.py:379
 msgid "Selected owners"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/interfaces/__init__.py:377
+#: ./src/pyams_content/shared/common/interfaces/__init__.py:380
 msgid "Manager will have access to contents owned by these principals"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/portlet/title.py:44
 msgid "Content title"
 msgstr ""
 
@@ -4757,15 +4773,15 @@
 msgstr ""
 
 #: ./src/pyams_content/shared/alert/interfaces.py:80
 msgid "Alert"
 msgstr ""
 
 #: ./src/pyams_content/shared/alert/interfaces.py:86
-#: ./src/pyams_content/shared/alert/zmi/types.py:223
+#: ./src/pyams_content/shared/alert/zmi/types.py:222
 msgid "Alert type"
 msgstr ""
 
 #: ./src/pyams_content/shared/alert/interfaces.py:87
 msgid "Alert type can affect renderer alert style"
 msgstr ""
 
@@ -4834,15 +4850,15 @@
 msgid "New alert type"
 msgstr ""
 
 #: ./src/pyams_content/shared/alert/zmi/types.py:182
 msgid "New alert type properties"
 msgstr ""
 
-#: ./src/pyams_content/shared/alert/zmi/types.py:238
+#: ./src/pyams_content/shared/alert/zmi/types.py:237
 msgid "Alert type properties"
 msgstr ""
 
 #: ./src/pyams_content/shared/alert/zmi/__init__.py:55
 msgid "Alert management"
 msgstr ""
```

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/alert/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 #
-# Copyright (c) 2015-2021 Thierry Florac <tflorac AT ulthar.net>
+# Copyright (c) 2015-2023 Thierry Florac <tflorac AT ulthar.net>
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 
-"""PyAMS_content.reference module
+"""PyAMS_content.shared.alert module
 
+This module defines alerts persistent classes.
 """
 
-from persistent import Persistent
-from pyramid.events import subscriber
-from zope.component.interfaces import ISite
-from zope.container.contained import Contained
-from zope.container.folder import Folder
 from zope.interface import implementer
-from zope.lifecycleevent import IObjectAddedEvent
 from zope.schema.fieldproperty import FieldProperty
 
-from pyams_content.interfaces import MANAGE_SITE_ROOT_PERMISSION
-from pyams_content.reference.interfaces import IReferenceInfo, IReferenceManager, IReferenceTable
-from pyams_i18n.interfaces import II18nManager
-from pyams_security.interfaces import IViewContextPermissionChecker
-from pyams_utils.adapter import ContextAdapter, adapter_config
+from pyams_content.component.thesaurus import ITagsTarget, IThemesTarget
+from pyams_content.feature.review import IReviewTarget
+from pyams_content.shared.alert.interfaces import ALERT_CONTENT_NAME, ALERT_CONTENT_TYPE, IAlert, IAlertManager, \
+    IAlertTypesManager, IWfAlert
+from pyams_content.shared.common import ISharedContent, IWfSharedContent, SharedContent, WfSharedContent
+from pyams_sequence.reference import InternalReferenceMixin, get_reference_target
 from pyams_utils.factory import factory_config
+from pyams_utils.request import check_request
 from pyams_utils.traversing import get_parent
 
-
 __docformat__ = 'restructuredtext'
 
 
-@factory_config(IReferenceManager)
-class ReferencesManager(Folder):
-    """References tables container"""
-
-    title = FieldProperty(IReferenceManager['title'])
-    short_name = FieldProperty(IReferenceManager['short_name'])
-
-    def __init__(self):
-        super().__init__()
-        self.title = {
-            'en': 'References tables',
-            'fr': 'Tables de références'
-        }
-        self.short_name = self.title.copy()
-
-
-@subscriber(IObjectAddedEvent, context_selector=IReferenceManager)
-def handle_added_references_manager(event):
-    """Handle new references manager"""
-    site = get_parent(event.object, ISite)
-    registry = site.getSiteManager()
-    if registry is not None:
-        registry.registerUtility(event.object, IReferenceManager)
-
-
-@implementer(IReferenceTable, II18nManager)
-class ReferenceTable(Folder):
-    """References table"""
-
-    title = FieldProperty(IReferenceTable['title'])
-    short_name = FieldProperty(IReferenceTable['short_name'])
-
-    languages = FieldProperty(II18nManager['languages'])
-
-
-@implementer(IReferenceInfo)
-class ReferenceInfo(Persistent, Contained):
-    """Reference record"""
-
-    title = FieldProperty(IReferenceInfo['title'])
-    short_name = FieldProperty(IReferenceInfo['short_name'])
-
-
-@adapter_config(required=IReferenceInfo,
-                provides=IViewContextPermissionChecker)
-class ReferenceInfoPermissionChecker(ContextAdapter):
-    """Reference info permission checker"""
-
-    edit_permission = MANAGE_SITE_ROOT_PERMISSION
+@factory_config(IWfAlert)
+@factory_config(IWfSharedContent, name=ALERT_CONTENT_TYPE)
+@implementer(ITagsTarget, IThemesTarget, IReviewTarget)
+class WfAlert(WfSharedContent, InternalReferenceMixin):
+    """Base alert"""
+
+    content_type = ALERT_CONTENT_TYPE
+    content_name = ALERT_CONTENT_NAME
+    content_intf = IWfAlert
+    content_view = False
+
+    handle_content_url = False
+    handle_header = False
+    handle_description = False
+
+    alert_type = FieldProperty(IWfAlert['alert_type'])
+    body = FieldProperty(IWfAlert['body'])
+    _reference = FieldProperty(IWfAlert['reference'])
+    external_url = FieldProperty(IWfAlert['external_url'])
+    references = FieldProperty(IWfAlert['references'])
+    maximum_interval = FieldProperty(IWfAlert['maximum_interval'])
+
+    def get_alert_type(self):
+        """Alert type getter"""
+        manager = get_parent(self, IAlertManager)
+        types = IAlertTypesManager(manager, None)
+        if types is not None:
+            return types.get(self.alert_type)
+
+    @property
+    def reference(self):
+        return self._reference
+
+    @reference.setter
+    def reference(self, value):
+        self._reference = value
+        del self.target
+
+    def get_targets(self, state=None):
+        request = check_request()
+        return [
+            get_reference_target(reference, state, request)
+            for reference in (self.references or ())
+        ]
+
+
+@factory_config(IAlert)
+@factory_config(ISharedContent, name=ALERT_CONTENT_TYPE)
+class Alert(SharedContent):
+    """Workflow managed alert class"""
+
+    content_type = ALERT_CONTENT_TYPE
+    content_name = ALERT_CONTENT_NAME
+    content_view = False
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/reference/interfaces.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,20 +10,24 @@
 # FOR A PARTICULAR PURPOSE.
 #
 
 """PyAMS_content.reference.interfaces module
 
 """
 
-__docformat__ = 'restructuredtext'
-
 from zope.container.constraints import containers, contains
 from zope.container.interfaces import IContainer
+from zope.interface import Interface
+
+from pyams_content.interfaces import IBaseContent, REFERENCE_MANAGER_ROLE
+from pyams_security.schema import PrincipalsSetField
+
+__docformat__ = 'restructuredtext'
 
-from pyams_content.interfaces import IBaseContent
+from pyams_content import _
 
 
 class IReferenceInfo(IBaseContent):
     """Base reference interface"""
 
     containers('.IReferenceTable')
 
@@ -31,11 +35,23 @@
 class IReferenceTable(IBaseContent):
     """Reference table interface"""
 
     containers('.IReferenceTableContainer')
     contains(IReferenceInfo)
 
 
+REFERENCE_TABLE_ROLES = 'pyams_content.reference.roles'
+
+
+class IReferenceTableRoles(Interface):
+    """Reference table roles interface"""
+
+    managers = PrincipalsSetField(title=_("Table managers"),
+                                  description=_("Table managers can handle all table contents"),
+                                  role_id=REFERENCE_MANAGER_ROLE,
+                                  required=False)
+
+
 class IReferenceManager(IBaseContent, IContainer):
     """References tables container"""
 
     contains(IReferenceTable)
```

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/pictogram/__init__.py` & `pyams_content-1.99.2/src/pyams_content/reference/pictogram/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,24 +16,20 @@
 
 __docformat__ = 'restructuredtext'
 
 from pyramid.events import subscriber
 from zope.component.interfaces import ISite
 from zope.lifecycleevent import IObjectAddedEvent
 from zope.schema.fieldproperty import FieldProperty
-from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
-from pyams_content.reference import ReferenceInfo, ReferenceTable
+from pyams_content.reference import ReferenceInfo, ReferenceTable, ReferencesVocabulary
 from pyams_content.reference.pictogram.interfaces import IPictogram, IPictogramTable, \
     PICTOGRAM_VOCABULARY
 from pyams_file.property import I18nFileProperty
-from pyams_i18n.interfaces import II18n
 from pyams_utils.factory import factory_config
-from pyams_utils.registry import query_utility
-from pyams_utils.request import check_request
 from pyams_utils.traversing import get_parent
 from pyams_utils.vocabulary import vocabulary_config
 
 
 @factory_config(IPictogramTable)
 class PictogramTable(ReferenceTable):
     """Pictogram table"""
@@ -54,22 +50,11 @@
 
     image = I18nFileProperty(IPictogram['image'])
     alt_title = FieldProperty(IPictogram['alt_title'])
     header = FieldProperty(IPictogram['header'])
 
 
 @vocabulary_config(name=PICTOGRAM_VOCABULARY)
-class PictogramsVocabulary(SimpleVocabulary):
+class PictogramsVocabulary(ReferencesVocabulary):
     """Pictograms vocabulary"""
 
-    def __init__(self, context=None):
-        table = query_utility(IPictogramTable)
-        if table is not None:
-            request = check_request()
-            terms = [
-                SimpleTerm(v.__name__,
-                           title=II18n(v).query_attribute('title', request=request))
-                for v in table.values()
-            ]
-        else:
-            terms = []
-        super(PictogramsVocabulary, self).__init__(terms)
+    table_interface = IPictogramTable
```

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/pictogram/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/reference/pictogram/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/pictogram/manager.py` & `pyams_content-1.99.2/src/pyams_content/reference/pictogram/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from pyramid.httpexceptions import HTTPNotFound
 from pyramid.renderers import render, render_to_response
 from pyramid.response import Response
 from pyramid.view import view_config
 from zope.interface import Interface
 
-from pyams_content.interfaces import MANAGE_SITE_ROOT_PERMISSION
+from pyams_content.interfaces import MANAGE_REFERENCE_TABLE_PERMISSION
 from pyams_content.reference.pictogram import IPictogram, IPictogramTable
 from pyams_content.reference.pictogram.zmi.table import PictogramTableContainerTable
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
 from pyams_form.interfaces.form import IAJAXFormRenderer
 from pyams_i18n.interfaces import II18n
 from pyams_layer.interfaces import IPyAMSLayer
@@ -51,25 +51,25 @@
 
 from pyams_content import _
 
 
 @viewlet_config(name='add-pictogram.menu',
                 context=IPictogramTable, layer=IAdminLayer, view=PictogramTableContainerTable,
                 manager=IToolbarViewletManager, weight=10,
-                permission=MANAGE_SITE_ROOT_PERMISSION)
+                permission=MANAGE_REFERENCE_TABLE_PERMISSION)
 class PictogramAddAction(ContextAddAction):
     """Pictogram add action"""
 
     label = _("Add pictogram")
     href = 'add-pictogram.html'
 
 
 @ajax_form_config(name='add-pictogram.html',
                   context=IPictogramTable, layer=IPyAMSLayer,
-                  permission=MANAGE_SITE_ROOT_PERMISSION)
+                  permission=MANAGE_REFERENCE_TABLE_PERMISSION)
 class PictogramAddForm(AdminModalAddForm):
     """Pictogram add form"""
 
     subtitle = _("New pictogram")
     legend = _("New pictogram properties")
     modal_class = 'modal-xl'
```

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/manager.py` & `pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/table.py` & `pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/table.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from pyams_pagelet.pagelet import pagelet_config
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_table.interfaces import IColumn
 from pyams_utils.adapter import adapter_config
 from pyams_utils.interfaces import MISSING_INFO
 from pyams_viewlet.manager import viewletmanager_config
 from pyams_zmi.interfaces import IAdminLayer, IObjectLabel
+from pyams_zmi.interfaces.form import IFormTitle, IPropertiesEditForm
 from pyams_zmi.interfaces.viewlet import IPropertiesMenu, ISiteManagementMenu
 from pyams_zmi.table import ActionColumn, TableAdminView
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
 __docformat__ = 'restructuredtext'
 
 from pyams_content import _
@@ -95,9 +96,18 @@
 @pagelet_config(name='contents.html',
                 context=IPictogramTable, layer=IPyAMSLayer,
                 permission=VIEW_SYSTEM_PERMISSION)
 class PictogramTableContentsView(TableAdminView):
     """Pictograms table contents view"""
 
     title = _("Pictograms")
+
     table_class = PictogramTableContainerTable
     table_label = _("Pictograms list")
+
+
+@adapter_config(required=(IPictogramTable, IAdminLayer, IPropertiesEditForm),
+                provides=IFormTitle)
+def pictograms_table_title(context, request, form):
+    """Pictograms table edit form title getter"""
+    translate = request.localizer.translate
+    return translate(_("Pictograms table"))
```

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/__init__.py` & `pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/manager.py` & `pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt` & `pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/reference/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/zmi/table.py` & `pyams_content-1.99.2/src/pyams_content/reference/zmi/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 #
 
 """PyAMS_content.reference.zmi.table module
 
 This module defines generic components used to handle references tables properties.
 """
 from pyramid.view import view_config
-from zope.interface import Interface
+from zope.interface import Interface, implementer
 
-from pyams_content.interfaces import MANAGE_SITE_ROOT_PERMISSION
+from pyams_content.interfaces import MANAGE_REFERENCE_TABLE_PERMISSION
 from pyams_content.reference import IReferenceTable
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
 from pyams_i18n.interfaces import II18n
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_table.column import GetAttrColumn
 from pyams_table.interfaces import IColumn, IValues
 from pyams_utils.adapter import ContextRequestViewAdapter, adapter_config
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.form import AdminEditForm
 from pyams_zmi.helper.container import delete_container_element
 from pyams_zmi.interfaces import IAdminLayer
+from pyams_zmi.interfaces.form import IPropertiesEditForm
 from pyams_zmi.interfaces.viewlet import IMenuHeader, IPropertiesMenu, ISiteManagementMenu
 from pyams_zmi.table import I18nColumnMixin, Table, TrashColumn
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
-
 __docformat__ = 'restructuredtext'
 
 from pyams_content import _
 
 
 @viewlet_config(name='properties.menu',
                 context=IReferenceTable, layer=IAdminLayer,
@@ -52,22 +52,22 @@
 
     href = '#properties.html'
 
 
 @ajax_form_config(name='properties.html',
                   context=IReferenceTable, layer=IPyAMSLayer,
                   permission=VIEW_SYSTEM_PERMISSION)
+@implementer(IPropertiesEditForm)
 class ReferenceTablePropertiesEditForm(AdminEditForm):
     """Reference table properties edit form"""
 
-    title = _("Pictograms table")
     legend = _("Edit table properties")
 
     fields = Fields(IReferenceTable).omit('__parent__', '__name__')
-    edit_permission = MANAGE_SITE_ROOT_PERMISSION
+    edit_permission = MANAGE_REFERENCE_TABLE_PERMISSION
 
 
 @adapter_config(required=(IReferenceTable, IAdminLayer, Interface, ISiteManagementMenu),
                 provides=IMenuHeader)
 def reference_table_site_management_menu_header(context, request, view, manager):
     """Reference table site management menu header adapter"""
     return _("Table management")
@@ -107,16 +107,17 @@
 
 @adapter_config(name='trash',
                 required=(IReferenceTable, IAdminLayer, ReferenceTableContainerTable),
                 provides=IColumn)
 class ReferenceTableTrashColumn(TrashColumn):
     """Reference table trash column"""
 
-    permission = MANAGE_SITE_ROOT_PERMISSION
+    permission = MANAGE_REFERENCE_TABLE_PERMISSION
 
 
 @view_config(name='delete-element.json',
              context=IReferenceTable, request_type=IPyAMSLayer,
-             permission=MANAGE_SITE_ROOT_PERMISSION, renderer='json', xhr=True)
+             permission=MANAGE_REFERENCE_TABLE_PERMISSION,
+             renderer='json', xhr=True)
 def delete_table_element(request):
     """Reference table delete view"""
     return delete_container_element(request)
```

### Comparing `pyams_content-1.99.1/src/pyams_content/reference/zmi/viewlet/__init__.py` & `pyams_content-1.99.2/src/pyams_content/reference/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/root/__init__.py` & `pyams_content-1.99.2/src/pyams_content/root/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/root/configuration.py` & `pyams_content-1.99.2/src/pyams_content/root/configuration.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/root/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/root/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/root/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/root/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/root/zmi/dashboard.py` & `pyams_content-1.99.2/src/pyams_content/root/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/root/zmi/search.py` & `pyams_content-1.99.2/src/pyams_content/root/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/root/zmi/sites.py` & `pyams_content-1.99.2/src/pyams_content/root/zmi/sites.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/alert/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/topic/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,59 @@
 #
-# Copyright (c) 2015-2023 Thierry Florac <tflorac AT ulthar.net>
+# Copyright (c) 2015-2021 Thierry Florac <tflorac AT ulthar.net>
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 
-"""PyAMS_content.shared.alert module
+"""PyAMS_content.shared.topic module
 
-This module defines alerts persistent classes.
 """
 
 from zope.interface import implementer
 from zope.schema.fieldproperty import FieldProperty
 
-from pyams_content.component.thesaurus import ITagsTarget, IThemesTarget
+from pyams_content.component.illustration.interfaces import IIllustrationTarget, \
+    ILinkIllustrationTarget
+from pyams_content.component.paragraph.interfaces import IParagraphContainerTarget
+from pyams_content.component.thesaurus.interfaces import ITagsTarget, IThemesTarget
+from pyams_content.feature.preview.interfaces import IPreviewTarget
 from pyams_content.feature.review import IReviewTarget
-from pyams_content.shared.alert.interfaces import ALERT_CONTENT_NAME, ALERT_CONTENT_TYPE, IAlert, IAlertManager, \
-    IAlertTypesManager, IWfAlert
-from pyams_content.shared.common import ISharedContent, IWfSharedContent, SharedContent, WfSharedContent
-from pyams_sequence.reference import InternalReferenceMixin, get_reference_target
+from pyams_content.shared.common import ISharedContent, IWfSharedContent, SharedContent, \
+    WfSharedContent
+from pyams_content.shared.common.types import WfTypedSharedContentMixin
+from pyams_content.shared.topic.interfaces import ITopic, IWfTopic, TOPIC_CONTENT_NAME, \
+    TOPIC_CONTENT_TYPE
 from pyams_utils.factory import factory_config
-from pyams_utils.request import check_request
-from pyams_utils.traversing import get_parent
+
 
 __docformat__ = 'restructuredtext'
 
 
-@factory_config(IWfAlert)
-@factory_config(IWfSharedContent, name=ALERT_CONTENT_TYPE)
-@implementer(ITagsTarget, IThemesTarget, IReviewTarget)
-class WfAlert(WfSharedContent, InternalReferenceMixin):
-    """Base alert"""
-
-    content_type = ALERT_CONTENT_TYPE
-    content_name = ALERT_CONTENT_NAME
-    content_intf = IWfAlert
-    content_view = False
-
-    handle_content_url = False
-    handle_header = False
-    handle_description = False
-
-    alert_type = FieldProperty(IWfAlert['alert_type'])
-    body = FieldProperty(IWfAlert['body'])
-    _reference = FieldProperty(IWfAlert['reference'])
-    external_url = FieldProperty(IWfAlert['external_url'])
-    references = FieldProperty(IWfAlert['references'])
-    maximum_interval = FieldProperty(IWfAlert['maximum_interval'])
-
-    def get_alert_type(self):
-        """Alert type getter"""
-        manager = get_parent(self, IAlertManager)
-        types = IAlertTypesManager(manager, None)
-        if types is not None:
-            return types.get(self.alert_type)
-
-    @property
-    def reference(self):
-        return self._reference
-
-    @reference.setter
-    def reference(self, value):
-        self._reference = value
-        del self.target
-
-    def get_targets(self, state=None):
-        request = check_request()
-        return [
-            get_reference_target(reference, state, request)
-            for reference in (self.references or ())
-        ]
-
-
-@factory_config(IAlert)
-@factory_config(ISharedContent, name=ALERT_CONTENT_TYPE)
-class Alert(SharedContent):
-    """Workflow managed alert class"""
-
-    content_type = ALERT_CONTENT_TYPE
-    content_name = ALERT_CONTENT_NAME
-    content_view = False
+@factory_config(IWfTopic)
+@factory_config(IWfSharedContent, name=TOPIC_CONTENT_TYPE)
+@implementer(IIllustrationTarget, ILinkIllustrationTarget, IParagraphContainerTarget,
+             ITagsTarget, IThemesTarget, IReviewTarget, IPreviewTarget)
+class WfTopic(WfSharedContent, WfTypedSharedContentMixin):
+    """Base topic"""
+
+    content_type = TOPIC_CONTENT_TYPE
+    content_name = TOPIC_CONTENT_NAME
+    content_intf = IWfTopic
+    content_view = True
+
+    references = FieldProperty(IWfTopic['references'])
+    data_type = FieldProperty(IWfTopic['data_type'])
+
+
+@factory_config(ITopic)
+@factory_config(ISharedContent, name=TOPIC_CONTENT_TYPE)
+class Topic(SharedContent):
+    """Workflow managed topic class"""
+
+    content_type = TOPIC_CONTENT_TYPE
+    content_name = TOPIC_CONTENT_NAME
```

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/alert/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/shared/alert/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/alert/manager.py` & `pyams_content-1.99.2/src/pyams_content/shared/alert/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/alert/types.py` & `pyams_content-1.99.2/src/pyams_content/shared/alert/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/alert/zmi/types.py` & `pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/blog/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/blog/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/calendar/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/interfaces/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/interfaces/types.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/interfaces/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/manager.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portal.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portal.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/header.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/header.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/specificities.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/skin/title.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/specificities.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/title.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/header.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/specificities.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/portlet/zmi/title.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/restrictions.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/restrictions.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/security.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/security.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from pyams_security.utility import get_principal
 from pyams_utils.adapter import ContextAdapter, adapter_config
 from pyams_utils.vocabulary import vocabulary_config
 
 __docformat__ = 'restructuredtext'
 
 
-
 @implementer(ISharedToolRoles)
 class SharedToolRoles(ProtectedObjectRoles):
     """Shared tool roles"""
 
     webmasters = RolePrincipalsFieldProperty(ISharedToolRoles['webmasters'])
     pilots = RolePrincipalsFieldProperty(ISharedToolRoles['pilots'])
     managers = RolePrincipalsFieldProperty(ISharedToolRoles['managers'])
```

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/skin/breadcrumb.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/skin/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/skin/oid.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/skin/oid.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/skin/specificities.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/skin/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/skin/title.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/skin/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/skin/types.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/skin/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/skin/url.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/skin/url.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/skin/workflow.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/skin/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/types.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/content.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/content.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/dashboard.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/header.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/manager.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/owner.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/owner.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/portal.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/portal.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/reference.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/restrictions.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/restrictions.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/search.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/summary.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/summary.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/quick-search.pt` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/quick-search.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/container.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 __docformat__ = 'restructuredtext'
 
 from pyams_content import _
 
 
 @viewlet_config(name='data-types.menu',
                 context=ITypedSharedTool, layer=IAdminLayer,
-                manager=IPropertiesMenu, weight=400,
+                manager=IPropertiesMenu, weight=405,
                 permission=MANAGE_TOOL_PERMISSION)
 class SharedToolTypesMenu(NavigationMenuItem):
     """Shared tool data types menu"""
 
     label = _("Content types")
     href = '#data-types.html'
```

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/content.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/content.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/types/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/viewlet/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/common/zmi/workflow.py` & `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/file/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/file/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/form/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/form/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/form/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/shared/form/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/form/manager.py` & `pyams_content-1.99.2/src/pyams_content/shared/form/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/form/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/form/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/form/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/form/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/hub/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/logo/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/logo/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/container.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/folder.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/link.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/link.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/manager.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/topic.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/topic.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/folder.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/link.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/link.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/manager.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/rename.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/rename.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/search.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/topic.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/topic.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/tree.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/tree.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/viewlet/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/folder.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt` & `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/topic/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/shared/topic/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/topic/manager.py` & `pyams_content-1.99.2/src/pyams_content/shared/topic/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/topic/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/topic/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/query.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/query.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/interfaces/settings.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/settings.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/manager.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/merge.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/merge.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt` & `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt` & `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt` & `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/skin/zmi.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/zmi.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt` & `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/query.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/query.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/reference.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/thesaurus.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/zmi/references.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/zmi/references.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/shared/view/zmi/thesaurus.py` & `pyams_content-1.99.2/src/pyams_content/shared/view/zmi/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/skin/__init__.py` & `pyams_content-1.99.2/src/pyams_content/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/skin/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/tests/__init__.py` & `pyams_content-1.99.2/src/pyams_content/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/tests/test_utilsdocs.py` & `pyams_content-1.99.2/src/pyams_content/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/tests/test_utilsdocstrings.py` & `pyams_content-1.99.2/src/pyams_content/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/utils/__init__.py` & `pyams_content-1.99.2/src/pyams_content/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/workflow/__init__.py` & `pyams_content-1.99.2/src/pyams_content/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/workflow/basic.py` & `pyams_content-1.99.2/src/pyams_content/workflow/basic.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/workflow/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/workflow/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/workflow/notify.py` & `pyams_content-1.99.2/src/pyams_content/workflow/notify.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/workflow/task.py` & `pyams_content-1.99.2/src/pyams_content/workflow/task.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/workflow/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/workflow/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/workflow/zmi/publication.py` & `pyams_content-1.99.2/src/pyams_content/workflow/zmi/publication.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/workflow/zmi/task.py` & `pyams_content-1.99.2/src/pyams_content/workflow/zmi/task.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/__init__.py` & `pyams_content-1.99.2/src/pyams_content/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/dashboard.py` & `pyams_content-1.99.2/src/pyams_content/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/html.py` & `pyams_content-1.99.2/src/pyams_content/zmi/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/properties.py` & `pyams_content-1.99.2/src/pyams_content/zmi/properties.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/resources/js/content.js` & `pyams_content-1.99.2/src/pyams_content/zmi/resources/js/content.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/resources/js/content.min.js` & `pyams_content-1.99.2/src/pyams_content/zmi/resources/js/content.min.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js` & `pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js` & `pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js` & `pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/viewlet/__init__.py` & `pyams_content-1.99.2/src/pyams_content/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/viewlet/toplinks.py` & `pyams_content-1.99.2/src/pyams_content/zmi/viewlet/toplinks.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/widget/__init__.py` & `pyams_content-1.99.2/src/pyams_content/zmi/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/widget/interfaces.py` & `pyams_content-1.99.2/src/pyams_content/zmi/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/widget/seo.py` & `pyams_content-1.99.2/src/pyams_content/zmi/widget/seo.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content/zmi/widget/templates/seo-textline-input.pt` & `pyams_content-1.99.2/src/pyams_content/zmi/widget/templates/seo-textline-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content.egg-info/PKG-INFO` & `pyams_content-1.99.2/src/pyams_content.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-content
-Version: 1.99.1
+Version: 1.99.2
 Summary: PyAMS content management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS CMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -48,14 +48,24 @@
 Please note that PyAMS_content only provide a basic Bootstrap based skin, so you will have to
 include other extension packages (like PyAMS_content_themes) to get more advanced graphical themes.
 
 
 Changelog
 =========
 
+1.99.2
+------
+ - added permission and role to manage references tables
+ - disable cache when using aggregated search results portlet renderer
+ - always open switcher in associations paragraph
+ - added method to paragraphs container to get iterator over paragraphs matching a given set of factories
+ - removed required flag on gallery files author
+ - updated menus order
+ - formatting and other minor updates
+
 1.99.1
 ------
  - added edit forms content getters
  - added alerts types
  - added vocabulary to handle shared contents which can be used by views and search folders
  - minor updates
```

### Comparing `pyams_content-1.99.1/src/pyams_content.egg-info/SOURCES.txt` & `pyams_content-1.99.2/src/pyams_content.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.1/src/pyams_content.egg-info/requires.txt` & `pyams_content-1.99.2/src/pyams_content.egg-info/requires.txt`

 * *Files identical despite different names*

