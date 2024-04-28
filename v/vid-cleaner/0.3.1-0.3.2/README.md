# Comparing `tmp/vid_cleaner-0.3.1.tar.gz` & `tmp/vid_cleaner-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vid_cleaner-0.3.1.tar", max compression
+gzip compressed data, was "vid_cleaner-0.3.2.tar", max compression
```

## Comparing `vid_cleaner-0.3.1.tar` & `vid_cleaner-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0    34523 2024-03-11 17:51:14.806275 vid_cleaner-0.3.1/LICENSE
--rw-r--r--   0        0        0     3039 2024-03-11 17:51:14.806275 vid_cleaner-0.3.1/README.md
--rw-r--r--   0        0        0     8852 2024-03-11 17:51:14.806275 vid_cleaner-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       27 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/__init__.py
--rw-r--r--   0        0        0       98 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/config/__init__.py
--rw-r--r--   0        0        0     1366 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/config/config.py
--rw-r--r--   0        0        0      788 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/constants.py
--rw-r--r--   0        0        0      399 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/default_config.toml
--rw-r--r--   0        0        0       94 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/models/__init__.py
--rw-r--r--   0        0        0    31688 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/models/video_file.py
--rw-r--r--   0        0        0      495 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/utils/__init__.py
--rw-r--r--   0        0        0      113 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/utils/console.py
--rw-r--r--   0        0        0      145 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/utils/errors.py
--rw-r--r--   0        0        0     8320 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/utils/helpers.py
--rw-r--r--   0        0        0     5062 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/utils/logging.py
--rw-r--r--   0        0        0    14859 2024-03-11 17:51:14.810274 vid_cleaner-0.3.1/src/vid_cleaner/vid_cleaner.py
--rw-r--r--   0        0        0     3892 1970-01-01 00:00:00.000000 vid_cleaner-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-28 17:42:29.399076 vid_cleaner-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3039 2024-04-28 17:42:29.399076 vid_cleaner-0.3.2/README.md
+-rw-r--r--   0        0        0     8943 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       27 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/cli/__init__.py
+-rw-r--r--   0        0        0     3810 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/cli/clean.py
+-rw-r--r--   0        0        0     2087 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/cli/clip.py
+-rw-r--r--   0        0        0     1050 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/cli/inspect.py
+-rw-r--r--   0        0        0       98 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/config/__init__.py
+-rw-r--r--   0        0        0     1337 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/config/config.py
+-rw-r--r--   0        0        0     1136 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/constants.py
+-rw-r--r--   0        0        0      399 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/default_config.toml
+-rw-r--r--   0        0        0      148 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/models/__init__.py
+-rw-r--r--   0        0        0    35440 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/models/video_file.py
+-rw-r--r--   0        0        0      495 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/utils/__init__.py
+-rw-r--r--   0        0        0      113 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/utils/console.py
+-rw-r--r--   0        0        0      145 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/utils/errors.py
+-rw-r--r--   0        0        0    10271 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/utils/helpers.py
+-rw-r--r--   0        0        0     6069 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/utils/logging.py
+-rw-r--r--   0        0        0    12160 2024-04-28 17:42:29.403076 vid_cleaner-0.3.2/src/vid_cleaner/vid_cleaner.py
+-rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 vid_cleaner-0.3.2/PKG-INFO
```

### Comparing `vid_cleaner-0.3.1/LICENSE` & `vid_cleaner-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vid_cleaner-0.3.1/README.md` & `vid_cleaner-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `vid_cleaner-0.3.1/pyproject.toml` & `vid_cleaner-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,49 +7,51 @@
     description = "Tools to transcode, inspect and convert videos."
     homepage    = "https://github.com/natelandau/vid-cleaner"
     keywords    = []
     license     = ""
     name        = "vid-cleaner"
     readme      = "README.md"
     repository  = "https://github.com/natelandau/vid-cleaner"
-    version     = "0.3.1"
+    version     = "0.3.2"
 
     [tool.poetry.scripts] # https://python-poetry.org/docs/pyproject/#scripts
         vidcleaner = "vid_cleaner.vid_cleaner:app"
 
     [tool.poetry.dependencies]
         confz                 = "^2.0.1"
         ffmpeg-progress-yield = "^0.7.8"
         ffmpeg-python         = "^0.2.0"
         iso639-lang           = "^2.2.3"
         loguru                = "^0.7.2"
         python                = "^3.11"
         requests              = "^2.31.0"
         rich                  = "^13.7.1"
-        typer                 = { extras = ["all"], version = "^0.9.0" }
+        shellingham           = "^1.5.4"
+        typer                 = "^0.12.3"
 
     [tool.poetry.group.test.dependencies]
-        pytest                 = "^8.1.1"
+        pytest                 = "^8.2.0"
         pytest-clarity         = "^1.0.1"
         pytest-env             = "^1.1.3"
         pytest-mock            = "^3.12.0"
         pytest-pretty-terminal = "^1.1.0"
         pytest-sugar           = "^1.0.0"
         pytest-xdist           = "^3.5.0"
 
     [tool.poetry.group.dev.dependencies]
-        commitizen     = "^3.18.2"
-        coverage       = "^7.4.3"
-        mypy           = "^1.9.0"
+        commitizen     = "^3.24.0"
+        coverage       = "^7.5.0"
+        mypy           = "^1.10.0"
         poethepoet     = "^0.25.0"
-        pre-commit     = "^3.6.2"
+        pre-commit     = "^3.7.0"
         pytest-asyncio = "^0.23.5.post1"
-        ruff           = "^0.3.2"
+        ruff           = "^0.4.2"
         types-requests = "^2.31.0.20240311"
-        typos          = "^1.19.0"
+        typos          = "^1.20.10"
+        yamllint       = "^1.35.1"
 
 [tool.commitizen]
     bump_message               = "bump(release): v$current_version → v$new_version"
     changelog_merge_prerelease = true
     tag_format                 = "v$version"
     update_changelog_on_bump   = true
     version_files              = ["src/vid_cleaner/constants.py:VERSION"]
@@ -167,17 +169,19 @@
         ignore-init-module-imports = true
         per-file-ignores = { "cli.py" = [
             "PLR0912",
             "PLR0913",
         ], "tests/*.py" = [
             "A002",
             "A003",
+            "ARG001",
             "ARG002",
             "ARG005",
             "D102",
+            "ERA001",
             "F403",
             "PGH003",
             "PLR0913",
             "PLR0917",
             "PLR2004",
             "PLR6301",
             "S101",
```

### Comparing `vid_cleaner-0.3.1/src/vid_cleaner/config/config.py` & `vid_cleaner-0.3.2/src/vid_cleaner/config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 from vid_cleaner.constants import APP_DIR, CONFIG_PATH
 
 PATH_CONFIG_DEFAULT = Path(__file__).parent / "default_config.toml"
 
 
 def pass_opt_without_value(value: str) -> bool:
     """Confz does not work well with Typer options. Confz requires a value for each CLI option, but Typer does not. To workaround this, for example, if --log-to-file is passed, we set the value to "True" regardless of what follows the CLI option."""
-    if value:
-        return True
-
-    return False
+    return bool(value)
 
 
 OPT_BOOLEAN = Annotated[
     bool,
     BeforeValidator(pass_opt_without_value),
 ]
```

### Comparing `vid_cleaner-0.3.1/src/vid_cleaner/constants.py` & `vid_cleaner-0.3.2/src/vid_cleaner/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,34 @@
 
 from enum import Enum
 from pathlib import Path
 
 import typer
 
 
