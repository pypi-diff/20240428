# Comparing `tmp/django-soft-delete-1.0.13.tar.gz` & `tmp/django-soft-delete-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-soft-delete-1.0.13.tar", last modified: Sun Apr 28 09:11:59 2024, max compression
+gzip compressed data, was "django-soft-delete-1.0.9.tar", last modified: Sun Jan 28 20:04:16 2024, max compression
```

## Comparing `django-soft-delete-1.0.13.tar` & `django-soft-delete-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-04-28 09:11:59.757934 django-soft-delete-1.0.13/
--rw-r--r--   0 alexander   (501) staff       (20)     1073 2021-03-12 11:18:14.000000 django-soft-delete-1.0.13/LICENSE
--rw-r--r--   0 alexander   (501) staff       (20)       17 2021-03-12 11:18:14.000000 django-soft-delete-1.0.13/MANIFEST.in
--rw-r--r--   0 alexander   (501) staff       (20)     3913 2024-04-28 09:11:59.757859 django-soft-delete-1.0.13/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)     3310 2023-04-02 16:04:54.000000 django-soft-delete-1.0.13/README.md
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-04-28 09:11:59.754773 django-soft-delete-1.0.13/django_soft_delete.egg-info/
--rw-r--r--   0 alexander   (501) staff       (20)     3913 2024-04-28 09:11:59.000000 django-soft-delete-1.0.13/django_soft_delete.egg-info/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)      483 2024-04-28 09:11:59.000000 django-soft-delete-1.0.13/django_soft_delete.egg-info/SOURCES.txt
--rw-r--r--   0 alexander   (501) staff       (20)        1 2024-04-28 09:11:59.000000 django-soft-delete-1.0.13/django_soft_delete.egg-info/dependency_links.txt
--rw-r--r--   0 alexander   (501) staff       (20)       18 2024-04-28 09:11:59.000000 django-soft-delete-1.0.13/django_soft_delete.egg-info/top_level.txt
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-04-28 09:11:59.756861 django-soft-delete-1.0.13/django_softdelete/
--rw-r--r--   0 alexander   (501) staff       (20)        1 2021-03-12 11:18:14.000000 django-soft-delete-1.0.13/django_softdelete/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     1909 2024-04-28 09:11:18.000000 django-soft-delete-1.0.13/django_softdelete/admin.py
--rw-r--r--   0 alexander   (501) staff       (20)       47 2024-01-27 20:13:47.000000 django-soft-delete-1.0.13/django_softdelete/exceptions.py
--rw-r--r--   0 alexander   (501) staff       (20)      630 2024-01-28 19:22:03.000000 django-soft-delete-1.0.13/django_softdelete/filters.py
--rw-r--r--   0 alexander   (501) staff       (20)     3109 2024-01-28 20:04:06.000000 django-soft-delete-1.0.13/django_softdelete/managers.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-04-28 09:11:59.757257 django-soft-delete-1.0.13/django_softdelete/migrations/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2021-03-12 11:18:14.000000 django-soft-delete-1.0.13/django_softdelete/migrations/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)    18708 2024-04-28 09:06:53.000000 django-soft-delete-1.0.13/django_softdelete/models.py
--rw-r--r--   0 alexander   (501) staff       (20)      192 2024-01-27 21:43:57.000000 django-soft-delete-1.0.13/django_softdelete/signals.py
--rw-r--r--   0 alexander   (501) staff       (20)       79 2024-04-28 09:11:59.758283 django-soft-delete-1.0.13/setup.cfg
--rw-r--r--   0 alexander   (501) staff       (20)      932 2024-04-28 09:11:25.000000 django-soft-delete-1.0.13/setup.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-04-28 09:11:59.757370 django-soft-delete-1.0.13/tests/
--rw-r--r--   0 alexander   (501) staff       (20)    14465 2024-02-03 16:53:35.000000 django-soft-delete-1.0.13/tests/test_models.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-01-28 20:04:16.828743 django-soft-delete-1.0.9/
+-rw-r--r--   0 alexander   (501) staff       (20)     1073 2021-03-12 11:18:14.000000 django-soft-delete-1.0.9/LICENSE
+-rw-r--r--   0 alexander   (501) staff       (20)       17 2021-03-12 11:18:14.000000 django-soft-delete-1.0.9/MANIFEST.in
+-rw-r--r--   0 alexander   (501) staff       (20)     3912 2024-01-28 20:04:16.828646 django-soft-delete-1.0.9/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)     3310 2023-04-02 16:04:54.000000 django-soft-delete-1.0.9/README.md
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-01-28 20:04:16.825069 django-soft-delete-1.0.9/django_soft_delete.egg-info/
+-rw-r--r--   0 alexander   (501) staff       (20)     3912 2024-01-28 20:04:16.000000 django-soft-delete-1.0.9/django_soft_delete.egg-info/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)      483 2024-01-28 20:04:16.000000 django-soft-delete-1.0.9/django_soft_delete.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander   (501) staff       (20)        1 2024-01-28 20:04:16.000000 django-soft-delete-1.0.9/django_soft_delete.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander   (501) staff       (20)       18 2024-01-28 20:04:16.000000 django-soft-delete-1.0.9/django_soft_delete.egg-info/top_level.txt
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-01-28 20:04:16.827259 django-soft-delete-1.0.9/django_softdelete/
+-rw-r--r--   0 alexander   (501) staff       (20)        1 2021-03-12 11:18:14.000000 django-soft-delete-1.0.9/django_softdelete/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1361 2024-01-28 19:18:23.000000 django-soft-delete-1.0.9/django_softdelete/admin.py
+-rw-r--r--   0 alexander   (501) staff       (20)       47 2024-01-27 20:13:47.000000 django-soft-delete-1.0.9/django_softdelete/exceptions.py
+-rw-r--r--   0 alexander   (501) staff       (20)      630 2024-01-28 19:22:03.000000 django-soft-delete-1.0.9/django_softdelete/filters.py
+-rw-r--r--   0 alexander   (501) staff       (20)     3109 2024-01-28 20:04:06.000000 django-soft-delete-1.0.9/django_softdelete/managers.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-01-28 20:04:16.827834 django-soft-delete-1.0.9/django_softdelete/migrations/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2021-03-12 11:18:14.000000 django-soft-delete-1.0.9/django_softdelete/migrations/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)    18141 2024-01-28 17:43:15.000000 django-soft-delete-1.0.9/django_softdelete/models.py
+-rw-r--r--   0 alexander   (501) staff       (20)      192 2024-01-27 21:43:57.000000 django-soft-delete-1.0.9/django_softdelete/signals.py
+-rw-r--r--   0 alexander   (501) staff       (20)       79 2024-01-28 20:04:16.829145 django-soft-delete-1.0.9/setup.cfg
+-rw-r--r--   0 alexander   (501) staff       (20)      931 2024-01-28 20:04:15.000000 django-soft-delete-1.0.9/setup.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2024-01-28 20:04:16.827964 django-soft-delete-1.0.9/tests/
+-rw-r--r--   0 alexander   (501) staff       (20)    14453 2024-01-28 16:53:52.000000 django-soft-delete-1.0.9/tests/test_models.py
```

### Comparing `django-soft-delete-1.0.13/LICENSE` & `django-soft-delete-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-soft-delete-1.0.13/PKG-INFO` & `django-soft-delete-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-soft-delete
-Version: 1.0.13
+Version: 1.0.9
 Summary: Soft delete models, managers, queryset for Django
 Home-page: https://github.com/san4ezy/django_softdelete
 Author: Alexander Yudkin
 Author-email: san4ezy@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `django-soft-delete-1.0.13/README.md` & `django-soft-delete-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-soft-delete-1.0.13/django_soft_delete.egg-info/PKG-INFO` & `django-soft-delete-1.0.9/django_soft_delete.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-soft-delete
-Version: 1.0.13
+Version: 1.0.9
 Summary: Soft delete models, managers, queryset for Django
 Home-page: https://github.com/san4ezy/django_softdelete
 Author: Alexander Yudkin
 Author-email: san4ezy@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `django-soft-delete-1.0.13/django_softdelete/admin.py` & `django-soft-delete-1.0.9/django_softdelete/admin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 from django.contrib import admin
 
 from django_softdelete.filters import SoftDeleteFilter
 
