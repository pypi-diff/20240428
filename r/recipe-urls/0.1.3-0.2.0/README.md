# Comparing `tmp/recipe_urls-0.1.3.tar.gz` & `tmp/recipe_urls-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recipe_urls-0.1.3.tar", last modified: Wed Apr 17 15:13:26 2024, max compression
+gzip compressed data, was "recipe_urls-0.2.0.tar", last modified: Sun Apr 28 20:53:24 2024, max compression
```

## Comparing `recipe_urls-0.1.3.tar` & `recipe_urls-0.2.0.tar`

### file list

```diff
@@ -1,238 +1,529 @@
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-17 15:13:26.402392 recipe_urls-0.1.3/
--rw-r--r--   0 mkayeterry   (501) staff       (20)     6148 2024-04-16 16:01:33.000000 recipe_urls-0.1.3/.DS_Store
--rw-r--r--   0 mkayeterry   (501) staff       (20)       37 2024-04-17 15:07:53.000000 recipe_urls-0.1.3/.gitignore
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1069 2024-04-01 22:10:57.000000 recipe_urls-0.1.3/LICENSE
--rw-r--r--   0 mkayeterry   (501) staff       (20)     4521 2024-04-17 15:13:26.401440 recipe_urls-0.1.3/PKG-INFO
--rw-r--r--   0 mkayeterry   (501) staff       (20)     3576 2024-04-16 22:07:26.000000 recipe_urls-0.1.3/README.md
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-17 15:13:26.299889 recipe_urls-0.1.3/dist/
--rw-r--r--   0 mkayeterry   (501) staff       (20)   231969 2024-04-16 22:09:50.000000 recipe_urls-0.1.3/dist/recipe_urls-0.1.2-py3-none-any.whl
--rw-r--r--   0 mkayeterry   (501) staff       (20)   572775 2024-04-16 22:09:47.000000 recipe_urls-0.1.3/dist/recipe_urls-0.1.2.tar.gz
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1073 2024-04-17 15:13:11.000000 recipe_urls-0.1.3/pyproject.toml
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-17 15:13:26.349376 recipe_urls-0.1.3/recipe_urls/
--rw-r--r--   0 mkayeterry   (501) staff       (20)     6148 2024-04-16 16:01:38.000000 recipe_urls-0.1.3/recipe_urls/.DS_Store
--rw-r--r--   0 mkayeterry   (501) staff       (20)    11850 2024-04-17 15:12:42.000000 recipe_urls-0.1.3/recipe_urls/__init__.py
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-17 15:13:26.397751 recipe_urls-0.1.3/recipe_urls/__pycache__/
--rw-r--r--   0 mkayeterry   (501) staff       (20)     8975 2024-04-17 13:08:51.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1640 2024-04-17 13:08:51.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/_abstract.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2741 2024-04-16 20:46:05.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/_utils.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2003 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/abuelascounter.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2136 2024-04-17 13:19:10.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/acouplecooks.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1682 2024-04-17 13:20:27.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/addapinch.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1782 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/afghankitchenrecipes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1704 2024-04-17 13:46:30.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/allrecipes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2253 2024-04-17 13:29:10.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/ambitiouskitchen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2165 2024-04-17 13:45:16.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/archanaskitchen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1982 2024-04-17 13:29:10.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/averiecooks.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1988 2024-04-17 13:31:08.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/bakingmischief.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1987 2024-04-17 13:34:11.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/bakingsense.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1744 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/barefootcontessa.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1584 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/base_scraper.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1658 2024-04-17 13:37:40.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/bbc.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2008 2024-04-17 14:53:34.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/bettycrocker.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1919 2024-04-17 14:01:00.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/bigoven.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1710 2024-04-17 13:38:44.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/bluejeanchef.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1704 2024-04-17 13:41:52.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/bonappetit.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1682 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/bongeats.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2028 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/bowlofdelicious.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2005 2024-04-17 13:50:36.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/budgetbytes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2010 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/carlsbadcravings.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1984 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/castironketo.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1708 2024-04-17 13:48:38.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/cdkitchen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1971 2024-04-17 13:51:29.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/chefsavvy.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1993 2024-04-17 13:51:57.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/closetcooking.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1967 2024-04-17 13:54:24.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/cookieandkate.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1721 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/cookpad.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1901 2024-04-17 13:56:13.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/copykat.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1751 2024-04-17 13:59:54.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/countryliving.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1993 2024-04-17 14:01:48.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/creativecanning.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2002 2024-04-17 14:03:55.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/davidlebovitz.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1696 2024-04-17 14:05:11.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/delish.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2029 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/domesticateme.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1971 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/downshiftology.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2035 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/eatingbirdfood.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2135 2024-04-17 14:13:57.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/eatingwell.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2102 2024-04-17 14:14:59.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/eatliverun.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2081 2024-04-17 14:17:03.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/eatsmarter.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1693 2024-04-17 14:18:56.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/eatwell101.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1976 2024-04-17 14:20:41.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/eatwhattonight.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1979 2024-04-17 14:22:23.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/elavegan.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1715 2024-04-17 14:22:51.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/epicurious.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2066 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/errenskitchen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2035 2024-04-17 14:25:14.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/ethanchlebowski.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2086 2024-04-17 14:28:24.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/farmhouseonboone.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1732 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/fifteenspatulas.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1758 2024-04-17 14:30:15.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/finedininglovers.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1933 2024-04-17 14:33:32.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/fitmencook.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2027 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/fitslowcookerqueen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1648 2024-04-17 14:34:37.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/food.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1669 2024-04-17 14:35:52.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/food52.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2011 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/foodandwine.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1732 2024-04-17 14:39:08.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/foodnetwork.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1726 2024-04-17 14:39:23.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/foodrepublic.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2008 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/forksoverknives.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1998 2024-04-17 14:40:43.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/forktospoon.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2008 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/gimmesomeoven.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2015 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/gonnawantseconds.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2062 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/goodfooddiscoveries.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2043 2024-04-17 14:54:15.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/goodhousekeeping.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1762 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/greatbritishchefs.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1693 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/grimgrains.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2089 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/halfbakedharvest.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1989 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/handletheheat.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2096 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/headbangerskitchen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1738 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/heatherchristo.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1651 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/heb.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1702 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/hellofresh.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1750 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/hersheyland.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1952 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/hostthetoast.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1913 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/imworthy.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2048 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/indianhealthyrecipes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2038 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/insanelygoodrecipes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2016 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/inspiralized.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1980 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/izzycooking.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1731 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/jamieoliver.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2010 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/jimcooksfoodgood.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2027 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/joyfoodsunshine.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1700 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/justataste.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1948 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/justbento.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2131 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/justonecookbook.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1767 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/kingarthurbaking.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2054 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/leanandgreenrecipes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2053 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/lifestyleofafoodie.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2012 2024-04-04 16:22:13.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/littlespicejar.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2057 2024-04-04 16:40:16.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/livelytable.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2010 2024-04-04 19:29:31.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/lovingitvegan.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1737 2024-04-01 22:06:07.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/ninjatestkitchen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1690 2024-04-17 14:57:42.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/nytimes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1982 2024-04-04 19:32:04.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/ohsheglows.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1727 2024-04-12 20:09:17.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/onceuponachef.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2056 2024-04-12 20:18:36.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/paleorunningmomma.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2028 2024-04-12 20:32:55.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/persnicketyplates.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1712 2024-04-16 14:21:04.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/pickuplimes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1921 2024-04-12 20:33:23.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/pinchofyum.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1985 2024-04-16 14:22:53.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/platingpixels.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2046 2024-04-16 14:37:50.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/rachlmansfield.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2122 2024-04-16 14:47:26.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/rainbowplantlife.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2009 2024-04-16 14:58:24.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/reciperunner.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2129 2024-04-16 15:05:11.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/sallysbakingaddiction.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2019 2024-04-16 15:11:06.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/simpleveganista.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1942 2024-04-16 15:16:27.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/simplyquinoa.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2024 2024-04-16 15:28:00.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/simplywhisked.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2012 2024-04-16 15:32:14.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/southernliving.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1974 2024-04-16 15:48:41.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/tasteofhome.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1649 2024-04-16 15:50:33.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/tasty.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)      919 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1654 2024-04-16 15:55:58.000000 recipe_urls-0.1.3/recipe_urls/__pycache__/yummly.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1298 2024-04-16 21:18:48.000000 recipe_urls-0.1.3/recipe_urls/_abstract.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     3849 2024-04-16 20:45:56.000000 recipe_urls-0.1.3/recipe_urls/_utils.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1421 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/abuelascounter.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1830 2024-04-17 13:18:54.000000 recipe_urls-0.1.3/recipe_urls/acouplecooks.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1154 2024-04-17 13:20:22.000000 recipe_urls-0.1.3/recipe_urls/addapinch.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1199 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/afghankitchenrecipes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1171 2024-04-17 13:46:22.000000 recipe_urls-0.1.3/recipe_urls/allrecipes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1971 2024-04-17 13:23:38.000000 recipe_urls-0.1.3/recipe_urls/ambitiouskitchen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1805 2024-04-17 13:45:08.000000 recipe_urls-0.1.3/recipe_urls/archanaskitchen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1392 2024-04-17 13:27:39.000000 recipe_urls-0.1.3/recipe_urls/averiecooks.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1371 2024-04-17 13:31:04.000000 recipe_urls-0.1.3/recipe_urls/bakingmischief.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1405 2024-04-17 13:34:03.000000 recipe_urls-0.1.3/recipe_urls/bakingsense.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1180 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/barefootcontessa.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1156 2024-04-17 13:37:34.000000 recipe_urls-0.1.3/recipe_urls/bbc.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1418 2024-04-17 14:53:26.000000 recipe_urls-0.1.3/recipe_urls/bettycrocker.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1330 2024-04-17 14:00:17.000000 recipe_urls-0.1.3/recipe_urls/bigoven.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1166 2024-04-17 13:38:38.000000 recipe_urls-0.1.3/recipe_urls/bluejeanchef.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1167 2024-04-17 13:41:47.000000 recipe_urls-0.1.3/recipe_urls/bonappetit.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1155 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/bongeats.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1450 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/bowlofdelicious.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1498 2024-04-17 13:50:32.000000 recipe_urls-0.1.3/recipe_urls/budgetbytes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1404 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/carlsbadcravings.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1409 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/castironketo.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1180 2024-04-17 13:48:32.000000 recipe_urls-0.1.3/recipe_urls/cdkitchen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1461 2024-04-17 13:51:25.000000 recipe_urls-0.1.3/recipe_urls/chefsavvy.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1414 2024-04-17 13:51:43.000000 recipe_urls-0.1.3/recipe_urls/closetcooking.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1350 2024-04-17 13:54:21.000000 recipe_urls-0.1.3/recipe_urls/cookieandkate.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1315 2024-04-17 13:56:08.000000 recipe_urls-0.1.3/recipe_urls/copykat.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1199 2024-04-17 13:59:24.000000 recipe_urls-0.1.3/recipe_urls/countryliving.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1387 2024-04-17 14:01:25.000000 recipe_urls-0.1.3/recipe_urls/creativecanning.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1438 2024-04-17 14:03:23.000000 recipe_urls-0.1.3/recipe_urls/davidlebovitz.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1179 2024-04-17 14:05:05.000000 recipe_urls-0.1.3/recipe_urls/delish.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1526 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/domesticateme.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1343 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/downshiftology.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1525 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/eatingbirdfood.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1887 2024-04-17 14:13:45.000000 recipe_urls-0.1.3/recipe_urls/eatingwell.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1766 2024-04-17 14:14:52.000000 recipe_urls-0.1.3/recipe_urls/eatliverun.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1617 2024-04-17 14:16:32.000000 recipe_urls-0.1.3/recipe_urls/eatsmarter.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1159 2024-04-17 14:17:26.000000 recipe_urls-0.1.3/recipe_urls/eatwell101.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1348 2024-04-17 14:20:36.000000 recipe_urls-0.1.3/recipe_urls/eatwhattonight.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1520 2024-04-17 14:21:59.000000 recipe_urls-0.1.3/recipe_urls/elavegan.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1178 2024-04-17 14:22:46.000000 recipe_urls-0.1.3/recipe_urls/epicurious.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1593 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/errenskitchen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1426 2024-04-17 14:25:09.000000 recipe_urls-0.1.3/recipe_urls/ethanchlebowski.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1624 2024-04-17 14:28:19.000000 recipe_urls-0.1.3/recipe_urls/farmhouseonboone.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1174 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/fifteenspatulas.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1191 2024-04-17 14:30:10.000000 recipe_urls-0.1.3/recipe_urls/finedininglovers.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1330 2024-04-17 14:33:26.000000 recipe_urls-0.1.3/recipe_urls/fitmencook.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1418 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/fitslowcookerqueen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1148 2024-04-17 14:34:29.000000 recipe_urls-0.1.3/recipe_urls/food.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1152 2024-04-17 14:35:44.000000 recipe_urls-0.1.3/recipe_urls/food52.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1424 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/foodandwine.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1193 2024-04-17 14:37:52.000000 recipe_urls-0.1.3/recipe_urls/foodnetwork.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1179 2024-04-17 14:39:19.000000 recipe_urls-0.1.3/recipe_urls/foodrepublic.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1371 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/forksoverknives.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1491 2024-04-17 14:40:36.000000 recipe_urls-0.1.3/recipe_urls/forktospoon.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1445 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/gimmesomeoven.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1405 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/gonnawantseconds.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1463 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/goodfooddiscoveries.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1401 2024-04-17 14:54:02.000000 recipe_urls-0.1.3/recipe_urls/goodhousekeeping.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1193 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/greatbritishchefs.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1568 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/halfbakedharvest.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1426 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/handletheheat.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1528 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/headbangerskitchen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1184 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/heatherchristo.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1168 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/hellofresh.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1203 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/hersheyland.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1337 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/hostthetoast.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1322 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/imworthy.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1396 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/indianhealthyrecipes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1414 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/insanelygoodrecipes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1490 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/inspiralized.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1429 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/izzycooking.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1189 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/jamieoliver.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1399 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/jimcooksfoodgood.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1452 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/joyfoodsunshine.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1166 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/justataste.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1348 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/justbento.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1721 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/justonecookbook.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1200 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/kingarthurbaking.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1405 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/leanandgreenrecipes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1475 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/lifestyleofafoodie.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1473 2024-04-04 16:22:06.000000 recipe_urls-0.1.3/recipe_urls/littlespicejar.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1640 2024-04-04 16:40:12.000000 recipe_urls-0.1.3/recipe_urls/livelytable.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1492 2024-04-04 19:16:48.000000 recipe_urls-0.1.3/recipe_urls/lovingitvegan.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1173 2024-04-01 22:04:35.000000 recipe_urls-0.1.3/recipe_urls/ninjatestkitchen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1168 2024-04-17 14:57:30.000000 recipe_urls-0.1.3/recipe_urls/nytimes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1500 2024-04-04 19:31:59.000000 recipe_urls-0.1.3/recipe_urls/ohsheglows.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1178 2024-04-04 19:36:45.000000 recipe_urls-0.1.3/recipe_urls/onceuponachef.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1484 2024-04-12 20:18:31.000000 recipe_urls-0.1.3/recipe_urls/paleorunningmomma.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1394 2024-04-12 20:24:05.000000 recipe_urls-0.1.3/recipe_urls/persnicketyplates.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1170 2024-04-16 14:17:37.000000 recipe_urls-0.1.3/recipe_urls/pickuplimes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1392 2024-04-16 14:22:48.000000 recipe_urls-0.1.3/recipe_urls/platingpixels.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1536 2024-04-16 14:34:49.000000 recipe_urls-0.1.3/recipe_urls/rachlmansfield.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1675 2024-04-16 14:47:20.000000 recipe_urls-0.1.3/recipe_urls/rainbowplantlife.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1481 2024-04-16 14:54:23.000000 recipe_urls-0.1.3/recipe_urls/reciperunner.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1622 2024-04-16 15:05:05.000000 recipe_urls-0.1.3/recipe_urls/sallysbakingaddiction.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1443 2024-04-16 15:11:01.000000 recipe_urls-0.1.3/recipe_urls/simpleveganista.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1475 2024-04-16 15:23:57.000000 recipe_urls-0.1.3/recipe_urls/simplywhisked.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1375 2024-04-16 15:36:30.000000 recipe_urls-0.1.3/recipe_urls/tasteofhome.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1137 2024-04-16 15:50:26.000000 recipe_urls-0.1.3/recipe_urls/tasty.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     5630 2024-04-17 15:01:23.000000 recipe_urls-0.1.3/recipe_urls/testing.py
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-17 15:13:26.400142 recipe_urls-0.1.3/recipe_urls.egg-info/
--rw-r--r--   0 mkayeterry   (501) staff       (20)     4521 2024-04-17 15:13:26.000000 recipe_urls-0.1.3/recipe_urls.egg-info/PKG-INFO
--rw-r--r--   0 mkayeterry   (501) staff       (20)     9270 2024-04-17 15:13:26.000000 recipe_urls-0.1.3/recipe_urls.egg-info/SOURCES.txt
--rw-r--r--   0 mkayeterry   (501) staff       (20)        1 2024-04-17 15:13:26.000000 recipe_urls-0.1.3/recipe_urls.egg-info/dependency_links.txt
--rw-r--r--   0 mkayeterry   (501) staff       (20)       75 2024-04-17 15:13:26.000000 recipe_urls-0.1.3/recipe_urls.egg-info/requires.txt
--rw-r--r--   0 mkayeterry   (501) staff       (20)       12 2024-04-17 15:13:26.000000 recipe_urls-0.1.3/recipe_urls.egg-info/top_level.txt
--rw-r--r--   0 mkayeterry   (501) staff       (20)       38 2024-04-17 15:13:26.402494 recipe_urls-0.1.3/setup.cfg
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-17 15:13:26.398253 recipe_urls-0.1.3/tests/
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-17 15:13:26.399382 recipe_urls-0.1.3/tests/__pycache__/
--rw-r--r--   0 mkayeterry   (501) staff       (20)    25473 2024-04-16 20:23:46.000000 recipe_urls-0.1.3/tests/__pycache__/test_get_site_origin.cpython-310-pytest-8.1.1.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)    33786 2024-04-16 20:23:36.000000 recipe_urls-0.1.3/tests/test_get_site_origin.py
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.403540 recipe_urls-0.2.0/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     6148 2024-04-16 16:01:33.000000 recipe_urls-0.2.0/.DS_Store
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     3113 2024-04-18 00:44:07.000000 recipe_urls-0.2.0/.gitignore
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1069 2024-04-01 22:10:57.000000 recipe_urls-0.2.0/LICENSE
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     5185 2024-04-28 20:53:24.403135 recipe_urls-0.2.0/PKG-INFO
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     4237 2024-04-26 17:06:00.000000 recipe_urls-0.2.0/README.md
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1076 2024-04-25 20:15:13.000000 recipe_urls-0.2.0/pyproject.toml
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.065211 recipe_urls-0.2.0/recipe_urls/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     6148 2024-04-16 16:01:38.000000 recipe_urls-0.2.0/recipe_urls/.DS_Store
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    12709 2024-04-28 17:26:22.000000 recipe_urls-0.2.0/recipe_urls/__init__.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2368 2024-04-28 17:20:04.000000 recipe_urls-0.2.0/recipe_urls/_abstract.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     6722 2024-04-28 17:26:37.000000 recipe_urls-0.2.0/recipe_urls/_utils.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      391 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/abuelascounter.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      849 2024-04-25 17:15:06.000000 recipe_urls-0.2.0/recipe_urls/acouplecooks.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      248 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/addapinch.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      302 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/afghankitchenrecipes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      282 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/allrecipes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      994 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/ambitiouskitchen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      811 2024-04-25 18:15:52.000000 recipe_urls-0.2.0/recipe_urls/archanaskitchen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      549 2024-04-25 18:58:58.000000 recipe_urls-0.2.0/recipe_urls/averiecooks.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      348 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/bakingmischief.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      400 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/bakingsense.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      272 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/barefootcontessa.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      235 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/bbc.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      419 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/bettycrocker.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      344 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/bigoven.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      262 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/bluejeanchef.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      234 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/bonappetit.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      226 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/bongeats.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      482 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/bowlofdelicious.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      553 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/budgetbytes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      452 2024-04-28 20:26:53.000000 recipe_urls-0.2.0/recipe_urls/carlsbadcravings.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      472 2024-04-25 18:56:10.000000 recipe_urls-0.2.0/recipe_urls/castironketo.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      286 2024-04-25 16:40:01.000000 recipe_urls-0.2.0/recipe_urls/cdkitchen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      497 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/chefsavvy.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      471 2024-04-25 18:56:32.000000 recipe_urls-0.2.0/recipe_urls/closetcooking.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      397 2024-04-25 18:56:39.000000 recipe_urls-0.2.0/recipe_urls/cookieandkate.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      357 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/copykat.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      260 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/countryliving.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      419 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/creativecanning.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      470 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/davidlebovitz.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      458 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/delish.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      684 2024-04-25 19:03:18.000000 recipe_urls-0.2.0/recipe_urls/domesticateme.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      378 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/downshiftology.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      552 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/eatingbirdfood.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1089 2024-04-25 19:11:32.000000 recipe_urls-0.2.0/recipe_urls/eatingwell.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      787 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/eatliverun.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      624 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/eatsmarter.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      257 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/eatwell101.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      383 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/eatwhattonight.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      552 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/elavegan.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      245 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/epicurious.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      618 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/errenskitchen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      353 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/ethanchlebowski.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      645 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/farmhouseonboone.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      559 2024-04-28 17:20:04.000000 recipe_urls-0.2.0/recipe_urls/fifteenspatulas.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      246 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/finedininglovers.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      368 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/fitmencook.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      379 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/fitslowcookerqueen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      248 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/food.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      227 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/food52.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      689 2024-04-26 15:43:15.000000 recipe_urls-0.2.0/recipe_urls/foodandwine.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      605 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/foodnetwork.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      242 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/foodrepublic.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      324 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/forksoverknives.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      578 2024-04-28 17:20:04.000000 recipe_urls-0.2.0/recipe_urls/forktospoon.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      405 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/gimmesomeoven.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      379 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/gonnawantseconds.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      417 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/goodfooddiscoveries.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      396 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/goodhousekeeping.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      298 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/greatbritishchefs.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      598 2024-04-25 19:33:28.000000 recipe_urls-0.2.0/recipe_urls/halfbakedharvest.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      386 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/handletheheat.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      522 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/headbangerskitchen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      593 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/heatherchristo.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      266 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/hellofresh.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      303 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/hersheyland.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      394 2024-04-25 19:36:32.000000 recipe_urls-0.2.0/recipe_urls/hostthetoast.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      362 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/imworthy.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      380 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/indianhealthyrecipes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      384 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/insanelygoodrecipes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      519 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/inspiralized.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      391 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/izzycooking.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      254 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/jamieoliver.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      429 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/jimcooksfoodgood.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      481 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/joyfoodsunshine.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      264 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/justataste.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      361 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/justbento.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      739 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/justonecookbook.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      255 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/kingarthurbaking.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      397 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/leanandgreenrecipes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      500 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/lifestyleofafoodie.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      501 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/littlespicejar.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      665 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/livelytable.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      520 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/lovingitvegan.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      265 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/ninjatestkitchen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      237 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/nytimes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      530 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/ohsheglows.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      287 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/onceuponachef.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      510 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/paleorunningmomma.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      367 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/persnicketyplates.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      235 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/pickuplimes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      425 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/platingpixels.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      577 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/rachlmansfield.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      709 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/rainbowplantlife.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      512 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/reciperunner.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      639 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/sallysbakingaddiction.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      399 2024-04-25 19:44:31.000000 recipe_urls-0.2.0/recipe_urls/simpleveganista.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      520 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/simplywhisked.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      412 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/tasteofhome.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      219 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/tasty.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    16605 2024-04-28 20:46:35.000000 recipe_urls-0.2.0/recipe_urls/testing.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      607 2024-04-21 13:34:16.000000 recipe_urls-0.2.0/recipe_urls/wellplated.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      341 2024-04-25 15:29:00.000000 recipe_urls-0.2.0/recipe_urls/whole30.py
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.402040 recipe_urls-0.2.0/recipe_urls.egg-info/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     5185 2024-04-28 20:53:23.000000 recipe_urls-0.2.0/recipe_urls.egg-info/PKG-INFO
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    20078 2024-04-28 20:53:24.000000 recipe_urls-0.2.0/recipe_urls.egg-info/SOURCES.txt
+-rw-r--r--   0 mkayeterry   (501) staff       (20)        1 2024-04-28 20:53:23.000000 recipe_urls-0.2.0/recipe_urls.egg-info/dependency_links.txt
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       78 2024-04-28 20:53:23.000000 recipe_urls-0.2.0/recipe_urls.egg-info/requires.txt
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       12 2024-04-28 20:53:23.000000 recipe_urls-0.2.0/recipe_urls.egg-info/top_level.txt
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       38 2024-04-28 20:53:24.403633 recipe_urls-0.2.0/setup.cfg
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.067942 recipe_urls-0.2.0/tests/
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.068293 recipe_urls-0.2.0/tests/__pycache__/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2933 2024-04-19 16:03:18.000000 recipe_urls-0.2.0/tests/__pycache__/test_get_site_origin.cpython-310-pytest-8.1.1.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2924 2024-04-28 17:20:04.000000 recipe_urls-0.2.0/tests/test_concat_host.py
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.023952 recipe_urls-0.2.0/tests/test_data/
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.070767 recipe_urls-0.2.0/tests/test_data/abuelascounter/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   110661 2024-04-28 20:44:58.000000 recipe_urls-0.2.0/tests/test_data/abuelascounter/abuelascounter.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:44:58.000000 recipe_urls-0.2.0/tests/test_data/abuelascounter/abuelascounter_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      883 2024-04-28 20:44:58.000000 recipe_urls-0.2.0/tests/test_data/abuelascounter/abuelascounter_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.073768 recipe_urls-0.2.0/tests/test_data/acouplecooks/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   469522 2024-04-28 20:45:01.000000 recipe_urls-0.2.0/tests/test_data/acouplecooks/acouplecooks.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       30 2024-04-28 20:45:01.000000 recipe_urls-0.2.0/tests/test_data/acouplecooks/acouplecooks_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     3119 2024-04-28 20:45:01.000000 recipe_urls-0.2.0/tests/test_data/acouplecooks/acouplecooks_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.076929 recipe_urls-0.2.0/tests/test_data/addapinch/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   393603 2024-04-28 20:45:02.000000 recipe_urls-0.2.0/tests/test_data/addapinch/addapinch.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       23 2024-04-28 20:45:02.000000 recipe_urls-0.2.0/tests/test_data/addapinch/addapinch_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1214 2024-04-28 20:45:02.000000 recipe_urls-0.2.0/tests/test_data/addapinch/addapinch_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.079002 recipe_urls-0.2.0/tests/test_data/afghankitchenrecipes/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    58446 2024-04-28 20:45:04.000000 recipe_urls-0.2.0/tests/test_data/afghankitchenrecipes/afghankitchenrecipes.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       37 2024-04-28 20:45:04.000000 recipe_urls-0.2.0/tests/test_data/afghankitchenrecipes/afghankitchenrecipes_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1582 2024-04-28 20:45:04.000000 recipe_urls-0.2.0/tests/test_data/afghankitchenrecipes/afghankitchenrecipes_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.081839 recipe_urls-0.2.0/tests/test_data/allrecipes/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   280232 2024-04-28 20:45:05.000000 recipe_urls-0.2.0/tests/test_data/allrecipes/allrecipes.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:45:05.000000 recipe_urls-0.2.0/tests/test_data/allrecipes/allrecipes_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1086 2024-04-28 20:45:05.000000 recipe_urls-0.2.0/tests/test_data/allrecipes/allrecipes_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.085589 recipe_urls-0.2.0/tests/test_data/ambitiouskitchen/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   538360 2024-04-28 20:45:06.000000 recipe_urls-0.2.0/tests/test_data/ambitiouskitchen/ambitiouskitchen.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       34 2024-04-28 20:45:06.000000 recipe_urls-0.2.0/tests/test_data/ambitiouskitchen/ambitiouskitchen_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2915 2024-04-28 20:45:06.000000 recipe_urls-0.2.0/tests/test_data/ambitiouskitchen/ambitiouskitchen_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.088429 recipe_urls-0.2.0/tests/test_data/archanaskitchen/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    59542 2024-04-28 20:45:07.000000 recipe_urls-0.2.0/tests/test_data/archanaskitchen/archanaskitchen.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       33 2024-04-28 20:45:07.000000 recipe_urls-0.2.0/tests/test_data/archanaskitchen/archanaskitchen_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2423 2024-04-28 20:45:07.000000 recipe_urls-0.2.0/tests/test_data/archanaskitchen/archanaskitchen_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.091355 recipe_urls-0.2.0/tests/test_data/averiecooks/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   539838 2024-04-28 20:45:07.000000 recipe_urls-0.2.0/tests/test_data/averiecooks/averiecooks.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       29 2024-04-28 20:45:07.000000 recipe_urls-0.2.0/tests/test_data/averiecooks/averiecooks_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     3342 2024-04-28 20:45:07.000000 recipe_urls-0.2.0/tests/test_data/averiecooks/averiecooks_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.093247 recipe_urls-0.2.0/tests/test_data/baking-sense/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   237477 2024-04-28 20:45:08.000000 recipe_urls-0.2.0/tests/test_data/baking-sense/baking-sense.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       30 2024-04-28 20:45:08.000000 recipe_urls-0.2.0/tests/test_data/baking-sense/baking-sense_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      584 2024-04-28 20:45:08.000000 recipe_urls-0.2.0/tests/test_data/baking-sense/baking-sense_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.096288 recipe_urls-0.2.0/tests/test_data/bakingmischief/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   356956 2024-04-28 20:45:08.000000 recipe_urls-0.2.0/tests/test_data/bakingmischief/bakingmischief.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:45:08.000000 recipe_urls-0.2.0/tests/test_data/bakingmischief/bakingmischief_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1099 2024-04-28 20:45:08.000000 recipe_urls-0.2.0/tests/test_data/bakingmischief/bakingmischief_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.099006 recipe_urls-0.2.0/tests/test_data/barefootcontessa/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   341371 2024-04-28 20:45:09.000000 recipe_urls-0.2.0/tests/test_data/barefootcontessa/barefootcontessa.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       30 2024-04-28 20:45:09.000000 recipe_urls-0.2.0/tests/test_data/barefootcontessa/barefootcontessa_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1386 2024-04-28 20:45:09.000000 recipe_urls-0.2.0/tests/test_data/barefootcontessa/barefootcontessa_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.102058 recipe_urls-0.2.0/tests/test_data/bbc/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   189010 2024-04-28 20:45:09.000000 recipe_urls-0.2.0/tests/test_data/bbc/bbc.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:45:09.000000 recipe_urls-0.2.0/tests/test_data/bbc/bbc_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      309 2024-04-28 20:45:09.000000 recipe_urls-0.2.0/tests/test_data/bbc/bbc_exp_output.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)        0 2024-04-21 13:25:03.000000 recipe_urls-0.2.0/tests/test_data/bbc/co.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   165923 2024-04-21 13:25:03.000000 recipe_urls-0.2.0/tests/test_data/bbc/co.testhtml
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.105604 recipe_urls-0.2.0/tests/test_data/bettycrocker/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   622041 2024-04-28 20:45:10.000000 recipe_urls-0.2.0/tests/test_data/bettycrocker/bettycrocker.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       30 2024-04-28 20:45:10.000000 recipe_urls-0.2.0/tests/test_data/bettycrocker/bettycrocker_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      709 2024-04-28 20:45:10.000000 recipe_urls-0.2.0/tests/test_data/bettycrocker/bettycrocker_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.107849 recipe_urls-0.2.0/tests/test_data/bigoven/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   108063 2024-04-28 20:45:10.000000 recipe_urls-0.2.0/tests/test_data/bigoven/bigoven.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       25 2024-04-28 20:45:10.000000 recipe_urls-0.2.0/tests/test_data/bigoven/bigoven_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      337 2024-04-28 20:45:10.000000 recipe_urls-0.2.0/tests/test_data/bigoven/bigoven_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.110117 recipe_urls-0.2.0/tests/test_data/bluejeanchef/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   146985 2024-04-28 20:45:11.000000 recipe_urls-0.2.0/tests/test_data/bluejeanchef/bluejeanchef.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       26 2024-04-28 20:45:11.000000 recipe_urls-0.2.0/tests/test_data/bluejeanchef/bluejeanchef_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      360 2024-04-28 20:45:11.000000 recipe_urls-0.2.0/tests/test_data/bluejeanchef/bluejeanchef_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.115124 recipe_urls-0.2.0/tests/test_data/bonappetit/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)  1917210 2024-04-28 20:45:11.000000 recipe_urls-0.2.0/tests/test_data/bonappetit/bonappetit.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:45:11.000000 recipe_urls-0.2.0/tests/test_data/bonappetit/bonappetit_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2318 2024-04-28 20:45:11.000000 recipe_urls-0.2.0/tests/test_data/bonappetit/bonappetit_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.117164 recipe_urls-0.2.0/tests/test_data/bongeats/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    69783 2024-04-28 20:45:12.000000 recipe_urls-0.2.0/tests/test_data/bongeats/bongeats.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       26 2024-04-28 20:45:12.000000 recipe_urls-0.2.0/tests/test_data/bongeats/bongeats_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      571 2024-04-28 20:45:12.000000 recipe_urls-0.2.0/tests/test_data/bongeats/bongeats_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.119517 recipe_urls-0.2.0/tests/test_data/bowlofdelicious/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   241853 2024-04-28 20:45:12.000000 recipe_urls-0.2.0/tests/test_data/bowlofdelicious/bowlofdelicious.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       33 2024-04-28 20:45:12.000000 recipe_urls-0.2.0/tests/test_data/bowlofdelicious/bowlofdelicious_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1033 2024-04-28 20:45:12.000000 recipe_urls-0.2.0/tests/test_data/bowlofdelicious/bowlofdelicious_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.122690 recipe_urls-0.2.0/tests/test_data/budgetbytes/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   426756 2024-04-28 20:45:12.000000 recipe_urls-0.2.0/tests/test_data/budgetbytes/budgetbytes.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       29 2024-04-28 20:45:12.000000 recipe_urls-0.2.0/tests/test_data/budgetbytes/budgetbytes_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2717 2024-04-28 20:45:12.000000 recipe_urls-0.2.0/tests/test_data/budgetbytes/budgetbytes_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.127429 recipe_urls-0.2.0/tests/test_data/carlsbadcravings/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   657276 2024-04-28 20:45:21.000000 recipe_urls-0.2.0/tests/test_data/carlsbadcravings/carlsbadcravings.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       30 2024-04-28 20:45:21.000000 recipe_urls-0.2.0/tests/test_data/carlsbadcravings/carlsbadcravings_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     8043 2024-04-28 20:45:21.000000 recipe_urls-0.2.0/tests/test_data/carlsbadcravings/carlsbadcravings_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.133849 recipe_urls-0.2.0/tests/test_data/castironketo/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   429550 2024-04-28 20:45:22.000000 recipe_urls-0.2.0/tests/test_data/castironketo/castironketo.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       30 2024-04-28 20:45:22.000000 recipe_urls-0.2.0/tests/test_data/castironketo/castironketo_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2135 2024-04-28 20:45:22.000000 recipe_urls-0.2.0/tests/test_data/castironketo/castironketo_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.139479 recipe_urls-0.2.0/tests/test_data/cdkitchen/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    49423 2024-04-28 20:45:24.000000 recipe_urls-0.2.0/tests/test_data/cdkitchen/cdkitchen.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       27 2024-04-28 20:45:24.000000 recipe_urls-0.2.0/tests/test_data/cdkitchen/cdkitchen_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      617 2024-04-28 20:45:24.000000 recipe_urls-0.2.0/tests/test_data/cdkitchen/cdkitchen_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.145465 recipe_urls-0.2.0/tests/test_data/chefsavvy/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   433712 2024-04-28 20:45:25.000000 recipe_urls-0.2.0/tests/test_data/chefsavvy/chefsavvy.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       23 2024-04-28 20:45:25.000000 recipe_urls-0.2.0/tests/test_data/chefsavvy/chefsavvy_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      882 2024-04-28 20:45:25.000000 recipe_urls-0.2.0/tests/test_data/chefsavvy/chefsavvy_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.148249 recipe_urls-0.2.0/tests/test_data/closetcooking/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   117248 2024-04-28 20:45:25.000000 recipe_urls-0.2.0/tests/test_data/closetcooking/closetcooking.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       31 2024-04-28 20:45:25.000000 recipe_urls-0.2.0/tests/test_data/closetcooking/closetcooking_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      818 2024-04-28 20:45:25.000000 recipe_urls-0.2.0/tests/test_data/closetcooking/closetcooking_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.153218 recipe_urls-0.2.0/tests/test_data/cookieandkate/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   234463 2024-04-28 20:45:26.000000 recipe_urls-0.2.0/tests/test_data/cookieandkate/cookieandkate.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       27 2024-04-28 20:45:26.000000 recipe_urls-0.2.0/tests/test_data/cookieandkate/cookieandkate_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      861 2024-04-28 20:45:26.000000 recipe_urls-0.2.0/tests/test_data/cookieandkate/cookieandkate_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.156307 recipe_urls-0.2.0/tests/test_data/copykat/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   248824 2024-04-28 20:45:26.000000 recipe_urls-0.2.0/tests/test_data/copykat/copykat.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       21 2024-04-28 20:45:26.000000 recipe_urls-0.2.0/tests/test_data/copykat/copykat_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      340 2024-04-28 20:45:26.000000 recipe_urls-0.2.0/tests/test_data/copykat/copykat_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.159721 recipe_urls-0.2.0/tests/test_data/countryliving/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   332758 2024-04-28 20:45:26.000000 recipe_urls-0.2.0/tests/test_data/countryliving/countryliving.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       44 2024-04-28 20:45:26.000000 recipe_urls-0.2.0/tests/test_data/countryliving/countryliving_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1554 2024-04-28 20:45:26.000000 recipe_urls-0.2.0/tests/test_data/countryliving/countryliving_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.161868 recipe_urls-0.2.0/tests/test_data/creativecanning/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    51418 2024-04-28 20:45:27.000000 recipe_urls-0.2.0/tests/test_data/creativecanning/creativecanning.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       29 2024-04-28 20:45:27.000000 recipe_urls-0.2.0/tests/test_data/creativecanning/creativecanning_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      289 2024-04-28 20:45:27.000000 recipe_urls-0.2.0/tests/test_data/creativecanning/creativecanning_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.164200 recipe_urls-0.2.0/tests/test_data/davidlebovitz/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   239019 2024-04-28 20:45:27.000000 recipe_urls-0.2.0/tests/test_data/davidlebovitz/davidlebovitz.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       37 2024-04-28 20:45:27.000000 recipe_urls-0.2.0/tests/test_data/davidlebovitz/davidlebovitz_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      752 2024-04-28 20:45:27.000000 recipe_urls-0.2.0/tests/test_data/davidlebovitz/davidlebovitz_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.167738 recipe_urls-0.2.0/tests/test_data/delish/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   530172 2024-04-28 20:45:27.000000 recipe_urls-0.2.0/tests/test_data/delish/delish.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       46 2024-04-28 20:45:27.000000 recipe_urls-0.2.0/tests/test_data/delish/delish_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     5584 2024-04-28 20:45:27.000000 recipe_urls-0.2.0/tests/test_data/delish/delish_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.169746 recipe_urls-0.2.0/tests/test_data/domesticate-me/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   149757 2024-04-28 20:45:28.000000 recipe_urls-0.2.0/tests/test_data/domesticate-me/domesticate-me.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       46 2024-04-28 20:45:28.000000 recipe_urls-0.2.0/tests/test_data/domesticate-me/domesticate-me_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1171 2024-04-28 20:45:28.000000 recipe_urls-0.2.0/tests/test_data/domesticate-me/domesticate-me_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.174773 recipe_urls-0.2.0/tests/test_data/downshiftology/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   478372 2024-04-28 20:45:28.000000 recipe_urls-0.2.0/tests/test_data/downshiftology/downshiftology.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:45:28.000000 recipe_urls-0.2.0/tests/test_data/downshiftology/downshiftology_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2340 2024-04-28 20:45:28.000000 recipe_urls-0.2.0/tests/test_data/downshiftology/downshiftology_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.178586 recipe_urls-0.2.0/tests/test_data/eatingbirdfood/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   692192 2024-04-28 20:45:30.000000 recipe_urls-0.2.0/tests/test_data/eatingbirdfood/eatingbirdfood.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       32 2024-04-28 20:45:30.000000 recipe_urls-0.2.0/tests/test_data/eatingbirdfood/eatingbirdfood_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     3186 2024-04-28 20:45:30.000000 recipe_urls-0.2.0/tests/test_data/eatingbirdfood/eatingbirdfood_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.184318 recipe_urls-0.2.0/tests/test_data/eatingwell/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   306027 2024-04-28 20:45:31.000000 recipe_urls-0.2.0/tests/test_data/eatingwell/eatingwell.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       37 2024-04-28 20:45:31.000000 recipe_urls-0.2.0/tests/test_data/eatingwell/eatingwell_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2338 2024-04-28 20:45:31.000000 recipe_urls-0.2.0/tests/test_data/eatingwell/eatingwell_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.186278 recipe_urls-0.2.0/tests/test_data/eatliverun/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   120912 2024-04-28 20:45:41.000000 recipe_urls-0.2.0/tests/test_data/eatliverun/eatliverun.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       37 2024-04-28 20:45:41.000000 recipe_urls-0.2.0/tests/test_data/eatliverun/eatliverun_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    25908 2024-04-28 20:45:41.000000 recipe_urls-0.2.0/tests/test_data/eatliverun/eatliverun_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.190613 recipe_urls-0.2.0/tests/test_data/eatsmarter/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   306971 2024-04-28 20:45:46.000000 recipe_urls-0.2.0/tests/test_data/eatsmarter/eatsmarter.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       24 2024-04-28 20:45:46.000000 recipe_urls-0.2.0/tests/test_data/eatsmarter/eatsmarter_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      143 2024-04-28 20:45:46.000000 recipe_urls-0.2.0/tests/test_data/eatsmarter/eatsmarter_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.193599 recipe_urls-0.2.0/tests/test_data/eatwell101/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   253600 2024-04-28 20:45:42.000000 recipe_urls-0.2.0/tests/test_data/eatwell101/eatwell101.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:45:42.000000 recipe_urls-0.2.0/tests/test_data/eatwell101/eatwell101_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1906 2024-04-28 20:45:42.000000 recipe_urls-0.2.0/tests/test_data/eatwell101/eatwell101_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.196409 recipe_urls-0.2.0/tests/test_data/eatwhattonight/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   446777 2024-04-28 20:45:49.000000 recipe_urls-0.2.0/tests/test_data/eatwhattonight/eatwhattonight.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:45:49.000000 recipe_urls-0.2.0/tests/test_data/eatwhattonight/eatwhattonight_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2092 2024-04-28 20:45:49.000000 recipe_urls-0.2.0/tests/test_data/eatwhattonight/eatwhattonight_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.198987 recipe_urls-0.2.0/tests/test_data/elavegan/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   186843 2024-04-28 20:45:49.000000 recipe_urls-0.2.0/tests/test_data/elavegan/elavegan.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       22 2024-04-28 20:45:49.000000 recipe_urls-0.2.0/tests/test_data/elavegan/elavegan_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1597 2024-04-28 20:45:49.000000 recipe_urls-0.2.0/tests/test_data/elavegan/elavegan_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.205476 recipe_urls-0.2.0/tests/test_data/epicurious/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)  3770172 2024-04-28 20:45:51.000000 recipe_urls-0.2.0/tests/test_data/epicurious/epicurious.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:45:51.000000 recipe_urls-0.2.0/tests/test_data/epicurious/epicurious_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     7729 2024-04-28 20:45:51.000000 recipe_urls-0.2.0/tests/test_data/epicurious/epicurious_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.208586 recipe_urls-0.2.0/tests/test_data/errenskitchen/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   263352 2024-04-28 20:45:51.000000 recipe_urls-0.2.0/tests/test_data/errenskitchen/errenskitchen.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       31 2024-04-28 20:45:51.000000 recipe_urls-0.2.0/tests/test_data/errenskitchen/errenskitchen_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1151 2024-04-28 20:45:51.000000 recipe_urls-0.2.0/tests/test_data/errenskitchen/errenskitchen_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.210356 recipe_urls-0.2.0/tests/test_data/ethanchlebowski/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    92950 2024-04-28 20:45:52.000000 recipe_urls-0.2.0/tests/test_data/ethanchlebowski/ethanchlebowski.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       60 2024-04-28 20:45:52.000000 recipe_urls-0.2.0/tests/test_data/ethanchlebowski/ethanchlebowski_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1595 2024-04-28 20:45:52.000000 recipe_urls-0.2.0/tests/test_data/ethanchlebowski/ethanchlebowski_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.213310 recipe_urls-0.2.0/tests/test_data/farmhouseonboone/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   426017 2024-04-28 20:45:52.000000 recipe_urls-0.2.0/tests/test_data/farmhouseonboone/farmhouseonboone.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       34 2024-04-28 20:45:52.000000 recipe_urls-0.2.0/tests/test_data/farmhouseonboone/farmhouseonboone_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1363 2024-04-28 20:45:52.000000 recipe_urls-0.2.0/tests/test_data/farmhouseonboone/farmhouseonboone_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.215757 recipe_urls-0.2.0/tests/test_data/fifteenspatulas/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   156688 2024-04-28 20:45:52.000000 recipe_urls-0.2.0/tests/test_data/fifteenspatulas/fifteenspatulas.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       33 2024-04-28 20:45:52.000000 recipe_urls-0.2.0/tests/test_data/fifteenspatulas/fifteenspatulas_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2289 2024-04-28 20:45:52.000000 recipe_urls-0.2.0/tests/test_data/fifteenspatulas/fifteenspatulas_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.216272 recipe_urls-0.2.0/tests/test_data/finedininglovers/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)        0 2024-04-21 13:25:03.000000 recipe_urls-0.2.0/tests/test_data/finedininglovers/finedininglovers.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   124856 2024-04-21 13:25:03.000000 recipe_urls-0.2.0/tests/test_data/finedininglovers/finedininglovers.testhtml
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.221346 recipe_urls-0.2.0/tests/test_data/fitmencook/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   236110 2024-04-28 20:45:53.000000 recipe_urls-0.2.0/tests/test_data/fitmencook/fitmencook.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       33 2024-04-28 20:45:53.000000 recipe_urls-0.2.0/tests/test_data/fitmencook/fitmencook_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      704 2024-04-28 20:45:53.000000 recipe_urls-0.2.0/tests/test_data/fitmencook/fitmencook_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.224473 recipe_urls-0.2.0/tests/test_data/fitslowcookerqueen/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   116453 2024-04-28 20:45:54.000000 recipe_urls-0.2.0/tests/test_data/fitslowcookerqueen/fitslowcookerqueen.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       32 2024-04-28 20:45:54.000000 recipe_urls-0.2.0/tests/test_data/fitslowcookerqueen/fitslowcookerqueen_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      388 2024-04-28 20:45:54.000000 recipe_urls-0.2.0/tests/test_data/fitslowcookerqueen/fitslowcookerqueen_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.227228 recipe_urls-0.2.0/tests/test_data/food/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   242750 2024-04-28 20:45:54.000000 recipe_urls-0.2.0/tests/test_data/food/food.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       22 2024-04-28 20:45:54.000000 recipe_urls-0.2.0/tests/test_data/food/food_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1437 2024-04-28 20:45:54.000000 recipe_urls-0.2.0/tests/test_data/food/food_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.230913 recipe_urls-0.2.0/tests/test_data/food52/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   296436 2024-04-28 20:45:54.000000 recipe_urls-0.2.0/tests/test_data/food52/food52.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       20 2024-04-28 20:45:54.000000 recipe_urls-0.2.0/tests/test_data/food52/food52_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      567 2024-04-28 20:45:54.000000 recipe_urls-0.2.0/tests/test_data/food52/food52_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.233738 recipe_urls-0.2.0/tests/test_data/foodandwine/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   382116 2024-04-28 20:45:56.000000 recipe_urls-0.2.0/tests/test_data/foodandwine/foodandwine.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       37 2024-04-28 20:45:56.000000 recipe_urls-0.2.0/tests/test_data/foodandwine/foodandwine_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     5891 2024-04-28 20:45:56.000000 recipe_urls-0.2.0/tests/test_data/foodandwine/foodandwine_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.234393 recipe_urls-0.2.0/tests/test_data/foodnetwork/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)        0 2024-04-21 13:25:03.000000 recipe_urls-0.2.0/tests/test_data/foodnetwork/foodnetwork.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   402789 2024-04-21 13:25:03.000000 recipe_urls-0.2.0/tests/test_data/foodnetwork/foodnetwork.testhtml
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.238568 recipe_urls-0.2.0/tests/test_data/foodrepublic/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   112027 2024-04-28 20:45:58.000000 recipe_urls-0.2.0/tests/test_data/foodrepublic/foodrepublic.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       48 2024-04-28 20:45:58.000000 recipe_urls-0.2.0/tests/test_data/foodrepublic/foodrepublic_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1895 2024-04-28 20:45:58.000000 recipe_urls-0.2.0/tests/test_data/foodrepublic/foodrepublic_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.241148 recipe_urls-0.2.0/tests/test_data/forksoverknives/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   243422 2024-04-28 20:45:58.000000 recipe_urls-0.2.0/tests/test_data/forksoverknives/forksoverknives.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       33 2024-04-28 20:45:58.000000 recipe_urls-0.2.0/tests/test_data/forksoverknives/forksoverknives_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      465 2024-04-28 20:45:58.000000 recipe_urls-0.2.0/tests/test_data/forksoverknives/forksoverknives_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.243081 recipe_urls-0.2.0/tests/test_data/forktospoon/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   221279 2024-04-28 20:45:58.000000 recipe_urls-0.2.0/tests/test_data/forktospoon/forktospoon.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       43 2024-04-28 20:45:58.000000 recipe_urls-0.2.0/tests/test_data/forktospoon/forktospoon_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2038 2024-04-28 20:45:58.000000 recipe_urls-0.2.0/tests/test_data/forktospoon/forktospoon_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.246582 recipe_urls-0.2.0/tests/test_data/gimmesomeoven/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   263515 2024-04-28 20:45:58.000000 recipe_urls-0.2.0/tests/test_data/gimmesomeoven/gimmesomeoven.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       31 2024-04-28 20:45:58.000000 recipe_urls-0.2.0/tests/test_data/gimmesomeoven/gimmesomeoven_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      674 2024-04-28 20:45:58.000000 recipe_urls-0.2.0/tests/test_data/gimmesomeoven/gimmesomeoven_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.249079 recipe_urls-0.2.0/tests/test_data/gonnawantseconds/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   274045 2024-04-28 20:45:59.000000 recipe_urls-0.2.0/tests/test_data/gonnawantseconds/gonnawantseconds.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       34 2024-04-28 20:45:59.000000 recipe_urls-0.2.0/tests/test_data/gonnawantseconds/gonnawantseconds_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1532 2024-04-28 20:45:59.000000 recipe_urls-0.2.0/tests/test_data/gonnawantseconds/gonnawantseconds_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.251098 recipe_urls-0.2.0/tests/test_data/goodfooddiscoveries/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   147870 2024-04-28 20:45:59.000000 recipe_urls-0.2.0/tests/test_data/goodfooddiscoveries/goodfooddiscoveries.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       33 2024-04-28 20:45:59.000000 recipe_urls-0.2.0/tests/test_data/goodfooddiscoveries/goodfooddiscoveries_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      771 2024-04-28 20:45:59.000000 recipe_urls-0.2.0/tests/test_data/goodfooddiscoveries/goodfooddiscoveries_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.253661 recipe_urls-0.2.0/tests/test_data/goodhousekeeping/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   507132 2024-04-28 20:45:59.000000 recipe_urls-0.2.0/tests/test_data/goodhousekeeping/goodhousekeeping.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       48 2024-04-28 20:45:59.000000 recipe_urls-0.2.0/tests/test_data/goodhousekeeping/goodhousekeeping_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1422 2024-04-28 20:45:59.000000 recipe_urls-0.2.0/tests/test_data/goodhousekeeping/goodhousekeeping_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.256679 recipe_urls-0.2.0/tests/test_data/greatbritishchefs/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   499901 2024-04-28 20:46:00.000000 recipe_urls-0.2.0/tests/test_data/greatbritishchefs/greatbritishchefs.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       35 2024-04-28 20:46:00.000000 recipe_urls-0.2.0/tests/test_data/greatbritishchefs/greatbritishchefs_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1526 2024-04-28 20:46:00.000000 recipe_urls-0.2.0/tests/test_data/greatbritishchefs/greatbritishchefs_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.260670 recipe_urls-0.2.0/tests/test_data/halfbakedharvest/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   512401 2024-04-28 20:46:00.000000 recipe_urls-0.2.0/tests/test_data/halfbakedharvest/halfbakedharvest.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       34 2024-04-28 20:46:00.000000 recipe_urls-0.2.0/tests/test_data/halfbakedharvest/halfbakedharvest_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      440 2024-04-28 20:46:00.000000 recipe_urls-0.2.0/tests/test_data/halfbakedharvest/halfbakedharvest_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.263794 recipe_urls-0.2.0/tests/test_data/handletheheat/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   657790 2024-04-28 20:46:01.000000 recipe_urls-0.2.0/tests/test_data/handletheheat/handletheheat.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       27 2024-04-28 20:46:01.000000 recipe_urls-0.2.0/tests/test_data/handletheheat/handletheheat_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1936 2024-04-28 20:46:01.000000 recipe_urls-0.2.0/tests/test_data/handletheheat/handletheheat_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.266474 recipe_urls-0.2.0/tests/test_data/headbangerskitchen/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   458279 2024-04-28 20:46:02.000000 recipe_urls-0.2.0/tests/test_data/headbangerskitchen/headbangerskitchen.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       32 2024-04-28 20:46:02.000000 recipe_urls-0.2.0/tests/test_data/headbangerskitchen/headbangerskitchen_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1102 2024-04-28 20:46:02.000000 recipe_urls-0.2.0/tests/test_data/headbangerskitchen/headbangerskitchen_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.269138 recipe_urls-0.2.0/tests/test_data/heatherchristo/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    68765 2024-04-28 20:46:02.000000 recipe_urls-0.2.0/tests/test_data/heatherchristo/heatherchristo.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:46:02.000000 recipe_urls-0.2.0/tests/test_data/heatherchristo/heatherchristo_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1803 2024-04-28 20:46:02.000000 recipe_urls-0.2.0/tests/test_data/heatherchristo/heatherchristo_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.273938 recipe_urls-0.2.0/tests/test_data/hellofresh/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)  2245425 2024-04-28 20:46:03.000000 recipe_urls-0.2.0/tests/test_data/hellofresh/hellofresh.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       36 2024-04-28 20:46:03.000000 recipe_urls-0.2.0/tests/test_data/hellofresh/hellofresh_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     8561 2024-04-28 20:46:03.000000 recipe_urls-0.2.0/tests/test_data/hellofresh/hellofresh_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.276399 recipe_urls-0.2.0/tests/test_data/hersheyland/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   135835 2024-04-28 20:46:03.000000 recipe_urls-0.2.0/tests/test_data/hersheyland/hersheyland.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       37 2024-04-28 20:46:03.000000 recipe_urls-0.2.0/tests/test_data/hersheyland/hersheyland_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      416 2024-04-28 20:46:03.000000 recipe_urls-0.2.0/tests/test_data/hersheyland/hersheyland_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.279042 recipe_urls-0.2.0/tests/test_data/hostthetoast/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   403510 2024-04-28 20:46:05.000000 recipe_urls-0.2.0/tests/test_data/hostthetoast/hostthetoast.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       35 2024-04-28 20:46:05.000000 recipe_urls-0.2.0/tests/test_data/hostthetoast/hostthetoast_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     5814 2024-04-28 20:46:05.000000 recipe_urls-0.2.0/tests/test_data/hostthetoast/hostthetoast_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.281498 recipe_urls-0.2.0/tests/test_data/im-worthy/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   125319 2024-04-28 20:46:05.000000 recipe_urls-0.2.0/tests/test_data/im-worthy/im-worthy.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       23 2024-04-28 20:46:05.000000 recipe_urls-0.2.0/tests/test_data/im-worthy/im-worthy_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      409 2024-04-28 20:46:05.000000 recipe_urls-0.2.0/tests/test_data/im-worthy/im-worthy_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.284628 recipe_urls-0.2.0/tests/test_data/indianhealthyrecipes/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   472899 2024-04-28 20:46:06.000000 recipe_urls-0.2.0/tests/test_data/indianhealthyrecipes/indianhealthyrecipes.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       38 2024-04-28 20:46:06.000000 recipe_urls-0.2.0/tests/test_data/indianhealthyrecipes/indianhealthyrecipes_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     3950 2024-04-28 20:46:06.000000 recipe_urls-0.2.0/tests/test_data/indianhealthyrecipes/indianhealthyrecipes_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.287336 recipe_urls-0.2.0/tests/test_data/insanelygoodrecipes/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   275885 2024-04-28 20:46:07.000000 recipe_urls-0.2.0/tests/test_data/insanelygoodrecipes/insanelygoodrecipes.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       33 2024-04-28 20:46:07.000000 recipe_urls-0.2.0/tests/test_data/insanelygoodrecipes/insanelygoodrecipes_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2347 2024-04-28 20:46:07.000000 recipe_urls-0.2.0/tests/test_data/insanelygoodrecipes/insanelygoodrecipes_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.289201 recipe_urls-0.2.0/tests/test_data/inspiralized/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   300289 2024-04-28 20:46:08.000000 recipe_urls-0.2.0/tests/test_data/inspiralized/inspiralized.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       26 2024-04-28 20:46:08.000000 recipe_urls-0.2.0/tests/test_data/inspiralized/inspiralized_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1933 2024-04-28 20:46:08.000000 recipe_urls-0.2.0/tests/test_data/inspiralized/inspiralized_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.292135 recipe_urls-0.2.0/tests/test_data/izzycooking/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   334445 2024-04-28 20:46:08.000000 recipe_urls-0.2.0/tests/test_data/izzycooking/izzycooking.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       25 2024-04-28 20:46:08.000000 recipe_urls-0.2.0/tests/test_data/izzycooking/izzycooking_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1527 2024-04-28 20:46:08.000000 recipe_urls-0.2.0/tests/test_data/izzycooking/izzycooking_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.300021 recipe_urls-0.2.0/tests/test_data/jamieoliver/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   344432 2024-04-28 20:46:09.000000 recipe_urls-0.2.0/tests/test_data/jamieoliver/jamieoliver.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       29 2024-04-28 20:46:09.000000 recipe_urls-0.2.0/tests/test_data/jamieoliver/jamieoliver_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     5872 2024-04-28 20:46:09.000000 recipe_urls-0.2.0/tests/test_data/jamieoliver/jamieoliver_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.302222 recipe_urls-0.2.0/tests/test_data/jimcooksfoodgood/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   154702 2024-04-28 20:46:10.000000 recipe_urls-0.2.0/tests/test_data/jimcooksfoodgood/jimcooksfoodgood.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       30 2024-04-28 20:46:10.000000 recipe_urls-0.2.0/tests/test_data/jimcooksfoodgood/jimcooksfoodgood_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      564 2024-04-28 20:46:10.000000 recipe_urls-0.2.0/tests/test_data/jimcooksfoodgood/jimcooksfoodgood_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.305297 recipe_urls-0.2.0/tests/test_data/joyfoodsunshine/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   402222 2024-04-28 20:46:10.000000 recipe_urls-0.2.0/tests/test_data/joyfoodsunshine/joyfoodsunshine.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       29 2024-04-28 20:46:10.000000 recipe_urls-0.2.0/tests/test_data/joyfoodsunshine/joyfoodsunshine_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2979 2024-04-28 20:46:10.000000 recipe_urls-0.2.0/tests/test_data/joyfoodsunshine/joyfoodsunshine_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.307696 recipe_urls-0.2.0/tests/test_data/justataste/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   334680 2024-04-28 20:46:11.000000 recipe_urls-0.2.0/tests/test_data/justataste/justataste.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:46:11.000000 recipe_urls-0.2.0/tests/test_data/justataste/justataste_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2373 2024-04-28 20:46:11.000000 recipe_urls-0.2.0/tests/test_data/justataste/justataste_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.311714 recipe_urls-0.2.0/tests/test_data/justbento/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    44375 2024-04-28 20:46:11.000000 recipe_urls-0.2.0/tests/test_data/justbento/justbento.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       35 2024-04-28 20:46:11.000000 recipe_urls-0.2.0/tests/test_data/justbento/justbento_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2238 2024-04-28 20:46:11.000000 recipe_urls-0.2.0/tests/test_data/justbento/justbento_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.316397 recipe_urls-0.2.0/tests/test_data/justonecookbook/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   533539 2024-04-28 20:46:12.000000 recipe_urls-0.2.0/tests/test_data/justonecookbook/justonecookbook.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       33 2024-04-28 20:46:12.000000 recipe_urls-0.2.0/tests/test_data/justonecookbook/justonecookbook_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      805 2024-04-28 20:46:12.000000 recipe_urls-0.2.0/tests/test_data/justonecookbook/justonecookbook_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.321110 recipe_urls-0.2.0/tests/test_data/kingarthurbaking/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   193979 2024-04-28 20:46:12.000000 recipe_urls-0.2.0/tests/test_data/kingarthurbaking/kingarthurbaking.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       34 2024-04-28 20:46:12.000000 recipe_urls-0.2.0/tests/test_data/kingarthurbaking/kingarthurbaking_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      310 2024-04-28 20:46:12.000000 recipe_urls-0.2.0/tests/test_data/kingarthurbaking/kingarthurbaking_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.325217 recipe_urls-0.2.0/tests/test_data/leanandgreenrecipes/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    68583 2024-04-28 20:46:12.000000 recipe_urls-0.2.0/tests/test_data/leanandgreenrecipes/leanandgreenrecipes.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       33 2024-04-28 20:46:12.000000 recipe_urls-0.2.0/tests/test_data/leanandgreenrecipes/leanandgreenrecipes_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1525 2024-04-28 20:46:12.000000 recipe_urls-0.2.0/tests/test_data/leanandgreenrecipes/leanandgreenrecipes_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.328034 recipe_urls-0.2.0/tests/test_data/lifestyleofafoodie/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   150175 2024-04-28 20:46:13.000000 recipe_urls-0.2.0/tests/test_data/lifestyleofafoodie/lifestyleofafoodie.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       32 2024-04-28 20:46:13.000000 recipe_urls-0.2.0/tests/test_data/lifestyleofafoodie/lifestyleofafoodie_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      521 2024-04-28 20:46:13.000000 recipe_urls-0.2.0/tests/test_data/lifestyleofafoodie/lifestyleofafoodie_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.332528 recipe_urls-0.2.0/tests/test_data/littlespicejar/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   293442 2024-04-28 20:46:13.000000 recipe_urls-0.2.0/tests/test_data/littlespicejar/littlespicejar.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:46:13.000000 recipe_urls-0.2.0/tests/test_data/littlespicejar/littlespicejar_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1291 2024-04-28 20:46:13.000000 recipe_urls-0.2.0/tests/test_data/littlespicejar/littlespicejar_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.335194 recipe_urls-0.2.0/tests/test_data/livelytable/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   191757 2024-04-28 20:46:14.000000 recipe_urls-0.2.0/tests/test_data/livelytable/livelytable.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       25 2024-04-28 20:46:14.000000 recipe_urls-0.2.0/tests/test_data/livelytable/livelytable_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2381 2024-04-28 20:46:14.000000 recipe_urls-0.2.0/tests/test_data/livelytable/livelytable_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.337506 recipe_urls-0.2.0/tests/test_data/lovingitvegan/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   366684 2024-04-28 20:46:14.000000 recipe_urls-0.2.0/tests/test_data/lovingitvegan/lovingitvegan.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       27 2024-04-28 20:46:14.000000 recipe_urls-0.2.0/tests/test_data/lovingitvegan/lovingitvegan_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     3918 2024-04-28 20:46:14.000000 recipe_urls-0.2.0/tests/test_data/lovingitvegan/lovingitvegan_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.341376 recipe_urls-0.2.0/tests/test_data/ninjatestkitchen/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   100240 2024-04-28 20:46:17.000000 recipe_urls-0.2.0/tests/test_data/ninjatestkitchen/ninjatestkitchen.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       29 2024-04-28 20:46:17.000000 recipe_urls-0.2.0/tests/test_data/ninjatestkitchen/ninjatestkitchen_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      662 2024-04-28 20:46:17.000000 recipe_urls-0.2.0/tests/test_data/ninjatestkitchen/ninjatestkitchen_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.347184 recipe_urls-0.2.0/tests/test_data/nytimes/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)  1775626 2024-04-28 20:46:20.000000 recipe_urls-0.2.0/tests/test_data/nytimes/nytimes.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       29 2024-04-28 20:46:20.000000 recipe_urls-0.2.0/tests/test_data/nytimes/nytimes_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    10823 2024-04-28 20:46:20.000000 recipe_urls-0.2.0/tests/test_data/nytimes/nytimes_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.351127 recipe_urls-0.2.0/tests/test_data/ohsheglows/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   267520 2024-04-28 20:46:20.000000 recipe_urls-0.2.0/tests/test_data/ohsheglows/ohsheglows.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       24 2024-04-28 20:46:20.000000 recipe_urls-0.2.0/tests/test_data/ohsheglows/ohsheglows_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      905 2024-04-28 20:46:20.000000 recipe_urls-0.2.0/tests/test_data/ohsheglows/ohsheglows_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.354962 recipe_urls-0.2.0/tests/test_data/onceuponachef/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   277915 2024-04-28 20:46:20.000000 recipe_urls-0.2.0/tests/test_data/onceuponachef/onceuponachef.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       31 2024-04-28 20:46:20.000000 recipe_urls-0.2.0/tests/test_data/onceuponachef/onceuponachef_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1052 2024-04-28 20:46:20.000000 recipe_urls-0.2.0/tests/test_data/onceuponachef/onceuponachef_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.358604 recipe_urls-0.2.0/tests/test_data/paleorunningmomma/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   290708 2024-04-28 20:46:20.000000 recipe_urls-0.2.0/tests/test_data/paleorunningmomma/paleorunningmomma.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       35 2024-04-28 20:46:20.000000 recipe_urls-0.2.0/tests/test_data/paleorunningmomma/paleorunningmomma_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      902 2024-04-28 20:46:20.000000 recipe_urls-0.2.0/tests/test_data/paleorunningmomma/paleorunningmomma_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.362103 recipe_urls-0.2.0/tests/test_data/persnicketyplates/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   691102 2024-04-28 20:46:21.000000 recipe_urls-0.2.0/tests/test_data/persnicketyplates/persnicketyplates.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       35 2024-04-28 20:46:21.000000 recipe_urls-0.2.0/tests/test_data/persnicketyplates/persnicketyplates_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1951 2024-04-28 20:46:21.000000 recipe_urls-0.2.0/tests/test_data/persnicketyplates/persnicketyplates_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.364746 recipe_urls-0.2.0/tests/test_data/platingpixels/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   272367 2024-04-28 20:46:22.000000 recipe_urls-0.2.0/tests/test_data/platingpixels/platingpixels.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       31 2024-04-28 20:46:22.000000 recipe_urls-0.2.0/tests/test_data/platingpixels/platingpixels_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1204 2024-04-28 20:46:22.000000 recipe_urls-0.2.0/tests/test_data/platingpixels/platingpixels_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.367144 recipe_urls-0.2.0/tests/test_data/rachlmansfield/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   346194 2024-04-28 20:46:22.000000 recipe_urls-0.2.0/tests/test_data/rachlmansfield/rachlmansfield.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:46:22.000000 recipe_urls-0.2.0/tests/test_data/rachlmansfield/rachlmansfield_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     3160 2024-04-28 20:46:22.000000 recipe_urls-0.2.0/tests/test_data/rachlmansfield/rachlmansfield_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.369722 recipe_urls-0.2.0/tests/test_data/rainbowplantlife/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   258321 2024-04-28 20:46:22.000000 recipe_urls-0.2.0/tests/test_data/rainbowplantlife/rainbowplantlife.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       30 2024-04-28 20:46:22.000000 recipe_urls-0.2.0/tests/test_data/rainbowplantlife/rainbowplantlife_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      422 2024-04-28 20:46:22.000000 recipe_urls-0.2.0/tests/test_data/rainbowplantlife/rainbowplantlife_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.372137 recipe_urls-0.2.0/tests/test_data/reciperunner/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   319663 2024-04-28 20:46:23.000000 recipe_urls-0.2.0/tests/test_data/reciperunner/reciperunner.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       26 2024-04-28 20:46:23.000000 recipe_urls-0.2.0/tests/test_data/reciperunner/reciperunner_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1502 2024-04-28 20:46:23.000000 recipe_urls-0.2.0/tests/test_data/reciperunner/reciperunner_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.376648 recipe_urls-0.2.0/tests/test_data/sallysbakingaddiction/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   590698 2024-04-28 20:46:25.000000 recipe_urls-0.2.0/tests/test_data/sallysbakingaddiction/sallysbakingaddiction.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       35 2024-04-28 20:46:25.000000 recipe_urls-0.2.0/tests/test_data/sallysbakingaddiction/sallysbakingaddiction_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     5318 2024-04-28 20:46:25.000000 recipe_urls-0.2.0/tests/test_data/sallysbakingaddiction/sallysbakingaddiction_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.384040 recipe_urls-0.2.0/tests/test_data/simple-veganista/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   535633 2024-04-28 20:46:25.000000 recipe_urls-0.2.0/tests/test_data/simple-veganista/simple-veganista.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       30 2024-04-28 20:46:25.000000 recipe_urls-0.2.0/tests/test_data/simple-veganista/simple-veganista_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2251 2024-04-28 20:46:25.000000 recipe_urls-0.2.0/tests/test_data/simple-veganista/simple-veganista_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.390545 recipe_urls-0.2.0/tests/test_data/simplywhisked/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   491237 2024-04-28 20:46:26.000000 recipe_urls-0.2.0/tests/test_data/simplywhisked/simplywhisked.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       31 2024-04-28 20:46:26.000000 recipe_urls-0.2.0/tests/test_data/simplywhisked/simplywhisked_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     3011 2024-04-28 20:46:26.000000 recipe_urls-0.2.0/tests/test_data/simplywhisked/simplywhisked_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.392940 recipe_urls-0.2.0/tests/test_data/tasteofhome/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   201999 2024-04-28 20:46:27.000000 recipe_urls-0.2.0/tests/test_data/tasteofhome/tasteofhome.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       29 2024-04-28 20:46:27.000000 recipe_urls-0.2.0/tests/test_data/tasteofhome/tasteofhome_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1028 2024-04-28 20:46:27.000000 recipe_urls-0.2.0/tests/test_data/tasteofhome/tasteofhome_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.396210 recipe_urls-0.2.0/tests/test_data/tasty/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   454175 2024-04-28 20:46:27.000000 recipe_urls-0.2.0/tests/test_data/tasty/tasty.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       18 2024-04-28 20:46:27.000000 recipe_urls-0.2.0/tests/test_data/tasty/tasty_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1150 2024-04-28 20:46:27.000000 recipe_urls-0.2.0/tests/test_data/tasty/tasty_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.398500 recipe_urls-0.2.0/tests/test_data/wellplated/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   447000 2024-04-28 20:46:29.000000 recipe_urls-0.2.0/tests/test_data/wellplated/wellplated.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       28 2024-04-28 20:46:29.000000 recipe_urls-0.2.0/tests/test_data/wellplated/wellplated_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2200 2024-04-28 20:46:29.000000 recipe_urls-0.2.0/tests/test_data/wellplated/wellplated_exp_output.csv
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-28 20:53:24.401433 recipe_urls-0.2.0/tests/test_data/whole30/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   508196 2024-04-28 20:46:29.000000 recipe_urls-0.2.0/tests/test_data/whole30/whole30.testhtml
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       21 2024-04-28 20:46:29.000000 recipe_urls-0.2.0/tests/test_data/whole30/whole30_base_url.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      584 2024-04-28 20:46:29.000000 recipe_urls-0.2.0/tests/test_data/whole30/whole30_exp_output.csv
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1785 2024-04-28 17:20:04.000000 recipe_urls-0.2.0/tests/test_get_site_origin.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     3414 2024-04-28 20:36:43.000000 recipe_urls-0.2.0/tests/test_scrapers_with_base_url.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2978 2024-04-28 20:48:07.000000 recipe_urls-0.2.0/tests/test_scrapers_with_html.py
```

### Comparing `recipe_urls-0.1.3/.DS_Store` & `recipe_urls-0.2.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.3/LICENSE` & `recipe_urls-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.3/PKG-INFO` & `recipe_urls-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,52 @@
-Metadata-Version: 2.1
-Name: recipe_urls
-Version: 0.1.3
-Summary: Scrapes all recipe URLs from provided base URL.
-Author-email: Melissa Terry <mkayeterry@gmail.com>
-License: MIT License
-Keywords: recipe,scraper,URLs,links
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: httpx>=0.26.0
-Requires-Dist: beautifulsoup4>=4.11.1
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pip-tools; extra == "test"
-Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-
 # recipe-urls
 
 ## Overview
 
