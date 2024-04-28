# Comparing `tmp/django-thumbor-0.5.7.tar.gz` & `tmp/django_thumbor-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-thumbor-0.5.7.tar", last modified: Sun Dec 10 16:34:34 2017, max compression
+gzip compressed data, was "django_thumbor-0.6.0.tar", last modified: Sun Apr 28 21:21:16 2024, max compression
```

## Comparing `django-thumbor-0.5.7.tar` & `django_thumbor-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 enrico.luz   (502) staff       (20)        0 2017-12-10 16:34:34.000000 django-thumbor-0.5.7/
-drwxr-xr-x   0 enrico.luz   (502) staff       (20)        0 2017-12-10 16:34:34.000000 django-thumbor-0.5.7/django_thumbor/
--rw-r--r--   0 enrico.luz   (502) staff       (20)     2243 2016-10-25 11:28:49.000000 django-thumbor-0.5.7/django_thumbor/__init__.py
--rw-r--r--   0 enrico.luz   (502) staff       (20)     1143 2016-10-25 11:28:49.000000 django-thumbor-0.5.7/django_thumbor/conf.py
-drwxr-xr-x   0 enrico.luz   (502) staff       (20)        0 2017-12-10 16:34:34.000000 django-thumbor-0.5.7/django_thumbor/templatetags/
--rw-r--r--   0 enrico.luz   (502) staff       (20)        0 2016-07-16 21:07:28.000000 django-thumbor-0.5.7/django_thumbor/templatetags/__init__.py
--rw-r--r--   0 enrico.luz   (502) staff       (20)     1227 2017-12-10 16:04:56.000000 django-thumbor-0.5.7/django_thumbor/templatetags/thumbor_tags.py
-drwxr-xr-x   0 enrico.luz   (502) staff       (20)        0 2017-12-10 16:34:34.000000 django-thumbor-0.5.7/django_thumbor.egg-info/
--rw-r--r--   0 enrico.luz   (502) staff       (20)        1 2017-12-10 16:34:34.000000 django-thumbor-0.5.7/django_thumbor.egg-info/dependency_links.txt
--rw-r--r--   0 enrico.luz   (502) staff       (20)     7513 2017-12-10 16:34:34.000000 django-thumbor-0.5.7/django_thumbor.egg-info/PKG-INFO
--rw-r--r--   0 enrico.luz   (502) staff       (20)       30 2017-12-10 16:34:34.000000 django-thumbor-0.5.7/django_thumbor.egg-info/requires.txt
--rw-r--r--   0 enrico.luz   (502) staff       (20)      354 2017-12-10 16:34:34.000000 django-thumbor-0.5.7/django_thumbor.egg-info/SOURCES.txt
--rw-r--r--   0 enrico.luz   (502) staff       (20)       15 2017-12-10 16:34:34.000000 django-thumbor-0.5.7/django_thumbor.egg-info/top_level.txt
--rw-r--r--   0 enrico.luz   (502) staff       (20)       39 2016-07-16 21:07:28.000000 django-thumbor-0.5.7/MANIFEST.in
--rw-r--r--   0 enrico.luz   (502) staff       (20)     7513 2017-12-10 16:34:34.000000 django-thumbor-0.5.7/PKG-INFO
--rw-r--r--   0 enrico.luz   (502) staff       (20)     5429 2016-10-25 11:28:49.000000 django-thumbor-0.5.7/README.rst
--rw-r--r--   0 enrico.luz   (502) staff       (20)       38 2017-12-10 16:34:34.000000 django-thumbor-0.5.7/setup.cfg
--rw-r--r--   0 enrico.luz   (502) staff       (20)      824 2017-12-10 16:33:21.000000 django-thumbor-0.5.7/setup.py
+drwxr-xr-x   0 enrico.luz   (502) staff       (20)        0 2024-04-28 21:21:16.759275 django_thumbor-0.6.0/
+-rw-r--r--   0 enrico.luz   (502) staff       (20)     1088 2022-01-28 09:49:52.000000 django_thumbor-0.6.0/LICENSE
+-rw-r--r--   0 enrico.luz   (502) staff       (20)       39 2022-01-28 09:49:52.000000 django_thumbor-0.6.0/MANIFEST.in
+-rw-r--r--   0 enrico.luz   (502) staff       (20)     5764 2024-04-28 21:21:16.758942 django_thumbor-0.6.0/PKG-INFO
+-rw-r--r--   0 enrico.luz   (502) staff       (20)     5279 2024-04-28 20:33:10.000000 django_thumbor-0.6.0/README.rst
+drwxr-xr-x   0 enrico.luz   (502) staff       (20)        0 2024-04-28 21:21:16.756289 django_thumbor-0.6.0/django_thumbor/
+-rw-r--r--   0 enrico.luz   (502) staff       (20)     2243 2022-01-28 10:39:29.000000 django_thumbor-0.6.0/django_thumbor/__init__.py
+-rw-r--r--   0 enrico.luz   (502) staff       (20)     1143 2022-01-28 10:40:03.000000 django_thumbor-0.6.0/django_thumbor/conf.py
+drwxr-xr-x   0 enrico.luz   (502) staff       (20)        0 2024-04-28 21:21:16.758059 django_thumbor-0.6.0/django_thumbor/templatetags/
+-rw-r--r--   0 enrico.luz   (502) staff       (20)        0 2022-01-28 09:49:52.000000 django_thumbor-0.6.0/django_thumbor/templatetags/__init__.py
+-rw-r--r--   0 enrico.luz   (502) staff       (20)     1227 2022-01-28 09:49:52.000000 django_thumbor-0.6.0/django_thumbor/templatetags/thumbor_tags.py
+drwxr-xr-x   0 enrico.luz   (502) staff       (20)        0 2024-04-28 21:21:16.758540 django_thumbor-0.6.0/django_thumbor.egg-info/
+-rw-r--r--   0 enrico.luz   (502) staff       (20)     5764 2024-04-28 21:21:16.000000 django_thumbor-0.6.0/django_thumbor.egg-info/PKG-INFO
+-rw-r--r--   0 enrico.luz   (502) staff       (20)      362 2024-04-28 21:21:16.000000 django_thumbor-0.6.0/django_thumbor.egg-info/SOURCES.txt
+-rw-r--r--   0 enrico.luz   (502) staff       (20)        1 2024-04-28 21:21:16.000000 django_thumbor-0.6.0/django_thumbor.egg-info/dependency_links.txt
+-rw-r--r--   0 enrico.luz   (502) staff       (20)       30 2024-04-28 21:21:16.000000 django_thumbor-0.6.0/django_thumbor.egg-info/requires.txt
+-rw-r--r--   0 enrico.luz   (502) staff       (20)       15 2024-04-28 21:21:16.000000 django_thumbor-0.6.0/django_thumbor.egg-info/top_level.txt
+-rw-r--r--   0 enrico.luz   (502) staff       (20)       38 2024-04-28 21:21:16.759340 django_thumbor-0.6.0/setup.cfg
+-rw-r--r--   0 enrico.luz   (502) staff       (20)      824 2024-04-28 20:41:59.000000 django_thumbor-0.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-thumbor-0.5.7/django_thumbor/__init__.py` & `django_thumbor-0.6.0/django_thumbor/__init__.py`

 * *Files identical despite different names*

### Comparing `django-thumbor-0.5.7/django_thumbor/conf.py` & `django_thumbor-0.6.0/django_thumbor/conf.py`

 * *Files identical despite different names*

### Comparing `django-thumbor-0.5.7/django_thumbor/templatetags/thumbor_tags.py` & `django_thumbor-0.6.0/django_thumbor/templatetags/thumbor_tags.py`

 * *Files identical despite different names*

### Comparing `django-thumbor-0.5.7/django_thumbor.egg-info/PKG-INFO` & `django_thumbor-0.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,214 +1,216 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-thumbor
-Version: 0.5.7
+Version: 0.6.0
 Summary: A django application to resize images using the thumbor service
 Home-page: http://github.com/ricobl/django-thumbor/
 Author: Enrico Batista da Luz
 Author-email: rico.bl@gmail.com
 License: django-thumbor is licensed under the MIT license. For more information, please see LICENSE file.
