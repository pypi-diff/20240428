# Comparing `tmp/simplenote_local-1.0.2.tar.gz` & `tmp/simplenote_local-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplenote_local-1.0.2.tar", last modified: Wed Apr 17 09:03:29 2024, max compression
+gzip compressed data, was "simplenote_local-1.0.3.tar", last modified: Sun Apr 28 06:32:47 2024, max compression
```

## Comparing `simplenote_local-1.0.2.tar` & `simplenote_local-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-17 09:03:29.867436 simplenote_local-1.0.2/
--rw-r--r--   0 norm       (502) staff       (20)     1076 2024-02-29 11:23:11.000000 simplenote_local-1.0.2/LICENSE
--rw-r--r--   0 norm       (502) staff       (20)     7629 2024-04-17 09:03:29.867251 simplenote_local-1.0.2/PKG-INFO
--rw-r--r--   0 norm       (502) staff       (20)     7115 2024-04-16 14:19:17.000000 simplenote_local-1.0.2/README.md
-drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-17 09:03:29.864546 simplenote_local-1.0.2/nv/
--rw-r--r--   0 norm       (502) staff       (20)        0 2024-02-29 11:31:47.000000 simplenote_local-1.0.2/nv/__init__.py
--rw-r--r--   0 norm       (502) staff       (20)    29466 2024-03-27 16:54:15.000000 simplenote_local-1.0.2/nv/nv.py
--rw-r--r--   0 norm       (502) staff       (20)       38 2024-04-17 09:03:29.867488 simplenote_local-1.0.2/setup.cfg
--rw-r--r--   0 norm       (502) staff       (20)      925 2024-04-16 14:12:25.000000 simplenote_local-1.0.2/setup.py
-drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-17 09:03:29.865887 simplenote_local-1.0.2/simplenote_local/
--rw-r--r--   0 norm       (502) staff       (20)    33607 2024-04-17 08:59:44.000000 simplenote_local-1.0.2/simplenote_local/__init__.py
--rw-r--r--   0 norm       (502) staff       (20)     7587 2024-04-16 09:05:24.000000 simplenote_local-1.0.2/simplenote_local/cli.py
--rw-r--r--   0 norm       (502) staff       (20)       22 2024-04-17 09:00:44.000000 simplenote_local-1.0.2/simplenote_local/version.py
-drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-17 09:03:29.867035 simplenote_local-1.0.2/simplenote_local.egg-info/
--rw-r--r--   0 norm       (502) staff       (20)     7629 2024-04-17 09:03:29.000000 simplenote_local-1.0.2/simplenote_local.egg-info/PKG-INFO
--rw-r--r--   0 norm       (502) staff       (20)      392 2024-04-17 09:03:29.000000 simplenote_local-1.0.2/simplenote_local.egg-info/SOURCES.txt
--rw-r--r--   0 norm       (502) staff       (20)        1 2024-04-17 09:03:29.000000 simplenote_local-1.0.2/simplenote_local.egg-info/dependency_links.txt
--rw-r--r--   0 norm       (502) staff       (20)       57 2024-04-17 09:03:29.000000 simplenote_local-1.0.2/simplenote_local.egg-info/entry_points.txt
--rw-r--r--   0 norm       (502) staff       (20)       57 2024-04-17 09:03:29.000000 simplenote_local-1.0.2/simplenote_local.egg-info/requires.txt
--rw-r--r--   0 norm       (502) staff       (20)       20 2024-04-17 09:03:29.000000 simplenote_local-1.0.2/simplenote_local.egg-info/top_level.txt
-drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-17 09:03:29.866763 simplenote_local-1.0.2/tests/
--rw-r--r--   0 norm       (502) staff       (20)      193 2024-03-09 12:03:31.000000 simplenote_local-1.0.2/tests/test_note.py
+drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-28 06:32:47.557814 simplenote_local-1.0.3/
+-rw-r--r--   0 norm       (502) staff       (20)     1076 2024-02-29 11:23:11.000000 simplenote_local-1.0.3/LICENSE
+-rw-r--r--   0 norm       (502) staff       (20)     7567 2024-04-28 06:32:47.557624 simplenote_local-1.0.3/PKG-INFO
+-rw-r--r--   0 norm       (502) staff       (20)     7044 2024-04-28 06:31:40.000000 simplenote_local-1.0.3/README.md
+drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-28 06:32:47.555321 simplenote_local-1.0.3/nv/
+-rw-r--r--   0 norm       (502) staff       (20)        0 2024-02-29 11:31:47.000000 simplenote_local-1.0.3/nv/__init__.py
+-rw-r--r--   0 norm       (502) staff       (20)    29466 2024-03-27 16:54:15.000000 simplenote_local-1.0.3/nv/nv.py
+-rw-r--r--   0 norm       (502) staff       (20)       38 2024-04-28 06:32:47.557863 simplenote_local-1.0.3/setup.cfg
+-rw-r--r--   0 norm       (502) staff       (20)      934 2024-04-28 06:16:03.000000 simplenote_local-1.0.3/setup.py
+drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-28 06:32:47.556182 simplenote_local-1.0.3/simplenote_local/
+-rw-r--r--   0 norm       (502) staff       (20)    33018 2024-04-28 06:31:01.000000 simplenote_local-1.0.3/simplenote_local/__init__.py
+-rw-r--r--   0 norm       (502) staff       (20)     7587 2024-04-28 06:31:07.000000 simplenote_local-1.0.3/simplenote_local/cli.py
+-rw-r--r--   0 norm       (502) staff       (20)       22 2024-04-26 10:12:52.000000 simplenote_local-1.0.3/simplenote_local/version.py
+drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-28 06:32:47.557389 simplenote_local-1.0.3/simplenote_local.egg-info/
+-rw-r--r--   0 norm       (502) staff       (20)     7567 2024-04-28 06:32:47.000000 simplenote_local-1.0.3/simplenote_local.egg-info/PKG-INFO
+-rw-r--r--   0 norm       (502) staff       (20)      392 2024-04-28 06:32:47.000000 simplenote_local-1.0.3/simplenote_local.egg-info/SOURCES.txt
+-rw-r--r--   0 norm       (502) staff       (20)        1 2024-04-28 06:32:47.000000 simplenote_local-1.0.3/simplenote_local.egg-info/dependency_links.txt
+-rw-r--r--   0 norm       (502) staff       (20)       57 2024-04-28 06:32:47.000000 simplenote_local-1.0.3/simplenote_local.egg-info/entry_points.txt
+-rw-r--r--   0 norm       (502) staff       (20)       66 2024-04-28 06:32:47.000000 simplenote_local-1.0.3/simplenote_local.egg-info/requires.txt
+-rw-r--r--   0 norm       (502) staff       (20)       20 2024-04-28 06:32:47.000000 simplenote_local-1.0.3/simplenote_local.egg-info/top_level.txt
+drwxr-xr-x   0 norm       (502) staff       (20)        0 2024-04-28 06:32:47.557091 simplenote_local-1.0.3/tests/
+-rw-r--r--   0 norm       (502) staff       (20)      193 2024-03-09 12:03:31.000000 simplenote_local-1.0.3/tests/test_note.py
```

### Comparing `simplenote_local-1.0.2/LICENSE` & `simplenote_local-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simplenote_local-1.0.2/PKG-INFO` & `simplenote_local-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: simplenote_local
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sync notes to/from simplenote.com
 Home-page: https://github.com/norm/simplenote-local
 Author: Mark Norman Francis
 Author-email: norm@201created.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4
 Requires-Dist: markdownify
