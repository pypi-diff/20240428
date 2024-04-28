# Comparing `tmp/isubrip-2.5.3.tar.gz` & `tmp/isubrip-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isubrip-2.5.3.tar", max compression
+gzip compressed data, was "isubrip-2.5.4.tar", max compression
```

## Comparing `isubrip-2.5.3.tar` & `isubrip-2.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2024-03-16 16:42:50.118731 isubrip-2.5.3/isubrip/__init__.py
--rw-r--r--   0        0        0    22220 2024-04-09 20:06:17.681572 isubrip-2.5.3/isubrip/__main__.py
--rw-r--r--   0        0        0    14124 2024-04-09 20:06:17.681572 isubrip-2.5.3/isubrip/config.py
--rw-r--r--   0        0        0     1858 2024-04-09 20:06:17.683080 isubrip-2.5.3/isubrip/constants.py
--rw-r--r--   0        0        0     8355 2024-04-09 20:06:17.683080 isubrip-2.5.3/isubrip/data_structures.py
--rw-r--r--   0        0        0     1640 2024-03-16 16:42:50.121730 isubrip-2.5.3/isubrip/logger.py
--rw-r--r--   0        0        0      574 2024-04-09 20:06:17.684089 isubrip-2.5.3/isubrip/resources/default_config.toml
--rw-r--r--   0        0        0        0 2023-05-26 10:40:55.098754 isubrip-2.5.3/isubrip/scrapers/__init__.py
--rw-r--r--   0        0        0    16052 2024-04-09 20:06:17.685090 isubrip-2.5.3/isubrip/scrapers/appletv_scraper.py
--rw-r--r--   0        0        0     6514 2024-04-09 20:06:17.685090 isubrip-2.5.3/isubrip/scrapers/itunes_scraper.py
--rw-r--r--   0        0        0    25550 2024-04-09 20:06:17.686091 isubrip-2.5.3/isubrip/scrapers/scraper.py
--rw-r--r--   0        0        0        0 2023-05-24 22:34:46.568839 isubrip-2.5.3/isubrip/subtitle_formats/__init__.py
--rw-r--r--   0        0        0     1406 2024-04-09 20:06:17.687091 isubrip-2.5.3/isubrip/subtitle_formats/subrip.py
--rw-r--r--   0        0        0    10934 2024-04-09 20:06:17.687091 isubrip-2.5.3/isubrip/subtitle_formats/subtitles.py
--rw-r--r--   0        0        0    10564 2024-04-09 20:06:17.688088 isubrip-2.5.3/isubrip/subtitle_formats/webvtt.py
--rw-r--r--   0        0        0    19715 2024-04-09 20:06:17.688088 isubrip-2.5.3/isubrip/utils.py
--rw-r--r--   0        0        0     1093 2022-01-28 09:13:22.249000 isubrip-2.5.3/LICENSE
--rw-r--r--   0        0        0     2999 2024-04-09 20:06:17.690088 isubrip-2.5.3/pyproject.toml
--rw-r--r--   0        0        0     2899 2024-04-09 20:06:17.680573 isubrip-2.5.3/README.md
--rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 isubrip-2.5.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-16 16:42:50.118731 isubrip-2.5.4/isubrip/__init__.py
+-rw-r--r--   0        0        0    22512 2024-04-28 16:29:01.833966 isubrip-2.5.4/isubrip/__main__.py
+-rw-r--r--   0        0        0    14124 2024-04-12 19:49:58.044518 isubrip-2.5.4/isubrip/config.py
+-rw-r--r--   0        0        0     1858 2024-04-28 16:29:01.833966 isubrip-2.5.4/isubrip/constants.py
+-rw-r--r--   0        0        0     8465 2024-04-28 16:29:01.834967 isubrip-2.5.4/isubrip/data_structures.py
+-rw-r--r--   0        0        0     1640 2024-03-16 16:42:50.121730 isubrip-2.5.4/isubrip/logger.py
+-rw-r--r--   0        0        0      574 2024-04-09 20:06:17.684089 isubrip-2.5.4/isubrip/resources/default_config.toml
+-rw-r--r--   0        0        0        0 2023-05-26 10:40:55.098754 isubrip-2.5.4/isubrip/scrapers/__init__.py
+-rw-r--r--   0        0        0    16052 2024-04-26 09:07:32.013359 isubrip-2.5.4/isubrip/scrapers/appletv_scraper.py
+-rw-r--r--   0        0        0     6774 2024-04-28 16:29:01.834967 isubrip-2.5.4/isubrip/scrapers/itunes_scraper.py
+-rw-r--r--   0        0        0    26590 2024-04-28 16:29:01.835965 isubrip-2.5.4/isubrip/scrapers/scraper.py
+-rw-r--r--   0        0        0        0 2023-05-24 22:34:46.568839 isubrip-2.5.4/isubrip/subtitle_formats/__init__.py
+-rw-r--r--   0        0        0     1406 2024-04-12 19:49:58.050030 isubrip-2.5.4/isubrip/subtitle_formats/subrip.py
+-rw-r--r--   0        0        0    10934 2024-04-12 19:49:58.050030 isubrip-2.5.4/isubrip/subtitle_formats/subtitles.py
+-rw-r--r--   0        0        0    10564 2024-04-09 20:06:17.688088 isubrip-2.5.4/isubrip/subtitle_formats/webvtt.py
+-rw-r--r--   0        0        0    19715 2024-04-28 09:49:22.678095 isubrip-2.5.4/isubrip/utils.py
+-rw-r--r--   0        0        0     1093 2022-01-28 09:13:22.249000 isubrip-2.5.4/LICENSE
+-rw-r--r--   0        0        0     3000 2024-04-28 16:29:01.836966 isubrip-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2899 2024-04-28 16:29:01.832966 isubrip-2.5.4/README.md
+-rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 isubrip-2.5.4/PKG-INFO
```

### Comparing `isubrip-2.5.3/isubrip/__main__.py` & `isubrip-2.5.4/isubrip/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ScrapedMediaResponse,
     Season,
     Series,
     SubtitlesData,
     SubtitlesDownloadResults,
 )
 from isubrip.logger import CustomLogFileFormatter, CustomStdoutFormatter, logger