-@admin.action(description="Hard delete selected items")
-def hard_delete_selected_items(modeladmin, request, queryset):
-    queryset.hard_delete()
-
-@admin.action(description="Restore selected items")
-def restore_selected_items(modeladmin, request, queryset):
-    queryset.restore()
-
-custom_admin_actions = [
-    hard_delete_selected_items,
-    restore_selected_items,
-]
-
 
 class SoftDeletedModelAdmin(admin.ModelAdmin):
     """
     SoftDeletedModelAdmin
     Class representing a ModelAdmin for soft deleted objects in Django admin.
     The standard ModelAdmin works with a default object manager as well.
     """
@@ -26,19 +13,14 @@
         super().get_queryset(request)
         qs = self.model.deleted_objects.get_queryset()
         ordering = self.get_ordering(request)
         if ordering:
             qs = qs.order_by(*ordering)
         return qs
 
-    actions = [
-        *admin.ModelAdmin.actions,
-        *custom_admin_actions,
-    ]
-
 
 class GlobalObjectsModelAdmin(admin.ModelAdmin):
     """
     GlobalObjectsModelAdmin
     Class representing a ModelAdmin for both: deleted and alive objects in Django admin.
     The standard ModelAdmin works with a default object manager as well.
     """
@@ -52,12 +34,7 @@
 
     def get_list_filter(self, request):
         list_filter = super().get_list_filter(request) or []
         if not isinstance(list_filter, list):
             list_filter = list(list_filter)
         list_filter.append(SoftDeleteFilter)
         return list_filter