+class VideoContainerTypes(str, Enum):
+    """Video container types for vid-cleaner."""
+
+    MKV = ".mkv"
+    MP4 = ".mp4"
+    AVI = ".avi"
+    WEBM = ".webm"
+    MOV = ".mov"
+    WMV = ".wmv"
+    M4V = ".m4v"
+
+
+class CodecTypes(str, Enum):
+    """Codec types for vid-cleaner."""
+
+    AUDIO = "audio"
+    VIDEO = "video"
+    SUBTITLE = "subtitle"
+
+
 class AudioLayout(Enum):
     """Audio layouts for vid-cleaner. Values are the number of streams."""
 
     MONO = 1
     STEREO = 2
     SURROUND5 = 6
     SURROUND7 = 8
@@ -19,13 +39,13 @@
 
 APP_DIR = Path(typer.get_app_dir("vid-cleaner"))
 CONFIG_PATH = APP_DIR / "config.toml"
 EXCLUDED_VIDEO_CODECS = {"mjpeg", "mjpg", "png"}
 FFMPEG_APPEND: list[str] = ["-max_muxing_queue_size", "9999"]
 FFMPEG_PREPEND: list[str] = ["-y", "-hide_banner"]
 H265_CODECS = {"hevc", "vp9"}
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 
 # how many bytes to read at once?
 # shutil.copy uses 1024 * 1024 if _WINDOWS else 64 * 1024
 # however, in my testing on MacOS with SSD, I've found a much larger buffer is faster
 BUFFER_SIZE = 4096 * 1024
```

### Comparing `vid_cleaner-0.3.1/src/vid_cleaner/models/video_file.py` & `vid_cleaner-0.3.2/src/vid_cleaner/models/video_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """VideoFile model."""
 
 import atexit
 import re
 import uuid
 from pathlib import Path
+from typing import Optional
 
 import typer
 from ffmpeg_progress_yield import FfmpegProgress
 from iso639 import Lang
 from loguru import logger
+from pydantic import BaseModel
 from rich.progress import Progress
+from rich.table import Table
 
 from vid_cleaner.constants import (
     APP_DIR,
     EXCLUDED_VIDEO_CODECS,
     FFMPEG_APPEND,
     FFMPEG_PREPEND,
     H265_CODECS,
     SYMBOL_CHECK,
     AudioLayout,
+    CodecTypes,
 )
 from vid_cleaner.utils import console, ffprobe, query_radarr, query_sonarr, query_tmdb
 
 
 def cleanup_on_exit(video_file: "VideoFile") -> None:  # pragma: no cover
     """Cleanup temporary files on exit.
 
@@ -31,14 +35,122 @@
 
     Returns:
         None
     """
     video_file.cleanup()
 
 
+class VideoStream(BaseModel):
+    """VideoStream model."""
+
+    index: int
+    codec_name: str
+    codec_long_name: str
+    codec_type: CodecTypes
+    duration: Optional[str]
+    width: Optional[int]
+    height: Optional[int]
+    bps: Optional[int]
+    sample_rate: Optional[int]
+    language: Optional[str]
+    channels: Optional[AudioLayout]
+    channel_layout: Optional[str]
+    layout: Optional[str]
+    title: Optional[str]
+
+
+class VideoProbe(BaseModel):
+    """VideoProbe model."""
+
+    name: str
+    streams: list[VideoStream]
+    format_name: Optional[str]
+    format_long_name: Optional[str]
+    duration: Optional[str]
+    start_time: Optional[float]
+    size: Optional[int]
+    bit_rate: Optional[int]
+    json_data: dict
+
+    @classmethod
+    def parse_probe_response(cls, json_obj: dict, stem: str) -> "VideoProbe":
+        """Parse ffprobe json object."""
+        # Find name
+        if "title" in json_obj["format"]["tags"]:
+            name = json_obj["format"]["tags"]["title"]
+        elif "filename" in json_obj["format"]:
+            name = json_obj["format"]["filename"]
+        else:
+            name = stem
+
+        # Find streams
+        streams = [
+            VideoStream(
+                index=stream["index"],
+                codec_name=stream["codec_name"],
+                codec_long_name=stream["codec_long_name"],
+                codec_type=CodecTypes(stream["codec_type"].lower()),
+                duration=stream.get("duration", None),
+                width=stream.get("width", None),
+                height=stream.get("height", None),
+                bps=stream.get("tags", {}).get("BPS", None),
+                sample_rate=stream.get("sample_rate", None),
+                language=stream.get("language", None)
+                or stream.get("tags", {}).get("language", None),
+                channels=AudioLayout(stream.get("channels"))
+                if stream.get("channels", False)
+                else None,
+                channel_layout=stream.get("channel_layout", None),
+                layout=stream.get("layout", None),
+                title=stream.get("tags", {}).get("title", None),
+            )
+            for stream in json_obj["streams"]
+        ]
+
+        return cls(
+            name=name,
+            format_name=json_obj["format"].get("format_name", None),
+            format_long_name=json_obj["format"].get("format_long_name", None),
+            duration=json_obj["format"].get("duration", None),
+            start_time=json_obj["format"].get("start_time", None),
+            size=json_obj["format"].get("size", None),
+            bit_rate=json_obj["format"].get("bit_rate", None),
+            streams=streams,
+            json_data=json_obj,
+        )
+
+    def as_table(self) -> Table:
+        """Return the video probe as a rich table."""
+        table = Table(title=self.name)
+        table.add_column("#")
+        table.add_column("Type")
+        table.add_column("Codec Name")
+        table.add_column("Language")
+        table.add_column("Channels")
+        table.add_column("Channel Layout")
+        table.add_column("Width")
+        table.add_column("Height")
+        table.add_column("Title")
+
+        for stream in self.streams:
+            table.add_row(
+                str(stream.index),
+                stream.codec_type.value,
+                stream.codec_name,
+                stream.language,
+                str(stream.channels.value) if stream.channels else "",
+                stream.channel_layout or "",
+                str(stream.width) if stream.width else "",
+                str(stream.height) if stream.height else "",
+                stream.title or "",
+            )
+
+        return table
+
+
 class VideoFile:
     """VideoFile model."""
 
     def __init__(self, path: Path):
         """Initialize VideoFile."""
         self.path = path.expanduser().resolve()
         self.name = path.name
@@ -54,201 +166,48 @@
         self.current_tmp_file: Path | None = None  # Current temporary file
         self.tmp_files: list[Path] = []  # All temporary files created by this VideoFile
         self.tmp_file_number = 1
 
         # Register cleanup on exit
         atexit.register(cleanup_on_exit, self)
 
