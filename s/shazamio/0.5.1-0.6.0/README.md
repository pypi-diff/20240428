# Comparing `tmp/shazamio-0.5.1.tar.gz` & `tmp/shazamio-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shazamio-0.5.1.tar", max compression
+gzip compressed data, was "shazamio-0.6.0.tar", max compression
```

## Comparing `shazamio-0.5.1.tar` & `shazamio-0.6.0.tar`

### file list

```diff
@@ -1,40 +1,45 @@
--rw-r--r--   0        0        0     1063 2024-02-25 01:12:57.278005 shazamio-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0    10417 2024-02-25 01:12:57.278005 shazamio-0.5.1/README.md
--rw-r--r--   0        0        0     1138 2024-02-25 01:13:10.278154 shazamio-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      231 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/__init__.py
--rw-r--r--   0        0        0    11260 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/algorithm.py
--rw-r--r--   0        0        0    20114 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/api.py
--rw-r--r--   0        0        0     2247 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/client.py
--rw-r--r--   0        0        0     2680 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/converter.py
--rw-r--r--   0        0        0        0 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/deprecated/__init__.py
--rw-r--r--   0        0        0      712 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/deprecated/decorator.py
--rw-r--r--   0        0        0      832 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/enums.py
--rw-r--r--   0        0        0      168 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/exceptions.py
--rw-r--r--   0        0        0     3458 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/factory.py
--rw-r--r--   0        0        0     1526 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/factory_misc.py
--rw-r--r--   0        0        0        0 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/interfaces/__init__.py
--rw-r--r--   0        0        0      318 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/interfaces/client.py
--rw-r--r--   0        0        0      101 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/loggers.py
--rw-r--r--   0        0        0     3270 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/misc.py
--rw-r--r--   0        0        0        0 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/artist/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/artist/views/__init__.py
--rw-r--r--   0        0        0     1874 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/artist/views/full_albums.py
--rw-r--r--   0        0        0     1487 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/artist/views/last_release.py
--rw-r--r--   0        0        0     1337 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/artist/views/simular_artists.py
--rw-r--r--   0        0        0     1406 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/artist/views/top_music.py
--rw-r--r--   0        0        0     1817 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/artist/views/top_song.py
--rw-r--r--   0        0        0     2752 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/artists.py
--rw-r--r--   0        0        0      345 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/attributes.py
--rw-r--r--   0        0        0      455 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/base.py
--rw-r--r--   0        0        0      464 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/enums.py
--rw-r--r--   0        0        0      138 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/errors.py
--rw-r--r--   0        0        0     4122 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/models.py
--rw-r--r--   0        0        0      526 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/photos.py
--rw-r--r--   0        0        0       71 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/schemas/urls.py
--rw-r--r--   0        0        0     1144 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/serializers.py
--rw-r--r--   0        0        0     8505 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/signature.py
--rw-r--r--   0        0        0      164 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/typehints.py
--rw-r--r--   0        0        0    59504 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/user_agent.py
--rw-r--r--   0        0        0     1776 2024-02-25 01:12:57.290005 shazamio-0.5.1/shazamio/utils.py
--rw-r--r--   0        0        0    11691 1970-01-01 00:00:00.000000 shazamio-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-27 22:22:33.991928 shazamio-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0    10417 2024-04-27 22:22:33.991928 shazamio-0.6.0/README.md
+-rw-r--r--   0        0        0     1129 2024-04-27 22:22:43.131991 shazamio-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/__init__.py
+-rw-r--r--   0        0        0    11260 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/algorithm.py
+-rw-r--r--   0        0        0    21200 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/api.py
+-rw-r--r--   0        0        0     2247 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/client.py
+-rw-r--r--   0        0        0     5161 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/converter.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/deprecated/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/deprecated/decorator.py
+-rw-r--r--   0        0        0     1015 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/enums.py
+-rw-r--r--   0        0        0      253 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/exceptions.py
+-rw-r--r--   0        0        0     3458 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/factory.py
+-rw-r--r--   0        0        0     1526 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/factory_misc.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/interfaces/__init__.py
+-rw-r--r--   0        0        0      318 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/interfaces/client.py
+-rw-r--r--   0        0        0      101 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/loggers.py
+-rw-r--r--   0        0        0     2691 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/misc.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/schemas/__init__.py
+-rw-r--r--   0        0        0      818 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/schemas/album.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/schemas/artist/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/schemas/artist/views/__init__.py
+-rw-r--r--   0        0        0     2091 2024-04-27 22:22:33.999928 shazamio-0.6.0/shazamio/schemas/artist/views/full_albums.py
+-rw-r--r--   0        0        0     1494 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/artist/views/last_release.py
+-rw-r--r--   0        0        0     1302 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/artist/views/simular_artists.py
+-rw-r--r--   0        0        0     1413 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/artist/views/top_music.py
+-rw-r--r--   0        0        0     1759 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/artist/views/top_song.py
+-rw-r--r--   0        0        0     2706 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/artists.py
+-rw-r--r--   0        0        0      345 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/attributes.py
+-rw-r--r--   0        0        0      725 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/base.py
+-rw-r--r--   0        0        0      279 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/content_version.py
+-rw-r--r--   0        0        0      464 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/enums.py
+-rw-r--r--   0        0        0      138 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/errors.py
+-rw-r--r--   0        0        0     4122 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/models.py
+-rw-r--r--   0        0        0      526 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/photos.py
+-rw-r--r--   0        0        0       88 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/play_params.py
+-rw-r--r--   0        0        0        0 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/playlist/__init__.py
+-rw-r--r--   0        0        0     1925 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/playlist/playlist.py
+-rw-r--r--   0        0        0       71 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/schemas/urls.py
+-rw-r--r--   0        0        0     1677 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/serializers.py
+-rw-r--r--   0        0        0     8505 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/signature.py
+-rw-r--r--   0        0        0      159 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/typehints.py
+-rw-r--r--   0        0        0    59504 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/user_agent.py
+-rw-r--r--   0        0        0     1776 2024-04-27 22:22:34.003928 shazamio-0.6.0/shazamio/utils.py
+-rw-r--r--   0        0        0    11588 1970-01-01 00:00:00.000000 shazamio-0.6.0/PKG-INFO
```

### Comparing `shazamio-0.5.1/LICENSE.txt` & `shazamio-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shazamio-0.5.1/README.md` & `shazamio-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `shazamio-0.5.1/pyproject.toml` & `shazamio-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shazamio"
-version = "0.5.1"
+version = "0.6.0"
 description = "Is a asynchronous framework from reverse engineered Shazam API written in Python 3.8+ with asyncio and aiohttp."
 authors = ["dotX12"]
 license = "MIT License"
 keywords = ["python", "shazam", "music", "recognize", "api", "async", "asyncio", "aiohttp", "identification"]
 readme = "README.md"
 homepage = "https://github.com/dotX12/ShazamIO"
 repository = "https://github.com/dotX12/ShazamIO"
@@ -15,24 +15,24 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.24.0"
 aiohttp = "^3.8.3"
 pydub = "^0.25.1"
 dataclass-factory = "2.16"
-aiofiles = "^22.1.0"
-pytest = "^7.2.0"
-pytest-asyncio = "^0.20.3"
-anyio = "^3.6.2"
+aiofiles = "23.2.1"
+anyio = "4.3.0"
 pydantic = "^1.10.2"
 shazamio-core = "^1.0.7"
 aiohttp-retry = "^2.8.3"
 
-[tool.poetry.group.dev.dependencies]
+[tool.poetry.dev-dependencies]
 black = {version = "^24.2.0", allow-prereleases = true}
+pytest = "8.1.2"
+pytest-asyncio = "^0.23.6"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "wheel>=0.36,<1.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.pytest.ini_options]
```