-Description-Content-Type: UNKNOWN
-Description: django-thumbor
-        ==============
-        
-        .. image:: https://travis-ci.org/ricobl/django-thumbor.png?branch=master
-            :target: https://travis-ci.org/ricobl/django-thumbor
-            :alt: CI status on Travis CI
-        
-        .. image:: http://img.shields.io/pypi/v/django-thumbor.svg
-            :target: https://pypi.python.org/pypi/django-thumbor/
-            :alt: Latest django-thumbor PyPI version
-        
-        .. image:: https://img.shields.io/pypi/dm/django-thumbor.svg
-            :target: https://pypi.python.org/pypi/django-thumbor/
-            :alt: Number of downloads for django-thumbor on PyPI
-        
-        .. image:: https://coveralls.io/repos/ricobl/django-thumbor/badge.png?branch=master
-            :target: https://coveralls.io/r/ricobl/django-thumbor?branch=master
-            :alt: Code coverage on Coveralls
-        
-        .. image:: https://gemnasium.com/ricobl/django-thumbor.svg
-            :target: https://gemnasium.com/ricobl/django-thumbor
-            :alt: Dependency Status on Gemnasium
-        
-        
-        A django application to resize images using the
-        `thumbor <https://github.com/globocom/thumbor>`_ service.
-        
-        Usage
-        -----
-        
-        Both ``thumbor_url`` templatetag and the ``generate_url`` helper uses the same
-        arguments as `libthumbor <https://github.com/heynemann/libthumbor>`_, you can
-        check the `wiki <https://github.com/heynemann/libthumbor/wiki>`_ for more info.
-        
-        On templates:
-        
-        .. code-block:: html
-        
-            {% load thumbor_tags %}
-            <img src="{% thumbor_url '/media/image.jpg' width=300 %}" width="300" />
-        
-            or
-        
-            {% load thumbor_tags %}
-            <img src="{% thumbor_url model.image_field width=300 %}" width="300" />
-        
-        If you need the result in a template variable, use `assign_thumbor_url` instead.
-        
-            {% load thumbor_tags %}
-            {% assign_thumbor_url '/media/image.jpg' width=300 as thumb_url %}
-            <img src="{{ thumb_url }}" width="300" />
-        
-        **Filters**
-        
-        Split `filters <https://github.com/thumbor/thumbor/wiki/Filters>`_ with
-        ``:`` (or use a ``list`` object):
-        
-        .. code-block:: html
-        
-            {% load thumbor_tags %}
-            <img src="{% thumbor_url url filters='watermark(http://domain.com/watermark.png,-10,-10,20):brightness(10)' %}" />
-            <img src="{% thumbor_url url filters=filter_list %}" />
-        
-        On code:
-        
-        .. code-block:: python
-        
-            from django_thumbor import generate_url
-            resized = generate_url("/media/image.jpg", width=300)
-        
-        
-        **Re-using argument sets (aliases)**
-        
-        You can re-use argument sets through globally defined aliases. This prevents
-        repeating thumbnail parameters all over the code and can improve thumbor
-        performance because thumbnails are re-used as well. If you're migrating
-        from django-easy-thumbnails, you'll find the pattern very familiar, and it
-        should make porting much more straight-forward.
-        
-        On templates:
-        
-        .. code-block:: html
-        
-            {% load thumbor_tags %}
-            <img src="{% thumbor_url '/media/image.jpg' alias="thumb-square" %}" />
-        
-        On code:
-        
-        .. code-block:: python
-        
-            from django_thumbor import generate_url
-            resized = generate_url("/media/image.jpg", alias="thumb-square")
-        
-        And in your ``settings.py``:
-        
-        .. code-block:: python
-        
-            THUMBOR_ALIASES = {
-                'thumb-square': {
-                    'width': 300,
-                    'height': 300,
-                    'filters': ['brightness(10)']}
-            }
-        
-        
-        **Override server address**
-        
-        There is an extra parameter to specify a custom server to be used instead of
-        ``settings.THUMBOR_SERVER``.
-        
-        On templates:
-        
-        .. code-block:: html
-        
-            {% load thumbor_tags %}
-            <img src="{% thumbor_url '/media/image.jpg' thumbor_server='http://localhost:8888/foo' width=300 %}" width="300" />
-        
-        On code:
-        
-        .. code-block:: python
-        
-            from django_thumbor import generate_url
-            custom_server = "http://localhost:8888/foo"
-            resized = generate_url(
-                "/media/image.jpg", thumbor_server=custom_server, width=300)
-        
-        
-        Installation
-        ------------
-        
-        .. code-block:: bash
-        
-            pip install django-thumbor
-        
-        
-        Configuration
-        -------------
-        
-        Add the app to the ``INSTALLED_APPS``:
-        
-        .. code-block:: python
-        
-            INSTALLED_APPS = (
-                # ...
-                'django_thumbor',
-            )
-        
-        Here are the default settings that you can override:
-        
-        .. code-block:: python
-        
-            # The host serving the thumbor resized images
-            THUMBOR_SERVER = 'http://localhost:8888'
-        
-            # The prefix for the host serving the original images
-            # This must be a resolvable address to allow thumbor to reach the images
-            THUMBOR_MEDIA_URL = 'http://localhost:8000/media'
-        
-            # If you want the static to be handled by django thumbor
-            # default as False, set True to handle it if you host your statics
-            THUMBOR_STATIC_ENABLED = False
-        
-            # The prefix for the host serving the original static images
-            # this must be a resolvable address to allow thumbor to reach the images
-            THUMBOR_STATIC_URL = 'http://localhost:8000/static'
-        
-            # The same security key used in the thumbor service to
-            # match the URL construction
-            THUMBOR_SECURITY_KEY = 'MY_SECURE_KEY'
-        
-            # Default arguments passed to the `generate_url` helper or
-            # the `thumbor_url` templatetag
-            THUMBOR_ARGUMENTS = {}
-        
-            # An alias represents a named set of arguments to the generate_url function
-            # or thumbor_url template tag. Use it to share general thumbnail
-            # configurations without repeating yourself.
-            THUMBOR_ALIASES = {}
-        
-        
-        Contributing
-        ------------
-        
-        Install
-        .......
-        
-        Fork, clone, create a virtualenv and run:
-        
-        .. code-block:: bash
-        
-            git clone git://github.com/ricobl/django-thumbor.git
-            mkvirtualenv django-thumbor
-            make install
-        
-        Test
-        ....
-        
-        Add tests on ``testproject/tests``, add code and run:
-        
-        .. code-block:: bash
-        
-            make test
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE
+Requires-Dist: Django>=1.4
+Requires-Dist: libthumbor>=1.2.0
+
+django-thumbor
+==============
+
+.. image:: https://travis-ci.org/ricobl/django-thumbor.png?branch=master
+    :target: https://travis-ci.org/ricobl/django-thumbor
+    :alt: CI status on Travis CI
+
+.. image:: http://img.shields.io/pypi/v/django-thumbor.svg
+    :target: https://pypi.python.org/pypi/django-thumbor/
+    :alt: Latest django-thumbor PyPI version
+
+.. image:: https://img.shields.io/pypi/dm/django-thumbor.svg
+    :target: https://pypi.python.org/pypi/django-thumbor/
+    :alt: Number of downloads for django-thumbor on PyPI
+
+
+A django application to resize images using the
+`thumbor <https://github.com/globocom/thumbor>`_ service.
+
+Usage
+-----
+
+Both ``thumbor_url`` templatetag and the ``generate_url`` helper uses the same
+arguments as `libthumbor <https://github.com/heynemann/libthumbor>`_, you can
+check the `wiki <https://github.com/heynemann/libthumbor/wiki>`_ for more info.
+
+On templates:
+
+.. code-block:: html
+
+    {% load thumbor_tags %}
+    <img src="{% thumbor_url '/media/image.jpg' width=300 %}" width="300" />
+
+    or
+
+    {% load thumbor_tags %}
+    <img src="{% thumbor_url model.image_field width=300 %}" width="300" />
+
+If you need the result in a template variable, use `assign_thumbor_url` instead.
+
+    {% load thumbor_tags %}
+    {% assign_thumbor_url '/media/image.jpg' width=300 as thumb_url %}
+    <img src="{{ thumb_url }}" width="300" />
+
+**Filters**
+
+Split `filters <https://github.com/thumbor/thumbor/wiki/Filters>`_ with
+``:`` (or use a ``list`` object):
+
+.. code-block:: html
+
+    {% load thumbor_tags %}
+    <img src="{% thumbor_url url filters='watermark(http://domain.com/watermark.png,-10,-10,20):brightness(10)' %}" />
+    <img src="{% thumbor_url url filters=filter_list %}" />
+
+On code:
+
+.. code-block:: python
+
+    from django_thumbor import generate_url
+    resized = generate_url("/media/image.jpg", width=300)
+
+
+**Re-using argument sets (aliases)**
+
+You can re-use argument sets through globally defined aliases. This prevents
+repeating thumbnail parameters all over the code and can improve thumbor
+performance because thumbnails are re-used as well. If you're migrating
+from django-easy-thumbnails, you'll find the pattern very familiar, and it
+should make porting much more straight-forward.
+
+On templates:
+
+.. code-block:: html
+
+    {% load thumbor_tags %}
+    <img src="{% thumbor_url '/media/image.jpg' alias="thumb-square" %}" />
+
+On code:
+
+.. code-block:: python
+
+    from django_thumbor import generate_url
+    resized = generate_url("/media/image.jpg", alias="thumb-square")
+
+And in your ``settings.py``:
+
+.. code-block:: python
+
+    THUMBOR_ALIASES = {
+        'thumb-square': {
+            'width': 300,
+            'height': 300,
+            'filters': ['brightness(10)']}
+    }
+
+
+**Override server address**
+
+There is an extra parameter to specify a custom server to be used instead of
+``settings.THUMBOR_SERVER``.
+
+On templates:
+
+.. code-block:: html
+
+    {% load thumbor_tags %}
+    <img src="{% thumbor_url '/media/image.jpg' thumbor_server='http://localhost:8888/foo' width=300 %}" width="300" />
+
+On code:
+
+.. code-block:: python
+
+    from django_thumbor import generate_url
+    custom_server = "http://localhost:8888/foo"
+    resized = generate_url(
+        "/media/image.jpg", thumbor_server=custom_server, width=300)
+
+
+Installation
+------------
+
+.. code-block:: bash
+
+    pip install django-thumbor
+
+
+Configuration
+-------------
+
+Add the app to the ``INSTALLED_APPS``:
+
+.. code-block:: python
+
+    INSTALLED_APPS = (
+        # ...
+        'django_thumbor',
+    )
+
+Here are the default settings that you can override:
+
+.. code-block:: python
+
+    # The host serving the thumbor resized images
+    THUMBOR_SERVER = 'http://localhost:8888'
+
+    # The prefix for the host serving the original images
+    # This must be a resolvable address to allow thumbor to reach the images
+    THUMBOR_MEDIA_URL = 'http://localhost:8000/media'
+
+    # If you want the static to be handled by django thumbor
+    # default as False, set True to handle it if you host your statics
+    THUMBOR_STATIC_ENABLED = False
+
+    # The prefix for the host serving the original static images
+    # this must be a resolvable address to allow thumbor to reach the images
+    THUMBOR_STATIC_URL = 'http://localhost:8000/static'
+
+    # The same security key used in the thumbor service to
+    # match the URL construction
+    THUMBOR_SECURITY_KEY = 'MY_SECURE_KEY'
+
+    # Default arguments passed to the `generate_url` helper or
+    # the `thumbor_url` templatetag
+    THUMBOR_ARGUMENTS = {}
+
+    # An alias represents a named set of arguments to the generate_url function
+    # or thumbor_url template tag. Use it to share general thumbnail
+    # configurations without repeating yourself.
+    THUMBOR_ALIASES = {}
+
+
+Contributing
+------------
+
+Install
+.......
+
+Fork, clone, create a virtualenv and run:
+
+.. code-block:: bash
+
+    git clone git://github.com/ricobl/django-thumbor.git
+    cd django-thumbor
+    pipenv shell
+    make install
+
+Test
+....
+
+Add tests on ``testproject/tests``, add code and run:
+
+.. code-block:: bash
+
+    make test
+
+Test Server
+...........
+
+- Instal thumbor server: ``pip install thumbor``
+- Run thumbor: ``thumbor``
+- Run local server: ``make run``
+- visit `http://127.0.0.1:8000/ <http://127.0.0.1:8000/>`_:
```

### Comparing `django-thumbor-0.5.7/PKG-INFO` & `django_thumbor-0.6.0/django_thumbor.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,214 +1,216 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-thumbor
-Version: 0.5.7
+Version: 0.6.0
 Summary: A django application to resize images using the thumbor service
 Home-page: http://github.com/ricobl/django-thumbor/
 Author: Enrico Batista da Luz
 Author-email: rico.bl@gmail.com
 License: django-thumbor is licensed under the MIT license. For more information, please see LICENSE file.
