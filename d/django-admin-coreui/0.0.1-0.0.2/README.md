# Comparing `tmp/django-admin-coreui-0.0.1.tar.gz` & `tmp/django-admin-coreui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-coreui-0.0.1.tar", last modified: Sun Apr 28 06:12:08 2024, max compression
+gzip compressed data, was "django-admin-coreui-0.0.2.tar", last modified: Sun Apr 28 06:16:49 2024, max compression
```

## Comparing `django-admin-coreui-0.0.1.tar` & `django-admin-coreui-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 06:12:08.233681 django-admin-coreui-0.0.1/
--rw-rw-rw-   0        0        0     1113 2022-12-05 15:06:59.000000 django-admin-coreui-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0      150 2022-12-05 15:14:11.000000 django-admin-coreui-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7442 2024-04-28 06:12:08.232723 django-admin-coreui-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6350 2024-04-28 06:09:28.000000 django-admin-coreui-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 06:12:08.185171 django-admin-coreui-0.0.1/django_admin_coreui/
--rw-rw-rw-   0        0        0        0 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.1/django_admin_coreui/__init__.py
--rw-rw-rw-   0        0        0       66 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.1/django_admin_coreui/admin.py
--rw-rw-rw-   0        0        0      174 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.1/django_admin_coreui/apps.py
--rw-rw-rw-   0        0        0     2623 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.1/django_admin_coreui/forms.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:12:08.225463 django-admin-coreui-0.0.1/django_admin_coreui/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.1/django_admin_coreui/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.1/django_admin_coreui/models.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:12:08.230683 django-admin-coreui-0.0.1/django_admin_coreui/templatetags/
--rw-rw-rw-   0        0        0        0 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.1/django_admin_coreui/templatetags/__init__.py
--rw-rw-rw-   0        0        0     2558 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.1/django_admin_coreui/templatetags/admin_coreui.py
--rw-rw-rw-   0        0        0      237 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.1/django_admin_coreui/templatetags/replace_value.py
--rw-rw-rw-   0        0        0       63 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.1/django_admin_coreui/tests.py
--rw-rw-rw-   0        0        0     3485 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.1/django_admin_coreui/urls.py
--rw-rw-rw-   0        0        0    16587 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.1/django_admin_coreui/utils.py
--rw-rw-rw-   0        0        0     5786 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.1/django_admin_coreui/views.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:12:08.223486 django-admin-coreui-0.0.1/django_admin_coreui.egg-info/
--rw-rw-rw-   0        0        0     7442 2024-04-28 06:12:07.000000 django-admin-coreui-0.0.1/django_admin_coreui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      705 2024-04-28 06:12:08.000000 django-admin-coreui-0.0.1/django_admin_coreui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 06:12:07.000000 django-admin-coreui-0.0.1/django_admin_coreui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-28 06:12:07.000000 django-admin-coreui-0.0.1/django_admin_coreui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2024-04-28 06:12:08.000000 django-admin-coreui-0.0.1/django_admin_coreui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 06:12:08.233681 django-admin-coreui-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1340 2024-04-28 06:05:33.000000 django-admin-coreui-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:16:49.855433 django-admin-coreui-0.0.2/
+-rw-rw-rw-   0        0        0     1113 2022-12-05 15:06:59.000000 django-admin-coreui-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0      150 2022-12-05 15:14:11.000000 django-admin-coreui-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7415 2024-04-28 06:16:49.854290 django-admin-coreui-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6323 2024-04-28 06:13:31.000000 django-admin-coreui-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 06:16:49.789312 django-admin-coreui-0.0.2/django_admin_coreui/
+-rw-rw-rw-   0        0        0        0 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.2/django_admin_coreui/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.2/django_admin_coreui/admin.py
+-rw-rw-rw-   0        0        0      174 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.2/django_admin_coreui/apps.py
+-rw-rw-rw-   0        0        0     2623 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.2/django_admin_coreui/forms.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:16:49.846247 django-admin-coreui-0.0.2/django_admin_coreui/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.2/django_admin_coreui/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2024-04-28 06:02:41.000000 django-admin-coreui-0.0.2/django_admin_coreui/models.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:16:49.851260 django-admin-coreui-0.0.2/django_admin_coreui/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.2/django_admin_coreui/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     2558 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.2/django_admin_coreui/templatetags/admin_coreui.py
+-rw-rw-rw-   0        0        0      237 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.2/django_admin_coreui/templatetags/replace_value.py
+-rw-rw-rw-   0        0        0       63 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.2/django_admin_coreui/tests.py
+-rw-rw-rw-   0        0        0     3485 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.2/django_admin_coreui/urls.py
+-rw-rw-rw-   0        0        0    16587 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.2/django_admin_coreui/utils.py
+-rw-rw-rw-   0        0        0     5786 2024-04-28 06:03:10.000000 django-admin-coreui-0.0.2/django_admin_coreui/views.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:16:49.842733 django-admin-coreui-0.0.2/django_admin_coreui.egg-info/
+-rw-rw-rw-   0        0        0     7415 2024-04-28 06:16:49.000000 django-admin-coreui-0.0.2/django_admin_coreui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2024-04-28 06:16:49.000000 django-admin-coreui-0.0.2/django_admin_coreui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 06:16:49.000000 django-admin-coreui-0.0.2/django_admin_coreui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-28 06:12:07.000000 django-admin-coreui-0.0.2/django_admin_coreui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2024-04-28 06:16:49.000000 django-admin-coreui-0.0.2/django_admin_coreui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 06:16:49.855433 django-admin-coreui-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2024-04-28 06:14:02.000000 django-admin-coreui-0.0.2/setup.py
```

### Comparing `django-admin-coreui-0.0.1/LICENSE.md` & `django-admin-coreui-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.1/PKG-INFO` & `django-admin-coreui-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-coreui
-Version: 0.0.1
+Version: 0.0.2
 Summary: Modern template for Django admin interface
 Home-page: https://appseed.us/product/coreui/django/
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -31,17 +31,17 @@
 
 > Actively supported by [AppSeed](https://appseed.us/) via `Email` and `Discord`.
 
 <br>
 
 **Links & Resources**
 
-- [Django CoreUI](https://appseed.us/product/adminlte/django/) - `Product` that uses the library
+- [Django CoreUI](https://appseed.us/product/coreui/django/) - `Product` that uses the library
   - `Features`: Fully-configured, `CI/CD` via Render
-- UI Kit: `AdminLTE` by ColorLib **v3.2.0**
+- UI Kit: `CoreUI`
 - **Sections Covered**: 
   - `Admin Section`, reserved for `superusers`
   - `All pages` managed by `Django.contrib.AUTH`
   - `Registration` page
   - `Misc pages`: colors, icons, typography, blank-page 
 
 <br />
```

### Comparing `django-admin-coreui-0.0.1/README.md` & `django-admin-coreui-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 > Actively supported by [AppSeed](https://appseed.us/) via `Email` and `Discord`.
 
 <br>
 
 **Links & Resources**
 
-- [Django CoreUI](https://appseed.us/product/adminlte/django/) - `Product` that uses the library
+- [Django CoreUI](https://appseed.us/product/coreui/django/) - `Product` that uses the library
   - `Features`: Fully-configured, `CI/CD` via Render
-- UI Kit: `AdminLTE` by ColorLib **v3.2.0**
+- UI Kit: `CoreUI`
 - **Sections Covered**: 
   - `Admin Section`, reserved for `superusers`
   - `All pages` managed by `Django.contrib.AUTH`
   - `Registration` page
   - `Misc pages`: colors, icons, typography, blank-page 
 
 <br />
```

### Comparing `django-admin-coreui-0.0.1/django_admin_coreui/forms.py` & `django-admin-coreui-0.0.2/django_admin_coreui/forms.py`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.1/django_admin_coreui/templatetags/admin_coreui.py` & `django-admin-coreui-0.0.2/django_admin_coreui/templatetags/admin_coreui.py`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.1/django_admin_coreui/urls.py` & `django-admin-coreui-0.0.2/django_admin_coreui/urls.py`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.1/django_admin_coreui/utils.py` & `django-admin-coreui-0.0.2/django_admin_coreui/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.1/django_admin_coreui/views.py` & `django-admin-coreui-0.0.2/django_admin_coreui/views.py`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.1/django_admin_coreui.egg-info/PKG-INFO` & `django-admin-coreui-0.0.2/django_admin_coreui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-coreui
-Version: 0.0.1
+Version: 0.0.2
 Summary: Modern template for Django admin interface
 Home-page: https://appseed.us/product/coreui/django/
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -31,17 +31,17 @@
 
 > Actively supported by [AppSeed](https://appseed.us/) via `Email` and `Discord`.
 
 <br>
 
 **Links & Resources**
 
-- [Django CoreUI](https://appseed.us/product/adminlte/django/) - `Product` that uses the library
+- [Django CoreUI](https://appseed.us/product/coreui/django/) - `Product` that uses the library
   - `Features`: Fully-configured, `CI/CD` via Render
-- UI Kit: `AdminLTE` by ColorLib **v3.2.0**
+- UI Kit: `CoreUI`
 - **Sections Covered**: 
   - `Admin Section`, reserved for `superusers`
   - `All pages` managed by `Django.contrib.AUTH`
   - `Registration` page
   - `Misc pages`: colors, icons, typography, blank-page 
 
 <br />
```

### Comparing `django-admin-coreui-0.0.1/django_admin_coreui.egg-info/SOURCES.txt` & `django-admin-coreui-0.0.2/django_admin_coreui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-coreui-0.0.1/setup.py` & `django-admin-coreui-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
 name='django-admin-coreui',
-version='0.0.1',
+version='0.0.2',
 zip_safe=False,
 packages=find_packages(),
 include_package_data=True,
 description='Modern template for Django admin interface',
 long_description=README,
 long_description_content_type="text/markdown",
 url='https://appseed.us/product/coreui/django/',
```