-`recipe-urls` is a Python package designed to gather recipe URLs from a given base URL.
+`recipe-urls` is a Python package designed to gather recipe URLs from a given base URL or from provided html content.
+
+<br>
 
 ## Installation
 
 ```bash
 pip install recipe-urls
 ```
 
 ## Usage
 
 ```python
-from recipe_urls import scrape_urls
+from recipe_urls import scrape_urls, scrape_html
 ```
 
 ## Example usage
 
 ```python
-base_urls = ['https://bakingmischief.com', 'https://www.allrecipes.com']
+base_urls = ['https://bakingmischief.com', 'https://www.allrecipes.com/recipes/80/main-dish/']
 compiled_recipe_links = []
 
 for base_url in base_urls:
+    scraped_links = scrape_urls(base_url)
+    compiled_recipe_links.extend(scraped_links)
+```
+```python
+input_html = [baking_mischief_html, all_recipes_html]
+compiled_recipe_links = []
 
-    scrape = scrape_urls(base_url)
-    compiled_recipe_links.extend(scrape)
+for html_content in input_html:
+    scraped_links = scrape_html(html) # optionally, scrape_html(html, base_url)
+    compiled_recipe_links.extend(scraped_links)
 ```
 
 ## Supported Websites
 
 - https://abuelascounter.com
 - https://www.acouplecooks.com
 - https://addapinch.com