-Description-Content-Type: UNKNOWN
-Description: django-thumbor
-        ==============
-        
-        .. image:: https://travis-ci.org/ricobl/django-thumbor.png?branch=master
-            :target: https://travis-ci.org/ricobl/django-thumbor
-            :alt: CI status on Travis CI
-        
-        .. image:: http://img.shields.io/pypi/v/django-thumbor.svg
-            :target: https://pypi.python.org/pypi/django-thumbor/
-            :alt: Latest django-thumbor PyPI version
-        
-        .. image:: https://img.shields.io/pypi/dm/django-thumbor.svg
-            :target: https://pypi.python.org/pypi/django-thumbor/
-            :alt: Number of downloads for django-thumbor on PyPI
-        
-        .. image:: https://coveralls.io/repos/ricobl/django-thumbor/badge.png?branch=master
-            :target: https://coveralls.io/r/ricobl/django-thumbor?branch=master
-            :alt: Code coverage on Coveralls
-        
-        .. image:: https://gemnasium.com/ricobl/django-thumbor.svg
-            :target: https://gemnasium.com/ricobl/django-thumbor
-            :alt: Dependency Status on Gemnasium
-        
-        
-        A django application to resize images using the
-        `thumbor <https://github.com/globocom/thumbor>`_ service.
-        
-        Usage
-        -----
-        
-        Both ``thumbor_url`` templatetag and the ``generate_url`` helper uses the same
-        arguments as `libthumbor <https://github.com/heynemann/libthumbor>`_, you can
-        check the `wiki <https://github.com/heynemann/libthumbor/wiki>`_ for more info.
-        
-        On templates:
-        
-        .. code-block:: html
-        
-            {% load thumbor_tags %}
-            <img src="{% thumbor_url '/media/image.jpg' width=300 %}" width="300" />
-        
-            or
-        
-            {% load thumbor_tags %}
-            <img src="{% thumbor_url model.image_field width=300 %}" width="300" />
-        
-        If you need the result in a template variable, use `assign_thumbor_url` instead.
-        
-            {% load thumbor_tags %}
-            {% assign_thumbor_url '/media/image.jpg' width=300 as thumb_url %}
-            <img src="{{ thumb_url }}" width="300" />
-        
-        **Filters**
-        
-        Split `filters <https://github.com/thumbor/thumbor/wiki/Filters>`_ with
-        ``:`` (or use a ``list`` object):
-        
-        .. code-block:: html
-        
-            {% load thumbor_tags %}
-            <img src="{% thumbor_url url filters='watermark(http://domain.com/watermark.png,-10,-10,20):brightness(10)' %}" />
-            <img src="{% thumbor_url url filters=filter_list %}" />
-        
-        On code:
-        
-        .. code-block:: python
-        
-            from django_thumbor import generate_url
-            resized = generate_url("/media/image.jpg", width=300)
-        
-        
-        **Re-using argument sets (aliases)**
-        
-        You can re-use argument sets through globally defined aliases. This prevents
-        repeating thumbnail parameters all over the code and can improve thumbor
-        performance because thumbnails are re-used as well. If you're migrating
-        from django-easy-thumbnails, you'll find the pattern very familiar, and it
-        should make porting much more straight-forward.
-        
-        On templates:
-        
-        .. code-block:: html
-        
-            {% load thumbor_tags %}
-            <img src="{% thumbor_url '/media/image.jpg' alias="thumb-square" %}" />
-        
-        On code:
-        
-        .. code-block:: python
-        
-            from django_thumbor import generate_url
-            resized = generate_url("/media/image.jpg", alias="thumb-square")
-        
-        And in your ``settings.py``:
-        
-        .. code-block:: python
-        
-            THUMBOR_ALIASES = {
-                'thumb-square': {
-                    'width': 300,
-                    'height': 300,
-                    'filters': ['brightness(10)']}
-            }
-        
-        
-        **Override server address**
-        
-        There is an extra parameter to specify a custom server to be used instead of
-        ``settings.THUMBOR_SERVER``.
-        
-        On templates:
-        
-        .. code-block:: html
-        
-            {% load thumbor_tags %}
-            <img src="{% thumbor_url '/media/image.jpg' thumbor_server='http://localhost:8888/foo' width=300 %}" width="300" />
-        
-        On code:
-        
-        .. code-block:: python
-        
-            from django_thumbor import generate_url
-            custom_server = "http://localhost:8888/foo"
-            resized = generate_url(
-                "/media/image.jpg", thumbor_server=custom_server, width=300)
-        
-        
-        Installation
-        ------------
-        
-        .. code-block:: bash
-        
-            pip install django-thumbor
-        
-        
-        Configuration
-        -------------
-        
-        Add the app to the ``INSTALLED_APPS``:
-        
-        .. code-block:: python
-        
-            INSTALLED_APPS = (
-                # ...
-                'django_thumbor',
-            )
-        
-        Here are the default settings that you can override:
-        
-        .. code-block:: python
-        
-            # The host serving the thumbor resized images
-            THUMBOR_SERVER = 'http://localhost:8888'
-        
-            # The prefix for the host serving the original images
-            # This must be a resolvable address to allow thumbor to reach the images
-            THUMBOR_MEDIA_URL = 'http://localhost:8000/media'
-        
-            # If you want the static to be handled by django thumbor
-            # default as False, set True to handle it if you host your statics
-            THUMBOR_STATIC_ENABLED = False
-        
-            # The prefix for the host serving the original static images
-            # this must be a resolvable address to allow thumbor to reach the images
-            THUMBOR_STATIC_URL = 'http://localhost:8000/static'
-        
-            # The same security key used in the thumbor service to
-            # match the URL construction
-            THUMBOR_SECURITY_KEY = 'MY_SECURE_KEY'
-        
-            # Default arguments passed to the `generate_url` helper or
-            # the `thumbor_url` templatetag
-            THUMBOR_ARGUMENTS = {}
-        
-            # An alias represents a named set of arguments to the generate_url function
-            # or thumbor_url template tag. Use it to share general thumbnail
-            # configurations without repeating yourself.
-            THUMBOR_ALIASES = {}
-        
-        
-        Contributing
-        ------------
-        
-        Install
-        .......
-        
-        Fork, clone, create a virtualenv and run:
-        
-        .. code-block:: bash
-        
-            git clone git://github.com/ricobl/django-thumbor.git
-            mkvirtualenv django-thumbor
-            make install
-        
-        Test
-        ....
-        
-        Add tests on ``testproject/tests``, add code and run:
-        
-        .. code-block:: bash
-        
-            make test
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE
+Requires-Dist: Django>=1.4
+Requires-Dist: libthumbor>=1.2.0
+
+django-thumbor
+==============
+
+.. image:: https://travis-ci.org/ricobl/django-thumbor.png?branch=master
+    :target: https://travis-ci.org/ricobl/django-thumbor
+    :alt: CI status on Travis CI
+
+.. image:: http://img.shields.io/pypi/v/django-thumbor.svg
+    :target: https://pypi.python.org/pypi/django-thumbor/
+    :alt: Latest django-thumbor PyPI version
+
+.. image:: https://img.shields.io/pypi/dm/django-thumbor.svg
+    :target: https://pypi.python.org/pypi/django-thumbor/
+    :alt: Number of downloads for django-thumbor on PyPI
+
+
+A django application to resize images using the
+`thumbor <https://github.com/globocom/thumbor>`_ service.
+
+Usage
+-----
+
+Both ``thumbor_url`` templatetag and the ``generate_url`` helper uses the same
+arguments as `libthumbor <https://github.com/heynemann/libthumbor>`_, you can
+check the `wiki <https://github.com/heynemann/libthumbor/wiki>`_ for more info.
+
+On templates:
+
+.. code-block:: html
+
+    {% load thumbor_tags %}
+    <img src="{% thumbor_url '/media/image.jpg' width=300 %}" width="300" />
+
+    or
+
+    {% load thumbor_tags %}
+    <img src="{% thumbor_url model.image_field width=300 %}" width="300" />
+
+If you need the result in a template variable, use `assign_thumbor_url` instead.
+
+    {% load thumbor_tags %}
+    {% assign_thumbor_url '/media/image.jpg' width=300 as thumb_url %}
+    <img src="{{ thumb_url }}" width="300" />
+
+**Filters**
+
+Split `filters <https://github.com/thumbor/thumbor/wiki/Filters>`_ with
+``:`` (or use a ``list`` object):
+
+.. code-block:: html
+
+    {% load thumbor_tags %}
+    <img src="{% thumbor_url url filters='watermark(http://domain.com/watermark.png,-10,-10,20):brightness(10)' %}" />
+    <img src="{% thumbor_url url filters=filter_list %}" />
+
+On code:
+
+.. code-block:: python
+
+    from django_thumbor import generate_url
+    resized = generate_url("/media/image.jpg", width=300)
+
+
+**Re-using argument sets (aliases)**
+
+You can re-use argument sets through globally defined aliases. This prevents
+repeating thumbnail parameters all over the code and can improve thumbor
+performance because thumbnails are re-used as well. If you're migrating
+from django-easy-thumbnails, you'll find the pattern very familiar, and it
+should make porting much more straight-forward.
+
+On templates:
+
+.. code-block:: html
+
+    {% load thumbor_tags %}
+    <img src="{% thumbor_url '/media/image.jpg' alias="thumb-square" %}" />
+
+On code:
+
+.. code-block:: python
+
+    from django_thumbor import generate_url
+    resized = generate_url("/media/image.jpg", alias="thumb-square")
+
+And in your ``settings.py``:
+
+.. code-block:: python
+
+    THUMBOR_ALIASES = {
+        'thumb-square': {
+            'width': 300,
+            'height': 300,
+            'filters': ['brightness(10)']}
+    }
+
+
+**Override server address**
+
+There is an extra parameter to specify a custom server to be used instead of
+``settings.THUMBOR_SERVER``.
+
+On templates:
+
+.. code-block:: html
+
+    {% load thumbor_tags %}
+    <img src="{% thumbor_url '/media/image.jpg' thumbor_server='http://localhost:8888/foo' width=300 %}" width="300" />
+
+On code:
+
+.. code-block:: python
+
+    from django_thumbor import generate_url
+    custom_server = "http://localhost:8888/foo"
+    resized = generate_url(
+        "/media/image.jpg", thumbor_server=custom_server, width=300)
+
+
+Installation
+------------
+
+.. code-block:: bash
+
+    pip install django-thumbor
+
+
+Configuration
+-------------
+
+Add the app to the ``INSTALLED_APPS``:
+
+.. code-block:: python
+
+    INSTALLED_APPS = (
+        # ...
+        'django_thumbor',
+    )
+
+Here are the default settings that you can override:
+
+.. code-block:: python
+
+    # The host serving the thumbor resized images
+    THUMBOR_SERVER = 'http://localhost:8888'
+
+    # The prefix for the host serving the original images
+    # This must be a resolvable address to allow thumbor to reach the images
+    THUMBOR_MEDIA_URL = 'http://localhost:8000/media'
+
+    # If you want the static to be handled by django thumbor
+    # default as False, set True to handle it if you host your statics
+    THUMBOR_STATIC_ENABLED = False
+
+    # The prefix for the host serving the original static images
+    # this must be a resolvable address to allow thumbor to reach the images
+    THUMBOR_STATIC_URL = 'http://localhost:8000/static'
+
+    # The same security key used in the thumbor service to
+    # match the URL construction
+    THUMBOR_SECURITY_KEY = 'MY_SECURE_KEY'
+
+    # Default arguments passed to the `generate_url` helper or
+    # the `thumbor_url` templatetag
+    THUMBOR_ARGUMENTS = {}
+
+    # An alias represents a named set of arguments to the generate_url function
+    # or thumbor_url template tag. Use it to share general thumbnail
+    # configurations without repeating yourself.
+    THUMBOR_ALIASES = {}
+
+
+Contributing
+------------
+
+Install
+.......
+
+Fork, clone, create a virtualenv and run:
+
+.. code-block:: bash
+
+    git clone git://github.com/ricobl/django-thumbor.git
+    cd django-thumbor
+    pipenv shell
+    make install
+
+Test
+....
+
+Add tests on ``testproject/tests``, add code and run:
+
+.. code-block:: bash
+
+    make test
+
+Test Server
+...........
+
+- Instal thumbor server: ``pip install thumbor``
+- Run thumbor: ``thumbor``
+- Run local server: ``make run``
+- visit `http://127.0.0.1:8000/ <http://127.0.0.1:8000/>`_:
```

### Comparing `django-thumbor-0.5.7/README.rst` & `django_thumbor-0.6.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -9,22 +9,14 @@
     :target: https://pypi.python.org/pypi/django-thumbor/
     :alt: Latest django-thumbor PyPI version
 
 .. image:: https://img.shields.io/pypi/dm/django-thumbor.svg
     :target: https://pypi.python.org/pypi/django-thumbor/
     :alt: Number of downloads for django-thumbor on PyPI
 
