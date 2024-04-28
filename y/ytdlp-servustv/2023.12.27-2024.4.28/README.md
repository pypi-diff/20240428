# Comparing `tmp/ytdlp_servustv-2023.12.27-py3-none-any.whl.zip` & `tmp/ytdlp_servustv-2024.4.28-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 10289 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    28336 b- defN 23-Dec-27 16:34 yt_dlp_plugins/extractor/servustv.py
--rw-rw-rw-  2.0 fat     1212 b- defN 23-Dec-27 16:35 ytdlp_servustv-2023.12.27.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3484 b- defN 23-Dec-27 16:35 ytdlp_servustv-2023.12.27.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Dec-27 16:35 ytdlp_servustv-2023.12.27.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 23-Dec-27 16:35 ytdlp_servustv-2023.12.27.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      540 b- defN 23-Dec-27 16:35 ytdlp_servustv-2023.12.27.dist-info/RECORD
-6 files, 33689 bytes uncompressed, 9301 bytes compressed:  72.4%
+Zip file size: 9357 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    22918 b- defN 24-Apr-28 07:48 yt_dlp_plugins/extractor/servustv.py
+-rw-rw-rw-  2.0 fat     1236 b- defN 24-Apr-28 07:49 ytdlp_servustv-2024.4.28.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3439 b- defN 24-Apr-28 07:49 ytdlp_servustv-2024.4.28.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 07:49 ytdlp_servustv-2024.4.28.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       25 b- defN 24-Apr-28 07:49 ytdlp_servustv-2024.4.28.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      535 b- defN 24-Apr-28 07:49 ytdlp_servustv-2024.4.28.dist-info/RECORD
+6 files, 28245 bytes uncompressed, 8379 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: yt_dlp_plugins/extractor/servustv.py
 Comment: 
 
-Filename: ytdlp_servustv-2023.12.27.dist-info/LICENSE
+Filename: ytdlp_servustv-2024.4.28.dist-info/LICENSE
 Comment: 
 
-Filename: ytdlp_servustv-2023.12.27.dist-info/METADATA
+Filename: ytdlp_servustv-2024.4.28.dist-info/METADATA
 Comment: 
 
-Filename: ytdlp_servustv-2023.12.27.dist-info/WHEEL
+Filename: ytdlp_servustv-2024.4.28.dist-info/WHEEL
 Comment: 
 
-Filename: ytdlp_servustv-2023.12.27.dist-info/top_level.txt
+Filename: ytdlp_servustv-2024.4.28.dist-info/top_level.txt
 Comment: 
 
-Filename: ytdlp_servustv-2023.12.27.dist-info/RECORD
+Filename: ytdlp_servustv-2024.4.28.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yt_dlp_plugins/extractor/servustv.py