-from isubrip.scrapers.scraper import PlaylistLoadError, Scraper, ScraperError, ScraperFactory
+from isubrip.scrapers.scraper import PlaylistLoadError, Scraper, ScraperError, ScraperFactory, SubtitlesDownloadError
 from isubrip.subtitle_formats.webvtt import Caption as WebVTTCaption
 from isubrip.utils import (
     TempDirGenerator,
     download_subtitles_to_file,
     format_media_description,
     format_release_name,
     format_subtitles_description,
@@ -146,21 +146,22 @@
 def main() -> None:
     try:
         # Assure at least one argument was passed
         if len(sys.argv) < 2:
             print_usage()
             exit(0)
 
+        if not DATA_FOLDER_PATH.is_dir():
+            DATA_FOLDER_PATH.mkdir(parents=True)
+
         setup_loggers(stdout_loglevel=logging.INFO,
                       file_loglevel=logging.DEBUG)
 
-        generate_project_folders()
-
         cli_args = " ".join(sys.argv[1:])
-        logger.debug(f"Used CLI Command: {PACKAGE_NAME} {cli_args}")
+        logger.debug(f"CLI Command: {PACKAGE_NAME} {cli_args}")
         logger.debug(f"Python version: {sys.version}")
         logger.debug(f"Package version: {PACKAGE_VERSION}")
         logger.debug(f"OS: {sys.platform}")
 
         config = generate_config()
         update_settings(config)
 
@@ -168,15 +169,15 @@
             check_for_updates(current_package_version=PACKAGE_VERSION)
 
         urls = single_to_list(sys.argv[1:])
         download(urls=urls, config=config)
 
     except Exception as ex:
         logger.error(f"Error: {ex}")
-        logger.debug(f"Stack trace: {ex}", exc_info=True)
+        logger.debug("Debug information:", exc_info=True)
         exit(1)
 
     finally:
         if log_rotation_size := LOG_ROTATION_SIZE:
             handle_log_rotation(log_rotation_size=log_rotation_size)
 
         # NOTE: This will only close scrapers that were initialized using the ScraperFactory.
@@ -280,20 +281,17 @@
             results = download_subtitles(scraper=scraper,
                                          media_data=media_item,
                                          **download_subtitles_kwargs)
 
             success_count = len(results.successful_subtitles)
             failed_count = len(results.failed_subtitles)
 
-            if success_count:
+            if success_count or failed_count:
                 logger.info(f"{success_count}/{success_count + failed_count} matching subtitles "
-                            f"have been successfully downloaded.")
-
-            elif failed_count:
-                logger.info(f"{failed_count} subtitles were matched, but failed to download.")
+                            f"were successfully downloaded.")
 
             else:
                 logger.info("No matching subtitles were found.")
 
             return  # noqa: TRY300
 
         except PlaylistLoadError:
@@ -335,29 +333,18 @@
                            f'\nConsider upgrading by running "python3 -m pip install --upgrade {PACKAGE_NAME}"\n')
 
         else:
             logger.debug(f"Latest version of '{PACKAGE_NAME}' ({current_package_version}) is currently installed.")
 
     except Exception as e:
         logger.warning(f"Update check failed: {e}")
-        logger.debug(f"Stack trace: {e}", exc_info=True)
+        logger.debug("Debug information:", exc_info=True)
         return
 
 
-def generate_project_folders() -> None:
-    if not DATA_FOLDER_PATH.is_dir():
-        logger.debug(f"'{DATA_FOLDER_PATH}' directory could not be found and will be created.")
-        LOG_FILES_PATH.mkdir(parents=True, exist_ok=True)
-
-    else:  # LOG_FILES_PATH is inside DATA_FOLDER_PATH
-        if not LOG_FILES_PATH.is_dir():
-            logger.debug(f"'{LOG_FILES_PATH}' directory could not be found and will be created.")
-            LOG_FILES_PATH.mkdir()
-
-
 def download_subtitles(scraper: Scraper, media_data: Movie | Episode, download_path: Path,
                        language_filter: list[str] | None = None, convert_to_srt: bool = False,
                        overwrite_existing: bool = True, zip_files: bool = False) -> SubtitlesDownloadResults:
     """
     Download subtitles for the given media data.
 
     Args:
@@ -374,42 +361,53 @@
     Returns:
         SubtitlesDownloadResults: A SubtitlesDownloadResults object containing the results of the download.
     """
     temp_dir_name = generate_media_folder_name(media_data=media_data, source=scraper.abbreviation)
     temp_download_path = TempDirGenerator.generate(directory_name=temp_dir_name)
 
     successful_downloads: list[SubtitlesData] = []
-    failed_downloads: list[SubtitlesData] = []
+    failed_downloads: list[SubtitlesDownloadError] = []
     temp_downloads: list[Path] = []
 
     for subtitles_data in scraper.get_subtitles(main_playlist=media_data.playlist,  # type: ignore[arg-type]
                                                 language_filter=language_filter,
                                                 subrip_conversion=convert_to_srt):
-
         language_info = format_subtitles_description(language_code=subtitles_data.language_code,
                                                      language_name=subtitles_data.language_name,
                                                      special_type=subtitles_data.special_type)
 