-- https://www.afghankitchenrecipes.com
+- http://www.afghankitchenrecipes.com
 - https://www.allrecipes.com
 - https://www.ambitiouskitchen.com
 - https://www.archanaskitchen.com
 - https://www.averiecooks.com
 - https://bakingmischief.com
 - https://www.baking-sense.com
 - https://barefootcontessa.com
@@ -152,13 +134,17 @@
 - https://rainbowplantlife.com
 - https://reciperunner.com
 - https://sallysbakingaddiction.com
 - https://simple-veganista.com
 - https://www.simplywhisked.com
 - https://www.tasteofhome.com
 - https://tasty.co
+- https://www.wellplated.com
+- https://whole30.com
 
 
+## Acknowledgments 
+This package was inspired by (and meant to be used in conjunction with) [recipe-scrapers](https://github.com/hhursev/recipe-scrapers) by [hhursev](https://github.com/hhursev). Thanks for making the intersection of programming and recipes more doable!
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `recipe_urls-0.1.3/README.md` & `recipe_urls-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,79 @@
+Metadata-Version: 2.1
+Name: recipe_urls
+Version: 0.2.0
+Summary: Scrapes all recipe URLs from provided base URL.
+Author-email: Melissa Terry <mkayeterry@gmail.com>
+License: MIT License
+Keywords: recipe,scraper,URLs,links
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.26.0
+Requires-Dist: beautifulsoup4>=4.11.1
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pip-tools; extra == "test"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+
 # recipe-urls
 
 ## Overview
 
-`recipe-urls` is a Python package designed to gather recipe URLs from a given base URL.
+`recipe-urls` is a Python package designed to gather recipe URLs from a given base URL or from provided html content.
+
+<br>
 
 ## Installation
 
 ```bash
 pip install recipe-urls
 ```
 
 ## Usage
 
 ```python
-from recipe_urls import scrape_urls
+from recipe_urls import scrape_urls, scrape_html
 ```
 
 ## Example usage
 
 ```python
-base_urls = ['https://bakingmischief.com', 'https://www.allrecipes.com']
+base_urls = ['https://bakingmischief.com', 'https://www.allrecipes.com/recipes/80/main-dish/']
 compiled_recipe_links = []
 
 for base_url in base_urls:
+    scraped_links = scrape_urls(base_url)
+    compiled_recipe_links.extend(scraped_links)
+```
+```python
+input_html = [baking_mischief_html, all_recipes_html]
+compiled_recipe_links = []
 
-    scrape = scrape_urls(base_url)
-    compiled_recipe_links.extend(scrape)
+for html_content in input_html:
+    scraped_links = scrape_html(html) # optionally, scrape_html(html, base_url)
+    compiled_recipe_links.extend(scraped_links)
 ```
 
 ## Supported Websites
 
 - https://abuelascounter.com
 - https://www.acouplecooks.com
 - https://addapinch.com
-- https://www.afghankitchenrecipes.com
+- http://www.afghankitchenrecipes.com
 - https://www.allrecipes.com
 - https://www.ambitiouskitchen.com
 - https://www.archanaskitchen.com
 - https://www.averiecooks.com
 - https://bakingmischief.com
 - https://www.baking-sense.com
 - https://barefootcontessa.com
@@ -125,13 +161,17 @@
 - https://rainbowplantlife.com
 - https://reciperunner.com
 - https://sallysbakingaddiction.com
 - https://simple-veganista.com
 - https://www.simplywhisked.com
 - https://www.tasteofhome.com
 - https://tasty.co
+- https://www.wellplated.com
+- https://whole30.com
 
 
+## Acknowledgments 
+This package was inspired by (and meant to be used in conjunction with) [recipe-scrapers](https://github.com/hhursev/recipe-scrapers) by [hhursev](https://github.com/hhursev). Thanks for making the intersection of programming and recipes more doable!
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `recipe_urls-0.1.3/pyproject.toml` & `recipe_urls-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "recipe_urls"
 authors = [
   {name = "Melissa Terry", email = "mkayeterry@gmail.com"},
 ]
-version = "0.1.3"
+version = "0.2.0"
 description = "Scrapes all recipe URLs from provided base URL."
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
@@ -19,15 +19,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Utilities",
 ]
 keywords = ["recipe", "scraper", "URLs", "links"]
 license = {text = "MIT License"}
 dependencies = [
-        "httpx >= 0.26.0", 
+        "requests >= 2.26.0", 
         "beautifulsoup4 >= 4.11.1"
     ]
 requires-python = ">=3.7"
 readme = "README.md"
 
 [project.optional-dependencies]
 test = [
```

### Comparing `recipe_urls-0.1.3/recipe_urls/.DS_Store` & `recipe_urls-0.2.0/recipe_urls/.DS_Store`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.3/recipe_urls/__init__.py` & `recipe_urls-0.2.0/recipe_urls/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-__version__ = "0.1.3"
+__version__ = "0.2.0"
 
 from typing import Optional
-import httpx
-
 from recipe_urls._abstract import AbstractScraper
 from recipe_urls._utils import get_site_origin
 
 from recipe_urls.abuelascounter import AbuelasCounterScraper
 from recipe_urls.acouplecooks import ACoupleCooksScraper
 from recipe_urls.addapinch import AddAPinchScraper
 from recipe_urls.afghankitchenrecipes import AfghanKitchenRecipesScraper
@@ -101,14 +99,16 @@
 from recipe_urls.rainbowplantlife import RainbowPlantLifeScraper
 from recipe_urls.reciperunner import RecipeRunnerScraper
 from recipe_urls.sallysbakingaddiction import SallysBakingAddictionScraper
 from recipe_urls.simpleveganista import SimpleVeganistaScraper
 from recipe_urls.simplywhisked import SimplyWhiskedScraper
 from recipe_urls.tasteofhome import TasteOfHomeScraper
 from recipe_urls.tasty import TastyScraper
+from recipe_urls.wellplated import WellPlatedScraper
+from recipe_urls.whole30 import Whole30Scraper
 
 
 
 SCRAPERS = {
     AbuelasCounterScraper.host(): AbuelasCounterScraper, 
     ACoupleCooksScraper.host(): ACoupleCooksScraper, 
     AddAPinchScraper.host(): AddAPinchScraper,
@@ -203,26 +203,48 @@
     RachlMansfieldScraper.host(): RachlMansfieldScraper, 
     RainbowPlantLifeScraper.host(): RainbowPlantLifeScraper, 
     RecipeRunnerScraper.host(): RecipeRunnerScraper, 
     SallysBakingAddictionScraper.host(): SallysBakingAddictionScraper, 
     SimpleVeganistaScraper.host(): SimpleVeganistaScraper, 
     SimplyWhiskedScraper.host(): SimplyWhiskedScraper, 
     TasteOfHomeScraper.host(): TasteOfHomeScraper, 
-    TastyScraper.host(): TastyScraper
+    TastyScraper.host(): TastyScraper, 
+    WellPlatedScraper.host(): WellPlatedScraper, 
+    Whole30Scraper.host(): Whole30Scraper
 }
 
 def scrape_urls(base_url: str) -> Optional[AbstractScraper]:
+    
     try:
-        scraper_class = SCRAPERS.get(get_site_origin(base_url))
+        origin = get_site_origin(base_url, html=None)
+        scraper_class = SCRAPERS.get(origin)
+
         if not scraper_class:
-            raise ValueError(f"Unsupported website {base_url}")
+            raise ValueError(f"Unsupported website: {base_url}")
 
-        scraper_instance = scraper_class(base_url)
-        return scraper_instance.scrape()
+        return scraper_class(base_url, html = None).scrape()
 
     except Exception as e:
-        raise e from None
+        raise ValueError(f"Failed to scrape {base_url}. {str(e)}") from None
+
+def scrape_html(html: str, base_url: str | None = None) -> Optional[AbstractScraper]:
+
+    try:
+        origin = get_site_origin(base_url, html=html)
 
+        if not origin:
+            raise ValueError(f"Base URL was not extracted from HTML content. Please provide a base URL.")
 
+        scraper_class = SCRAPERS.get(origin)
+
+        if not scraper_class:
+            raise ValueError(f"Unsupported website: {origin}")
+
+        return scraper_class(base_url, html = html).scrape()
+
+    except Exception as e:
+        raise ValueError(f"Failed to scrape HTML content. {str(e)}") from None
+        
 __all__ = [
-    'scrape_urls'
+    'scrape_urls', 
+    'scrape_html'
 ]
```