```diff
@@ -1,26 +1,27 @@
 # coding: utf-8
+
 import re
 from typing import Any, Dict, Iterator, Optional, Sequence, Tuple
-from urllib.parse import parse_qsl, quote_plus, urlparse, urlunparse
+from urllib.parse import parse_qsl, urlparse, urlunparse
 
 from yt_dlp.extractor.common import InfoExtractor
 from yt_dlp.utils import (
     ExtractorError,
     GeoRestrictedError,
     OnDemandPagedList,
     UnsupportedError,
     get_element_by_id,
     int_or_none,
     parse_iso8601,
     traverse_obj,
     unescapeHTML,
 )
 
-__version__ = "2023.12.27"
+__version__ = "2024.04.28"
 AnyDict = Dict[str, Any]
 
 
 class ServusTVIE(InfoExtractor):
     IE_NAME = "servustv"
     _VALID_URL = r"""(?x)
                     https?://
@@ -99,32 +100,32 @@
                 "id": "aa-1qcy94h3s1w11",
                 "title": "startswith:Ich, Bauer",
                 "description": "md5:04cd98226e5c07ca50d0dc90f4a27ea1",
             },
             "playlist": [
                 {
                     "info_dict": {
-                        "id": "aarj7qi65ikr255p922y",
-                        "title": "Wir suchen keine Idylle",
+                        "id": "aat544m75z6xm4p93c7z",
+                        "title": "Jetzt oder nie!",
                         "series": "Ich, Bauer",
-                        "season_number": 4,
-                        "episode_number": 2,
-                        "description": "md5:8375fc598827c13c36bda1a98f89fa22",
+                        "season_number": 3,
+                        "episode_number": 4,
+                        "description": "md5:483c6d034a102caab4398826358b76af",
                         "timestamp": int,
                         "upload_date": "20220101",
                     },
                 },
                 {
                     "info_dict": {
-                        "id": "aat544m75z6xm4p93c7z",
-                        "title": "Jetzt oder nie!",
+                        "id": "aarj7qi65ikr255p922y",
+                        "title": "Wir suchen keine Idylle",
                         "series": "Ich, Bauer",
-                        "season_number": 3,
-                        "episode_number": 4,
-                        "description": "md5:483c6d034a102caab4398826358b76af",
+                        "season_number": 4,
+                        "episode_number": 2,
+                        "description": "md5:8375fc598827c13c36bda1a98f89fa22",
                         "timestamp": int,
                         "upload_date": "20220101",
                     },
                 },
             ],
             "params": {
                 "geo_bypass_country": "AT",
@@ -518,15 +519,16 @@
             page_data = traverse_obj(
                 json_obj, f"props/pageProps/{item}".split("/"), default={}
             )
             if page_data:
                 break
         return page_data
 
-    def _filter_query(self, json_obj: AnyDict, *names: str) -> Tuple[str, AnyDict]:
+    @staticmethod
+    def _filter_query(json_obj: AnyDict, *names: str) -> Tuple[str, AnyDict]:
         data = traverse_obj(
             json_obj,
             "props/pageProps/initialLibData".split("/"),
             "props/pageProps/data".split("/"),
             default={},
         )
         for filter_info in data.get("filters", ()):
@@ -589,159 +591,7 @@
         if not entries:
             raise UnsupportedError(url)
 
         return self.playlist_result(
             entries,
             **self._playlist_meta(page_data, webpage),
         )
-
-
-class ServusSearchIE(ServusTVIE):
-    IE_NAME = "servustv:search"
-    _VALID_URL = r"""(?x)
-                    https?://
-                        (?:www\.)?servustv.com
-                        /search
-                        /(?P<id>[^/?#]+)
-                        (?:/all-videos/\d+)?/?$
-                    """
-
-    _TESTS = [
-        {
-            # search playlist
-            "url": "https://www.servustv.com/search/hubert+staller/",
-            "info_dict": {
-                "id": "search_hubert+staller",
-                "title": "search: 'hubert staller'",
-                "description": None,
-            },
-            "params": {"skip_download": True, "geo_bypass": False},
-            "playlist_mincount": 1,
-            "playlist_maxcount": 10,
-        }
-    ]
-
-    def _playlist_meta(self, page_data, webpage):
-        search_term = page_data.get("searchTerm", "[searchTerm]")
-
-        return {
-            "playlist_id": f"search_{quote_plus(search_term)}",
-            "playlist_title": f"search: {search_term!r}",
-        }
-
-
-class PmWissenIE(ServusTVIE):
-    IE_NAME = "pm-wissen"
-    _VALID_URL = r"""(?x)
-                    https?://
-                        (?:www\.)?(?:pm-wissen)\.com/
-                        (?:
-                            videos | (?: [\w-]+/(?: v | [p]/[\w-]+ ) )
-                        )
-                        /(?P<id>[A-Za-z0-9-]+)
-                    """
-    _TESTS = [
-        {
-            # test embedded links from 3rd party sites
-            "url": "https://www.pm-wissen.com/umwelt/v/aaljbkmy7jwhcb6lb8lt/",
-            "info_dict": {
-                "id": "aaljbkmy7jwhcb6lb8lt",
-                "ext": "mp4",
-                "title": "Wie geht Weingärung?",
-                "description": str,
-                "duration": 340,
-                "timestamp": int,
-                "upload_date": str,
-                "is_live": False,
-                "thumbnail": r"re:^https?://.*\.jpg",
-            },
-            "params": {"skip_download": True, "format": "bestvideo"},
-        },
-        {
-            # topic playlist
-            "url": "https://www.pm-wissen.com/mediathek/p/redewendungen-mediathek/11908/",
-            "info_dict": {
-                "id": "redewendungen-mediathek",
-                "title": "Redewendungen Mediathek",
-                "description": "Alle Videos zum Thema Redewendungen",
-            },
-            "playlist_mincount": 10,
-            "params": {"skip_download": True},
-        },
-        {
-            # playlist from blocks (fails on older yt-dlp versions)
-            "url": "https://www.pm-wissen.com/mediathek/p/highlights-mediathek/11900/",
-            "info_dict": {
-                "id": "highlights-mediathek",
-                "title": "Mediathek",
-                "description": "md5:2260ac68a6ee376912beb4c73e3d5b33",
-            },
-            "playlist_mincount": 12,
-            "params": {"skip_download": True},
-        },
-    ]
-    JSON_OBJ_ID = "__FRONTITY_CONNECT_STATE__"
-
-    @staticmethod
-    def _page_data(json_obj):
-        for item in ("page", "data"):
-            page_data = traverse_obj(json_obj, f"source/{item}".split("/"), default={})
-            if page_data:
-                page_data = next(iter(page_data.values()))
-                break
-
-        return page_data
-
-    def _filter_query(self, json_obj, *names: str) -> Tuple[str, Dict]:
-        link = traverse_obj(json_obj, ("router", "link"), default="")
-        data = traverse_obj(
-            json_obj,
-            ("source", "data", link),
-            default={},
-        )
-        for filter_info in data.get("filters", ()):
-            name = filter_info.get("value", "none")
-            if name in names:
-                return name, filter_info
-
-        page_data = self._page_data(json_obj)
-        category = page_data.get("categories", ())
-        if category:
-            return category[0], {
-                "url": "https://backend.pm-wissen.com/wp-json/rbmh/v2/query-filters/query/?"
-                f"categories={category[0]}&f[primary_type_group]=all-videos&filter_bundles=true&"
-                "filter_non_visible_types=true&geo_override=DE&orderby=rbmh_playability&"
-                "page=3&per_page=12&post_type=media_asset&query_filters=primary_type_group"
-            }
-
-        return "none", {}
-
-
-class PmWissenSearchIE(PmWissenIE):
-    IE_NAME = "pm-wissen:search"
-    _VALID_URL = r"""(?x)
-                    https?://
-                        (?:www\.)?pm-wissen.com
-                        /search
-                        /(?P<id>[^/?#]+)
-                        (?:/all-videos/\d+)?/?$
-                    """
-    _TESTS = [
-        {
-            # search playlist
-            "url": "https://www.pm-wissen.com/search/weltall/",
-            "info_dict": {
-                "id": "search_weltall",
-                "title": "search: 'weltall'",
-            },
-            "params": {"skip_download": True, "geo_bypass": False},
-            "playlist_mincount": 15,
-        }
-    ]
-
-    def _playlist_meta(self, page_data, webpage):
-        search_query = page_data.get("searchQuery", "[searchQuery]")
-
-        return {
-            "playlist_id": f"search_{quote_plus(search_query)}",
-            "playlist_title": f"search: {search_query!r}",
-        }
```