+        if isinstance(subtitles_data, SubtitlesDownloadError):
+            logger.warning(f"Failed to download '{language_info}' subtitles. Skipping...")
+            logger.debug("Debug information:", exc_info=subtitles_data.original_exc)
+            failed_downloads.append(subtitles_data)
+            continue
+
         try:
             temp_downloads.append(download_subtitles_to_file(
                 media_data=media_data,
                 subtitles_data=subtitles_data,
                 output_path=temp_download_path,
                 source_abbreviation=scraper.abbreviation,
                 overwrite=overwrite_existing,
             ))
 
-            logger.info(f"{language_info} subtitles were successfully downloaded.")
+            logger.info(f"'{language_info}' subtitles were successfully downloaded.")
             successful_downloads.append(subtitles_data)
 
         except Exception as e:
-            logger.error(f"Error: Failed to download '{language_info}' subtitles: {e}")
-            logger.debug("Stack trace:", exc_info=True)
-            failed_downloads.append(subtitles_data)
-            continue
+            logger.error(f"Error: Failed to save '{language_info}' subtitles: {e}")
+            logger.debug("Debug information:", exc_info=True)
+            failed_downloads.append(
+                SubtitlesDownloadError(
+                    language_code=subtitles_data.language_code,
+                    language_name=subtitles_data.language_name,
+                    special_type=subtitles_data.special_type,
+                    original_exc=e,
+                ),
+            )
 
     if not zip_files or len(temp_downloads) == 1:
         for file_path in temp_downloads:
             if overwrite_existing:
                 new_path = download_path / file_path.name
 
             else:
@@ -592,16 +590,21 @@
     # Setup STDOUT logger
     stdout_handler = logging.StreamHandler(sys.stdout)
     stdout_handler.setLevel(stdout_loglevel)
     stdout_handler.setFormatter(CustomStdoutFormatter())
     logger.addHandler(stdout_handler)
 
     # Setup logfile logger
+    if not LOG_FILES_PATH.is_dir():
+        logger.debug("Logs directory could not be found and will be created.")
+        LOG_FILES_PATH.mkdir()
+
     logfile_path = generate_non_conflicting_path(file_path=LOG_FILES_PATH / LOG_FILE_NAME)
     logfile_handler = logging.FileHandler(filename=logfile_path, encoding="utf-8")
     logfile_handler.setLevel(file_loglevel)
     logfile_handler.setFormatter(CustomLogFileFormatter())
+    logger.debug(f"Log file location: '{logfile_path}'")
     logger.addHandler(logfile_handler)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `isubrip-2.5.3/isubrip/config.py` & `isubrip-2.5.4/isubrip/config.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.5.3/isubrip/constants.py` & `isubrip-2.5.4/isubrip/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime as dt
 import logging
 from pathlib import Path
 from tempfile import gettempdir
 
 # General
 PACKAGE_NAME = "isubrip"
-PACKAGE_VERSION = "2.5.3"
+PACKAGE_VERSION = "2.5.4"
 
 # Logging
 PREORDER_MESSAGE = ("'{movie_name}' is currently unavailable on {scraper_name}, "
                     "and will be available on {preorder_date}.")
 
 ANSI_COLORS = {
     logging.DEBUG: "\x1b[37;20m",  # Light Grey
```

### Comparing `isubrip-2.5.3/isubrip/data_structures.py` & `isubrip-2.5.4/isubrip/data_structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 from abc import ABC
 import datetime as dt  # noqa: TCH003
 from enum import Enum
-from typing import Generic, List, NamedTuple, Optional, TypeVar, Union
+from typing import TYPE_CHECKING, Generic, List, NamedTuple, Optional, TypeVar, Union
 
 from pydantic import BaseModel
 
+if TYPE_CHECKING:
+    from isubrip.scrapers.scraper import SubtitlesDownloadError
+
 MediaData = TypeVar("MediaData", bound="MediaBase")
 
 
 class SubtitlesDownloadResults(NamedTuple):
     """
     A named tuple containing download results.
 
@@ -18,15 +21,15 @@
         media_data (Movie | Episode): An object containing metadata about the media the subtitles were downloaded for.
         successful_subtitles (list[SubtitlesData]): List of subtitles that were successfully downloaded.
         failed_subtitles (list[SubtitlesData]): List of subtitles that failed to download.
         is_zip (bool): Whether the subtitles were saved in a zip file.
     """
     media_data: Movie | Episode
     successful_subtitles: list[SubtitlesData]