### Comparing `shazamio-0.5.1/shazamio/algorithm.py` & `shazamio-0.6.0/shazamio/algorithm.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.5.1/shazamio/api.py` & `shazamio-0.6.0/shazamio/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 
         self.core_recognizer = Recognizer()
         self.language = language
         self.endpoint_country = endpoint_country
 
         self.http_client = http_client or HTTPClient(
             retry_options=ExponentialRetry(
-                attempts=20, max_timeout=60, statuses={500, 502, 503, 504, 429}
+                attempts=20,
+                max_timeout=60,
+                statuses={500, 502, 503, 504, 429},
             ),
         )
         self.geo_service = GeoService(self.http_client)
 
     async def top_world_tracks(
         self,
         limit: int = 200,
@@ -58,17 +60,20 @@
                 Example: If 5 is specified, the query will return no more than 5 songs.
             :param offset: A parameter that determines with which song to display the request.
                 The default is 0. If you want to skip the first few songs, set this parameter to
                 your own.
             :param proxy: Proxy server
             :return: dict tracks
         """
+
+        top_playlist_id = await self.geo_service.get_top()
         return await self.http_client.request(
             "GET",
-            ShazamUrl.TOP_TRACKS_WORLD.format(
+            ShazamUrl.TOP_TRACKS_PLAYLIST.format(
+                playlist_id=top_playlist_id,
                 language=self.language,
                 endpoint_country=self.endpoint_country,
                 limit=limit,
                 offset=offset,
             ),
             headers=self.headers(),
             proxy=proxy,
@@ -129,15 +134,15 @@
             ),
             headers=self.headers(),
             proxy=proxy,
         )
 
     async def top_country_tracks(
         self,
-        country_code: Union[CountryCode, str],
+        country_code: str,
         limit: int = 200,
         offset: int = 0,
         proxy: Optional[str] = None,
     ) -> Dict[str, Any]:
         """
         Get the best tracks by country code
         https://www.shazam.com/charts/discovery/netherlands
@@ -147,30 +152,35 @@
                 Example: If 5 is specified, the query will return no more than 5 songs.
             :param offset: A parameter that determines with which song to display the request.
                 The default is 0. If you want to skip the first few songs, set this parameter to
                 your own.
             :param proxy: Proxy server
             :return: dict songs
         """
+        country_playlist_id = await self.geo_service.get_country_playlist(
+            country=CountryCode(country_code),
+        )
+
         return await self.http_client.request(
             "GET",
-            ShazamUrl.TOP_TRACKS_COUNTRY.format(
+            ShazamUrl.TOP_TRACKS_PLAYLIST.format(
+                playlist_id=country_playlist_id,
                 language=self.language,
                 endpoint_country=self.endpoint_country,
                 country_code=country_code,
                 limit=limit,
                 offset=offset,
             ),
             headers=self.headers(),
             proxy=proxy,
         )
 
     async def top_city_tracks(
         self,
-        country_code: Union[CountryCode, str],
+        country_code: str,
         city_name: str,
         limit: int = 200,
         offset: int = 0,
         proxy: Optional[str] = None,
     ) -> Dict[str, Any]:
         """
         Retrieving information from an artist profile
@@ -184,72 +194,75 @@
             :param offset: A parameter that determines with which song to display the request.
                 The default is 0. If you want to skip the first few songs, set this parameter to
                 your own.
             :param proxy: Proxy server
 
             :return: dict songs
         """
-        city_id = await self.geo_service.city_id_from(country=country_code, city=city_name)
+        city_playlist_id = await self.geo_service.get_city_playlist(
+            country=CountryCode(country_code),
+            city=city_name,
+        )
+
         return await self.http_client.request(
             "GET",
-            ShazamUrl.TOP_TRACKS_CITY.format(
+            ShazamUrl.TOP_TRACKS_PLAYLIST.format(
+                playlist_id=city_playlist_id,
                 language=self.language,
                 endpoint_country=self.endpoint_country,
+                country_code=country_code,
                 limit=limit,
                 offset=offset,
-                city_id=city_id,
             ),
             headers=self.headers(),
             proxy=proxy,
         )
 
     async def top_world_genre_tracks(
         self,
-        genre: Union[GenreMusic, int],
+        genre: Union[GenreMusic, str],
         limit: int = 100,
         offset: int = 0,
         proxy: Optional[str] = None,
     ) -> Dict[str, Any]:
         """
         Get world tracks by certain genre
         https://www.shazam.com/charts/genre/world/rock
 
-            :param genre: Genre name or ID:
-                POP = 1, HIP_HOP_RAP = 2, DANCE = 3, ELECTRONIC = 4, RNB_SOUL = 5, ALTERNATIVE =
-                6, ROCK = 7
-                LATIN = 8, FILM_TV_STAGE = 9, COUNTRY = 10, AFRO_BEATS = 11, WORLDWIDE = 12,
-                REGGAE_DANCE_HALL = 13
-                HOUSE = 14, K_POP = 15, FRENCH_POP = 16, SINGER_SONGWRITER = 17,
-                REGIONAL_MEXICANO = 18
-
+            :param genre: Genre urlName from https://www.shazam.com/services/charts/locations
             :param limit: Determines how many songs the maximum can be in the request.
                     Example: If 5 is specified, the query will return no more than 5 songs.
             :param offset: A parameter that determines with which song to display the request.
                     The default is 0. If you want to skip the first few songs, set this parameter
                     to your own.
             :param proxy: Proxy server
             :return: dict songs
         """
+
+        if isinstance(genre, str):
+            genre = GenreMusic(genre)
+
+        genre_playlist_id = await self.geo_service.get_genre(genre=genre)
         return await self.http_client.request(
             "GET",
-            ShazamUrl.GENRE_WORLD.format(
+            ShazamUrl.TOP_TRACKS_PLAYLIST.format(
+                playlist_id=genre_playlist_id,
                 language=self.language,
                 endpoint_country=self.endpoint_country,
                 limit=limit,
                 offset=offset,
-                genre=genre,
             ),
             headers=self.headers(),
             proxy=proxy,
         )
 
     async def top_country_genre_tracks(
         self,
         country_code: str,
-        genre: Union[GenreMusic, int],
+        genre: Union[GenreMusic, str],
         limit: int = 200,
         offset: int = 0,
         proxy: Optional[str] = None,
     ) -> Dict[str, Any]:
         """
         The best tracks by a genre in the country
         https://www.shazam.com/charts/genre/spain/hip-hop-rap
@@ -265,23 +278,31 @@
                 Example: If 5 is specified, the query will return no more than 5 songs
             :param offset: A parameter that determines with which song to display the request.
                 The default is 0. If you want to skip the first few songs, set this parameter to
                 your own.
             :param proxy: Proxy server
             :return: dict songs
         """
+        if isinstance(genre, str):
+            genre = GenreMusic(genre)
+
+        genre_playlist_id = await self.geo_service.get_genre_from_country(
+            country=CountryCode(country_code),
+            genre=genre,
+        )
+
         return await self.http_client.request(
             "GET",
-            ShazamUrl.GENRE_COUNTRY.format(
+            ShazamUrl.TOP_TRACKS_PLAYLIST.format(
+                playlist_id=genre_playlist_id,
                 language=self.language,
                 endpoint_country=self.endpoint_country,
+                country_code=country_code,
                 limit=limit,
                 offset=offset,
-                country=country_code,
-                genre=genre,
             ),
             headers=self.headers(),
             proxy=proxy,
         )
 
     async def related_tracks(
         self,
@@ -449,14 +470,37 @@
                 offset=offset,
                 artist_id=artist_id,
             ),
             headers=self.headers(),
             proxy=proxy,
         )
 
+    async def search_album(
+        self,
+        album_id: int,
+        proxy: Optional[str] = None,
+    ):
+        """
+        Get album info by id
+
+          :param album_id: Album number. Example (203347991)
+          :param proxy: Proxy server
+          :return: dict albums
+        """
+
+        return await self.http_client.request(
+            "GET",
+            ShazamUrl.ARTIST_ALBUM_INFO.format(
+                endpoint_country=self.endpoint_country,
+                album_id=album_id,
+            ),
+            headers=self.headers(),
+            proxy=proxy,
+        )
+
     async def get_youtube_data(
         self,
         link: str,
         proxy: Optional[str] = None,
     ) -> Dict[str, Any]:
         return await self.http_client.request(
             "GET",
@@ -514,15 +558,15 @@
             headers=self.headers(),
             proxy=proxy,
             json=data,
         )
 
     async def recognize(
         self,
-        data: Union[str, pathlib.Path, bytes, bytearray],
+        data: Union[str, bytes, bytearray],
         proxy: Optional[str] = None,
     ) -> Dict[str, Any]:
         """
         All logic and mathematics are transferred to RUST lang.
 
         Creating a song signature based on a file and searching for this signature in the shazam
         database.
```

### Comparing `shazamio-0.5.1/shazamio/client.py` & `shazamio-0.6.0/shazamio/client.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.5.1/shazamio/deprecated/decorator.py` & `shazamio-0.6.0/shazamio/deprecated/decorator.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.5.1/shazamio/enums.py` & `shazamio-0.6.0/shazamio/enums.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from enum import IntEnum
+from enum import IntEnum, Enum
 
 
-class GenreMusic(IntEnum):
-    POP = 1
-    HIP_HOP_RAP = 2
-    DANCE = 3
-    ELECTRONIC = 4
-    RNB_SOUL = 5
-    ALTERNATIVE = 6
-    ROCK = 7
-    LATIN = 8
-    FILM_TV_STAGE = 9
-    COUNTRY = 10
-    AFRO_BEATS = 11
-    WORLDWIDE = 12
-    REGGAE_DANCE_HALL = 13
-    HOUSE = 14
-    K_POP = 15
-    FRENCH_POP = 16
-    SINGER_SONGWRITER = 17
-    REGIONAL_MEXICANO = 18
+class GenreMusic(Enum):
+    POP = "pop"
+    HIP_HOP_RAP = "hip-hop-rap"
+    DANCE = "dance"
+    ELECTRONIC = "electronic"
+    RNB_SOUL = "randb-soul"
+    ALTERNATIVE = "alternative"
+    ROCK = "rock"
+    LATIN = "latin"
+    FILM_TV_STAGE = "film-tv-and-stage"
+    COUNTRY = "country"
+    AFRO_BEATS = "afrobeats"
+    WORLDWIDE = "worldwide"
+    REGGAE_DANCE_HALL = "reggae-dancehall"
+    HOUSE = "house"
+    K_POP = "k-pop"
+    FRENCH_POP = "french-pop"
+    SINGER_SONGWRITER = "singer-songwriter"
+    REGIONAL_MEXICANO = "regional-mexicano"
 
 
 class SampleRate(IntEnum):
     # Enum keys are sample rates in Hz
     _8000 = 1
     _11025 = 2
     _16000 = 3
```

### Comparing `shazamio-0.5.1/shazamio/factory.py` & `shazamio-0.6.0/shazamio/factory.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.5.1/shazamio/factory_misc.py` & `shazamio-0.6.0/shazamio/factory_misc.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.5.1/shazamio/misc.py` & `shazamio-0.6.0/shazamio/misc.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,39 +5,24 @@
 
 class ShazamUrl:
     SEARCH_FROM_FILE = (
         "https://amp.shazam.com/discovery/v5/{language}/{endpoint_country}/{device}/-/tag"
         "/{uuid_1}/{uuid_2}?sync=true&webv3=true&sampling=true"
         "&connected=&shazamapiversion=v3&sharehub=true&hubv5minorversion=v5.1&hidelb=true&video=v3"
     )
-    TOP_TRACKS_WORLD = (
-        "https://www.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
-        "/ip-global-chart?pageSize={limit}&startFrom={offset}"
-    )
     ABOUT_TRACK = (
         "https://www.shazam.com/discovery/v5/{language}/{endpoint_country}/web/-/track"
         "/{track_id}?shazamapiversion=v3&video=v3 "
     )
-    TOP_TRACKS_COUNTRY = (
-        "https://www.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
-        "/ip-country-chart-{country_code}?pageSize={limit}&startFrom={offset}"
-    )
-    TOP_TRACKS_CITY = (
-        "https://www.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
-        "/ip-city-chart-{city_id}?pageSize={limit}&startFrom={offset}"
+    TOP_TRACKS_PLAYLIST = (
+        "https://www.shazam.com/services/amapi/v1/catalog/{endpoint_country}"
+        "/playlists/{playlist_id}/tracks?limit={limit}&offset={offset}&"
+        "l={language}&relate[songs]=artists,music-videos"
     )
     LOCATIONS = "https://www.shazam.com/services/charts/locations"
-    GENRE_WORLD = (
-        "https://www.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
-        "/genre-global-chart-{genre}?pageSize={limit}&startFrom={offset}"
-    )
-    GENRE_COUNTRY = (
-        "https://www.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
-        "/genre-country-chart-{country}-{genre}?pageSize={limit}&startFrom={offset}"
-    )
     RELATED_SONGS = (
         "https://cdn.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
         "/track-similarities-id-{track_id}?startFrom={offset}&pageSize={limit}&connected=&channel="
     )
     SEARCH_ARTIST = (
         "https://www.shazam.com/services/search/v4/{language}/{endpoint_country}/web"
         "/search?term={query}&limit={limit}&offset={offset}&types=artists"
@@ -52,14 +37,17 @@
     SEARCH_ARTIST_V2 = (
         "https://www.shazam.com/services/amapi/v1/catalog/{endpoint_country}/artists/{artist_id}"
     )
     ARTIST_ALBUMS = (
         "https://www.shazam.com/services/amapi/v1/catalog/{endpoint_country}"
         "/artists/{artist_id}/albums?limit={limit}&offset={offset}"
     )
+    ARTIST_ALBUM_INFO = (
+        "https://www.shazam.com/services/amapi/v1/catalog/{endpoint_country}/albums/{album_id}"
+    )
 
 
 class Request:
     TIME_ZONE = "Europe/Moscow"
 
     def __init__(self, language: str):
         self.language = language
```

### Comparing `shazamio-0.5.1/shazamio/schemas/artist/views/full_albums.py` & `shazamio-0.6.0/shazamio/schemas/artist/views/full_albums.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
 from pydantic import BaseModel, Field
 
+from shazamio.schemas.play_params import PlayParams
 from shazamio.schemas.attributes import AttributeName
-from shazamio.schemas.base import BaseDataModel
+from shazamio.schemas.base import BaseIdTypeHrefAttributesModel
 from shazamio.schemas.photos import ImageModel
 
 
-class PlayParams(BaseModel):
-    id: str
-    kind: str
-
-
 class EditorialArtwork(BaseModel):
     subscription_hero: Optional[ImageModel] = Field(None, alias="subscriptionHero")
     store_flow_case: Optional[ImageModel] = Field(None, alias="storeFlowcase")
 
 
 class EditorialNotes(BaseModel):
     standard: Optional[str] = None
@@ -46,8 +42,14 @@
     is_complete: bool = Field(..., alias="isComplete")
     editorial_notes: Optional[EditorialNotes] = Field(None, alias="editorialNotes")
 
 
 class FullAlbumsModel(BaseModel):
     href: Optional[str] = None
     attributes: Optional[AttributeName] = None
-    data: Optional[List[BaseDataModel[AttributesFullAlbums]]] = None
+    data: List[BaseIdTypeHrefAttributesModel[AttributesFullAlbums]] = Field([])
+
+
+class SmallAlbumsModel(BaseModel):
+    href: Optional[str] = None
+    attributes: Optional[AttributeName] = None
+    data: List[BaseIdTypeHrefAttributesModel[AttributesFullAlbums]] = Field([])
```

### Comparing `shazamio-0.5.1/shazamio/schemas/artist/views/last_release.py` & `shazamio-0.6.0/shazamio/schemas/artist/views/last_release.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, Field
 
+from shazamio.schemas.play_params import PlayParams
 from shazamio.schemas.attributes import AttributeName
-from shazamio.schemas.base import BaseDataModel
+from shazamio.schemas.base import BaseAttributesModel
 from shazamio.schemas.photos import ImageModel
 
 
-class PlayParams(BaseModel):
-    id: str
-    kind: str
-
-
 class AttributeLastRelease(BaseModel):
     copyright: str
     genre_names: List[str] = Field(..., alias="genreNames")
     release_date: str = Field(..., alias="releaseDate")
     is_mastered_for_itunes: bool = Field(..., alias="isMasteredForItunes")
     upc: str
     artwork: ImageModel
@@ -35,8 +31,8 @@
     content_rating: Optional[str] = Field(None, alias="contentRating")
     is_complete: bool = Field(..., alias="isComplete")
 
 
 class LastReleaseModel(BaseModel):
     href: Optional[str] = None
     attributes: Optional[AttributeName] = None
-    data: Optional[List[BaseDataModel[AttributeLastRelease]]] = None
+    data: Optional[List[BaseAttributesModel[AttributeLastRelease]]] = None
```

### Comparing `shazamio-0.5.1/shazamio/schemas/artist/views/simular_artists.py` & `shazamio-0.6.0/shazamio/schemas/artist/views/simular_artists.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,18 +28,15 @@
     artist_bio: Optional[str] = Field(None, alias="artistBio")
 
 
 class Relationships(BaseModel):
     albums: BaseHrefNextData[List[BaseIdTypeHref]]
 
 
-class Datum(BaseModel):
-    id: str
-    type: str
-    href: str
+class Datum(BaseIdTypeHref):
     attributes: Attributes
     relationships: Relationships
 
 
 class SimularArtist(BaseModel):
     href: Optional[str] = None
     next: Optional[str] = None
```

### Comparing `shazamio-0.5.1/shazamio/schemas/artist/views/top_music.py` & `shazamio-0.6.0/shazamio/schemas/artist/views/top_music.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, Field
 
+from shazamio.schemas.play_params import PlayParams
 from shazamio.schemas.attributes import AttributeName
-from shazamio.schemas.base import BaseDataModel
+from shazamio.schemas.base import BaseAttributesModel
 from shazamio.schemas.photos import ImageModel
 
 
-class PlayParams(BaseModel):
-    id: str
-    kind: str
-
-
 class Preview(BaseModel):
     url: str
     hls_url: str = Field(..., alias="hlsUrl")
     artwork: ImageModel
 
 
 class Attributes(BaseModel):
@@ -38,8 +34,8 @@
     album_name: Optional[str] = Field(None, alias="albumName")
     track_number: Optional[int] = Field(None, alias="trackNumber")
 
 
 class TopMusicVideosView(BaseModel):
     href: Optional[str] = None
     attributes: Optional[AttributeName] = None
-    data: Optional[List[BaseDataModel[Attributes]]] = None
+    data: Optional[List[BaseAttributesModel[Attributes]]] = None
```

### Comparing `shazamio-0.5.1/shazamio/schemas/artist/views/top_song.py` & `shazamio-0.6.0/shazamio/schemas/artist/views/top_song.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import List, Optional
 
 from pydantic import BaseModel, Field
 
 from shazamio.schemas.artist.views.top_music import PlayParams
 from shazamio.schemas.attributes import AttributeName
-from shazamio.schemas.base import BaseDataModel
+from shazamio.schemas.base import BaseAttributesModel, BaseIdTypeHref
 from shazamio.schemas.photos import ImageModel
 from shazamio.schemas.urls import UrlDTO
 
 
 class AttributesTopSong(BaseModel):
     has_time_synced_lyrics: bool = Field(..., alias="hasTimeSyncedLyrics")
     album_name: Optional[str] = Field(None, alias="albumName")
@@ -32,13 +32,10 @@
     audio_traits: List[str] = Field(..., alias="audioTraits")
     name: str
     previews: List[UrlDTO] = Field([])
     artist_name: str = Field(..., alias="artistName")
     content_rating: Optional[str] = Field(None, alias="contentRating")
 
 
-class TopSong(BaseModel):
-    id: Optional[str] = None
-    type: Optional[str] = None
-    href: Optional[str] = None
+class TopSong(BaseIdTypeHref):
     attributes: Optional[AttributeName] = None
-    data: Optional[List[BaseDataModel[AttributesTopSong]]] = None
+    data: Optional[List[BaseAttributesModel[AttributesTopSong]]] = None
```

### Comparing `shazamio-0.5.1/shazamio/schemas/artists.py` & `shazamio-0.6.0/shazamio/schemas/artists.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List
 from typing import Optional
 from typing import Union
 
 from pydantic import BaseModel
 from pydantic import Field
 
+from shazamio.schemas.base import BaseIdTypeHref
 from shazamio.schemas.artist.views.full_albums import FullAlbumsModel
 from shazamio.schemas.artist.views.last_release import LastReleaseModel
 from shazamio.schemas.artist.views.simular_artists import SimularArtist
 from shazamio.schemas.artist.views.top_music import TopMusicVideosView
 from shazamio.schemas.artist.views.top_song import TopSong
 from shazamio.schemas.attributes import ArtistAttribute
 from shazamio.schemas.enums import ArtistExtend
@@ -59,24 +60,18 @@
     url: str
 
     @classmethod
     def url_with_size(cls, height: int, width: int) -> str:
         return cls.url.format(w=width, h=height)
 
 
-class AlbumRelationshipElement(BaseModel):
-    id: str
-    type: str
-    href: str
-
-
 class AlbumRelationship(BaseModel):
     href: str
     next: Optional[str] = None
-    data: List[AlbumRelationshipElement]
+    data: List[BaseIdTypeHref]
 
 
 class ArtistRelationships(BaseModel):
     albums: AlbumRelationship
 
 
 class ArtistViews(BaseModel):
```

### Comparing `shazamio-0.5.1/shazamio/schemas/models.py` & `shazamio-0.6.0/shazamio/schemas/models.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.5.1/shazamio/schemas/photos.py` & `shazamio-0.6.0/shazamio/schemas/photos.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.5.1/shazamio/serializers.py` & `shazamio-0.6.0/shazamio/serializers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,37 @@
-from typing import Union
+from typing import Union, List
 
+from shazamio.schemas.base import BaseDataModel
 from shazamio.factory_misc import FACTORY_ARTIST
 from shazamio.factory_misc import FACTORY_TRACK
 from shazamio.schemas.artist.views.full_albums import FullAlbumsModel
 from shazamio.schemas.artists import ArtistInfo
 from shazamio.schemas.artists import ArtistResponse
 from shazamio.schemas.artists import ArtistV2
 from shazamio.schemas.models import ResponseTrack
 from shazamio.schemas.models import TrackInfo
 from shazamio.schemas.models import YoutubeData
+from shazamio.schemas.album import AlbumModel
+from shazamio.schemas.playlist.playlist import PlayList
 
 
 class Serialize:
     @classmethod
     def track(cls, data):
         return FACTORY_TRACK.load(data, TrackInfo)
 
     @classmethod
+    def playlist(cls, data) -> PlayList:
+        return PlayList.parse_obj(data)
+
+    @classmethod
+    def playlists(cls, data) -> List[PlayList]:
+        return [cls.playlist(pl) for pl in data.get("data", [])]
+
+    @classmethod
     def youtube(cls, data):
         return FACTORY_TRACK.load(data, YoutubeData)
 
     @classmethod
     def artist_v2(cls, data) -> ArtistResponse:
         return ArtistResponse.parse_obj(data)
 
@@ -31,7 +42,11 @@
     @classmethod
     def artist(cls, data):
         return FACTORY_ARTIST.load(data, Union[ArtistV2, ArtistInfo])
 
     @classmethod
     def full_track(cls, data):
         return FACTORY_TRACK.load(data, ResponseTrack)
+
+    @classmethod
+    def album_info(cls, data) -> BaseDataModel[List[AlbumModel]]:
+        return BaseDataModel[List[AlbumModel]].parse_obj(data)
```

### Comparing `shazamio-0.5.1/shazamio/signature.py` & `shazamio-0.6.0/shazamio/signature.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.5.1/shazamio/user_agent.py` & `shazamio-0.6.0/shazamio/user_agent.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.5.1/shazamio/utils.py` & `shazamio-0.6.0/shazamio/utils.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.5.1/PKG-INFO` & `shazamio-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: shazamio
-Version: 0.5.1
+Version: 0.6.0
 Summary: Is a asynchronous framework from reverse engineered Shazam API written in Python 3.8+ with asyncio and aiohttp.
 Home-page: https://github.com/dotX12/ShazamIO
 License: MIT
 Keywords: python,shazam,music,recognize,api,async,asyncio,aiohttp,identification
 Author: dotX12
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiofiles (>=22.1.0,<23.0.0)
+Requires-Dist: aiofiles (==23.2.1)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiohttp-retry (>=2.8.3,<3.0.0)
-Requires-Dist: anyio (>=3.6.2,<4.0.0)
+Requires-Dist: anyio (==4.3.0)
 Requires-Dist: dataclass-factory (==2.16)
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
-Requires-Dist: pytest (>=7.2.0,<8.0.0)
-Requires-Dist: pytest-asyncio (>=0.20.3,<0.21.0)
 Requires-Dist: shazamio-core (>=1.0.7,<2.0.0)
 Project-URL: Repository, https://github.com/dotX12/ShazamIO
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://scrutinizer-ci.com/g/dotX12/ShazamIO/badges/quality-score.png?b=master" alt="https://scrutinizer-ci.com/g/dotX12/ShazamIO/">
 <img src="https://scrutinizer-ci.com/g/dotX12/ShazamIO/badges/code-intelligence.svg?b=master" alt="https://scrutinizer-ci.com/g/dotX12/ShazamIO/">
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: shazamio Version: 0.5.1 Summary: Is a asynchronous
+Metadata-Version: 2.1 Name: shazamio Version: 0.6.0 Summary: Is a asynchronous
 framework from reverse engineered Shazam API written in Python 3.8+ with
 asyncio and aiohttp. Home-page: https://github.com/dotX12/ShazamIO License: MIT
 Keywords:
 python,shazam,music,recognize,api,async,asyncio,aiohttp,identification Author:
 dotX12 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiofiles (>=22.1.0,<23.0.0) Requires-Dist: aiohttp
-(>=3.8.3,<4.0.0) Requires-Dist: aiohttp-retry (>=2.8.3,<3.0.0) Requires-Dist:
-anyio (>=3.6.2,<4.0.0) Requires-Dist: dataclass-factory (==2.16) Requires-Dist:
-numpy (>=1.24.0,<2.0.0) Requires-Dist: pydantic (>=1.10.2,<2.0.0) Requires-
-Dist: pydub (>=0.25.1,<0.26.0) Requires-Dist: pytest (>=7.2.0,<8.0.0) Requires-
-Dist: pytest-asyncio (>=0.20.3,<0.21.0) Requires-Dist: shazamio-core
-(>=1.0.7,<2.0.0) Project-URL: Repository, https://github.com/dotX12/ShazamIO
-Description-Content-Type: text/markdown
+Requires-Dist: aiofiles (==23.2.1) Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: aiohttp-retry (>=2.8.3,<3.0.0) Requires-Dist: anyio (==4.3.0)
+Requires-Dist: dataclass-factory (==2.16) Requires-Dist: numpy
+(>=1.24.0,<2.0.0) Requires-Dist: pydantic (>=1.10.2,<2.0.0) Requires-Dist:
+pydub (>=0.25.1,<0.26.0) Requires-Dist: shazamio-core (>=1.0.7,<2.0.0) Project-
+URL: Repository, https://github.com/dotX12/ShazamIO Description-Content-Type:
+text/markdown
  [https://scrutinizer-ci.com/g/dotX12/ShazamIO/][https://scrutinizer-ci.com/g/
    dotX12/ShazamIO/][https://scrutinizer-ci.com/g/dotX12/ShazamIO/][https://
     badge.fury.io/py/shazamio][https://pepy.tech/project/shazamio][https://
   pepy.tech/project/shazamio][https://github.com/dotX12/ShazamIO/blob/master/
                                  LICENSE.txt]
 
  [https://user-images.githubusercontent.com/64792903/109359596-ca561a00-7896-
```