## Comparing `ytdlp_servustv-2023.12.27.dist-info/LICENSE` & `ytdlp_servustv-2024.4.28.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-This is free and unencumbered software released into the public domain.
-
-Anyone is free to copy, modify, publish, use, compile, sell, or
-distribute this software, either in source code form or as a compiled
-binary, for any purpose, commercial or non-commercial, and by any
-means.
-
-In jurisdictions that recognize copyright laws, the author or authors
-of this software dedicate any and all copyright interest in the
-software to the public domain. We make this dedication for the benefit
-of the public at large and to the detriment of our heirs and
-successors. We intend this dedication to be an overt act of
-relinquishment in perpetuity of all present and future rights to this
-software under copyright law.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
-
-For more information, please refer to <https://unlicense.org/>
+This is free and unencumbered software released into the public domain.
+
+Anyone is free to copy, modify, publish, use, compile, sell, or
+distribute this software, either in source code form or as a compiled
+binary, for any purpose, commercial or non-commercial, and by any
+means.
+
+In jurisdictions that recognize copyright laws, the author or authors
+of this software dedicate any and all copyright interest in the
+software to the public domain. We make this dedication for the benefit
+of the public at large and to the detriment of our heirs and
+successors. We intend this dedication to be an overt act of
+relinquishment in perpetuity of all present and future rights to this
+software under copyright law.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
+
+For more information, please refer to <https://unlicense.org/>
```

## Comparing `ytdlp_servustv-2023.12.27.dist-info/METADATA` & `ytdlp_servustv-2024.4.28.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdlp-servustv
-Version: 2023.12.27
+Version: 2024.4.28
 Summary: yt-dlp extractor for servustv.com
 Home-page: https://github.com/flashdagger/ytdlp-plugins/tree/servustv
 Author: flashdagger
 Author-email: flashdagger@googlemail.com
 License: The Unlicense
 Keywords: yt-dlp,youtube-dl,servustv,extractors,plugins
 Platform: any
@@ -34,25 +34,26 @@
 > 
 > Since version 2023.01.06 yt-dlp supports plugins from python packages.
 > The ytdlp-plugins package is no longer necessary.
 > 
 > For further details see https://github.com/yt-dlp/yt-dlp#plugins
 
 
-* supported domains: [servustv.com](https://servustv.com) and [pm-wissen.com](https://pm-wissen.com)
+* supported domains: [servustv.com](https://servustv.com) 
+* unsupported domain: [pm-wissen.com](https://pm-wissen.com)
 * supported live channels:
   * [Hauptkanal](https://www.servustv.com/allgemein/p/jetzt-live/119753/) 
   * [Wetterpanorama](https://www.servustv.com/aktuelles/v/aa9bgcvsvf7sq8y4sm14/) 
   * [Kanal: Natur](https://www.servustv.com/natur/k/natur-kanal/269299/)
   * [Kanal: Wissen](https://www.servustv.com/wissen/k/wissen-kanal/269302/)
   * [Kanal: Sport](https://www.servustv.com/sport/k/sport-kanal/269300/)
   * [Kanal: Wintersport](https://www.servustv.com/sport/k/wintersport-kanal/269301/)
 * playlist from topics (e.g. [Servus Nachrichten](https://www.servustv.com/aktuelles/b/servus-nachrichten/aa-1y5rjcd1h2111/)
   or [Motorsport](https://www.servustv.com/sport/p/motorsport/325/))
-* playlist from searches (e.g. [search term 'Spielfilme\'](https://www.servustv.com/search/spielfilme/))
+* playlist from searches (not supported)
 
 ## installation
 
 You can install ytdlp-servustv via pip:
 
 * Use [PyPI package](https://pypi.org/project/yt-dlp):
```

