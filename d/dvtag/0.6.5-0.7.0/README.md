# Comparing `tmp/dvtag-0.6.5.tar.gz` & `tmp/dvtag-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvtag-0.6.5.tar", last modified: Tue Apr 16 06:28:30 2024, max compression
+gzip compressed data, was "dvtag-0.7.0.tar", last modified: Sun Apr 28 12:07:14 2024, max compression
```

## Comparing `dvtag-0.6.5.tar` & `dvtag-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:28:30.953558 dvtag-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-16 06:28:20.000000 dvtag-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-16 06:28:30.953558 dvtag-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-16 06:28:20.000000 dvtag-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:28:30.953558 dvtag-0.6.5/dvtag/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 06:28:20.000000 dvtag-0.6.5/dvtag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-16 06:28:20.000000 dvtag-0.6.5/dvtag/doujinvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-16 06:28:20.000000 dvtag-0.6.5/dvtag/dvtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-16 06:28:20.000000 dvtag-0.6.5/dvtag/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:28:30.953558 dvtag-0.6.5/dvtag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-16 06:28:30.000000 dvtag-0.6.5/dvtag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-16 06:28:30.000000 dvtag-0.6.5/dvtag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 06:28:30.000000 dvtag-0.6.5/dvtag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 06:28:30.000000 dvtag-0.6.5/dvtag.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-16 06:28:30.000000 dvtag-0.6.5/dvtag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 06:28:30.000000 dvtag-0.6.5/dvtag.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-16 06:28:20.000000 dvtag-0.6.5/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-16 06:28:30.957558 dvtag-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 06:28:20.000000 dvtag-0.6.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-16 06:28:20.000000 dvtag-0.6.5/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:07:14.428568 dvtag-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-28 12:06:57.000000 dvtag-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-28 12:07:14.428568 dvtag-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-28 12:06:57.000000 dvtag-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:07:14.428568 dvtag-0.7.0/dvtag/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-28 12:06:57.000000 dvtag-0.7.0/dvtag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-28 12:06:57.000000 dvtag-0.7.0/dvtag/doujinvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-28 12:06:57.000000 dvtag-0.7.0/dvtag/dvtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-28 12:06:57.000000 dvtag-0.7.0/dvtag/scrape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-28 12:06:57.000000 dvtag-0.7.0/dvtag/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:07:14.428568 dvtag-0.7.0/dvtag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-28 12:07:14.000000 dvtag-0.7.0/dvtag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-28 12:07:14.000000 dvtag-0.7.0/dvtag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:07:14.000000 dvtag-0.7.0/dvtag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-28 12:07:14.000000 dvtag-0.7.0/dvtag.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-28 12:07:14.000000 dvtag-0.7.0/dvtag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 12:07:14.000000 dvtag-0.7.0/dvtag.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-28 12:06:57.000000 dvtag-0.7.0/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-28 12:07:14.432568 dvtag-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:06:57.000000 dvtag-0.7.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-28 12:06:57.000000 dvtag-0.7.0/utils.py
```

### Comparing `dvtag-0.6.5/LICENSE` & `dvtag-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvtag-0.6.5/PKG-INFO` & `dvtag-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvtag
-Version: 0.6.5
+Version: 0.7.0
 Summary: A tool for tagging your doujin voice library.
 Home-page: https://github.com/nobekanai/dvtag
 Author: Nobe Kanai
 Author-email: nobekanai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dvtag-0.6.5/README.md` & `dvtag-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dvtag-0.6.5/dvtag/dvtag.py` & `dvtag-0.7.0/dvtag/dvtag.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,108 @@
-from io import BytesIO
 import logging
+from io import BytesIO
 from pathlib import Path
 from typing import List, Optional
 
-from PIL.Image import Image
 from mutagen.flac import FLAC
-from mutagen.id3 import APIC, ID3, ID3NoHeaderError, TALB, TDRC, TPE1, TPE2, TPOS, TRCK, TCON
+from mutagen.id3 import APIC, ID3, TALB, TCON, TDRC, TIT2, TPE1, TPE2, TPOS, TRCK, ID3NoHeaderError
 from natsort import os_sorted
-
-from dvtag.utils import (
-    get_audio_paths_list,
-    get_image,
-    get_picture,
-    get_png_byte_arr,
-    get_rjid,
-)
+from PIL.Image import Image
 
 from .doujinvoice import DoujinVoice
+from .scrape import scrape
+from .utils import extract_titles, get_audio_paths_list, get_image, get_picture, get_png_byte_arr
+
+__all__ = ["tag"]
 
 
 def tag_mp3s(mp3_paths: List[Path], dv: DoujinVoice, png_bytes_arr: BytesIO, disc_number: Optional[int]):
     tags = ID3()
 
