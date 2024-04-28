# Comparing `tmp/toolong-1.4.0.tar.gz` & `tmp/toolong-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolong-1.4.0.tar", max compression
+gzip compressed data, was "toolong-1.5.0.tar", max compression
```

## Comparing `toolong-1.4.0.tar` & `toolong-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1069 2024-02-07 10:19:07.993997 toolong-1.4.0/LICENSE
--rw-r--r--   0        0        0     5532 2024-02-20 09:49:27.194239 toolong-1.4.0/README.md
--rw-r--r--   0        0        0      661 2024-03-02 11:21:31.926266 toolong-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-07 17:25:09.037948 toolong-1.4.0/src/toolong/__init__.py
--rw-r--r--   0        0        0       66 2024-02-07 10:30:58.308009 toolong-1.4.0/src/toolong/__main__.py
--rw-r--r--   0        0        0     2569 2024-02-19 16:32:14.796295 toolong-1.4.0/src/toolong/cli.py
--rw-r--r--   0        0        0     4545 2024-02-15 13:52:30.193410 toolong-1.4.0/src/toolong/find_dialog.py
--rw-r--r--   0        0        0     3527 2024-03-02 11:21:31.926511 toolong-1.4.0/src/toolong/format_parser.py
--rw-r--r--   0        0        0     1658 2024-02-15 15:27:41.382992 toolong-1.4.0/src/toolong/goto_screen.py
--rw-r--r--   0        0        0     5587 2024-02-11 13:49:19.936140 toolong-1.4.0/src/toolong/help.py
--rw-r--r--   0        0        0     1832 2024-03-02 11:21:31.926690 toolong-1.4.0/src/toolong/highlighter.py
--rw-r--r--   0        0        0     1629 2024-03-02 11:21:31.926860 toolong-1.4.0/src/toolong/line_panel.py
--rw-r--r--   0        0        0     7156 2024-03-02 11:21:31.927138 toolong-1.4.0/src/toolong/log_file.py
--rw-r--r--   0        0        0    34915 2024-03-02 11:21:31.927400 toolong-1.4.0/src/toolong/log_lines.py
--rw-r--r--   0        0        0    13179 2024-03-02 11:21:31.927716 toolong-1.4.0/src/toolong/log_view.py
--rw-r--r--   0        0        0     1657 2024-02-15 15:24:03.569473 toolong-1.4.0/src/toolong/messages.py
--rw-r--r--   0        0        0     1099 2024-02-19 15:02:46.407492 toolong-1.4.0/src/toolong/poll_watcher.py
--rw-r--r--   0        0        0     1147 2024-02-06 10:50:15.140933 toolong-1.4.0/src/toolong/scan_progress_bar.py
--rw-r--r--   0        0        0     2051 2024-02-14 19:48:14.107912 toolong-1.4.0/src/toolong/selector_watcher.py
--rw-r--r--   0        0        0     6463 2024-03-02 11:21:31.927978 toolong-1.4.0/src/toolong/timestamps.py
--rw-r--r--   0        0        0     3594 2024-02-15 17:00:10.470510 toolong-1.4.0/src/toolong/ui.py
--rw-r--r--   0        0        0     2297 2024-02-19 15:02:46.407805 toolong-1.4.0/src/toolong/watcher.py
--rw-r--r--   0        0        0     6385 1970-01-01 00:00:00.000000 toolong-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-02-07 10:19:07.993997 toolong-1.5.0/LICENSE
+-rw-r--r--   0        0        0     5532 2024-02-20 09:49:27.194239 toolong-1.5.0/README.md
+-rw-r--r--   0        0        0      661 2024-04-28 16:07:22.642813 toolong-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-07 17:25:09.037948 toolong-1.5.0/src/toolong/__init__.py
+-rw-r--r--   0        0        0       66 2024-02-07 10:30:58.308009 toolong-1.5.0/src/toolong/__main__.py
+-rw-r--r--   0        0        0     2569 2024-02-19 16:32:14.796295 toolong-1.5.0/src/toolong/cli.py
+-rw-r--r--   0        0        0     4545 2024-02-15 13:52:30.193410 toolong-1.5.0/src/toolong/find_dialog.py
+-rw-r--r--   0        0        0     3820 2024-04-28 15:01:21.455147 toolong-1.5.0/src/toolong/format_parser.py
+-rw-r--r--   0        0        0     1658 2024-02-15 15:27:41.382992 toolong-1.5.0/src/toolong/goto_screen.py
+-rw-r--r--   0        0        0     5691 2024-04-28 15:46:11.109005 toolong-1.5.0/src/toolong/help.py
+-rw-r--r--   0        0        0     1832 2024-03-02 11:21:31.926690 toolong-1.5.0/src/toolong/highlighter.py
+-rw-r--r--   0        0        0     1899 2024-04-28 16:12:31.652531 toolong-1.5.0/src/toolong/line_panel.py
+-rw-r--r--   0        0        0     7154 2024-04-28 16:29:46.565239 toolong-1.5.0/src/toolong/log_file.py
+-rw-r--r--   0        0        0    34935 2024-04-28 16:11:01.678525 toolong-1.5.0/src/toolong/log_lines.py
+-rw-r--r--   0        0        0    13138 2024-03-19 11:05:09.655354 toolong-1.5.0/src/toolong/log_view.py
+-rw-r--r--   0        0        0     1657 2024-02-15 15:24:03.569473 toolong-1.5.0/src/toolong/messages.py
+-rw-r--r--   0        0        0     1099 2024-04-28 16:16:26.420053 toolong-1.5.0/src/toolong/poll_watcher.py
+-rw-r--r--   0        0        0     1202 2024-03-19 11:56:04.649421 toolong-1.5.0/src/toolong/scan_progress_bar.py
+-rw-r--r--   0        0        0     2050 2024-04-28 16:23:48.882715 toolong-1.5.0/src/toolong/selector_watcher.py
+-rw-r--r--   0        0        0     6463 2024-03-02 11:21:31.927978 toolong-1.5.0/src/toolong/timestamps.py
+-rw-r--r--   0        0        0     3687 2024-03-18 16:30:30.409517 toolong-1.5.0/src/toolong/ui.py
+-rw-r--r--   0        0        0     2297 2024-02-19 15:02:46.407805 toolong-1.5.0/src/toolong/watcher.py
+-rw-r--r--   0        0        0     6436 1970-01-01 00:00:00.000000 toolong-1.5.0/PKG-INFO
```

### Comparing `toolong-1.4.0/LICENSE` & `toolong-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toolong-1.4.0/README.md` & `toolong-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `toolong-1.4.0/pyproject.toml` & `toolong-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "toolong"
-version = "1.4.0"
+version = "1.5.0"
 description = "A terminal log file viewer / tailer / analyzer"
 authors = ["Will McGugan <will@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/textualize/toolong"
 repository = "https://github.com/textualize/toolong"
 documentation = "https://github.com/textualize/toolong"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.7"
-textual = "^0.52.0"
+textual = "^0.58.0"
 typing-extensions = "^4.9.0"
 
 [tool.poetry.group.dev.dependencies]
 textual-dev = "^1.4.0"
 
 [tool.poetry.scripts]
 tl = "toolong.cli:run"
```