-Requires-Dist: nltk
+Requires-Dist: simple-colors
 Requires-Dist: simplenote
 Requires-Dist: toml
 Requires-Dist: watchdog
 
 # simplenote-local
 
 A command-line tool to fetch, edit, and synchronise local notes files with
@@ -262,13 +262,11 @@
 
     simplenote --list-changes
 
 **Note:** this does not automatically fetch the current state of notes, so
 it is not 100% authoritative.
 
 
+* rename local note
 * revert local changes
 * archive copy of all historic notes
 * create a git repo of all historic notes replayed as individual commits
-
-* can get into an inconsistent state when notes are deleted and purged on simplenote.com
-
```

### Comparing `simplenote_local-1.0.2/README.md` & `simplenote_local-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -243,13 +243,11 @@
 
     simplenote --list-changes
 
 **Note:** this does not automatically fetch the current state of notes, so
 it is not 100% authoritative.
 
 
+* rename local note
 * revert local changes
 * archive copy of all historic notes
 * create a git repo of all historic notes replayed as individual commits
-
-* can get into an inconsistent state when notes are deleted and purged on simplenote.com
-
```

### Comparing `simplenote_local-1.0.2/nv/nv.py` & `simplenote_local-1.0.3/nv/nv.py`

 * *Files identical despite different names*

### Comparing `simplenote_local-1.0.2/setup.py` & `simplenote_local-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         'console_scripts': [
             'simplenote=simplenote_local.cli:main',
         ],
     },
     install_requires = [
         'beautifulsoup4',
         'markdownify',
-        'nltk',
+        'simple-colors',
         'simplenote',
         'toml',
         'watchdog',
     ],
     python_requires = '>=3.8',
     classifiers = [
         'License :: OSI Approved :: MIT License',
```

### Comparing `simplenote_local-1.0.2/simplenote_local/__init__.py` & `simplenote_local-1.0.3/simplenote_local/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from datetime import datetime, timedelta
 import hashlib
 from markdownify import markdownify
 import nltk
 import os
 import pickle
 import re
+from simple_colors import *
 from simplenote import Simplenote
 import subprocess
 import sys
 import time
 import toml
 
 
@@ -31,14 +32,16 @@
         self.body = note.get('body', '')
         content = note.get('content', None)
         if content:
             self.title, self.body = self.title_and_body(content)
             self.fingerprint = hashlib.sha256(self.body.encode('utf-8')).hexdigest()
             self.content = content
         else:
+            if not self.title:
+                self.title = 'new note'
             self.content = self.title + "\n\n" + self.body
         self.filename = note.get('filename', '%s.txt' % self.title)
 
     @classmethod
     def title_and_body(cls, text):
         # fix problems with very old notes
         text = text.replace(u'\xa0', u' ')
@@ -127,38 +130,29 @@
 class SimplenoteLocal:
     def __init__(self, directory='.', user=False, password=False, editor='ed'):
         self.directory = directory
         self.editor = editor
         self.user = user
         self.password = password
         self.simplenote_api = Simplenote(self.user, self.password)
-        self.notes, self.cursor, self.words = self.load_data()
+        self.reload_data()
         os.makedirs(self.directory, exist_ok=True)
 
-        try:
-            self.stop_words = set(nltk.corpus.stopwords.words('english'))
-        except:
-            nltk.download('stopwords')
-            self.stop_words = set(nltk.corpus.stopwords.words('english'))
+    def reload_data(self):
+        self.notes, self.cursor, self.words = self.load_data()
 
     def fetch_changes(self):
+        received_change = False
         updates = self.get_note_updates()
         for entry in updates:
             update = Note(entry)
             current = None
             if update.key in self.notes:
                 current = self.notes[update.key]
 
-            # from pprint import pprint
-            # print('====')
-            # pprint(update.as_dict())
-            # if current:
-            #     print('----')
-            #     pprint(current.as_dict())
-            # print('====')
 
             if current and current.version >= update.version:
                 # because of the stored cursor position, running fetch after
                 # sending a local update will include the already known version
                 continue
 
             if current and not current.deleted and current.title == update.title:
@@ -178,115 +172,114 @@
                         update.increment_filename()
 
             if current and not current.deleted and current.filename != update.filename:
                 os.rename(
                     os.path.join(self.directory, current.filename),
                     os.path.join(self.directory, update.filename),
                 )
-                print('  ', current.filename, '->', update.filename)
+                print('  ', current.filename, green('->'), update.filename)
 
             if update.deleted:
                 if current and not current.deleted:
                     self.remove_note_file(update)
                 update.filename = ''
             else:
                 self.add_to_words_cache(update.filename, update.content)
                 self.save_note_file(update)
 
             self.notes[update.key] = update
-        self.save_data()
+            received_change = True
+        if received_change:
+            self.save_data()
 
     def send_changes(self):
         for note in self.list_changed_notes():
-            new_note = self.send_one_change(note)
-            self.notes[note.key] = new_note
+            self.send_one_change(note)
         self.save_data()
 
     def watch_for_changes(self, fetch_interval, send_wait):
         import threading
         from watchdog.observers import Observer
         from watchdog.events import FileSystemEventHandler
 
         class Changes(FileSystemEventHandler):
             def __init__(self, local):
                 super().__init__()
-                self.local = local
                 self.lock = threading.Lock()
-                self.found = self.local.list_changed_notes()
+                self.events = False
 
             def on_any_event(self, event):
                 filename = os.path.basename(event.src_path)
                 if filename.endswith('.txt') and not filename.startswith('.'):
                     with self.lock:
-                        self.found = self.local.list_changed_notes()
+                        self.events = True
 
         changes = Changes(self)
         observer = Observer()
         observer.schedule(changes, path=self.directory, recursive=True)
         observer.start()
 
         fetch_interval = timedelta(seconds=fetch_interval)
         send_wait = timedelta(seconds=send_wait)
         last_fetch = datetime.now() - fetch_interval
 
         try:
             while True:
                 time.sleep(1)
-                # print('...', datetime.now(), end='\r')
 
                 if datetime.now() - fetch_interval >= last_fetch:
-                    # print('... fetching                  ')
                     self.fetch_changes()
                     last_fetch = datetime.now()
 
                 sent_change = False
                 with changes.lock:
-                    if changes.found:
-                        # print('... changes:')
-                        for note in changes.found:
-                            # print('   ', note.filename)
+                    if changes.events:
+                        # a slight pause to account for another
+                        # command performing file changing actions
+                        time.sleep(1)
+                        self.reload_data()
+                        for note in self.list_changed_notes():
                             send = False
                             filename = note.filename
                             pathname = os.path.join(self.directory, filename)
                             if os.path.exists(pathname):
                                 stamp = datetime.fromtimestamp(
                                     os.path.getmtime(pathname)
                                 )
                                 if stamp + send_wait < datetime.now():
                                     send = True
                             else:
                                 send = True
                             if send:
-                                # print('    sending')
-                                new_note = self.send_one_change(note)
-                                self.notes[note.key] = new_note
+                                self.send_one_change(note)
                                 sent_change = True
-                if sent_change:
-                    self.save_data()
-                changes.found = self.list_changed_notes()
+                        if sent_change:
+                            self.save_data()
+                        if not self.list_changed_notes():
+                            changes.events = False
 
         except KeyboardInterrupt:
             observer.stop()
         observer.join()
 
     def list_matching_notes(self, matches):
         for note in self.find_matching_notes(matches):
             filename = note.filename.replace('"', '\\"')
             pinned = ''
             shared = ''
             tags = ''
             url = ''
             if 'pinned' in note.system_tags:
-                pinned = ' pinned' 
-            if 'shared' in note.system_tags:
-                shared = ' shared'
+                pinned = blue(' pinned', 'bold')
+            if note.share_list:
+                shared = red(' shared ' + note.share_list)
             if note.tags:
-                tags = ' ' + note.tag_list
+                tags = ' ' + blue(note.tag_list)
             if 'published' in note.system_tags:
-                url = ' %s' % note.published_url
+                url = yellow(' %s' % note.published_url)
             print(f'"{filename}"{pinned}{shared}{tags}{url}')
 
     def list_tags(self):
         tags = dict()
         for note in self.get_local_note_state():
             for tag in note.tags:
                 if tag in tags:
@@ -309,16 +302,15 @@
 
                 # touch the file even though the contents haven't changed
                 pathname = os.path.join(self.directory, match.filename)
                 now = int(datetime.now().timestamp())
                 os.utime(pathname, (now, now))
                 match.modified = now
 
-                new_note = self.send_one_change(match)
-                self.notes[match.key] = new_note
+                self.send_one_change(match)
                 sent_change = True
         if sent_change:
             self.save_data()
 
     def remove_tag(self, tag, matches):
         matching = self.find_matching_notes(matches)
         sent_change = False
@@ -328,16 +320,15 @@
 
                 # touch the file even though the contents haven't changed
                 pathname = os.path.join(self.directory, match.filename)
                 now = int(datetime.now().timestamp())
                 os.utime(pathname, (now, now))
                 match.modified = now
 
-                new_note = self.send_one_change(match)
-                self.notes[match.key] = new_note
+                self.send_one_change(match)
                 sent_change = True
         if sent_change:
             self.save_data()
 
     def edit_matching_notes(self, matches):
         matching = self.find_matching_notes(matches)
 
@@ -358,16 +349,15 @@
 
             subprocess.run(command, check=True)
 
             changes = False
             for note in self.list_changed_notes():
                 for match in matching:
                     if note.filename.lower() == match.filename.lower():
-                        new_note = self.send_one_change(note)
-                        self.notes[note.key] = new_note
+                        self.send_one_change(note)
                         changes = True
             if changes:
                 self.save_data()
         else:
             print("""** No notes found matching all of: %s.
 
 To edit an individual note using this tool, the filename must contain a space
@@ -427,25 +417,31 @@
                 'creationDate': now,
                 'modificationDate': now,
                 'content': title + "\n\n" + body,
                 'state': 'new',
                 'systemTags': system_tags,
             })
 
+        unique_filename = False
+        while not unique_filename:
+            by_filename = self.get_note_by_filename(note.filename)
+            if not by_filename:
+                unique_filename = True
+            else:
+                note.increment_filename()
+
         new_note = self.send_one_change(note)
-        self.notes[note.key] = new_note
         self.save_data()
 
     def trash_notes(self, matches):
         sent_change = False
         for match in self.find_matching_notes(matches):
             match.state = 'deleted'
             self.remove_note_file(match, 'quiet')
-            new_note = self.send_one_change(match)
-            self.notes[match.key] = new_note
+            self.send_one_change(match)
             sent_change = True
 
         if sent_change:
             self.save_data()
 
     def restore_notes(self, matches):
         sent_change = False
@@ -460,16 +456,15 @@
                         latest = Note(latest)
                         latest.deleted = False
                         latest.modified = datetime.now().timestamp()
                         pathname = os.path.join(self.directory, latest.filename)
                         with open(pathname, 'w') as handle:
                             handle.write(latest.body)
                         os.utime(pathname, (latest.modified, latest.modified))
-                        new_note = self.send_one_change(latest)
-                        self.notes[latest.key] = new_note
+                        self.send_one_change(latest)
                         sent_change = True
 
         if sent_change:
             self.save_data()
 
     def purge_notes(self, matches):
         sent_change = False
@@ -479,39 +474,37 @@
             if note.deleted:
                 for match in matches:
                     if match.lower() in note.title.lower():
                         _, error = self.simplenote_api.delete_note(note.key)
                         if error:
                             sys.exit(error)
                         sent_change = True
-                        print('XX', note.title)
+                        print(red('XX'), note.title)
                         deleted.append(note.key)
 
         if sent_change:
             for key in deleted:
                 del self.notes[key]
             self.save_data()
 
     def pin_notes(self, matches):
         sent_change = False
         for match in self.find_matching_notes(matches):
             match.system_tags.append('pinned')
-            new_note = self.send_one_change(match)
-            self.notes[match.key] = new_note
+            self.send_one_change(match)
             sent_change = True
 
         if sent_change:
             self.save_data()
 
     def unpin_notes(self, matches):
         sent_change = False
         for match in self.find_matching_notes(matches):
             match.system_tags.remove('pinned')
-            new_note = self.send_one_change(match)
-            self.notes[match.key] = new_note
+            self.send_one_change(match)
             sent_change = True
 
         if sent_change:
             self.save_data()
 
     def publish_notes(self, matches):
         sent_change = False
@@ -622,36 +615,33 @@
                     ((version // 10) * 10 + 11),
                 ),
                 file=sys.stderr
             )
         else:
             note.state = 'restored'
             note.version = None
-            new_note = self.send_one_change(note)
-            self.notes[note.key] = new_note
+            self.send_one_change(note)
             self.save_data()
 
     def list_changes(self):
         for note in self.list_changed_notes():
             key = note.key
             if key:
-                # from pprint import pprint
-                # pprint([note.state, note.as_dict()])
                 updated = False
                 if note.modified != self.notes[key].modified:
                     updated = True
                 if note.fingerprint != self.notes[key].fingerprint:
                     updated = True
                 if updated:
-                    print('>>', note.filename)
+                    print(blue('>>'), note.filename)
                 else:
-                    print('XX', note.filename, end='\n\n')
+                    print(magenta('--'), note.filename, end='\n\n')
                     continue
             else:
-                print('++', note.filename)
+                print(green('++'), note.filename)
             print(
                 '   last updated:',
                 datetime.utcfromtimestamp(int(note.modified)),
                 end='\n\n',
             )
 
     def get_note_version(self, key, version):
@@ -686,17 +676,16 @@
                 for note in notes:
                     if match.lower() in note.filename.lower():
                         matching.add(note)
             else:
                 for word in self.words:
                     if match in word:
                         for note in notes:
-                            for filename in self.words[word]:
-                                if note.filename == filename:
-                                    matching.add(note)
+                            if note.filename in self.words[word]:
+                                matching.add(note)
             notes = notes.intersection(matching)
 
         return sorted(
             notes,
             key=lambda note: ('pinned' in note.system_tags, note.modified),
             reverse=True,
         )
@@ -708,27 +697,30 @@
             notes
         ))
 
     def send_one_change(self, note):
         if note.state == 'deleted':
             new_note = self.trash_note(note)
             new_note = Note(new_note)
-            print('XX', note.filename)
+            print(magenta('--'), note.filename)
         elif note.state == 'new':
             new_note = self.send_note_update(note)
-            pathname = os.path.join(self.directory, new_note.filename)
+            pathname = os.path.join(self.directory, note.filename)
             with open(pathname, 'w') as handle:
                 handle.write(new_note.body)
             os.utime(pathname, (new_note.modified, new_note.modified))
-            print('++ note "%s" (%s)' % (note.filename, new_note.key))
+            print(green('++'), 'note "%s" (%s)' % (note.filename, new_note.key))
         else:
-            note.content = note.filename[:-4] + "\n\n" + note.body
+            note.content = note.title + "\n\n" + note.body
             new_note = self.send_note_update(note)
             self.save_note_file(new_note)
-            print('>>', new_note.filename)
+            print(blue('>>'), new_note.filename)
+
+        if note.title == new_note.title:
+            new_note.filename = note.filename
         self.notes[new_note.key] = new_note
         return new_note
 
     def get_note_updates(self):
         notes, error = self.simplenote_api.get_note_list(since=self.cursor)
         if error:
             sys.exit(error)
@@ -792,36 +784,32 @@
             with open(pathname, 'r') as handle:
                 body = handle.read()
                 sha = hashlib.sha256(body.encode('utf-8')).hexdigest()
 
             if filename in expected_files:
                 note = deepcopy(self.notes[expected_files[filename]])
                 note.body = body
+                note.content = note.title + "\n\n" + note.body
                 note.state = 'unchanged'
-                # if current != note.modified:
-                #     print('  ', current, '!=', note.modified)
-                # if sha != note.fingerprint:
-                #     print('  ', sha, '!=', note.fingerprint)
                 if current != note.modified or sha != note.fingerprint:
-                    # print('  ', note.filename)
                     note.modified = current
                     note.state = 'changed'
-                    self.add_to_words_cache(filename, body)
+                    self.add_to_words_cache(filename, note.content)
                 del expected_files[filename]
                 local_notes.append(note)
             else:
                 note = Note({
                     'creationDate': current,
                     'modificationDate': current,
                     'body': body,
                     'content': filename[:-4] + "\n\n" + body,
                     'filename': filename,
                     'state': 'new',
                 })
-                self.add_to_words_cache(filename, body)
+                self.add_to_words_cache(filename, note.content)
                 local_notes.append(note)
 
         # deal with any known notes now removed
         for filename in expected_files:
             note = deepcopy(self.notes[expected_files[filename]])
             note.state = 'deleted'
             local_notes.append(note)
@@ -837,25 +825,25 @@
         except FileNotFoundError:
             current = None
 
         if note.body != current:
             with open(pathname, 'w') as handle:
                 handle.write(note.body)
             if not current:
-                print('++', note.filename)
+                print(green('++'), note.filename)
             else:
-                print('<<', note.filename)
+                print(blue('<<'), note.filename)
         os.utime(pathname, (note.modified, note.modified))
 
     def remove_note_file(self, note, quiet=False):
         pathname = os.path.join(self.directory, note.filename)
         try:
             os.remove(pathname)
             if not quiet:
-                print('--', note.filename)
+                print(magenta('--'), note.filename)
         except FileNotFoundError:
             # after deleting a file locally the next fetch will
             # include the state that the file has been removed,
             # but it has already been removed -- so, not an error
             pass
         self.remove_file_from_words_cache(note.filename)
 
@@ -867,18 +855,18 @@
                 pass
             except ValueError:
                 pass
 
     def add_to_words_cache(self, filename, content):
         self.remove_file_from_words_cache(filename)
         words = set(
-            word for word in [
-                re.sub(r'[\W_]+', '', word.lower())
-                    for word in re.split(r'\b', filename[:-4] + content)
-                ] if word and len(word) < 30 and word not in self.stop_words
+            word[:60] for word in [
+                re.sub(r'[\W_]+', ' ', word.lower())
+                    for word in re.split(r'\b', content)
+                ] if word and len(word) > 2
         )
         for word in words:
             if word not in self.words:
                 self.words[word] = [ filename, ]
             else:
                 if filename not in self.words[word]:
                     self.words[word].append(filename)
@@ -901,20 +889,26 @@
         words = {}
         for key in data['notes']:
             notes[key] = Note(data['notes'][key])
 
         return notes, data['cursor'], data['words']
 
     def save_data(self):
-        with open(os.path.join(self.directory, 'notes.data'), 'wb') as handle:
+        tmp_file = os.path.join(self.directory, '.notes.save')
+        with open(tmp_file, 'wb') as handle:
             pickle.dump({
                 'notes': self.notes_as_dict(),
                 'cursor': self.cursor,
                 'words': self.words,
             }, handle)
-        with open(os.path.join(self.directory, 'notes.toml'), 'w') as handle:
+            handle.flush()
+            os.fsync(handle.fileno())
+        os.rename(tmp_file, os.path.join(self.directory, 'notes.data'))
+        with open(tmp_file, 'w') as handle:
             toml.dump({
                 'notes': self.notes_as_dict(),
                 'cursor': self.cursor,
                 'words': self.words,
             }, handle)
-
+            handle.flush()
+            os.fsync(handle.fileno())
+        os.rename(tmp_file, os.path.join(self.directory, 'notes.toml'))
```

### Comparing `simplenote_local-1.0.2/simplenote_local/cli.py` & `simplenote_local-1.0.3/simplenote_local/cli.py`

 * *Files identical despite different names*

### Comparing `simplenote_local-1.0.2/simplenote_local.egg-info/PKG-INFO` & `simplenote_local-1.0.3/simplenote_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: simplenote_local
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sync notes to/from simplenote.com
 Home-page: https://github.com/norm/simplenote-local
 Author: Mark Norman Francis
 Author-email: norm@201created.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4
 Requires-Dist: markdownify
-Requires-Dist: nltk
+Requires-Dist: simple-colors
 Requires-Dist: simplenote
 Requires-Dist: toml
 Requires-Dist: watchdog
 
 # simplenote-local
 
 A command-line tool to fetch, edit, and synchronise local notes files with
@@ -262,13 +262,11 @@
 
     simplenote --list-changes
 
 **Note:** this does not automatically fetch the current state of notes, so
 it is not 100% authoritative.
 
 
+* rename local note
 * revert local changes
 * archive copy of all historic notes
 * create a git repo of all historic notes replayed as individual commits
-
-* can get into an inconsistent state when notes are deleted and purged on simplenote.com
-
```