-
-    actions = [
-        *admin.ModelAdmin.actions,
-        *custom_admin_actions,
-    ]
```

### Comparing `django-soft-delete-1.0.13/django_softdelete/filters.py` & `django-soft-delete-1.0.9/django_softdelete/filters.py`

 * *Files identical despite different names*

### Comparing `django-soft-delete-1.0.13/django_softdelete/managers.py` & `django-soft-delete-1.0.9/django_softdelete/managers.py`

 * *Files identical despite different names*

### Comparing `django-soft-delete-1.0.13/django_softdelete/models.py` & `django-soft-delete-1.0.9/django_softdelete/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from django.db import models
 from django.db import transaction
 from django.db.models.deletion import ProtectedError
 from django.db.models.signals import pre_delete, post_delete
 from django.utils import timezone
 
 from django_softdelete.exceptions import SoftDeleteException
+from django_softdelete.managers import SoftDeleteManager
 from django_softdelete.managers import DeletedManager
 from django_softdelete.managers import GlobalManager
-from django_softdelete.managers import SoftDeleteManager
 from django_softdelete.signals import post_hard_delete, post_soft_delete, post_restore
 
 
 class SoftDeleteModel(models.Model):
     """
     A Django model which has been enhanced with soft deletion characteristics.
 
@@ -140,16 +140,14 @@
             If False, the related objects are restored regardless.
         :param args: Additional positional arguments.
         :param kwargs: Additional keyword arguments.
         :return: None
         """
 
         now = timezone.now()
-        self.deleted_at = None
-        self.restored_at = now
         with transaction.atomic():
             for field in self._meta.get_fields():
 
                 # Skip generic relations
                 if isinstance(field, GenericRelation):
                     continue
 
@@ -175,14 +173,17 @@
                             field, strict, *args, **kwargs
                         )
                     except ValueError as e:
                         continue
 
                 else:
                     continue
+
+            self.deleted_at = None
+            self.restored_at = now
             self.save(
                 update_fields=['deleted_at', 'restored_at', ]
             )
             post_restore.send(sender=self.__class__, instance=self)
 
     # PRIVATE SECTION
 
@@ -221,64 +222,57 @@
         if hasattr(field, 'on_delete'):
             on_delete = field.on_delete
         elif hasattr(field, 'remote_field') and hasattr(field.remote_field, 'on_delete'):
             on_delete = field.remote_field.on_delete
         else:
             return
 
-        if on_delete == models.CASCADE:
-            if strict:
-                kwargs['strict'] = strict
-            related_object.delete(*args, **kwargs)
-
-        elif on_delete == models.SET_NULL:
-            setattr(related_object, field.remote_field.name, None)
-            related_object.save()
-
-        elif on_delete == models.PROTECT:
-            related_query_name = (field.remote_field.related_query_name or
-                                    field.remote_field.related_name or
-                                    field.opts.model_name)
-
-            if callable(related_query_name):
-                related_query_name = related_query_name()
-
-            if related_object:
-                related_manager_name = related_query_name if hasattr(self,
-                                                                        related_query_name) else f"{related_query_name}_set"
-                protected_objects = list(getattr(self, related_manager_name).all())
-                raise ProtectedError(
-                    f"Cannot delete {self} because {related_object} is related with PROTECT",
-                    protected_objects=protected_objects
-                )
-
-        elif on_delete == models.SET_DEFAULT:
-            default_value = field.get_default()
-            setattr(related_object, field.remote_field.name, default_value)
-            related_object.save()
-
-        elif on_delete == models.SET:
-            if callable(field.remote_field.on_delete_set_function):
-                value = field.remote_field.on_delete_set_function(self)
-                setattr(related_object, field.remote_field.name, value)
+        match on_delete:
+
+            case models.CASCADE:
+                if strict:
+                    kwargs['strict'] = strict
+                related_object.delete(*args, **kwargs)
+
+            case models.SET_NULL:
+                setattr(related_object, field.remote_field.name, None)
+                related_object.save()
+
+            case models.PROTECT:
+                if related_object:
+                    raise ProtectedError(
+                        f"Cannot delete {self} because {related_object} "
+                        f"is related with PROTECT",
+                        [related_object]
+                    )
+
+            case models.SET_DEFAULT:
+                default_value = field.get_default()
+                setattr(related_object, field.remote_field.name, default_value)
                 related_object.save()
 