-    def _convert_to_h265(
-        self,
-        force: bool = False,
-        dry_run: bool = False,
-    ) -> Path:
-        """Convert the video to H.265 codec format.
-
-        Check if conversion is necessary and perform it if so. This involves calculating the
-        bitrate, building the ffmpeg command, and running it. Return the path to the converted
-        video or the original video if conversion isn't needed.
-
-        Args:
-            force (bool, optional): Flag to force conversion even if the video is already H.265. Defaults to False.
-            dry_run (bool, optional): Run in dry run mode. Defaults to False.
-
-        Returns:
-            Path: Path to the converted or original video file.
-        """
-        input_path, _ = self._get_input_and_output()
-
-        # Get ffprobe probe
-        probe = self._get_probe()
-        video_stream = [  # noqa: RUF015
-            stream
-            for stream in probe["streams"]
-            if stream["codec_type"].lower() == "video"
-            and stream["codec_name"].lower() not in EXCLUDED_VIDEO_CODECS
-        ][0]
-
-        # Fail if no video stream is found
-        if not video_stream:
-            logger.error("No video stream found")
-            return input_path
-
-        # Return if video is already H.265
-        if not force and video_stream["codec_name"].lower() in H265_CODECS:
-            logger.warning(
-                "H265 ENCODE: Video already H.265 or VP9. Run with `--force` to re-encode. Skipping"
-            )
-            return input_path
-
-        # Calculate Bitrate
-        # ############################
-        # Check if duration info is filled, if so times it by 0.0166667 to get time in minutes.
-        # If not filled then get duration of stream 0 and do the same.
-        stream_duration = float(probe["format"].get("duration", None)) or float(
-            video_stream.get("duration", None)
-        )
-        if not stream_duration:
-            logger.error("Could not calculate video duration")
-            return input_path
-
-        duration = stream_duration * 0.0166667
-
-        # Work out currentBitrate using "Bitrate = file size / (number of minutes * .0075)"
-        # Used from here https://blog.frame.io/2017/03/06/calculate-video-bitrates/
-        stat = input_path.stat()
-        file_size_megabytes = stat.st_size / 1000000
-
-        current_bitrate = int(file_size_megabytes / (duration * 0.0075))
-        target_bitrate = int(file_size_megabytes / (duration * 0.0075) / 2)
-        min_bitrate = int(current_bitrate * 0.7)
-        max_bitrate = int(current_bitrate * 1.3)
-
-        # Build FFMPEG Command
-        command: list[str] = ["-map", "0", "-c:v", "libx265"]
-
-        # Create bitrate command
-        command.extend(
-            [
-                "-b:v",
-                f"{target_bitrate}k",
-                "-minrate",
-                f"{min_bitrate}k",
-                "-maxrate",
-                f"{max_bitrate}k",
-                "-bufsize",
-                f"{current_bitrate}k",
-            ]
-        )
-
-        # Copy audio and subtitles
-        command.extend(["-c:a", "copy", "-c:s", "copy"])
-
-        # Run ffmpeg
-        return self._run_ffmpeg(command, title="Convert to H.265", step="h265", dry_run=dry_run)
-
-    def _convert_to_vp9(
-        self,
-        force: bool = False,
-        dry_run: bool = False,
-    ) -> Path:
-        """Convert the video to the VP9 codec format.
-
-        Verify if conversion is required and proceed with it using ffmpeg. This method specifically
-        targets the VP9 video codec. Return the path to the converted video or the original video
-        if conversion is not necessary.
-
-        Args:
-            dry_run (bool, optional): Run in dry run mode. Defaults to False.
-            force (bool, optional): Flag to force conversion even if the video is already VP9. Defaults to False.
-
-        Returns:
-            Path: Path to the converted or original video file.
-        """
-        input_path, _ = self._get_input_and_output()
-
-        # Get ffprobe probe
-        probe = self._get_probe()
-        video_stream = [  # noqa: RUF015
-            stream
-            for stream in probe["streams"]
-            if stream["codec_type"].lower() == "video"
-            and stream["codec_name"].lower() not in EXCLUDED_VIDEO_CODECS
-        ][0]
-
-        # Fail if no video stream is found
-        if not video_stream:
-            logger.error("No video stream found")
-            return input_path
-
-        # Return if video is already H.265
-        if not force and video_stream["codec_name"].lower() in H265_CODECS:
-            logger.warning(
-                "VP9 ENCODE: Video already H.265 or VP9. Run with `--force` to re-encode. Skipping"
-            )
-            return input_path
-
-        # Build ffmpeg command
-        command: list[str] = [
-            "-map",
-            "0",
-            "-c:v",
-            "libvpx-vp9",
-            "-b:v",
-            "0",
-            "-crf",
-            "30",
-            "-c:a",
-            "libvorbis",
-            "-dn",
-            "-map_chapters",
-            "-1",
-        ]
-
-        # Copy subtitles
-        command.extend(["-c:s", "copy"])
-
-        # Run ffmpeg
-        return self._run_ffmpeg(
-            command, title="Convert to vp9", suffix=".webm", step="vp9", dry_run=dry_run
-        )
-
     @staticmethod
-    def _downmix_to_stereo(streams: list[dict]) -> list[str]:
+    def _downmix_to_stereo(streams: list[VideoStream]) -> list[str]:
         """Generate a partial ffmpeg command to downmix audio streams to stereo if needed.
 
         Analyze the provided audio streams and construct a command to downmix 5.1 or 7.1 audio
         streams to stereo. Handle cases where stereo is already present or needs to be created
         from surround sound streams.
 
         Args:
-            streams (list[dict]): List of audio stream dictionaries.
+            streams (list[VideoStream]): List of audio stream dictionaries.
 
         Returns:
             list[str]: A list of strings forming part of an ffmpeg command for audio downmixing.
         """
         downmix_command: list[str] = []
         new_index = 0
         has_stereo = False
         surround5 = []  # index of 5.1 streams
         surround7 = []  # index of 7.1 streams
 
         for stream in streams:
-            if stream["channels"] == AudioLayout.STEREO.value:
+            if stream.channels == AudioLayout.STEREO:
                 has_stereo = True
-            if stream["channels"] == AudioLayout.SURROUND5.value:
+            if stream.channels == AudioLayout.SURROUND5:
                 surround5.append(stream)