-    tags.add(TALB(text=[dv.work_name]))
+    tags.add(TALB(text=[dv.name]))
     tags.add(TPE2(text=[dv.circle]))
     tags.add(TDRC(text=[dv.sale_date]))
     if dv.genres:
         tags.add(TCON(text=[";".join(dv.genres)]))
     if disc_number:
         tags.add(TPOS(text=[str(disc_number)]))
     if dv.seiyus:
         tags.add(TPE1(text=dv.seiyus))
     tags.add(APIC(mime="image/png", desc="Front Cover", data=png_bytes_arr.getvalue()))
 
-    for trck, p in enumerate(os_sorted(mp3_paths), start=1):
+    sorted = list(os_sorted(mp3_paths))
+    titles = extract_titles(sorted_stems=[f.stem for f in sorted])
+
+    for trck, title, p in zip(range(1, len(sorted) + 1), titles, sorted):
+        tags.add(TIT2(text=[title]))
         tags.add(TRCK(text=[str(trck)]))
 
         try:
             if ID3(p) != tags:
                 tags.save(p, v1=0)
-                logging.info(f"Tagged <track: {trck}, disc: {disc_number}> to '{p.name}'")
+                logging.info(f"Tagged <track: {trck}, disc: {disc_number}, title: '{title}'> to '{p.name}'")
         except ID3NoHeaderError:
             tags.save(p, v1=0)
-            logging.info(f"Tagged <track: {trck}, disc: {disc_number}> to '{p.name}'")
+            logging.info(f"Tagged <track: {trck}, disc: {disc_number}, title: '{title}'> to '{p.name}'")
         tags.delall("TRCK")
 
 
 def tag_flacs(files: List[Path], dv: DoujinVoice, image: Image, png_bytes_arr: BytesIO, disc: Optional[int]):
     picture = get_picture(png_bytes_arr, image.width, image.height, image.mode)
 
-    for trck, file in enumerate(os_sorted(files), start=1):
-        tags = FLAC(file)
+    sorted = list(os_sorted(files))
+    titles = extract_titles(sorted_stems=[f.stem for f in sorted])
+
+    for trck, title, p in zip(range(1, len(sorted) + 1), titles, sorted):
+        tags = FLAC(p)
         tags.clear()
         tags.clear_pictures()
 
         tags.add_picture(picture)
-        tags["album"] = [dv.work_name]
-        tags["tracknumber"] = [str(trck)]
-        tags["artist"] = dv.seiyus
+        tags["album"] = [dv.name]
         tags["albumartist"] = [dv.circle]
         tags["date"] = [dv.sale_date]
-        tags["genre"] = dv.genres
+        tags["title"] = [title]
+        tags["tracknumber"] = [str(trck)]
+        if dv.genres:
+            tags["genre"] = dv.genres
+        if dv.seiyus:
+            tags["artist"] = dv.seiyus
         if disc:
             tags["discnumber"] = [str(disc)]
 
-        if tags != FLAC(file):
-            tags.save(file)
-            logging.info(f"Tagged <track: {trck}, disc: {disc}> to '{file.name}'")
-
-
-def tag(basepath: Path):
-    rjid = get_rjid(basepath.name)
-    dv = DoujinVoice(rjid)
-    logging.info(f"[{rjid}] Ready to tag...")
-    logging.info(f"Circle: {dv.circle}")
-    logging.info(f"Album:  {dv.work_name}")
-    logging.info(f"Seiyu:  {','.join(dv.seiyus)}")
-    logging.info(f"Genre:  {','.join(dv.genres)}")
-    logging.info(f"Date:   {dv.sale_date}")
+        if tags != FLAC(p):
+            tags.save(p)
+            logging.info(f"Tagged <track: {trck}, disc: {disc}>, title: '{title}'>  to '{p.name}'")
 
-    image = get_image(dv.work_image)
-    png_bytes_arr = get_png_byte_arr(image)
 
+def tag(basepath: Path, workno: str):
     flac_paths_list, mp3_paths_list = get_audio_paths_list(basepath)
+    if not flac_paths_list and not mp3_paths_list:
+        return
+
+    dv = scrape(workno)
+    logging.info(f"[{workno}] Ready to tag...")
+    logging.info(f" Circle: {dv.circle}")
+    logging.info(f" Album:  {dv.name}")
+    logging.info(f" Seiyu:  {','.join(dv.seiyus)}")
+    logging.info(f" Genre:  {','.join(dv.genres)}")
+    logging.info(f" Date:   {dv.sale_date}")
+
+    image = get_image(dv.image_url)
+    png_bytes_arr = get_png_byte_arr(image)
 
-    set_disc = False
     disc = None
     if len(flac_paths_list) + len(mp3_paths_list) > 1:
-        set_disc = True
         disc = 1
 
     for flac_files in flac_paths_list:
         tag_flacs(flac_files, dv, image, png_bytes_arr, disc)