-    failed_subtitles: list[SubtitlesData]
+    failed_subtitles: list[SubtitlesDownloadError]
     is_zip: bool
 
 
 class SubtitlesFormat(BaseModel):
     """
     An object containing subtitles format data.
```

### Comparing `isubrip-2.5.3/isubrip/logger.py` & `isubrip-2.5.4/isubrip/logger.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.5.3/isubrip/resources/default_config.toml` & `isubrip-2.5.4/isubrip/resources/default_config.toml`

 * *Files identical despite different names*

### Comparing `isubrip-2.5.3/isubrip/scrapers/appletv_scraper.py` & `isubrip-2.5.4/isubrip/scrapers/appletv_scraper.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.5.3/isubrip/scrapers/itunes_scraper.py` & `isubrip-2.5.4/isubrip/scrapers/itunes_scraper.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING, Iterator
 
 import m3u8
 from requests.exceptions import HTTPError
 
 from isubrip.data_structures import SubtitlesData, SubtitlesFormatType
 from isubrip.logger import logger
-from isubrip.scrapers.scraper import HLSScraper, PlaylistLoadError, ScraperError, ScraperFactory
+from isubrip.scrapers.scraper import HLSScraper, PlaylistLoadError, ScraperError, ScraperFactory, SubtitlesDownloadError
 from isubrip.subtitle_formats.webvtt import WebVTTSubtitles
 from isubrip.utils import merge_dict_values, raise_for_status
 
 if TYPE_CHECKING:
     from isubrip.data_structures import Movie, ScrapedMediaResponse
 
 
@@ -84,15 +84,15 @@
         if not self._appletv_scraper.match_url(redirect_location):
             logger.debug(f"iTunes URL: {url} redirected to an invalid Apple TV URL: '{redirect_location}'.")
             raise ScraperError("Redirect URL is not a valid Apple TV URL.")
 
         return self._appletv_scraper.get_data(redirect_location)
 
     def get_subtitles(self, main_playlist: str | list[str], language_filter: list[str] | str | None = None,
-                      subrip_conversion: bool = False) -> Iterator[SubtitlesData]:
+                      subrip_conversion: bool = False) -> Iterator[SubtitlesData | SubtitlesDownloadError]:
         language_filters = {self.M3U8Attribute.LANGUAGE.value: language_filter} if language_filter else None
         main_playlist_m3u8 = self.load_m3u8(url=main_playlist)
 
         if main_playlist_m3u8 is None:
             raise PlaylistLoadError("Could not load M3U8 playlist.")
 
         playlist_filters = (merge_dict_values(self._subtitles_filters, language_filters)
@@ -101,15 +101,15 @@
 
         matched_media_items = self.get_media_playlists(main_playlist=main_playlist_m3u8,
                                                        playlist_filters=playlist_filters)
 
         for matched_media in matched_media_items:
             language_name = matched_media.name.replace(' (forced)', '').strip()
             language_code = matched_media.language
-            language_info_str = f"{language_name} ({language_code})"
+            special_type = self.detect_subtitles_type(subtitles_media=matched_media)
 
             try:
                 m3u8_data = self._session.get(url=matched_media.absolute_uri)
                 matched_media_playlist = m3u8.loads(content=m3u8_data.text, uri=matched_media.absolute_uri)
 
                 subtitles_segments = self._download_segments(matched_media_playlist.segments)
                 subtitles = self.subtitles_class(data=subtitles_segments[0], language_code=language_code)
@@ -122,21 +122,31 @@
                 subtitles.polish(
                     fix_rtl=self.subtitles_fix_rtl,
                     remove_duplicates=self.subtitles_remove_duplicates,
                 )
 
                 language_name = matched_media.name.replace(' (forced)', '').strip()
 
+                if subrip_conversion:
+                    subtitles_format = SubtitlesFormatType.SUBRIP
+                    content = subtitles.to_srt().dump()
+
+                else:
+                    subtitles_format = SubtitlesFormatType.WEBVTT
+                    content = subtitles.dump()
+
                 yield SubtitlesData(
                     language_code=language_code,
                     language_name=language_name,
-                    subtitles_format=SubtitlesFormatType.SUBRIP if subrip_conversion else SubtitlesFormatType.WEBVTT,
-                    content=subtitles.to_srt().dump() if subrip_conversion else subtitles.dump(),
+                    subtitles_format=subtitles_format,
+                    content=content,
                     content_encoding=subtitles.encoding,
-                    special_type=self.detect_subtitles_type(matched_media),
+                    special_type=special_type,
                 )
 
             except Exception as e:
-                logger.warning(f"Failed to download {language_info_str} subtitles. "
-                               f"Skipping...")
-                logger.debug(e, exc_info=True)
-                continue
+                yield SubtitlesDownloadError(
+                    language_code=language_code,
+                    language_name=language_name,
+                    special_type=special_type,
+                    original_exc=e,
+                )
```

### Comparing `isubrip-2.5.3/isubrip/scrapers/scraper.py` & `isubrip-2.5.4/isubrip/scrapers/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,27 +220,27 @@
 
         Returns:
             ScrapedMediaResponse: A ScrapedMediaResponse object containing scraped media information.
         """
 
     @abstractmethod
     def get_subtitles(self, main_playlist: str | list[str], language_filter: list[str] | None = None,
-                      subrip_conversion: bool = False) -> Iterator[SubtitlesData]:
+                      subrip_conversion: bool = False) -> Iterator[SubtitlesData | SubtitlesDownloadError]:
         """
         Find and yield subtitles data from a main_playlist.
 
         Args:
             main_playlist(str | list[str]): A URL or a list of URLs (for redundancy) of the main playlist.
             language_filter (list[str] | str | None, optional):
                 A language or a list of languages to filter for. Defaults to None.
             subrip_conversion (bool, optional): Whether to convert the subtitles to SubRip format. Defaults to False.
 
         Yields:
-            SubtitlesData: A SubtitlesData object for each subtitle found
-                in the main playlist (matching the filters, if given).
+            SubtitlesData | SubtitlesDownloadError: A SubtitlesData object containing subtitles data,
+                or a SubtitlesDownloadError object if an error occurred.
         """
 
 
 class AsyncScraper(Scraper, ABC):
     """A base class for scrapers that utilize async requests."""
     def __init__(self,  user_agent: str | None = None, config_data: dict | None = None):
         super().__init__(user_agent=user_agent, config_data=config_data)