-.. image:: https://coveralls.io/repos/ricobl/django-thumbor/badge.png?branch=master
-    :target: https://coveralls.io/r/ricobl/django-thumbor?branch=master
-    :alt: Code coverage on Coveralls
-
-.. image:: https://gemnasium.com/ricobl/django-thumbor.svg
-    :target: https://gemnasium.com/ricobl/django-thumbor
-    :alt: Dependency Status on Gemnasium
-
 
 A django application to resize images using the
 `thumbor <https://github.com/globocom/thumbor>`_ service.
 
 Usage
 -----
 
@@ -185,18 +177,27 @@
 .......
 
 Fork, clone, create a virtualenv and run:
 
 .. code-block:: bash
 
     git clone git://github.com/ricobl/django-thumbor.git
-    mkvirtualenv django-thumbor
+    cd django-thumbor
+    pipenv shell
     make install
 
 Test
 ....
 
 Add tests on ``testproject/tests``, add code and run:
 
 .. code-block:: bash
 
     make test
+
+Test Server
+...........
+
+- Instal thumbor server: ``pip install thumbor``
+- Run thumbor: ``thumbor``
+- Run local server: ``make run``
+- visit `http://127.0.0.1:8000/ <http://127.0.0.1:8000/>`_:
```

### Comparing `django-thumbor-0.5.7/setup.py` & `django_thumbor-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 setup(
     name='django-thumbor',
-    version='0.5.7',
+    version='0.6.0',
     description=(
         'A django application to resize images using the thumbor service'),
     long_description=open('README.rst').read(),
     author=u'Enrico Batista da Luz',
     author_email='rico.bl@gmail.com',
     url='http://github.com/ricobl/django-thumbor/',
     license=(
```