-        elif on_delete == models.DO_NOTHING:
-            pass  # Explicitly do nothing
+            case models.SET:
+                if callable(field.remote_field.on_delete_set_function):
+                    value = field.remote_field.on_delete_set_function(self)
+                    setattr(related_object, field.remote_field.name, value)
+                    related_object.save()
+
+            case models.DO_NOTHING:
+                pass  # Explicitly do nothing
 
-        elif on_delete == models.RESTRICT:
-            if related_object:
-                raise ProtectedError(
-                    f"Cannot delete {self} because {related_object} "
-                    f"is related with RESTRICT",
-                    [related_object]
-                )
+            case models.RESTRICT:
+                if related_object:
+                    raise ProtectedError(
+                        f"Cannot delete {self} because {related_object} "
+                        f"is related with RESTRICT",
+                        [related_object]
+                    )
 
-        else:  # M2M
-            related_object.delete(strict=strict, *args, **kwargs)
+            case _:  # M2M
+                related_object.delete(strict=strict, *args, **kwargs)
 
         try:
             if related_object.pk is not None:
                 related_object.save()
         except AttributeError:
             pass
 
@@ -295,21 +289,20 @@
         :param args: Additional positional arguments for the related object's restore method.
         :type args: Any
         :param kwargs: Additional keyword arguments for the related object's restore method.
         :type kwargs: Any
         :return: None
         :rtype: None
         """
-        if related_object.is_deleted:
-            related_object.restore(strict=strict, *args, **kwargs)
-            try:
-                if related_object.pk is not None:
-                    related_object.save()
-            except AttributeError:
-                pass
+        related_object.restore(strict=strict, *args, **kwargs)
+        try:
+            if related_object.pk is not None:
+                related_object.save()
+        except AttributeError:
+            pass
 
     def __delete_related_one_to_one(self, field, strict, *args, **kwargs):
         """
         Delete related one-to-one object.
 
         :param field: The field representing the one-to-one relationship.
         :param strict: If True, raise an exception if the related object does not exist. If False, do nothing if the related object does not exist.
```

### Comparing `django-soft-delete-1.0.13/setup.py` & `django-soft-delete-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-soft-delete",
-    version="1.0.13",
+    version="1.0.9",
     author="Alexander Yudkin",
     author_email="san4ezy@gmail.com",
     description="Soft delete models, managers, queryset for Django",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/san4ezy/django_softdelete",
     packages=setuptools.find_packages(
```

### Comparing `django-soft-delete-1.0.13/tests/test_models.py` & `django-soft-delete-1.0.9/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,20 +350,20 @@
             assert f"ProductRestrictedCategory object ({p.pk})" in err_msg
             assert f"related with RESTRICT" in err_msg
 
         p.refresh_from_db()
         assert not p.is_deleted
         assert not category.is_deleted
 
-    # def test_delete_with_not_soft_delete_model_relation(
-    #         self, not_soft_related_model, product_not_soft_relation,
-    # ):
-    #     with pytest.raises(SoftDeleteException) as e:
-    #         product_not_soft_relation.delete()
-    #     assert str(e.value) == "NotSoftRelatedModel is not a subclass of SoftDeleteModel."
+    def test_delete_with_not_soft_delete_model_relation(
+            self, not_soft_related_model, product_not_soft_relation,
+    ):
+        with pytest.raises(SoftDeleteException) as e:
+            product_not_soft_relation.delete()
+        assert str(e.value) == "NotSoftRelatedModel is not a subclass of SoftDeleteModel."
 
     def test_delete_with_not_soft_delete_model_relation_not_strict(
             self, not_soft_related_model, product_not_soft_relation,
     ):
         product_not_soft_relation.delete(strict=False)
         product_not_soft_relation.refresh_from_db()
         assert product_not_soft_relation.is_deleted
```