@@ -612,7 +612,26 @@
 
 class ScraperError(Exception):
     pass
 
 
 class PlaylistLoadError(ScraperError):
     pass
+
+
+class SubtitlesDownloadError(ScraperError):
+    def __init__(self, language_code: str, language_name: str | None = None, special_type: SubtitlesType | None = None,
+                 original_exc: Exception | None = None, *args: Any, **kwargs: dict[str, Any]):
+        """
+        Initialize a SubtitlesDownloadError instance.
+
+        Args:
+            language_code (str): Language code of the subtitles that failed to download.
+            language_name (str | None, optional): Language name of the subtitles that failed to download.
+            special_type (SubtitlesType | None, optional): Type of the subtitles that failed to download.
+            original_exc (Exception | None, optional): The original exception that caused the error.
+        """
+        super().__init__(*args, **kwargs)
+        self.language_code = language_code
+        self.language_name = language_name
+        self.special_type = special_type
+        self.original_exc = original_exc
```

### Comparing `isubrip-2.5.3/isubrip/subtitle_formats/subrip.py` & `isubrip-2.5.4/isubrip/subtitle_formats/subrip.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.5.3/isubrip/subtitle_formats/subtitles.py` & `isubrip-2.5.4/isubrip/subtitle_formats/subtitles.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.5.3/isubrip/subtitle_formats/webvtt.py` & `isubrip-2.5.4/isubrip/subtitle_formats/webvtt.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.5.3/isubrip/utils.py` & `isubrip-2.5.4/isubrip/utils.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.5.3/LICENSE` & `isubrip-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `isubrip-2.5.3/pyproject.toml` & `isubrip-2.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "isubrip"
-version = "2.5.3"
+version = "2.5.4"
 description = "A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages."
 license = "MIT"
 authors = ["Michael Yochpaz"]
 readme = "README.md"
 homepage = "https://github.com/MichaelYochpaz/iSubRip"
 repository = "https://github.com/MichaelYochpaz/iSubRip"
 keywords = [
@@ -54,21 +54,21 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
 httpx = {extras = ["http2"], version = "^0.27.0"}
 m3u8 = "^4.1.0"
 mergedeep = "^1.3.4"
-pydantic = "^2.6.4"
+pydantic = "^2.7.0"
 tomli = "^2.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^1.9.0"
-ruff = "^0.3.5"
+mypy = "^1.10.0"
+ruff = "^0.4.2"
 types-requests = "^2.31.0.20240406"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry_bumpversion.file."isubrip/constants.py"]
```