-        if set_disc:
+        if disc:
             disc += 1
 
     for mp3_files in mp3_paths_list:
         tag_mp3s(mp3_files, dv, png_bytes_arr, disc)
-        if set_disc:
+        if disc:
             disc += 1
 
-    logging.info(f"[{rjid}] Done.")
+    logging.info(f"[{workno}] Done.")
```

### Comparing `dvtag-0.6.5/dvtag/utils.py` & `dvtag-0.7.0/dvtag/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,36 @@
 import io
+import re
 from io import BytesIO
 from pathlib import Path
-import re
 from typing import List, Optional, Tuple
 
-from PIL import Image
+import requests
 from mutagen.flac import Picture
 from mutagen.id3 import PictureType
 from natsort import os_sort_key
-import requests
+from PIL import Image
 from requests.adapters import HTTPAdapter
 
-rjid_pat = re.compile(r"RJ\d{6}(\d\d)?", flags=re.IGNORECASE)
+__all__ = [
+    "create_request_session",
+    "extract_titles",
+    "get_audio_paths_list",
+    "get_image",
+    "get_picture",
+    "get_png_byte_arr",
+    "get_workno",
+]
 
-
-def _split(audio_files: List[Path]) -> List[List[Path]]:
-    regexes = [
-        r"^omake_?.*[0-9]{1,2}.*$",
-        r"^.*ex[0-9]{1,2}.*$",
-        r"^ex_.+$",
-        r"^後日談.*$",
-        r"^おまけ_?[0-9]{0,2}.*$",
-        r"^反転おまけ_?[0-9]{1,2}.*$",
-        r"^反転_?[0-9]{1,2}.*$",
-        r"^20..年?[0-9]{1,2}月配信.*$",
-        r"^.*特典.*$",
-        r"^追加[0-9]{1,2}.*$",
-        r"^opt[0-9]?.*",
-        r"^#[0-9]+(-|ー)B",
-        r"^#[0-9]+(-|ー)C",
-        r"^ASMR_.*",
-        r"^.+Bパート",
-        r"^番外編",
-    ]  # Regular expressions must keep no collision with each other
-
-    results = {}
-    paths = []
-    regular = []
-    for audio_file in audio_files:
-        matched = False
-        for regex_expr in regexes:
-            if re.match(regex_expr, audio_file.stem, re.IGNORECASE):
-                matched = True
-                if results.get(regex_expr):
-                    results[regex_expr].append(audio_file)
-                else:
-                    results[regex_expr] = [audio_file]
-                break
-
-        if not matched:
-            regular.append(audio_file)
-
-    if len(regular):
-        paths.append(regular)
-
-    for _, v in results.items():
-        paths.append(v)
-
-    return paths
+workno_pat = re.compile(r"(R|B|V)J\d{6}(\d\d)?", flags=re.IGNORECASE)
 
 
 def _walk(basepath: Path):
-    dirs = []
-    files = []
+    dirs: List[Path] = []
+    files: List[Path] = []
     for file in basepath.iterdir():
         if file.is_dir():
             dirs.append(file)
         else:
             files.append(file)
     yield files
 
@@ -81,44 +45,44 @@
 
     Args:
         basepath (Path): base path
 
     Returns:
         Tuple[List[List[Path]], List[List[Path]]]: flac paths list, mp3 paths list
     """
-    flac_paths_list = []
-    mp3_paths_list = []
+    flac_paths_list: List[List[Path]] = []
+    mp3_paths_list: List[List[Path]] = []
 
     for files in _walk(basepath):
-        mp3_paths = []
-        flac_paths = []
+        mp3_paths: List[Path] = []
+        flac_paths: List[Path] = []
         for file in files:
             if file.suffix.lower() == ".flac":
                 flac_paths.append(file)
             elif file.suffix.lower() == ".mp3":
                 mp3_paths.append(file)
 
         if len(flac_paths):
-            flac_paths_list.extend(_split(flac_paths))
+            flac_paths_list.append(flac_paths)
         if len(mp3_paths):
-            mp3_paths_list.extend(_split(mp3_paths))
+            mp3_paths_list.append(mp3_paths)
 
     return flac_paths_list, mp3_paths_list
 
 
-def get_rjid(name: str) -> Optional[str]:
-    """Gets rjid(or rather, rj code) from a given string
+def get_workno(name: str) -> Optional[str]:
+    """Gets workno(of dlsite) from a given string
 
     Args:
         name (str): A string
 
     Returns:
         Optional[str]: Returns a string(upper case, like RJ123123) if found, otherwise return None
     """
-    m = rjid_pat.search(name)
+    m = workno_pat.search(name)
     if m:
         return m.group().upper()
     return None
 
 
 def get_image(url: str) -> Image.Image:
     cover_path = create_request_session().get(url, stream=True).raw
