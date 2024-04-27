# Comparing `tmp/nokey-0.3.1.tar.gz` & `tmp/nokey-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nokey-0.3.1.tar", last modified: Sat Apr 27 14:06:34 2024, max compression
+gzip compressed data, was "nokey-0.3.2.tar", last modified: Sat Apr 27 23:51:19 2024, max compression
```

## Comparing `nokey-0.3.1.tar` & `nokey-0.3.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.797063 nokey-0.3.1/
--rw-------   0 root         (0) root         (0)     1068 2024-04-10 23:28:41.000000 nokey-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3685 2024-04-27 14:06:34.797063 nokey-0.3.1/PKG-INFO
--rw-------   0 root         (0) root         (0)     3164 2024-04-27 13:46:03.000000 nokey-0.3.1/README.md
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.489063 nokey-0.3.1/nokey/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/__init__.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.509063 nokey-0.3.1/nokey/activities/
--rw-------   0 root         (0) root         (0)     5116 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/activities/bored_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.521063 nokey-0.3.1/nokey/animals/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/animals/__init__.py
--rw-------   0 root         (0) root         (0)     2754 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/animals/dog_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.525063 nokey-0.3.1/nokey/art_and_images/
--rw-------   0 root         (0) root         (0)     7770 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/art_and_images/lorem_picsum.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.537063 nokey-0.3.1/nokey/books_and_literature/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/books_and_literature/__init__.py
--rw-------   0 root         (0) root         (0)     6079 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/books_and_literature/gutendex.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.545063 nokey-0.3.1/nokey/calendar/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/calendar/__init__.py
--rw-------   0 root         (0) root         (0)     4848 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/calendar/nager_date.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.557063 nokey-0.3.1/nokey/country_info/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/country_info/__init__.py
--rw-------   0 root         (0) root         (0)     4740 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/country_info/rest_country.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.589063 nokey-0.3.1/nokey/developer_tools/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/developer_tools/__init__.py
--rw-------   0 root         (0) root         (0)     3945 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/developer_tools/apis_guru.py
--rw-------   0 root         (0) root         (0)     3564 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/developer_tools/filter_lists.py
--rw-------   0 root         (0) root         (0)     2578 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/developer_tools/microlink.py
--rw-------   0 root         (0) root         (0)     7314 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/developer_tools/url_haus.py
--rw-------   0 root         (0) root         (0)     1621 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/developer_tools/url_shortener.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.601063 nokey-0.3.1/nokey/education/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/education/__init__.py
--rw-------   0 root         (0) root         (0)     2348 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/education/university_domains_and_names.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.621063 nokey-0.3.1/nokey/finance_and_crypto/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/finance_and_crypto/__init__.py
--rw-------   0 root         (0) root         (0)     5877 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/finance_and_crypto/coinmap.py
--rw-------   0 root         (0) root         (0)     2513 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/finance_and_crypto/exchange_api.py
--rw-------   0 root         (0) root         (0)     1127 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/finance_and_crypto/wall_street_bets.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.633063 nokey-0.3.1/nokey/food/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/food/__init__.py
--rw-------   0 root         (0) root         (0)     3198 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/food/fruityvice.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.649063 nokey-0.3.1/nokey/games/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/games/__init__.py
--rw-------   0 root         (0) root         (0)     6542 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/games/free_to_game.py
--rw-------   0 root         (0) root         (0)     5382 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/games/open_trivia_db.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.661063 nokey-0.3.1/nokey/geolocation/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/geolocation/__init__.py
--rw-------   0 root         (0) root         (0)     1045 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/geolocation/ip_api.py
--rw-------   0 root         (0) root         (0)     1874 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/geolocation/zippopotamus.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.673063 nokey-0.3.1/nokey/government/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/government/__init__.py
--rw-------   0 root         (0) root         (0)    10654 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/government/federal_register.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.693063 nokey-0.3.1/nokey/helperFuncs/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/helperFuncs/__init__.py
--rw-------   0 root         (0) root         (0)      822 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/helperFuncs/get_api_list.py
--rw-------   0 root         (0) root         (0)     3234 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/helperFuncs/make_request.py
--rw-------   0 root         (0) root         (0)      954 2024-04-27 14:00:02.000000 nokey-0.3.1/nokey/helperFuncs/nokey_apis.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.705063 nokey-0.3.1/nokey/inspiration/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/inspiration/__init__.py
--rw-------   0 root         (0) root         (0)     5925 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/inspiration/dictum.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.717063 nokey-0.3.1/nokey/jokes/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/jokes/__init__.py
--rw-------   0 root         (0) root         (0)     3004 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/jokes/joke_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.725063 nokey-0.3.1/nokey/language/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/language/__init__.py
--rw-------   0 root         (0) root         (0)     1185 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/language/free_dictionary.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.737063 nokey-0.3.1/nokey/random/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/random/__init__.py
--rw-------   0 root         (0) root         (0)     1119 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/random/random_user.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.753063 nokey-0.3.1/nokey/science_and_nature/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/science_and_nature/__init__.py
--rw-------   0 root         (0) root         (0)    50596 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/science_and_nature/integrated_taxonomic_information_system.py
--rw-------   0 root         (0) root         (0)     2948 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/science_and_nature/nobel_prize.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.765063 nokey-0.3.1/nokey/spaceflight/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/spaceflight/__init__.py
--rw-------   0 root         (0) root         (0)     8784 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/spaceflight/spaceflight_news.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.773063 nokey-0.3.1/nokey/tv_and_film/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/tv_and_film/__init__.py
--rw-------   0 root         (0) root         (0)    43523 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/tv_and_film/star_trek_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.785063 nokey-0.3.1/nokey/weather/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/weather/__init__.py
--rw-------   0 root         (0) root         (0)    26115 2024-04-27 13:48:18.000000 nokey-0.3.1/nokey/weather/national_weather_service.py
-drwx------   0 root         (0) root         (0)        0 2024-04-27 14:06:34.793063 nokey-0.3.1/nokey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3685 2024-04-27 14:06:34.000000 nokey-0.3.1/nokey.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)     1918 2024-04-27 14:06:34.000000 nokey-0.3.1/nokey.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2024-04-27 14:06:34.000000 nokey-0.3.1/nokey.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)        6 2024-04-27 14:06:34.000000 nokey-0.3.1/nokey.egg-info/top_level.txt
--rw-------   0 root         (0) root         (0)      503 2024-04-27 14:05:13.000000 nokey-0.3.1/pyproject.toml
--rw-------   0 root         (0) root         (0)       38 2024-04-27 14:06:34.801063 nokey-0.3.1/setup.cfg
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.326280 nokey-0.3.2/
+-rw-------   0 root         (0) root         (0)     1068 2024-04-10 23:28:41.000000 nokey-0.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3685 2024-04-27 23:51:19.322280 nokey-0.3.2/PKG-INFO
+-rw-------   0 root         (0) root         (0)     3164 2024-04-27 13:46:03.000000 nokey-0.3.2/README.md
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.022280 nokey-0.3.2/nokey/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/__init__.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.042280 nokey-0.3.2/nokey/activities/
+-rw-------   0 root         (0) root         (0)     5116 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/activities/bored_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.050280 nokey-0.3.2/nokey/animals/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/animals/__init__.py
+-rw-------   0 root         (0) root         (0)     2754 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/animals/dog_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.058280 nokey-0.3.2/nokey/art_and_images/
+-rw-------   0 root         (0) root         (0)     7770 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/art_and_images/lorem_picsum.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.070280 nokey-0.3.2/nokey/books_and_literature/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/books_and_literature/__init__.py
+-rw-------   0 root         (0) root         (0)     6079 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/books_and_literature/gutendex.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.078280 nokey-0.3.2/nokey/calendar/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/calendar/__init__.py
+-rw-------   0 root         (0) root         (0)     4848 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/calendar/nager_date.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.090280 nokey-0.3.2/nokey/country_info/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/country_info/__init__.py
+-rw-------   0 root         (0) root         (0)     4740 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/country_info/rest_country.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.122280 nokey-0.3.2/nokey/developer_tools/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/developer_tools/__init__.py
+-rw-------   0 root         (0) root         (0)     3945 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/developer_tools/apis_guru.py
+-rw-------   0 root         (0) root         (0)     3564 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/developer_tools/filter_lists.py
+-rw-------   0 root         (0) root         (0)     2578 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/developer_tools/microlink.py
+-rw-------   0 root         (0) root         (0)     7314 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/developer_tools/url_haus.py
+-rw-------   0 root         (0) root         (0)     1621 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/developer_tools/url_shortener.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.130280 nokey-0.3.2/nokey/education/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/education/__init__.py
+-rw-------   0 root         (0) root         (0)     2348 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/education/university_domains_and_names.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.154280 nokey-0.3.2/nokey/finance_and_crypto/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/finance_and_crypto/__init__.py
+-rw-------   0 root         (0) root         (0)     5877 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/finance_and_crypto/coinmap.py
+-rw-------   0 root         (0) root         (0)     2513 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/finance_and_crypto/exchange_api.py
+-rw-------   0 root         (0) root         (0)     1127 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/finance_and_crypto/wall_street_bets.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.162280 nokey-0.3.2/nokey/food/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/food/__init__.py
+-rw-------   0 root         (0) root         (0)     3198 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/food/fruityvice.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.178280 nokey-0.3.2/nokey/games/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/games/__init__.py
+-rw-------   0 root         (0) root         (0)     6542 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/games/free_to_game.py
+-rw-------   0 root         (0) root         (0)     5382 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/games/open_trivia_db.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.194280 nokey-0.3.2/nokey/geolocation/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/geolocation/__init__.py
+-rw-------   0 root         (0) root         (0)     1045 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/geolocation/ip_api.py
+-rw-------   0 root         (0) root         (0)     1874 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/geolocation/zippopotamus.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.202280 nokey-0.3.2/nokey/government/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/government/__init__.py
+-rw-------   0 root         (0) root         (0)    10654 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/government/federal_register.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.222280 nokey-0.3.2/nokey/helperFuncs/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/helperFuncs/__init__.py
+-rw-------   0 root         (0) root         (0)      822 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/helperFuncs/get_api_list.py
+-rw-------   0 root         (0) root         (0)     3234 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/helperFuncs/make_request.py
+-rw-------   0 root         (0) root         (0)      954 2024-04-27 14:00:02.000000 nokey-0.3.2/nokey/helperFuncs/nokey_apis.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.234280 nokey-0.3.2/nokey/inspiration/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/inspiration/__init__.py
+-rw-------   0 root         (0) root         (0)     5925 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/inspiration/dictum.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.242280 nokey-0.3.2/nokey/jokes/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/jokes/__init__.py
+-rw-------   0 root         (0) root         (0)     3004 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/jokes/joke_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.254280 nokey-0.3.2/nokey/language/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/language/__init__.py
+-rw-------   0 root         (0) root         (0)     1185 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/language/free_dictionary.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.262280 nokey-0.3.2/nokey/random/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/random/__init__.py
+-rw-------   0 root         (0) root         (0)     1119 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/random/random_user.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.278280 nokey-0.3.2/nokey/science_and_nature/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/science_and_nature/__init__.py
+-rw-------   0 root         (0) root         (0)    50596 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/science_and_nature/integrated_taxonomic_information_system.py
+-rw-------   0 root         (0) root         (0)     2948 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/science_and_nature/nobel_prize.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.290280 nokey-0.3.2/nokey/spaceflight/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/spaceflight/__init__.py
+-rw-------   0 root         (0) root         (0)     8784 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/spaceflight/spaceflight_news.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.302280 nokey-0.3.2/nokey/tv_and_film/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/tv_and_film/__init__.py
+-rw-------   0 root         (0) root         (0)    43523 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/tv_and_film/star_trek_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.314280 nokey-0.3.2/nokey/weather/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/weather/__init__.py
+-rw-------   0 root         (0) root         (0)    26115 2024-04-27 13:48:18.000000 nokey-0.3.2/nokey/weather/national_weather_service.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 23:51:19.318280 nokey-0.3.2/nokey.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3685 2024-04-27 23:51:18.000000 nokey-0.3.2/nokey.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)     1918 2024-04-27 23:51:18.000000 nokey-0.3.2/nokey.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2024-04-27 23:51:18.000000 nokey-0.3.2/nokey.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)        6 2024-04-27 23:51:18.000000 nokey-0.3.2/nokey.egg-info/top_level.txt
+-rw-------   0 root         (0) root         (0)      597 2024-04-27 23:49:01.000000 nokey-0.3.2/pyproject.toml
+-rw-------   0 root         (0) root         (0)       38 2024-04-27 23:51:19.326280 nokey-0.3.2/setup.cfg
```

### Comparing `nokey-0.3.1/LICENSE` & `nokey-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/PKG-INFO` & `nokey-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.3.1
+Version: 0.3.2
 Summary: A python package for accessing APIs that require no key.
 Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
 Project-URL: Homepage, https://github.com/SpyderRex/nokey
 Project-URL: Issues, https://github.com/Spyder/nokey/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nokey-0.3.1/README.md` & `nokey-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/activities/bored_api.py` & `nokey-0.3.2/nokey/activities/bored_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/animals/dog_api.py` & `nokey-0.3.2/nokey/animals/dog_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/art_and_images/lorem_picsum.py` & `nokey-0.3.2/nokey/art_and_images/lorem_picsum.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/books_and_literature/gutendex.py` & `nokey-0.3.2/nokey/books_and_literature/gutendex.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/calendar/nager_date.py` & `nokey-0.3.2/nokey/calendar/nager_date.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/country_info/rest_country.py` & `nokey-0.3.2/nokey/country_info/rest_country.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/developer_tools/apis_guru.py` & `nokey-0.3.2/nokey/developer_tools/apis_guru.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/developer_tools/filter_lists.py` & `nokey-0.3.2/nokey/developer_tools/filter_lists.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/developer_tools/microlink.py` & `nokey-0.3.2/nokey/developer_tools/microlink.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/developer_tools/url_haus.py` & `nokey-0.3.2/nokey/developer_tools/url_haus.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/developer_tools/url_shortener.py` & `nokey-0.3.2/nokey/developer_tools/url_shortener.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/education/university_domains_and_names.py` & `nokey-0.3.2/nokey/education/university_domains_and_names.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/finance_and_crypto/coinmap.py` & `nokey-0.3.2/nokey/finance_and_crypto/coinmap.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/finance_and_crypto/exchange_api.py` & `nokey-0.3.2/nokey/finance_and_crypto/exchange_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/finance_and_crypto/wall_street_bets.py` & `nokey-0.3.2/nokey/finance_and_crypto/wall_street_bets.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/food/fruityvice.py` & `nokey-0.3.2/nokey/food/fruityvice.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/games/free_to_game.py` & `nokey-0.3.2/nokey/games/free_to_game.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/games/open_trivia_db.py` & `nokey-0.3.2/nokey/games/open_trivia_db.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/geolocation/ip_api.py` & `nokey-0.3.2/nokey/geolocation/ip_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/geolocation/zippopotamus.py` & `nokey-0.3.2/nokey/geolocation/zippopotamus.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/government/federal_register.py` & `nokey-0.3.2/nokey/government/federal_register.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/helperFuncs/get_api_list.py` & `nokey-0.3.2/nokey/helperFuncs/get_api_list.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/helperFuncs/make_request.py` & `nokey-0.3.2/nokey/helperFuncs/make_request.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/helperFuncs/nokey_apis.py` & `nokey-0.3.2/nokey/helperFuncs/nokey_apis.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/inspiration/dictum.py` & `nokey-0.3.2/nokey/inspiration/dictum.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/jokes/joke_api.py` & `nokey-0.3.2/nokey/jokes/joke_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/language/free_dictionary.py` & `nokey-0.3.2/nokey/language/free_dictionary.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/random/random_user.py` & `nokey-0.3.2/nokey/random/random_user.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/science_and_nature/integrated_taxonomic_information_system.py` & `nokey-0.3.2/nokey/science_and_nature/integrated_taxonomic_information_system.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/science_and_nature/nobel_prize.py` & `nokey-0.3.2/nokey/science_and_nature/nobel_prize.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/spaceflight/spaceflight_news.py` & `nokey-0.3.2/nokey/spaceflight/spaceflight_news.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/tv_and_film/star_trek_api.py` & `nokey-0.3.2/nokey/tv_and_film/star_trek_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey/weather/national_weather_service.py` & `nokey-0.3.2/nokey/weather/national_weather_service.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.1/nokey.egg-info/PKG-INFO` & `nokey-0.3.2/nokey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.3.1
+Version: 0.3.2
 Summary: A python package for accessing APIs that require no key.
 Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
 Project-URL: Homepage, https://github.com/SpyderRex/nokey
 Project-URL: Issues, https://github.com/Spyder/nokey/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nokey-0.3.1/nokey.egg-info/SOURCES.txt` & `nokey-0.3.2/nokey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