### Comparing `isubrip-2.5.3/README.md` & `isubrip-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.5.3 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.5.4 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # iSubRip A Python package for scraping and downloading subtitles from AppleTV
-/ iTunes movie pages. Latest version: 2.5.3 ([changelog](https://github.com/
+/ iTunes movie pages. Latest version: 2.5.4 ([changelog](https://github.com/
 MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
 pypi/isubrip) [![GitHub - License](https://img.shields.io/github/license/
```

### Comparing `isubrip-2.5.3/PKG-INFO` & `isubrip-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isubrip
-Version: 2.5.3
+Version: 2.5.4
 Summary: A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.
 Home-page: https://github.com/MichaelYochpaz/iSubRip
 License: MIT
 Keywords: iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8
 Author: Michael Yochpaz
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,24 +20,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
 Requires-Dist: m3u8 (>=4.1.0,<5.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
-Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Repository, https://github.com/MichaelYochpaz/iSubRip
 Description-Content-Type: text/markdown
 
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.5.3 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.5.4 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: isubrip Version: 2.5.3 Summary: A Python package
+Metadata-Version: 2.1 Name: isubrip Version: 2.5.4 Summary: A Python package
 for scraping and downloading subtitles from AppleTV / iTunes movie pages. Home-
 page: https://github.com/MichaelYochpaz/iSubRip License: MIT Keywords:
 iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8 Author: Michael
 Yochpaz Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: End Users/Desktop Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: MacOS Classifier: Operating System
 :: Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
 Requires-Dist: m3u8 (>=4.1.0,<5.0.0) Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
-Requires-Dist: pydantic (>=2.6.4,<3.0.0) Requires-Dist: requests
+Requires-Dist: pydantic (>=2.7.0,<3.0.0) Requires-Dist: requests
 (>=2.31.0,<3.0.0) Requires-Dist: tomli (>=2.0.1,<3.0.0) Project-URL: Bug
 Reports, https://github.com/MichaelYochpaz/iSubRip/issues Project-URL:
 Repository, https://github.com/MichaelYochpaz/iSubRip Description-Content-Type:
 text/markdown # iSubRip A Python package for scraping and downloading subtitles
-from AppleTV / iTunes movie pages. Latest version: 2.5.3 ([changelog](https://
+from AppleTV / iTunes movie pages. Latest version: 2.5.4 ([changelog](https://
 github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
 pypi/isubrip) [![GitHub - License](https://img.shields.io/github/license/
```