@@ -166,7 +130,50 @@
         requests.Session: Request session
     """
     session = requests.Session()
     adapter = HTTPAdapter(max_retries=max_retries)
     session.mount("http://", adapter)
     session.mount("https://", adapter)
     return session
+
+
+_title_pat = re.compile(
+    r"^(#|■|◆|【|\(|(?:【?tr(?:ack)?|トラック|音轨|とらっく)[\-_‗\s\.．・,：]*)?([\d]+)([\-_‗\s\.．・,：】\)]+|(?=[「『【]))(.+)",
+    re.IGNORECASE,
+)
+
+
+def extract_titles(sorted_stems: List[str]) -> List[str]:
+    if len(sorted_stems) <= 1:
+        return sorted_stems
+
+    if (m := _title_pat.match(sorted_stems[0])) is None:
+        return sorted_stems
+
+    pref: str | None = m.group(1)
+    suff: str = m.group(3)
+    diff: int = int(m.group(2))
+
+    if pref:
+        if pref == "【" and not suff.startswith("】"):
+            return sorted_stems
+        if pref == "(" and not suff.startswith(")"):
+            return sorted_stems
+
+    extracted: List[str] = [m.group(4)]
+
+    for i in range(1, len(sorted_stems)):
+        m = _title_pat.match(sorted_stems[i])
+        if not m:
+            return sorted_stems
+
+        if m.group(1) != pref or m.group(3) != suff:
+            return sorted_stems
+        if int(m.group(2)) - i != diff:
+            return sorted_stems
+
+        if (title := m.group(4)) in extracted:
+            return sorted_stems
+
+        extracted.append(title)
+
+    return extracted
```

### Comparing `dvtag-0.6.5/dvtag.egg-info/PKG-INFO` & `dvtag-0.7.0/dvtag.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvtag
-Version: 0.6.5
+Version: 0.7.0
 Summary: A tool for tagging your doujin voice library.
 Home-page: https://github.com/nobekanai/dvtag
 Author: Nobe Kanai
 Author-email: nobekanai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dvtag-0.6.5/main.py` & `dvtag-0.7.0/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import argparse
 import logging
 from importlib.metadata import version
 from pathlib import Path
 
-from dvtag import get_rjid, tag
+from dvtag import get_workno, tag
 from utils import wav_to_flac, wav_to_mp3
 
-logging.basicConfig(
-    level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s", datefmt="%Y-%m-%d %a %H:%M:%S"
-)
+logging.basicConfig(level=logging.INFO, format="%(message)s")
 
 
 def start(dirpath: Path, w2f: bool, w2m: bool):
-    if get_rjid(dirpath.name):
+    if workno := get_workno(dirpath.name):
         if w2f:
             wav_to_flac(dirpath)
         if w2m:
             wav_to_mp3(dirpath)
-        tag(dirpath)
+        tag(dirpath, workno)
         return
 
     for file in dirpath.iterdir():
         if not file.is_dir():
             continue
         start(file, w2f, w2m)
```

### Comparing `dvtag-0.6.5/setup.cfg` & `dvtag-0.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dvtag
-version = 0.6.5
+version = 0.7.0
 author = Nobe Kanai
 author_email = nobekanai@gmail.com
 description = A tool for tagging your doujin voice library.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nobekanai/dvtag
 classifiers =
```

### Comparing `dvtag-0.6.5/utils.py` & `dvtag-0.7.0/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,34 @@
+"""This module provides a minimal implementation of some functions for transcoding `.wav` files to other formats using `ffmpeg`.
+
+If users need more flexible encoding options or advanced features(like parallel transcoding), we recommend directly using `ffmpeg` or a more feature-rich library.
+"""
+
 import logging
 import os
-from pathlib import Path
 import subprocess
+from pathlib import Path
 from typing import List
 
+__all__ = [
+    "wav_to_mp3",
+    "wav_to_flac",
+]
+
 
 def transcode_wav(dir: Path, format: str, options: List[str] = []):
     for dirpath, _, filenames in os.walk(dir):
         for filename_wav in filenames:
             if not filename_wav.endswith(".wav"):
                 continue
             filename_trans = filename_wav[:-3] + format
 
             file_wav = os.path.join(dirpath, filename_wav)
             file_trans = os.path.join(dirpath, filename_trans)
             if os.path.exists(file_trans):
-                # this should not happen
                 logging.warning(f"{filename_trans} already exists.")
                 continue
 
             logging.info(f"Start transcoding {filename_wav} to {format}")
 
             returncode = subprocess.call(
                 ["ffmpeg", "-i", file_wav, *options, file_trans], stdout=open(os.devnull, "w"), stderr=subprocess.STDOUT
```