-            if stream["channels"] == AudioLayout.SURROUND7.value:
+            if stream.channels == AudioLayout.SURROUND7:
                 surround7.append(stream)
 
         if not has_stereo and surround5:
             for surround5_stream in surround5:
                 downmix_command.extend(
                     [
                         "-map",
-                        f"0:{surround5_stream['index']}",
+                        f"0:{surround5_stream.index}",
                         f"-c:a:{new_index}",
                         "aac",
                         f"-ac:a:{new_index}",
                         "2",
                         f"-b:a:{new_index}",
                         "256k",
                         f"-filter:a:{new_index}",
@@ -267,15 +226,15 @@
                 "PROCESS AUDIO: Audio track is 5 channel, no 2 channel exists. Creating 2 channel from 5 channel"
             )
 
             for surround7_stream in surround7:
                 downmix_command.extend(
                     [
                         "-map",
-                        f"0:{surround7_stream['index']}",
+                        f"0:{surround7_stream.index}",
                         f"-c:a:{new_index}",
                         "aac",
                         f"-ac:a:{new_index}",
                         "2",
                         f"-b:a:{new_index}",
                         "256k",
                         f"-metadata:s:a:{new_index}",
@@ -332,32 +291,26 @@
             return None
 
         # Set language attribute
         self.language = language
         self.ran_language_check = True
         return language
 
-    def _get_probe(self, key: str | None = None) -> dict:  # pragma: no cover
+    def _get_probe(self) -> VideoProbe:  # pragma: no cover
         """Retrieve the ffprobe probe information for the video.
 
         Fetch detailed information about the video file using ffprobe. Optionally filter
         the information by a specific key.
 
-        Args:
-            key (str | None, optional): A specific key to filter the probe information. Default is None.
-
         Returns:
-            dict: The ffprobe probe information.
+            VideoProbe: The ffprobe probe information.
         """
         input_path, _ = self._get_input_and_output()
 
-        if key:
-            return ffprobe(input_path)[key]
-
-        return ffprobe(input_path)
+        return VideoProbe.parse_probe_response(ffprobe(input_path), self.stem)
 
     def _get_input_and_output(
         self, suffix: str | None = None, step: str | None = None
     ) -> tuple[Path, Path]:
         """Determine input and output file paths for processing steps.
 
         Calculate the paths based on the current state of the video file, its temporary directory,
@@ -370,15 +323,15 @@
         Returns:
             tuple[Path, Path]: A tuple containing the input and output file paths.
         """
         # Input file is most recent temp file or self.path
         input_file = self.tmp_files[-1] if self.tmp_files else self.path
 
         # Get the output file name
-        suffix = suffix if suffix else self.suffix
+        suffix = suffix or self.suffix
         self.tmp_dir.mkdir(parents=True, exist_ok=True)
 
         # Create a new tmp file name
         for file in self.tmp_dir.iterdir():
             if file.stem.startswith(f"{self.tmp_file_number}_"):
                 self.tmp_file_number += 1
 
@@ -389,90 +342,53 @@
             if file != input_file:
                 logger.trace(f"Remove: {file}")
                 file.unlink()
 
         return input_file, output_file
 
     @staticmethod
-    def _process_video(streams: list[dict]) -> list[str]:
+    def _process_video(streams: list[VideoStream]) -> list[str]:
         """Create a command list for processing video streams.
 
         Iterate through the provided video streams and construct a list of ffmpeg commands
         to process them, excluding any streams with codecs in the exclusion list.
 
         Args:
             streams (list[dict]): A list of video stream dictionaries.
 
         Returns:
             list[str]: A list of strings forming part of an ffmpeg command for video processing.
         """
         command: list[str] = []
         for stream in streams:
-            if stream["codec_name"].lower() in EXCLUDED_VIDEO_CODECS:
+            if stream.codec_name.lower() in EXCLUDED_VIDEO_CODECS:
                 continue
 
-            command.extend(["-map", f"0:{stream['index']}"])
+            command.extend(["-map", f"0:{stream.index}"])
 
         logger.trace(f"PROCESS VIDEO: {command}")
         return command
 
-    def video_to_1080p(self, force: bool = False, dry_run: bool = False) -> Path:
-        """Convert the video to 1080p resolution."""
-        input_path, _ = self._get_input_and_output()
-
-        # Get ffprobe probe
-        probe = self._get_probe()
-
-        video_stream = [  # noqa: RUF015
-            stream
-            for stream in probe["streams"]
-            if stream["codec_type"].lower() == "video"
-            and stream["codec_name"].lower() not in EXCLUDED_VIDEO_CODECS
-        ][0]
-
-        # Fail if no video stream is found
-        if not video_stream:
-            logger.error("No video stream found")
-            return input_path
-
-        # Return if video is not 4K
-        if not force and video_stream.get("width", 0) <= 1920:  # noqa: PLR2004
-            logger.info(f"{SYMBOL_CHECK} No convert to 1080p needed")
-            return input_path
-
-        # Build ffmpeg command
-        command: list[str] = [
-            "-filter:v",
-            "scale=width=1920:height=-2",
-            "-c:a",
-            "copy",
-            "-c:s",
-            "copy",
-        ]
-
-        # Run ffmpeg
-        return self._run_ffmpeg(command, title="Convert to 1080p", step="1080p", dry_run=dry_run)
-
     def _process_subtitles(
         self,
-        streams: list[dict],
+        streams: list[VideoStream],
         langs_to_keep: list[str],
         keep_commentary: bool,
         keep_all_subtitles: bool,
         keep_local_subtitles: bool,
         verbosity: int,
         subs_drop_local: bool = False,
     ) -> list[str]:
         """Construct a command list for processing subtitle streams.
 
         Analyze and filter subtitle streams based on language preferences, commentary options,
         and other criteria. Build an ffmpeg command list accordingly.
 
         Args:
-            streams (list[dict]): A list of subtitle stream dictionaries.
+            streams (list[VideoStream]): A list of subtitle stream objects.
             langs_to_keep (list[str]): Languages of subtitles to keep.
             keep_commentary (bool): Flag to keep or discard commentary subtitles.
             keep_all_subtitles (bool): Flag to keep all subtitles regardless of language.
             keep_local_subtitles (bool): Flag to keep subtitles with 'undetermined' language or in the specified list.
             subs_drop_local (bool, optional): Drop subtitles if the original language is not in the list. Defaults to False.
             verbosity (int): The verbosity level of the logger.
 
@@ -490,107 +406,110 @@
         # Return no streams if no languages are specified
         if not keep_all_subtitles and not keep_local_subtitles and subs_drop_local:
             return command
 
         for stream in streams:
             if (
                 not keep_commentary
-                and "title" in stream["tags"]
-                and re.search(r"commentary|sdh|description", stream["tags"]["title"], re.IGNORECASE)
+                and stream.title is not None
+                and re.search(r"commentary|sdh|description", stream.title, re.IGNORECASE)
             ):
+                logger.trace(rf"PROCESS SUBTITLES: Remove stream #{stream.index} \[commentary]")
                 continue
 
             if keep_all_subtitles:
-                command.extend(["-map", f"0:{stream['index']}"])
+                command.extend(["-map", f"0:{stream.index}"])
                 continue
 
-            if "tags" in stream and "language" in stream["tags"]:
+            if stream.language:
                 if keep_local_subtitles and (
-                    stream["tags"]["language"].lower() == "und"
-                    or Lang(stream["tags"]["language"]) in langs
+                    stream.language.lower() == "und" or Lang(stream.language) in langs
                 ):
-                    command.extend(["-map", f"0:{stream['index']}"])
+                    command.extend(["-map", f"0:{stream.index}"])
                     continue
 
                 if (
                     not subs_drop_local
                     and langs
                     and original_language not in langs
-                    and (
-                        stream["tags"]["language"].lower == "und"
-                        or Lang(stream["tags"]["language"]) in langs
-                    )
+                    and (stream.language.lower == "und" or Lang(stream.language) in langs)
                 ):
-                    command.extend(["-map", f"0:{stream['index']}"])
+                    command.extend(["-map", f"0:{stream.index}"])
                     continue
 
+            logger.trace(f"PROCESS SUBTITLES: Remove stream #{stream.index}")
+
         logger.trace(f"PROCESS SUBTITLES: {command}")
         return command
 
     def _process_audio(
         self,
-        streams: list[dict],
+        streams: list[VideoStream],
         langs_to_keep: list[str],
         drop_original_audio: bool,
         keep_commentary: bool,
         downmix_stereo: bool,
         verbosity: int,
     ) -> tuple[list[str], list[str]]:
         """Construct commands for processing audio streams.
 
         Analyze and process audio streams based on language, commentary, and downmixing criteria.
         Generate ffmpeg commands for keeping or altering audio streams as required.
 
         Args:
-            streams (list[dict]): A list of audio stream dictionaries.
+            streams (list[VideoStream]): A list of audio stream objects.
             langs_to_keep (list[str]): Languages of audio to keep.
             drop_original_audio (bool): Flag to drop the original audio track.
             keep_commentary (bool): Flag to keep or discard commentary audio tracks.
             downmix_stereo (bool): Flag to downmix to stereo if required.
             verbosity (int): The verbosity level of the logger.
 
         Returns:
             tuple[list[str], list[str]]: A tuple containing two lists of strings forming part of an ffmpeg command for audio processing.
         """
         command: list[str] = []
+
         # Turn language codes into iso639 objects
         langs = [Lang(lang) for lang in langs_to_keep]
 
         # Add original language to list of languages to keep
         if not drop_original_audio:
             original_language = self._find_original_language(verbosity=verbosity)
             if original_language and original_language not in langs:
                 langs.append(original_language)
 
         streams_to_keep = []
         for stream in streams:
             # Keep unknown language streams
-            if "tags" not in stream or "language" not in stream["tags"]:
-                command.extend(["-map", f"0:{stream['index']}"])
+            if not stream.language:
+                command.extend(["-map", f"0:{stream.index}"])
                 streams_to_keep.append(stream)
                 continue
 
             # Remove commentary streams
             if (
                 not keep_commentary
-                and "title" in stream["tags"]
-                and re.search(r"commentary|sdh|description", stream["tags"]["title"], re.IGNORECASE)
+                and stream.title
+                and re.search(r"commentary|sdh|description", stream.title, re.IGNORECASE)
             ):
+                logger.trace(rf"PROCESS AUDIO: Remove stream #{stream.index} \[commentary]")
                 continue
 
             # Keep streams with specified languages
-            if stream["tags"]["language"] == "und" or Lang(stream["tags"]["language"]) in langs:
-                command.extend(["-map", f"0:{stream['index']}"])
+            if stream.language == "und" or Lang(stream.language) in langs:
+                command.extend(["-map", f"0:{stream.index}"])
                 streams_to_keep.append(stream)
                 continue
 
+            logger.trace(f"PROCESS AUDIO: Remove stream #{stream.index}")
+
         # Failsafe to cancel processing if all streams would be removed following this plugin. We don't want no audio.
         if not command:
             for stream in streams:
-                command.extend(["-map", f"0:{stream['index']}"])
+                command.extend(["-map", f"0:{stream.index}"])
                 streams_to_keep.append(stream)
 
         # Downmix to stereo if needed
         downmix_command = self._downmix_to_stereo(streams_to_keep) if downmix_stereo else []
 
         logger.trace(f"PROCESS AUDIO: {command}")
         return command, downmix_command
@@ -705,14 +624,165 @@
         """
         # Build ffmpeg command
         ffmpeg_command: list[str] = ["-ss", start, "-t", duration, "-map", "0", "-c", "copy"]
 
         # Run ffmpeg
         return self._run_ffmpeg(ffmpeg_command, title="Clip video", step="clip", dry_run=dry_run)
 
+    def convert_to_h265(
+        self,
+        force: bool = False,
+        dry_run: bool = False,
+    ) -> Path:
+        """Convert the video to H.265 codec format.
+
+        Check if conversion is necessary and perform it if so. This involves calculating the
+        bitrate, building the ffmpeg command, and running it. Return the path to the converted
+        video or the original video if conversion isn't needed.
+
+        Args:
+            force (bool, optional): Flag to force conversion even if the video is already H.265. Defaults to False.
+            dry_run (bool, optional): Run in dry run mode. Defaults to False.
+
+        Returns:
+            Path: Path to the converted or original video file.
+        """
+        input_path, _ = self._get_input_and_output()
+
+        # Get ffprobe probe
+        probe = self._get_probe()
+        video_stream = [  # noqa: RUF015
+            stream
+            for stream in probe.streams
+            if stream.codec_type == CodecTypes.VIDEO
+            and stream.codec_name.lower() not in EXCLUDED_VIDEO_CODECS
+        ][0]
+
+        # Fail if no video stream is found
+        if not video_stream:
+            logger.error("No video stream found")
+            return input_path
+
+        # Return if video is already H.265
+        if not force and video_stream.codec_name.lower() in H265_CODECS:
+            logger.warning(
+                "H265 ENCODE: Video already H.265 or VP9. Run with `--force` to re-encode. Skipping"
+            )
+            return input_path
+
+        # Calculate Bitrate
+        # ############################
+        # Check if duration info is filled, if so times it by 0.0166667 to get time in minutes.
+        # If not filled then get duration of stream 0 and do the same.
+        stream_duration = float(probe.duration) or float(video_stream.duration)
+        if not stream_duration:
+            logger.error("Could not calculate video duration")
+            return input_path
+
+        duration = stream_duration * 0.0166667
+
+        # Work out currentBitrate using "Bitrate = file size / (number of minutes * .0075)"
+        # Used from here https://blog.frame.io/2017/03/06/calculate-video-bitrates/
+
+        stat = input_path.stat()
+        logger.trace(f"File size: {stat}")
+        file_size_megabytes = stat.st_size / 1000000
+
+        current_bitrate = int(file_size_megabytes / (duration * 0.0075))
+        target_bitrate = int(file_size_megabytes / (duration * 0.0075) / 2)
+        min_bitrate = int(current_bitrate * 0.7)
+        max_bitrate = int(current_bitrate * 1.3)
+
+        # Build FFMPEG Command
+        command: list[str] = ["-map", "0", "-c:v", "libx265"]
+        # Create bitrate command
+        command.extend(
+            [
+                "-b:v",
+                f"{target_bitrate}k",
+                "-minrate",
+                f"{min_bitrate}k",
+                "-maxrate",
+                f"{max_bitrate}k",
+                "-bufsize",
+                f"{current_bitrate}k",
+            ]
+        )
+
+        # Copy audio and subtitles
+        command.extend(["-c:a", "copy", "-c:s", "copy"])
+        # Run ffmpeg
+        return self._run_ffmpeg(command, title="Convert to H.265", step="h265", dry_run=dry_run)
+
+    def convert_to_vp9(
+        self,
+        force: bool = False,
+        dry_run: bool = False,
+    ) -> Path:
+        """Convert the video to the VP9 codec format.
+
+        Verify if conversion is required and proceed with it using ffmpeg. This method specifically
+        targets the VP9 video codec. Return the path to the converted video or the original video
+        if conversion is not necessary.
+
+        Args:
+            dry_run (bool, optional): Run in dry run mode. Defaults to False.
+            force (bool, optional): Flag to force conversion even if the video is already VP9. Defaults to False.
+
+        Returns:
+            Path: Path to the converted or original video file.
+        """
+        input_path, _ = self._get_input_and_output()
+
+        # Get ffprobe probe
+        probe = self._get_probe()
+        video_stream = [  # noqa: RUF015
+            stream
+            for stream in probe.streams
+            if stream.codec_type == CodecTypes.VIDEO
+            and stream.codec_name.lower() not in EXCLUDED_VIDEO_CODECS
+        ][0]
+
+        # Fail if no video stream is found
+        if not video_stream:
+            logger.error("No video stream found")
+            return input_path
+
+        # Return if video is already H.265
+        if not force and video_stream.codec_name.lower() in H265_CODECS:
+            logger.warning(
+                "VP9 ENCODE: Video already H.265 or VP9. Run with `--force` to re-encode. Skipping"
+            )
+            return input_path
+
+        # Build ffmpeg command
+        command: list[str] = [
+            "-map",
+            "0",
+            "-c:v",
+            "libvpx-vp9",
+            "-b:v",
+            "0",
+            "-crf",
+            "30",
+            "-c:a",
+            "libvorbis",
+            "-dn",
+            "-map_chapters",
+            "-1",
+        ]
+
+        # Copy subtitles
+        command.extend(["-c:s", "copy"])
+
+        # Run ffmpeg
+        return self._run_ffmpeg(
+            command, title="Convert to vp9", suffix=".webm", step="vp9", dry_run=dry_run
+        )
+
     def process_streams(
         self,
         langs_to_keep: list[str],
         drop_original_audio: bool,
         keep_commentary: bool,
         downmix_stereo: bool,
         keep_all_subtitles: bool,
@@ -735,20 +805,19 @@
             keep_local_subtitles (bool): Flag to keep subtitles with 'undetermined' language or in the specified list.
             subs_drop_local (bool): Flag to drop subtitles if the original language is not in the list.
             verbosity (int): The verbosity level of the logger.
 
         Returns:
             Path: Path to the processed video file.
         """
-        streams = self._get_probe("streams")
-        video_streams = [stream for stream in streams if stream["codec_type"].lower() == "video"]
-        audio_streams = [stream for stream in streams if stream["codec_type"].lower() == "audio"]
-        subtitle_streams = [
-            stream for stream in streams if stream["codec_type"].lower() == "subtitle"
-        ]
+        probe = self._get_probe()
+
+        video_streams = [s for s in probe.streams if s.codec_type == CodecTypes.VIDEO]
+        audio_streams = [s for s in probe.streams if s.codec_type == CodecTypes.AUDIO]
+        subtitle_streams = [s for s in probe.streams if s.codec_type == CodecTypes.SUBTITLE]
 
         video_map_command = self._process_video(video_streams)
         audio_map_command, downmix_command = self._process_audio(
             streams=audio_streams,
             langs_to_keep=langs_to_keep,
             drop_original_audio=drop_original_audio,
             keep_commentary=keep_commentary,
@@ -784,53 +853,96 @@
         """Reorder the media streams within the video file.
 
         Arrange the streams in the video file so that video streams appear first, followed by audio streams, and then subtitle streams. Exclude certain types of video streams like 'mjpeg' and 'png'.
 
         Returns:
             Path: Path to the video file with reordered streams.
         """
-        streams = self._get_probe("streams")
+        probe = self._get_probe()
 
-        # Categorize streams
-        categorized_streams: dict[str, list[dict]] = {"video": [], "audio": [], "subtitle": []}
-        for stream in streams:
-            codec_type = stream["codec_type"]
-            if codec_type in categorized_streams and (
-                codec_type != "video" or stream["codec_name"].lower() not in EXCLUDED_VIDEO_CODECS
-            ):
-                categorized_streams[codec_type].append(stream)
+        video_streams = [
+            s
+            for s in probe.streams
+            if s.codec_type == CodecTypes.VIDEO
+            and s.codec_name.lower() not in EXCLUDED_VIDEO_CODECS
+        ]
+        audio_streams = [s for s in probe.streams if s.codec_type == CodecTypes.AUDIO]
+        subtitle_streams = [s for s in probe.streams if s.codec_type == CodecTypes.SUBTITLE]
 
         # Fail if no video or audio streams are found
-        if not categorized_streams["video"]:
+        if not video_streams:
             logger.error("No video streams found")
             raise typer.Exit(1)
-        if not categorized_streams["audio"]:
+        if not audio_streams:
             logger.error("No audio streams found")
             raise typer.Exit(1)
 
         # Check if reordering is needed
         reorder = any(
-            stream["index"] != i
-            for i, stream in enumerate(
-                categorized_streams["video"]
-                + categorized_streams["audio"]
-                + categorized_streams["subtitle"]
-            )
+            stream.index != i
+            for i, stream in enumerate(video_streams + audio_streams + subtitle_streams)
         )
 
         if not reorder:
             logger.info(f"{SYMBOL_CHECK} No streams to reorder")
             input_path, _ = self._get_input_and_output()
             return input_path
 
-        # Build ffmpeg command
-        command = sum(
-            [
-                ["-map", f"0:{stream['index']}"]
-                for stream_type in categorized_streams
-                for stream in categorized_streams[stream_type]
-            ],
-            start=["-c", "copy"],
-        )
+        # Initial command parts
+        initial_command = ["-c", "copy"]
+
+        # Build the command list using list comprehension and concatenation
+        command = initial_command + [
+            item
+            for stream_list in [video_streams, audio_streams, subtitle_streams]
+            for stream in stream_list
+            for item in ["-map", f"0:{stream.index}"]
+        ]
 
         # Run ffmpeg
         return self._run_ffmpeg(command, title="Reorder streams", step="reorder", dry_run=dry_run)
+
+    def video_to_1080p(self, force: bool = False, dry_run: bool = False) -> Path:
+        """Convert the video to 1080p resolution."""
+        input_path, _ = self._get_input_and_output()
+
+        # Get ffprobe probe
+        probe = self._get_probe()
+
+        video_stream = [  # noqa: RUF015
+            stream
+            for stream in probe.streams
+            if stream.codec_type == CodecTypes.VIDEO
+            and stream.codec_type.value not in EXCLUDED_VIDEO_CODECS
+        ][0]
+
+        # Fail if no video stream is found
+        if not video_stream:
+            logger.error("No video stream found")
+            return input_path
+
+        # Return if video is not 4K
+        if not force and getattr(video_stream, "width", 0) <= 1920:  # noqa: PLR2004
+            logger.info(f"{SYMBOL_CHECK} No convert to 1080p needed")
+            return input_path
+
+        # Build ffmpeg command
+        command: list[str] = [
+            "-filter:v",
+            "scale=width=1920:height=-2",
+            "-c:a",
+            "copy",
+            "-c:s",
+            "copy",
+        ]
+
+        # Run ffmpeg
+        return self._run_ffmpeg(command, title="Convert to 1080p", step="1080p", dry_run=dry_run)
+
+    def as_stream_table(self) -> Table:
+        """Return the video probe as a rich table."""
+        probe = self._get_probe()
+        return probe.as_table()
+
+    def ffprobe_json(self) -> dict:
+        """Return the ffprobe json response."""
+        return self._get_probe().json_data
```

### Comparing `vid_cleaner-0.3.1/src/vid_cleaner/utils/helpers.py` & `vid_cleaner-0.3.2/src/vid_cleaner/utils/helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -179,23 +179,26 @@
 
 def _copyfileobj(
     src_bytes: io.BufferedReader,
     dest_bytes: io.BufferedWriter,
     callback: Callable,
     length: int,
 ) -> None:
-    """Copy from src_bytes to dest_bytes.
+    """Copy bytes from a source file to a destination file, with callback support.
 
-    Args:
-        src_bytes (io.BufferedReader): Source file
-        dest_bytes (io.BufferedWriter): Destination file
-        callback (Callable): Callback to call after every length bytes copied
-        total (int): Total number of bytes to copy
-        length (int): How many bytes to copy at once
+    This function reads bytes from a source file and writes them to a destination file in chunks,
+    calling a specified callback function after each chunk is written. It continues this process
+    until all bytes are copied or the end of the source file is reached.
 
+    Args:
+        src_bytes: The source file from which to read bytes. Must support the buffer protocol.
+        dest_bytes: The destination file to which bytes are written. Must support the buffer protocol.
+        callback: A callable that is invoked after each chunk of bytes is copied. The callable
+                  should accept a single argument, which is the total number of bytes copied so far.
+        length: The size of each chunk of bytes to be read and written at a time.
     """
     copied = 0
     while True:
         buf = src_bytes.read(length)
         if not buf:
             break
         dest_bytes.write(buf)
@@ -206,32 +209,41 @@
 
 def copy_with_callback(
     src: Path,
     dest: Path,
     callback: Callable | None = None,
     buffer_size: int = BUFFER_SIZE,
 ) -> Path:
-    """Copy file with a callback.
+    """Copy a file from a source to a destination, with optional progress callback.
+
+    This function copies a file from a specified source path to a destination path. During the
+    copy operation, it can optionally call a provided callback function after each chunk of data
+    is copied, allowing for progress tracking or other notifications. The size of the chunks copied
+    at each step can be customized.
 
     Args:
-        src (Path): Path to source file
-        dest (Path): Path to destination file
-        callback (Callable, optional): Callable callback that will be called after every buffer_size bytes copied. Defaults to None.
-        buffer_size (int, optional): How many bytes to copy at once (between calls to callback). Defaults to BUFFER_SIZE (4mb).
+        src: The path of the source file to copy.
+        dest: The path of the destination file or directory. If a directory is provided, the source
+              file will be copied into this directory with the same filename.
+        callback: An optional callable that is invoked after each chunk of data is copied. The callback
+                  receives one argument: the number of bytes copied so far. If not provided, no callback
+                  is called.
+        buffer_size: The size of each chunk of data to copy, in bytes. This determines how often the
+                     callback function is called, if provided.
 
     Returns:
-        Path: Path to destination file
-
+        The path to the copied destination file.
 
     Raises:
-        FileNotFoundError: If source file does not exist
-        SameFileError: If source and destination are the same file
-        ValueError: If callback is not callable
+        FileNotFoundError: If the source file does not exist.
+        SameFileError: If the source and destination paths refer to the same file.
+        ValueError: If the `callback` is provided but is not callable.
 
-    Note: Does not copy extended attributes, resource forks or other metadata.
+    Note:
+        This function does not copy file metadata such as extended attributes or resource forks.
     """
     if not src.is_file():
         msg = f"src file `{src}` doesn't exist"
         raise FileNotFoundError(msg)
 
     dest = dest / src.name if dest.is_dir() else dest
 
@@ -253,26 +265,29 @@
 
 def tmp_to_output(
     tmp_file: Path,
     stem: str,
     overwrite: bool = False,
     new_file: Path | None = None,
 ) -> Path:
-    """Copy a temporary file to an output file.
+    """Copy a temporary file to an output location with optional renaming and overwrite control.
 
-    If no output file is given, the name and directory of the source file will be used.  If overwrite is False, a number will be appended to the stem if the output file already exists.
+    This function copies a temporary file to a specified output location. If the output file path is not provided, the function uses the current working directory and the provided stem for the file name. If the target file exists and overwrite is False, the function will append a number to the stem to create a unique filename.
 
     Args:
-        tmp_file (Path): Path to input file
-        stem (str): Stem of output file
-        new_file (Path, optional): Path to output file. Defaults to None.
-        overwrite (bool, optional): Overwrite output file if it exists. Defaults to False.
+        tmp_file: The path to the temporary input file to be copied.
+        stem: The base name (stem) to use for the output file if `new_file` is not provided. If `new_file` is provided, `stem` is ignored.
+        overwrite: A flag to indicate whether to overwrite the output file if it already exists. If False and the file exists, a number is appended to the file's stem to avoid overwriting.
+        new_file: An optional path to the output file. If provided, this path is used as the target for the copy operation, and `stem` is ignored.
 
     Returns:
-        Path: Path to output file
+        The path to the output file where the temporary file has been copied.
+
+    Note:
+        This function uses a progress bar to indicate the copy progress and handles file naming conflicts by appending a number to the file stem if `overwrite` is False.
     """
     # When a path is given, use that
     if new_file:
         parent = new_file.parent.expanduser().resolve()
         stem = new_file.stem
     else:
         parent = Path.cwd()
```

### Comparing `vid_cleaner-0.3.1/src/vid_cleaner/utils/logging.py` & `vid_cleaner-0.3.2/src/vid_cleaner/utils/logging.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,31 @@
     DEBUG = 1
     TRACE = 2
     WARNING = 3
     ERROR = 4
 
 
 def log_formatter(record: dict) -> str:
-    """Use rich to style log messages."""
+    """Format log records for output with styling based on log level.
+
+    This function takes a log record dictionary and returns a formatted string using the Rich
+    library's syntax for text styling. It assigns different colors and icons to log messages
+    based on their severity level (e.g., DEBUG, INFO, ERROR). For DEBUG and TRACE levels, it
+    includes additional information like the logger name, function, and line number.
+
+    Args:
+        record: A dictionary containing log record information. Expected keys include 'level',
+                'message', 'name', 'function', and 'line'. The 'level' key should have a 'name'
+                attribute indicating the log level as a string.
+
+    Returns:
+        A formatted and styled string representing the log record, ready to be printed or
+        displayed. The string includes styling directives that are compatible with the Rich
+        library.
+    """
     color_map = {
         "TRACE": "turquoise2",
         "DEBUG": "cyan",
         "INFO": "bold",
         "SUCCESS": "bold green",
         "WARNING": "bold yellow",
         "ERROR": "bold red",
@@ -53,30 +69,30 @@
 
     return f"{msg} {debug}" if name in {"DEBUG", "TRACE"} else msg
 
 
 def instantiate_logger(
     verbosity: int, log_file: Path, log_to_file: bool
 ) -> None:  # pragma: no cover
-    """Instantiate the Loguru logger for brewup.
+    """Initialize and configure the logging system for the application.
 
-    Configure the logger with the specified verbosity level, log file path,
-    and whether to log to a file.
+    This function sets up the Loguru logger with a specified verbosity level and optionally
+    directs the log output to both the console and a file. It supports different verbosity
+    levels for controlling the amount of log information produced and can also capture logs
+    from installed libraries when verbosity is high enough.
 
     Args:
-        verbosity (int): The verbosity level of the logger. Valid values are:
-            - 0: Only log messages with severity level INFO and above will be displayed.
-            - 1: Only log messages with severity level DEBUG and above will be displayed.
-            - 2: Only log messages with severity level TRACE and above will be displayed.
-            > 2: Include debug from installed libraries
-        log_file (Path): The path to the log file where the log messages will be written.
-        log_to_file (bool): Whether to log the messages to the file specified by `log_file`.
-
-    Returns:
-        None
+        verbosity: Controls the amount of detail in the logs. Levels are as follows:
+            - 0 for INFO and above,
+            - 1 for DEBUG and above,
+            - 2 for TRACE and above,
+            - Greater than 2 includes DEBUG logs from installed libraries.
+        log_file: The file path where logs should be written if `log_to_file` is True.
+        log_to_file: A boolean indicating whether logs should also be saved to the file specified
+                     by `log_file`.
     """
     level = verbosity if verbosity < 3 else 2  # noqa: PLR2004
 
     logger.remove()
     logger.add(
         console.print,
         level=LogLevel(level).name,
```

### Comparing `vid_cleaner-0.3.1/src/vid_cleaner/vid_cleaner.py` & `vid_cleaner-0.3.2/src/vid_cleaner/vid_cleaner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 """vid-cleaner CLI."""
 
-import re
 import shutil
 from pathlib import Path
 from typing import Annotated, Optional
 
 import typer
 from confz import validate_all_configs
 from loguru import logger
 from pydantic import ValidationError
-from rich.table import Table
 
-from vid_cleaner.config import VidCleanerConfig
-from vid_cleaner.constants import CONFIG_PATH, VERSION
+from vid_cleaner.cli import clean, clip, inspect
+from vid_cleaner.constants import CONFIG_PATH, VERSION, VideoContainerTypes
 from vid_cleaner.models import VideoFile
 from vid_cleaner.utils import (
     console,
     existing_file_path,
-    ffprobe,
     instantiate_logger,
-    tmp_to_output,
 )
 
 typer.rich_utils.STYLE_HELPTEXT = ""
 
 app = typer.Typer(
     add_completion=False,
     no_args_is_help=True,
@@ -49,16 +45,16 @@
         console.print(f"{__package__}: v{VERSION}")
         raise typer.Exit()
 
 
 def parse_video_input(path: str) -> VideoFile:
     """Takes a string of a path and converts it to a VideoFile object."""
     file_path = existing_file_path(path)
-    if file_path.suffix not in {".mkv", ".mp4", ".avi", "vp9", ".webm", ".mov", ".wmv"}:
-        msg = f"File type '{file_path.suffix}' is not supported"
+    if file_path.suffix not in VideoContainerTypes.__members__.values():
+        msg = f"Vidcleaner supports {', '.join(VideoContainerTypes.__members__.values())} files.  '{file_path.suffix}' is not supported."
         raise typer.BadParameter(msg)
 
     return VideoFile(file_path)
 
 
 @app.command("inspect")
 def inspect_command(
@@ -79,54 +75,15 @@
     """Inspect video files to display detailed stream information.
 
     Use this command to view detailed information about the video and audio streams
     of a video file. The information includes stream type, codec, language,
     and audio channel details. This command is useful for understanding the
     composition of a video file before performing operations like clipping or transcoding.
     """
-    for video in files:
-        probe = ffprobe(video.path)
-
-        if json:
-            console.print(probe)
-            return
-
-        if "title" in probe["format"]["tags"]:
-            name = probe["format"]["tags"]["title"]
-        elif "filename" in probe["format"]:
-            name = probe["format"]["filename"]
-        else:
-            name = video.stem
-
-        table = Table(title=name)
-        table.add_column("#")
-        table.add_column("Stream")
-        table.add_column("Type")
-        table.add_column("Language")
-        table.add_column("Channels")
-        table.add_column("Channel Layout")
-        table.add_column("Title")
-
-        for i, stream in enumerate(probe["streams"]):
-            language = stream["tags"].get("language", "-")
-            channels = stream.get("channels", "-")
-            layout = stream.get("channel_layout", "-")
-            title = stream["tags"].get("title", "-")
-
-            table.add_row(
-                str(i),
-                stream["codec_type"],
-                stream.get("codec_name", "-"),
-                language,
-                str(channels),
-                layout,
-                title,
-            )
-
-        console.print(table)
+    inspect(files, json_output=json)
 
 
 @app.command("clip")
 def clip_command(
     files: Annotated[
         list[VideoFile],
         typer.Argument(
@@ -162,35 +119,15 @@
     This command allows you to extract a specific portion of a video file based on start time and duration.
 
     * The start time and duration should be specified in [code]HH:MM:SS[/code] format.
     * You can also specify an output file to save the clipped video. If the output file is not specified, the clip will be saved with a default naming convention.
 
     Use the [code]--overwrite[/code] option to overwrite the output file if it already exists.
     """
-    time_pattern = re.compile(r"^\d{2}:\d{2}:\d{2}$")
-
-    if not time_pattern.match(start):
-        msg = "Start must be in format HH:MM:SS"  # type: ignore [unreachable]
-        raise typer.BadParameter(msg)
-
-    if not time_pattern.match(duration):
-        msg = "Duration must be in format HH:MM:SS"  # type: ignore [unreachable]
-        raise typer.BadParameter(msg)
-
-    for video in files:
-        logger.info(f"⇨ {video.path.name}")
-
-        video.clip(start, duration, dry_run=dry_run)
-
-        if not dry_run:
-            out_file = tmp_to_output(
-                video.current_tmp_file, stem=video.stem, new_file=out, overwrite=overwrite
-            )
-            video.cleanup()
-            logger.success(f"{out_file}")
+    clip(files, start, duration, out, overwrite, dry_run)
 
 
 @docstring_parameter(CONFIG_PATH)
 @app.command("clean")
 def clean_command(
     ctx: typer.Context,
     files: Annotated[
@@ -227,15 +164,17 @@
         typer.Option(
             "--downmix", help="Create a stereo track if none exist", rich_help_panel="Audio"
         ),
     ] = False,
     drop_original_audio: Annotated[
         bool,
         typer.Option(
-            "--drop-original", help="Drop original language audio", rich_help_panel="Audio"
+            "--drop-original",
+            help="Drop original language audio if not in config",
+            rich_help_panel="Audio",
         ),
     ] = False,
     keep_all_subtitles: Annotated[
         bool, typer.Option("--keep-subs", help="Keep all subtitles", rich_help_panel="Subtitles")
     ] = False,
     keep_commentary: Annotated[
         bool,
@@ -304,59 +243,32 @@
 
     [#999999]Transcode a video to H265 format and keep English audio:[/#999999]
     vidcleaner clean --h265 --langs=eng <video_file>
 
     [#999999]Downmix audio to stereo and keep all subtitles:[/#999999]
     vidcleaner clean --downmix --keep-subs <video_file>
     """
-    verbosity = ctx.meta["verbosity"]
-
-    languages = langs or ",".join(VidCleanerConfig().keep_languages)
-
-    for video in files:
-        logger.info(f"⇨ {video.path.name}")
-
-        if h265 and vp9:
-            msg = "Cannot convert to both H265 and VP9"
-            raise typer.BadParameter(msg)
-
-        video.reorder_streams(dry_run=dry_run)
-
-        video.process_streams(
-            langs_to_keep=languages.split(","),
-            drop_original_audio=drop_original_audio,
-            keep_commentary=keep_commentary,
-            downmix_stereo=downmix_stereo,
-            keep_all_subtitles=keep_all_subtitles,
-            keep_local_subtitles=keep_local_subtitles,
-            subs_drop_local=subs_drop_local,
-            dry_run=dry_run,
-            verbosity=verbosity,
-        )
-
-        if video_1080:
-            video.video_to_1080p(force=force, dry_run=dry_run)
-
-        if h265:
-            video._convert_to_h265(force=force, dry_run=dry_run)
-
-        if vp9:
-            video._convert_to_vp9(force=force, dry_run=dry_run)
-
-        if not dry_run:
-            out_file = tmp_to_output(
-                video.current_tmp_file, stem=video.stem, new_file=out, overwrite=replace
-            )
-            video.cleanup()
-
-            if replace and out_file != video.path:
-                logger.debug(f"Delete: {video.path}")
-                video.path.unlink()
-
-            logger.success(f"{out_file}")
+    clean(
+        files=files,
+        out=out,
+        replace=replace,
+        downmix_stereo=downmix_stereo,
+        drop_original_audio=drop_original_audio,
+        keep_all_subtitles=keep_all_subtitles,
+        keep_commentary=keep_commentary,
+        keep_local_subtitles=keep_local_subtitles,
+        subs_drop_local=subs_drop_local,
+        langs=langs,
+        h265=h265,
+        vp9=vp9,
+        video_1080=video_1080,
+        force=force,
+        dry_run=dry_run,
+        verbosity=ctx.meta["verbosity"],
+    )
 
 
 @docstring_parameter(CONFIG_PATH)
 @app.callback()
 def main(
     ctx: typer.Context,
     log_file: Annotated[
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `vid_cleaner-0.3.1/PKG-INFO` & `vid_cleaner-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vid-cleaner
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tools to transcode, inspect and convert videos.
 Home-page: https://github.com/natelandau/vid-cleaner
 Author: Nate Landau
 Author-email: github@natenate.org
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -12,15 +12,16 @@
 Requires-Dist: confz (>=2.0.1,<3.0.0)
 Requires-Dist: ffmpeg-progress-yield (>=0.7.8,<0.8.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: iso639-lang (>=2.2.3,<3.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: shellingham (>=1.5.4,<2.0.0)
+Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Repository, https://github.com/natelandau/vid-cleaner
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/vid-cleaner.svg)](https://badge.fury.io/py/vid-cleaner) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vid-cleaner) [![Python Code Checker](https://github.com/natelandau/vid-cleaner/actions/workflows/automated-tests.yml/badge.svg)](https://github.com/natelandau/vid-cleaner/actions/workflows/automated-tests.yml) [![codecov](https://codecov.io/gh/natelandau/vid-cleaner/graph/badge.svg?token=NHBKL0B6CL)](https://codecov.io/gh/natelandau/vid-cleaner)
 
 # Vid Cleaner
```

