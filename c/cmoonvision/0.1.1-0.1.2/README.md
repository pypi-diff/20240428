# Comparing `tmp/cmoonvision-0.1.1.tar.gz` & `tmp/cmoonvision-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmoonvision-0.1.1.tar", max compression
+gzip compressed data, was "cmoonvision-0.1.2.tar", max compression
```

## Comparing `cmoonvision-0.1.1.tar` & `cmoonvision-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-26 13:48:25.163207 cmoonvision-0.1.1/README.md
--rw-r--r--   0        0        0     5219 2024-04-27 16:03:55.383760 cmoonvision-0.1.1/cmoonvision/CmoonVision.py
--rw-r--r--   0        0        0      201 2024-04-28 02:52:22.565891 cmoonvision-0.1.1/cmoonvision/__init__.py
--rw-r--r--   0        0        0    12606 2024-04-28 02:47:45.135158 cmoonvision-0.1.1/cmoonvision/cmoon_utils.py
--rw-r--r--   0        0        0      410 2024-04-28 03:37:12.716443 cmoonvision-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      459 1970-01-01 00:00:00.000000 cmoonvision-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-26 13:48:25.163207 cmoonvision-0.1.2/README.md
+-rw-r--r--   0        0        0     5219 2024-04-27 16:03:55.383760 cmoonvision-0.1.2/cmoonvision/CmoonVision.py
+-rw-r--r--   0        0        0      201 2024-04-28 02:52:22.565891 cmoonvision-0.1.2/cmoonvision/__init__.py
+-rw-r--r--   0        0        0    12733 2024-04-28 04:04:59.359664 cmoonvision-0.1.2/cmoonvision/cmoon_utils.py
+-rw-r--r--   0        0        0      410 2024-04-28 04:07:42.766199 cmoonvision-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      459 1970-01-01 00:00:00.000000 cmoonvision-0.1.2/PKG-INFO
```

### Comparing `cmoonvision-0.1.1/cmoonvision/CmoonVision.py` & `cmoonvision-0.1.2/cmoonvision/CmoonVision.py`

 * *Files identical despite different names*

### Comparing `cmoonvision-0.1.1/cmoonvision/cmoon_utils.py` & `cmoonvision-0.1.2/cmoonvision/cmoon_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,18 @@
 
     @cached_property
     def img_shape(self) -> Tuple[int, int]:
         return self.raw_result.orig_shape[::-1]
 
     @cached_property
     def mask(self) -> np.ndarray:
-        segments = self.raw_result.masks.xy
+        try:
+            segments = self.raw_result.masks.xy
+        except AttributeError:
+            raise ValueError("No segment data. Ensure using a segment model.")
         _mask = np.zeros((480, 640), dtype=np.uint8)
         for segment in segments:
             x_coords = segment[:, 0]
             y_coords = segment[:, 1]
             points = np.array(list(zip(x_coords, y_coords)), dtype=np.int32)
             cv2.fillPoly(_mask, [points.reshape((-1, 1, 2))], color=(255, 255, 255))
         return _mask
```