### Comparing `toolong-1.4.0/src/toolong/cli.py` & `toolong-1.5.0/src/toolong/cli.py`

 * *Files identical despite different names*

### Comparing `toolong-1.4.0/src/toolong/find_dialog.py` & `toolong-1.5.0/src/toolong/find_dialog.py`

 * *Files identical despite different names*

### Comparing `toolong-1.4.0/src/toolong/format_parser.py` & `toolong-1.5.0/src/toolong/format_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 from __future__ import annotations
 from datetime import datetime
 import json
 import re
 from typing_extensions import TypeAlias
 
 from rich.highlighter import JSONHighlighter
+import rich.repr
 from rich.text import Text
 
 from toolong.highlighter import LogHighlighter
 from toolong import timestamps
 from typing import Optional
 
 
 ParseResult: TypeAlias = "tuple[Optional[datetime], str, Text]"
 
 
+@rich.repr.auto
 class LogFormat:
     def parse(self, line: str) -> ParseResult | None:
         raise NotImplementedError()
 
 
+HTTP_GROUPS = {
+    "1": "cyan",
+    "2": "green",
+    "3": "yellow",
+    "4": "red",
+    "5": "reverse red",
+}
+
+
 class RegexLogFormat(LogFormat):
     REGEX = re.compile(".*?")
     HIGHLIGHT_WORDS = [
         "GET",
         "POST",
         "PUT",
         "HEAD",
@@ -42,17 +53,15 @@
         groups = match.groupdict()
         _, timestamp = timestamps.parse(groups["date"].strip("[]"))
 
         text = Text.from_ansi(line)
         if not text.spans:
             text = self.highlighter(text)
         if status := groups.get("status", None):
-            text.highlight_words(
-                [f" {status} "], "bold red" if status.startswith("4") else "magenta"
-            )
+            text.highlight_words([f" {status} "], HTTP_GROUPS.get(status[0], "magenta"))
         text.highlight_words(self.HIGHLIGHT_WORDS, "bold yellow")
 
         return timestamp, line, text
 
 
 class CommonLogFormat(RegexLogFormat):
     REGEX = re.compile(
@@ -73,15 +82,14 @@
         text = Text.from_ansi(line)
         if not text.spans:
             text = self.highlighter(text)
         return None, line, text
 
 
 class JSONLogFormat(LogFormat):
-
     highlighter = JSONHighlighter()
 
     def parse(self, line: str) -> ParseResult | None:
         line = line.strip()
         if not line:
             return None
         try:
@@ -95,29 +103,34 @@
         return timestamp, line, text
 
 
 FORMATS = [
     JSONLogFormat(),
     CommonLogFormat(),
     CombinedLogFormat(),
-    DefaultLogFormat(),
+    # DefaultLogFormat(),
 ]
 
+default_log_format = DefaultLogFormat()
+
 
 class FormatParser:
     """Parses a log line."""
 
     def __init__(self) -> None:
         self._formats = FORMATS.copy()
 
     def parse(self, line: str) -> ParseResult:
         """Parse a line."""
         if len(line) > 10_000:
             line = line[:10_000]
-        for index, format in enumerate(self._formats):
-            parse_result = format.parse(line)
-            if parse_result is not None:
-                if index:
-                    del self._formats[index : index + 1]
-                    self._formats.insert(0, format)
-                return parse_result
+        if line.strip():
+            for index, format in enumerate(self._formats):
+                parse_result = format.parse(line)
+                if parse_result is not None:
+                    if index:
+                        self._formats = [*self._formats[index:], *self._formats[:index]]
+                    return parse_result
+        parse_result = default_log_format.parse(line)
+        if parse_result is not None:
+            return parse_result
         return None, "", Text()
```

### Comparing `toolong-1.4.0/src/toolong/goto_screen.py` & `toolong-1.5.0/src/toolong/goto_screen.py`

 * *Files identical despite different names*

### Comparing `toolong-1.4.0/src/toolong/help.py` & `toolong-1.5.0/src/toolong/help.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,20 @@
 Repository: [https://github.com/Textualize/toolong](https://github.com/Textualize/toolong) Author: [Will McGugan](https://www.willmcgugan.com)
 
 ---
 
 ### Navigation
 
 - `tab` / `shift+tab` to navigate between widgets.
-- `home` / `end` Jump to start or end of file. Press `end` a second time to *tail* the current file.
-- `page up` / `page down` to go to the next / previous page.
-- `↑` / `↓` Move up / down a line.
+- `home` or `G` / `end` or `g` Jump to start or end of file. Press `end` a second time to *tail* the current file.
+- `page up` / `page down` or `space` to go to the next / previous page.
+- `←` or `h` / `→` or `l` Scroll left / right.
+- `↑` or `w` or `k` / `↓` or `s` or `j` Move up / down a line.
 - `m` / `M` Advance +1 / -1 minutes.
-- `h` / `H` Advance +1 / -1 hours.
+- `o` / `O` Advance +1 / -1 hours.
 - `d` / `D` Advance +1 / -1 days.
 - `enter` Toggle pointer mode.
 - `escape` Dismiss.
 
 ### Other keys
 
 - `ctrl+f` or `/` Show find dialog.
```

### Comparing `toolong-1.4.0/src/toolong/highlighter.py` & `toolong-1.5.0/src/toolong/highlighter.py`

 * *Files identical despite different names*

### Comparing `toolong-1.4.0/src/toolong/line_panel.py` & `toolong-1.5.0/src/toolong/line_panel.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,18 @@
         width: auto;
         height: auto;        
         Label {
             width: 1fr;
         }  
         .json {
             width: auto;        
-        }      
+        }
+        .nl {
+            width: auto;
+        }  
     }
     """
 
     def __init__(self, line: str, text: Text, timestamp: datetime | None) -> None:
         self.line = line
         self.text = text
         self.timestamp = timestamp
@@ -38,22 +41,29 @@
         try:
             json_data = json.loads(self.line)
         except Exception:
             pass
         else:
             yield Static(JSON.from_data(json_data), expand=True, classes="json")
             return
-        yield Label(self.text)
+
+        if "\\n" in self.text.plain:
+            lines = self.text.split("\\n")
+            text = Text("\n", no_wrap=True).join(lines)
+            yield Label(text, classes="nl")
+        else:
+            yield Label(self.text)
 
 
 class LinePanel(ScrollableContainer):
     DEFAULT_CSS = """
     LinePanel {
         background: $panel;        
         overflow-y: auto;
+        overflow-x: auto;
         border: blank transparent;                
         scrollbar-gutter: stable;
         &:focus {
             border: heavy $accent;
         }
     }
     """
```

### Comparing `toolong-1.4.0/src/toolong/log_file.py` & `toolong-1.5.0/src/toolong/log_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
         except AttributeError:
             # No birthtime for Linux, so we assume the epoch start
             return datetime.fromtimestamp(0)
         timestamp = datetime.fromtimestamp(create_time_seconds)
         return timestamp
 
     def open(self, exit_event: Event) -> bool:
-
         # Check for compressed files
         _, encoding = mimetypes.guess_type(self.path.name, strict=False)
 
         # Open compressed files
         if encoding in ("gzip", "bzip2"):
             return self.open_compressed(exit_event, encoding)
 
@@ -147,15 +146,14 @@
 
         def get_raw(self, start: int, end: int) -> bytes:
             if start >= end or self.file is None:
                 return b""
             return os.pread(self.fileno, end - start, start)
 
     def get_line(self, start: int, end: int) -> str:
-
         return (
             self.get_raw(start, end)
             .decode("utf-8", errors="replace")
             .strip("\n\r")
             .expandtabs(4)
         )
```

### Comparing `toolong-1.4.0/src/toolong/log_lines.py` & `toolong-1.5.0/src/toolong/log_lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,28 +125,28 @@
         if search_hit is None:
             return None
         return start + search_hit
 
 
 class LogLines(ScrollView, inherit_bindings=False):
     BINDINGS = [
-        Binding("up,k", "scroll_up", "Scroll Up", show=False),
-        Binding("down,j", "scroll_down", "Scroll Down", show=False),
-        Binding("left", "scroll_left", "Scroll Up", show=False),
-        Binding("right", "scroll_right", "Scroll Right", show=False),
-        Binding("home", "scroll_home", "Scroll Home", show=False),
-        Binding("end", "scroll_end", "Scroll End", show=False),
-        Binding("pageup", "page_up", "Page Up", show=False),
-        Binding("pagedown", "page_down", "Page Down", show=False),
+        Binding("up,w,k", "scroll_up", "Scroll Up", show=False),
+        Binding("down,s,j", "scroll_down", "Scroll Down", show=False),
+        Binding("left,h", "scroll_left", "Scroll Left", show=False),
+        Binding("right,l", "scroll_right", "Scroll Right", show=False),
+        Binding("home,G", "scroll_home", "Scroll Home", show=False),
+        Binding("end,g", "scroll_end", "Scroll End", show=False),
+        Binding("pageup,b", "page_up", "Page Up", show=False),
+        Binding("pagedown,space", "page_down", "Page Down", show=False),
         Binding("enter", "select", "Select line", show=False),
         Binding("escape", "dismiss", "Dismiss", show=False, priority=True),
         Binding("m", "navigate(+1, 'm')"),
         Binding("M", "navigate(-1, 'm')"),
-        Binding("h", "navigate(+1, 'h')"),
-        Binding("H", "navigate(-1, 'h')"),
+        Binding("o", "navigate(+1, 'h')"),
+        Binding("O", "navigate(-1, 'h')"),
         Binding("d", "navigate(+1, 'd')"),
         Binding("D", "navigate(-1, 'd')"),
     ]
 
     DEFAULT_CSS = """
     LogLines {
         scrollbar-gutter: stable;
@@ -781,15 +781,14 @@
 
     def watch_regex(self) -> None:
         self.clear_caches()
 
     def watch_pointer_line(
         self, old_pointer_line: int | None, pointer_line: int | None
     ) -> None:
-
         if old_pointer_line is not None:
             self.refresh_line(old_pointer_line)
         if pointer_line is not None:
             self.refresh_line(pointer_line)
         self.show_gutter = pointer_line is not None
         self.post_message(PointerMoved(pointer_line))
 
@@ -863,15 +862,14 @@
                 "Stopped scanning. Some lines may not be available.", severity="warning"
             )
         else:
             self.post_message(DismissOverlay())
 
     # @work(thread=True)
     def action_navigate(self, steps: int, unit: Literal["m", "h", "d"]) -> None:
-
         initial_line_no = line_no = (
             self.scroll_offset.y if self.pointer_line is None else self.pointer_line
         )
 
         count = 0
         # If the current line doesn't have a timestamp, try to find the next one
         while (timestamp := self.get_timestamp(line_no)) is None:
```

### Comparing `toolong-1.4.0/src/toolong/log_view.py` & `toolong-1.5.0/src/toolong/log_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 from asyncio import Lock
 from datetime import datetime
 
-from rich.text import Text
-
 from textual import on
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Horizontal
 from textual.dom import NoScreen
 from textual import events
 from textual.reactive import reactive
@@ -96,14 +94,17 @@
 
 class FooterKey(Label):
     """Displays a clickable label for a key."""
 
     DEFAULT_CSS = """
     FooterKey {
         color: $success;
+        &:light {
+            color: $primary;
+        }
         padding: 0 1 0 0;        
         &:hover {
             text-style: bold underline;                        
         }
     }
     """
     DEFAULT_CLASSES = "key"
@@ -288,16 +289,15 @@
 
     def __init__(
         self, file_paths: list[str], watcher: WatcherBase, can_tail: bool = True
     ) -> None:
         self.file_paths = file_paths
         self.watcher = watcher
         super().__init__()
-        # Need a better solution for this
-        self.call_later(setattr, self, "can_tail", can_tail)
+        self.can_tail = can_tail
 
     def compose(self) -> ComposeResult:
         yield (
             log_lines := LogLines(self.watcher, self.file_paths).data_bind(
                 LogView.tail,
                 LogView.show_line_numbers,
                 LogView.show_find,
```

### Comparing `toolong-1.4.0/src/toolong/messages.py` & `toolong-1.5.0/src/toolong/messages.py`

 * *Files identical despite different names*

### Comparing `toolong-1.4.0/src/toolong/poll_watcher.py` & `toolong-1.5.0/src/toolong/poll_watcher.py`

 * *Files identical despite different names*

### Comparing `toolong-1.4.0/src/toolong/scan_progress_bar.py` & `toolong-1.5.0/src/toolong/scan_progress_bar.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,15 +13,18 @@
         margin: 2 4;
         dock: top;                    
         padding: 1 2;
         background: $primary;        
         display: block;
         text-align: center;
         display: none;
-        align: center top;        
+        align: center top;       
+        ProgressBar {
+            margin: 1 0;
+        } 
     }
 
     LogLines:focus ScanProgressBar.-has-content {
         display: block;
     }
     """
 
@@ -32,10 +35,10 @@
         self.query_one(".message", Label).update(message)
         self.set_class(bool(message), "-has-content")
 
     def compose(self) -> ComposeResult:
         with Center():
             yield Label(classes="message")
         with Center():
-            yield ProgressBar(
-                total=1.0, show_eta=False, show_percentage=False
-            ).data_bind(progress=ScanProgressBar.complete)
+            yield ProgressBar(total=1.0, show_eta=True, show_percentage=True).data_bind(
+                progress=ScanProgressBar.complete
+            )
```

### Comparing `toolong-1.4.0/src/toolong/selector_watcher.py` & `toolong-1.5.0/src/toolong/selector_watcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         fileno = log_file.fileno
         size = log_file.size
         os.lseek(fileno, size, os.SEEK_SET)
         self._selector.register(fileno, EVENT_READ)
 
     def run(self) -> None:
         """Thread runner."""
-
         chunk_size = 64 * 1024
         scan_chunk = self.scan_chunk
 
         while not self._exit_event.is_set():
             for key, mask in self._selector.select(timeout=0.1):
                 if self._exit_event.is_set():
                     break
```

### Comparing `toolong-1.4.0/src/toolong/timestamps.py` & `toolong-1.5.0/src/toolong/timestamps.py`

 * *Files identical despite different names*

### Comparing `toolong-1.4.0/src/toolong/ui.py` & `toolong-1.5.0/src/toolong/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import locale
 
 from pathlib import Path
 
+from rich import terminal_theme
 from textual.app import App, ComposeResult
 from textual.binding import Binding
 from textual.lazy import Lazy
 from textual.screen import Screen
 from textual.widgets import TabbedContent, TabPane
 
 from toolong.log_view import LogView
@@ -114,13 +115,14 @@
         self.file_paths = self.sort_paths(file_paths)
         self.merge = merge
         self.save_merge = save_merge
         self.watcher = get_watcher()
         super().__init__()
 
     async def on_mount(self) -> None:
+        self.ansi_theme_dark = terminal_theme.DIMMED_MONOKAI
         await self.push_screen(LogScreen())
         self.screen.query("LogLines").focus()
         self.watcher.start()
 
     def on_unmount(self) -> None:
         self.watcher.close()
```

### Comparing `toolong-1.4.0/src/toolong/watcher.py` & `toolong-1.5.0/src/toolong/watcher.py`

 * *Files identical despite different names*

### Comparing `toolong-1.4.0/PKG-INFO` & `toolong-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: toolong
-Version: 1.4.0
+Version: 1.5.0
 Summary: A terminal log file viewer / tailer / analyzer
 Home-page: https://github.com/textualize/toolong
 License: MIT
 Author: Will McGugan
 Author-email: will@textualize.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: textual (>=0.52.0,<0.53.0)
+Requires-Dist: textual (>=0.58.0,<0.59.0)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Documentation, https://github.com/textualize/toolong
 Project-URL: Repository, https://github.com/textualize/toolong
 Description-Content-Type: text/markdown
 
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: toolong Version: 1.4.0 Summary: A terminal log file
+Metadata-Version: 2.1 Name: toolong Version: 1.5.0 Summary: A terminal log file
 viewer / tailer / analyzer Home-page: https://github.com/textualize/toolong
 License: MIT Author: Will McGugan Author-email: will@textualize.io Requires-
 Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: click (>=8.1.7,<9.0.0) Requires-Dist:
-textual (>=0.52.0,<0.53.0) Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
-Project-URL: Documentation, https://github.com/textualize/toolong Project-URL:
-Repository, https://github.com/textualize/toolong Description-Content-Type:
-text/markdown
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0) Requires-Dist: textual (>=0.58.0,<0.59.0)
+Requires-Dist: typing-extensions (>=4.9.0,<5.0.0) Project-URL: Documentation,
+https://github.com/textualize/toolong Project-URL: Repository, https://
+github.com/textualize/toolong Description-Content-Type: text/markdown
                       [A Kookaburra sitting on a scroll]
 [![Discord](https://img.shields.io/discord/1026214085173461072)](https://
 discord.gg/Enf6Z3qhVr) # Toolong A terminal application to view, tail, merge,
 and search log files (plus JSONL). ð¬ Viewing a single file  
 ## Keep calm and log files See [Toolong on Calmcode.io](https://calmcode.io/
 shorts/toolong.py) for a calming introduction to Toolong. ## What? [Screenshot
 2024-02-08 at 13 47 28]- Live tailing of log files. - Syntax highlights common
```

