# Comparing `tmp/kss-6.0.0.tar.gz` & `tmp/kss-6.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kss-6.0.0.tar", last modified: Sat Apr 27 14:20:50 2024, max compression
+gzip compressed data, was "kss-6.0.0.dev0.tar", last modified: Sun Apr 28 13:41:19 2024, max compression
```

## Comparing `kss-6.0.0.tar` & `kss-6.0.0.dev0.tar`

### file list

```diff
@@ -1,235 +1,236 @@
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.456971 kss-6.0.0/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1569 2024-04-01 04:29:21.000000 kss-6.0.0/LICENSE
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-26 04:11:11.000000 kss-6.0.0/MANIFEST.in
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   204750 2024-04-27 14:20:50.457167 kss-6.0.0/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   203997 2024-04-27 14:03:15.000000 kss-6.0.0/README.md
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.432871 kss-6.0.0/bench/
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.438034 kss-6.0.0/bench/sentence_split/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 04:39:09.000000 kss-6.0.0/bench/sentence_split/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4379 2023-05-16 17:34:32.000000 kss-6.0.0/bench/sentence_split/sentence_split.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      615 2023-05-16 17:34:32.000000 kss-6.0.0/bench/sentence_split/test_baseline.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      600 2023-05-16 17:34:32.000000 kss-6.0.0/bench/sentence_split/test_kiwi.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1015 2023-05-16 17:34:32.000000 kss-6.0.0/bench/sentence_split/test_koalanlp.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      700 2024-03-31 14:00:52.000000 kss-6.0.0/bench/sentence_split/test_kss.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      587 2023-05-16 17:34:32.000000 kss-6.0.0/bench/sentence_split/test_word_split.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.438611 kss-6.0.0/csrc/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2024-03-31 20:12:01.000000 kss-6.0.0/csrc/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      563 2024-03-31 20:36:14.000000 kss-6.0.0/csrc/kss_cython.pyx
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5965 2024-03-31 20:12:01.000000 kss-6.0.0/csrc/sentence_splitter.cpp
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7830 2024-03-31 20:12:01.000000 kss-6.0.0/csrc/sentence_splitter.h
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.438706 kss-6.0.0/kss/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6879 2024-04-27 14:20:34.000000 kss-6.0.0/kss/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.439775 kss-6.0.0/kss/_elements/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_elements/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4888 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_elements/element.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2702 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_elements/empty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      536 2024-04-14 01:15:11.000000 kss-6.0.0/kss/_elements/subclasses.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.439874 kss-6.0.0/kss/_modules/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.440428 kss-6.0.0/kss/_modules/augmentation/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:47:16.000000 kss-6.0.0/kss/_modules/augmentation/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.440551 kss-6.0.0/kss/_modules/augmentation/assets/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)  4865459 2021-09-26 12:11:43.000000 kss-6.0.0/kss/_modules/augmentation/assets/wordnet.json
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3892 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/augmentation/augment.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3251 2024-04-23 11:22:09.000000 kss-6.0.0/kss/_modules/augmentation/distance.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3602 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/augmentation/replacement.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1411 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/augmentation/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.443519 kss-6.0.0/kss/_modules/collocation/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 18:49:12.000000 kss-6.0.0/kss/_modules/collocation/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9351 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/collocation/collocate.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.444218 kss-6.0.0/kss/_modules/g2p/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 11:01:28.000000 kss-6.0.0/kss/_modules/g2p/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.444424 kss-6.0.0/kss/_modules/g2p/assets/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    14802 2024-04-21 10:45:23.000000 kss-6.0.0/kss/_modules/g2p/assets/rules.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5390 2024-04-21 10:46:10.000000 kss-6.0.0/kss/_modules/g2p/assets/table.csv
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6586 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/g2p/english.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7184 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/g2p/g2p.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4459 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/g2p/numerals.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2722 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/g2p/regular.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4949 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/g2p/special.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8131 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/g2p/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.444601 kss-6.0.0/kss/_modules/hangulization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-26 07:28:27.000000 kss-6.0.0/kss/_modules/hangulization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3616 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/hangulization/hangulization.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445130 kss-6.0.0/kss/_modules/hangulization/hangulize/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     2277 2024-04-27 09:12:39.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/__init__.py
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)    10423 2024-04-27 09:00:03.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/hangul.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445232 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     1426 2018-08-18 18:42:06.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445328 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/aze/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5272 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/aze/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445429 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/bel/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5425 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/bel/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445526 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/bul/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4925 2018-08-18 18:42:06.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/bul/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445636 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/cat/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4328 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/cat/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445745 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ces/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4820 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ces/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445848 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/cym/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5791 2018-08-18 18:42:06.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/cym/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445951 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/deu/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     7415 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/deu/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446068 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ell/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     9068 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ell/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446176 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/epo/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4103 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/epo/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446285 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/est/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3931 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/est/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446394 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/fin/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3410 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/fin/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446509 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/grc/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     8626 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/grc/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446628 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/hbs/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5606 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446736 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/hun/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4990 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/hun/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446840 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/isl/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5626 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/isl/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446943 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ita/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4371 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ita/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447047 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/jpn/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4446 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447255 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/kat/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6118 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/kat/__init__.py
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6408 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/kat/narrow.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447352 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lat/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3314 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lat/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447464 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lav/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4116 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lav/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447560 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lit/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4080 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lit/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447665 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/mkd/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5354 2018-08-18 18:42:06.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447764 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/nld/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)    22064 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/nld/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447880 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/pol/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5785 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/pol/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448080 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/por/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6048 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/por/__init__.py
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/por/br.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448184 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ron/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5120 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ron/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448280 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/rus/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4994 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/rus/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448379 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/slk/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6693 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/slk/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448475 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/slv/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3836 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/slv/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448578 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/spa/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4002 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/spa/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448672 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/sqi/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3177 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448769 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/swe/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     7896 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/swe/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448864 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/tur/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3528 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/tur/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448961 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ukr/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5072 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.449066 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/vie/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4742 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/vie/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.449161 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/wlm/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5599 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)    16108 2024-04-27 09:00:03.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/models.py
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     1069 2018-08-18 18:42:06.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/normalization.py
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     2897 2024-04-27 08:57:42.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/processing.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.449429 kss-6.0.0/kss/_modules/hanja/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:46:48.000000 kss-6.0.0/kss/_modules/hanja/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4462 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/hanja/_hanja.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2021 2024-04-25 08:27:31.000000 kss-6.0.0/kss/_modules/hanja/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.449694 kss-6.0.0/kss/_modules/jamo/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:46:59.000000 kss-6.0.0/kss/_modules/jamo/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    12624 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/jamo/_jamo.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      912 2024-04-25 08:38:54.000000 kss-6.0.0/kss/_modules/jamo/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.449969 kss-6.0.0/kss/_modules/josa/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 07:12:50.000000 kss-6.0.0/kss/_modules/josa/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2580 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/josa/josa.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7030 2024-04-25 16:33:55.000000 kss-6.0.0/kss/_modules/josa/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.450239 kss-6.0.0/kss/_modules/keywords/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 11:01:42.000000 kss-6.0.0/kss/_modules/keywords/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6362 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/keywords/extract_keywords.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    17289 2024-04-27 12:31:02.000000 kss-6.0.0/kss/_modules/keywords/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.450647 kss-6.0.0/kss/_modules/morphemes/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/morphemes/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2652 2024-03-31 13:42:10.000000 kss-6.0.0/kss/_modules/morphemes/analyzers.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1849 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/morphemes/split_morphemes.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3588 2024-04-23 09:05:15.000000 kss-6.0.0/kss/_modules/morphemes/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.450821 kss-6.0.0/kss/_modules/paradigm/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 08:40:05.000000 kss-6.0.0/kss/_modules/paradigm/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    18316 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/paradigm/paradigm.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.451926 kss-6.0.0/kss/_modules/preprocessing/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-26 07:58:23.000000 kss-6.0.0/kss/_modules/preprocessing/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    15532 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/anonymize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    29789 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/clean_news.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    81169 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/completed_form.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    24570 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/filter_out.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2088 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/half2full.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/normalize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    26257 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/preprocess.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7186 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/reduce_repeats.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7661 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/remove_invisible_chars.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.452201 kss-6.0.0/kss/_modules/qwerty/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 08:21:28.000000 kss-6.0.0/kss/_modules/qwerty/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6262 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/qwerty/qwerty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5941 2024-04-21 19:55:18.000000 kss-6.0.0/kss/_modules/qwerty/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.452475 kss-6.0.0/kss/_modules/romanization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:48:29.000000 kss-6.0.0/kss/_modules/romanization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5813 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/romanization/romanize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8901 2024-04-21 17:45:54.000000 kss-6.0.0/kss/_modules/romanization/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.452757 kss-6.0.0/kss/_modules/safety/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 04:59:07.000000 kss-6.0.0/kss/_modules/safety/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3525 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/safety/check_safety.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    35374 2024-04-21 06:06:58.000000 kss-6.0.0/kss/_modules/safety/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.453649 kss-6.0.0/kss/_modules/sentences/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/sentences/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9334 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/sentences/embracing_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    22898 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/sentences/sentence_postprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6751 2024-03-31 07:55:02.000000 kss-6.0.0/kss/_modules/sentences/sentence_preprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2298 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/sentences/sentence_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    30242 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/sentences/sentence_splitter.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    13304 2024-03-31 20:36:14.000000 kss-6.0.0/kss/_modules/sentences/sentence_splitter_fast.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8322 2024-04-27 14:18:12.000000 kss-6.0.0/kss/_modules/sentences/split_sentences.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.453928 kss-6.0.0/kss/_modules/spacing/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 14:16:36.000000 kss-6.0.0/kss/_modules/spacing/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5539 2024-04-27 13:58:40.000000 kss-6.0.0/kss/_modules/spacing/correct_spacing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   296979 2024-04-27 02:42:16.000000 kss-6.0.0/kss/_modules/spacing/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.454394 kss-6.0.0/kss/_modules/summarization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/summarization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5603 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/summarization/summarize_sentences.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3396 2024-04-26 07:26:56.000000 kss-6.0.0/kss/_modules/summarization/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.455070 kss-6.0.0/kss/_utils/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_utils/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       66 2024-04-27 04:09:55.000000 kss-6.0.0/kss/_utils/api.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    10329 2024-03-31 07:46:03.000000 kss-6.0.0/kss/_utils/const.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1399 2024-04-21 19:08:53.000000 kss-6.0.0/kss/_utils/emojis.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      910 2024-04-23 08:15:52.000000 kss-6.0.0/kss/_utils/logger.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1001 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_utils/multiprocessing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    17275 2024-04-27 03:50:29.000000 kss-6.0.0/kss/_utils/sanity_checks.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.439392 kss-6.0.0/kss.egg-info/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   204750 2024-04-27 14:20:50.000000 kss-6.0.0/kss.egg-info/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6339 2024-04-27 14:20:50.000000 kss-6.0.0/kss.egg-info/SOURCES.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:20:50.000000 kss-6.0.0/kss.egg-info/dependency_links.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:04:55.000000 kss-6.0.0/kss.egg-info/not-zip-safe
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      136 2024-04-27 14:20:50.000000 kss-6.0.0/kss.egg-info/requires.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       32 2024-04-27 14:20:50.000000 kss-6.0.0/kss.egg-info/top_level.txt
--rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2024-04-27 14:20:50.457410 kss-6.0.0/setup.cfg
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6191 2024-04-27 09:17:01.000000 kss-6.0.0/setup.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.456879 kss-6.0.0/tests/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 02:40:08.000000 kss-6.0.0/tests/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1033 2024-04-27 09:25:57.000000 kss-6.0.0/tests/test_augmentation.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8258 2024-04-27 08:00:32.000000 kss-6.0.0/tests/test_collocation.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      250 2024-04-27 08:00:32.000000 kss-6.0.0/tests/test_g2p.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      238 2024-04-27 08:00:32.000000 kss-6.0.0/tests/test_hangulize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      747 2024-04-27 04:21:47.000000 kss-6.0.0/tests/test_hanja.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      978 2024-04-27 04:13:17.000000 kss-6.0.0/tests/test_jamo.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      442 2024-04-27 04:17:41.000000 kss-6.0.0/tests/test_josa.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3405 2024-04-27 04:17:41.000000 kss-6.0.0/tests/test_keywords.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-27 09:20:57.000000 kss-6.0.0/tests/test_morphemes.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    19148 2024-04-27 04:25:01.000000 kss-6.0.0/tests/test_paradigm.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    97981 2024-04-27 13:38:44.000000 kss-6.0.0/tests/test_preprocessing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      290 2024-04-27 07:33:52.000000 kss-6.0.0/tests/test_qwerty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      257 2024-04-27 07:39:43.000000 kss-6.0.0/tests/test_romanize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      313 2024-04-27 08:03:40.000000 kss-6.0.0/tests/test_safety.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      776 2024-04-27 07:56:55.000000 kss-6.0.0/tests/test_sentences.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      236 2024-04-27 08:00:32.000000 kss-6.0.0/tests/test_spacing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1966 2024-04-27 08:00:32.000000 kss-6.0.0/tests/test_summarization.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.550542 kss-6.0.0.dev0/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1569 2024-04-01 04:29:21.000000 kss-6.0.0.dev0/LICENSE
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      379 2024-04-28 13:40:34.000000 kss-6.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   159355 2024-04-28 13:41:19.550707 kss-6.0.0.dev0/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   158598 2024-04-27 15:21:43.000000 kss-6.0.0.dev0/README.md
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.526052 kss-6.0.0.dev0/bench/
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.530930 kss-6.0.0.dev0/bench/sentence_split/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4379 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/sentence_split.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      615 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/test_baseline.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      600 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/test_kiwi.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1015 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/test_koalanlp.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      700 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/test_kss.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      587 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/test_word_split.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.531329 kss-6.0.0.dev0/csrc/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2024-03-31 20:12:01.000000 kss-6.0.0.dev0/csrc/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      563 2024-03-31 20:36:14.000000 kss-6.0.0.dev0/csrc/kss_cython.pyx
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5965 2024-03-31 20:12:01.000000 kss-6.0.0.dev0/csrc/sentence_splitter.cpp
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7830 2024-03-31 20:12:01.000000 kss-6.0.0.dev0/csrc/sentence_splitter.h
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.531426 kss-6.0.0.dev0/kss/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6884 2024-04-28 13:41:15.000000 kss-6.0.0.dev0/kss/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.532462 kss-6.0.0.dev0/kss/_elements/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_elements/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4888 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_elements/element.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2702 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_elements/empty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      536 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_elements/subclasses.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.532558 kss-6.0.0.dev0/kss/_modules/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.533024 kss-6.0.0.dev0/kss/_modules/augmentation/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/augmentation/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.533134 kss-6.0.0.dev0/kss/_modules/augmentation/assets/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)  4865459 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/augmentation/assets/wordnet.json
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3892 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/augmentation/augment.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3251 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/augmentation/distance.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3602 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/augmentation/replacement.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1411 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/augmentation/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.535905 kss-6.0.0.dev0/kss/_modules/collocation/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/collocation/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9351 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/collocation/collocate.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.537083 kss-6.0.0.dev0/kss/_modules/g2p/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.537396 kss-6.0.0.dev0/kss/_modules/g2p/assets/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2634 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/assets/idioms.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    14802 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/assets/rules.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5390 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/assets/table.csv
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6586 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/english.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7184 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/g2p.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4459 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/numerals.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2722 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/regular.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4949 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/special.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8131 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.537576 kss-6.0.0.dev0/kss/_modules/hangulization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3616 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulization.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538120 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2277 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    10423 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/hangul.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538231 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1426 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538335 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/aze/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5272 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/aze/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538437 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/bel/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5425 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/bel/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538563 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/bul/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4925 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/bul/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538674 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/cat/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4328 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/cat/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538784 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ces/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4820 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ces/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538886 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/cym/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5791 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/cym/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538998 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/deu/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7415 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/deu/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539159 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ell/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9068 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ell/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539265 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/epo/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4103 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/epo/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539370 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/est/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3931 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/est/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539465 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/fin/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3410 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/fin/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539564 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/grc/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8626 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/grc/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539664 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/hbs/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5606 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539768 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/hun/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4990 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/hun/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539868 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/isl/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5626 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/isl/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539965 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ita/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4371 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ita/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540064 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/jpn/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4446 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540264 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6118 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6408 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/narrow.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540369 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lat/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3314 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lat/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540485 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lav/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4116 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lav/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540581 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lit/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4080 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lit/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540680 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/mkd/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5354 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540780 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/nld/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    22064 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/nld/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540925 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/pol/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5785 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/pol/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541148 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/por/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6048 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/por/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/por/br.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541251 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ron/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5120 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ron/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541350 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/rus/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4994 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/rus/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541472 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/slk/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6693 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/slk/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541610 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/slv/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3836 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/slv/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541745 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/spa/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4002 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/spa/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541844 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/sqi/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3177 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541953 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/swe/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7896 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/swe/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.542078 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/tur/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3528 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/tur/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.542176 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ukr/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5072 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.542293 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/vie/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4742 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/vie/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.542412 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/wlm/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5599 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    16108 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/models.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1069 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/normalization.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2897 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/processing.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.542705 kss-6.0.0.dev0/kss/_modules/hanja/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hanja/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4462 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hanja/_hanja.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2021 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hanja/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.542998 kss-6.0.0.dev0/kss/_modules/jamo/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/jamo/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    12624 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/jamo/_jamo.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      912 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/jamo/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.543280 kss-6.0.0.dev0/kss/_modules/josa/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/josa/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2580 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/josa/josa.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7030 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/josa/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.543584 kss-6.0.0.dev0/kss/_modules/keywords/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/keywords/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6362 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/keywords/extract_keywords.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    17289 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/keywords/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.544046 kss-6.0.0.dev0/kss/_modules/morphemes/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/morphemes/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2652 2024-03-31 13:42:10.000000 kss-6.0.0.dev0/kss/_modules/morphemes/analyzers.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1849 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/morphemes/split_morphemes.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3588 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/morphemes/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.544245 kss-6.0.0.dev0/kss/_modules/paradigm/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/paradigm/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    18316 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/paradigm/paradigm.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.545329 kss-6.0.0.dev0/kss/_modules/preprocessing/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    15538 2024-04-27 14:56:06.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/anonymize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    29795 2024-04-27 14:58:49.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/clean_news.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    81165 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/completed_form.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    24570 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/filter_out.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2088 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/half2full.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/normalize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    26257 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/preprocess.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7186 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/reduce_repeats.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7661 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/remove_invisible_chars.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.545623 kss-6.0.0.dev0/kss/_modules/qwerty/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/qwerty/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6262 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/qwerty/qwerty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5941 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/qwerty/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.545923 kss-6.0.0.dev0/kss/_modules/romanization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/romanization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5813 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/romanization/romanize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8901 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/romanization/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.546214 kss-6.0.0.dev0/kss/_modules/safety/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/safety/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3531 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/safety/check_safety.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    35374 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/safety/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.547078 kss-6.0.0.dev0/kss/_modules/sentences/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/sentences/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9334 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/sentences/embracing_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    22898 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/sentences/sentence_postprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6751 2024-03-31 07:55:02.000000 kss-6.0.0.dev0/kss/_modules/sentences/sentence_preprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2298 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/sentences/sentence_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    30242 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/sentences/sentence_splitter.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    13304 2024-03-31 20:36:14.000000 kss-6.0.0.dev0/kss/_modules/sentences/sentence_splitter_fast.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8322 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/sentences/split_sentences.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.547353 kss-6.0.0.dev0/kss/_modules/spacing/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/spacing/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5539 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/spacing/correct_spacing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   296979 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/spacing/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.547822 kss-6.0.0.dev0/kss/_modules/summarization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/summarization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5603 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/summarization/summarize_sentences.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3396 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/summarization/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.548513 kss-6.0.0.dev0/kss/_utils/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_utils/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       66 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_utils/api.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    10329 2024-03-31 07:46:03.000000 kss-6.0.0.dev0/kss/_utils/const.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1399 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_utils/emojis.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      910 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_utils/logger.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1001 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_utils/multiprocessing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    17275 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_utils/sanity_checks.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.532072 kss-6.0.0.dev0/kss.egg-info/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   159355 2024-04-28 13:41:19.000000 kss-6.0.0.dev0/kss.egg-info/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6374 2024-04-28 13:41:19.000000 kss-6.0.0.dev0/kss.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-28 13:41:19.000000 kss-6.0.0.dev0/kss.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:04:55.000000 kss-6.0.0.dev0/kss.egg-info/not-zip-safe
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      136 2024-04-28 13:41:19.000000 kss-6.0.0.dev0/kss.egg-info/requires.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       32 2024-04-28 13:41:19.000000 kss-6.0.0.dev0/kss.egg-info/top_level.txt
+-rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2024-04-28 13:41:19.550940 kss-6.0.0.dev0/setup.cfg
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6191 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/setup.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.550448 kss-6.0.0.dev0/tests/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1033 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_augmentation.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8258 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_collocation.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      250 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_g2p.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      238 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_hangulize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      747 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_hanja.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      978 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_jamo.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      442 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_josa.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3405 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_keywords.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_morphemes.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    19148 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_paradigm.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    97981 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_preprocessing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      290 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_qwerty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      257 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_romanize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      313 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_safety.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      776 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_sentences.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      236 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_spacing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1966 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_summarization.py
```

### Comparing `kss-6.0.0/LICENSE` & `kss-6.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/PKG-INFO` & `kss-6.0.0.dev0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,13 @@
-Metadata-Version: 2.1
-Name: kss
-Version: 6.0.0
-Summary: A Toolkit for Korean sentence segmentation
-Home-page: https://github.com/hyunwoongko/kss
-Author: Hyunwoong Ko
-Author-email: kevin.brain@kakaobrain.com
-License: BSD 3-Clause "New" or "Revised" License
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">
 KSS: Korean String processing Suite
 </h1>
 
 <p align="center">
-    <a href="https://github.com/hyunwoongko/kss/releases">
-        <img alt="GitHub release" src="https://img.shields.io/github/release/hyunwoongko/kss.svg">
-    </a> 
-    <a href="https://github.com/hyunwoongko/kss/issues">
-        <img alt="Issues" src="https://img.shields.io/github/issues/hyunwoongko/kss">
-    </a>
-    <a href="https://github.com/hyunwoongko/kss/actions">
-        <img alt="Tests on Ubuntu" src="https://github.com/hyunwoongko/kss/actions/workflows/test_ubuntu.yaml/badge.svg">
-    </a>
-    <a href="https://github.com/hyunwoongko/kss/actions">
-        <img alt="Tests on MacOS" src="https://github.com/hyunwoongko/kss/actions/workflows/test_macos.yaml/badge.svg">
-    </a>
-    <a href="https://github.com/hyunwoongko/kss/actions">
-        <img alt="Tests on Windows" src="https://github.com/hyunwoongko/kss/actions/workflows/test_windows.yaml/badge.svg">
-    </a>
+    <a href="https://github.com/hyunwoongko/kss/releases"><img alt="GitHub release" src="https://img.shields.io/github/release/hyunwoongko/kss.svg"></a> <a href="https://github.com/hyunwoongko/kss/issues"><img alt="Issues" src="https://img.shields.io/github/issues/hyunwoongko/kss"></a> <a href="https://github.com/hyunwoongko/kss/actions"><img alt="Tests on Ubuntu" src="https://github.com/hyunwoongko/kss/actions/workflows/test_ubuntu.yaml/badge.svg"></a> <a href="https://github.com/hyunwoongko/kss/actions"><img alt="Tests on MacOS" src="https://github.com/hyunwoongko/kss/actions/workflows/test_macos.yaml/badge.svg"></a> <a href="https://github.com/hyunwoongko/kss/actions"><img alt="Tests on Windows" src="https://github.com/hyunwoongko/kss/actions/workflows/test_windows.yaml/badge.svg"></a>
 </p>
 
 
 KSS is a Korean string processing suite that provides various functions for processing Korean strings. It is designed to be simple and easy to use, and it is designed to be used in various fields such as natural language processing, data preprocessing, and data analysis.
 
 ### What's New:
 - April 27, 2024 [Released Kss 6.0 Python](https://github.com/hyunwoongko/kss/releases/tag/6.0.0).
@@ -119,15 +84,15 @@
     >>> text = "회사 동료 분들과 다녀왔는데 분위기도 좋고 음식도 맛있었어요 다만, 강남 토끼정이 강남 쉑쉑버거 골목길로 쭉 올라가야 하는데 다들 쉑쉑버거의 유혹에 넘어갈 뻔 했답니다 강남역 맛집 토끼정의 외부 모습."
     >>> split_sentences(text)
     ['회사 동료 분들과 다녀왔는데 분위기도 좋고 음식도 맛있었어요', '다만, 강남 토끼정이 강남 쉑쉑버거 골목길로 쭉 올라가야 하는데 다들 쉑쉑버거의 유혹에 넘어갈 뻔 했답니다', '강남역 맛집 토끼정의 외부 모습.']
 ```
 ### 4. Multiprocessing
 If you input a list of strings, Kss will automatically use multiprocessing to process the strings in parallel.
 And you can set the number of processes to use by setting the `num_workers` parameter.
-If you input `num_workers<2`, Kss will not use multiprocessing.
+If you input `num_workers < 2`, Kss will not use multiprocessing.
 
 ```python
 from kss import Kss
 
 module = Kss("MODULE_NAME")
 
 # using all cores
@@ -802,15 +767,16 @@
 
 References:
 - This was copied from [KoParadigm](https://github.com/Kyubyong/KoParadigm) and modified by Kss
 </details>
 
 <details>
 <summary>24. anonymize</summary>
-Anonymize sensitive information in the given text.
+
+This anonymizes sensitive information in the given text.
 
 Args:
 - text (`Union[str, List[str], Tuple[str]`): single text or list of texts
 - phone_number_anonymization (`bool`): whether to anonymize phone numbers or not
 - rrn_anonymization (`bool`): whether to anonymize resident registration numbers or not
 - card_anonymization (`bool`): whether to anonymize card numbers or not
 - email_anonymization (`bool`): whether to anonymize email addresses or not
@@ -846,15 +812,16 @@
 >>> print(output)
 "제 전화번호는 <PHONE_NUMBER>, 이메일 주소는 <EMAIL>입니다."
 ```
 </details>
 
 <details>
 <summary>25. clean_news</summary>
-Clean news articles by removing useless headers and footers.
+
+This cleans news articles by removing useless headers and footers.
 
 Args:
 - text (`Union[str, List[str], Tuple[str]]`): Input text or list of texts.
 - min_sentences (`int`): Minimum number of sentences to keep. Defaults to 3.
 - header_ratio (`float`): Ratio of the number of sentences to check in the header. Defaults to 0.4.
 - footer_ratio (`float`): Ratio of the number of sentences to check in the footer. Defaults to 0.4.
 - num_workers (`Union[int, str]`): the number of multiprocessing workers
@@ -900,36 +867,36 @@
 False
 ```
 </details>
 
 <details>
 <summary>27. get_all_completed_form_hangul_chars</summary>
 
-This returns all non-completed form Hangul characters.
+This returns all completed form Hangul characters.
 
 Returns:
-- `List[str]`: all non-completed form Hangul characters
+- `List[str]`: all completed form Hangul characters
 
 Examples:
 ```python
 >>> from kss import Kss
->>> get_all_incompleted_form_hangul_chars = Kss("get_all_incompleted_form_hangul_chars")
->>> output = get_all_incompleted_form_hangul_chars()
+>>> get_all_completed_form_hangul_chars = Kss("get_all_completed_form_hangul_chars")
+>>> output = get_all_completed_form_hangul_chars()
 >>> print(output)
-['갂', '갃', '갅', '갆', '갋', '갌', '갍', '갎', '갏', '갘', '갞', '갟', '갡', '갢', '갣', '갥', '갦', '갧', '갨', '갩', '갪', '갫', '갮', '갲', '갳', '갴', '갵', '갶', '갷', '갺', '갻', '갽', '갾', '갿', '걁', '걂', '걃', '걄', '걅', '걆', '걇', '걈', '걉', '걊', '걌', '걎', '걏', '걐', '걑', '걒', '걓', '걕', '걖', '걗', '걙', '걚', '걛', '걝', '걞', '걟', '걠', '걡', '걢', '걣', '걤', '걥', '걦', '걧', '걨', '걩', '걪', '걫', '걬', '걭', '걮', '걯', '걲', '걳', '걵', '걶', '걹', '걻', '걼', '걽', '걾', '걿', '겂', '겇', '겈', '겍', '겎', '겏', '겑', '겒', '겓', '겕', '겖', '겗', '겘', '겙', '겚', '겛', '겞', '겢', '겣', '겤', '겥', '겦', '겧', '겫', '겭', '겮', '겱', '겲', '겳', '겴', '겵', '겶', '겷', '겺', '겾', '겿', '곀', '곂', '곃', '곅', '곆', '곇', '곉', '곊', '곋', '곍', '곎', '곏', '곐', '곑', '곒', '곓', '곔', '곖', '곘', '곙', '곚', '곛', '곜', '곝', '곞', '곟', '곢', '곣', '곥', '곦', '곩', '곫', '곭', '곮', '곲', '곴', '곷', '곸', '곹', '곺', '곻', '곾', '곿', '괁', '괂', '괃', '괅', '괇', '괈', '괉', '괊', '괋', '괎', '괐', '괒', '괓', '괔', '괕', '괖', '괗', '괙', '괚', '괛', '괝', '괞', '괟', '괡', '괢', '괣', '괤', '괥', '괦', '괧', '괨', '괪', '괫', '괮', '괯', '괰', '괱', '괲', '괳', '괶', '괷', '괹', '괺', '괻', '괽', '괾', '괿', '굀', '굁', '굂', '굃', '굆', '굈', '굊', '굋', '굌', '굍', '굎', '굏', '굑', '굒', '굓', '굕', '굖', '굗', '굙', '굚', '굛', '굜', '굝', '굞', '굟', '굠', '굢', '굤', '굥', '굦', '굧', '굨', '굩', '굪', '굫', '굮', '굯', '굱', '굲', '굷', '굸', '굹', '굺', '굾', '궀', '궃', '궄', '궅', '궆', '궇', '궊', '궋', '궍', '궎', '궏', '궑', '궒', '궓', '궔', '궕', '궖', '궗', '궘', '궙', '궚', '궛', '궞', '궟', '궠', '궡', '궢', '궣', '궥', '궦', '궧', '궨', '궩', '궪', '궫', '궬', '궭', '궮', '궯', '궰', '궱', '궲', '궳', '궴', '궵', '궶', '궸', '궹', '궺', '궻', '궼', '궽', '궾', '궿', '귂', '귃', '귅', '귆', '귇', '귉', '귊', '귋', '귌', '귍', '귎', '귏', '귒', '귔', '귕', '귖', '귗', '귘', '귙', '귚', '귛', '귝', '귞', '귟', '귡', '귢', '귣', '귥', '귦', '귧', '귨', '귩', '귪', '귫', '귬', '귭', '귮', '귯', '귰', '귱', '귲', '귳', '귴', '귵', '귶', '귷', '귺', '귻', '귽', '귾', '긂', '긃', '긄', '긅', '긆', '긇', '긊', '긌', '긎', '긏', '긐', '긑', '긒', '긓', '긕', '긖', '긗', '긘', '긙', '긚', '긛', '긜', '긝', '긞', '긟', '긠', '긡', '긢', '긣', '긤', '긥', '긦', '긧', '긨', '긩', '긪', '긫', '긬', '긭', '긮', '긯', '긲', '긳', '긵', '긶', '긹', '긻', '긼', '긽', '긾', '긿', '깂', '깄', '깇', '깈', '깉', '깋', '깏', '깑', '깒', '깓', '깕', '깗', '깘', '깙', '깚', '깛', '깞', '깢', '깣', '깤', '깦', '깧', '깪', '깫', '깭', '깮', '깯', '깱', '깲', '깳', '깴', '깵', '깶', '깷', '깺', '깾', '깿', '꺀', '꺁', '꺂', '꺃', '꺆', '꺇', '꺈', '꺉', '꺊', '꺋', '꺍', '꺎', '꺏', '꺐', '꺑', '꺒', '꺓', '꺔', '꺕', '꺖', '꺗', '꺘', '꺙', '꺚', '꺛', '꺜', '꺝', '꺞', '꺟', '꺠', '꺡', '꺢', '꺣', '꺤', '꺥', '꺦', '꺧', '꺨', '꺩', '꺪', '꺫', '꺬', '꺭', '꺮', '꺯', '꺰', '꺱', '꺲', '꺳', '꺴', '꺵', '꺶', '꺷', '꺸', '꺹', '꺺', '꺻', '꺿', '껁', '껂', '껃', '껅', '껆', '껇', '껈', '껉', '껊', '껋', '껎', '껒', '껓', '껔', '껕', '껖', '껗', '껚', '껛', '껝', '껞', '껟', '껠', '껡', '껢', '껣', '껤', '껥', '껦', '껧', '껩', '껪', '껬', '껮', '껯', '껰', '껱', '껲', '껳', '껵', '껶', '껷', '껹', '껺', '껻', '껽', '껾', '껿', '꼀', '꼁', '꼂', '꼃', '꼄', '꼅', '꼆', '꼉', '꼊', '꼋', '꼌', '꼎', '꼏', '꼑', '꼒', '꼓', '꼔', '꼕', '꼖', '꼗', '꼘', '꼙', '꼚', '꼛', '꼜', '꼝', '꼞', '꼟', '꼠', '꼡', '꼢', '꼣', '꼤', '꼥', '꼦', '꼧', '꼨', '꼩', '꼪', '꼫', '꼮', '꼯', '꼱', '꼳', '꼵', '꼶', '꼷', '꼸', '꼹', '꼺', '꼻', '꼾', '꽀', '꽄', '꽅', '꽆', '꽇', '꽊', '꽋', '꽌', '꽍', '꽎', '꽏', '꽑', '꽒', '꽓', '꽔', '꽕', '꽖', '꽗', '꽘', '꽙', '꽚', '꽛', '꽞', '꽟', '꽠', '꽡', '꽢', '꽣', '꽦', '꽧', '꽨', '꽩', '꽪', '꽫', '꽬', '꽭', '꽮', '꽯', '꽰', '꽱', '꽲', '꽳', '꽴', '꽵', '꽶', '꽷', '꽸', '꽺', '꽻', '꽼', '꽽', '꽾', '꽿', '꾁', '꾂', '꾃', '꾅', '꾆', '꾇', '꾉', '꾊', '꾋', '꾌', '꾍', '꾎', '꾏', '꾒', '꾓', '꾔', '꾖', '꾗', '꾘', '꾙', '꾚', '꾛', '꾝', '꾞', '꾟', '꾠', '꾡', '꾢', '꾣', '꾤', '꾥', '꾦', '꾧', '꾨', '꾩', '꾪', '꾫', '꾬', '꾭', '꾮', '꾯', '꾰', '꾱', '꾲', '꾳', '꾴', '꾵', '꾶', '꾷', '꾺', '꾻', '꾽', '꾾', '꾿', '꿁', '꿂', '꿃', '꿄', '꿅', '꿆', '꿊', '꿌', '꿏', '꿐', '꿑', '꿒', '꿓', '꿕', '꿖', '꿗', '꿘', '꿙', '꿚', '꿛', '꿝', '꿞', '꿟', '꿠', '꿡', '꿢', '꿣', '꿤', '꿥', '꿦', '꿧', '꿪', '꿫', '꿬', '꿭', '꿮', '꿯', '꿲', '꿳', '꿵', '꿶', '꿷', '꿹', '꿺', '꿻', '꿼', '꿽', '꿾', '꿿', '뀂', '뀃', '뀅', '뀆', '뀇', '뀈', '뀉', '뀊', '뀋', '뀍', '뀎', '뀏', '뀑', '뀒', '뀓', '뀕', '뀖', '뀗', '뀘', '뀙', '뀚', '뀛', '뀞', '뀟', '뀠', '뀡', '뀢', '뀣', '뀤', '뀥', '뀦', '뀧', '뀩', '뀪', '뀫', '뀬', '뀭', '뀮', '뀯', '뀰', '뀱', '뀲', '뀳', '뀴', '뀵', '뀶', '뀷', '뀸', '뀹', '뀺', '뀻', '뀼', '뀽', '뀾', '뀿', '끀', '끁', '끂', '끃', '끆', '끇', '끉', '끋', '끍', '끏', '끐', '끑', '끒', '끖', '끘', '끚', '끛', '끜', '끞', '끟', '끠', '끡', '끢', '끣', '끤', '끥', '끦', '끧', '끨', '끩', '끪', '끫', '끬', '끭', '끮', '끯', '끰', '끱', '끲', '끳', '끴', '끵', '끶', '끷', '끸', '끹', '끺', '끻', '끾', '끿', '낁', '낂', '낃', '낅', '낆', '낇', '낈', '낉', '낊', '낋', '낎', '낐', '낒', '낓', '낔', '낕', '낖', '낗', '낛', '낝', '낞', '낣', '낤', '낥', '낦', '낧', '낪', '낰', '낲', '낶', '낷', '낹', '낺', '낻', '낽', '낾', '낿', '냀', '냁', '냂', '냃', '냆', '냊', '냋', '냌', '냍', '냎', '냏', '냒', '냓', '냕', '냖', '냗', '냙', '냚', '냛', '냜', '냝', '냞', '냟', '냡', '냢', '냣', '냤', '냦', '냧', '냨', '냩', '냪', '냫', '냬', '냭', '냮', '냯', '냰', '냱', '냲', '냳', '냴', '냵', '냶', '냷', '냸', '냹', '냺', '냻', '냼', '냽', '냾', '냿', '넀', '넁', '넂', '넃', '넄', '넅', '넆', '넇', '넊', '넍', '넎', '넏', '넑', '넔', '넕', '넖', '넗', '넚', '넞', '넟', '넠', '넡', '넢', '넦', '넧', '넩', '넪', '넫', '넭', '넮', '넯', '넰', '넱', '넲', '넳', '넶', '넺', '넻', '넼', '넽', '넾', '넿', '녂', '녃', '녅', '녆', '녇', '녉', '녊', '녋', '녌', '녍', '녎', '녏', '녒', '녓', '녖', '녗', '녙', '녚', '녛', '녝', '녞', '녟', '녡', '녢', '녣', '녤', '녥', '녦', '녧', '녨', '녩', '녪', '녫', '녬', '녭', '녮', '녯', '녰', '녱', '녲', '녳', '녴', '녵', '녶', '녷', '녺', '녻', '녽', '녾', '녿', '놁', '놃', '놄', '놅', '놆', '놇', '놊', '놌', '놎', '놏', '놐', '놑', '놕', '놖', '놗', '놙', '놚', '놛', '놝', '놞', '놟', '놠', '놡', '놢', '놣', '놤', '놥', '놦', '놧', '놩', '놪', '놫', '놬', '놭', '놮', '놯', '놰', '놱', '놲', '놳', '놴', '놵', '놶', '놷', '놸', '놹', '놺', '놻', '놼', '놽', '놾', '놿', '뇀', '뇁', '뇂', '뇃', '뇄', '뇅', '뇆', '뇇', '뇈', '뇉', '뇊', '뇋', '뇍', '뇎', '뇏', '뇑', '뇒', '뇓', '뇕', '뇖', '뇗', '뇘', '뇙', '뇚', '뇛', '뇞', '뇠', '뇡', '뇢', '뇣', '뇤', '뇥', '뇦', '뇧', '뇪', '뇫', '뇭', '뇮', '뇯', '뇱', '뇲', '뇳', '뇴', '뇵', '뇶', '뇷', '뇸', '뇺', '뇼', '뇾', '뇿', '눀', '눁', '눂', '눃', '눆', '눇', '눉', '눊', '눍', '눎', '눏', '눐', '눑', '눒', '눓', '눖', '눘', '눚', '눛', '눜', '눝', '눞', '눟', '눡', '눢', '눣', '눤', '눥', '눦', '눧', '눨', '눩', '눪', '눫', '눬', '눭', '눮', '눯', '눰', '눱', '눲', '눳', '눵', '눶', '눷', '눸', '눹', '눺', '눻', '눽', '눾', '눿', '뉀', '뉁', '뉂', '뉃', '뉄', '뉅', '뉆', '뉇', '뉈', '뉉', '뉊', '뉋', '뉌', '뉍', '뉎', '뉏', '뉐', '뉑', '뉒', '뉓', '뉔', '뉕', '뉖', '뉗', '뉙', '뉚', '뉛', '뉝', '뉞', '뉟', '뉡', '뉢', '뉣', '뉤', '뉥', '뉦', '뉧', '뉪', '뉫', '뉬', '뉭', '뉮', '뉯', '뉰', '뉱', '뉲', '뉳', '뉶', '뉷', '뉸', '뉹', '뉺', '뉻', '뉽', '뉾', '뉿', '늀', '늁', '늂', '늃', '늆', '늇', '늈', '늊', '늋', '늌', '늍', '늎', '늏', '늒', '늓', '늕', '늖', '늗', '늛', '늜', '늝', '늞', '늟', '늢', '늤', '늧', '늨', '늩', '늫', '늭', '늮', '늯', '늱', '늲', '늳', '늵', '늶', '늷', '늸', '늹', '늺', '늻', '늼', '늽', '늾', '늿', '닀', '닁', '닂', '닃', '닄', '닅', '닆', '닇', '닊', '닋', '닍', '닎', '닏', '닑', '닓', '닔', '닕', '닖', '닗', '닚', '닜', '닞', '닟', '닠', '닡', '닣', '닧', '닩', '닪', '닰', '닱', '닲', '닶', '닼', '닽', '닾', '댂', '댃', '댅', '댆', '댇', '댉', '댊', '댋', '댌', '댍', '댎', '댏', '댒', '댖', '댗', '댘', '댙', '댚', '댛', '댝', '댞', '댟', '댠', '댡', '댢', '댣', '댤', '댥', '댦', '댧', '댨', '댩', '댪', '댫', '댬', '댭', '댮', '댯', '댰', '댱', '댲', '댳', '댴', '댵', '댶', '댷', '댸', '댹', '댺', '댻', '댼', '댽', '댾', '댿', '덀', '덁', '덂', '덃', '덄', '덅', '덆', '덇', '덈', '덉', '덊', '덋', '덌', '덍', '덎', '덏', '덐', '덑', '덒', '덓', '덗', '덙', '덚', '덝', '덠', '덡', '덢', '덣', '덦', '덨', '덪', '덬', '덭', '덯', '덲', '덳', '덵', '덶', '덷', '덹', '덺', '덻', '덼', '덽', '덾', '덿', '뎂', '뎆', '뎇', '뎈', '뎉', '뎊', '뎋', '뎍', '뎎', '뎏', '뎑', '뎒', '뎓', '뎕', '뎖', '뎗', '뎘', '뎙', '뎚', '뎛', '뎜', '뎝', '뎞', '뎟', '뎢', '뎣', '뎤', '뎥', '뎦', '뎧', '뎩', '뎪', '뎫', '뎭', '뎮', '뎯', '뎰', '뎱', '뎲', '뎳', '뎴', '뎵', '뎶', '뎷', '뎸', '뎹', '뎺', '뎻', '뎼', '뎽', '뎾', '뎿', '돀', '돁', '돂', '돃', '돆', '돇', '돉', '돊', '돍', '돏', '돑', '돒', '돓', '돖', '돘', '돚', '돜', '돞', '돟', '돡', '돢', '돣', '돥', '돦', '돧', '돩', '돪', '돫', '돬', '돭', '돮', '돯', '돰', '돱', '돲', '돳', '돴', '돵', '돶', '돷', '돸', '돹', '돺', '돻', '돽', '돾', '돿', '됀', '됁', '됂', '됃', '됄', '됅', '됆', '됇', '됈', '됉', '됊', '됋', '됌', '됍', '됎', '됏', '됑', '됒', '됓', '됔', '됕', '됖', '됗', '됙', '됚', '됛', '됝', '됞', '됟', '됡', '됢', '됣', '됤', '됥', '됦', '됧', '됪', '됬', '됭', '됮', '됯', '됰', '됱', '됲', '됳', '됵', '됶', '됷', '됸', '됹', '됺', '됻', '됼', '됽', '됾', '됿', '둀', '둁', '둂', '둃', '둄', '둅', '둆', '둇', '둈', '둉', '둊', '둋', '둌', '둍', '둎', '둏', '둒', '둓', '둕', '둖', '둗', '둙', '둚', '둛', '둜', '둝', '둞', '둟', '둢', '둤', '둦', '둧', '둨', '둩', '둪', '둫', '둭', '둮', '둯', '둰', '둱', '둲', '둳', '둴', '둵', '둶', '둷', '둸', '둹', '둺', '둻', '둼', '둽', '둾', '둿', '뒁', '뒂', '뒃', '뒄', '뒅', '뒆', '뒇', '뒉', '뒊', '뒋', '뒌', '뒍', '뒎', '뒏', '뒐', '뒑', '뒒', '뒓', '뒔', '뒕', '뒖', '뒗', '뒘', '뒙', '뒚', '뒛', '뒜', '뒞', '뒟', '뒠', '뒡', '뒢', '뒣', '뒥', '뒦', '뒧', '뒩', '뒪', '뒫', '뒭', '뒮', '뒯', '뒰', '뒱', '뒲', '뒳', '뒴', '뒶', '뒸', '뒺', '뒻', '뒼', '뒽', '뒾', '뒿', '듁', '듂', '듃', '듅', '듆', '듇', '듉', '듊', '듋', '듌', '듍', '듎', '듏', '듑', '듒', '듓', '듔', '듖', '듗', '듘', '듙', '듚', '듛', '듞', '듟', '듡', '듢', '듥', '듧', '듨', '듩', '듪', '듫', '듮', '듰', '듲', '듳', '듴', '듵', '듶', '듷', '듹', '듺', '듻', '듼', '듽', '듾', '듿', '딀', '딁', '딂', '딃', '딄', '딅', '딆', '딇', '딈', '딉', '딊', '딋', '딌', '딍', '딎', '딏', '딐', '딑', '딒', '딓', '딖', '딗', '딙', '딚', '딝', '딞', '딟', '딠', '딡', '딢', '딣', '딦', '딫', '딬', '딭', '딮', '딯', '딲', '딳', '딵', '딶', '딷', '딹', '딺', '딻', '딼', '딽', '딾', '딿', '땂', '땆', '땇', '땈', '땉', '땊', '땎', '땏', '땑', '땒', '땓', '땕', '땖', '땗', '땘', '땙', '땚', '땛', '땞', '땢', '땣', '땤', '땥', '땦', '땧', '땨', '땩', '땪', '땫', '땬', '땭', '땮', '땯', '땰', '땱', '땲', '땳', '땴', '땵', '땶', '땷', '땸', '땹', '땺', '땻', '땼', '땽', '땾', '땿', '떀', '떁', '떂', '떃', '떄', '떅', '떆', '떇', '떈', '떉', '떊', '떋', '떌', '떍', '떎', '떏', '떐', '떑', '떒', '떓', '떔', '떕', '떖', '떗', '떘', '떙', '떚', '떛', '떜', '떝', '떞', '떟', '떢', '떣', '떥', '떦', '떧', '떩', '떬', '떭', '떮', '떯', '떲', '떶', '떷', '떸', '떹', '떺', '떾', '떿', '뗁', '뗂', '뗃', '뗅', '뗆', '뗇', '뗈', '뗉', '뗊', '뗋', '뗎', '뗒', '뗓', '뗔', '뗕', '뗖', '뗗', '뗙', '뗚', '뗛', '뗜', '뗝', '뗞', '뗟', '뗠', '뗡', '뗢', '뗣', '뗤', '뗥', '뗦', '뗧', '뗨', '뗩', '뗪', '뗫', '뗭', '뗮', '뗯', '뗰', '뗱', '뗲', '뗳', '뗴', '뗵', '뗶', '뗷', '뗸', '뗹', '뗺', '뗻', '뗼', '뗽', '뗾', '뗿', '똀', '똁', '똂', '똃', '똄', '똅', '똆', '똇', '똈', '똉', '똊', '똋', '똌', '똍', '똎', '똏', '똒', '똓', '똕', '똖', '똗', '똙', '똚', '똛', '똜', '똝', '똞', '똟', '똠', '똡', '똢', '똣', '똤', '똦', '똧', '똨', '똩', '똪', '똫', '똭', '똮', '똯', '똰', '똱', '똲', '똳', '똵', '똶', '똷', '똸', '똹', '똺', '똻', '똼', '똽', '똾', '똿', '뙀', '뙁', '뙂', '뙃', '뙄', '뙅', '뙆', '뙇', '뙉', '뙊', '뙋', '뙌', '뙍', '뙎', '뙏', '뙐', '뙑', '뙒', '뙓', '뙔', '뙕', '뙖', '뙗', '뙘', '뙙', '뙚', '뙛', '뙜', '뙝', '뙞', '뙟', '뙠', '뙡', '뙢', '뙣', '뙥', '뙦', '뙧', '뙩', '뙪', '뙫', '뙬', '뙭', '뙮', '뙯', '뙰', '뙱', '뙲', '뙳', '뙴', '뙵', '뙶', '뙷', '뙸', '뙹', '뙺', '뙻', '뙼', '뙽', '뙾', '뙿', '뚀', '뚁', '뚂', '뚃', '뚄', '뚅', '뚆', '뚇', '뚈', '뚉', '뚊', '뚋', '뚌', '뚍', '뚎', '뚏', '뚐', '뚑', '뚒', '뚓', '뚔', '뚕', '뚖', '뚗', '뚘', '뚙', '뚚', '뚛', '뚞', '뚟', '뚡', '뚢', '뚣', '뚥', '뚦', '뚧', '뚨', '뚩', '뚪', '뚭', '뚮', '뚯', '뚰', '뚲', '뚳', '뚴', '뚵', '뚶', '뚷', '뚸', '뚹', '뚺', '뚻', '뚼', '뚽', '뚾', '뚿', '뛀', '뛁', '뛂', '뛃', '뛄', '뛅', '뛆', '뛇', '뛈', '뛉', '뛊', '뛋', '뛌', '뛍', '뛎', '뛏', '뛐', '뛑', '뛒', '뛓', '뛕', '뛖', '뛗', '뛘', '뛙', '뛚', '뛛', '뛜', '뛝', '뛞', '뛟', '뛠', '뛡', '뛢', '뛣', '뛤', '뛥', '뛦', '뛧', '뛨', '뛩', '뛪', '뛫', '뛬', '뛭', '뛮', '뛯', '뛱', '뛲', '뛳', '뛵', '뛶', '뛷', '뛹', '뛺', '뛻', '뛼', '뛽', '뛾', '뛿', '뜂', '뜃', '뜄', '뜆', '뜇', '뜈', '뜉', '뜊', '뜋', '뜌', '뜍', '뜎', '뜏', '뜐', '뜑', '뜒', '뜓', '뜔', '뜕', '뜖', '뜗', '뜘', '뜙', '뜚', '뜛', '뜜', '뜝', '뜞', '뜟', '뜠', '뜡', '뜢', '뜣', '뜤', '뜥', '뜦', '뜧', '뜪', '뜫', '뜭', '뜮', '뜱', '뜲', '뜳', '뜴', '뜵', '뜶', '뜷', '뜺', '뜼', '뜽', '뜾', '뜿', '띀', '띁', '띂', '띃', '띅', '띆', '띇', '띉', '띊', '띋', '띍', '띎', '띏', '띐', '띑', '띒', '띓', '띖', '띗', '띘', '띙', '띚', '띛', '띜', '띝', '띞', '띟', '띡', '띢', '띣', '띥', '띦', '띧', '띩', '띪', '띫', '띬', '띭', '띮', '띯', '띲', '띴', '띶', '띷', '띸', '띹', '띺', '띻', '띾', '띿', '랁', '랂', '랃', '랅', '랆', '랇', '랈', '랉', '랊', '랋', '랎', '랓', '랔', '랕', '랚', '랛', '랝', '랞', '랟', '랡', '랢', '랣', '랤', '랥', '랦', '랧', '랪', '랮', '랯', '랰', '랱', '랲', '랳', '랶', '랷', '랹', '랺', '랻', '랼', '랽', '랾', '랿', '럀', '럁', '럂', '럃', '럄', '럅', '럆', '럈', '럊', '럋', '럌', '럍', '럎', '럏', '럐', '럑', '럒', '럓', '럔', '럕', '럖', '럗', '럘', '럙', '럚', '럛', '럜', '럝', '럞', '럟', '럠', '럡', '럢', '럣', '럤', '럥', '럦', '럧', '럨', '럩', '럪', '럫', '럮', '럯', '럱', '럲', '럳', '럵', '럶', '럷', '럸', '럹', '럺', '럻', '럾', '렂', '렃', '렄', '렅', '렆', '렊', '렋', '렍', '렎', '렏', '렑', '렒', '렓', '렔', '렕', '렖', '렗', '렚', '렜', '렞', '렟', '렠', '렡', '렢', '렣', '렦', '렧', '렩', '렪', '렫', '렭', '렮', '렯', '렰', '렱', '렲', '렳', '렶', '렺', '렻', '렼', '렽', '렾', '렿', '롁', '롂', '롃', '롅', '롆', '롇', '롈', '롉', '롊', '롋', '롌', '롍', '롎', '롏', '롐', '롒', '롔', '롕', '롖', '롗', '롘', '롙', '롚', '롛', '롞', '롟', '롡', '롢', '롣', '롥', '롦', '롧', '롨', '롩', '롪', '롫', '롮', '롰', '롲', '롳', '롴', '롵', '롶', '롷', '롹', '롺', '롻', '롽', '롾', '롿', '뢀', '뢁', '뢂', '뢃', '뢄', '뢅', '뢆', '뢇', '뢈', '뢉', '뢊', '뢋', '뢌', '뢎', '뢏', '뢐', '뢑', '뢒', '뢓', '뢔', '뢕', '뢖', '뢗', '뢘', '뢙', '뢚', '뢛', '뢜', '뢝', '뢞', '뢟', '뢠', '뢡', '뢢', '뢣', '뢤', '뢥', '뢦', '뢧', '뢩', '뢪', '뢫', '뢬', '뢭', '뢮', '뢯', '뢱', '뢲', '뢳', '뢵', '뢶', '뢷', '뢹', '뢺', '뢻', '뢼', '뢽', '뢾', '뢿', '룂', '룄', '룆', '룇', '룈', '룉', '룊', '룋', '룍', '룎', '룏', '룑', '룒', '룓', '룕', '룖', '룗', '룘', '룙', '룚', '룛', '룜', '룞', '룠', '룢', '룣', '룤', '룥', '룦', '룧', '룪', '룫', '룭', '룮', '룯', '룱', '룲', '룳', '룴', '룵', '룶', '룷', '룺', '룼', '룾', '룿', '뤀', '뤁', '뤂', '뤃', '뤅', '뤆', '뤇', '뤈', '뤉', '뤊', '뤋', '뤌', '뤍', '뤎', '뤏', '뤐', '뤑', '뤒', '뤓', '뤔', '뤕', '뤖', '뤗', '뤙', '뤚', '뤛', '뤜', '뤝', '뤞', '뤟', '뤡', '뤢', '뤣', '뤤', '뤥', '뤦', '뤧', '뤨', '뤩', '뤪', '뤫', '뤬', '뤭', '뤮', '뤯', '뤰', '뤱', '뤲', '뤳', '뤴', '뤵', '뤶', '뤷', '뤸', '뤹', '뤺', '뤻', '뤾', '뤿', '륁', '륂', '륃', '륅', '륆', '륇', '륈', '륉', '륊', '륋', '륍', '륎', '륐', '륒', '륓', '륔', '륕', '륖', '륗', '륚', '륛', '륝', '륞', '륟', '륡', '륢', '륣', '륤', '륥', '륦', '륧', '륪', '륬', '륮', '륯', '륰', '륱', '륲', '륳', '륶', '륷', '륹', '륺', '륻', '륽', '륾', '륿', '릀', '릁', '릂', '릃', '릆', '릈', '릋', '릌', '릏', '릐', '릑', '릒', '릓', '릔', '릕', '릖', '릗', '릘', '릙', '릚', '릛', '릜', '릝', '릞', '릟', '릠', '릡', '릢', '릣', '릤', '릥', '릦', '릧', '릨', '릩', '릪', '릫', '릮', '릯', '릱', '릲', '릳', '릵', '릶', '릷', '릸', '릹', '릺', '릻', '릾', '맀', '맂', '맃', '맄', '맅', '맆', '맇', '맊', '맋', '맍', '맓', '맔', '맕', '맖', '맗', '맚', '맜', '맟', '맠', '맢', '맦', '맧', '맩', '맪', '맫', '맭', '맮', '맯', '맰', '맱', '맲', '맳', '맶', '맻', '맼', '맽', '맾', '맿', '먂', '먃', '먄', '먅', '먆', '먇', '먉', '먊', '먋', '먌', '먍', '먎', '먏', '먐', '먑', '먒', '먓', '먔', '먖', '먗', '먘', '먙', '먚', '먛', '먜', '먝', '먞', '먟', '먠', '먡', '먢', '먣', '먤', '먥', '먦', '먧', '먨', '먩', '먪', '먫', '먬', '먭', '먮', '먯', '먰', '먱', '먲', '먳', '먴', '먵', '먶', '먷', '먺', '먻', '먽', '먾', '먿', '멁', '멃', '멄', '멅', '멆', '멇', '멊', '멌', '멏', '멐', '멑', '멒', '멖', '멗', '멙', '멚', '멛', '멝', '멞', '멟', '멠', '멡', '멢', '멣', '멦', '멪', '멫', '멬', '멭', '멮', '멯', '멲', '멳', '멵', '멶', '멷', '멹', '멺', '멻', '멼', '멽', '멾', '멿', '몀', '몁', '몂', '몆', '몈', '몉', '몊', '몋', '몍', '몎', '몏', '몐', '몑', '몒', '몓', '몔', '몕', '몖', '몗', '몘', '몙', '몚', '몛', '몜', '몝', '몞', '몟', '몠', '몡', '몢', '몣', '몤', '몥', '몦', '몧', '몪', '몭', '몮', '몯', '몱', '몳', '몴', '몵', '몶', '몷', '몺', '몼', '몾', '몿', '뫀', '뫁', '뫂', '뫃', '뫅', '뫆', '뫇', '뫉', '뫊', '뫋', '뫌', '뫍', '뫎', '뫏', '뫐', '뫑', '뫒', '뫓', '뫔', '뫕', '뫖', '뫗', '뫚', '뫛', '뫜', '뫝', '뫞', '뫟', '뫠', '뫡', '뫢', '뫣', '뫤', '뫥', '뫦', '뫧', '뫨', '뫩', '뫪', '뫫', '뫬', '뫭', '뫮', '뫯', '뫰', '뫱', '뫲', '뫳', '뫴', '뫵', '뫶', '뫷', '뫸', '뫹', '뫺', '뫻', '뫽', '뫾', '뫿', '묁', '묂', '묃', '묅', '묆', '묇', '묈', '묉', '묊', '묋', '묌', '묎', '묐', '묒', '묓', '묔', '묕', '묖', '묗', '묙', '묚', '묛', '묝', '묞', '묟', '묡', '묢', '묣', '묤', '묥', '묦', '묧', '묨', '묪', '묬', '묭', '묮', '묯', '묰', '묱', '묲', '묳', '묷', '묹', '묺', '묿', '뭀', '뭁', '뭂', '뭃', '뭆', '뭈', '뭊', '뭋', '뭌', '뭎', '뭑', '뭒', '뭓', '뭕', '뭖', '뭗', '뭙', '뭚', '뭛', '뭜', '뭝', '뭞', '뭟', '뭠', '뭢', '뭤', '뭥', '뭦', '뭧', '뭨', '뭩', '뭪', '뭫', '뭭', '뭮', '뭯', '뭰', '뭱', '뭲', '뭳', '뭴', '뭵', '뭶', '뭷', '뭸', '뭹', '뭺', '뭻', '뭼', '뭽', '뭾', '뭿', '뮀', '뮁', '뮂', '뮃', '뮄', '뮅', '뮆', '뮇', '뮉', '뮊', '뮋', '뮍', '뮎', '뮏', '뮑', '뮒', '뮓', '뮔', '뮕', '뮖', '뮗', '뮘', '뮙', '뮚', '뮛', '뮜', '뮝', '뮞', '뮟', '뮠', '뮡', '뮢', '뮣', '뮥', '뮦', '뮧', '뮩', '뮪', '뮫', '뮭', '뮮', '뮯', '뮰', '뮱', '뮲', '뮳', '뮵', '뮶', '뮸', '뮹', '뮺', '뮻', '뮼', '뮽', '뮾', '뮿', '믁', '믂', '믃', '믅', '믆', '믇', '믉', '믊', '믋', '믌', '믍', '믎', '믏', '믑', '믒', '믔', '믕', '믖', '믗', '믘', '믙', '믚', '믛', '믜', '믝', '믞', '믟', '믠', '믡', '믢', '믣', '믤', '믥', '믦', '믧', '믨', '믩', '믪', '믫', '믬', '믭', '믮', '믯', '믰', '믱', '믲', '믳', '믴', '믵', '믶', '믷', '믺', '믻', '믽', '믾', '밁', '밃', '밄', '밅', '밆', '밇', '밊', '밎', '밐', '밒', '밓', '밙', '밚', '밠', '밡', '밢', '밣', '밦', '밨', '밪', '밫', '밬', '밮', '밯', '밲', '밳', '밵', '밶', '밷', '밹', '밺', '밻', '밼', '밽', '밾', '밿', '뱂', '뱆', '뱇', '뱈', '뱊', '뱋', '뱎', '뱏', '뱑', '뱒', '뱓', '뱔', '뱕', '뱖', '뱗', '뱘', '뱙', '뱚', '뱛', '뱜', '뱞', '뱟', '뱠', '뱡', '뱢', '뱣', '뱤', '뱥', '뱦', '뱧', '뱨', '뱩', '뱪', '뱫', '뱬', '뱭', '뱮', '뱯', '뱰', '뱱', '뱲', '뱳', '뱴', '뱵', '뱶', '뱷', '뱸', '뱹', '뱺', '뱻', '뱼', '뱽', '뱾', '뱿', '벀', '벁', '벂', '벃', '벆', '벇', '벉', '벊', '벍', '벏', '벐', '벑', '벒', '벓', '벖', '벘', '벛', '벜', '벝', '벞', '벟', '벢', '벣', '벥', '벦', '벩', '벪', '벫', '벬', '벭', '벮', '벯', '벲', '벶', '벷', '벸', '벹', '벺', '벻', '벾', '벿', '볁', '볂', '볃', '볅', '볆', '볇', '볈', '볉', '볊', '볋', '볌', '볎', '볒', '볓', '볔', '볖', '볗', '볙', '볚', '볛', '볝', '볞', '볟', '볠', '볡', '볢', '볣', '볤', '볥', '볦', '볧', '볨', '볩', '볪', '볫', '볬', '볭', '볮', '볯', '볰', '볱', '볲', '볳', '볷', '볹', '볺', '볻', '볽', '볾', '볿', '봀', '봁', '봂', '봃', '봆', '봈', '봊', '봋', '봌', '봍', '봎', '봏', '봑', '봒', '봓', '봕', '봖', '봗', '봘', '봙', '봚', '봛', '봜', '봝', '봞', '봟', '봠', '봡', '봢', '봣', '봥', '봦', '봧', '봨', '봩', '봪', '봫', '봭', '봮', '봯', '봰', '봱', '봲', '봳', '봴', '봵', '봶', '봷', '봸', '봹', '봺', '봻', '봼', '봽', '봾', '봿', '뵁', '뵂', '뵃', '뵄', '뵅', '뵆', '뵇', '뵊', '뵋', '뵍', '뵎', '뵏', '뵑', '뵒', '뵓', '뵔', '뵕', '뵖', '뵗', '뵚', '뵛', '뵜', '뵝', '뵞', '뵟', '뵠', '뵡', '뵢', '뵣', '뵥', '뵦', '뵧', '뵩', '뵪', '뵫', '뵬', '뵭', '뵮', '뵯', '뵰', '뵱', '뵲', '뵳', '뵴', '뵵', '뵶', '뵷', '뵸', '뵹', '뵺', '뵻', '뵼', '뵽', '뵾', '뵿', '붂', '붃', '붅', '붆', '붋', '붌', '붍', '붎', '붏', '붒', '붔', '붖', '붗', '붘', '붛', '붝', '붞', '붟', '붠', '붡', '붢', '붣', '붥', '붦', '붧', '붨', '붩', '붪', '붫', '붬', '붭', '붮', '붯', '붱', '붲', '붳', '붴', '붵', '붶', '붷', '붹', '붺', '붻', '붼', '붽', '붾', '붿', '뷀', '뷁', '뷂', '뷃', '뷄', '뷅', '뷆', '뷇', '뷈', '뷉', '뷊', '뷋', '뷌', '뷍', '뷎', '뷏', '뷐', '뷑', '뷒', '뷓', '뷖', '뷗', '뷙', '뷚', '뷛', '뷝', '뷞', '뷟', '뷠', '뷡', '뷢', '뷣', '뷤', '뷥', '뷦', '뷧', '뷨', '뷪', '뷫', '뷬', '뷭', '뷮', '뷯', '뷱', '뷲', '뷳', '뷵', '뷶', '뷷', '뷹', '뷺', '뷻', '뷼', '뷽', '뷾', '뷿', '븁', '븂', '븄', '븆', '븇', '븈', '븉', '븊', '븋', '븎', '븏', '븑', '븒', '븓', '븕', '븖', '븗', '븘', '븙', '븚', '븛', '븞', '븠', '븡', '븢', '븣', '븤', '븥', '븦', '븧', '븨', '븩', '븪', '븫', '븬', '븭', '븮', '븯', '븰', '븱', '븲', '븳', '븴', '븵', '븶', '븷', '븸', '븹', '븺', '븻', '븼', '븽', '븾', '븿', '빀', '빁', '빂', '빃', '빆', '빇', '빉', '빊', '빋', '빍', '빏', '빐', '빑', '빒', '빓', '빖', '빘', '빜', '빝', '빞', '빟', '빢', '빣', '빥', '빦', '빧', '빩', '빫', '빬', '빭', '빮', '빯', '빲', '빶', '빷', '빸', '빹', '빺', '빾', '빿', '뺁', '뺂', '뺃', '뺅', '뺆', '뺇', '뺈', '뺉', '뺊', '뺋', '뺎', '뺒', '뺓', '뺔', '뺕', '뺖', '뺗', '뺚', '뺛', '뺜', '뺝', '뺞', '뺟', '뺠', '뺡', '뺢', '뺣', '뺤', '뺥', '뺦', '뺧', '뺩', '뺪', '뺫', '뺬', '뺭', '뺮', '뺯', '뺰', '뺱', '뺲', '뺳', '뺴', '뺵', '뺶', '뺷', '뺸', '뺹', '뺺', '뺻', '뺼', '뺽', '뺾', '뺿', '뻀', '뻁', '뻂', '뻃', '뻄', '뻅', '뻆', '뻇', '뻈', '뻉', '뻊', '뻋', '뻌', '뻍', '뻎', '뻏', '뻒', '뻓', '뻕', '뻖', '뻙', '뻚', '뻛', '뻜', '뻝', '뻞', '뻟', '뻡', '뻢', '뻦', '뻧', '뻨', '뻩', '뻪', '뻫', '뻭', '뻮', '뻯', '뻰', '뻱', '뻲', '뻳', '뻴', '뻵', '뻶', '뻷', '뻸', '뻹', '뻺', '뻻', '뻼', '뻽', '뻾', '뻿', '뼀', '뼂', '뼃', '뼄', '뼅', '뼆', '뼇', '뼊', '뼋', '뼌', '뼍', '뼎', '뼏', '뼐', '뼑', '뼒', '뼓', '뼔', '뼕', '뼖', '뼗', '뼚', '뼞', '뼟', '뼠', '뼡', '뼢', '뼣', '뼤', '뼥', '뼦', '뼧', '뼨', '뼩', '뼪', '뼫', '뼬', '뼭', '뼮', '뼯', '뼰', '뼱', '뼲', '뼳', '뼴', '뼵', '뼶', '뼷', '뼸', '뼹', '뼺', '뼻', '뼼', '뼽', '뼾', '뼿', '뽂', '뽃', '뽅', '뽆', '뽇', '뽉', '뽊', '뽋', '뽌', '뽍', '뽎', '뽏', '뽒', '뽓', '뽔', '뽖', '뽗', '뽘', '뽙', '뽚', '뽛', '뽜', '뽝', '뽞', '뽟', '뽠', '뽡', '뽢', '뽣', '뽤', '뽥', '뽦', '뽧', '뽨', '뽩', '뽪', '뽫', '뽬', '뽭', '뽮', '뽯', '뽰', '뽱', '뽲', '뽳', '뽴', '뽵', '뽶', '뽷', '뽸', '뽹', '뽺', '뽻', '뽼', '뽽', '뽾', '뽿', '뾀', '뾁', '뾂', '뾃', '뾄', '뾅', '뾆', '뾇', '뾈', '뾉', '뾊', '뾋', '뾌', '뾍', '뾎', '뾏', '뾐', '뾑', '뾒', '뾓', '뾕', '뾖', '뾗', '뾘', '뾙', '뾚', '뾛', '뾜', '뾝', '뾞', '뾟', '뾠', '뾡', '뾢', '뾣', '뾤', '뾥', '뾦', '뾧', '뾨', '뾩', '뾪', '뾫', '뾬', '뾭', '뾮', '뾯', '뾱', '뾲', '뾳', '뾴', '뾵', '뾶', '뾷', '뾸', '뾹', '뾺', '뾻', '뾼', '뾽', '뾾', '뾿', '뿀', '뿁', '뿂', '뿃', '뿄', '뿆', '뿇', '뿈', '뿉', '뿊', '뿋', '뿎', '뿏', '뿑', '뿒', '뿓', '뿕', '뿖', '뿗', '뿘', '뿙', '뿚', '뿛', '뿝', '뿞', '뿠', '뿢', '뿣', '뿤', '뿥', '뿦', '뿧', '뿨', '뿩', '뿪', '뿫', '뿬', '뿭', '뿮', '뿯', '뿰', '뿱', '뿲', '뿳', '뿴', '뿵', '뿶', '뿷', '뿸', '뿹', '뿺', '뿻', '뿼', '뿽', '뿾', '뿿', '쀀', '쀁', '쀂', '쀃', '쀄', '쀅', '쀆', '쀇', '쀈', '쀉', '쀊', '쀋', '쀌', '쀍', '쀎', '쀏', '쀐', '쀑', '쀒', '쀓', '쀔', '쀕', '쀖', '쀗', '쀘', '쀙', '쀚', '쀛', '쀜', '쀝', '쀞', '쀟', '쀠', '쀡', '쀢', '쀣', '쀤', '쀥', '쀦', '쀧', '쀨', '쀩', '쀪', '쀫', '쀬', '쀭', '쀮', '쀯', '쀰', '쀱', '쀲', '쀳', '쀴', '쀵', '쀶', '쀷', '쀸', '쀹', '쀺', '쀻', '쀽', '쀾', '쀿', '쁀', '쁁', '쁂', '쁃', '쁄', '쁅', '쁆', '쁇', '쁈', '쁉', '쁊', '쁋', '쁌', '쁍', '쁎', '쁏', '쁐', '쁒', '쁓', '쁔', '쁕', '쁖', '쁗', '쁙', '쁚', '쁛', '쁝', '쁞', '쁟', '쁡', '쁢', '쁣', '쁤', '쁥', '쁦', '쁧', '쁪', '쁫', '쁬', '쁭', '쁮', '쁯', '쁰', '쁱', '쁲', '쁳', '쁴', '쁵', '쁶', '쁷', '쁸', '쁹', '쁺', '쁻', '쁼', '쁽', '쁾', '쁿', '삀', '삁', '삂', '삃', '삄', '삅', '삆', '삇', '삈', '삉', '삊', '삋', '삌', '삍', '삎', '삏', '삒', '삓', '삕', '삖', '삗', '삙', '삚', '삛', '삜', '삝', '삞', '삟', '삢', '삤', '삦', '삧', '삨', '삩', '삪', '삫', '삮', '삱', '삲', '삷', '삸', '삹', '삺', '삻', '삾', '샂', '샃', '샄', '샆', '샇', '샊', '샋', '샍', '샎', '샏', '샑', '샒', '샓', '샔', '샕', '샖', '샗', '샚', '샞', '샟', '샠', '샡', '샢', '샣', '샦', '샧', '샩', '샪', '샫', '샭', '샮', '샯', '샰', '샱', '샲', '샳', '샶', '샸', '샺', '샻', '샼', '샽', '샾', '샿', '섁', '섂', '섃', '섅', '섆', '섇', '섉', '섊', '섋', '섌', '섍', '섎', '섏', '섑', '섒', '섓', '섔', '섖', '섗', '섘', '섙', '섚', '섛', '섡', '섢', '섥', '섨', '섩', '섪', '섫', '섮', '섲', '섳', '섴', '섵', '섷', '섺', '섻', '섽', '섾', '섿', '셁', '셂', '셃', '셄', '셅', '셆', '셇', '셊', '셎', '셏', '셐', '셑', '셒', '셓', '셖', '셗', '셙', '셚', '셛', '셝', '셞', '셟', '셠', '셡', '셢', '셣', '셦', '셪', '셫', '셬', '셭', '셮', '셯', '셱', '셲', '셳', '셵', '셶', '셷', '셹', '셺', '셻', '셼', '셽', '셾', '셿', '솀', '솁', '솂', '솃', '솄', '솆', '솇', '솈', '솉', '솊', '솋', '솏', '솑', '솒', '솓', '솕', '솗', '솘', '솙', '솚', '솛', '솞', '솠', '솢', '솣', '솤', '솦', '솧', '솪', '솫', '솭', '솮', '솯', '솱', '솲', '솳', '솴', '솵', '솶', '솷', '솸', '솹', '솺', '솻', '솼', '솾', '솿', '쇀', '쇁', '쇂', '쇃', '쇅', '쇆', '쇇', '쇉', '쇊', '쇋', '쇍', '쇎', '쇏', '쇐', '쇑', '쇒', '쇓', '쇕', '쇖', '쇙', '쇚', '쇛', '쇜', '쇝', '쇞', '쇟', '쇡', '쇢', '쇣', '쇥', '쇦', '쇧', '쇩', '쇪', '쇫', '쇬', '쇭', '쇮', '쇯', '쇲', '쇴', '쇵', '쇶', '쇷', '쇸', '쇹', '쇺', '쇻', '쇾', '쇿', '숁', '숂', '숃', '숅', '숆', '숇', '숈', '숉', '숊', '숋', '숎', '숐', '숒', '숓', '숔', '숕', '숖', '숗', '숚', '숛', '숝', '숞', '숡', '숢', '숣', '숤', '숥', '숦', '숧', '숪', '숬', '숮', '숰', '숳', '숵', '숶', '숷', '숸', '숹', '숺', '숻', '숼', '숽', '숾', '숿', '쉀', '쉁', '쉂', '쉃', '쉄', '쉅', '쉆', '쉇', '쉉', '쉊', '쉋', '쉌', '쉍', '쉎', '쉏', '쉒', '쉓', '쉕', '쉖', '쉗', '쉙', '쉚', '쉛', '쉜', '쉝', '쉞', '쉟', '쉡', '쉢', '쉣', '쉤', '쉦', '쉧', '쉨', '쉩', '쉪', '쉫', '쉮', '쉯', '쉱', '쉲', '쉳', '쉵', '쉶', '쉷', '쉸', '쉹', '쉺', '쉻', '쉾', '슀', '슂', '슃', '슄', '슅', '슆', '슇', '슊', '슋', '슌', '슍', '슎', '슏', '슑', '슒', '슓', '슔', '슕', '슖', '슗', '슙', '슚', '슜', '슞', '슟', '슠', '슡', '슢', '슣', '슦', '슧', '슩', '슪', '슫', '슮', '슯', '슰', '슱', '슲', '슳', '슶', '슸', '슺', '슻', '슼', '슽', '슾', '슿', '싀', '싁', '싂', '싃', '싄', '싅', '싆', '싇', '싈', '싉', '싊', '싋', '싌', '싍', '싎', '싏', '싐', '싑', '싒', '싓', '싔', '싕', '싖', '싗', '싘', '싙', '싚', '싛', '싞', '싟', '싡', '싢', '싥', '싦', '싧', '싨', '싩', '싪', '싮', '싰', '싲', '싳', '싴', '싵', '싷', '싺', '싽', '싾', '싿', '쌁', '쌂', '쌃', '쌄', '쌅', '쌆', '쌇', '쌊', '쌋', '쌎', '쌏', '쌐', '쌑', '쌒', '쌖', '쌗', '쌙', '쌚', '쌛', '쌝', '쌞', '쌟', '쌠', '쌡', '쌢', '쌣', '쌦', '쌧', '쌪', '쌫', '쌬', '쌭', '쌮', '쌯', '쌰', '쌱', '쌲', '쌳', '쌴', '쌵', '쌶', '쌷', '쌸', '쌹', '쌺', '쌻', '쌼', '쌽', '쌾', '쌿', '썀', '썁', '썂', '썃', '썄', '썆', '썇', '썈', '썉', '썊', '썋', '썌', '썍', '썎', '썏', '썐', '썑', '썒', '썓', '썔', '썕', '썖', '썗', '썘', '썙', '썚', '썛', '썜', '썝', '썞', '썟', '썠', '썡', '썢', '썣', '썤', '썥', '썦', '썧', '썪', '썫', '썭', '썮', '썯', '썱', '썳', '썴', '썵', '썶', '썷', '썺', '썻', '썾', '썿', '쎀', '쎁', '쎂', '쎃', '쎅', '쎆', '쎇', '쎉', '쎊', '쎋', '쎍', '쎎', '쎏', '쎐', '쎑', '쎒', '쎓', '쎔', '쎕', '쎖', '쎗', '쎘', '쎙', '쎚', '쎛', '쎜', '쎝', '쎞', '쎟', '쎠', '쎡', '쎢', '쎣', '쎤', '쎥', '쎦', '쎧', '쎨', '쎩', '쎪', '쎫', '쎬', '쎭', '쎮', '쎯', '쎰', '쎱', '쎲', '쎳', '쎴', '쎵', '쎶', '쎷', '쎸', '쎹', '쎺', '쎻', '쎼', '쎽', '쎾', '쎿', '쏁', '쏂', '쏃', '쏄', '쏅', '쏆', '쏇', '쏈', '쏉', '쏊', '쏋', '쏌', '쏍', '쏎', '쏏', '쏐', '쏑', '쏒', '쏓', '쏔', '쏕', '쏖', '쏗', '쏚', '쏛', '쏝', '쏞', '쏡', '쏣', '쏤', '쏥', '쏦', '쏧', '쏪', '쏫', '쏬', '쏮', '쏯', '쏰', '쏱', '쏲', '쏳', '쏶', '쏷', '쏹', '쏺', '쏻', '쏼', '쏽', '쏾', '쏿', '쐀', '쐁', '쐂', '쐃', '쐄', '쐅', '쐆', '쐇', '쐉', '쐊', '쐋', '쐌', '쐍', '쐎', '쐏', '쐑', '쐒', '쐓', '쐔', '쐕', '쐖', '쐗', '쐘', '쐙', '쐚', '쐛', '쐜', '쐝', '쐞', '쐟', '쐠', '쐡', '쐢', '쐣', '쐥', '쐦', '쐧', '쐨', '쐩', '쐪', '쐫', '쐭', '쐮', '쐯', '쐱', '쐲', '쐳', '쐵', '쐶', '쐷', '쐸', '쐹', '쐺', '쐻', '쐾', '쐿', '쑀', '쑁', '쑂', '쑃', '쑄', '쑅', '쑆', '쑇', '쑉', '쑊', '쑋', '쑌', '쑍', '쑎', '쑏', '쑐', '쑑', '쑒', '쑓', '쑔', '쑕', '쑖', '쑗', '쑘', '쑙', '쑚', '쑛', '쑜', '쑝', '쑞', '쑟', '쑠', '쑡', '쑢', '쑣', '쑦', '쑧', '쑩', '쑪', '쑫', '쑭', '쑮', '쑯', '쑰', '쑱', '쑲', '쑳', '쑶', '쑷', '쑸', '쑺', '쑻', '쑼', '쑽', '쑾', '쑿', '쒁', '쒂', '쒃', '쒄', '쒅', '쒆', '쒇', '쒈', '쒉', '쒊', '쒋', '쒌', '쒍', '쒎', '쒏', '쒐', '쒑', '쒒', '쒓', '쒕', '쒖', '쒗', '쒘', '쒙', '쒚', '쒛', '쒝', '쒞', '쒟', '쒠', '쒡', '쒢', '쒣', '쒤', '쒥', '쒦', '쒧', '쒨', '쒩', '쒪', '쒫', '쒬', '쒭', '쒮', '쒯', '쒰', '쒱', '쒲', '쒳', '쒴', '쒵', '쒶', '쒷', '쒹', '쒺', '쒻', '쒽', '쒾', '쒿', '쓀', '쓁', '쓂', '쓃', '쓄', '쓅', '쓆', '쓇', '쓈', '쓉', '쓊', '쓋', '쓌', '쓍', '쓎', '쓏', '쓐', '쓑', '쓒', '쓓', '쓔', '쓕', '쓖', '쓗', '쓘', '쓙', '쓚', '쓛', '쓜', '쓝', '쓞', '쓟', '쓠', '쓡', '쓢', '쓣', '쓤', '쓥', '쓦', '쓧', '쓨', '쓪', '쓫', '쓬', '쓭', '쓮', '쓯', '쓲', '쓳', '쓵', '쓶', '쓷', '쓹', '쓻', '쓼', '쓽', '쓾', '씂', '씃', '씄', '씅', '씆', '씇', '씈', '씉', '씊', '씋', '씍', '씎', '씏', '씑', '씒', '씓', '씕', '씖', '씗', '씘', '씙', '씚', '씛', '씝', '씞', '씟', '씠', '씡', '씢', '씣', '씤', '씥', '씦', '씧', '씪', '씫', '씭', '씮', '씯', '씱', '씲', '씳', '씴', '씵', '씶', '씷', '씺', '씼', '씾', '씿', '앀', '앁', '앂', '앃', '앆', '앇', '앋', '앏', '앐', '앑', '앒', '앖', '앚', '앛', '앜', '앟', '앢', '앣', '앥', '앦', '앧', '앩', '앪', '앫', '앬', '앭', '앮', '앯', '앲', '앶', '앷', '앸', '앹', '앺', '앻', '앾', '앿', '얁', '얂', '얃', '얅', '얆', '얈', '얉', '얊', '얋', '얎', '얐', '얒', '얓', '얔', '얖', '얙', '얚', '얛', '얝', '얞', '얟', '얡', '얢', '얣', '얤', '얥', '얦', '얧', '얨', '얪', '얫', '얬', '얭', '얮', '얯', '얰', '얱', '얲', '얳', '얶', '얷', '얺', '얿', '엀', '엁', '엂', '엃', '엋', '엍', '엏', '엒', '엓', '엕', '엖', '엗', '엙', '엚', '엛', '엜', '엝', '엞', '엟', '엢', '엤', '엦', '엧', '엨', '엩', '엪', '엫', '엯', '엱', '엲', '엳', '엵', '엸', '엹', '엺', '엻', '옂', '옃', '옄', '옉', '옊', '옋', '옍', '옎', '옏', '옑', '옒', '옓', '옔', '옕', '옖', '옗', '옚', '옝', '옞', '옟', '옠', '옡', '옢', '옣', '옦', '옧', '옩', '옪', '옫', '옯', '옱', '옲', '옶', '옸', '옺', '옼', '옽', '옾', '옿', '왂', '왃', '왅', '왆', '왇', '왉', '왊', '왋', '왌', '왍', '왎', '왏', '왒', '왖', '왗', '왘', '왙', '왚', '왛', '왞', '왟', '왡', '왢', '왣', '왤', '왥', '왦', '왧', '왨', '왩', '왪', '왫', '왭', '왮', '왰', '왲', '왳', '왴', '왵', '왶', '왷', '왺', '왻', '왽', '왾', '왿', '욁', '욂', '욃', '욄', '욅', '욆', '욇', '욊', '욌', '욎', '욏', '욐', '욑', '욒', '욓', '욖', '욗', '욙', '욚', '욛', '욝', '욞', '욟', '욠', '욡', '욢', '욣', '욦', '욨', '욪', '욫', '욬', '욭', '욮', '욯', '욲', '욳', '욵', '욶', '욷', '욻', '욼', '욽', '욾', '욿', '웂', '웄', '웆', '웇', '웈', '웉', '웊', '웋', '웎', '웏', '웑', '웒', '웓', '웕', '웖', '웗', '웘', '웙', '웚', '웛', '웞', '웟', '웢', '웣', '웤', '웥', '웦', '웧', '웪', '웫', '웭', '웮', '웯', '웱', '웲', '웳', '웴', '웵', '웶', '웷', '웺', '웻', '웼', '웾', '웿', '윀', '윁', '윂', '윃', '윆', '윇', '윉', '윊', '윋', '윍', '윎', '윏', '윐', '윑', '윒', '윓', '윖', '윘', '윚', '윛', '윜', '윝', '윞', '윟', '윢', '윣', '윥', '윦', '윧', '윩', '윪', '윫', '윬', '윭', '윮', '윯', '윲', '윴', '윶', '윸', '윹', '윺', '윻', '윾', '윿', '읁', '읂', '읃', '읅', '읆', '읇', '읈', '읉', '읋', '읎', '읐', '읙', '읚', '읛', '읝', '읞', '읟', '읡', '읢', '읣', '읤', '읥', '읦', '읧', '읩', '읪', '읬', '읭', '읮', '읯', '읰', '읱', '읲', '읳', '읶', '읷', '읹', '읺', '읻', '읿', '잀', '잁', '잂', '잆', '잋', '잌', '잍', '잏', '잒', '잓', '잕', '잙', '잛', '잜', '잝', '잞', '잟', '잢', '잧', '잨', '잩', '잪', '잫', '잮', '잯', '잱', '잲', '잳', '잵', '잶', '잷', '잸', '잹', '잺', '잻', '잾', '쟂', '쟃', '쟄', '쟅', '쟆', '쟇', '쟊', '쟋', '쟍', '쟏', '쟑', '쟒', '쟓', '쟔', '쟕', '쟖', '쟗', '쟙', '쟚', '쟛', '쟜', '쟞', '쟟', '쟠', '쟡', '쟢', '쟣', '쟥', '쟦', '쟧', '쟩', '쟪', '쟫', '쟭', '쟮', '쟯', '쟰', '쟱', '쟲', '쟳', '쟴', '쟵', '쟶', '쟷', '쟸', '쟹', '쟺', '쟻', '쟼', '쟽', '쟾', '쟿', '젂', '젃', '젅', '젆', '젇', '젉', '젋', '젌', '젍', '젎', '젏', '젒', '젔', '젗', '젘', '젙', '젚', '젛', '젞', '젟', '젡', '젢', '젣', '젥', '젦', '젧', '젨', '젩', '젪', '젫', '젮', '젰', '젲', '젳', '젴', '젵', '젶', '젷', '젹', '젺', '젻', '젽', '젾', '젿', '졁', '졂', '졃', '졄', '졅', '졆', '졇', '졊', '졋', '졎', '졏', '졐', '졑', '졒', '졓', '졕', '졖', '졗', '졘', '졙', '졚', '졛', '졜', '졝', '졞', '졟', '졠', '졡', '졢', '졣', '졤', '졥', '졦', '졧', '졨', '졩', '졪', '졫', '졬', '졭', '졮', '졯', '졲', '졳', '졵', '졶', '졷', '졹', '졻', '졼', '졽', '졾', '졿', '좂', '좄', '좈', '좉', '좊', '좎', '좏', '좐', '좑', '좒', '좓', '좕', '좖', '좗', '좘', '좙', '좚', '좛', '좜', '좞', '좠', '좢', '좣', '좤', '좥', '좦', '좧', '좩', '좪', '좫', '좬', '좭', '좮', '좯', '좰', '좱', '좲', '좳', '좴', '좵', '좶', '좷', '좸', '좹', '좺', '좻', '좾', '좿', '죀', '죁', '죂', '죃', '죅', '죆', '죇', '죉', '죊', '죋', '죍', '죎', '죏', '죐', '죑', '죒', '죓', '죖', '죘', '죚', '죛', '죜', '죝', '죞', '죟', '죢', '죣', '죥', '죦', '죧', '죨', '죩', '죪', '죫', '죬', '죭', '죮', '죯', '죰', '죱', '죲', '죳', '죴', '죶', '죷', '죸', '죹', '죺', '죻', '죾', '죿', '줁', '줂', '줃', '줇', '줈', '줉', '줊', '줋', '줎', '줐', '줒', '줓', '줔', '줕', '줖', '줗', '줙', '줚', '줛', '줜', '줝', '줞', '줟', '줠', '줡', '줢', '줣', '줤', '줥', '줦', '줧', '줨', '줩', '줪', '줫', '줭', '줮', '줯', '줰', '줱', '줲', '줳', '줵', '줶', '줷', '줸', '줹', '줺', '줻', '줼', '줽', '줾', '줿', '쥀', '쥁', '쥂', '쥃', '쥄', '쥅', '쥆', '쥇', '쥈', '쥉', '쥊', '쥋', '쥌', '쥍', '쥎', '쥏', '쥒', '쥓', '쥕', '쥖', '쥗', '쥙', '쥚', '쥛', '쥜', '쥝', '쥞', '쥟', '쥢', '쥤', '쥥', '쥦', '쥧', '쥨', '쥩', '쥪', '쥫', '쥭', '쥮', '쥯', '쥱', '쥲', '쥳', '쥵', '쥶', '쥷', '쥸', '쥹', '쥺', '쥻', '쥽', '쥾', '쥿', '즀', '즁', '즂', '즃', '즄', '즅', '즆', '즇', '즊', '즋', '즍', '즎', '즏', '즑', '즒', '즓', '즔', '즕', '즖', '즗', '즚', '즜', '즞', '즟', '즠', '즡', '즢', '즣', '즤', '즥', '즦', '즧', '즨', '즩', '즪', '즫', '즬', '즭', '즮', '즯', '즰', '즱', '즲', '즳', '즴', '즵', '즶', '즷', '즸', '즹', '즺', '즻', '즼', '즽', '즾', '즿', '짂', '짃', '짅', '짆', '짉', '짋', '짌', '짍', '짎', '짏', '짒', '짔', '짗', '짘', '짛', '짞', '짟', '짡', '짣', '짥', '짦', '짨', '짩', '짪', '짫', '짮', '짲', '짳', '짴', '짵', '짶', '짷', '짺', '짻', '짽', '짾', '짿', '쨁', '쨂', '쨃', '쨄', '쨅', '쨆', '쨇', '쨊', '쨎', '쨏', '쨐', '쨑', '쨒', '쨓', '쨕', '쨖', '쨗', '쨙', '쨚', '쨛', '쨜', '쨝', '쨞', '쨟', '쨠', '쨡', '쨢', '쨣', '쨤', '쨥', '쨦', '쨧', '쨨', '쨪', '쨫', '쨬', '쨭', '쨮', '쨯', '쨰', '쨱', '쨲', '쨳', '쨴', '쨵', '쨶', '쨷', '쨸', '쨹', '쨺', '쨻', '쨼', '쨽', '쨾', '쨿', '쩀', '쩁', '쩂', '쩃', '쩄', '쩅', '쩆', '쩇', '쩈', '쩉', '쩊', '쩋', '쩎', '쩏', '쩑', '쩒', '쩓', '쩕', '쩖', '쩗', '쩘', '쩙', '쩚', '쩛', '쩞', '쩢', '쩣', '쩤', '쩥', '쩦', '쩧', '쩩', '쩪', '쩫', '쩬', '쩭', '쩮', '쩯', '쩰', '쩱', '쩲', '쩳', '쩴', '쩵', '쩶', '쩷', '쩸', '쩹', '쩺', '쩻', '쩼', '쩾', '쩿', '쪀', '쪁', '쪂', '쪃', '쪅', '쪆', '쪇', '쪈', '쪉', '쪊', '쪋', '쪌', '쪍', '쪎', '쪏', '쪐', '쪑', '쪒', '쪓', '쪔', '쪕', '쪖', '쪗', '쪙', '쪚', '쪛', '쪜', '쪝', '쪞', '쪟', '쪠', '쪡', '쪢', '쪣', '쪤', '쪥', '쪦', '쪧', '쪨', '쪩', '쪪', '쪫', '쪬', '쪭', '쪮', '쪯', '쪰', '쪱', '쪲', '쪳', '쪴', '쪵', '쪶', '쪷', '쪸', '쪹', '쪺', '쪻', '쪾', '쪿', '쫁', '쫂', '쫃', '쫅', '쫆', '쫇', '쫈', '쫉', '쫊', '쫋', '쫎', '쫐', '쫒', '쫔', '쫕', '쫖', '쫗', '쫚', '쫛', '쫜', '쫝', '쫞', '쫟', '쫡', '쫢', '쫣', '쫤', '쫥', '쫦', '쫧', '쫨', '쫩', '쫪', '쫫', '쫭', '쫮', '쫯', '쫰', '쫱', '쫲', '쫳', '쫵', '쫶', '쫷', '쫸', '쫹', '쫺', '쫻', '쫼', '쫽', '쫾', '쫿', '쬀', '쬁', '쬂', '쬃', '쬄', '쬅', '쬆', '쬇', '쬉', '쬊', '쬋', '쬌', '쬍', '쬎', '쬏', '쬑', '쬒', '쬓', '쬕', '쬖', '쬗', '쬙', '쬚', '쬛', '쬜', '쬝', '쬞', '쬟', '쬢', '쬣', '쬤', '쬥', '쬦', '쬧', '쬨', '쬩', '쬪', '쬫', '쬬', '쬭', '쬮', '쬯', '쬰', '쬱', '쬲', '쬳', '쬴', '쬵', '쬶', '쬷', '쬸', '쬹', '쬺', '쬻', '쬼', '쬽', '쬾', '쬿', '쭀', '쭂', '쭃', '쭄', '쭅', '쭆', '쭇', '쭊', '쭋', '쭍', '쭎', '쭏', '쭑', '쭒', '쭓', '쭔', '쭕', '쭖', '쭗', '쭚', '쭛', '쭜', '쭞', '쭟', '쭠', '쭡', '쭢', '쭣', '쭥', '쭦', '쭧', '쭨', '쭩', '쭪', '쭫', '쭬', '쭭', '쭮', '쭯', '쭰', '쭱', '쭲', '쭳', '쭴', '쭵', '쭶', '쭷', '쭺', '쭻', '쭼', '쭽', '쭾', '쭿', '쮀', '쮁', '쮂', '쮃', '쮄', '쮅', '쮆', '쮇', '쮈', '쮉', '쮊', '쮋', '쮌', '쮍', '쮎', '쮏', '쮐', '쮑', '쮒', '쮓', '쮔', '쮕', '쮖', '쮗', '쮘', '쮙', '쮚', '쮛', '쮝', '쮞', '쮟', '쮠', '쮡', '쮢', '쮣', '쮤', '쮥', '쮦', '쮧', '쮨', '쮩', '쮪', '쮫', '쮬', '쮭', '쮮', '쮯', '쮰', '쮱', '쮲', '쮳', '쮴', '쮵', '쮶', '쮷', '쮹', '쮺', '쮻', '쮼', '쮽', '쮾', '쮿', '쯀', '쯁', '쯂', '쯃', '쯄', '쯅', '쯆', '쯇', '쯈', '쯉', '쯊', '쯋', '쯌', '쯍', '쯎', '쯏', '쯐', '쯑', '쯒', '쯓', '쯕', '쯖', '쯗', '쯘', '쯙', '쯚', '쯛', '쯜', '쯝', '쯞', '쯟', '쯠', '쯡', '쯢', '쯣', '쯥', '쯦', '쯨', '쯪', '쯫', '쯬', '쯭', '쯮', '쯯', '쯰', '쯱', '쯲', '쯳', '쯴', '쯵', '쯶', '쯷', '쯸', '쯹', '쯺', '쯻', '쯼', '쯽', '쯾', '쯿', '찀', '찁', '찂', '찃', '찄', '찅', '찆', '찇', '찈', '찉', '찊', '찋', '찎', '찏', '찑', '찒', '찓', '찕', '찖', '찗', '찘', '찙', '찚', '찛', '찞', '찟', '찠', '찣', '찤', '찥', '찦', '찪', '찫', '찭', '찯', '찱', '찲', '찳', '찴', '찵', '찶', '찷', '찺', '찿', '챀', '챁', '챂', '챃', '챆', '챇', '챉', '챊', '챋', '챍', '챎', '챏', '챐', '챑', '챒', '챓', '챖', '챚', '챛', '챜', '챝', '챞', '챟', '챡', '챢', '챣', '챥', '챧', '챩', '챪', '챫', '챬', '챭', '챮', '챯', '챱', '챲', '챳', '챴', '챶', '챷', '챸', '챹', '챺', '챻', '챼', '챽', '챾', '챿', '첀', '첁', '첂', '첃', '첄', '첅', '첆', '첇', '첈', '첉', '첊', '첋', '첌', '첍', '첎', '첏', '첐', '첑', '첒', '첓', '첔', '첕', '첖', '첗', '첚', '첛', '첝', '첞', '첟', '첡', '첢', '첣', '첤', '첥', '첦', '첧', '첪', '첮', '첯', '첰', '첱', '첲', '첳', '첶', '첷', '첹', '첺', '첻', '첽', '첾', '첿', '쳀', '쳁', '쳂', '쳃', '쳆', '쳈', '쳊', '쳋', '쳌', '쳍', '쳎', '쳏', '쳑', '쳒', '쳓', '쳕', '쳖', '쳗', '쳘', '쳙', '쳚', '쳛', '쳜', '쳝', '쳞', '쳟', '쳠', '쳡', '쳢', '쳣', '쳥', '쳦', '쳧', '쳨', '쳩', '쳪', '쳫', '쳭', '쳮', '쳯', '쳱', '쳲', '쳳', '쳴', '쳵', '쳶', '쳷', '쳸', '쳹', '쳺', '쳻', '쳼', '쳽', '쳾', '쳿', '촀', '촂', '촃', '촄', '촅', '촆', '촇', '촊', '촋', '촍', '촎', '촏', '촑', '촒', '촓', '촔', '촕', '촖', '촗', '촚', '촜', '촞', '촟', '촠', '촡', '촢', '촣', '촥', '촦', '촧', '촩', '촪', '촫', '촭', '촮', '촯', '촰', '촱', '촲', '촳', '촴', '촵', '촶', '촷', '촸', '촺', '촻', '촼', '촽', '촾', '촿', '쵀', '쵁', '쵂', '쵃', '쵄', '쵅', '쵆', '쵇', '쵈', '쵉', '쵊', '쵋', '쵌', '쵍', '쵎', '쵏', '쵐', '쵑', '쵒', '쵓', '쵔', '쵕', '쵖', '쵗', '쵘', '쵙', '쵚', '쵛', '쵝', '쵞', '쵟', '쵡', '쵢', '쵣', '쵥', '쵦', '쵧', '쵨', '쵩', '쵪', '쵫', '쵮', '쵰', '쵲', '쵳', '쵴', '쵵', '쵶', '쵷', '쵹', '쵺', '쵻', '쵼', '쵽', '쵾', '쵿', '춀', '춁', '춂', '춃', '춄', '춅', '춆', '춇', '춉', '춊', '춋', '춌', '춍', '춎', '춏', '춐', '춑', '춒', '춓', '춖', '춗', '춙', '춚', '춛', '춝', '춞', '춟', '춠', '춡', '춢', '춣', '춦', '춨', '춪', '춫', '춬', '춭', '춮', '춯', '춱', '춲', '춳', '춴', '춵', '춶', '춷', '춸', '춹', '춺', '춻', '춼', '춽', '춾', '춿', '췀', '췁', '췂', '췃', '췅', '췆', '췇', '췈', '췉', '췊', '췋', '췍', '췎', '췏', '췑', '췒', '췓', '췔', '췕', '췖', '췗', '췘', '췙', '췚', '췛', '췜', '췝', '췞', '췟', '췠', '췡', '췢', '췣', '췤', '췥', '췦', '췧', '췩', '췪', '췫', '췭', '췮', '췯', '췱', '췲', '췳', '췴', '췵', '췶', '췷', '췺', '췼', '췾', '췿', '츀', '츁', '츂', '츃', '츅', '츆', '츇', '츉', '츊', '츋', '츍', '츎', '츏', '츐', '츑', '츒', '츓', '츕', '츖', '츗', '츘', '츚', '츛', '츜', '츝', '츞', '츟', '츢', '츣', '츥', '츦', '츧', '츩', '츪', '츫', '츬', '츭', '츮', '츯', '츲', '츴', '츶', '츷', '츸', '츹', '츺', '츻', '츼', '츽', '츾', '츿', '칀', '칁', '칂', '칃', '칄', '칅', '칆', '칇', '칈', '칉', '칊', '칋', '칌', '칍', '칎', '칏', '칐', '칑', '칒', '칓', '칔', '칕', '칖', '칗', '칚', '칛', '칝', '칞', '칢', '칣', '칤', '칥', '칦', '칧', '칪', '칬', '칮', '칯', '칰', '칱', '칲', '칳', '칶', '칷', '칹', '칺', '칻', '칽', '칾', '칿', '캀', '캁', '캂', '캃', '캆', '캈', '캊', '캋', '캌', '캍', '캎', '캏', '캒', '캓', '캕', '캖', '캗', '캙', '캚', '캛', '캜', '캝', '캞', '캟', '캢', '캦', '캧', '캨', '캩', '캪', '캫', '캮', '캯', '캰', '캱', '캲', '캳', '캴', '캵', '캶', '캷', '캸', '캹', '캺', '캻', '캼', '캽', '캾', '캿', '컀', '컂', '컃', '컄', '컅', '컆', '컇', '컈', '컉', '컊', '컋', '컌', '컍', '컎', '컏', '컐', '컑', '컒', '컓', '컔', '컕', '컖', '컗', '컘', '컙', '컚', '컛', '컜', '컝', '컞', '컟', '컠', '컡', '컢', '컣', '컦', '컧', '컩', '컪', '컭', '컮', '컯', '컰', '컱', '컲', '컳', '컶', '컺', '컻', '컼', '컽', '컾', '컿', '켂', '켃', '켅', '켆', '켇', '켉', '켊', '켋', '켌', '켍', '켎', '켏', '켒', '켔', '켖', '켗', '켘', '켙', '켚', '켛', '켝', '켞', '켟', '켡', '켢', '켣', '켥', '켦', '켧', '켨', '켩', '켪', '켫', '켮', '켲', '켳', '켴', '켵', '켶', '켷', '켹', '켺', '켻', '켼', '켽', '켾', '켿', '콀', '콁', '콂', '콃', '콄', '콅', '콆', '콇', '콈', '콉', '콊', '콋', '콌', '콍', '콎', '콏', '콐', '콑', '콒', '콓', '콖', '콗', '콙', '콚', '콛', '콝', '콞', '콟', '콠', '콡', '콢', '콣', '콦', '콨', '콪', '콫', '콬', '콭', '콮', '콯', '콲', '콳', '콵', '콶', '콷', '콹', '콺', '콻', '콼', '콽', '콾', '콿', '쾁', '쾂', '쾃', '쾄', '쾆', '쾇', '쾈', '쾉', '쾊', '쾋', '쾍', '쾎', '쾏', '쾐', '쾑', '쾒', '쾓', '쾔', '쾕', '쾖', '쾗', '쾘', '쾙', '쾚', '쾛', '쾜', '쾝', '쾞', '쾟', '쾠', '쾢', '쾣', '쾤', '쾥', '쾦', '쾧', '쾩', '쾪', '쾫', '쾬', '쾭', '쾮', '쾯', '쾱', '쾲', '쾳', '쾴', '쾵', '쾶', '쾷', '쾸', '쾹', '쾺', '쾻', '쾼', '쾽', '쾾', '쾿', '쿀', '쿁', '쿂', '쿃', '쿅', '쿆', '쿇', '쿈', '쿉', '쿊', '쿋', '쿌', '쿍', '쿎', '쿏', '쿐', '쿑', '쿒', '쿓', '쿔', '쿕', '쿖', '쿗', '쿘', '쿙', '쿚', '쿛', '쿜', '쿝', '쿞', '쿟', '쿢', '쿣', '쿥', '쿦', '쿧', '쿩', '쿪', '쿫', '쿬', '쿭', '쿮', '쿯', '쿲', '쿴', '쿶', '쿷', '쿸', '쿹', '쿺', '쿻', '쿽', '쿾', '쿿', '퀁', '퀂', '퀃', '퀅', '퀆', '퀇', '퀈', '퀉', '퀊', '퀋', '퀌', '퀍', '퀎', '퀏', '퀐', '퀒', '퀓', '퀔', '퀕', '퀖', '퀗', '퀙', '퀚', '퀛', '퀜', '퀝', '퀞', '퀟', '퀠', '퀡', '퀢', '퀣', '퀤', '퀥', '퀦', '퀧', '퀨', '퀩', '퀪', '퀫', '퀬', '퀮', '퀯', '퀰', '퀱', '퀲', '퀳', '퀶', '퀷', '퀹', '퀺', '퀻', '퀽', '퀾', '퀿', '큀', '큁', '큂', '큃', '큆', '큈', '큊', '큋', '큌', '큍', '큎', '큏', '큑', '큒', '큓', '큕', '큖', '큗', '큙', '큚', '큛', '큜', '큝', '큞', '큟', '큡', '큢', '큣', '큤', '큥', '큦', '큧', '큨', '큩', '큪', '큫', '큮', '큯', '큱', '큲', '큳', '큵', '큶', '큷', '큸', '큹', '큺', '큻', '큾', '큿', '킀', '킂', '킃', '킄', '킅', '킆', '킇', '킈', '킉', '킊', '킋', '킌', '킍', '킎', '킏', '킐', '킑', '킒', '킓', '킔', '킕', '킖', '킗', '킘', '킙', '킚', '킛', '킜', '킝', '킞', '킟', '킠', '킡', '킢', '킣', '킦', '킧', '킩', '킪', '킫', '킭', '킮', '킯', '킰', '킱', '킲', '킳', '킶', '킸', '킺', '킻', '킼', '킽', '킾', '킿', '탂', '탃', '탅', '탆', '탇', '탊', '탋', '탌', '탍', '탎', '탏', '탒', '탖', '탗', '탘', '탙', '탚', '탛', '탞', '탟', '탡', '탢', '탣', '탥', '탦', '탧', '탨', '탩', '탪', '탫', '탮', '탲', '탳', '탴', '탵', '탶', '탷', '탹', '탺', '탻', '탼', '탽', '탾', '탿', '턀', '턁', '턂', '턃', '턄', '턅', '턆', '턇', '턈', '턉', '턊', '턋', '턌', '턎', '턏', '턐', '턑', '턒', '턓', '턔', '턕', '턖', '턗', '턘', '턙', '턚', '턛', '턜', '턝', '턞', '턟', '턠', '턡', '턢', '턣', '턤', '턥', '턦', '턧', '턨', '턩', '턪', '턫', '턬', '턭', '턮', '턯', '턲', '턳', '턵', '턶', '턷', '턹', '턻', '턼', '턽', '턾', '턿', '텂', '텆', '텇', '텈', '텉', '텊', '텋', '텎', '텏', '텑', '텒', '텓', '텕', '텖', '텗', '텘', '텙', '텚', '텛', '텞', '텠', '텢', '텣', '텤', '텥', '텦', '텧', '텩', '텪', '텫', '텭', '텮', '텯', '텰', '텱', '텲', '텳', '텴', '텵', '텶', '텷', '텸', '텹', '텺', '텻', '텽', '텾', '텿', '톀', '톁', '톂', '톃', '톅', '톆', '톇', '톉', '톊', '톋', '톌', '톍', '톎', '톏', '톐', '톑', '톒', '톓', '톔', '톕', '톖', '톗', '톘', '톙', '톚', '톛', '톜', '톝', '톞', '톟', '톢', '톣', '톥', '톦', '톧', '톩', '톪', '톫', '톬', '톭', '톮', '톯', '톲', '톴', '톶', '톷', '톸', '톹', '톻', '톽', '톾', '톿', '퇁', '퇂', '퇃', '퇄', '퇅', '퇆', '퇇', '퇈', '퇉', '퇊', '퇋', '퇌', '퇍', '퇎', '퇏', '퇐', '퇑', '퇒', '퇓', '퇔', '퇕', '퇖', '퇗', '퇙', '퇚', '퇛', '퇜', '퇝', '퇞', '퇟', '퇠', '퇡', '퇢', '퇣', '퇤', '퇥', '퇦', '퇧', '퇨', '퇩', '퇪', '퇫', '퇬', '퇭', '퇮', '퇯', '퇰', '퇱', '퇲', '퇳', '퇵', '퇶', '퇷', '퇹', '퇺', '퇻', '퇼', '퇽', '퇾', '퇿', '툀', '툁', '툂', '툃', '툄', '툅', '툆', '툈', '툊', '툋', '툌', '툍', '툎', '툏', '툑', '툒', '툓', '툔', '툕', '툖', '툗', '툘', '툙', '툚', '툛', '툜', '툝', '툞', '툟', '툠', '툡', '툢', '툣', '툤', '툥', '툦', '툧', '툨', '툩', '툪', '툫', '툮', '툯', '툱', '툲', '툳', '툵', '툶', '툷', '툸', '툹', '툺', '툻', '툾', '퉀', '퉂', '퉃', '퉄', '퉅', '퉆', '퉇', '퉉', '퉊', '퉋', '퉌', '퉍', '퉎', '퉏', '퉐', '퉑', '퉒', '퉓', '퉔', '퉕', '퉖', '퉗', '퉘', '퉙', '퉚', '퉛', '퉝', '퉞', '퉟', '퉠', '퉡', '퉢', '퉣', '퉥', '퉦', '퉧', '퉨', '퉩', '퉪', '퉫', '퉬', '퉭', '퉮', '퉯', '퉰', '퉱', '퉲', '퉳', '퉴', '퉵', '퉶', '퉷', '퉸', '퉹', '퉺', '퉻', '퉼', '퉽', '퉾', '퉿', '튂', '튃', '튅', '튆', '튇', '튉', '튊', '튋', '튌', '튍', '튎', '튏', '튒', '튓', '튔', '튖', '튗', '튘', '튙', '튚', '튛', '튝', '튞', '튟', '튡', '튢', '튣', '튥', '튦', '튧', '튨', '튩', '튪', '튫', '튭', '튮', '튯', '튰', '튲', '튳', '튴', '튵', '튶', '튷', '튺', '튻', '튽', '튾', '틁', '틃', '틄', '틅', '틆', '틇', '틊', '틌', '틍', '틎', '틏', '틐', '틑', '틒', '틓', '틕', '틖', '틗', '틙', '틚', '틛', '틝', '틞', '틟', '틠', '틡', '틢', '틣', '틦', '틧', '틨', '틩', '틪', '틫', '틬', '틭', '틮', '틯', '틲', '틳', '틵', '틶', '틷', '틹', '틺', '틻', '틼', '틽', '틾', '틿', '팂', '팄', '팆', '팇', '팈', '팉', '팊', '팋', '팏', '팑', '팒', '팓', '팕', '팗', '팘', '팙', '팚', '팛', '팞', '팢', '팣', '팤', '팦', '팧', '팪', '팫', '팭', '팮', '팯', '팱', '팲', '팳', '팴', '팵', '팶', '팷', '팺', '팾', '팿', '퍀', '퍁', '퍂', '퍃', '퍆', '퍇', '퍈', '퍉', '퍊', '퍋', '퍌', '퍍', '퍎', '퍏', '퍐', '퍑', '퍒', '퍓', '퍔', '퍕', '퍖', '퍗', '퍘', '퍙', '퍚', '퍛', '퍜', '퍝', '퍞', '퍟', '퍠', '퍡', '퍢', '퍣', '퍤', '퍥', '퍦', '퍧', '퍨', '퍩', '퍪', '퍫', '퍬', '퍭', '퍮', '퍯', '퍰', '퍱', '퍲', '퍳', '퍴', '퍵', '퍶', '퍷', '퍸', '퍹', '퍺', '퍻', '퍾', '퍿', '펁', '펂', '펃', '펅', '펆', '펇', '펈', '펉', '펊', '펋', '펎', '펒', '펓', '펔', '펕', '펖', '펗', '펚', '펛', '펝', '펞', '펟', '펡', '펢', '펣', '펤', '펥', '펦', '펧', '펪', '펬', '펮', '펯', '펰', '펱', '펲', '펳', '펵', '펶', '펷', '펹', '펺', '펻', '펽', '펾', '펿', '폀', '폁', '폂', '폃', '폆', '폇', '폊', '폋', '폌', '폍', '폎', '폏', '폑', '폒', '폓', '폔', '폕', '폖', '폗', '폙', '폚', '폛', '폜', '폝', '폞', '폟', '폠', '폢', '폤', '폥', '폦', '폧', '폨', '폩', '폪', '폫', '폮', '폯', '폱', '폲', '폳', '폵', '폶', '폷', '폸', '폹', '폺', '폻', '폾', '퐀', '퐂', '퐃', '퐄', '퐅', '퐆', '퐇', '퐉', '퐊', '퐋', '퐌', '퐍', '퐎', '퐏', '퐐', '퐑', '퐒', '퐓', '퐔', '퐕', '퐖', '퐗', '퐘', '퐙', '퐚', '퐛', '퐜', '퐞', '퐟', '퐠', '퐡', '퐢', '퐣', '퐤', '퐥', '퐦', '퐧', '퐨', '퐩', '퐪', '퐫', '퐬', '퐭', '퐮', '퐯', '퐰', '퐱', '퐲', '퐳', '퐴', '퐵', '퐶', '퐷', '퐸', '퐹', '퐺', '퐻', '퐼', '퐽', '퐾', '퐿', '푁', '푂', '푃', '푅', '푆', '푇', '푈', '푉', '푊', '푋', '푌', '푍', '푎', '푏', '푐', '푑', '푒', '푓', '푔', '푕', '푖', '푗', '푘', '푙', '푚', '푛', '푝', '푞', '푟', '푡', '푢', '푣', '푥', '푦', '푧', '푨', '푩', '푪', '푫', '푬', '푮', '푰', '푱', '푲', '푳', '푴', '푵', '푶', '푷', '푺', '푻', '푽', '푾', '풁', '풃', '풄', '풅', '풆', '풇', '풊', '풌', '풎', '풏', '풐', '풑', '풒', '풓', '풕', '풖', '풗', '풘', '풙', '풚', '풛', '풜', '풝', '풞', '풟', '풠', '풡', '풢', '풣', '풤', '풥', '풦', '풧', '풨', '풪', '풫', '풬', '풭', '풮', '풯', '풰', '풱', '풲', '풳', '풴', '풵', '풶', '풷', '풸', '풹', '풺', '풻', '풼', '풽', '풾', '풿', '퓀', '퓁', '퓂', '퓃', '퓄', '퓅', '퓆', '퓇', '퓈', '퓉', '퓊', '퓋', '퓍', '퓎', '퓏', '퓑', '퓒', '퓓', '퓕', '퓖', '퓗', '퓘', '퓙', '퓚', '퓛', '퓝', '퓞', '퓠', '퓡', '퓢', '퓣', '퓤', '퓥', '퓦', '퓧', '퓩', '퓪', '퓫', '퓭', '퓮', '퓯', '퓱', '퓲', '퓳', '퓴', '퓵', '퓶', '퓷', '퓹', '퓺', '퓼', '퓾', '퓿', '픀', '픁', '픂', '픃', '픅', '픆', '픇', '픉', '픊', '픋', '픍', '픎', '픏', '픐', '픑', '픒', '픓', '픖', '픘', '픙', '픚', '픛', '픜', '픝', '픞', '픟', '픠', '픡', '픢', '픣', '픤', '픥', '픦', '픧', '픨', '픩', '픪', '픫', '픬', '픭', '픮', '픯', '픰', '픱', '픲', '픳', '픴', '픵', '픶', '픷', '픸', '픹', '픺', '픻', '픾', '픿', '핁', '핂', '핃', '핅', '핆', '핇', '핈', '핉', '핊', '핋', '핎', '핐', '핒', '핓', '핔', '핕', '핖', '핗', '핚', '핛', '핝', '핞', '핟', '핡', '핢', '핣', '핤', '핦', '핧', '핪', '핬', '핮', '핯', '핰', '핱', '핲', '핳', '핶', '핷', '핹', '핺', '핻', '핽', '핾', '핿', '햀', '햁', '햂', '햃', '햆', '햊', '햋', '햌', '햍', '햎', '햏', '햑', '햒', '햓', '햔', '햕', '햖', '햗', '햘', '햙', '햚', '햛', '햜', '햝', '햞', '햟', '햠', '햡', '햢', '햣', '햤', '햦', '햧', '햨', '햩', '햪', '햫', '햬', '햭', '햮', '햯', '햰', '햱', '햲', '햳', '햴', '햵', '햶', '햷', '햸', '햹', '햺', '햻', '햼', '햽', '햾', '햿', '헀', '헁', '헂', '헃', '헄', '헅', '헆', '헇', '헊', '헋', '헍', '헎', '헏', '헑', '헓', '헔', '헕', '헖', '헗', '헚', '헜', '헞', '헟', '헠', '헡', '헢', '헣', '헦', '헧', '헩', '헪', '헫', '헭', '헮', '헯', '헰', '헱', '헲', '헳', '헶', '헸', '헺', '헻', '헼', '헽', '헾', '헿', '혂', '혃', '혅', '혆', '혇', '혉', '혊', '혋', '혌', '혍', '혎', '혏', '혒', '혖', '혗', '혘', '혙', '혚', '혛', '혝', '혞', '혟', '혡', '혢', '혣', '혥', '혦', '혧', '혨', '혩', '혪', '혫', '혬', '혮', '혯', '혰', '혱', '혲', '혳', '혴', '혵', '혶', '혷', '혺', '혻', '혽', '혾', '혿', '홁', '홂', '홃', '홄', '홆', '홇', '홊', '홌', '홎', '홏', '홐', '홒', '홓', '홖', '홗', '홙', '홚', '홛', '홝', '홞', '홟', '홠', '홡', '홢', '홣', '홤', '홥', '홦', '홨', '홪', '홫', '홬', '홭', '홮', '홯', '홲', '홳', '홵', '홶', '홷', '홸', '홹', '홺', '홻', '홼', '홽', '홾', '홿', '횀', '횁', '횂', '횄', '횆', '횇', '횈', '횉', '횊', '횋', '횎', '횏', '횑', '횒', '횓', '횕', '횖', '횗', '횘', '횙', '횚', '횛', '횜', '횞', '횠', '횢', '횣', '횤', '횥', '횦', '횧', '횩', '횪', '횫', '횭', '횮', '횯', '횱', '횲', '횳', '횴', '횵', '횶', '횷', '횸', '횺', '횼', '횽', '횾', '횿', '훀', '훁', '훂', '훃', '훆', '훇', '훉', '훊', '훋', '훍', '훎', '훏', '훐', '훒', '훓', '훕', '훖', '훘', '훚', '훛', '훜', '훝', '훞', '훟', '훡', '훢', '훣', '훥', '훦', '훧', '훩', '훪', '훫', '훬', '훭', '훮', '훯', '훱', '훲', '훳', '훴', '훶', '훷', '훸', '훹', '훺', '훻', '훾', '훿', '휁', '휂', '휃', '휅', '휆', '휇', '휈', '휉', '휊', '휋', '휌', '휍', '휎', '휏', '휐', '휒', '휓', '휔', '휕', '휖', '휗', '휚', '휛', '휝', '휞', '휟', '휡', '휢', '휣', '휤', '휥', '휦', '휧', '휪', '휬', '휮', '휯', '휰', '휱', '휲', '휳', '휶', '휷', '휹', '휺', '휻', '휽', '휾', '휿', '흀', '흁', '흂', '흃', '흅', '흆', '흈', '흊', '흋', '흌', '흍', '흎', '흏', '흒', '흓', '흕', '흚', '흛', '흜', '흝', '흞', '흟', '흢', '흤', '흦', '흧', '흨', '흪', '흫', '흭', '흮', '흯', '흱', '흲', '흳', '흵', '흶', '흷', '흸', '흹', '흺', '흻', '흾', '흿', '힀', '힂', '힃', '힄', '힅', '힆', '힇', '힊', '힋', '힍', '힎', '힏', '힑', '힒', '힓', '힔', '힕', '힖', '힗', '힚', '힜', '힞', '힟', '힠', '힡', '힢', '힣', '\ud7a4']
+['가', '각', '간', '갇', '갈', '갉', '갊', '감', '갑', '값', '갓', '갔', '강', '갖', '갗', '같', '갚', '갛', '개', '객', '갠', '갤', '갬', '갭', '갯', '갰', '갱', '갸', '갹', '갼', '걀', '걋', '걍', '걔', '걘', '걜', '거', '걱', '건', '걷', '걸', '걺', '검', '겁', '것', '겄', '겅', '겆', '겉', '겊', '겋', '게', '겐', '겔', '겜', '겝', '겟', '겠', '겡', '겨', '격', '겪', '견', '겯', '결', '겸', '겹', '겻', '겼', '경', '곁', '계', '곈', '곌', '곕', '곗', '고', '곡', '곤', '곧', '골', '곪', '곬', '곯', '곰', '곱', '곳', '공', '곶', '과', '곽', '관', '괄', '괆', '괌', '괍', '괏', '광', '괘', '괜', '괠', '괩', '괬', '괭', '괴', '괵', '괸', '괼', '굄', '굅', '굇', '굉', '교', '굔', '굘', '굡', '굣', '구', '국', '군', '굳', '굴', '굵', '굶', '굻', '굼', '굽', '굿', '궁', '궂', '궈', '궉', '권', '궐', '궜', '궝', '궤', '궷', '귀', '귁', '귄', '귈', '귐', '귑', '귓', '규', '균', '귤', '그', '극', '근', '귿', '글', '긁', '금', '급', '긋', '긍', '긔', '기', '긱', '긴', '긷', '길', '긺', '김', '깁', '깃', '깅', '깆', '깊', '까', '깍', '깎', '깐', '깔', '깖', '깜', '깝', '깟', '깠', '깡', '깥', '깨', '깩', '깬', '깰', '깸', '깹', '깻', '깼', '깽', '꺄', '꺅', '꺌', '꺼', '꺽', '꺾', '껀', '껄', '껌', '껍', '껏', '껐', '껑', '께', '껙', '껜', '껨', '껫', '껭', '껴', '껸', '껼', '꼇', '꼈', '꼍', '꼐', '꼬', '꼭', '꼰', '꼲', '꼴', '꼼', '꼽', '꼿', '꽁', '꽂', '꽃', '꽈', '꽉', '꽐', '꽜', '꽝', '꽤', '꽥', '꽹', '꾀', '꾄', '꾈', '꾐', '꾑', '꾕', '꾜', '꾸', '꾹', '꾼', '꿀', '꿇', '꿈', '꿉', '꿋', '꿍', '꿎', '꿔', '꿜', '꿨', '꿩', '꿰', '꿱', '꿴', '꿸', '뀀', '뀁', '뀄', '뀌', '뀐', '뀔', '뀜', '뀝', '뀨', '끄', '끅', '끈', '끊', '끌', '끎', '끓', '끔', '끕', '끗', '끙', '끝', '끼', '끽', '낀', '낄', '낌', '낍', '낏', '낑', '나', '낙', '낚', '난', '낟', '날', '낡', '낢', '남', '납', '낫', '났', '낭', '낮', '낯', '낱', '낳', '내', '낵', '낸', '낼', '냄', '냅', '냇', '냈', '냉', '냐', '냑', '냔', '냘', '냠', '냥', '너', '넉', '넋', '넌', '널', '넒', '넓', '넘', '넙', '넛', '넜', '넝', '넣', '네', '넥', '넨', '넬', '넴', '넵', '넷', '넸', '넹', '녀', '녁', '년', '녈', '념', '녑', '녔', '녕', '녘', '녜', '녠', '노', '녹', '논', '놀', '놂', '놈', '놉', '놋', '농', '높', '놓', '놔', '놘', '놜', '놨', '뇌', '뇐', '뇔', '뇜', '뇝', '뇟', '뇨', '뇩', '뇬', '뇰', '뇹', '뇻', '뇽', '누', '눅', '눈', '눋', '눌', '눔', '눕', '눗', '눙', '눠', '눴', '눼', '뉘', '뉜', '뉠', '뉨', '뉩', '뉴', '뉵', '뉼', '늄', '늅', '늉', '느', '늑', '는', '늘', '늙', '늚', '늠', '늡', '늣', '능', '늦', '늪', '늬', '늰', '늴', '니', '닉', '닌', '닐', '닒', '님', '닙', '닛', '닝', '닢', '다', '닥', '닦', '단', '닫', '달', '닭', '닮', '닯', '닳', '담', '답', '닷', '닸', '당', '닺', '닻', '닿', '대', '댁', '댄', '댈', '댐', '댑', '댓', '댔', '댕', '댜', '더', '덕', '덖', '던', '덛', '덜', '덞', '덟', '덤', '덥', '덧', '덩', '덫', '덮', '데', '덱', '덴', '델', '뎀', '뎁', '뎃', '뎄', '뎅', '뎌', '뎐', '뎔', '뎠', '뎡', '뎨', '뎬', '도', '독', '돈', '돋', '돌', '돎', '돐', '돔', '돕', '돗', '동', '돛', '돝', '돠', '돤', '돨', '돼', '됐', '되', '된', '될', '됨', '됩', '됫', '됴', '두', '둑', '둔', '둘', '둠', '둡', '둣', '둥', '둬', '뒀', '뒈', '뒝', '뒤', '뒨', '뒬', '뒵', '뒷', '뒹', '듀', '듄', '듈', '듐', '듕', '드', '득', '든', '듣', '들', '듦', '듬', '듭', '듯', '등', '듸', '디', '딕', '딘', '딛', '딜', '딤', '딥', '딧', '딨', '딩', '딪', '따', '딱', '딴', '딸', '땀', '땁', '땃', '땄', '땅', '땋', '때', '땍', '땐', '땔', '땜', '땝', '땟', '땠', '땡', '떠', '떡', '떤', '떨', '떪', '떫', '떰', '떱', '떳', '떴', '떵', '떻', '떼', '떽', '뗀', '뗄', '뗌', '뗍', '뗏', '뗐', '뗑', '뗘', '뗬', '또', '똑', '똔', '똘', '똥', '똬', '똴', '뙈', '뙤', '뙨', '뚜', '뚝', '뚠', '뚤', '뚫', '뚬', '뚱', '뛔', '뛰', '뛴', '뛸', '뜀', '뜁', '뜅', '뜨', '뜩', '뜬', '뜯', '뜰', '뜸', '뜹', '뜻', '띄', '띈', '띌', '띔', '띕', '띠', '띤', '띨', '띰', '띱', '띳', '띵', '라', '락', '란', '랄', '람', '랍', '랏', '랐', '랑', '랒', '랖', '랗', '래', '랙', '랜', '랠', '램', '랩', '랫', '랬', '랭', '랴', '략', '랸', '럇', '량', '러', '럭', '런', '럴', '럼', '럽', '럿', '렀', '렁', '렇', '레', '렉', '렌', '렐', '렘', '렙', '렛', '렝', '려', '력', '련', '렬', '렴', '렵', '렷', '렸', '령', '례', '롄', '롑', '롓', '로', '록', '론', '롤', '롬', '롭', '롯', '롱', '롸', '롼', '뢍', '뢨', '뢰', '뢴', '뢸', '룀', '룁', '룃', '룅', '료', '룐', '룔', '룝', '룟', '룡', '루', '룩', '룬', '룰', '룸', '룹', '룻', '룽', '뤄', '뤘', '뤠', '뤼', '뤽', '륀', '륄', '륌', '륏', '륑', '류', '륙', '륜', '률', '륨', '륩', '륫', '륭', '르', '륵', '른', '를', '름', '릅', '릇', '릉', '릊', '릍', '릎', '리', '릭', '린', '릴', '림', '립', '릿', '링', '마', '막', '만', '많', '맏', '말', '맑', '맒', '맘', '맙', '맛', '망', '맞', '맡', '맣', '매', '맥', '맨', '맬', '맴', '맵', '맷', '맸', '맹', '맺', '먀', '먁', '먈', '먕', '머', '먹', '먼', '멀', '멂', '멈', '멉', '멋', '멍', '멎', '멓', '메', '멕', '멘', '멜', '멤', '멥', '멧', '멨', '멩', '며', '멱', '면', '멸', '몃', '몄', '명', '몇', '몌', '모', '목', '몫', '몬', '몰', '몲', '몸', '몹', '못', '몽', '뫄', '뫈', '뫘', '뫙', '뫼', '묀', '묄', '묍', '묏', '묑', '묘', '묜', '묠', '묩', '묫', '무', '묵', '묶', '문', '묻', '물', '묽', '묾', '뭄', '뭅', '뭇', '뭉', '뭍', '뭏', '뭐', '뭔', '뭘', '뭡', '뭣', '뭬', '뮈', '뮌', '뮐', '뮤', '뮨', '뮬', '뮴', '뮷', '므', '믄', '믈', '믐', '믓', '미', '믹', '민', '믿', '밀', '밂', '밈', '밉', '밋', '밌', '밍', '및', '밑', '바', '박', '밖', '밗', '반', '받', '발', '밝', '밞', '밟', '밤', '밥', '밧', '방', '밭', '배', '백', '밴', '밸', '뱀', '뱁', '뱃', '뱄', '뱅', '뱉', '뱌', '뱍', '뱐', '뱝', '버', '벅', '번', '벋', '벌', '벎', '범', '법', '벗', '벙', '벚', '베', '벡', '벤', '벧', '벨', '벰', '벱', '벳', '벴', '벵', '벼', '벽', '변', '별', '볍', '볏', '볐', '병', '볕', '볘', '볜', '보', '복', '볶', '본', '볼', '봄', '봅', '봇', '봉', '봐', '봔', '봤', '봬', '뵀', '뵈', '뵉', '뵌', '뵐', '뵘', '뵙', '뵤', '뵨', '부', '북', '분', '붇', '불', '붉', '붊', '붐', '붑', '붓', '붕', '붙', '붚', '붜', '붤', '붰', '붸', '뷔', '뷕', '뷘', '뷜', '뷩', '뷰', '뷴', '뷸', '븀', '븃', '븅', '브', '븍', '븐', '블', '븜', '븝', '븟', '비', '빅', '빈', '빌', '빎', '빔', '빕', '빗', '빙', '빚', '빛', '빠', '빡', '빤', '빨', '빪', '빰', '빱', '빳', '빴', '빵', '빻', '빼', '빽', '뺀', '뺄', '뺌', '뺍', '뺏', '뺐', '뺑', '뺘', '뺙', '뺨', '뻐', '뻑', '뻔', '뻗', '뻘', '뻠', '뻣', '뻤', '뻥', '뻬', '뼁', '뼈', '뼉', '뼘', '뼙', '뼛', '뼜', '뼝', '뽀', '뽁', '뽄', '뽈', '뽐', '뽑', '뽕', '뾔', '뾰', '뿅', '뿌', '뿍', '뿐', '뿔', '뿜', '뿟', '뿡', '쀼', '쁑', '쁘', '쁜', '쁠', '쁨', '쁩', '삐', '삑', '삔', '삘', '삠', '삡', '삣', '삥', '사', '삭', '삯', '산', '삳', '살', '삵', '삶', '삼', '삽', '삿', '샀', '상', '샅', '새', '색', '샌', '샐', '샘', '샙', '샛', '샜', '생', '샤', '샥', '샨', '샬', '샴', '샵', '샷', '샹', '섀', '섄', '섈', '섐', '섕', '서', '석', '섞', '섟', '선', '섣', '설', '섦', '섧', '섬', '섭', '섯', '섰', '성', '섶', '세', '섹', '센', '셀', '셈', '셉', '셋', '셌', '셍', '셔', '셕', '션', '셜', '셤', '셥', '셧', '셨', '셩', '셰', '셴', '셸', '솅', '소', '속', '솎', '손', '솔', '솖', '솜', '솝', '솟', '송', '솥', '솨', '솩', '솬', '솰', '솽', '쇄', '쇈', '쇌', '쇔', '쇗', '쇘', '쇠', '쇤', '쇨', '쇰', '쇱', '쇳', '쇼', '쇽', '숀', '숄', '숌', '숍', '숏', '숑', '수', '숙', '순', '숟', '술', '숨', '숩', '숫', '숭', '숯', '숱', '숲', '숴', '쉈', '쉐', '쉑', '쉔', '쉘', '쉠', '쉥', '쉬', '쉭', '쉰', '쉴', '쉼', '쉽', '쉿', '슁', '슈', '슉', '슐', '슘', '슛', '슝', '스', '슥', '슨', '슬', '슭', '슴', '습', '슷', '승', '시', '식', '신', '싣', '실', '싫', '심', '십', '싯', '싱', '싶', '싸', '싹', '싻', '싼', '쌀', '쌈', '쌉', '쌌', '쌍', '쌓', '쌔', '쌕', '쌘', '쌜', '쌤', '쌥', '쌨', '쌩', '썅', '써', '썩', '썬', '썰', '썲', '썸', '썹', '썼', '썽', '쎄', '쎈', '쎌', '쏀', '쏘', '쏙', '쏜', '쏟', '쏠', '쏢', '쏨', '쏩', '쏭', '쏴', '쏵', '쏸', '쐈', '쐐', '쐤', '쐬', '쐰', '쐴', '쐼', '쐽', '쑈', '쑤', '쑥', '쑨', '쑬', '쑴', '쑵', '쑹', '쒀', '쒔', '쒜', '쒸', '쒼', '쓩', '쓰', '쓱', '쓴', '쓸', '쓺', '쓿', '씀', '씁', '씌', '씐', '씔', '씜', '씨', '씩', '씬', '씰', '씸', '씹', '씻', '씽', '아', '악', '안', '앉', '않', '알', '앍', '앎', '앓', '암', '압', '앗', '았', '앙', '앝', '앞', '애', '액', '앤', '앨', '앰', '앱', '앳', '앴', '앵', '야', '약', '얀', '얄', '얇', '얌', '얍', '얏', '양', '얕', '얗', '얘', '얜', '얠', '얩', '어', '억', '언', '얹', '얻', '얼', '얽', '얾', '엄', '업', '없', '엇', '었', '엉', '엊', '엌', '엎', '에', '엑', '엔', '엘', '엠', '엡', '엣', '엥', '여', '역', '엮', '연', '열', '엶', '엷', '염', '엽', '엾', '엿', '였', '영', '옅', '옆', '옇', '예', '옌', '옐', '옘', '옙', '옛', '옜', '오', '옥', '온', '올', '옭', '옮', '옰', '옳', '옴', '옵', '옷', '옹', '옻', '와', '왁', '완', '왈', '왐', '왑', '왓', '왔', '왕', '왜', '왝', '왠', '왬', '왯', '왱', '외', '왹', '왼', '욀', '욈', '욉', '욋', '욍', '요', '욕', '욘', '욜', '욤', '욥', '욧', '용', '우', '욱', '운', '울', '욹', '욺', '움', '웁', '웃', '웅', '워', '웍', '원', '월', '웜', '웝', '웠', '웡', '웨', '웩', '웬', '웰', '웸', '웹', '웽', '위', '윅', '윈', '윌', '윔', '윕', '윗', '윙', '유', '육', '윤', '율', '윰', '윱', '윳', '융', '윷', '으', '윽', '은', '을', '읊', '음', '읍', '읏', '응', '읒', '읓', '읔', '읕', '읖', '읗', '의', '읜', '읠', '읨', '읫', '이', '익', '인', '일', '읽', '읾', '잃', '임', '입', '잇', '있', '잉', '잊', '잎', '자', '작', '잔', '잖', '잗', '잘', '잚', '잠', '잡', '잣', '잤', '장', '잦', '재', '잭', '잰', '잴', '잼', '잽', '잿', '쟀', '쟁', '쟈', '쟉', '쟌', '쟎', '쟐', '쟘', '쟝', '쟤', '쟨', '쟬', '저', '적', '전', '절', '젊', '점', '접', '젓', '정', '젖', '제', '젝', '젠', '젤', '젬', '젭', '젯', '젱', '져', '젼', '졀', '졈', '졉', '졌', '졍', '졔', '조', '족', '존', '졸', '졺', '좀', '좁', '좃', '종', '좆', '좇', '좋', '좌', '좍', '좔', '좝', '좟', '좡', '좨', '좼', '좽', '죄', '죈', '죌', '죔', '죕', '죗', '죙', '죠', '죡', '죤', '죵', '주', '죽', '준', '줄', '줅', '줆', '줌', '줍', '줏', '중', '줘', '줬', '줴', '쥐', '쥑', '쥔', '쥘', '쥠', '쥡', '쥣', '쥬', '쥰', '쥴', '쥼', '즈', '즉', '즌', '즐', '즘', '즙', '즛', '증', '지', '직', '진', '짇', '질', '짊', '짐', '집', '짓', '징', '짖', '짙', '짚', '짜', '짝', '짠', '짢', '짤', '짧', '짬', '짭', '짯', '짰', '짱', '째', '짹', '짼', '쨀', '쨈', '쨉', '쨋', '쨌', '쨍', '쨔', '쨘', '쨩', '쩌', '쩍', '쩐', '쩔', '쩜', '쩝', '쩟', '쩠', '쩡', '쩨', '쩽', '쪄', '쪘', '쪼', '쪽', '쫀', '쫄', '쫌', '쫍', '쫏', '쫑', '쫓', '쫘', '쫙', '쫠', '쫬', '쫴', '쬈', '쬐', '쬔', '쬘', '쬠', '쬡', '쭁', '쭈', '쭉', '쭌', '쭐', '쭘', '쭙', '쭝', '쭤', '쭸', '쭹', '쮜', '쮸', '쯔', '쯤', '쯧', '쯩', '찌', '찍', '찐', '찔', '찜', '찝', '찡', '찢', '찧', '차', '착', '찬', '찮', '찰', '참', '찹', '찻', '찼', '창', '찾', '채', '책', '챈', '챌', '챔', '챕', '챗', '챘', '챙', '챠', '챤', '챦', '챨', '챰', '챵', '처', '척', '천', '철', '첨', '첩', '첫', '첬', '청', '체', '첵', '첸', '첼', '쳄', '쳅', '쳇', '쳉', '쳐', '쳔', '쳤', '쳬', '쳰', '촁', '초', '촉', '촌', '촐', '촘', '촙', '촛', '총', '촤', '촨', '촬', '촹', '최', '쵠', '쵤', '쵬', '쵭', '쵯', '쵱', '쵸', '춈', '추', '축', '춘', '출', '춤', '춥', '춧', '충', '춰', '췄', '췌', '췐', '취', '췬', '췰', '췸', '췹', '췻', '췽', '츄', '츈', '츌', '츔', '츙', '츠', '측', '츤', '츨', '츰', '츱', '츳', '층', '치', '칙', '친', '칟', '칠', '칡', '침', '칩', '칫', '칭', '카', '칵', '칸', '칼', '캄', '캅', '캇', '캉', '캐', '캑', '캔', '캘', '캠', '캡', '캣', '캤', '캥', '캬', '캭', '컁', '커', '컥', '컨', '컫', '컬', '컴', '컵', '컷', '컸', '컹', '케', '켁', '켄', '켈', '켐', '켑', '켓', '켕', '켜', '켠', '켤', '켬', '켭', '켯', '켰', '켱', '켸', '코', '콕', '콘', '콜', '콤', '콥', '콧', '콩', '콰', '콱', '콴', '콸', '쾀', '쾅', '쾌', '쾡', '쾨', '쾰', '쿄', '쿠', '쿡', '쿤', '쿨', '쿰', '쿱', '쿳', '쿵', '쿼', '퀀', '퀄', '퀑', '퀘', '퀭', '퀴', '퀵', '퀸', '퀼', '큄', '큅', '큇', '큉', '큐', '큔', '큘', '큠', '크', '큭', '큰', '클', '큼', '큽', '킁', '키', '킥', '킨', '킬', '킴', '킵', '킷', '킹', '타', '탁', '탄', '탈', '탉', '탐', '탑', '탓', '탔', '탕', '태', '택', '탠', '탤', '탬', '탭', '탯', '탰', '탱', '탸', '턍', '터', '턱', '턴', '털', '턺', '텀', '텁', '텃', '텄', '텅', '테', '텍', '텐', '텔', '템', '텝', '텟', '텡', '텨', '텬', '텼', '톄', '톈', '토', '톡', '톤', '톨', '톰', '톱', '톳', '통', '톺', '톼', '퇀', '퇘', '퇴', '퇸', '툇', '툉', '툐', '투', '툭', '툰', '툴', '툼', '툽', '툿', '퉁', '퉈', '퉜', '퉤', '튀', '튁', '튄', '튈', '튐', '튑', '튕', '튜', '튠', '튤', '튬', '튱', '트', '특', '튼', '튿', '틀', '틂', '틈', '틉', '틋', '틔', '틘', '틜', '틤', '틥', '티', '틱', '틴', '틸', '팀', '팁', '팃', '팅', '파', '팍', '팎', '판', '팔', '팖', '팜', '팝', '팟', '팠', '팡', '팥', '패', '팩', '팬', '팰', '팸', '팹', '팻', '팼', '팽', '퍄', '퍅', '퍼', '퍽', '펀', '펄', '펌', '펍', '펏', '펐', '펑', '페', '펙', '펜', '펠', '펨', '펩', '펫', '펭', '펴', '편', '펼', '폄', '폅', '폈', '평', '폐', '폘', '폡', '폣', '포', '폭', '폰', '폴', '폼', '폽', '폿', '퐁', '퐈', '퐝', '푀', '푄', '표', '푠', '푤', '푭', '푯', '푸', '푹', '푼', '푿', '풀', '풂', '품', '풉', '풋', '풍', '풔', '풩', '퓌', '퓐', '퓔', '퓜', '퓟', '퓨', '퓬', '퓰', '퓸', '퓻', '퓽', '프', '픈', '플', '픔', '픕', '픗', '피', '픽', '핀', '필', '핌', '핍', '핏', '핑', '하', '학', '한', '할', '핥', '함', '합', '핫', '항', '해', '핵', '핸', '핼', '햄', '햅', '햇', '했', '행', '햐', '향', '허', '헉', '헌', '헐', '헒', '험', '헙', '헛', '헝', '헤', '헥', '헨', '헬', '헴', '헵', '헷', '헹', '혀', '혁', '현', '혈', '혐', '협', '혓', '혔', '형', '혜', '혠', '혤', '혭', '호', '혹', '혼', '홀', '홅', '홈', '홉', '홋', '홍', '홑', '화', '확', '환', '활', '홧', '황', '홰', '홱', '홴', '횃', '횅', '회', '획', '횐', '횔', '횝', '횟', '횡', '효', '횬', '횰', '횹', '횻', '후', '훅', '훈', '훌', '훑', '훔', '훗', '훙', '훠', '훤', '훨', '훰', '훵', '훼', '훽', '휀', '휄', '휑', '휘', '휙', '휜', '휠', '휨', '휩', '휫', '휭', '휴', '휵', '휸', '휼', '흄', '흇', '흉', '흐', '흑', '흔', '흖', '흗', '흘', '흙', '흠', '흡', '흣', '흥', '흩', '희', '흰', '흴', '흼', '흽', '힁', '히', '힉', '힌', '힐', '힘', '힙', '힛', '힝']
 ```
 </details>
 
 <details>
 <summary>28. get_all_incompleted_form_hangul_chars</summary>
 
-This returns all non-completed form Hangul characters.
+This returns all incompleted form Hangul characters.
 
 Returns:
-- `List[str]`: all non-completed form Hangul characters
+- `List[str]`: all incompleted form Hangul characters
 
 Examples:
 ```python
 >>> from kss import Kss
 >>> get_all_incompleted_form_hangul_chars = Kss("get_all_incompleted_form_hangul_chars")
 >>> output = get_all_incompleted_form_hangul_chars()
 >>> print(output)
@@ -1043,17 +1010,17 @@
 Returns:
 - `Union[str, List[str]]`: normalized text or list of normalized texts
 
 Examples:
 ```python
 >>> from kss import Kss
 >>> normalize = Kss("normalize")
->>> text = "안녕\u200b하세요 ﾻﾻﾻﾻﾻﾻ   <br>오늘\u200b은 날이 참 좋네요.\\n\\n\\n200 &lt; 300 &amp; 400"
+>>> text = "안녕\u200b하세요 ﾻﾻﾻﾻﾻﾻ   <br>오늘\u200b은 날이 참 좋네요.\n\n\n200 &lt; 300 &amp; 400"
 >>> normalize(text, allow_doubled_spaces=False, allow_html_tags=False, allow_html_escape=False, allow_halfwidth_hangul=False, allow_hangul_jamo=False, allow_invisible_chars=False, reduce_char_repeats_over=2, reduce_emoticon_repeats_over=2)
-'안녕하세요 ㅋㅋ 오늘은 날이 참 좋네요.\\n200 < 300 & 400'
+'안녕하세요 ㅋㅋ 오늘은 날이 참 좋네요.\n200 < 300 & 400'
 ```
 </details>
 
 <details>
 <summary>32. preprocess</summary>
 
 This preprocesses text with various options.
@@ -1270,15 +1237,16 @@
 ```
 References:
 - This was copied from [korean-romanizer](https://github.com/osori/korean-romanizer) and modified by Kss
 </details>
 
 <details>
 <summary>38. is_unsafe</summary>
-Check if the text is unsafe or not.
+
+This checks if the text is unsafe or not.
 
 Args:
 - text (`Union[str, List[str], Tuple[str]]`): single text or list of texts
 - return_matches (`bool`): whether to return matches or not
 - num_workers (`Union[int, str]`): the number of multiprocessing workers
 
 Returns:
```

#### html2text {}

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1 Name: kss Version: 6.0.0 Summary: A Toolkit for Korean
-sentence segmentation Home-page: https://github.com/hyunwoongko/kss Author:
-Hyunwoong Ko Author-email: kevin.brain@kakaobrain.com License: BSD 3-Clause
-"New" or "Revised" License Platform: any Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.2 Classifier:
-Programming Language :: Python :: 3.3 Classifier: Programming Language ::
-Python :: 3.4 Classifier: Programming Language :: Python :: 3.5 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Requires-
-Python: >=3 Description-Content-Type: text/markdown License-File: LICENSE
                ************ KKSSSS:: KKoorreeaann SSttrriinngg pprroocceessssiinngg SSuuiittee ************
   _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_I_s_s_u_e_s_]_[_T_e_s_t_s_ _o_n_ _U_b_u_n_t_u_]_[_T_e_s_t_s_ _o_n_ _M_a_c_O_S_]_[_T_e_s_t_s_ _o_n_ _W_i_n_d_o_w_s_]
 KSS is a Korean string processing suite that provides various functions for
 processing Korean strings. It is designed to be simple and easy to use, and it
 is designed to be used in various fields such as natural language processing,
 data preprocessing, and data analysis. ### What's New: - April 27, 2024
 [Released Kss 6.0 Python](https://github.com/hyunwoongko/kss/releases/tag/
@@ -62,15 +52,15 @@
 (text) ['íì¬ ëë£ ë¶ë¤ê³¼ ë¤ëìëë° ë¶ìê¸°ë ì¢ê³  ììë
 ë§ììì´ì', 'ë¤ë§, ê°ë¨ í ë¼ì ì´ ê°ë¨ ììë²ê±° ê³¨ëª©ê¸¸ë¡
 ì­ ì¬ë¼ê°ì¼ íëë° ë¤ë¤ ììë²ê±°ì ì í¹ì ëì´ê° ë»
 íëµëë¤', 'ê°ë¨ì­ ë§ì§ í ë¼ì ì ì¸ë¶ ëª¨ìµ.'] ``` ### 4.
 Multiprocessing If you input a list of strings, Kss will automatically use
 multiprocessing to process the strings in parallel. And you can set the number
 of processes to use by setting the `num_workers` parameter. If you input
-`num_workers<2`, Kss will not use multiprocessing. ```python from kss import
+`num_workers < 2`, Kss will not use multiprocessing. ```python from kss import
 Kss module = Kss("MODULE_NAME") # using all cores output = module(
 ["YOUR_INPUT_STRING1", "YOUR_INPUT_STRING2", ...], **kwargs) # using 4 cores
 output = module(["YOUR_INPUT_STRING1", "YOUR_INPUT_STRING2", ...],
 num_workers=4, **kwargs) # using 1 core (no multiprocessing) output = module(
 ["YOUR_INPUT_STRING1", "YOUR_INPUT_STRING2", ...], num_workers=1, **kwargs) ```
 ### 5. Backward Compatibility The old version of Kss used functional usage. KSS
 also supports this for backward compatibility. ```python from kss import
@@ -655,27 +645,27 @@
 'ê³±ëì'), ('ë', 'ê³±ë'), ('ì°', 'ê³±ì°'), ('ì¼ë', 'ê³ ì°ë'),
 ('ì¼ëê³ ', 'ê³ ì°ëê³ '), ('ì¼ë¨', 'ê³ ì°ë¨'), ('ì¼ë',
 'ê³ ì°ë'), ('ì¼ëë¼', 'ê³ ì°ëë¼'), ('ì¼ì´', 'ê³ ì°ì´'),
 ('ìê°', 'ê³ ì´ê°'), ('ìê°', 'ê³ ì´ê°'), ('ìê³ ', 'ê³ ì´ê³ '),
 ('ìë°', 'ê³ ì´ë°'), ('ìëì¼', 'ê³ ì´ëì¼'), ('ìì§',
 'ê³ ì´ì§'), ('ìë°ë¼ë', 'ê³ ì¸ë°ë¼ë'), ('ììê³ ',
 'ê³ ì¸ìê³ ')]} ``` References: - This was copied from [KoParadigm](https://
-github.com/Kyubyong/KoParadigm) and modified by Kss 24. anonymize Anonymize
-sensitive information in the given text. Args: - text (`Union[str, List[str],
-Tuple[str]`): single text or list of texts - phone_number_anonymization
-(`bool`): whether to anonymize phone numbers or not - rrn_anonymization
-(`bool`): whether to anonymize resident registration numbers or not -
-card_anonymization (`bool`): whether to anonymize card numbers or not -
-email_anonymization (`bool`): whether to anonymize email addresses or not -
-back_account_anonymization (`bool`): whether to anonymize bank account numbers
-or not - credit_card_anonymization (`bool`): whether to anonymize credit card
-numbers or not - zip_anonymization (`bool`): whether to anonymize zip codes or
-not - bitcoin_anonymization (`bool`): whether to anonymize bitcoin addresses or
-not - url_anonymization (`bool`): whether to anonymize URLs or not -
-ip_v6_anonymization (`bool`): whether to anonymize IPv6 addresses or not -
+github.com/Kyubyong/KoParadigm) and modified by Kss 24. anonymize This
+anonymizes sensitive information in the given text. Args: - text (`Union[str,
+List[str], Tuple[str]`): single text or list of texts -
+phone_number_anonymization (`bool`): whether to anonymize phone numbers or not
+- rrn_anonymization (`bool`): whether to anonymize resident registration
+numbers or not - card_anonymization (`bool`): whether to anonymize card numbers
+or not - email_anonymization (`bool`): whether to anonymize email addresses or
+not - back_account_anonymization (`bool`): whether to anonymize bank account
+numbers or not - credit_card_anonymization (`bool`): whether to anonymize
+credit card numbers or not - zip_anonymization (`bool`): whether to anonymize
+zip codes or not - bitcoin_anonymization (`bool`): whether to anonymize bitcoin
+addresses or not - url_anonymization (`bool`): whether to anonymize URLs or not
+- ip_v6_anonymization (`bool`): whether to anonymize IPv6 addresses or not -
 ip_v4_anonymization (`bool`): whether to anonymize IPv4 addresses or not -
 phone_number_replacement (`str`): the replacement string for phone numbers,
 default is "" - rrn_replacement (`str`): the replacement string for resident
 registration numbers, default is "" - card_replacement (`str`): the replacement
 string for card numbers, default is "" - email_replacement (`str`): the
 replacement string for email addresses, default is "" -
 back_account_replacement (`str`): the replacement string for bank account
@@ -688,24 +678,24 @@
 ip_v4_replacement (`str`): the replacement string for IPv4 addresses, default
 is "" - num_workers (`Union[int, str]`): the number of multiprocessing workers
 Returns: - `Union[str, List[str], Tuple[str]]`: anonymized text or list of
 anonymized texts Examples: ```python >>> from kss import Kss >>> anonymize =
 Kss("anonymize") >>> text = "ì  ì íë²í¸ë 010-1234-5678, ì´ë©ì¼
 ì£¼ìë kevin.brain@kakaobrain.comìëë¤." >>> output = anonymize(text)
 >>> print(output) "ì  ì íë²í¸ë , ì´ë©ì¼ ì£¼ìë ìëë¤." ```
-25. clean_news Clean news articles by removing useless headers and footers.
-Args: - text (`Union[str, List[str], Tuple[str]]`): Input text or list of
-texts. - min_sentences (`int`): Minimum number of sentences to keep. Defaults
-to 3. - header_ratio (`float`): Ratio of the number of sentences to check in
-the header. Defaults to 0.4. - footer_ratio (`float`): Ratio of the number of
-sentences to check in the footer. Defaults to 0.4. - num_workers (`Union[int,
-str]`): the number of multiprocessing workers - verbose (`bool`): whether to
-print verbose outputs or not Returns: - `Union[str, List[str]]`: Cleaned text
-or list of cleaned texts. Examples: ```python >>> from kss import Kss >>>
-clean_news = Kss("clean_news") >>> text = "[ì¬ì§]ìë²ëë, ë´ê½
+25. clean_news This cleans news articles by removing useless headers and
+footers. Args: - text (`Union[str, List[str], Tuple[str]]`): Input text or list
+of texts. - min_sentences (`int`): Minimum number of sentences to keep.
+Defaults to 3. - header_ratio (`float`): Ratio of the number of sentences to
+check in the header. Defaults to 0.4. - footer_ratio (`float`): Ratio of the
+number of sentences to check in the footer. Defaults to 0.4. - num_workers
+(`Union[int, str]`): the number of multiprocessing workers - verbose (`bool`):
+whether to print verbose outputs or not Returns: - `Union[str, List[str]]`:
+Cleaned text or list of cleaned texts. Examples: ```python >>> from kss import
+Kss >>> clean_news = Kss("clean_news") >>> text = "[ì¬ì§]ìë²ëë, ë´ê½
 í¼ì³ì§ 'í¤ë¦½ì¶ì ' ì¤í\n\n[ ë´ì¤1 ì ê³µ](ìì¸=ë´ì¤1) ì´ëì
 ê¸°ì = ìë²ëëê° ì¤ë 22ì¼ë¶í° ë´ì ìì§íë í¤ë¦½ 120ë§
 ì¡ì´ì í¨ê» 'í¤ë¦½ì¶ì 'ë¥¼ ì¤íí´ ë³¸ê²©ì ì¸ ë´ì ììì
 ìë¦°ë¤. ì§ë 1992ë êµ­ë´ ì²« í¤ë¦½ ì¶ì ë¥¼ ì° ì´í ì¬í´ë¡
 22íì§¸ë¥¼ ë§ì´í ìë²ëë 'í¤ë¦½ì¶ì 'ë ì§ëí´ ì²« ì ì
 ë³´ì´ë©° ì¢ì ë°ìì ì»ìë ì¤ê°(äºæ)ì²´í 'ìí¬ë¦¿ê°ë 'ì
 ë¦¬ë´ì¼íê³ , ì ê· íë§ ê½ê¸¸ì ì¡°ì±íë ë± ë´ê½ì íì©í
@@ -741,826 +731,237 @@
 completed form. Args: - text (`Union[str, List[str], Tuple[str]`): single text
 or list of texts - num_workers (`Union[int, str]`): the number of
 multiprocessing workers Returns: - `Union[bool, List[bool]]`: whether the given
 text is in completed form or not Examples: ```python >>> from kss import Kss
 >>> is_completed_form = Kss("is_completed_form") >>> text = "ë°±" >>> output =
 is_completed_form(text) >>> print(output) True >>> text = "ë´¯" >>> output =
 is_completed_form(text) >>> print(output) False ``` 27.
-get_all_completed_form_hangul_chars This returns all non-completed form Hangul
-characters. Returns: - `List[str]`: all non-completed form Hangul characters
+get_all_completed_form_hangul_chars This returns all completed form Hangul
+characters. Returns: - `List[str]`: all completed form Hangul characters
 Examples: ```python >>> from kss import Kss >>>
-get_all_incompleted_form_hangul_chars = Kss
-("get_all_incompleted_form_hangul_chars") >>> output =
-get_all_incompleted_form_hangul_chars() >>> print(output) ['ê°', 'ê°', 'ê°',
-'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°¡', 'ê°¢',
-'ê°£', 'ê°¥', 'ê°¦', 'ê°§', 'ê°¨', 'ê°©', 'ê°ª', 'ê°«', 'ê°®', 'ê°²', 'ê°³',
-'ê°´', 'ê°µ', 'ê°¶', 'ê°·', 'ê°º', 'ê°»', 'ê°½', 'ê°¾', 'ê°¿', 'ê±', 'ê±',
-'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
-'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
-'ê±', 'ê±', 'ê± ', 'ê±¡', 'ê±¢', 'ê±£', 'ê±¤', 'ê±¥', 'ê±¦', 'ê±§', 'ê±¨',
-'ê±©', 'ê±ª', 'ê±«', 'ê±¬', 'ê±­', 'ê±®', 'ê±¯', 'ê±²', 'ê±³', 'ê±µ', 'ê±¶',
-'ê±¹', 'ê±»', 'ê±¼', 'ê±½', 'ê±¾', 'ê±¿', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²',
-'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²',
-'ê²', 'ê²¢', 'ê²£', 'ê²¤', 'ê²¥', 'ê²¦', 'ê²§', 'ê²«', 'ê²­', 'ê²®', 'ê²±',
-'ê²²', 'ê²³', 'ê²´', 'ê²µ', 'ê²¶', 'ê²·', 'ê²º', 'ê²¾', 'ê²¿', 'ê³', 'ê³',
-'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³',
-'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³',
-'ê³', 'ê³', 'ê³¢', 'ê³£', 'ê³¥', 'ê³¦', 'ê³©', 'ê³«', 'ê³­', 'ê³®', 'ê³²',
-'ê³´', 'ê³·', 'ê³¸', 'ê³¹', 'ê³º', 'ê³»', 'ê³¾', 'ê³¿', 'ê´', 'ê´', 'ê´',
-'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´',
-'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´¡', 'ê´¢',
-'ê´£', 'ê´¤', 'ê´¥', 'ê´¦', 'ê´§', 'ê´¨', 'ê´ª', 'ê´«', 'ê´®', 'ê´¯', 'ê´°',
-'ê´±', 'ê´²', 'ê´³', 'ê´¶', 'ê´·', 'ê´¹', 'ê´º', 'ê´»', 'ê´½', 'ê´¾', 'ê´¿',
-'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ',
-'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ',
-'êµ', 'êµ', 'êµ', 'êµ ', 'êµ¢', 'êµ¤', 'êµ¥', 'êµ¦', 'êµ§', 'êµ¨', 'êµ©',
-'êµª', 'êµ«', 'êµ®', 'êµ¯', 'êµ±', 'êµ²', 'êµ·', 'êµ¸', 'êµ¹', 'êµº', 'êµ¾',
-'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶',
-'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶',
-'ê¶', 'ê¶', 'ê¶ ', 'ê¶¡', 'ê¶¢', 'ê¶£', 'ê¶¥', 'ê¶¦', 'ê¶§', 'ê¶¨', 'ê¶©',
-'ê¶ª', 'ê¶«', 'ê¶¬', 'ê¶­', 'ê¶®', 'ê¶¯', 'ê¶°', 'ê¶±', 'ê¶²', 'ê¶³', 'ê¶´',
-'ê¶µ', 'ê¶¶', 'ê¶¸', 'ê¶¹', 'ê¶º', 'ê¶»', 'ê¶¼', 'ê¶½', 'ê¶¾', 'ê¶¿', 'ê·',
-'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·',
-'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·',
-'ê·', 'ê·¡', 'ê·¢', 'ê·£', 'ê·¥', 'ê·¦', 'ê·§', 'ê·¨', 'ê·©', 'ê·ª', 'ê·«',
-'ê·¬', 'ê·­', 'ê·®', 'ê·¯', 'ê·°', 'ê·±', 'ê·²', 'ê·³', 'ê·´', 'ê·µ', 'ê·¶',
-'ê··', 'ê·º', 'ê·»', 'ê·½', 'ê·¾', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸',
-'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸',
-'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸ ', 'ê¸¡', 'ê¸¢',
-'ê¸£', 'ê¸¤', 'ê¸¥', 'ê¸¦', 'ê¸§', 'ê¸¨', 'ê¸©', 'ê¸ª', 'ê¸«', 'ê¸¬', 'ê¸­',
-'ê¸®', 'ê¸¯', 'ê¸²', 'ê¸³', 'ê¸µ', 'ê¸¶', 'ê¸¹', 'ê¸»', 'ê¸¼', 'ê¸½', 'ê¸¾',
-'ê¸¿', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹',
-'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹¢', 'ê¹£', 'ê¹¤', 'ê¹¦',
-'ê¹§', 'ê¹ª', 'ê¹«', 'ê¹­', 'ê¹®', 'ê¹¯', 'ê¹±', 'ê¹²', 'ê¹³', 'ê¹´', 'ê¹µ',
-'ê¹¶', 'ê¹·', 'ê¹º', 'ê¹¾', 'ê¹¿', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº',
-'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº',
-'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº',
-'êº', 'êº ', 'êº¡', 'êº¢', 'êº£', 'êº¤', 'êº¥', 'êº¦', 'êº§', 'êº¨', 'êº©',
-'êºª', 'êº«', 'êº¬', 'êº­', 'êº®', 'êº¯', 'êº°', 'êº±', 'êº²', 'êº³', 'êº´',
-'êºµ', 'êº¶', 'êº·', 'êº¸', 'êº¹', 'êºº', 'êº»', 'êº¿', 'ê»', 'ê»', 'ê»',
-'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»',
-'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê» ', 'ê»¡', 'ê»¢',
-'ê»£', 'ê»¤', 'ê»¥', 'ê»¦', 'ê»§', 'ê»©', 'ê»ª', 'ê»¬', 'ê»®', 'ê»¯', 'ê»°',
-'ê»±', 'ê»²', 'ê»³', 'ê»µ', 'ê»¶', 'ê»·', 'ê»¹', 'ê»º', 'ê»»', 'ê»½', 'ê»¾',
-'ê»¿', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼',
-'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼',
-'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼ ', 'ê¼¡', 'ê¼¢', 'ê¼£',
-'ê¼¤', 'ê¼¥', 'ê¼¦', 'ê¼§', 'ê¼¨', 'ê¼©', 'ê¼ª', 'ê¼«', 'ê¼®', 'ê¼¯', 'ê¼±',
-'ê¼³', 'ê¼µ', 'ê¼¶', 'ê¼·', 'ê¼¸', 'ê¼¹', 'ê¼º', 'ê¼»', 'ê¼¾', 'ê½', 'ê½',
-'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½',
-'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½',
-'ê½ ', 'ê½¡', 'ê½¢', 'ê½£', 'ê½¦', 'ê½§', 'ê½¨', 'ê½©', 'ê½ª', 'ê½«', 'ê½¬',
-'ê½­', 'ê½®', 'ê½¯', 'ê½°', 'ê½±', 'ê½²', 'ê½³', 'ê½´', 'ê½µ', 'ê½¶', 'ê½·',
-'ê½¸', 'ê½º', 'ê½»', 'ê½¼', 'ê½½', 'ê½¾', 'ê½¿', 'ê¾', 'ê¾', 'ê¾', 'ê¾',
-'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾',
-'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾ ',
-'ê¾¡', 'ê¾¢', 'ê¾£', 'ê¾¤', 'ê¾¥', 'ê¾¦', 'ê¾§', 'ê¾¨', 'ê¾©', 'ê¾ª', 'ê¾«',
-'ê¾¬', 'ê¾­', 'ê¾®', 'ê¾¯', 'ê¾°', 'ê¾±', 'ê¾²', 'ê¾³', 'ê¾´', 'ê¾µ', 'ê¾¶',
-'ê¾·', 'ê¾º', 'ê¾»', 'ê¾½', 'ê¾¾', 'ê¾¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿',
-'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿',
-'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿ ', 'ê¿¡', 'ê¿¢', 'ê¿£',
-'ê¿¤', 'ê¿¥', 'ê¿¦', 'ê¿§', 'ê¿ª', 'ê¿«', 'ê¿¬', 'ê¿­', 'ê¿®', 'ê¿¯', 'ê¿²',
-'ê¿³', 'ê¿µ', 'ê¿¶', 'ê¿·', 'ê¿¹', 'ê¿º', 'ê¿»', 'ê¿¼', 'ê¿½', 'ê¿¾', 'ê¿¿',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë©',
-'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´',
-'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡',
-'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬',
-'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·',
-'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª',
-'ë°', 'ë²', 'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬',
-'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·',
-'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë¦', 'ë§',
-'ë©', 'ëª', 'ë«', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë¶',
-'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥',
-'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°',
-'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ëº', 'ë»', 'ë½', 'ë¾',
-'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ëª', 'ë«',
-'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶',
-'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª',
-'ë«', 'ë­', 'ë®', 'ë¯', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·',
-'ë¸', 'ëº', 'ë¼', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥',
-'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°',
-'ë±', 'ë²', 'ë³', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë½',
-'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë¡',
-'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®',
-'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»',
-'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë¢', 'ë¤', 'ë§', 'ë¨', 'ë©', 'ë«', 'ë­',
-'ë®', 'ë¯', 'ë±', 'ë²', 'ë³', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº',
-'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë£', 'ë§', 'ë©',
-'ëª', 'ë°', 'ë±', 'ë²', 'ë¶', 'ë¼', 'ë½', 'ë¾', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢',
-'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­',
-'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸',
-'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡',
-'ë¢', 'ë£', 'ë¦', 'ë¨', 'ëª', 'ë¬', 'ë­', 'ë¯', 'ë²', 'ë³', 'ëµ',
-'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ëª', 'ë«', 'ë­', 'ë®',
-'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹',
-'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ëª',
-'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ',
-'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦',
-'ë§', 'ëª', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ëµ',
-'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë¢', 'ë¤', 'ë¦', 'ë§', 'ë¨', 'ë©',
-'ëª', 'ë«', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ',
-'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¥',
-'ë¦', 'ë§', 'ë©', 'ëª', 'ë«', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²',
-'ë³', 'ë´', 'ë¶', 'ë¸', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë¡', 'ë¢', 'ë¥', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë®',
-'ë°', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼',
-'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢',
-'ë£', 'ë¦', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë²', 'ë³', 'ëµ', 'ë¶',
-'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§',
-'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²',
-'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½',
-'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë¢', 'ë£', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ë¬', 'ë­', 'ë®', 'ë¯',
-'ë²', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë¾', 'ë¿', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ',
-'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«',
-'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·',
-'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¦', 'ë§', 'ë¨',
-'ë©', 'ëª', 'ë«', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ëµ',
-'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢',
-'ë£', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯',
-'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº',
-'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª',
-'ë­', 'ë®', 'ë¯', 'ë°', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸',
-'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥',
-'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë±',
-'ë²', 'ë³', 'ëµ', 'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾',
-'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢',
-'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª', 'ë«', 'ë­', 'ë®', 'ë±', 'ë²',
-'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ëº', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¥', 'ë¦', 'ë§', 'ë©',
-'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë²', 'ë´', 'ë¶', 'ë·', 'ë¸',
-'ë¹', 'ëº', 'ë»', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª', 'ë®',
-'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼',
-'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª',
-'ë«', 'ë®', 'ë¯', 'ë±', 'ë²', 'ë³', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹',
-'ëº', 'ë»', 'ë¾', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ',
-'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ',
-'ë ', 'ë ', 'ë  ', 'ë ¡', 'ë ¢', 'ë £', 'ë ¦', 'ë §', 'ë ©', 'ë ª', 'ë «',
-'ë ­', 'ë ®', 'ë ¯', 'ë °', 'ë ±', 'ë ²', 'ë ³', 'ë ¶', 'ë º', 'ë »', 'ë ¼',
-'ë ½', 'ë ¾', 'ë ¿', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡',
-'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡',
-'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡¡', 'ë¡¢', 'ë¡£', 'ë¡¥',
-'ë¡¦', 'ë¡§', 'ë¡¨', 'ë¡©', 'ë¡ª', 'ë¡«', 'ë¡®', 'ë¡°', 'ë¡²', 'ë¡³', 'ë¡´',
-'ë¡µ', 'ë¡¶', 'ë¡·', 'ë¡¹', 'ë¡º', 'ë¡»', 'ë¡½', 'ë¡¾', 'ë¡¿', 'ë¢', 'ë¢',
-'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢',
-'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢',
-'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢ ', 'ë¢¡', 'ë¢¢', 'ë¢£',
-'ë¢¤', 'ë¢¥', 'ë¢¦', 'ë¢§', 'ë¢©', 'ë¢ª', 'ë¢«', 'ë¢¬', 'ë¢­', 'ë¢®', 'ë¢¯',
-'ë¢±', 'ë¢²', 'ë¢³', 'ë¢µ', 'ë¢¶', 'ë¢·', 'ë¢¹', 'ë¢º', 'ë¢»', 'ë¢¼', 'ë¢½',
-'ë¢¾', 'ë¢¿', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£',
-'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£',
-'ë£', 'ë£', 'ë£', 'ë£ ', 'ë£¢', 'ë££', 'ë£¤', 'ë£¥', 'ë£¦', 'ë£§', 'ë£ª',
-'ë£«', 'ë£­', 'ë£®', 'ë£¯', 'ë£±', 'ë£²', 'ë£³', 'ë£´', 'ë£µ', 'ë£¶', 'ë£·',
-'ë£º', 'ë£¼', 'ë£¾', 'ë£¿', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤',
-'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤',
-'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤',
-'ë¤', 'ë¤¡', 'ë¤¢', 'ë¤£', 'ë¤¤', 'ë¤¥', 'ë¤¦', 'ë¤§', 'ë¤¨', 'ë¤©', 'ë¤ª',
-'ë¤«', 'ë¤¬', 'ë¤­', 'ë¤®', 'ë¤¯', 'ë¤°', 'ë¤±', 'ë¤²', 'ë¤³', 'ë¤´', 'ë¤µ',
-'ë¤¶', 'ë¤·', 'ë¤¸', 'ë¤¹', 'ë¤º', 'ë¤»', 'ë¤¾', 'ë¤¿', 'ë¥', 'ë¥', 'ë¥',
-'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥',
-'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥¡',
-'ë¥¢', 'ë¥£', 'ë¥¤', 'ë¥¥', 'ë¥¦', 'ë¥§', 'ë¥ª', 'ë¥¬', 'ë¥®', 'ë¥¯', 'ë¥°',
-'ë¥±', 'ë¥²', 'ë¥³', 'ë¥¶', 'ë¥·', 'ë¥¹', 'ë¥º', 'ë¥»', 'ë¥½', 'ë¥¾', 'ë¥¿',
-'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦',
-'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦',
-'ë¦', 'ë¦', 'ë¦', 'ë¦ ', 'ë¦¡', 'ë¦¢', 'ë¦£', 'ë¦¤', 'ë¦¥', 'ë¦¦', 'ë¦§',
-'ë¦¨', 'ë¦©', 'ë¦ª', 'ë¦«', 'ë¦®', 'ë¦¯', 'ë¦±', 'ë¦²', 'ë¦³', 'ë¦µ', 'ë¦¶',
-'ë¦·', 'ë¦¸', 'ë¦¹', 'ë¦º', 'ë¦»', 'ë¦¾', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§',
-'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§',
-'ë§', 'ë§', 'ë§ ', 'ë§¢', 'ë§¦', 'ë§§', 'ë§©', 'ë§ª', 'ë§«', 'ë§­', 'ë§®',
-'ë§¯', 'ë§°', 'ë§±', 'ë§²', 'ë§³', 'ë§¶', 'ë§»', 'ë§¼', 'ë§½', 'ë§¾', 'ë§¿',
-'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨',
-'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨',
-'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨ ', 'ë¨¡', 'ë¨¢', 'ë¨£', 'ë¨¤',
-'ë¨¥', 'ë¨¦', 'ë¨§', 'ë¨¨', 'ë¨©', 'ë¨ª', 'ë¨«', 'ë¨¬', 'ë¨­', 'ë¨®', 'ë¨¯',
-'ë¨°', 'ë¨±', 'ë¨²', 'ë¨³', 'ë¨´', 'ë¨µ', 'ë¨¶', 'ë¨·', 'ë¨º', 'ë¨»', 'ë¨½',
-'ë¨¾', 'ë¨¿', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©',
-'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©',
-'ë© ', 'ë©¡', 'ë©¢', 'ë©£', 'ë©¦', 'ë©ª', 'ë©«', 'ë©¬', 'ë©­', 'ë©®', 'ë©¯',
-'ë©²', 'ë©³', 'ë©µ', 'ë©¶', 'ë©·', 'ë©¹', 'ë©º', 'ë©»', 'ë©¼', 'ë©½', 'ë©¾',
-'ë©¿', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª',
-'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª',
-'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª ', 'ëª¡', 'ëª¢', 'ëª£', 'ëª¤',
-'ëª¥', 'ëª¦', 'ëª§', 'ëªª', 'ëª­', 'ëª®', 'ëª¯', 'ëª±', 'ëª³', 'ëª´', 'ëªµ',
-'ëª¶', 'ëª·', 'ëªº', 'ëª¼', 'ëª¾', 'ëª¿', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«',
-'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«',
-'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«',
-'ë«', 'ë« ', 'ë«¡', 'ë«¢', 'ë«£', 'ë«¤', 'ë«¥', 'ë«¦', 'ë«§', 'ë«¨', 'ë«©',
-'ë«ª', 'ë««', 'ë«¬', 'ë«­', 'ë«®', 'ë«¯', 'ë«°', 'ë«±', 'ë«²', 'ë«³', 'ë«´',
-'ë«µ', 'ë«¶', 'ë«·', 'ë«¸', 'ë«¹', 'ë«º', 'ë«»', 'ë«½', 'ë«¾', 'ë«¿', 'ë¬',
-'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬',
-'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬',
-'ë¬', 'ë¬', 'ë¬¡', 'ë¬¢', 'ë¬£', 'ë¬¤', 'ë¬¥', 'ë¬¦', 'ë¬§', 'ë¬¨', 'ë¬ª',
-'ë¬¬', 'ë¬­', 'ë¬®', 'ë¬¯', 'ë¬°', 'ë¬±', 'ë¬²', 'ë¬³', 'ë¬·', 'ë¬¹', 'ë¬º',
-'ë¬¿', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­',
-'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­',
-'ë­', 'ë­', 'ë­ ', 'ë­¢', 'ë­¤', 'ë­¥', 'ë­¦', 'ë­§', 'ë­¨', 'ë­©', 'ë­ª',
-'ë­«', 'ë­­', 'ë­®', 'ë­¯', 'ë­°', 'ë­±', 'ë­²', 'ë­³', 'ë­´', 'ë­µ', 'ë­¶',
-'ë­·', 'ë­¸', 'ë­¹', 'ë­º', 'ë­»', 'ë­¼', 'ë­½', 'ë­¾', 'ë­¿', 'ë®', 'ë®',
-'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®',
-'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®',
-'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë® ', 'ë®¡', 'ë®¢', 'ë®£', 'ë®¥', 'ë®¦',
-'ë®§', 'ë®©', 'ë®ª', 'ë®«', 'ë®­', 'ë®®', 'ë®¯', 'ë®°', 'ë®±', 'ë®²', 'ë®³',
-'ë®µ', 'ë®¶', 'ë®¸', 'ë®¹', 'ë®º', 'ë®»', 'ë®¼', 'ë®½', 'ë®¾', 'ë®¿', 'ë¯',
-'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯',
-'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯',
-'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯ ', 'ë¯¡', 'ë¯¢', 'ë¯£', 'ë¯¤', 'ë¯¥', 'ë¯¦',
-'ë¯§', 'ë¯¨', 'ë¯©', 'ë¯ª', 'ë¯«', 'ë¯¬', 'ë¯­', 'ë¯®', 'ë¯¯', 'ë¯°', 'ë¯±',
-'ë¯²', 'ë¯³', 'ë¯´', 'ë¯µ', 'ë¯¶', 'ë¯·', 'ë¯º', 'ë¯»', 'ë¯½', 'ë¯¾', 'ë°',
-'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°',
-'ë°', 'ë° ', 'ë°¡', 'ë°¢', 'ë°£', 'ë°¦', 'ë°¨', 'ë°ª', 'ë°«', 'ë°¬', 'ë°®',
-'ë°¯', 'ë°²', 'ë°³', 'ë°µ', 'ë°¶', 'ë°·', 'ë°¹', 'ë°º', 'ë°»', 'ë°¼', 'ë°½',
-'ë°¾', 'ë°¿', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±',
-'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±',
-'ë±', 'ë±', 'ë± ', 'ë±¡', 'ë±¢', 'ë±£', 'ë±¤', 'ë±¥', 'ë±¦', 'ë±§', 'ë±¨',
-'ë±©', 'ë±ª', 'ë±«', 'ë±¬', 'ë±­', 'ë±®', 'ë±¯', 'ë±°', 'ë±±', 'ë±²', 'ë±³',
-'ë±´', 'ë±µ', 'ë±¶', 'ë±·', 'ë±¸', 'ë±¹', 'ë±º', 'ë±»', 'ë±¼', 'ë±½', 'ë±¾',
-'ë±¿', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²',
-'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²',
-'ë²¢', 'ë²£', 'ë²¥', 'ë²¦', 'ë²©', 'ë²ª', 'ë²«', 'ë²¬', 'ë²­', 'ë²®', 'ë²¯',
-'ë²²', 'ë²¶', 'ë²·', 'ë²¸', 'ë²¹', 'ë²º', 'ë²»', 'ë²¾', 'ë²¿', 'ë³', 'ë³',
-'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³',
-'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³ ',
-'ë³¡', 'ë³¢', 'ë³£', 'ë³¤', 'ë³¥', 'ë³¦', 'ë³§', 'ë³¨', 'ë³©', 'ë³ª', 'ë³«',
-'ë³¬', 'ë³­', 'ë³®', 'ë³¯', 'ë³°', 'ë³±', 'ë³²', 'ë³³', 'ë³·', 'ë³¹', 'ë³º',
-'ë³»', 'ë³½', 'ë³¾', 'ë³¿', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´',
-'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´',
-'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´ ', 'ë´¡', 'ë´¢',
-'ë´£', 'ë´¥', 'ë´¦', 'ë´§', 'ë´¨', 'ë´©', 'ë´ª', 'ë´«', 'ë´­', 'ë´®', 'ë´¯',
-'ë´°', 'ë´±', 'ë´²', 'ë´³', 'ë´´', 'ë´µ', 'ë´¶', 'ë´·', 'ë´¸', 'ë´¹', 'ë´º',
-'ë´»', 'ë´¼', 'ë´½', 'ë´¾', 'ë´¿', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ',
-'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ',
-'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ ', 'ëµ¡', 'ëµ¢',
-'ëµ£', 'ëµ¥', 'ëµ¦', 'ëµ§', 'ëµ©', 'ëµª', 'ëµ«', 'ëµ¬', 'ëµ­', 'ëµ®', 'ëµ¯',
-'ëµ°', 'ëµ±', 'ëµ²', 'ëµ³', 'ëµ´', 'ëµµ', 'ëµ¶', 'ëµ·', 'ëµ¸', 'ëµ¹', 'ëµº',
-'ëµ»', 'ëµ¼', 'ëµ½', 'ëµ¾', 'ëµ¿', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶',
-'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶',
-'ë¶', 'ë¶ ', 'ë¶¡', 'ë¶¢', 'ë¶£', 'ë¶¥', 'ë¶¦', 'ë¶§', 'ë¶¨', 'ë¶©', 'ë¶ª',
-'ë¶«', 'ë¶¬', 'ë¶­', 'ë¶®', 'ë¶¯', 'ë¶±', 'ë¶²', 'ë¶³', 'ë¶´', 'ë¶µ', 'ë¶¶',
-'ë¶·', 'ë¶¹', 'ë¶º', 'ë¶»', 'ë¶¼', 'ë¶½', 'ë¶¾', 'ë¶¿', 'ë·', 'ë·', 'ë·',
-'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·',
-'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·',
-'ë·', 'ë·', 'ë·', 'ë· ', 'ë·¡', 'ë·¢', 'ë·£', 'ë·¤', 'ë·¥', 'ë·¦', 'ë·§',
-'ë·¨', 'ë·ª', 'ë·«', 'ë·¬', 'ë·­', 'ë·®', 'ë·¯', 'ë·±', 'ë·²', 'ë·³', 'ë·µ',
-'ë·¶', 'ë··', 'ë·¹', 'ë·º', 'ë·»', 'ë·¼', 'ë·½', 'ë·¾', 'ë·¿', 'ë¸', 'ë¸',
-'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸',
-'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸ ', 'ë¸¡',
-'ë¸¢', 'ë¸£', 'ë¸¤', 'ë¸¥', 'ë¸¦', 'ë¸§', 'ë¸¨', 'ë¸©', 'ë¸ª', 'ë¸«', 'ë¸¬',
-'ë¸­', 'ë¸®', 'ë¸¯', 'ë¸°', 'ë¸±', 'ë¸²', 'ë¸³', 'ë¸´', 'ë¸µ', 'ë¸¶', 'ë¸·',
-'ë¸¸', 'ë¸¹', 'ë¸º', 'ë¸»', 'ë¸¼', 'ë¸½', 'ë¸¾', 'ë¸¿', 'ë¹', 'ë¹', 'ë¹',
-'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹',
-'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹¢', 'ë¹£', 'ë¹¥', 'ë¹¦',
-'ë¹§', 'ë¹©', 'ë¹«', 'ë¹¬', 'ë¹­', 'ë¹®', 'ë¹¯', 'ë¹²', 'ë¹¶', 'ë¹·', 'ë¹¸',
-'ë¹¹', 'ë¹º', 'ë¹¾', 'ë¹¿', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº',
-'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº',
-'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº ', 'ëº¡', 'ëº¢', 'ëº£', 'ëº¤', 'ëº¥',
-'ëº¦', 'ëº§', 'ëº©', 'ëºª', 'ëº«', 'ëº¬', 'ëº­', 'ëº®', 'ëº¯', 'ëº°', 'ëº±',
-'ëº²', 'ëº³', 'ëº´', 'ëºµ', 'ëº¶', 'ëº·', 'ëº¸', 'ëº¹', 'ëºº', 'ëº»', 'ëº¼',
-'ëº½', 'ëº¾', 'ëº¿', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»',
-'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»',
-'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»¡', 'ë»¢', 'ë»¦',
-'ë»§', 'ë»¨', 'ë»©', 'ë»ª', 'ë»«', 'ë»­', 'ë»®', 'ë»¯', 'ë»°', 'ë»±', 'ë»²',
-'ë»³', 'ë»´', 'ë»µ', 'ë»¶', 'ë»·', 'ë»¸', 'ë»¹', 'ë»º', 'ë»»', 'ë»¼', 'ë»½',
-'ë»¾', 'ë»¿', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼',
-'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼',
-'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼ ', 'ë¼¡', 'ë¼¢', 'ë¼£', 'ë¼¤', 'ë¼¥', 'ë¼¦',
-'ë¼§', 'ë¼¨', 'ë¼©', 'ë¼ª', 'ë¼«', 'ë¼¬', 'ë¼­', 'ë¼®', 'ë¼¯', 'ë¼°', 'ë¼±',
-'ë¼²', 'ë¼³', 'ë¼´', 'ë¼µ', 'ë¼¶', 'ë¼·', 'ë¼¸', 'ë¼¹', 'ë¼º', 'ë¼»', 'ë¼¼',
-'ë¼½', 'ë¼¾', 'ë¼¿', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½',
-'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½',
-'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½ ', 'ë½¡', 'ë½¢', 'ë½£', 'ë½¤',
-'ë½¥', 'ë½¦', 'ë½§', 'ë½¨', 'ë½©', 'ë½ª', 'ë½«', 'ë½¬', 'ë½­', 'ë½®', 'ë½¯',
-'ë½°', 'ë½±', 'ë½²', 'ë½³', 'ë½´', 'ë½µ', 'ë½¶', 'ë½·', 'ë½¸', 'ë½¹', 'ë½º',
-'ë½»', 'ë½¼', 'ë½½', 'ë½¾', 'ë½¿', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾',
-'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾',
-'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾',
-'ë¾', 'ë¾', 'ë¾', 'ë¾ ', 'ë¾¡', 'ë¾¢', 'ë¾£', 'ë¾¤', 'ë¾¥', 'ë¾¦', 'ë¾§',
-'ë¾¨', 'ë¾©', 'ë¾ª', 'ë¾«', 'ë¾¬', 'ë¾­', 'ë¾®', 'ë¾¯', 'ë¾±', 'ë¾²', 'ë¾³',
-'ë¾´', 'ë¾µ', 'ë¾¶', 'ë¾·', 'ë¾¸', 'ë¾¹', 'ë¾º', 'ë¾»', 'ë¾¼', 'ë¾½', 'ë¾¾',
-'ë¾¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿',
-'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿',
-'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿ ', 'ë¿¢', 'ë¿£', 'ë¿¤', 'ë¿¥', 'ë¿¦', 'ë¿§',
-'ë¿¨', 'ë¿©', 'ë¿ª', 'ë¿«', 'ë¿¬', 'ë¿­', 'ë¿®', 'ë¿¯', 'ë¿°', 'ë¿±', 'ë¿²',
-'ë¿³', 'ë¿´', 'ë¿µ', 'ë¿¶', 'ë¿·', 'ë¿¸', 'ë¿¹', 'ë¿º', 'ë¿»', 'ë¿¼', 'ë¿½',
-'ë¿¾', 'ë¿¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ì¨', 'ì©',
-'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì´',
-'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì½', 'ì¾', 'ì¿', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥',
-'ì¦', 'ì§', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²',
-'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½',
-'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¢', 'ì¤', 'ì¦',
-'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì®', 'ì±', 'ì²', 'ì·', 'ì¸', 'ì¹',
-'ìº', 'ì»', 'ì¾', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì­',
-'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì¶', 'ì¸', 'ìº', 'ì»', 'ì¼',
-'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì¥', 'ì¨', 'ì©', 'ìª', 'ì«',
-'ì®', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì·', 'ìº', 'ì»', 'ì½', 'ì¾', 'ì¿',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¦', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯',
-'ì±', 'ì²', 'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½',
-'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì ', 'ì¢', 'ì£', 'ì¤', 'ì¦', 'ì§', 'ìª', 'ì«', 'ì­',
-'ì®', 'ì¯', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹',
-'ìº', 'ì»', 'ì¼', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢',
-'ì£', 'ì¥', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯',
-'ì²', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì¿',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ìª', 'ì¬', 'ì®', 'ì°',
-'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾',
-'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¦',
-'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì®', 'ì¯', 'ì±', 'ì²', 'ì³', 'ìµ',
-'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ',
-'ì¡', 'ì¢', 'ì£', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì®', 'ì¯', 'ì°',
-'ì±', 'ì²', 'ì³', 'ì¶', 'ì¸', 'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì¥',
-'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì®', 'ì°', 'ì²', 'ì³', 'ì´', 'ìµ',
-'ì·', 'ìº', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¦', 'ì§',
-'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì´',
-'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡',
-'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ìª', 'ì«', 'ì­', 'ì®', 'ì¯',
-'ì±', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ìº', 'ì»', 'ì¾', 'ì¿', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¤',
-'ì¥', 'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯',
-'ì°', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº',
-'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡',
-'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ìª', 'ì«', 'ì¬', 'ì®', 'ì¯', 'ì°',
-'ì±', 'ì²', 'ì³', 'ì¶', 'ì·', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾',
-'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡',
-'ì¢', 'ì£', 'ì¥', 'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì­', 'ì®',
-'ì¯', 'ì±', 'ì²', 'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»',
-'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì­', 'ì®',
-'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì¶', 'ì·', 'ì¸', 'ìº', 'ì»', 'ì¼',
-'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ',
-'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì«',
-'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶',
-'ì·', 'ì¹', 'ìº', 'ì»', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¤',
-'ì¥', 'ì¦', 'ì§', 'ì¨', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì²',
-'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¹', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ìª',
-'ì«', 'ì­', 'ì®', 'ì¯', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·',
-'ìº', 'ì¼', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¢', 'ì£',
-'ì¥', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì²',
-'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì¿', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤',
-'ì¥', 'ì¦', 'ì§', 'ì¨', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°',
-'ì±', 'ì²', 'ì³', 'ì¶', 'ì·', 'ìº', 'ì¿', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì¢', 'ì¤', 'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª',
-'ì«', 'ì¯', 'ì±', 'ì²', 'ì³', 'ìµ', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢',
-'ì£', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì¯', 'ì±', 'ì²', 'ì¶', 'ì¸',
-'ìº', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§',
-'ì¨', 'ì©', 'ìª', 'ì«', 'ì­', 'ì®', 'ì°', 'ì²', 'ì³', 'ì´', 'ìµ',
-'ì¶', 'ì·', 'ìº', 'ì»', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢',
-'ì£', 'ì¦', 'ì¨', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì²', 'ì³',
-'ìµ', 'ì¶', 'ì·', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¢', 'ì£', 'ì¤',
-'ì¥', 'ì¦', 'ì§', 'ìª', 'ì«', 'ì­', 'ì®', 'ì¯', 'ì±', 'ì²', 'ì³',
-'ì´', 'ìµ', 'ì¶', 'ì·', 'ìº', 'ì»', 'ì¼', 'ì¾', 'ì¿', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì¢', 'ì£', 'ì¥', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®',
-'ì¯', 'ì²', 'ì´', 'ì¶', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì¿', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦',
-'ì§', 'ì©', 'ìª', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³',
-'ì¶', 'ì·', 'ì¹', 'ìº', 'ì»', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì¢', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì®', 'ì¯', 'ì±', 'ì²',
-'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ',
-'ì¡', 'ì¢', 'ì£', 'ì¥', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì­', 'ì®',
-'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹',
-'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ',
-'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ',
-'ì ', 'ì ', 'ì ', 'ì ', 'ì ¡', 'ì ¢', 'ì £', 'ì ¥', 'ì ¦', 'ì §', 'ì ¨',
-'ì ©', 'ì ª', 'ì «', 'ì ®', 'ì °', 'ì ²', 'ì ³', 'ì ´', 'ì µ', 'ì ¶', 'ì ·',
-'ì ¹', 'ì º', 'ì »', 'ì ½', 'ì ¾', 'ì ¿', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡',
-'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡',
-'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡ ',
-'ì¡¡', 'ì¡¢', 'ì¡£', 'ì¡¤', 'ì¡¥', 'ì¡¦', 'ì¡§', 'ì¡¨', 'ì¡©', 'ì¡ª', 'ì¡«',
-'ì¡¬', 'ì¡­', 'ì¡®', 'ì¡¯', 'ì¡²', 'ì¡³', 'ì¡µ', 'ì¡¶', 'ì¡·', 'ì¡¹', 'ì¡»',
-'ì¡¼', 'ì¡½', 'ì¡¾', 'ì¡¿', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢',
-'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢',
-'ì¢', 'ì¢', 'ì¢ ', 'ì¢¢', 'ì¢£', 'ì¢¤', 'ì¢¥', 'ì¢¦', 'ì¢§', 'ì¢©', 'ì¢ª',
-'ì¢«', 'ì¢¬', 'ì¢­', 'ì¢®', 'ì¢¯', 'ì¢°', 'ì¢±', 'ì¢²', 'ì¢³', 'ì¢´', 'ì¢µ',
-'ì¢¶', 'ì¢·', 'ì¢¸', 'ì¢¹', 'ì¢º', 'ì¢»', 'ì¢¾', 'ì¢¿', 'ì£', 'ì£', 'ì£',
-'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£',
-'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£',
-'ì£¢', 'ì££', 'ì£¥', 'ì£¦', 'ì£§', 'ì£¨', 'ì£©', 'ì£ª', 'ì£«', 'ì£¬', 'ì£­',
-'ì£®', 'ì£¯', 'ì£°', 'ì£±', 'ì£²', 'ì£³', 'ì£´', 'ì£¶', 'ì£·', 'ì£¸', 'ì£¹',
-'ì£º', 'ì£»', 'ì£¾', 'ì£¿', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤',
-'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤',
-'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤ ', 'ì¤¡', 'ì¤¢', 'ì¤£', 'ì¤¤', 'ì¤¥',
-'ì¤¦', 'ì¤§', 'ì¤¨', 'ì¤©', 'ì¤ª', 'ì¤«', 'ì¤­', 'ì¤®', 'ì¤¯', 'ì¤°', 'ì¤±',
-'ì¤²', 'ì¤³', 'ì¤µ', 'ì¤¶', 'ì¤·', 'ì¤¸', 'ì¤¹', 'ì¤º', 'ì¤»', 'ì¤¼', 'ì¤½',
-'ì¤¾', 'ì¤¿', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥',
-'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥',
-'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥¢', 'ì¥¤', 'ì¥¥',
-'ì¥¦', 'ì¥§', 'ì¥¨', 'ì¥©', 'ì¥ª', 'ì¥«', 'ì¥­', 'ì¥®', 'ì¥¯', 'ì¥±', 'ì¥²',
-'ì¥³', 'ì¥µ', 'ì¥¶', 'ì¥·', 'ì¥¸', 'ì¥¹', 'ì¥º', 'ì¥»', 'ì¥½', 'ì¥¾', 'ì¥¿',
-'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦',
-'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦',
-'ì¦', 'ì¦', 'ì¦ ', 'ì¦¡', 'ì¦¢', 'ì¦£', 'ì¦¤', 'ì¦¥', 'ì¦¦', 'ì¦§', 'ì¦¨',
-'ì¦©', 'ì¦ª', 'ì¦«', 'ì¦¬', 'ì¦­', 'ì¦®', 'ì¦¯', 'ì¦°', 'ì¦±', 'ì¦²', 'ì¦³',
-'ì¦´', 'ì¦µ', 'ì¦¶', 'ì¦·', 'ì¦¸', 'ì¦¹', 'ì¦º', 'ì¦»', 'ì¦¼', 'ì¦½', 'ì¦¾',
-'ì¦¿', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§',
-'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§¡', 'ì§£', 'ì§¥', 'ì§¦',
-'ì§¨', 'ì§©', 'ì§ª', 'ì§«', 'ì§®', 'ì§²', 'ì§³', 'ì§´', 'ì§µ', 'ì§¶', 'ì§·',
-'ì§º', 'ì§»', 'ì§½', 'ì§¾', 'ì§¿', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨',
-'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨',
-'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨ ', 'ì¨¡', 'ì¨¢', 'ì¨£',
-'ì¨¤', 'ì¨¥', 'ì¨¦', 'ì¨§', 'ì¨¨', 'ì¨ª', 'ì¨«', 'ì¨¬', 'ì¨­', 'ì¨®', 'ì¨¯',
-'ì¨°', 'ì¨±', 'ì¨²', 'ì¨³', 'ì¨´', 'ì¨µ', 'ì¨¶', 'ì¨·', 'ì¨¸', 'ì¨¹', 'ì¨º',
-'ì¨»', 'ì¨¼', 'ì¨½', 'ì¨¾', 'ì¨¿', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©',
-'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©',
-'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©¢', 'ì©£', 'ì©¤',
-'ì©¥', 'ì©¦', 'ì©§', 'ì©©', 'ì©ª', 'ì©«', 'ì©¬', 'ì©­', 'ì©®', 'ì©¯', 'ì©°',
-'ì©±', 'ì©²', 'ì©³', 'ì©´', 'ì©µ', 'ì©¶', 'ì©·', 'ì©¸', 'ì©¹', 'ì©º', 'ì©»',
-'ì©¼', 'ì©¾', 'ì©¿', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª',
-'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª',
-'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª',
-'ìª ', 'ìª¡', 'ìª¢', 'ìª£', 'ìª¤', 'ìª¥', 'ìª¦', 'ìª§', 'ìª¨', 'ìª©', 'ìªª',
-'ìª«', 'ìª¬', 'ìª­', 'ìª®', 'ìª¯', 'ìª°', 'ìª±', 'ìª²', 'ìª³', 'ìª´', 'ìªµ',
-'ìª¶', 'ìª·', 'ìª¸', 'ìª¹', 'ìªº', 'ìª»', 'ìª¾', 'ìª¿', 'ì«', 'ì«', 'ì«',
-'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«',
-'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«¡', 'ì«¢',
-'ì«£', 'ì«¤', 'ì«¥', 'ì«¦', 'ì«§', 'ì«¨', 'ì«©', 'ì«ª', 'ì««', 'ì«­', 'ì«®',
-'ì«¯', 'ì«°', 'ì«±', 'ì«²', 'ì«³', 'ì«µ', 'ì«¶', 'ì«·', 'ì«¸', 'ì«¹', 'ì«º',
-'ì«»', 'ì«¼', 'ì«½', 'ì«¾', 'ì«¿', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬',
-'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬',
-'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬',
-'ì¬¢', 'ì¬£', 'ì¬¤', 'ì¬¥', 'ì¬¦', 'ì¬§', 'ì¬¨', 'ì¬©', 'ì¬ª', 'ì¬«', 'ì¬¬',
-'ì¬­', 'ì¬®', 'ì¬¯', 'ì¬°', 'ì¬±', 'ì¬²', 'ì¬³', 'ì¬´', 'ì¬µ', 'ì¬¶', 'ì¬·',
-'ì¬¸', 'ì¬¹', 'ì¬º', 'ì¬»', 'ì¬¼', 'ì¬½', 'ì¬¾', 'ì¬¿', 'ì­', 'ì­', 'ì­',
-'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­',
-'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­ ',
-'ì­¡', 'ì­¢', 'ì­£', 'ì­¥', 'ì­¦', 'ì­§', 'ì­¨', 'ì­©', 'ì­ª', 'ì­«', 'ì­¬',
-'ì­­', 'ì­®', 'ì­¯', 'ì­°', 'ì­±', 'ì­²', 'ì­³', 'ì­´', 'ì­µ', 'ì­¶', 'ì­·',
-'ì­º', 'ì­»', 'ì­¼', 'ì­½', 'ì­¾', 'ì­¿', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®',
-'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®',
-'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®',
-'ì®', 'ì®', 'ì®', 'ì®', 'ì® ', 'ì®¡', 'ì®¢', 'ì®£', 'ì®¤', 'ì®¥', 'ì®¦',
-'ì®§', 'ì®¨', 'ì®©', 'ì®ª', 'ì®«', 'ì®¬', 'ì®­', 'ì®®', 'ì®¯', 'ì®°', 'ì®±',
-'ì®²', 'ì®³', 'ì®´', 'ì®µ', 'ì®¶', 'ì®·', 'ì®¹', 'ì®º', 'ì®»', 'ì®¼', 'ì®½',
-'ì®¾', 'ì®¿', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯',
-'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯',
-'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯',
-'ì¯ ', 'ì¯¡', 'ì¯¢', 'ì¯£', 'ì¯¥', 'ì¯¦', 'ì¯¨', 'ì¯ª', 'ì¯«', 'ì¯¬', 'ì¯­',
-'ì¯®', 'ì¯¯', 'ì¯°', 'ì¯±', 'ì¯²', 'ì¯³', 'ì¯´', 'ì¯µ', 'ì¯¶', 'ì¯·', 'ì¯¸',
-'ì¯¹', 'ì¯º', 'ì¯»', 'ì¯¼', 'ì¯½', 'ì¯¾', 'ì¯¿', 'ì°', 'ì°', 'ì°', 'ì°',
-'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°',
-'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°',
-'ì° ', 'ì°£', 'ì°¤', 'ì°¥', 'ì°¦', 'ì°ª', 'ì°«', 'ì°­', 'ì°¯', 'ì°±', 'ì°²',
-'ì°³', 'ì°´', 'ì°µ', 'ì°¶', 'ì°·', 'ì°º', 'ì°¿', 'ì±', 'ì±', 'ì±', 'ì±',
-'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±',
-'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±¡', 'ì±¢', 'ì±£',
-'ì±¥', 'ì±§', 'ì±©', 'ì±ª', 'ì±«', 'ì±¬', 'ì±­', 'ì±®', 'ì±¯', 'ì±±', 'ì±²',
-'ì±³', 'ì±´', 'ì±¶', 'ì±·', 'ì±¸', 'ì±¹', 'ì±º', 'ì±»', 'ì±¼', 'ì±½', 'ì±¾',
-'ì±¿', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²',
-'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²',
-'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²¡', 'ì²¢', 'ì²£',
-'ì²¤', 'ì²¥', 'ì²¦', 'ì²§', 'ì²ª', 'ì²®', 'ì²¯', 'ì²°', 'ì²±', 'ì²²', 'ì²³',
-'ì²¶', 'ì²·', 'ì²¹', 'ì²º', 'ì²»', 'ì²½', 'ì²¾', 'ì²¿', 'ì³', 'ì³', 'ì³',
-'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³',
-'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³',
-'ì³', 'ì³ ', 'ì³¡', 'ì³¢', 'ì³£', 'ì³¥', 'ì³¦', 'ì³§', 'ì³¨', 'ì³©', 'ì³ª',
-'ì³«', 'ì³­', 'ì³®', 'ì³¯', 'ì³±', 'ì³²', 'ì³³', 'ì³´', 'ì³µ', 'ì³¶', 'ì³·',
-'ì³¸', 'ì³¹', 'ì³º', 'ì³»', 'ì³¼', 'ì³½', 'ì³¾', 'ì³¿', 'ì´', 'ì´', 'ì´',
-'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´',
-'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´ ', 'ì´¡',
-'ì´¢', 'ì´£', 'ì´¥', 'ì´¦', 'ì´§', 'ì´©', 'ì´ª', 'ì´«', 'ì´­', 'ì´®', 'ì´¯',
-'ì´°', 'ì´±', 'ì´²', 'ì´³', 'ì´´', 'ì´µ', 'ì´¶', 'ì´·', 'ì´¸', 'ì´º', 'ì´»',
-'ì´¼', 'ì´½', 'ì´¾', 'ì´¿', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ',
-'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ',
-'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ',
-'ìµ', 'ìµ', 'ìµ¡', 'ìµ¢', 'ìµ£', 'ìµ¥', 'ìµ¦', 'ìµ§', 'ìµ¨', 'ìµ©', 'ìµª',
-'ìµ«', 'ìµ®', 'ìµ°', 'ìµ²', 'ìµ³', 'ìµ´', 'ìµµ', 'ìµ¶', 'ìµ·', 'ìµ¹', 'ìµº',
-'ìµ»', 'ìµ¼', 'ìµ½', 'ìµ¾', 'ìµ¿', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶',
-'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶',
-'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶ ',
-'ì¶¡', 'ì¶¢', 'ì¶£', 'ì¶¦', 'ì¶¨', 'ì¶ª', 'ì¶«', 'ì¶¬', 'ì¶­', 'ì¶®', 'ì¶¯',
-'ì¶±', 'ì¶²', 'ì¶³', 'ì¶´', 'ì¶µ', 'ì¶¶', 'ì¶·', 'ì¶¸', 'ì¶¹', 'ì¶º', 'ì¶»',
-'ì¶¼', 'ì¶½', 'ì¶¾', 'ì¶¿', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·',
-'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·',
-'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·',
-'ì· ', 'ì·¡', 'ì·¢', 'ì·£', 'ì·¤', 'ì·¥', 'ì·¦', 'ì·§', 'ì·©', 'ì·ª', 'ì·«',
-'ì·­', 'ì·®', 'ì·¯', 'ì·±', 'ì·²', 'ì·³', 'ì·´', 'ì·µ', 'ì·¶', 'ì··', 'ì·º',
-'ì·¼', 'ì·¾', 'ì·¿', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸',
-'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸',
-'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸¢', 'ì¸£', 'ì¸¥',
-'ì¸¦', 'ì¸§', 'ì¸©', 'ì¸ª', 'ì¸«', 'ì¸¬', 'ì¸­', 'ì¸®', 'ì¸¯', 'ì¸²', 'ì¸´',
-'ì¸¶', 'ì¸·', 'ì¸¸', 'ì¸¹', 'ì¸º', 'ì¸»', 'ì¸¼', 'ì¸½', 'ì¸¾', 'ì¸¿', 'ì¹',
-'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹',
-'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹',
-'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹¢', 'ì¹£', 'ì¹¤', 'ì¹¥', 'ì¹¦', 'ì¹§',
-'ì¹ª', 'ì¹¬', 'ì¹®', 'ì¹¯', 'ì¹°', 'ì¹±', 'ì¹²', 'ì¹³', 'ì¹¶', 'ì¹·', 'ì¹¹',
-'ì¹º', 'ì¹»', 'ì¹½', 'ì¹¾', 'ì¹¿', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº',
-'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº',
-'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº¢', 'ìº¦', 'ìº§', 'ìº¨',
-'ìº©', 'ìºª', 'ìº«', 'ìº®', 'ìº¯', 'ìº°', 'ìº±', 'ìº²', 'ìº³', 'ìº´', 'ìºµ',
-'ìº¶', 'ìº·', 'ìº¸', 'ìº¹', 'ìºº', 'ìº»', 'ìº¼', 'ìº½', 'ìº¾', 'ìº¿', 'ì»',
-'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»',
-'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»',
-'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì» ', 'ì»¡', 'ì»¢',
-'ì»£', 'ì»¦', 'ì»§', 'ì»©', 'ì»ª', 'ì»­', 'ì»®', 'ì»¯', 'ì»°', 'ì»±', 'ì»²',
-'ì»³', 'ì»¶', 'ì»º', 'ì»»', 'ì»¼', 'ì»½', 'ì»¾', 'ì»¿', 'ì¼', 'ì¼', 'ì¼',
-'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼',
-'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼¡', 'ì¼¢',
-'ì¼£', 'ì¼¥', 'ì¼¦', 'ì¼§', 'ì¼¨', 'ì¼©', 'ì¼ª', 'ì¼«', 'ì¼®', 'ì¼²', 'ì¼³',
-'ì¼´', 'ì¼µ', 'ì¼¶', 'ì¼·', 'ì¼¹', 'ì¼º', 'ì¼»', 'ì¼¼', 'ì¼½', 'ì¼¾', 'ì¼¿',
-'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½',
-'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½',
-'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½ ', 'ì½¡', 'ì½¢', 'ì½£', 'ì½¦',
-'ì½¨', 'ì½ª', 'ì½«', 'ì½¬', 'ì½­', 'ì½®', 'ì½¯', 'ì½²', 'ì½³', 'ì½µ', 'ì½¶',
-'ì½·', 'ì½¹', 'ì½º', 'ì½»', 'ì½¼', 'ì½½', 'ì½¾', 'ì½¿', 'ì¾', 'ì¾', 'ì¾',
-'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾',
-'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾',
-'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾ ', 'ì¾¢', 'ì¾£', 'ì¾¤', 'ì¾¥', 'ì¾¦', 'ì¾§',
-'ì¾©', 'ì¾ª', 'ì¾«', 'ì¾¬', 'ì¾­', 'ì¾®', 'ì¾¯', 'ì¾±', 'ì¾²', 'ì¾³', 'ì¾´',
-'ì¾µ', 'ì¾¶', 'ì¾·', 'ì¾¸', 'ì¾¹', 'ì¾º', 'ì¾»', 'ì¾¼', 'ì¾½', 'ì¾¾', 'ì¾¿',
-'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿',
-'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿',
-'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿¢', 'ì¿£',
-'ì¿¥', 'ì¿¦', 'ì¿§', 'ì¿©', 'ì¿ª', 'ì¿«', 'ì¿¬', 'ì¿­', 'ì¿®', 'ì¿¯', 'ì¿²',
-'ì¿´', 'ì¿¶', 'ì¿·', 'ì¿¸', 'ì¿¹', 'ì¿º', 'ì¿»', 'ì¿½', 'ì¿¾', 'ì¿¿', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¥',
-'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬', 'í®', 'í¯', 'í°', 'í±',
-'í²', 'í³', 'í¶', 'í·', 'í¹', 'íº', 'í»', 'í½', 'í¾', 'í¿', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©',
-'íª', 'í«', 'í®', 'í¯', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¸',
-'í¹', 'íº', 'í»', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¦', 'í§', 'í©', 'íª',
-'í«', 'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í¶', 'í¸', 'íº',
-'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¥', 'í¦', 'í§', 'í¨', 'í©',
-'íª', 'í«', 'í®', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¹', 'íº',
-'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§',
-'í¨', 'í©', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯', 'í²', 'í³', 'íµ',
-'í¶', 'í·', 'í¹', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¢', 'í£', 'í¤', 'í¥',
-'í¦', 'í§', 'í©', 'íª', 'í«', 'í­', 'í®', 'í¯', 'í°', 'í±', 'í²',
-'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¸', 'í¹', 'íº', 'í»', 'í½', 'í¾',
-'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í¢', 'í£',
-'í¥', 'í¦', 'í§', 'í©', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯', 'í²',
-'í´', 'í¶', 'í·', 'í¸', 'í¹', 'í»', 'í½', 'í¾', 'í¿', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤',
-'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯',
-'í°', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¹', 'íº', 'í»', 'í¼',
-'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ',
-'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¸', 'í¹', 'íº',
-'í»', 'í¾', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬', 'í­',
-'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¸',
-'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¢',
-'í£', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í­', 'í®', 'í¯',
-'í°', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'íº', 'í»', 'í½', 'í¾',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¦', 'í§', 'í¨', 'í©', 'íª',
-'í«', 'í¬', 'í­', 'í®', 'í¯', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¹',
-'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í¢', 'í£', 'í¤', 'í¦', 'í§', 'íª', 'í«', 'í­',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'íº', 'í¾',
-'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬',
-'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'í¸', 'í¹', 'íº', 'í»', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¤', 'í¥',
-'í¦', 'í§', 'íª', 'í¬', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'íµ',
-'í¶', 'í·', 'í¹', 'íº', 'í»', 'í½', 'í¾', 'í¿', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í ', 'í¢', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¸', 'í¹', 'íº',
-'í»', 'í¾', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬',
-'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'í¸', 'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¥', 'í¦', 'í§', 'í¨',
-'í©', 'íª', 'í«', 'í¬', 'í®', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ',
-'í¶', 'í·', 'íº', 'í»', 'í½', 'í¾', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'íª', 'í«', 'í¬', 'í­',
-'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¸',
-'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í©', 'íª',
-'í«', 'í­', 'í®', 'í¯', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'í¹', 'íº', 'í¼', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬',
-'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'í¸', 'í¹', 'íº', 'í»', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¤',
-'í¦', 'í§', 'íª', 'í¬', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í¶',
-'í·', 'í¹', 'íº', 'í»', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«',
-'í¬', 'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶',
-'í·', 'í¸', 'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ',
-'í¡', 'í¢', 'í£', 'í¦', 'í§', 'í©', 'íª', 'í«', 'í­', 'í®', 'í¯',
-'í°', 'í±', 'í²', 'í³', 'í¶', 'í¸', 'íº', 'í»', 'í¼', 'í½', 'í¾',
-'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í¡', 'í¢', 'í£', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«',
-'í¬', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'íº', 'í»', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦',
-'í¨', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯', 'í²', 'í³', 'íµ', 'í¶',
-'í·', 'í¸', 'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í ', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í©', 'íª', 'í«', 'í­',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¸', 'íº',
-'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¥', 'í¦',
-'í§', 'í©', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯', 'í±', 'í²', 'í³',
-'í´', 'í¶', 'í·', 'í¸', 'í¹', 'íº', 'í»', 'í¾', 'í¿', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'íª', 'í¬',
-'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í¶', 'í·', 'í¹', 'íº', 'í»',
-'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í¢', 'í¤', 'í¦', 'í§', 'í¨', 'íª', 'í«', 'í­',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¸', 'í¹', 'íº',
-'í»', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', '\ud7a4'] ``` 28.
-get_all_incompleted_form_hangul_chars This returns all non-completed form
-Hangul characters. Returns: - `List[str]`: all non-completed form Hangul
-characters Examples: ```python >>> from kss import Kss >>>
-get_all_incompleted_form_hangul_chars = Kss
+get_all_completed_form_hangul_chars = Kss
+("get_all_completed_form_hangul_chars") >>> output =
+get_all_completed_form_hangul_chars() >>> print(output) ['ê°', 'ê°', 'ê°',
+'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°',
+'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê° ', 'ê°¤', 'ê°¬', 'ê°­', 'ê°¯',
+'ê°°', 'ê°±', 'ê°¸', 'ê°¹', 'ê°¼', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
+'ê±°', 'ê±±', 'ê±´', 'ê±·', 'ê±¸', 'ê±º', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²',
+'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê² ',
+'ê²¡', 'ê²¨', 'ê²©', 'ê²ª', 'ê²¬', 'ê²¯', 'ê²°', 'ê²¸', 'ê²¹', 'ê²»', 'ê²¼',
+'ê²½', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³ ', 'ê³¡', 'ê³¤', 'ê³§',
+'ê³¨', 'ê³ª', 'ê³¬', 'ê³¯', 'ê³°', 'ê³±', 'ê³³', 'ê³µ', 'ê³¶', 'ê³¼', 'ê³½',
+'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´ ', 'ê´©',
+'ê´¬', 'ê´­', 'ê´´', 'ê´µ', 'ê´¸', 'ê´¼', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ',
+'êµ', 'êµ', 'êµ¡', 'êµ£', 'êµ¬', 'êµ­', 'êµ°', 'êµ³', 'êµ´', 'êµµ', 'êµ¶',
+'êµ»', 'êµ¼', 'êµ½', 'êµ¿', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶',
+'ê¶', 'ê¶¤', 'ê¶·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·',
+'ê· ', 'ê·¤', 'ê·¸', 'ê·¹', 'ê·¼', 'ê·¿', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸',
+'ê¸', 'ê¸', 'ê¸°', 'ê¸±', 'ê¸´', 'ê¸·', 'ê¸¸', 'ê¸º', 'ê¹', 'ê¹', 'ê¹',
+'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹',
+'ê¹', 'ê¹ ', 'ê¹¡', 'ê¹¥', 'ê¹¨', 'ê¹©', 'ê¹¬', 'ê¹°', 'ê¹¸', 'ê¹¹', 'ê¹»',
+'ê¹¼', 'ê¹½', 'êº', 'êº', 'êº', 'êº¼', 'êº½', 'êº¾', 'ê»', 'ê»', 'ê»',
+'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»¨', 'ê»«', 'ê»­', 'ê»´',
+'ê»¸', 'ê»¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼¬', 'ê¼­', 'ê¼°', 'ê¼²', 'ê¼´',
+'ê¼¼', 'ê¼½', 'ê¼¿', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½',
+'ê½¤', 'ê½¥', 'ê½¹', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾¸',
+'ê¾¹', 'ê¾¼', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿',
+'ê¿¨', 'ê¿©', 'ê¿°', 'ê¿±', 'ê¿´', 'ê¿¸', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë¨', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë¼', 'ë½', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë¨',
+'ë©', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë±', 'ë³', 'ë´', 'ëµ', 'ë¸',
+'ë¼', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ',
+'ë¥', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë£', 'ë¤', 'ë¥', 'ë¨', 'ë¬', 'ë´', 'ëµ', 'ë·', 'ë¸',
+'ë¹', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë ', 'ë¸', 'ë¹', 'ë¼', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë¨', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë¨', 'ë©', 'ë¬', 'ë°', 'ë¹', 'ë»', 'ë½', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë´', 'ë¼', 'ë', 'ë', 'ë ',
+'ë¨', 'ë©', 'ë´', 'ëµ', 'ë¼', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë£', 'ë¥', 'ë¦', 'ëª', 'ë¬', 'ë°',
+'ë´', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë¢',
+'ë¤', 'ë¥', 'ë¦', 'ë¨', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë³', 'ë´',
+'ëµ', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¿', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë¤', 'ë¥', 'ë§', 'ë©', 'ë«', 'ë®', 'ë°', 'ë±',
+'ë´', 'ë¸', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ',
+'ë¡', 'ë¨', 'ë¬', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¤', 'ë¨', 'ë¼', 'ë', 'ë',
+'ë', 'ë ', 'ë¨', 'ë©', 'ë«', 'ë´', 'ë', 'ë', 'ë', 'ë', 'ë ',
+'ë¡', 'ë£', 'ë¥', 'ë¬', 'ë', 'ë', 'ë', 'ë¤', 'ë¨', 'ë¬', 'ëµ',
+'ë·', 'ë¹', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë£',
+'ë¤', 'ë¦', 'ë¬', 'ë­', 'ë¯', 'ë±', 'ë¸', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë¤', 'ë¥', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë°', 'ë±', 'ë´', 'ë¸',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë ', 'ë¡', 'ë ', 'ë¡', 'ë¤', 'ë¨', 'ëª', 'ë«', 'ë°',
+'ë±', 'ë³', 'ë´', 'ëµ', 'ë»', 'ë¼', 'ë½', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë¬', 'ë', 'ë', 'ë', 'ë', 'ë¥', 'ë¬',
+'ë´', 'ë', 'ë¤', 'ë¨', 'ë', 'ë', 'ë ', 'ë¤', 'ë«', 'ë¬', 'ë±',
+'ë', 'ë°', 'ë´', 'ë¸', 'ë', 'ë', 'ë', 'ë¨', 'ë©', 'ë¬', 'ë¯',
+'ë°', 'ë¸', 'ë¹', 'ë»', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¤',
+'ë¨', 'ë°', 'ë±', 'ë³', 'ëµ', 'ë¼', 'ë½', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¨',
+'ë©', 'ë«', 'ë¬', 'ë­', 'ë´', 'ëµ', 'ë¸', 'ë', 'ë', 'ë¬', 'ë­',
+'ë°', 'ë´', 'ë¼', 'ë½', 'ë¿', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ',
+'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ¤', 'ë ¥', 'ë ¨', 'ë ¬', 'ë ´', 'ë µ',
+'ë ·', 'ë ¸', 'ë ¹', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡ ', 'ë¡¤',
+'ë¡¬', 'ë¡­', 'ë¡¯', 'ë¡±', 'ë¡¸', 'ë¡¼', 'ë¢', 'ë¢¨', 'ë¢°', 'ë¢´', 'ë¢¸',
+'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£¡', 'ë£¨',
+'ë£©', 'ë£¬', 'ë£°', 'ë£¸', 'ë£¹', 'ë£»', 'ë£½', 'ë¤', 'ë¤', 'ë¤ ', 'ë¤¼',
+'ë¤½', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥ ', 'ë¥¨',
+'ë¥©', 'ë¥«', 'ë¥­', 'ë¥´', 'ë¥µ', 'ë¥¸', 'ë¥¼', 'ë¦', 'ë¦', 'ë¦', 'ë¦',
+'ë¦', 'ë¦', 'ë¦', 'ë¦¬', 'ë¦­', 'ë¦°', 'ë¦´', 'ë¦¼', 'ë¦½', 'ë¦¿', 'ë§',
+'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§',
+'ë§', 'ë§', 'ë§¡', 'ë§£', 'ë§¤', 'ë§¥', 'ë§¨', 'ë§¬', 'ë§´', 'ë§µ', 'ë§·',
+'ë§¸', 'ë§¹', 'ë§º', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨¸', 'ë¨¹', 'ë¨¼', 'ë©',
+'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©',
+'ë©¤', 'ë©¥', 'ë©§', 'ë©¨', 'ë©©', 'ë©°', 'ë©±', 'ë©´', 'ë©¸', 'ëª', 'ëª',
+'ëª', 'ëª', 'ëª', 'ëª¨', 'ëª©', 'ëª«', 'ëª¬', 'ëª°', 'ëª²', 'ëª¸', 'ëª¹',
+'ëª»', 'ëª½', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«¼', 'ë¬', 'ë¬', 'ë¬', 'ë¬',
+'ë¬', 'ë¬', 'ë¬', 'ë¬ ', 'ë¬©', 'ë¬«', 'ë¬´', 'ë¬µ', 'ë¬¶', 'ë¬¸', 'ë¬»',
+'ë¬¼', 'ë¬½', 'ë¬¾', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­',
+'ë­', 'ë­¡', 'ë­£', 'ë­¬', 'ë®', 'ë®', 'ë®', 'ë®¤', 'ë®¨', 'ë®¬', 'ë®´',
+'ë®·', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯¸', 'ë¯¹', 'ë¯¼', 'ë¯¿', 'ë°',
+'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°',
+'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°¤', 'ë°¥', 'ë°§', 'ë°©',
+'ë°­', 'ë°°', 'ë°±', 'ë°´', 'ë°¸', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±',
+'ë±', 'ë±', 'ë±', 'ë±', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²',
+'ë²', 'ë²', 'ë²', 'ë²', 'ë² ', 'ë²¡', 'ë²¤', 'ë²§', 'ë²¨', 'ë²°', 'ë²±',
+'ë²³', 'ë²´', 'ë²µ', 'ë²¼', 'ë²½', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³',
+'ë³', 'ë³', 'ë³', 'ë³´', 'ë³µ', 'ë³¶', 'ë³¸', 'ë³¼', 'ë´', 'ë´', 'ë´',
+'ë´', 'ë´', 'ë´', 'ë´¤', 'ë´¬', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ',
+'ëµ', 'ëµ¤', 'ëµ¨', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶',
+'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶¤', 'ë¶°', 'ë¶¸', 'ë·', 'ë·',
+'ë·', 'ë·', 'ë·©', 'ë·°', 'ë·´', 'ë·¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸',
+'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹',
+'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹ ', 'ë¹¡', 'ë¹¤', 'ë¹¨', 'ë¹ª', 'ë¹°',
+'ë¹±', 'ë¹³', 'ë¹´', 'ë¹µ', 'ë¹»', 'ë¹¼', 'ë¹½', 'ëº', 'ëº', 'ëº', 'ëº',
+'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº¨', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»',
+'ë» ', 'ë»£', 'ë»¤', 'ë»¥', 'ë»¬', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼',
+'ë¼', 'ë¼', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë¾', 'ë¾°',
+'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿¡', 'ì¼', 'ì', 'ì',
+'ì', 'ì ', 'ì¨', 'ì©', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì£',
+'ì¥', 'ì¬', 'ì­', 'ì¯', 'ì°', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì¼', 'ì½',
+'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì¤', 'ì¥', 'ì¨', 'ì¬', 'ì´', 'ìµ', 'ì·', 'ì¹', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì£', 'ì¤',
+'ì¦', 'ì§', 'ì¬', 'ì­', 'ì¯', 'ì°', 'ì±', 'ì¶', 'ì¸', 'ì¹', 'ì¼',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¤',
+'ì¥', 'ì§', 'ì¨', 'ì©', 'ì°', 'ì´', 'ì¸', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¥', 'ì¨', 'ì©', 'ì¬',
+'ì°', 'ì½', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¤', 'ì¨',
+'ì°', 'ì±', 'ì³', 'ì¼', 'ì½', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¨', 'ì©', 'ì«', 'ì­', 'ì¯', 'ì±',
+'ì²', 'ì´', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¥', 'ì¬', 'ì­',
+'ì°', 'ì´', 'ì¼', 'ì½', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì¤', 'ì¥', 'ì¨', 'ì¬', 'ì­', 'ì´', 'ìµ', 'ì·', 'ì¹', 'ì',
+'ì', 'ì ', 'ì£', 'ì¤', 'ì«', 'ì¬', 'ì­', 'ì¯', 'ì±', 'ì¶', 'ì¸',
+'ì¹', 'ì»', 'ì¼', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì¤', 'ì¥', 'ì¨', 'ì©', 'ì', 'ì¨', 'ì©', 'ì¬', 'ì°',
+'ì²', 'ì¸', 'ì¹', 'ì¼', 'ì½', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì ', 'ì¢', 'ì¨', 'ì©', 'ì­', 'ì´', 'ìµ', 'ì¸', 'ì',
+'ì', 'ì¤', 'ì¬', 'ì°', 'ì´', 'ì¼', 'ì½', 'ì', 'ì¤', 'ì¥', 'ì¨',
+'ì¬', 'ì´', 'ìµ', 'ì¹', 'ì', 'ì', 'ì', 'ì¸', 'ì¼', 'ì©', 'ì°',
+'ì±', 'ì´', 'ì¸', 'ìº', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì¨', 'ì©', 'ì¬', 'ì°', 'ì¸', 'ì¹', 'ì»', 'ì½', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì ', 'ì¡', 'ì¤', 'ì¨', 'ì°', 'ì±', 'ì³', 'ì´', 'ìµ',
+'ì¼', 'ì½', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì ', 'ì©', 'ì´', 'ìµ', 'ì¸', 'ì¹', 'ì»', 'ì¼', 'ì½',
+'ì¾', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì£', 'ì¥', 'ì¬', 'ì­', 'ì®', 'ì°',
+'ì´', 'ì¶', 'ì·', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¤', 'ì¥', 'ì¨',
+'ì¬', 'ì­', 'ì®', 'ì°', 'ì³', 'ì´', 'ìµ', 'ì·', 'ì¹', 'ì»', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ',
+'ì¬', 'ì¯', 'ì±', 'ì¸', 'ì¹', 'ì¼', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì¤', 'ì¥', 'ì§', 'ì©', 'ì°', 'ì±', 'ì´',
+'ì¸', 'ì¹', 'ìº', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì ', 'ì¡', 'ì¨', 'ì©', 'ì¬', 'ì°', 'ì¸', 'ì¹', 'ì½',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¤',
+'ì¨', 'ì°', 'ì±', 'ì³', 'ìµ', 'ì·', 'ì¼', 'ì½', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì ', 'ì¨', 'ì«', 'ì´', 'ìµ', 'ì¸', 'ì¼', 'ì½', 'ì¾', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì¬', 'ì­',
+'ì°', 'ì´', 'ì¼', 'ì½', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì¤', 'ì¨', 'ì¬', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ',
+'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì  ', 'ì ¤', 'ì ¬', 'ì ­',
+'ì ¯', 'ì ±', 'ì ¸', 'ì ¼', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡°',
+'ì¡±', 'ì¡´', 'ì¡¸', 'ì¡º', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢',
+'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢¡', 'ì¢¨', 'ì¢¼', 'ì¢½', 'ì£', 'ì£',
+'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£ ', 'ì£¡', 'ì£¤', 'ì£µ', 'ì£¼', 'ì£½',
+'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤¬', 'ì¤´',
+'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥ ', 'ì¥¡', 'ì¥£', 'ì¥¬', 'ì¥°', 'ì¥´', 'ì¥¼',
+'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì§', 'ì§', 'ì§',
+'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§',
+'ì§', 'ì§ ', 'ì§¢', 'ì§¤', 'ì§§', 'ì§¬', 'ì§­', 'ì§¯', 'ì§°', 'ì§±', 'ì§¸',
+'ì§¹', 'ì§¼', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨©',
+'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì© ', 'ì©¡', 'ì©¨', 'ì©½',
+'ìª', 'ìª', 'ìª¼', 'ìª½', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«',
+'ì«', 'ì«', 'ì« ', 'ì«¬', 'ì«´', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬ ', 'ì¬¡',
+'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­¤', 'ì­¸', 'ì­¹',
+'ì®', 'ì®¸', 'ì¯', 'ì¯¤', 'ì¯§', 'ì¯©', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°',
+'ì°', 'ì°¡', 'ì°¢', 'ì°§', 'ì°¨', 'ì°©', 'ì°¬', 'ì°®', 'ì°°', 'ì°¸', 'ì°¹',
+'ì°»', 'ì°¼', 'ì°½', 'ì°¾', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±',
+'ì±', 'ì±', 'ì± ', 'ì±¤', 'ì±¦', 'ì±¨', 'ì±°', 'ì±µ', 'ì²', 'ì²', 'ì²',
+'ì² ', 'ì²¨', 'ì²©', 'ì²«', 'ì²¬', 'ì²­', 'ì²´', 'ì²µ', 'ì²¸', 'ì²¼', 'ì³',
+'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³¤', 'ì³¬', 'ì³°', 'ì´', 'ì´', 'ì´',
+'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´¤', 'ì´¨', 'ì´¬', 'ì´¹', 'ìµ',
+'ìµ ', 'ìµ¤', 'ìµ¬', 'ìµ­', 'ìµ¯', 'ìµ±', 'ìµ¸', 'ì¶', 'ì¶', 'ì¶', 'ì¶',
+'ì¶', 'ì¶¤', 'ì¶¥', 'ì¶§', 'ì¶©', 'ì¶°', 'ì·', 'ì·', 'ì·', 'ì·¨', 'ì·¬',
+'ì·°', 'ì·¸', 'ì·¹', 'ì·»', 'ì·½', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸ ',
+'ì¸¡', 'ì¸¤', 'ì¸¨', 'ì¸°', 'ì¸±', 'ì¸³', 'ì¸µ', 'ì¹', 'ì¹', 'ì¹', 'ì¹',
+'ì¹ ', 'ì¹¡', 'ì¹¨', 'ì¹©', 'ì¹«', 'ì¹­', 'ì¹´', 'ì¹µ', 'ì¹¸', 'ì¹¼', 'ìº',
+'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº ', 'ìº¡', 'ìº£', 'ìº¤',
+'ìº¥', 'ìº¬', 'ìº­', 'ì»', 'ì»¤', 'ì»¥', 'ì»¨', 'ì»«', 'ì»¬', 'ì»´', 'ì»µ',
+'ì»·', 'ì»¸', 'ì»¹', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼',
+'ì¼', 'ì¼ ', 'ì¼¤', 'ì¼¬', 'ì¼­', 'ì¼¯', 'ì¼°', 'ì¼±', 'ì¼¸', 'ì½', 'ì½',
+'ì½', 'ì½', 'ì½¤', 'ì½¥', 'ì½§', 'ì½©', 'ì½°', 'ì½±', 'ì½´', 'ì½¸', 'ì¾',
+'ì¾', 'ì¾', 'ì¾¡', 'ì¾¨', 'ì¾°', 'ì¿', 'ì¿ ', 'ì¿¡', 'ì¿¤', 'ì¿¨', 'ì¿°',
+'ì¿±', 'ì¿³', 'ì¿µ', 'ì¿¼', 'í', 'í', 'í', 'í', 'í­', 'í´', 'íµ',
+'í¸', 'í¼', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¬',
+'í­', 'í°', 'í´', 'í¼', 'í½', 'í', 'í¤', 'í¥', 'í¨', 'í¬', 'í´',
+'íµ', 'í·', 'í¹', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í ', 'í¤', 'í¬', 'í­', 'í¯', 'í°', 'í±',
+'í¸', 'í', 'í°', 'í±', 'í´', 'í¸', 'íº', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¨', 'í¬',
+'í¼', 'í', 'í', 'í ', 'í¡', 'í¤', 'í¨', 'í°', 'í±', 'í³', 'íµ',
+'íº', 'í¼', 'í', 'í', 'í´', 'í¸', 'í', 'í', 'í', 'í¬', 'í­',
+'í°', 'í´', 'í¼', 'í½', 'í¿', 'í', 'í', 'í', 'í¤', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¤', 'í¬', 'í±', 'í¸',
+'í¹', 'í¼', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í¤', 'í¥', 'í°', 'í±', 'í´', 'í¸', 'í', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¥',
+'í¨', 'í©', 'í¬', 'í°', 'í¸', 'í¹', 'í»', 'í¼', 'í½', 'í', 'í',
+'í¼', 'í½', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í ', 'í¨', 'í©', 'í«', 'í­', 'í´', 'í¸', 'í¼', 'í', 'í',
+'í', 'í', 'í', 'í', 'í¡', 'í£', 'í¬', 'í­', 'í°', 'í´', 'í¼',
+'í½', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¤', 'í­',
+'í¯', 'í¸', 'í¹', 'í¼', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í©', 'í', 'í', 'í', 'í', 'í', 'í¨', 'í¬', 'í°', 'í¸',
+'í»', 'í½', 'í', 'í', 'í', 'í', 'í', 'í', 'í¼', 'í½', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¥', 'í¨',
+'í©', 'í«', 'í­', 'í´', 'íµ', 'í¸', 'í¼', 'í', 'í', 'í', 'í',
+'í', 'í', 'í¥', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í¤', 'í¥', 'í¨', 'í¬', 'í´', 'íµ', 'í·', 'í¹', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¤', 'í­',
+'í¸', 'í¹', 'í¼', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í§', 'í©', 'í°', 'í±', 'í´', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í¡', 'í¨', 'í¬', 'í°', 'í¹', 'í»',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¤', 'í¨',
+'í°', 'íµ', 'í¼', 'í½', 'í', 'í', 'í', 'í', 'í', 'í', 'í ',
+'í¨', 'í©', 'í«', 'í­', 'í´', 'íµ', 'í¸', 'í¼', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡', 'í£', 'í¥',
+'í©', 'í¬', 'í°', 'í´', 'í¼', 'í½', 'í', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í'] ``` 28. get_all_incompleted_form_hangul_chars This
+returns all incompleted form Hangul characters. Returns: - `List[str]`: all
+incompleted form Hangul characters Examples: ```python >>> from kss import Kss
+>>> get_all_incompleted_form_hangul_chars = Kss
 ("get_all_incompleted_form_hangul_chars") >>> output =
 get_all_incompleted_form_hangul_chars() >>> print(output) ['ê°', 'ê°', 'ê°',
 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°¡', 'ê°¢',
 'ê°£', 'ê°¥', 'ê°¦', 'ê°§', 'ê°¨', 'ê°©', 'ê°ª', 'ê°«', 'ê°®', 'ê°²', 'ê°³',
 'ê°´', 'ê°µ', 'ê°¶', 'ê°·', 'ê°º', 'ê°»', 'ê°½', 'ê°¾', 'ê°¿', 'ê±', 'ê±',
 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
@@ -2443,20 +1844,20 @@
 reduce_char_repeats_over (`int`): the maximum number of character that can be
 repeated - reduce_emoticon_repeats_over (`int`): the maximum number of emoticon
 that can be repeated - num_workers (`Union[int, str]`): the number of
 multiprocessing workers Returns: - `Union[str, List[str]]`: normalized text or
 list of normalized texts Examples: ```python >>> from kss import Kss >>>
 normalize = Kss("normalize") >>> text = "ìë\u200bíì¸ì
 ï¾»ï¾»ï¾»ï¾»ï¾»ï¾»
-ì¤ë\u200bì ë ì´ ì°¸ ì¢ë¤ì.\\n\\n\\n200 < 300 & 400" >>> normalize
-(text, allow_doubled_spaces=False, allow_html_tags=False,
-allow_html_escape=False, allow_halfwidth_hangul=False, allow_hangul_jamo=False,
+ì¤ë\u200bì ë ì´ ì°¸ ì¢ë¤ì.\n\n\n200 < 300 & 400" >>> normalize(text,
+allow_doubled_spaces=False, allow_html_tags=False, allow_html_escape=False,
+allow_halfwidth_hangul=False, allow_hangul_jamo=False,
 allow_invisible_chars=False, reduce_char_repeats_over=2,
 reduce_emoticon_repeats_over=2) 'ìëíì¸ì ãã ì¤ëì ë ì´ ì°¸
-ì¢ë¤ì.\\n200 < 300 & 400' ``` 32. preprocess This preprocesses text with
+ì¢ë¤ì.\n200 < 300 & 400' ``` 32. preprocess This preprocesses text with
 various options. This does 1) normalization, 2) filtering out, and 3)
 anonymization in order. Args: - text (`Union[str, List[str], Tuple[str]]`):
 single text or list of texts - normalization_type (`Optional[str]`):
 normalization type - allow_doubled_spaces (`bool`): whether to allow doubled
 spaces or not - allow_html_tags (`bool`): whether to allow HTML tags or not -
 allow_html_escape (`bool`): whether to allow HTML escape or not -
 allow_halfwidth_hangul (`bool`): whether to allow halfwidth Hangul or not -
@@ -2564,17 +1965,17 @@
 convert_numbers_to_hangul_phonemes (`bool`): whether to convert numbers to
 Hangul phonemes or not - num_workers (`Union[int, str]`): the number of
 multiprocessing workers Returns: - `Union[str, List[str]]`: romanized text or
 list of romanized texts Examples: ```python >>> from kss import Kss >>>
 romanize = Kss("romanize") >>> text = "ìëíì¸ì" >>> romanize(text)
 'annyeonghaseyo' >>> text = "ëê´ë ¹" >>> romanize(text) 'daegwallyeong' ```
 References: - This was copied from [korean-romanizer](https://github.com/osori/
-korean-romanizer) and modified by Kss 38. is_unsafe Check if the text is unsafe
-or not. Args: - text (`Union[str, List[str], Tuple[str]]`): single text or list
-of texts - return_matches (`bool`): whether to return matches or not -
+korean-romanizer) and modified by Kss 38. is_unsafe This checks if the text is
+unsafe or not. Args: - text (`Union[str, List[str], Tuple[str]]`): single text
+or list of texts - return_matches (`bool`): whether to return matches or not -
 num_workers (`Union[int, str]`): the number of multiprocessing workers Returns:
 - `Union[bool, List[bool], List[bool], List[List[str]]]`: whether the text is
 unsafe or not or list of whether the texts are unsafe or not or list of matched
 bad words in the texts Examples: ```python >>> from kss import Kss >>>
 is_unsafe = Kss("is_unsafe") >>> text = "ìëíì¸ì" >>> is_unsafe(text)
 False >>> text = "ìëíì¸ì. ì¨ë°" >>> is_unsafe(text) True >>> text =
 ["ìëíì¸ì", "ìëíì¸ì. ì¨ë°"] >>> is_unsafe(text) [False,
```

### Comparing `kss-6.0.0/README.md` & `kss-6.0.0.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,34 @@
+Metadata-Version: 2.1
+Name: kss
+Version: 6.0.0.dev0
+Summary: A Toolkit for Korean sentence segmentation
+Home-page: https://github.com/hyunwoongko/kss
+Author: Hyunwoong Ko
+Author-email: kevin.brain@kakaobrain.com
+License: BSD 3-Clause "New" or "Revised" License
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.2
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 align="center">
 KSS: Korean String processing Suite
 </h1>
 
 <p align="center">
-    <a href="https://github.com/hyunwoongko/kss/releases">
-        <img alt="GitHub release" src="https://img.shields.io/github/release/hyunwoongko/kss.svg">
-    </a> 
-    <a href="https://github.com/hyunwoongko/kss/issues">
-        <img alt="Issues" src="https://img.shields.io/github/issues/hyunwoongko/kss">
-    </a>
-    <a href="https://github.com/hyunwoongko/kss/actions">
-        <img alt="Tests on Ubuntu" src="https://github.com/hyunwoongko/kss/actions/workflows/test_ubuntu.yaml/badge.svg">
-    </a>
-    <a href="https://github.com/hyunwoongko/kss/actions">
-        <img alt="Tests on MacOS" src="https://github.com/hyunwoongko/kss/actions/workflows/test_macos.yaml/badge.svg">
-    </a>
-    <a href="https://github.com/hyunwoongko/kss/actions">
-        <img alt="Tests on Windows" src="https://github.com/hyunwoongko/kss/actions/workflows/test_windows.yaml/badge.svg">
-    </a>
+    <a href="https://github.com/hyunwoongko/kss/releases"><img alt="GitHub release" src="https://img.shields.io/github/release/hyunwoongko/kss.svg"></a> <a href="https://github.com/hyunwoongko/kss/issues"><img alt="Issues" src="https://img.shields.io/github/issues/hyunwoongko/kss"></a> <a href="https://github.com/hyunwoongko/kss/actions"><img alt="Tests on Ubuntu" src="https://github.com/hyunwoongko/kss/actions/workflows/test_ubuntu.yaml/badge.svg"></a> <a href="https://github.com/hyunwoongko/kss/actions"><img alt="Tests on MacOS" src="https://github.com/hyunwoongko/kss/actions/workflows/test_macos.yaml/badge.svg"></a> <a href="https://github.com/hyunwoongko/kss/actions"><img alt="Tests on Windows" src="https://github.com/hyunwoongko/kss/actions/workflows/test_windows.yaml/badge.svg"></a>
 </p>
 
 
 KSS is a Korean string processing suite that provides various functions for processing Korean strings. It is designed to be simple and easy to use, and it is designed to be used in various fields such as natural language processing, data preprocessing, and data analysis.
 
 ### What's New:
 - April 27, 2024 [Released Kss 6.0 Python](https://github.com/hyunwoongko/kss/releases/tag/6.0.0).
@@ -98,15 +105,15 @@
     >>> text = "회사 동료 분들과 다녀왔는데 분위기도 좋고 음식도 맛있었어요 다만, 강남 토끼정이 강남 쉑쉑버거 골목길로 쭉 올라가야 하는데 다들 쉑쉑버거의 유혹에 넘어갈 뻔 했답니다 강남역 맛집 토끼정의 외부 모습."
     >>> split_sentences(text)
     ['회사 동료 분들과 다녀왔는데 분위기도 좋고 음식도 맛있었어요', '다만, 강남 토끼정이 강남 쉑쉑버거 골목길로 쭉 올라가야 하는데 다들 쉑쉑버거의 유혹에 넘어갈 뻔 했답니다', '강남역 맛집 토끼정의 외부 모습.']
 ```
 ### 4. Multiprocessing
 If you input a list of strings, Kss will automatically use multiprocessing to process the strings in parallel.
 And you can set the number of processes to use by setting the `num_workers` parameter.
-If you input `num_workers<2`, Kss will not use multiprocessing.
+If you input `num_workers < 2`, Kss will not use multiprocessing.
 
 ```python
 from kss import Kss
 
 module = Kss("MODULE_NAME")
 
 # using all cores
@@ -781,15 +788,16 @@
 
 References:
 - This was copied from [KoParadigm](https://github.com/Kyubyong/KoParadigm) and modified by Kss
 </details>
 
 <details>
 <summary>24. anonymize</summary>
-Anonymize sensitive information in the given text.
+
+This anonymizes sensitive information in the given text.
 
 Args:
 - text (`Union[str, List[str], Tuple[str]`): single text or list of texts
 - phone_number_anonymization (`bool`): whether to anonymize phone numbers or not
 - rrn_anonymization (`bool`): whether to anonymize resident registration numbers or not
 - card_anonymization (`bool`): whether to anonymize card numbers or not
 - email_anonymization (`bool`): whether to anonymize email addresses or not
@@ -825,15 +833,16 @@
 >>> print(output)
 "제 전화번호는 <PHONE_NUMBER>, 이메일 주소는 <EMAIL>입니다."
 ```
 </details>
 
 <details>
 <summary>25. clean_news</summary>
-Clean news articles by removing useless headers and footers.
+
+This cleans news articles by removing useless headers and footers.
 
 Args:
 - text (`Union[str, List[str], Tuple[str]]`): Input text or list of texts.
 - min_sentences (`int`): Minimum number of sentences to keep. Defaults to 3.
 - header_ratio (`float`): Ratio of the number of sentences to check in the header. Defaults to 0.4.
 - footer_ratio (`float`): Ratio of the number of sentences to check in the footer. Defaults to 0.4.
 - num_workers (`Union[int, str]`): the number of multiprocessing workers
@@ -879,36 +888,36 @@
 False
 ```
 </details>
 
 <details>
 <summary>27. get_all_completed_form_hangul_chars</summary>
 
-This returns all non-completed form Hangul characters.
+This returns all completed form Hangul characters.
 
 Returns:
-- `List[str]`: all non-completed form Hangul characters
+- `List[str]`: all completed form Hangul characters
 
 Examples:
 ```python
 >>> from kss import Kss
->>> get_all_incompleted_form_hangul_chars = Kss("get_all_incompleted_form_hangul_chars")
->>> output = get_all_incompleted_form_hangul_chars()
+>>> get_all_completed_form_hangul_chars = Kss("get_all_completed_form_hangul_chars")
+>>> output = get_all_completed_form_hangul_chars()
 >>> print(output)
-['갂', '갃', '갅', '갆', '갋', '갌', '갍', '갎', '갏', '갘', '갞', '갟', '갡', '갢', '갣', '갥', '갦', '갧', '갨', '갩', '갪', '갫', '갮', '갲', '갳', '갴', '갵', '갶', '갷', '갺', '갻', '갽', '갾', '갿', '걁', '걂', '걃', '걄', '걅', '걆', '걇', '걈', '걉', '걊', '걌', '걎', '걏', '걐', '걑', '걒', '걓', '걕', '걖', '걗', '걙', '걚', '걛', '걝', '걞', '걟', '걠', '걡', '걢', '걣', '걤', '걥', '걦', '걧', '걨', '걩', '걪', '걫', '걬', '걭', '걮', '걯', '걲', '걳', '걵', '걶', '걹', '걻', '걼', '걽', '걾', '걿', '겂', '겇', '겈', '겍', '겎', '겏', '겑', '겒', '겓', '겕', '겖', '겗', '겘', '겙', '겚', '겛', '겞', '겢', '겣', '겤', '겥', '겦', '겧', '겫', '겭', '겮', '겱', '겲', '겳', '겴', '겵', '겶', '겷', '겺', '겾', '겿', '곀', '곂', '곃', '곅', '곆', '곇', '곉', '곊', '곋', '곍', '곎', '곏', '곐', '곑', '곒', '곓', '곔', '곖', '곘', '곙', '곚', '곛', '곜', '곝', '곞', '곟', '곢', '곣', '곥', '곦', '곩', '곫', '곭', '곮', '곲', '곴', '곷', '곸', '곹', '곺', '곻', '곾', '곿', '괁', '괂', '괃', '괅', '괇', '괈', '괉', '괊', '괋', '괎', '괐', '괒', '괓', '괔', '괕', '괖', '괗', '괙', '괚', '괛', '괝', '괞', '괟', '괡', '괢', '괣', '괤', '괥', '괦', '괧', '괨', '괪', '괫', '괮', '괯', '괰', '괱', '괲', '괳', '괶', '괷', '괹', '괺', '괻', '괽', '괾', '괿', '굀', '굁', '굂', '굃', '굆', '굈', '굊', '굋', '굌', '굍', '굎', '굏', '굑', '굒', '굓', '굕', '굖', '굗', '굙', '굚', '굛', '굜', '굝', '굞', '굟', '굠', '굢', '굤', '굥', '굦', '굧', '굨', '굩', '굪', '굫', '굮', '굯', '굱', '굲', '굷', '굸', '굹', '굺', '굾', '궀', '궃', '궄', '궅', '궆', '궇', '궊', '궋', '궍', '궎', '궏', '궑', '궒', '궓', '궔', '궕', '궖', '궗', '궘', '궙', '궚', '궛', '궞', '궟', '궠', '궡', '궢', '궣', '궥', '궦', '궧', '궨', '궩', '궪', '궫', '궬', '궭', '궮', '궯', '궰', '궱', '궲', '궳', '궴', '궵', '궶', '궸', '궹', '궺', '궻', '궼', '궽', '궾', '궿', '귂', '귃', '귅', '귆', '귇', '귉', '귊', '귋', '귌', '귍', '귎', '귏', '귒', '귔', '귕', '귖', '귗', '귘', '귙', '귚', '귛', '귝', '귞', '귟', '귡', '귢', '귣', '귥', '귦', '귧', '귨', '귩', '귪', '귫', '귬', '귭', '귮', '귯', '귰', '귱', '귲', '귳', '귴', '귵', '귶', '귷', '귺', '귻', '귽', '귾', '긂', '긃', '긄', '긅', '긆', '긇', '긊', '긌', '긎', '긏', '긐', '긑', '긒', '긓', '긕', '긖', '긗', '긘', '긙', '긚', '긛', '긜', '긝', '긞', '긟', '긠', '긡', '긢', '긣', '긤', '긥', '긦', '긧', '긨', '긩', '긪', '긫', '긬', '긭', '긮', '긯', '긲', '긳', '긵', '긶', '긹', '긻', '긼', '긽', '긾', '긿', '깂', '깄', '깇', '깈', '깉', '깋', '깏', '깑', '깒', '깓', '깕', '깗', '깘', '깙', '깚', '깛', '깞', '깢', '깣', '깤', '깦', '깧', '깪', '깫', '깭', '깮', '깯', '깱', '깲', '깳', '깴', '깵', '깶', '깷', '깺', '깾', '깿', '꺀', '꺁', '꺂', '꺃', '꺆', '꺇', '꺈', '꺉', '꺊', '꺋', '꺍', '꺎', '꺏', '꺐', '꺑', '꺒', '꺓', '꺔', '꺕', '꺖', '꺗', '꺘', '꺙', '꺚', '꺛', '꺜', '꺝', '꺞', '꺟', '꺠', '꺡', '꺢', '꺣', '꺤', '꺥', '꺦', '꺧', '꺨', '꺩', '꺪', '꺫', '꺬', '꺭', '꺮', '꺯', '꺰', '꺱', '꺲', '꺳', '꺴', '꺵', '꺶', '꺷', '꺸', '꺹', '꺺', '꺻', '꺿', '껁', '껂', '껃', '껅', '껆', '껇', '껈', '껉', '껊', '껋', '껎', '껒', '껓', '껔', '껕', '껖', '껗', '껚', '껛', '껝', '껞', '껟', '껠', '껡', '껢', '껣', '껤', '껥', '껦', '껧', '껩', '껪', '껬', '껮', '껯', '껰', '껱', '껲', '껳', '껵', '껶', '껷', '껹', '껺', '껻', '껽', '껾', '껿', '꼀', '꼁', '꼂', '꼃', '꼄', '꼅', '꼆', '꼉', '꼊', '꼋', '꼌', '꼎', '꼏', '꼑', '꼒', '꼓', '꼔', '꼕', '꼖', '꼗', '꼘', '꼙', '꼚', '꼛', '꼜', '꼝', '꼞', '꼟', '꼠', '꼡', '꼢', '꼣', '꼤', '꼥', '꼦', '꼧', '꼨', '꼩', '꼪', '꼫', '꼮', '꼯', '꼱', '꼳', '꼵', '꼶', '꼷', '꼸', '꼹', '꼺', '꼻', '꼾', '꽀', '꽄', '꽅', '꽆', '꽇', '꽊', '꽋', '꽌', '꽍', '꽎', '꽏', '꽑', '꽒', '꽓', '꽔', '꽕', '꽖', '꽗', '꽘', '꽙', '꽚', '꽛', '꽞', '꽟', '꽠', '꽡', '꽢', '꽣', '꽦', '꽧', '꽨', '꽩', '꽪', '꽫', '꽬', '꽭', '꽮', '꽯', '꽰', '꽱', '꽲', '꽳', '꽴', '꽵', '꽶', '꽷', '꽸', '꽺', '꽻', '꽼', '꽽', '꽾', '꽿', '꾁', '꾂', '꾃', '꾅', '꾆', '꾇', '꾉', '꾊', '꾋', '꾌', '꾍', '꾎', '꾏', '꾒', '꾓', '꾔', '꾖', '꾗', '꾘', '꾙', '꾚', '꾛', '꾝', '꾞', '꾟', '꾠', '꾡', '꾢', '꾣', '꾤', '꾥', '꾦', '꾧', '꾨', '꾩', '꾪', '꾫', '꾬', '꾭', '꾮', '꾯', '꾰', '꾱', '꾲', '꾳', '꾴', '꾵', '꾶', '꾷', '꾺', '꾻', '꾽', '꾾', '꾿', '꿁', '꿂', '꿃', '꿄', '꿅', '꿆', '꿊', '꿌', '꿏', '꿐', '꿑', '꿒', '꿓', '꿕', '꿖', '꿗', '꿘', '꿙', '꿚', '꿛', '꿝', '꿞', '꿟', '꿠', '꿡', '꿢', '꿣', '꿤', '꿥', '꿦', '꿧', '꿪', '꿫', '꿬', '꿭', '꿮', '꿯', '꿲', '꿳', '꿵', '꿶', '꿷', '꿹', '꿺', '꿻', '꿼', '꿽', '꿾', '꿿', '뀂', '뀃', '뀅', '뀆', '뀇', '뀈', '뀉', '뀊', '뀋', '뀍', '뀎', '뀏', '뀑', '뀒', '뀓', '뀕', '뀖', '뀗', '뀘', '뀙', '뀚', '뀛', '뀞', '뀟', '뀠', '뀡', '뀢', '뀣', '뀤', '뀥', '뀦', '뀧', '뀩', '뀪', '뀫', '뀬', '뀭', '뀮', '뀯', '뀰', '뀱', '뀲', '뀳', '뀴', '뀵', '뀶', '뀷', '뀸', '뀹', '뀺', '뀻', '뀼', '뀽', '뀾', '뀿', '끀', '끁', '끂', '끃', '끆', '끇', '끉', '끋', '끍', '끏', '끐', '끑', '끒', '끖', '끘', '끚', '끛', '끜', '끞', '끟', '끠', '끡', '끢', '끣', '끤', '끥', '끦', '끧', '끨', '끩', '끪', '끫', '끬', '끭', '끮', '끯', '끰', '끱', '끲', '끳', '끴', '끵', '끶', '끷', '끸', '끹', '끺', '끻', '끾', '끿', '낁', '낂', '낃', '낅', '낆', '낇', '낈', '낉', '낊', '낋', '낎', '낐', '낒', '낓', '낔', '낕', '낖', '낗', '낛', '낝', '낞', '낣', '낤', '낥', '낦', '낧', '낪', '낰', '낲', '낶', '낷', '낹', '낺', '낻', '낽', '낾', '낿', '냀', '냁', '냂', '냃', '냆', '냊', '냋', '냌', '냍', '냎', '냏', '냒', '냓', '냕', '냖', '냗', '냙', '냚', '냛', '냜', '냝', '냞', '냟', '냡', '냢', '냣', '냤', '냦', '냧', '냨', '냩', '냪', '냫', '냬', '냭', '냮', '냯', '냰', '냱', '냲', '냳', '냴', '냵', '냶', '냷', '냸', '냹', '냺', '냻', '냼', '냽', '냾', '냿', '넀', '넁', '넂', '넃', '넄', '넅', '넆', '넇', '넊', '넍', '넎', '넏', '넑', '넔', '넕', '넖', '넗', '넚', '넞', '넟', '넠', '넡', '넢', '넦', '넧', '넩', '넪', '넫', '넭', '넮', '넯', '넰', '넱', '넲', '넳', '넶', '넺', '넻', '넼', '넽', '넾', '넿', '녂', '녃', '녅', '녆', '녇', '녉', '녊', '녋', '녌', '녍', '녎', '녏', '녒', '녓', '녖', '녗', '녙', '녚', '녛', '녝', '녞', '녟', '녡', '녢', '녣', '녤', '녥', '녦', '녧', '녨', '녩', '녪', '녫', '녬', '녭', '녮', '녯', '녰', '녱', '녲', '녳', '녴', '녵', '녶', '녷', '녺', '녻', '녽', '녾', '녿', '놁', '놃', '놄', '놅', '놆', '놇', '놊', '놌', '놎', '놏', '놐', '놑', '놕', '놖', '놗', '놙', '놚', '놛', '놝', '놞', '놟', '놠', '놡', '놢', '놣', '놤', '놥', '놦', '놧', '놩', '놪', '놫', '놬', '놭', '놮', '놯', '놰', '놱', '놲', '놳', '놴', '놵', '놶', '놷', '놸', '놹', '놺', '놻', '놼', '놽', '놾', '놿', '뇀', '뇁', '뇂', '뇃', '뇄', '뇅', '뇆', '뇇', '뇈', '뇉', '뇊', '뇋', '뇍', '뇎', '뇏', '뇑', '뇒', '뇓', '뇕', '뇖', '뇗', '뇘', '뇙', '뇚', '뇛', '뇞', '뇠', '뇡', '뇢', '뇣', '뇤', '뇥', '뇦', '뇧', '뇪', '뇫', '뇭', '뇮', '뇯', '뇱', '뇲', '뇳', '뇴', '뇵', '뇶', '뇷', '뇸', '뇺', '뇼', '뇾', '뇿', '눀', '눁', '눂', '눃', '눆', '눇', '눉', '눊', '눍', '눎', '눏', '눐', '눑', '눒', '눓', '눖', '눘', '눚', '눛', '눜', '눝', '눞', '눟', '눡', '눢', '눣', '눤', '눥', '눦', '눧', '눨', '눩', '눪', '눫', '눬', '눭', '눮', '눯', '눰', '눱', '눲', '눳', '눵', '눶', '눷', '눸', '눹', '눺', '눻', '눽', '눾', '눿', '뉀', '뉁', '뉂', '뉃', '뉄', '뉅', '뉆', '뉇', '뉈', '뉉', '뉊', '뉋', '뉌', '뉍', '뉎', '뉏', '뉐', '뉑', '뉒', '뉓', '뉔', '뉕', '뉖', '뉗', '뉙', '뉚', '뉛', '뉝', '뉞', '뉟', '뉡', '뉢', '뉣', '뉤', '뉥', '뉦', '뉧', '뉪', '뉫', '뉬', '뉭', '뉮', '뉯', '뉰', '뉱', '뉲', '뉳', '뉶', '뉷', '뉸', '뉹', '뉺', '뉻', '뉽', '뉾', '뉿', '늀', '늁', '늂', '늃', '늆', '늇', '늈', '늊', '늋', '늌', '늍', '늎', '늏', '늒', '늓', '늕', '늖', '늗', '늛', '늜', '늝', '늞', '늟', '늢', '늤', '늧', '늨', '늩', '늫', '늭', '늮', '늯', '늱', '늲', '늳', '늵', '늶', '늷', '늸', '늹', '늺', '늻', '늼', '늽', '늾', '늿', '닀', '닁', '닂', '닃', '닄', '닅', '닆', '닇', '닊', '닋', '닍', '닎', '닏', '닑', '닓', '닔', '닕', '닖', '닗', '닚', '닜', '닞', '닟', '닠', '닡', '닣', '닧', '닩', '닪', '닰', '닱', '닲', '닶', '닼', '닽', '닾', '댂', '댃', '댅', '댆', '댇', '댉', '댊', '댋', '댌', '댍', '댎', '댏', '댒', '댖', '댗', '댘', '댙', '댚', '댛', '댝', '댞', '댟', '댠', '댡', '댢', '댣', '댤', '댥', '댦', '댧', '댨', '댩', '댪', '댫', '댬', '댭', '댮', '댯', '댰', '댱', '댲', '댳', '댴', '댵', '댶', '댷', '댸', '댹', '댺', '댻', '댼', '댽', '댾', '댿', '덀', '덁', '덂', '덃', '덄', '덅', '덆', '덇', '덈', '덉', '덊', '덋', '덌', '덍', '덎', '덏', '덐', '덑', '덒', '덓', '덗', '덙', '덚', '덝', '덠', '덡', '덢', '덣', '덦', '덨', '덪', '덬', '덭', '덯', '덲', '덳', '덵', '덶', '덷', '덹', '덺', '덻', '덼', '덽', '덾', '덿', '뎂', '뎆', '뎇', '뎈', '뎉', '뎊', '뎋', '뎍', '뎎', '뎏', '뎑', '뎒', '뎓', '뎕', '뎖', '뎗', '뎘', '뎙', '뎚', '뎛', '뎜', '뎝', '뎞', '뎟', '뎢', '뎣', '뎤', '뎥', '뎦', '뎧', '뎩', '뎪', '뎫', '뎭', '뎮', '뎯', '뎰', '뎱', '뎲', '뎳', '뎴', '뎵', '뎶', '뎷', '뎸', '뎹', '뎺', '뎻', '뎼', '뎽', '뎾', '뎿', '돀', '돁', '돂', '돃', '돆', '돇', '돉', '돊', '돍', '돏', '돑', '돒', '돓', '돖', '돘', '돚', '돜', '돞', '돟', '돡', '돢', '돣', '돥', '돦', '돧', '돩', '돪', '돫', '돬', '돭', '돮', '돯', '돰', '돱', '돲', '돳', '돴', '돵', '돶', '돷', '돸', '돹', '돺', '돻', '돽', '돾', '돿', '됀', '됁', '됂', '됃', '됄', '됅', '됆', '됇', '됈', '됉', '됊', '됋', '됌', '됍', '됎', '됏', '됑', '됒', '됓', '됔', '됕', '됖', '됗', '됙', '됚', '됛', '됝', '됞', '됟', '됡', '됢', '됣', '됤', '됥', '됦', '됧', '됪', '됬', '됭', '됮', '됯', '됰', '됱', '됲', '됳', '됵', '됶', '됷', '됸', '됹', '됺', '됻', '됼', '됽', '됾', '됿', '둀', '둁', '둂', '둃', '둄', '둅', '둆', '둇', '둈', '둉', '둊', '둋', '둌', '둍', '둎', '둏', '둒', '둓', '둕', '둖', '둗', '둙', '둚', '둛', '둜', '둝', '둞', '둟', '둢', '둤', '둦', '둧', '둨', '둩', '둪', '둫', '둭', '둮', '둯', '둰', '둱', '둲', '둳', '둴', '둵', '둶', '둷', '둸', '둹', '둺', '둻', '둼', '둽', '둾', '둿', '뒁', '뒂', '뒃', '뒄', '뒅', '뒆', '뒇', '뒉', '뒊', '뒋', '뒌', '뒍', '뒎', '뒏', '뒐', '뒑', '뒒', '뒓', '뒔', '뒕', '뒖', '뒗', '뒘', '뒙', '뒚', '뒛', '뒜', '뒞', '뒟', '뒠', '뒡', '뒢', '뒣', '뒥', '뒦', '뒧', '뒩', '뒪', '뒫', '뒭', '뒮', '뒯', '뒰', '뒱', '뒲', '뒳', '뒴', '뒶', '뒸', '뒺', '뒻', '뒼', '뒽', '뒾', '뒿', '듁', '듂', '듃', '듅', '듆', '듇', '듉', '듊', '듋', '듌', '듍', '듎', '듏', '듑', '듒', '듓', '듔', '듖', '듗', '듘', '듙', '듚', '듛', '듞', '듟', '듡', '듢', '듥', '듧', '듨', '듩', '듪', '듫', '듮', '듰', '듲', '듳', '듴', '듵', '듶', '듷', '듹', '듺', '듻', '듼', '듽', '듾', '듿', '딀', '딁', '딂', '딃', '딄', '딅', '딆', '딇', '딈', '딉', '딊', '딋', '딌', '딍', '딎', '딏', '딐', '딑', '딒', '딓', '딖', '딗', '딙', '딚', '딝', '딞', '딟', '딠', '딡', '딢', '딣', '딦', '딫', '딬', '딭', '딮', '딯', '딲', '딳', '딵', '딶', '딷', '딹', '딺', '딻', '딼', '딽', '딾', '딿', '땂', '땆', '땇', '땈', '땉', '땊', '땎', '땏', '땑', '땒', '땓', '땕', '땖', '땗', '땘', '땙', '땚', '땛', '땞', '땢', '땣', '땤', '땥', '땦', '땧', '땨', '땩', '땪', '땫', '땬', '땭', '땮', '땯', '땰', '땱', '땲', '땳', '땴', '땵', '땶', '땷', '땸', '땹', '땺', '땻', '땼', '땽', '땾', '땿', '떀', '떁', '떂', '떃', '떄', '떅', '떆', '떇', '떈', '떉', '떊', '떋', '떌', '떍', '떎', '떏', '떐', '떑', '떒', '떓', '떔', '떕', '떖', '떗', '떘', '떙', '떚', '떛', '떜', '떝', '떞', '떟', '떢', '떣', '떥', '떦', '떧', '떩', '떬', '떭', '떮', '떯', '떲', '떶', '떷', '떸', '떹', '떺', '떾', '떿', '뗁', '뗂', '뗃', '뗅', '뗆', '뗇', '뗈', '뗉', '뗊', '뗋', '뗎', '뗒', '뗓', '뗔', '뗕', '뗖', '뗗', '뗙', '뗚', '뗛', '뗜', '뗝', '뗞', '뗟', '뗠', '뗡', '뗢', '뗣', '뗤', '뗥', '뗦', '뗧', '뗨', '뗩', '뗪', '뗫', '뗭', '뗮', '뗯', '뗰', '뗱', '뗲', '뗳', '뗴', '뗵', '뗶', '뗷', '뗸', '뗹', '뗺', '뗻', '뗼', '뗽', '뗾', '뗿', '똀', '똁', '똂', '똃', '똄', '똅', '똆', '똇', '똈', '똉', '똊', '똋', '똌', '똍', '똎', '똏', '똒', '똓', '똕', '똖', '똗', '똙', '똚', '똛', '똜', '똝', '똞', '똟', '똠', '똡', '똢', '똣', '똤', '똦', '똧', '똨', '똩', '똪', '똫', '똭', '똮', '똯', '똰', '똱', '똲', '똳', '똵', '똶', '똷', '똸', '똹', '똺', '똻', '똼', '똽', '똾', '똿', '뙀', '뙁', '뙂', '뙃', '뙄', '뙅', '뙆', '뙇', '뙉', '뙊', '뙋', '뙌', '뙍', '뙎', '뙏', '뙐', '뙑', '뙒', '뙓', '뙔', '뙕', '뙖', '뙗', '뙘', '뙙', '뙚', '뙛', '뙜', '뙝', '뙞', '뙟', '뙠', '뙡', '뙢', '뙣', '뙥', '뙦', '뙧', '뙩', '뙪', '뙫', '뙬', '뙭', '뙮', '뙯', '뙰', '뙱', '뙲', '뙳', '뙴', '뙵', '뙶', '뙷', '뙸', '뙹', '뙺', '뙻', '뙼', '뙽', '뙾', '뙿', '뚀', '뚁', '뚂', '뚃', '뚄', '뚅', '뚆', '뚇', '뚈', '뚉', '뚊', '뚋', '뚌', '뚍', '뚎', '뚏', '뚐', '뚑', '뚒', '뚓', '뚔', '뚕', '뚖', '뚗', '뚘', '뚙', '뚚', '뚛', '뚞', '뚟', '뚡', '뚢', '뚣', '뚥', '뚦', '뚧', '뚨', '뚩', '뚪', '뚭', '뚮', '뚯', '뚰', '뚲', '뚳', '뚴', '뚵', '뚶', '뚷', '뚸', '뚹', '뚺', '뚻', '뚼', '뚽', '뚾', '뚿', '뛀', '뛁', '뛂', '뛃', '뛄', '뛅', '뛆', '뛇', '뛈', '뛉', '뛊', '뛋', '뛌', '뛍', '뛎', '뛏', '뛐', '뛑', '뛒', '뛓', '뛕', '뛖', '뛗', '뛘', '뛙', '뛚', '뛛', '뛜', '뛝', '뛞', '뛟', '뛠', '뛡', '뛢', '뛣', '뛤', '뛥', '뛦', '뛧', '뛨', '뛩', '뛪', '뛫', '뛬', '뛭', '뛮', '뛯', '뛱', '뛲', '뛳', '뛵', '뛶', '뛷', '뛹', '뛺', '뛻', '뛼', '뛽', '뛾', '뛿', '뜂', '뜃', '뜄', '뜆', '뜇', '뜈', '뜉', '뜊', '뜋', '뜌', '뜍', '뜎', '뜏', '뜐', '뜑', '뜒', '뜓', '뜔', '뜕', '뜖', '뜗', '뜘', '뜙', '뜚', '뜛', '뜜', '뜝', '뜞', '뜟', '뜠', '뜡', '뜢', '뜣', '뜤', '뜥', '뜦', '뜧', '뜪', '뜫', '뜭', '뜮', '뜱', '뜲', '뜳', '뜴', '뜵', '뜶', '뜷', '뜺', '뜼', '뜽', '뜾', '뜿', '띀', '띁', '띂', '띃', '띅', '띆', '띇', '띉', '띊', '띋', '띍', '띎', '띏', '띐', '띑', '띒', '띓', '띖', '띗', '띘', '띙', '띚', '띛', '띜', '띝', '띞', '띟', '띡', '띢', '띣', '띥', '띦', '띧', '띩', '띪', '띫', '띬', '띭', '띮', '띯', '띲', '띴', '띶', '띷', '띸', '띹', '띺', '띻', '띾', '띿', '랁', '랂', '랃', '랅', '랆', '랇', '랈', '랉', '랊', '랋', '랎', '랓', '랔', '랕', '랚', '랛', '랝', '랞', '랟', '랡', '랢', '랣', '랤', '랥', '랦', '랧', '랪', '랮', '랯', '랰', '랱', '랲', '랳', '랶', '랷', '랹', '랺', '랻', '랼', '랽', '랾', '랿', '럀', '럁', '럂', '럃', '럄', '럅', '럆', '럈', '럊', '럋', '럌', '럍', '럎', '럏', '럐', '럑', '럒', '럓', '럔', '럕', '럖', '럗', '럘', '럙', '럚', '럛', '럜', '럝', '럞', '럟', '럠', '럡', '럢', '럣', '럤', '럥', '럦', '럧', '럨', '럩', '럪', '럫', '럮', '럯', '럱', '럲', '럳', '럵', '럶', '럷', '럸', '럹', '럺', '럻', '럾', '렂', '렃', '렄', '렅', '렆', '렊', '렋', '렍', '렎', '렏', '렑', '렒', '렓', '렔', '렕', '렖', '렗', '렚', '렜', '렞', '렟', '렠', '렡', '렢', '렣', '렦', '렧', '렩', '렪', '렫', '렭', '렮', '렯', '렰', '렱', '렲', '렳', '렶', '렺', '렻', '렼', '렽', '렾', '렿', '롁', '롂', '롃', '롅', '롆', '롇', '롈', '롉', '롊', '롋', '롌', '롍', '롎', '롏', '롐', '롒', '롔', '롕', '롖', '롗', '롘', '롙', '롚', '롛', '롞', '롟', '롡', '롢', '롣', '롥', '롦', '롧', '롨', '롩', '롪', '롫', '롮', '롰', '롲', '롳', '롴', '롵', '롶', '롷', '롹', '롺', '롻', '롽', '롾', '롿', '뢀', '뢁', '뢂', '뢃', '뢄', '뢅', '뢆', '뢇', '뢈', '뢉', '뢊', '뢋', '뢌', '뢎', '뢏', '뢐', '뢑', '뢒', '뢓', '뢔', '뢕', '뢖', '뢗', '뢘', '뢙', '뢚', '뢛', '뢜', '뢝', '뢞', '뢟', '뢠', '뢡', '뢢', '뢣', '뢤', '뢥', '뢦', '뢧', '뢩', '뢪', '뢫', '뢬', '뢭', '뢮', '뢯', '뢱', '뢲', '뢳', '뢵', '뢶', '뢷', '뢹', '뢺', '뢻', '뢼', '뢽', '뢾', '뢿', '룂', '룄', '룆', '룇', '룈', '룉', '룊', '룋', '룍', '룎', '룏', '룑', '룒', '룓', '룕', '룖', '룗', '룘', '룙', '룚', '룛', '룜', '룞', '룠', '룢', '룣', '룤', '룥', '룦', '룧', '룪', '룫', '룭', '룮', '룯', '룱', '룲', '룳', '룴', '룵', '룶', '룷', '룺', '룼', '룾', '룿', '뤀', '뤁', '뤂', '뤃', '뤅', '뤆', '뤇', '뤈', '뤉', '뤊', '뤋', '뤌', '뤍', '뤎', '뤏', '뤐', '뤑', '뤒', '뤓', '뤔', '뤕', '뤖', '뤗', '뤙', '뤚', '뤛', '뤜', '뤝', '뤞', '뤟', '뤡', '뤢', '뤣', '뤤', '뤥', '뤦', '뤧', '뤨', '뤩', '뤪', '뤫', '뤬', '뤭', '뤮', '뤯', '뤰', '뤱', '뤲', '뤳', '뤴', '뤵', '뤶', '뤷', '뤸', '뤹', '뤺', '뤻', '뤾', '뤿', '륁', '륂', '륃', '륅', '륆', '륇', '륈', '륉', '륊', '륋', '륍', '륎', '륐', '륒', '륓', '륔', '륕', '륖', '륗', '륚', '륛', '륝', '륞', '륟', '륡', '륢', '륣', '륤', '륥', '륦', '륧', '륪', '륬', '륮', '륯', '륰', '륱', '륲', '륳', '륶', '륷', '륹', '륺', '륻', '륽', '륾', '륿', '릀', '릁', '릂', '릃', '릆', '릈', '릋', '릌', '릏', '릐', '릑', '릒', '릓', '릔', '릕', '릖', '릗', '릘', '릙', '릚', '릛', '릜', '릝', '릞', '릟', '릠', '릡', '릢', '릣', '릤', '릥', '릦', '릧', '릨', '릩', '릪', '릫', '릮', '릯', '릱', '릲', '릳', '릵', '릶', '릷', '릸', '릹', '릺', '릻', '릾', '맀', '맂', '맃', '맄', '맅', '맆', '맇', '맊', '맋', '맍', '맓', '맔', '맕', '맖', '맗', '맚', '맜', '맟', '맠', '맢', '맦', '맧', '맩', '맪', '맫', '맭', '맮', '맯', '맰', '맱', '맲', '맳', '맶', '맻', '맼', '맽', '맾', '맿', '먂', '먃', '먄', '먅', '먆', '먇', '먉', '먊', '먋', '먌', '먍', '먎', '먏', '먐', '먑', '먒', '먓', '먔', '먖', '먗', '먘', '먙', '먚', '먛', '먜', '먝', '먞', '먟', '먠', '먡', '먢', '먣', '먤', '먥', '먦', '먧', '먨', '먩', '먪', '먫', '먬', '먭', '먮', '먯', '먰', '먱', '먲', '먳', '먴', '먵', '먶', '먷', '먺', '먻', '먽', '먾', '먿', '멁', '멃', '멄', '멅', '멆', '멇', '멊', '멌', '멏', '멐', '멑', '멒', '멖', '멗', '멙', '멚', '멛', '멝', '멞', '멟', '멠', '멡', '멢', '멣', '멦', '멪', '멫', '멬', '멭', '멮', '멯', '멲', '멳', '멵', '멶', '멷', '멹', '멺', '멻', '멼', '멽', '멾', '멿', '몀', '몁', '몂', '몆', '몈', '몉', '몊', '몋', '몍', '몎', '몏', '몐', '몑', '몒', '몓', '몔', '몕', '몖', '몗', '몘', '몙', '몚', '몛', '몜', '몝', '몞', '몟', '몠', '몡', '몢', '몣', '몤', '몥', '몦', '몧', '몪', '몭', '몮', '몯', '몱', '몳', '몴', '몵', '몶', '몷', '몺', '몼', '몾', '몿', '뫀', '뫁', '뫂', '뫃', '뫅', '뫆', '뫇', '뫉', '뫊', '뫋', '뫌', '뫍', '뫎', '뫏', '뫐', '뫑', '뫒', '뫓', '뫔', '뫕', '뫖', '뫗', '뫚', '뫛', '뫜', '뫝', '뫞', '뫟', '뫠', '뫡', '뫢', '뫣', '뫤', '뫥', '뫦', '뫧', '뫨', '뫩', '뫪', '뫫', '뫬', '뫭', '뫮', '뫯', '뫰', '뫱', '뫲', '뫳', '뫴', '뫵', '뫶', '뫷', '뫸', '뫹', '뫺', '뫻', '뫽', '뫾', '뫿', '묁', '묂', '묃', '묅', '묆', '묇', '묈', '묉', '묊', '묋', '묌', '묎', '묐', '묒', '묓', '묔', '묕', '묖', '묗', '묙', '묚', '묛', '묝', '묞', '묟', '묡', '묢', '묣', '묤', '묥', '묦', '묧', '묨', '묪', '묬', '묭', '묮', '묯', '묰', '묱', '묲', '묳', '묷', '묹', '묺', '묿', '뭀', '뭁', '뭂', '뭃', '뭆', '뭈', '뭊', '뭋', '뭌', '뭎', '뭑', '뭒', '뭓', '뭕', '뭖', '뭗', '뭙', '뭚', '뭛', '뭜', '뭝', '뭞', '뭟', '뭠', '뭢', '뭤', '뭥', '뭦', '뭧', '뭨', '뭩', '뭪', '뭫', '뭭', '뭮', '뭯', '뭰', '뭱', '뭲', '뭳', '뭴', '뭵', '뭶', '뭷', '뭸', '뭹', '뭺', '뭻', '뭼', '뭽', '뭾', '뭿', '뮀', '뮁', '뮂', '뮃', '뮄', '뮅', '뮆', '뮇', '뮉', '뮊', '뮋', '뮍', '뮎', '뮏', '뮑', '뮒', '뮓', '뮔', '뮕', '뮖', '뮗', '뮘', '뮙', '뮚', '뮛', '뮜', '뮝', '뮞', '뮟', '뮠', '뮡', '뮢', '뮣', '뮥', '뮦', '뮧', '뮩', '뮪', '뮫', '뮭', '뮮', '뮯', '뮰', '뮱', '뮲', '뮳', '뮵', '뮶', '뮸', '뮹', '뮺', '뮻', '뮼', '뮽', '뮾', '뮿', '믁', '믂', '믃', '믅', '믆', '믇', '믉', '믊', '믋', '믌', '믍', '믎', '믏', '믑', '믒', '믔', '믕', '믖', '믗', '믘', '믙', '믚', '믛', '믜', '믝', '믞', '믟', '믠', '믡', '믢', '믣', '믤', '믥', '믦', '믧', '믨', '믩', '믪', '믫', '믬', '믭', '믮', '믯', '믰', '믱', '믲', '믳', '믴', '믵', '믶', '믷', '믺', '믻', '믽', '믾', '밁', '밃', '밄', '밅', '밆', '밇', '밊', '밎', '밐', '밒', '밓', '밙', '밚', '밠', '밡', '밢', '밣', '밦', '밨', '밪', '밫', '밬', '밮', '밯', '밲', '밳', '밵', '밶', '밷', '밹', '밺', '밻', '밼', '밽', '밾', '밿', '뱂', '뱆', '뱇', '뱈', '뱊', '뱋', '뱎', '뱏', '뱑', '뱒', '뱓', '뱔', '뱕', '뱖', '뱗', '뱘', '뱙', '뱚', '뱛', '뱜', '뱞', '뱟', '뱠', '뱡', '뱢', '뱣', '뱤', '뱥', '뱦', '뱧', '뱨', '뱩', '뱪', '뱫', '뱬', '뱭', '뱮', '뱯', '뱰', '뱱', '뱲', '뱳', '뱴', '뱵', '뱶', '뱷', '뱸', '뱹', '뱺', '뱻', '뱼', '뱽', '뱾', '뱿', '벀', '벁', '벂', '벃', '벆', '벇', '벉', '벊', '벍', '벏', '벐', '벑', '벒', '벓', '벖', '벘', '벛', '벜', '벝', '벞', '벟', '벢', '벣', '벥', '벦', '벩', '벪', '벫', '벬', '벭', '벮', '벯', '벲', '벶', '벷', '벸', '벹', '벺', '벻', '벾', '벿', '볁', '볂', '볃', '볅', '볆', '볇', '볈', '볉', '볊', '볋', '볌', '볎', '볒', '볓', '볔', '볖', '볗', '볙', '볚', '볛', '볝', '볞', '볟', '볠', '볡', '볢', '볣', '볤', '볥', '볦', '볧', '볨', '볩', '볪', '볫', '볬', '볭', '볮', '볯', '볰', '볱', '볲', '볳', '볷', '볹', '볺', '볻', '볽', '볾', '볿', '봀', '봁', '봂', '봃', '봆', '봈', '봊', '봋', '봌', '봍', '봎', '봏', '봑', '봒', '봓', '봕', '봖', '봗', '봘', '봙', '봚', '봛', '봜', '봝', '봞', '봟', '봠', '봡', '봢', '봣', '봥', '봦', '봧', '봨', '봩', '봪', '봫', '봭', '봮', '봯', '봰', '봱', '봲', '봳', '봴', '봵', '봶', '봷', '봸', '봹', '봺', '봻', '봼', '봽', '봾', '봿', '뵁', '뵂', '뵃', '뵄', '뵅', '뵆', '뵇', '뵊', '뵋', '뵍', '뵎', '뵏', '뵑', '뵒', '뵓', '뵔', '뵕', '뵖', '뵗', '뵚', '뵛', '뵜', '뵝', '뵞', '뵟', '뵠', '뵡', '뵢', '뵣', '뵥', '뵦', '뵧', '뵩', '뵪', '뵫', '뵬', '뵭', '뵮', '뵯', '뵰', '뵱', '뵲', '뵳', '뵴', '뵵', '뵶', '뵷', '뵸', '뵹', '뵺', '뵻', '뵼', '뵽', '뵾', '뵿', '붂', '붃', '붅', '붆', '붋', '붌', '붍', '붎', '붏', '붒', '붔', '붖', '붗', '붘', '붛', '붝', '붞', '붟', '붠', '붡', '붢', '붣', '붥', '붦', '붧', '붨', '붩', '붪', '붫', '붬', '붭', '붮', '붯', '붱', '붲', '붳', '붴', '붵', '붶', '붷', '붹', '붺', '붻', '붼', '붽', '붾', '붿', '뷀', '뷁', '뷂', '뷃', '뷄', '뷅', '뷆', '뷇', '뷈', '뷉', '뷊', '뷋', '뷌', '뷍', '뷎', '뷏', '뷐', '뷑', '뷒', '뷓', '뷖', '뷗', '뷙', '뷚', '뷛', '뷝', '뷞', '뷟', '뷠', '뷡', '뷢', '뷣', '뷤', '뷥', '뷦', '뷧', '뷨', '뷪', '뷫', '뷬', '뷭', '뷮', '뷯', '뷱', '뷲', '뷳', '뷵', '뷶', '뷷', '뷹', '뷺', '뷻', '뷼', '뷽', '뷾', '뷿', '븁', '븂', '븄', '븆', '븇', '븈', '븉', '븊', '븋', '븎', '븏', '븑', '븒', '븓', '븕', '븖', '븗', '븘', '븙', '븚', '븛', '븞', '븠', '븡', '븢', '븣', '븤', '븥', '븦', '븧', '븨', '븩', '븪', '븫', '븬', '븭', '븮', '븯', '븰', '븱', '븲', '븳', '븴', '븵', '븶', '븷', '븸', '븹', '븺', '븻', '븼', '븽', '븾', '븿', '빀', '빁', '빂', '빃', '빆', '빇', '빉', '빊', '빋', '빍', '빏', '빐', '빑', '빒', '빓', '빖', '빘', '빜', '빝', '빞', '빟', '빢', '빣', '빥', '빦', '빧', '빩', '빫', '빬', '빭', '빮', '빯', '빲', '빶', '빷', '빸', '빹', '빺', '빾', '빿', '뺁', '뺂', '뺃', '뺅', '뺆', '뺇', '뺈', '뺉', '뺊', '뺋', '뺎', '뺒', '뺓', '뺔', '뺕', '뺖', '뺗', '뺚', '뺛', '뺜', '뺝', '뺞', '뺟', '뺠', '뺡', '뺢', '뺣', '뺤', '뺥', '뺦', '뺧', '뺩', '뺪', '뺫', '뺬', '뺭', '뺮', '뺯', '뺰', '뺱', '뺲', '뺳', '뺴', '뺵', '뺶', '뺷', '뺸', '뺹', '뺺', '뺻', '뺼', '뺽', '뺾', '뺿', '뻀', '뻁', '뻂', '뻃', '뻄', '뻅', '뻆', '뻇', '뻈', '뻉', '뻊', '뻋', '뻌', '뻍', '뻎', '뻏', '뻒', '뻓', '뻕', '뻖', '뻙', '뻚', '뻛', '뻜', '뻝', '뻞', '뻟', '뻡', '뻢', '뻦', '뻧', '뻨', '뻩', '뻪', '뻫', '뻭', '뻮', '뻯', '뻰', '뻱', '뻲', '뻳', '뻴', '뻵', '뻶', '뻷', '뻸', '뻹', '뻺', '뻻', '뻼', '뻽', '뻾', '뻿', '뼀', '뼂', '뼃', '뼄', '뼅', '뼆', '뼇', '뼊', '뼋', '뼌', '뼍', '뼎', '뼏', '뼐', '뼑', '뼒', '뼓', '뼔', '뼕', '뼖', '뼗', '뼚', '뼞', '뼟', '뼠', '뼡', '뼢', '뼣', '뼤', '뼥', '뼦', '뼧', '뼨', '뼩', '뼪', '뼫', '뼬', '뼭', '뼮', '뼯', '뼰', '뼱', '뼲', '뼳', '뼴', '뼵', '뼶', '뼷', '뼸', '뼹', '뼺', '뼻', '뼼', '뼽', '뼾', '뼿', '뽂', '뽃', '뽅', '뽆', '뽇', '뽉', '뽊', '뽋', '뽌', '뽍', '뽎', '뽏', '뽒', '뽓', '뽔', '뽖', '뽗', '뽘', '뽙', '뽚', '뽛', '뽜', '뽝', '뽞', '뽟', '뽠', '뽡', '뽢', '뽣', '뽤', '뽥', '뽦', '뽧', '뽨', '뽩', '뽪', '뽫', '뽬', '뽭', '뽮', '뽯', '뽰', '뽱', '뽲', '뽳', '뽴', '뽵', '뽶', '뽷', '뽸', '뽹', '뽺', '뽻', '뽼', '뽽', '뽾', '뽿', '뾀', '뾁', '뾂', '뾃', '뾄', '뾅', '뾆', '뾇', '뾈', '뾉', '뾊', '뾋', '뾌', '뾍', '뾎', '뾏', '뾐', '뾑', '뾒', '뾓', '뾕', '뾖', '뾗', '뾘', '뾙', '뾚', '뾛', '뾜', '뾝', '뾞', '뾟', '뾠', '뾡', '뾢', '뾣', '뾤', '뾥', '뾦', '뾧', '뾨', '뾩', '뾪', '뾫', '뾬', '뾭', '뾮', '뾯', '뾱', '뾲', '뾳', '뾴', '뾵', '뾶', '뾷', '뾸', '뾹', '뾺', '뾻', '뾼', '뾽', '뾾', '뾿', '뿀', '뿁', '뿂', '뿃', '뿄', '뿆', '뿇', '뿈', '뿉', '뿊', '뿋', '뿎', '뿏', '뿑', '뿒', '뿓', '뿕', '뿖', '뿗', '뿘', '뿙', '뿚', '뿛', '뿝', '뿞', '뿠', '뿢', '뿣', '뿤', '뿥', '뿦', '뿧', '뿨', '뿩', '뿪', '뿫', '뿬', '뿭', '뿮', '뿯', '뿰', '뿱', '뿲', '뿳', '뿴', '뿵', '뿶', '뿷', '뿸', '뿹', '뿺', '뿻', '뿼', '뿽', '뿾', '뿿', '쀀', '쀁', '쀂', '쀃', '쀄', '쀅', '쀆', '쀇', '쀈', '쀉', '쀊', '쀋', '쀌', '쀍', '쀎', '쀏', '쀐', '쀑', '쀒', '쀓', '쀔', '쀕', '쀖', '쀗', '쀘', '쀙', '쀚', '쀛', '쀜', '쀝', '쀞', '쀟', '쀠', '쀡', '쀢', '쀣', '쀤', '쀥', '쀦', '쀧', '쀨', '쀩', '쀪', '쀫', '쀬', '쀭', '쀮', '쀯', '쀰', '쀱', '쀲', '쀳', '쀴', '쀵', '쀶', '쀷', '쀸', '쀹', '쀺', '쀻', '쀽', '쀾', '쀿', '쁀', '쁁', '쁂', '쁃', '쁄', '쁅', '쁆', '쁇', '쁈', '쁉', '쁊', '쁋', '쁌', '쁍', '쁎', '쁏', '쁐', '쁒', '쁓', '쁔', '쁕', '쁖', '쁗', '쁙', '쁚', '쁛', '쁝', '쁞', '쁟', '쁡', '쁢', '쁣', '쁤', '쁥', '쁦', '쁧', '쁪', '쁫', '쁬', '쁭', '쁮', '쁯', '쁰', '쁱', '쁲', '쁳', '쁴', '쁵', '쁶', '쁷', '쁸', '쁹', '쁺', '쁻', '쁼', '쁽', '쁾', '쁿', '삀', '삁', '삂', '삃', '삄', '삅', '삆', '삇', '삈', '삉', '삊', '삋', '삌', '삍', '삎', '삏', '삒', '삓', '삕', '삖', '삗', '삙', '삚', '삛', '삜', '삝', '삞', '삟', '삢', '삤', '삦', '삧', '삨', '삩', '삪', '삫', '삮', '삱', '삲', '삷', '삸', '삹', '삺', '삻', '삾', '샂', '샃', '샄', '샆', '샇', '샊', '샋', '샍', '샎', '샏', '샑', '샒', '샓', '샔', '샕', '샖', '샗', '샚', '샞', '샟', '샠', '샡', '샢', '샣', '샦', '샧', '샩', '샪', '샫', '샭', '샮', '샯', '샰', '샱', '샲', '샳', '샶', '샸', '샺', '샻', '샼', '샽', '샾', '샿', '섁', '섂', '섃', '섅', '섆', '섇', '섉', '섊', '섋', '섌', '섍', '섎', '섏', '섑', '섒', '섓', '섔', '섖', '섗', '섘', '섙', '섚', '섛', '섡', '섢', '섥', '섨', '섩', '섪', '섫', '섮', '섲', '섳', '섴', '섵', '섷', '섺', '섻', '섽', '섾', '섿', '셁', '셂', '셃', '셄', '셅', '셆', '셇', '셊', '셎', '셏', '셐', '셑', '셒', '셓', '셖', '셗', '셙', '셚', '셛', '셝', '셞', '셟', '셠', '셡', '셢', '셣', '셦', '셪', '셫', '셬', '셭', '셮', '셯', '셱', '셲', '셳', '셵', '셶', '셷', '셹', '셺', '셻', '셼', '셽', '셾', '셿', '솀', '솁', '솂', '솃', '솄', '솆', '솇', '솈', '솉', '솊', '솋', '솏', '솑', '솒', '솓', '솕', '솗', '솘', '솙', '솚', '솛', '솞', '솠', '솢', '솣', '솤', '솦', '솧', '솪', '솫', '솭', '솮', '솯', '솱', '솲', '솳', '솴', '솵', '솶', '솷', '솸', '솹', '솺', '솻', '솼', '솾', '솿', '쇀', '쇁', '쇂', '쇃', '쇅', '쇆', '쇇', '쇉', '쇊', '쇋', '쇍', '쇎', '쇏', '쇐', '쇑', '쇒', '쇓', '쇕', '쇖', '쇙', '쇚', '쇛', '쇜', '쇝', '쇞', '쇟', '쇡', '쇢', '쇣', '쇥', '쇦', '쇧', '쇩', '쇪', '쇫', '쇬', '쇭', '쇮', '쇯', '쇲', '쇴', '쇵', '쇶', '쇷', '쇸', '쇹', '쇺', '쇻', '쇾', '쇿', '숁', '숂', '숃', '숅', '숆', '숇', '숈', '숉', '숊', '숋', '숎', '숐', '숒', '숓', '숔', '숕', '숖', '숗', '숚', '숛', '숝', '숞', '숡', '숢', '숣', '숤', '숥', '숦', '숧', '숪', '숬', '숮', '숰', '숳', '숵', '숶', '숷', '숸', '숹', '숺', '숻', '숼', '숽', '숾', '숿', '쉀', '쉁', '쉂', '쉃', '쉄', '쉅', '쉆', '쉇', '쉉', '쉊', '쉋', '쉌', '쉍', '쉎', '쉏', '쉒', '쉓', '쉕', '쉖', '쉗', '쉙', '쉚', '쉛', '쉜', '쉝', '쉞', '쉟', '쉡', '쉢', '쉣', '쉤', '쉦', '쉧', '쉨', '쉩', '쉪', '쉫', '쉮', '쉯', '쉱', '쉲', '쉳', '쉵', '쉶', '쉷', '쉸', '쉹', '쉺', '쉻', '쉾', '슀', '슂', '슃', '슄', '슅', '슆', '슇', '슊', '슋', '슌', '슍', '슎', '슏', '슑', '슒', '슓', '슔', '슕', '슖', '슗', '슙', '슚', '슜', '슞', '슟', '슠', '슡', '슢', '슣', '슦', '슧', '슩', '슪', '슫', '슮', '슯', '슰', '슱', '슲', '슳', '슶', '슸', '슺', '슻', '슼', '슽', '슾', '슿', '싀', '싁', '싂', '싃', '싄', '싅', '싆', '싇', '싈', '싉', '싊', '싋', '싌', '싍', '싎', '싏', '싐', '싑', '싒', '싓', '싔', '싕', '싖', '싗', '싘', '싙', '싚', '싛', '싞', '싟', '싡', '싢', '싥', '싦', '싧', '싨', '싩', '싪', '싮', '싰', '싲', '싳', '싴', '싵', '싷', '싺', '싽', '싾', '싿', '쌁', '쌂', '쌃', '쌄', '쌅', '쌆', '쌇', '쌊', '쌋', '쌎', '쌏', '쌐', '쌑', '쌒', '쌖', '쌗', '쌙', '쌚', '쌛', '쌝', '쌞', '쌟', '쌠', '쌡', '쌢', '쌣', '쌦', '쌧', '쌪', '쌫', '쌬', '쌭', '쌮', '쌯', '쌰', '쌱', '쌲', '쌳', '쌴', '쌵', '쌶', '쌷', '쌸', '쌹', '쌺', '쌻', '쌼', '쌽', '쌾', '쌿', '썀', '썁', '썂', '썃', '썄', '썆', '썇', '썈', '썉', '썊', '썋', '썌', '썍', '썎', '썏', '썐', '썑', '썒', '썓', '썔', '썕', '썖', '썗', '썘', '썙', '썚', '썛', '썜', '썝', '썞', '썟', '썠', '썡', '썢', '썣', '썤', '썥', '썦', '썧', '썪', '썫', '썭', '썮', '썯', '썱', '썳', '썴', '썵', '썶', '썷', '썺', '썻', '썾', '썿', '쎀', '쎁', '쎂', '쎃', '쎅', '쎆', '쎇', '쎉', '쎊', '쎋', '쎍', '쎎', '쎏', '쎐', '쎑', '쎒', '쎓', '쎔', '쎕', '쎖', '쎗', '쎘', '쎙', '쎚', '쎛', '쎜', '쎝', '쎞', '쎟', '쎠', '쎡', '쎢', '쎣', '쎤', '쎥', '쎦', '쎧', '쎨', '쎩', '쎪', '쎫', '쎬', '쎭', '쎮', '쎯', '쎰', '쎱', '쎲', '쎳', '쎴', '쎵', '쎶', '쎷', '쎸', '쎹', '쎺', '쎻', '쎼', '쎽', '쎾', '쎿', '쏁', '쏂', '쏃', '쏄', '쏅', '쏆', '쏇', '쏈', '쏉', '쏊', '쏋', '쏌', '쏍', '쏎', '쏏', '쏐', '쏑', '쏒', '쏓', '쏔', '쏕', '쏖', '쏗', '쏚', '쏛', '쏝', '쏞', '쏡', '쏣', '쏤', '쏥', '쏦', '쏧', '쏪', '쏫', '쏬', '쏮', '쏯', '쏰', '쏱', '쏲', '쏳', '쏶', '쏷', '쏹', '쏺', '쏻', '쏼', '쏽', '쏾', '쏿', '쐀', '쐁', '쐂', '쐃', '쐄', '쐅', '쐆', '쐇', '쐉', '쐊', '쐋', '쐌', '쐍', '쐎', '쐏', '쐑', '쐒', '쐓', '쐔', '쐕', '쐖', '쐗', '쐘', '쐙', '쐚', '쐛', '쐜', '쐝', '쐞', '쐟', '쐠', '쐡', '쐢', '쐣', '쐥', '쐦', '쐧', '쐨', '쐩', '쐪', '쐫', '쐭', '쐮', '쐯', '쐱', '쐲', '쐳', '쐵', '쐶', '쐷', '쐸', '쐹', '쐺', '쐻', '쐾', '쐿', '쑀', '쑁', '쑂', '쑃', '쑄', '쑅', '쑆', '쑇', '쑉', '쑊', '쑋', '쑌', '쑍', '쑎', '쑏', '쑐', '쑑', '쑒', '쑓', '쑔', '쑕', '쑖', '쑗', '쑘', '쑙', '쑚', '쑛', '쑜', '쑝', '쑞', '쑟', '쑠', '쑡', '쑢', '쑣', '쑦', '쑧', '쑩', '쑪', '쑫', '쑭', '쑮', '쑯', '쑰', '쑱', '쑲', '쑳', '쑶', '쑷', '쑸', '쑺', '쑻', '쑼', '쑽', '쑾', '쑿', '쒁', '쒂', '쒃', '쒄', '쒅', '쒆', '쒇', '쒈', '쒉', '쒊', '쒋', '쒌', '쒍', '쒎', '쒏', '쒐', '쒑', '쒒', '쒓', '쒕', '쒖', '쒗', '쒘', '쒙', '쒚', '쒛', '쒝', '쒞', '쒟', '쒠', '쒡', '쒢', '쒣', '쒤', '쒥', '쒦', '쒧', '쒨', '쒩', '쒪', '쒫', '쒬', '쒭', '쒮', '쒯', '쒰', '쒱', '쒲', '쒳', '쒴', '쒵', '쒶', '쒷', '쒹', '쒺', '쒻', '쒽', '쒾', '쒿', '쓀', '쓁', '쓂', '쓃', '쓄', '쓅', '쓆', '쓇', '쓈', '쓉', '쓊', '쓋', '쓌', '쓍', '쓎', '쓏', '쓐', '쓑', '쓒', '쓓', '쓔', '쓕', '쓖', '쓗', '쓘', '쓙', '쓚', '쓛', '쓜', '쓝', '쓞', '쓟', '쓠', '쓡', '쓢', '쓣', '쓤', '쓥', '쓦', '쓧', '쓨', '쓪', '쓫', '쓬', '쓭', '쓮', '쓯', '쓲', '쓳', '쓵', '쓶', '쓷', '쓹', '쓻', '쓼', '쓽', '쓾', '씂', '씃', '씄', '씅', '씆', '씇', '씈', '씉', '씊', '씋', '씍', '씎', '씏', '씑', '씒', '씓', '씕', '씖', '씗', '씘', '씙', '씚', '씛', '씝', '씞', '씟', '씠', '씡', '씢', '씣', '씤', '씥', '씦', '씧', '씪', '씫', '씭', '씮', '씯', '씱', '씲', '씳', '씴', '씵', '씶', '씷', '씺', '씼', '씾', '씿', '앀', '앁', '앂', '앃', '앆', '앇', '앋', '앏', '앐', '앑', '앒', '앖', '앚', '앛', '앜', '앟', '앢', '앣', '앥', '앦', '앧', '앩', '앪', '앫', '앬', '앭', '앮', '앯', '앲', '앶', '앷', '앸', '앹', '앺', '앻', '앾', '앿', '얁', '얂', '얃', '얅', '얆', '얈', '얉', '얊', '얋', '얎', '얐', '얒', '얓', '얔', '얖', '얙', '얚', '얛', '얝', '얞', '얟', '얡', '얢', '얣', '얤', '얥', '얦', '얧', '얨', '얪', '얫', '얬', '얭', '얮', '얯', '얰', '얱', '얲', '얳', '얶', '얷', '얺', '얿', '엀', '엁', '엂', '엃', '엋', '엍', '엏', '엒', '엓', '엕', '엖', '엗', '엙', '엚', '엛', '엜', '엝', '엞', '엟', '엢', '엤', '엦', '엧', '엨', '엩', '엪', '엫', '엯', '엱', '엲', '엳', '엵', '엸', '엹', '엺', '엻', '옂', '옃', '옄', '옉', '옊', '옋', '옍', '옎', '옏', '옑', '옒', '옓', '옔', '옕', '옖', '옗', '옚', '옝', '옞', '옟', '옠', '옡', '옢', '옣', '옦', '옧', '옩', '옪', '옫', '옯', '옱', '옲', '옶', '옸', '옺', '옼', '옽', '옾', '옿', '왂', '왃', '왅', '왆', '왇', '왉', '왊', '왋', '왌', '왍', '왎', '왏', '왒', '왖', '왗', '왘', '왙', '왚', '왛', '왞', '왟', '왡', '왢', '왣', '왤', '왥', '왦', '왧', '왨', '왩', '왪', '왫', '왭', '왮', '왰', '왲', '왳', '왴', '왵', '왶', '왷', '왺', '왻', '왽', '왾', '왿', '욁', '욂', '욃', '욄', '욅', '욆', '욇', '욊', '욌', '욎', '욏', '욐', '욑', '욒', '욓', '욖', '욗', '욙', '욚', '욛', '욝', '욞', '욟', '욠', '욡', '욢', '욣', '욦', '욨', '욪', '욫', '욬', '욭', '욮', '욯', '욲', '욳', '욵', '욶', '욷', '욻', '욼', '욽', '욾', '욿', '웂', '웄', '웆', '웇', '웈', '웉', '웊', '웋', '웎', '웏', '웑', '웒', '웓', '웕', '웖', '웗', '웘', '웙', '웚', '웛', '웞', '웟', '웢', '웣', '웤', '웥', '웦', '웧', '웪', '웫', '웭', '웮', '웯', '웱', '웲', '웳', '웴', '웵', '웶', '웷', '웺', '웻', '웼', '웾', '웿', '윀', '윁', '윂', '윃', '윆', '윇', '윉', '윊', '윋', '윍', '윎', '윏', '윐', '윑', '윒', '윓', '윖', '윘', '윚', '윛', '윜', '윝', '윞', '윟', '윢', '윣', '윥', '윦', '윧', '윩', '윪', '윫', '윬', '윭', '윮', '윯', '윲', '윴', '윶', '윸', '윹', '윺', '윻', '윾', '윿', '읁', '읂', '읃', '읅', '읆', '읇', '읈', '읉', '읋', '읎', '읐', '읙', '읚', '읛', '읝', '읞', '읟', '읡', '읢', '읣', '읤', '읥', '읦', '읧', '읩', '읪', '읬', '읭', '읮', '읯', '읰', '읱', '읲', '읳', '읶', '읷', '읹', '읺', '읻', '읿', '잀', '잁', '잂', '잆', '잋', '잌', '잍', '잏', '잒', '잓', '잕', '잙', '잛', '잜', '잝', '잞', '잟', '잢', '잧', '잨', '잩', '잪', '잫', '잮', '잯', '잱', '잲', '잳', '잵', '잶', '잷', '잸', '잹', '잺', '잻', '잾', '쟂', '쟃', '쟄', '쟅', '쟆', '쟇', '쟊', '쟋', '쟍', '쟏', '쟑', '쟒', '쟓', '쟔', '쟕', '쟖', '쟗', '쟙', '쟚', '쟛', '쟜', '쟞', '쟟', '쟠', '쟡', '쟢', '쟣', '쟥', '쟦', '쟧', '쟩', '쟪', '쟫', '쟭', '쟮', '쟯', '쟰', '쟱', '쟲', '쟳', '쟴', '쟵', '쟶', '쟷', '쟸', '쟹', '쟺', '쟻', '쟼', '쟽', '쟾', '쟿', '젂', '젃', '젅', '젆', '젇', '젉', '젋', '젌', '젍', '젎', '젏', '젒', '젔', '젗', '젘', '젙', '젚', '젛', '젞', '젟', '젡', '젢', '젣', '젥', '젦', '젧', '젨', '젩', '젪', '젫', '젮', '젰', '젲', '젳', '젴', '젵', '젶', '젷', '젹', '젺', '젻', '젽', '젾', '젿', '졁', '졂', '졃', '졄', '졅', '졆', '졇', '졊', '졋', '졎', '졏', '졐', '졑', '졒', '졓', '졕', '졖', '졗', '졘', '졙', '졚', '졛', '졜', '졝', '졞', '졟', '졠', '졡', '졢', '졣', '졤', '졥', '졦', '졧', '졨', '졩', '졪', '졫', '졬', '졭', '졮', '졯', '졲', '졳', '졵', '졶', '졷', '졹', '졻', '졼', '졽', '졾', '졿', '좂', '좄', '좈', '좉', '좊', '좎', '좏', '좐', '좑', '좒', '좓', '좕', '좖', '좗', '좘', '좙', '좚', '좛', '좜', '좞', '좠', '좢', '좣', '좤', '좥', '좦', '좧', '좩', '좪', '좫', '좬', '좭', '좮', '좯', '좰', '좱', '좲', '좳', '좴', '좵', '좶', '좷', '좸', '좹', '좺', '좻', '좾', '좿', '죀', '죁', '죂', '죃', '죅', '죆', '죇', '죉', '죊', '죋', '죍', '죎', '죏', '죐', '죑', '죒', '죓', '죖', '죘', '죚', '죛', '죜', '죝', '죞', '죟', '죢', '죣', '죥', '죦', '죧', '죨', '죩', '죪', '죫', '죬', '죭', '죮', '죯', '죰', '죱', '죲', '죳', '죴', '죶', '죷', '죸', '죹', '죺', '죻', '죾', '죿', '줁', '줂', '줃', '줇', '줈', '줉', '줊', '줋', '줎', '줐', '줒', '줓', '줔', '줕', '줖', '줗', '줙', '줚', '줛', '줜', '줝', '줞', '줟', '줠', '줡', '줢', '줣', '줤', '줥', '줦', '줧', '줨', '줩', '줪', '줫', '줭', '줮', '줯', '줰', '줱', '줲', '줳', '줵', '줶', '줷', '줸', '줹', '줺', '줻', '줼', '줽', '줾', '줿', '쥀', '쥁', '쥂', '쥃', '쥄', '쥅', '쥆', '쥇', '쥈', '쥉', '쥊', '쥋', '쥌', '쥍', '쥎', '쥏', '쥒', '쥓', '쥕', '쥖', '쥗', '쥙', '쥚', '쥛', '쥜', '쥝', '쥞', '쥟', '쥢', '쥤', '쥥', '쥦', '쥧', '쥨', '쥩', '쥪', '쥫', '쥭', '쥮', '쥯', '쥱', '쥲', '쥳', '쥵', '쥶', '쥷', '쥸', '쥹', '쥺', '쥻', '쥽', '쥾', '쥿', '즀', '즁', '즂', '즃', '즄', '즅', '즆', '즇', '즊', '즋', '즍', '즎', '즏', '즑', '즒', '즓', '즔', '즕', '즖', '즗', '즚', '즜', '즞', '즟', '즠', '즡', '즢', '즣', '즤', '즥', '즦', '즧', '즨', '즩', '즪', '즫', '즬', '즭', '즮', '즯', '즰', '즱', '즲', '즳', '즴', '즵', '즶', '즷', '즸', '즹', '즺', '즻', '즼', '즽', '즾', '즿', '짂', '짃', '짅', '짆', '짉', '짋', '짌', '짍', '짎', '짏', '짒', '짔', '짗', '짘', '짛', '짞', '짟', '짡', '짣', '짥', '짦', '짨', '짩', '짪', '짫', '짮', '짲', '짳', '짴', '짵', '짶', '짷', '짺', '짻', '짽', '짾', '짿', '쨁', '쨂', '쨃', '쨄', '쨅', '쨆', '쨇', '쨊', '쨎', '쨏', '쨐', '쨑', '쨒', '쨓', '쨕', '쨖', '쨗', '쨙', '쨚', '쨛', '쨜', '쨝', '쨞', '쨟', '쨠', '쨡', '쨢', '쨣', '쨤', '쨥', '쨦', '쨧', '쨨', '쨪', '쨫', '쨬', '쨭', '쨮', '쨯', '쨰', '쨱', '쨲', '쨳', '쨴', '쨵', '쨶', '쨷', '쨸', '쨹', '쨺', '쨻', '쨼', '쨽', '쨾', '쨿', '쩀', '쩁', '쩂', '쩃', '쩄', '쩅', '쩆', '쩇', '쩈', '쩉', '쩊', '쩋', '쩎', '쩏', '쩑', '쩒', '쩓', '쩕', '쩖', '쩗', '쩘', '쩙', '쩚', '쩛', '쩞', '쩢', '쩣', '쩤', '쩥', '쩦', '쩧', '쩩', '쩪', '쩫', '쩬', '쩭', '쩮', '쩯', '쩰', '쩱', '쩲', '쩳', '쩴', '쩵', '쩶', '쩷', '쩸', '쩹', '쩺', '쩻', '쩼', '쩾', '쩿', '쪀', '쪁', '쪂', '쪃', '쪅', '쪆', '쪇', '쪈', '쪉', '쪊', '쪋', '쪌', '쪍', '쪎', '쪏', '쪐', '쪑', '쪒', '쪓', '쪔', '쪕', '쪖', '쪗', '쪙', '쪚', '쪛', '쪜', '쪝', '쪞', '쪟', '쪠', '쪡', '쪢', '쪣', '쪤', '쪥', '쪦', '쪧', '쪨', '쪩', '쪪', '쪫', '쪬', '쪭', '쪮', '쪯', '쪰', '쪱', '쪲', '쪳', '쪴', '쪵', '쪶', '쪷', '쪸', '쪹', '쪺', '쪻', '쪾', '쪿', '쫁', '쫂', '쫃', '쫅', '쫆', '쫇', '쫈', '쫉', '쫊', '쫋', '쫎', '쫐', '쫒', '쫔', '쫕', '쫖', '쫗', '쫚', '쫛', '쫜', '쫝', '쫞', '쫟', '쫡', '쫢', '쫣', '쫤', '쫥', '쫦', '쫧', '쫨', '쫩', '쫪', '쫫', '쫭', '쫮', '쫯', '쫰', '쫱', '쫲', '쫳', '쫵', '쫶', '쫷', '쫸', '쫹', '쫺', '쫻', '쫼', '쫽', '쫾', '쫿', '쬀', '쬁', '쬂', '쬃', '쬄', '쬅', '쬆', '쬇', '쬉', '쬊', '쬋', '쬌', '쬍', '쬎', '쬏', '쬑', '쬒', '쬓', '쬕', '쬖', '쬗', '쬙', '쬚', '쬛', '쬜', '쬝', '쬞', '쬟', '쬢', '쬣', '쬤', '쬥', '쬦', '쬧', '쬨', '쬩', '쬪', '쬫', '쬬', '쬭', '쬮', '쬯', '쬰', '쬱', '쬲', '쬳', '쬴', '쬵', '쬶', '쬷', '쬸', '쬹', '쬺', '쬻', '쬼', '쬽', '쬾', '쬿', '쭀', '쭂', '쭃', '쭄', '쭅', '쭆', '쭇', '쭊', '쭋', '쭍', '쭎', '쭏', '쭑', '쭒', '쭓', '쭔', '쭕', '쭖', '쭗', '쭚', '쭛', '쭜', '쭞', '쭟', '쭠', '쭡', '쭢', '쭣', '쭥', '쭦', '쭧', '쭨', '쭩', '쭪', '쭫', '쭬', '쭭', '쭮', '쭯', '쭰', '쭱', '쭲', '쭳', '쭴', '쭵', '쭶', '쭷', '쭺', '쭻', '쭼', '쭽', '쭾', '쭿', '쮀', '쮁', '쮂', '쮃', '쮄', '쮅', '쮆', '쮇', '쮈', '쮉', '쮊', '쮋', '쮌', '쮍', '쮎', '쮏', '쮐', '쮑', '쮒', '쮓', '쮔', '쮕', '쮖', '쮗', '쮘', '쮙', '쮚', '쮛', '쮝', '쮞', '쮟', '쮠', '쮡', '쮢', '쮣', '쮤', '쮥', '쮦', '쮧', '쮨', '쮩', '쮪', '쮫', '쮬', '쮭', '쮮', '쮯', '쮰', '쮱', '쮲', '쮳', '쮴', '쮵', '쮶', '쮷', '쮹', '쮺', '쮻', '쮼', '쮽', '쮾', '쮿', '쯀', '쯁', '쯂', '쯃', '쯄', '쯅', '쯆', '쯇', '쯈', '쯉', '쯊', '쯋', '쯌', '쯍', '쯎', '쯏', '쯐', '쯑', '쯒', '쯓', '쯕', '쯖', '쯗', '쯘', '쯙', '쯚', '쯛', '쯜', '쯝', '쯞', '쯟', '쯠', '쯡', '쯢', '쯣', '쯥', '쯦', '쯨', '쯪', '쯫', '쯬', '쯭', '쯮', '쯯', '쯰', '쯱', '쯲', '쯳', '쯴', '쯵', '쯶', '쯷', '쯸', '쯹', '쯺', '쯻', '쯼', '쯽', '쯾', '쯿', '찀', '찁', '찂', '찃', '찄', '찅', '찆', '찇', '찈', '찉', '찊', '찋', '찎', '찏', '찑', '찒', '찓', '찕', '찖', '찗', '찘', '찙', '찚', '찛', '찞', '찟', '찠', '찣', '찤', '찥', '찦', '찪', '찫', '찭', '찯', '찱', '찲', '찳', '찴', '찵', '찶', '찷', '찺', '찿', '챀', '챁', '챂', '챃', '챆', '챇', '챉', '챊', '챋', '챍', '챎', '챏', '챐', '챑', '챒', '챓', '챖', '챚', '챛', '챜', '챝', '챞', '챟', '챡', '챢', '챣', '챥', '챧', '챩', '챪', '챫', '챬', '챭', '챮', '챯', '챱', '챲', '챳', '챴', '챶', '챷', '챸', '챹', '챺', '챻', '챼', '챽', '챾', '챿', '첀', '첁', '첂', '첃', '첄', '첅', '첆', '첇', '첈', '첉', '첊', '첋', '첌', '첍', '첎', '첏', '첐', '첑', '첒', '첓', '첔', '첕', '첖', '첗', '첚', '첛', '첝', '첞', '첟', '첡', '첢', '첣', '첤', '첥', '첦', '첧', '첪', '첮', '첯', '첰', '첱', '첲', '첳', '첶', '첷', '첹', '첺', '첻', '첽', '첾', '첿', '쳀', '쳁', '쳂', '쳃', '쳆', '쳈', '쳊', '쳋', '쳌', '쳍', '쳎', '쳏', '쳑', '쳒', '쳓', '쳕', '쳖', '쳗', '쳘', '쳙', '쳚', '쳛', '쳜', '쳝', '쳞', '쳟', '쳠', '쳡', '쳢', '쳣', '쳥', '쳦', '쳧', '쳨', '쳩', '쳪', '쳫', '쳭', '쳮', '쳯', '쳱', '쳲', '쳳', '쳴', '쳵', '쳶', '쳷', '쳸', '쳹', '쳺', '쳻', '쳼', '쳽', '쳾', '쳿', '촀', '촂', '촃', '촄', '촅', '촆', '촇', '촊', '촋', '촍', '촎', '촏', '촑', '촒', '촓', '촔', '촕', '촖', '촗', '촚', '촜', '촞', '촟', '촠', '촡', '촢', '촣', '촥', '촦', '촧', '촩', '촪', '촫', '촭', '촮', '촯', '촰', '촱', '촲', '촳', '촴', '촵', '촶', '촷', '촸', '촺', '촻', '촼', '촽', '촾', '촿', '쵀', '쵁', '쵂', '쵃', '쵄', '쵅', '쵆', '쵇', '쵈', '쵉', '쵊', '쵋', '쵌', '쵍', '쵎', '쵏', '쵐', '쵑', '쵒', '쵓', '쵔', '쵕', '쵖', '쵗', '쵘', '쵙', '쵚', '쵛', '쵝', '쵞', '쵟', '쵡', '쵢', '쵣', '쵥', '쵦', '쵧', '쵨', '쵩', '쵪', '쵫', '쵮', '쵰', '쵲', '쵳', '쵴', '쵵', '쵶', '쵷', '쵹', '쵺', '쵻', '쵼', '쵽', '쵾', '쵿', '춀', '춁', '춂', '춃', '춄', '춅', '춆', '춇', '춉', '춊', '춋', '춌', '춍', '춎', '춏', '춐', '춑', '춒', '춓', '춖', '춗', '춙', '춚', '춛', '춝', '춞', '춟', '춠', '춡', '춢', '춣', '춦', '춨', '춪', '춫', '춬', '춭', '춮', '춯', '춱', '춲', '춳', '춴', '춵', '춶', '춷', '춸', '춹', '춺', '춻', '춼', '춽', '춾', '춿', '췀', '췁', '췂', '췃', '췅', '췆', '췇', '췈', '췉', '췊', '췋', '췍', '췎', '췏', '췑', '췒', '췓', '췔', '췕', '췖', '췗', '췘', '췙', '췚', '췛', '췜', '췝', '췞', '췟', '췠', '췡', '췢', '췣', '췤', '췥', '췦', '췧', '췩', '췪', '췫', '췭', '췮', '췯', '췱', '췲', '췳', '췴', '췵', '췶', '췷', '췺', '췼', '췾', '췿', '츀', '츁', '츂', '츃', '츅', '츆', '츇', '츉', '츊', '츋', '츍', '츎', '츏', '츐', '츑', '츒', '츓', '츕', '츖', '츗', '츘', '츚', '츛', '츜', '츝', '츞', '츟', '츢', '츣', '츥', '츦', '츧', '츩', '츪', '츫', '츬', '츭', '츮', '츯', '츲', '츴', '츶', '츷', '츸', '츹', '츺', '츻', '츼', '츽', '츾', '츿', '칀', '칁', '칂', '칃', '칄', '칅', '칆', '칇', '칈', '칉', '칊', '칋', '칌', '칍', '칎', '칏', '칐', '칑', '칒', '칓', '칔', '칕', '칖', '칗', '칚', '칛', '칝', '칞', '칢', '칣', '칤', '칥', '칦', '칧', '칪', '칬', '칮', '칯', '칰', '칱', '칲', '칳', '칶', '칷', '칹', '칺', '칻', '칽', '칾', '칿', '캀', '캁', '캂', '캃', '캆', '캈', '캊', '캋', '캌', '캍', '캎', '캏', '캒', '캓', '캕', '캖', '캗', '캙', '캚', '캛', '캜', '캝', '캞', '캟', '캢', '캦', '캧', '캨', '캩', '캪', '캫', '캮', '캯', '캰', '캱', '캲', '캳', '캴', '캵', '캶', '캷', '캸', '캹', '캺', '캻', '캼', '캽', '캾', '캿', '컀', '컂', '컃', '컄', '컅', '컆', '컇', '컈', '컉', '컊', '컋', '컌', '컍', '컎', '컏', '컐', '컑', '컒', '컓', '컔', '컕', '컖', '컗', '컘', '컙', '컚', '컛', '컜', '컝', '컞', '컟', '컠', '컡', '컢', '컣', '컦', '컧', '컩', '컪', '컭', '컮', '컯', '컰', '컱', '컲', '컳', '컶', '컺', '컻', '컼', '컽', '컾', '컿', '켂', '켃', '켅', '켆', '켇', '켉', '켊', '켋', '켌', '켍', '켎', '켏', '켒', '켔', '켖', '켗', '켘', '켙', '켚', '켛', '켝', '켞', '켟', '켡', '켢', '켣', '켥', '켦', '켧', '켨', '켩', '켪', '켫', '켮', '켲', '켳', '켴', '켵', '켶', '켷', '켹', '켺', '켻', '켼', '켽', '켾', '켿', '콀', '콁', '콂', '콃', '콄', '콅', '콆', '콇', '콈', '콉', '콊', '콋', '콌', '콍', '콎', '콏', '콐', '콑', '콒', '콓', '콖', '콗', '콙', '콚', '콛', '콝', '콞', '콟', '콠', '콡', '콢', '콣', '콦', '콨', '콪', '콫', '콬', '콭', '콮', '콯', '콲', '콳', '콵', '콶', '콷', '콹', '콺', '콻', '콼', '콽', '콾', '콿', '쾁', '쾂', '쾃', '쾄', '쾆', '쾇', '쾈', '쾉', '쾊', '쾋', '쾍', '쾎', '쾏', '쾐', '쾑', '쾒', '쾓', '쾔', '쾕', '쾖', '쾗', '쾘', '쾙', '쾚', '쾛', '쾜', '쾝', '쾞', '쾟', '쾠', '쾢', '쾣', '쾤', '쾥', '쾦', '쾧', '쾩', '쾪', '쾫', '쾬', '쾭', '쾮', '쾯', '쾱', '쾲', '쾳', '쾴', '쾵', '쾶', '쾷', '쾸', '쾹', '쾺', '쾻', '쾼', '쾽', '쾾', '쾿', '쿀', '쿁', '쿂', '쿃', '쿅', '쿆', '쿇', '쿈', '쿉', '쿊', '쿋', '쿌', '쿍', '쿎', '쿏', '쿐', '쿑', '쿒', '쿓', '쿔', '쿕', '쿖', '쿗', '쿘', '쿙', '쿚', '쿛', '쿜', '쿝', '쿞', '쿟', '쿢', '쿣', '쿥', '쿦', '쿧', '쿩', '쿪', '쿫', '쿬', '쿭', '쿮', '쿯', '쿲', '쿴', '쿶', '쿷', '쿸', '쿹', '쿺', '쿻', '쿽', '쿾', '쿿', '퀁', '퀂', '퀃', '퀅', '퀆', '퀇', '퀈', '퀉', '퀊', '퀋', '퀌', '퀍', '퀎', '퀏', '퀐', '퀒', '퀓', '퀔', '퀕', '퀖', '퀗', '퀙', '퀚', '퀛', '퀜', '퀝', '퀞', '퀟', '퀠', '퀡', '퀢', '퀣', '퀤', '퀥', '퀦', '퀧', '퀨', '퀩', '퀪', '퀫', '퀬', '퀮', '퀯', '퀰', '퀱', '퀲', '퀳', '퀶', '퀷', '퀹', '퀺', '퀻', '퀽', '퀾', '퀿', '큀', '큁', '큂', '큃', '큆', '큈', '큊', '큋', '큌', '큍', '큎', '큏', '큑', '큒', '큓', '큕', '큖', '큗', '큙', '큚', '큛', '큜', '큝', '큞', '큟', '큡', '큢', '큣', '큤', '큥', '큦', '큧', '큨', '큩', '큪', '큫', '큮', '큯', '큱', '큲', '큳', '큵', '큶', '큷', '큸', '큹', '큺', '큻', '큾', '큿', '킀', '킂', '킃', '킄', '킅', '킆', '킇', '킈', '킉', '킊', '킋', '킌', '킍', '킎', '킏', '킐', '킑', '킒', '킓', '킔', '킕', '킖', '킗', '킘', '킙', '킚', '킛', '킜', '킝', '킞', '킟', '킠', '킡', '킢', '킣', '킦', '킧', '킩', '킪', '킫', '킭', '킮', '킯', '킰', '킱', '킲', '킳', '킶', '킸', '킺', '킻', '킼', '킽', '킾', '킿', '탂', '탃', '탅', '탆', '탇', '탊', '탋', '탌', '탍', '탎', '탏', '탒', '탖', '탗', '탘', '탙', '탚', '탛', '탞', '탟', '탡', '탢', '탣', '탥', '탦', '탧', '탨', '탩', '탪', '탫', '탮', '탲', '탳', '탴', '탵', '탶', '탷', '탹', '탺', '탻', '탼', '탽', '탾', '탿', '턀', '턁', '턂', '턃', '턄', '턅', '턆', '턇', '턈', '턉', '턊', '턋', '턌', '턎', '턏', '턐', '턑', '턒', '턓', '턔', '턕', '턖', '턗', '턘', '턙', '턚', '턛', '턜', '턝', '턞', '턟', '턠', '턡', '턢', '턣', '턤', '턥', '턦', '턧', '턨', '턩', '턪', '턫', '턬', '턭', '턮', '턯', '턲', '턳', '턵', '턶', '턷', '턹', '턻', '턼', '턽', '턾', '턿', '텂', '텆', '텇', '텈', '텉', '텊', '텋', '텎', '텏', '텑', '텒', '텓', '텕', '텖', '텗', '텘', '텙', '텚', '텛', '텞', '텠', '텢', '텣', '텤', '텥', '텦', '텧', '텩', '텪', '텫', '텭', '텮', '텯', '텰', '텱', '텲', '텳', '텴', '텵', '텶', '텷', '텸', '텹', '텺', '텻', '텽', '텾', '텿', '톀', '톁', '톂', '톃', '톅', '톆', '톇', '톉', '톊', '톋', '톌', '톍', '톎', '톏', '톐', '톑', '톒', '톓', '톔', '톕', '톖', '톗', '톘', '톙', '톚', '톛', '톜', '톝', '톞', '톟', '톢', '톣', '톥', '톦', '톧', '톩', '톪', '톫', '톬', '톭', '톮', '톯', '톲', '톴', '톶', '톷', '톸', '톹', '톻', '톽', '톾', '톿', '퇁', '퇂', '퇃', '퇄', '퇅', '퇆', '퇇', '퇈', '퇉', '퇊', '퇋', '퇌', '퇍', '퇎', '퇏', '퇐', '퇑', '퇒', '퇓', '퇔', '퇕', '퇖', '퇗', '퇙', '퇚', '퇛', '퇜', '퇝', '퇞', '퇟', '퇠', '퇡', '퇢', '퇣', '퇤', '퇥', '퇦', '퇧', '퇨', '퇩', '퇪', '퇫', '퇬', '퇭', '퇮', '퇯', '퇰', '퇱', '퇲', '퇳', '퇵', '퇶', '퇷', '퇹', '퇺', '퇻', '퇼', '퇽', '퇾', '퇿', '툀', '툁', '툂', '툃', '툄', '툅', '툆', '툈', '툊', '툋', '툌', '툍', '툎', '툏', '툑', '툒', '툓', '툔', '툕', '툖', '툗', '툘', '툙', '툚', '툛', '툜', '툝', '툞', '툟', '툠', '툡', '툢', '툣', '툤', '툥', '툦', '툧', '툨', '툩', '툪', '툫', '툮', '툯', '툱', '툲', '툳', '툵', '툶', '툷', '툸', '툹', '툺', '툻', '툾', '퉀', '퉂', '퉃', '퉄', '퉅', '퉆', '퉇', '퉉', '퉊', '퉋', '퉌', '퉍', '퉎', '퉏', '퉐', '퉑', '퉒', '퉓', '퉔', '퉕', '퉖', '퉗', '퉘', '퉙', '퉚', '퉛', '퉝', '퉞', '퉟', '퉠', '퉡', '퉢', '퉣', '퉥', '퉦', '퉧', '퉨', '퉩', '퉪', '퉫', '퉬', '퉭', '퉮', '퉯', '퉰', '퉱', '퉲', '퉳', '퉴', '퉵', '퉶', '퉷', '퉸', '퉹', '퉺', '퉻', '퉼', '퉽', '퉾', '퉿', '튂', '튃', '튅', '튆', '튇', '튉', '튊', '튋', '튌', '튍', '튎', '튏', '튒', '튓', '튔', '튖', '튗', '튘', '튙', '튚', '튛', '튝', '튞', '튟', '튡', '튢', '튣', '튥', '튦', '튧', '튨', '튩', '튪', '튫', '튭', '튮', '튯', '튰', '튲', '튳', '튴', '튵', '튶', '튷', '튺', '튻', '튽', '튾', '틁', '틃', '틄', '틅', '틆', '틇', '틊', '틌', '틍', '틎', '틏', '틐', '틑', '틒', '틓', '틕', '틖', '틗', '틙', '틚', '틛', '틝', '틞', '틟', '틠', '틡', '틢', '틣', '틦', '틧', '틨', '틩', '틪', '틫', '틬', '틭', '틮', '틯', '틲', '틳', '틵', '틶', '틷', '틹', '틺', '틻', '틼', '틽', '틾', '틿', '팂', '팄', '팆', '팇', '팈', '팉', '팊', '팋', '팏', '팑', '팒', '팓', '팕', '팗', '팘', '팙', '팚', '팛', '팞', '팢', '팣', '팤', '팦', '팧', '팪', '팫', '팭', '팮', '팯', '팱', '팲', '팳', '팴', '팵', '팶', '팷', '팺', '팾', '팿', '퍀', '퍁', '퍂', '퍃', '퍆', '퍇', '퍈', '퍉', '퍊', '퍋', '퍌', '퍍', '퍎', '퍏', '퍐', '퍑', '퍒', '퍓', '퍔', '퍕', '퍖', '퍗', '퍘', '퍙', '퍚', '퍛', '퍜', '퍝', '퍞', '퍟', '퍠', '퍡', '퍢', '퍣', '퍤', '퍥', '퍦', '퍧', '퍨', '퍩', '퍪', '퍫', '퍬', '퍭', '퍮', '퍯', '퍰', '퍱', '퍲', '퍳', '퍴', '퍵', '퍶', '퍷', '퍸', '퍹', '퍺', '퍻', '퍾', '퍿', '펁', '펂', '펃', '펅', '펆', '펇', '펈', '펉', '펊', '펋', '펎', '펒', '펓', '펔', '펕', '펖', '펗', '펚', '펛', '펝', '펞', '펟', '펡', '펢', '펣', '펤', '펥', '펦', '펧', '펪', '펬', '펮', '펯', '펰', '펱', '펲', '펳', '펵', '펶', '펷', '펹', '펺', '펻', '펽', '펾', '펿', '폀', '폁', '폂', '폃', '폆', '폇', '폊', '폋', '폌', '폍', '폎', '폏', '폑', '폒', '폓', '폔', '폕', '폖', '폗', '폙', '폚', '폛', '폜', '폝', '폞', '폟', '폠', '폢', '폤', '폥', '폦', '폧', '폨', '폩', '폪', '폫', '폮', '폯', '폱', '폲', '폳', '폵', '폶', '폷', '폸', '폹', '폺', '폻', '폾', '퐀', '퐂', '퐃', '퐄', '퐅', '퐆', '퐇', '퐉', '퐊', '퐋', '퐌', '퐍', '퐎', '퐏', '퐐', '퐑', '퐒', '퐓', '퐔', '퐕', '퐖', '퐗', '퐘', '퐙', '퐚', '퐛', '퐜', '퐞', '퐟', '퐠', '퐡', '퐢', '퐣', '퐤', '퐥', '퐦', '퐧', '퐨', '퐩', '퐪', '퐫', '퐬', '퐭', '퐮', '퐯', '퐰', '퐱', '퐲', '퐳', '퐴', '퐵', '퐶', '퐷', '퐸', '퐹', '퐺', '퐻', '퐼', '퐽', '퐾', '퐿', '푁', '푂', '푃', '푅', '푆', '푇', '푈', '푉', '푊', '푋', '푌', '푍', '푎', '푏', '푐', '푑', '푒', '푓', '푔', '푕', '푖', '푗', '푘', '푙', '푚', '푛', '푝', '푞', '푟', '푡', '푢', '푣', '푥', '푦', '푧', '푨', '푩', '푪', '푫', '푬', '푮', '푰', '푱', '푲', '푳', '푴', '푵', '푶', '푷', '푺', '푻', '푽', '푾', '풁', '풃', '풄', '풅', '풆', '풇', '풊', '풌', '풎', '풏', '풐', '풑', '풒', '풓', '풕', '풖', '풗', '풘', '풙', '풚', '풛', '풜', '풝', '풞', '풟', '풠', '풡', '풢', '풣', '풤', '풥', '풦', '풧', '풨', '풪', '풫', '풬', '풭', '풮', '풯', '풰', '풱', '풲', '풳', '풴', '풵', '풶', '풷', '풸', '풹', '풺', '풻', '풼', '풽', '풾', '풿', '퓀', '퓁', '퓂', '퓃', '퓄', '퓅', '퓆', '퓇', '퓈', '퓉', '퓊', '퓋', '퓍', '퓎', '퓏', '퓑', '퓒', '퓓', '퓕', '퓖', '퓗', '퓘', '퓙', '퓚', '퓛', '퓝', '퓞', '퓠', '퓡', '퓢', '퓣', '퓤', '퓥', '퓦', '퓧', '퓩', '퓪', '퓫', '퓭', '퓮', '퓯', '퓱', '퓲', '퓳', '퓴', '퓵', '퓶', '퓷', '퓹', '퓺', '퓼', '퓾', '퓿', '픀', '픁', '픂', '픃', '픅', '픆', '픇', '픉', '픊', '픋', '픍', '픎', '픏', '픐', '픑', '픒', '픓', '픖', '픘', '픙', '픚', '픛', '픜', '픝', '픞', '픟', '픠', '픡', '픢', '픣', '픤', '픥', '픦', '픧', '픨', '픩', '픪', '픫', '픬', '픭', '픮', '픯', '픰', '픱', '픲', '픳', '픴', '픵', '픶', '픷', '픸', '픹', '픺', '픻', '픾', '픿', '핁', '핂', '핃', '핅', '핆', '핇', '핈', '핉', '핊', '핋', '핎', '핐', '핒', '핓', '핔', '핕', '핖', '핗', '핚', '핛', '핝', '핞', '핟', '핡', '핢', '핣', '핤', '핦', '핧', '핪', '핬', '핮', '핯', '핰', '핱', '핲', '핳', '핶', '핷', '핹', '핺', '핻', '핽', '핾', '핿', '햀', '햁', '햂', '햃', '햆', '햊', '햋', '햌', '햍', '햎', '햏', '햑', '햒', '햓', '햔', '햕', '햖', '햗', '햘', '햙', '햚', '햛', '햜', '햝', '햞', '햟', '햠', '햡', '햢', '햣', '햤', '햦', '햧', '햨', '햩', '햪', '햫', '햬', '햭', '햮', '햯', '햰', '햱', '햲', '햳', '햴', '햵', '햶', '햷', '햸', '햹', '햺', '햻', '햼', '햽', '햾', '햿', '헀', '헁', '헂', '헃', '헄', '헅', '헆', '헇', '헊', '헋', '헍', '헎', '헏', '헑', '헓', '헔', '헕', '헖', '헗', '헚', '헜', '헞', '헟', '헠', '헡', '헢', '헣', '헦', '헧', '헩', '헪', '헫', '헭', '헮', '헯', '헰', '헱', '헲', '헳', '헶', '헸', '헺', '헻', '헼', '헽', '헾', '헿', '혂', '혃', '혅', '혆', '혇', '혉', '혊', '혋', '혌', '혍', '혎', '혏', '혒', '혖', '혗', '혘', '혙', '혚', '혛', '혝', '혞', '혟', '혡', '혢', '혣', '혥', '혦', '혧', '혨', '혩', '혪', '혫', '혬', '혮', '혯', '혰', '혱', '혲', '혳', '혴', '혵', '혶', '혷', '혺', '혻', '혽', '혾', '혿', '홁', '홂', '홃', '홄', '홆', '홇', '홊', '홌', '홎', '홏', '홐', '홒', '홓', '홖', '홗', '홙', '홚', '홛', '홝', '홞', '홟', '홠', '홡', '홢', '홣', '홤', '홥', '홦', '홨', '홪', '홫', '홬', '홭', '홮', '홯', '홲', '홳', '홵', '홶', '홷', '홸', '홹', '홺', '홻', '홼', '홽', '홾', '홿', '횀', '횁', '횂', '횄', '횆', '횇', '횈', '횉', '횊', '횋', '횎', '횏', '횑', '횒', '횓', '횕', '횖', '횗', '횘', '횙', '횚', '횛', '횜', '횞', '횠', '횢', '횣', '횤', '횥', '횦', '횧', '횩', '횪', '횫', '횭', '횮', '횯', '횱', '횲', '횳', '횴', '횵', '횶', '횷', '횸', '횺', '횼', '횽', '횾', '횿', '훀', '훁', '훂', '훃', '훆', '훇', '훉', '훊', '훋', '훍', '훎', '훏', '훐', '훒', '훓', '훕', '훖', '훘', '훚', '훛', '훜', '훝', '훞', '훟', '훡', '훢', '훣', '훥', '훦', '훧', '훩', '훪', '훫', '훬', '훭', '훮', '훯', '훱', '훲', '훳', '훴', '훶', '훷', '훸', '훹', '훺', '훻', '훾', '훿', '휁', '휂', '휃', '휅', '휆', '휇', '휈', '휉', '휊', '휋', '휌', '휍', '휎', '휏', '휐', '휒', '휓', '휔', '휕', '휖', '휗', '휚', '휛', '휝', '휞', '휟', '휡', '휢', '휣', '휤', '휥', '휦', '휧', '휪', '휬', '휮', '휯', '휰', '휱', '휲', '휳', '휶', '휷', '휹', '휺', '휻', '휽', '휾', '휿', '흀', '흁', '흂', '흃', '흅', '흆', '흈', '흊', '흋', '흌', '흍', '흎', '흏', '흒', '흓', '흕', '흚', '흛', '흜', '흝', '흞', '흟', '흢', '흤', '흦', '흧', '흨', '흪', '흫', '흭', '흮', '흯', '흱', '흲', '흳', '흵', '흶', '흷', '흸', '흹', '흺', '흻', '흾', '흿', '힀', '힂', '힃', '힄', '힅', '힆', '힇', '힊', '힋', '힍', '힎', '힏', '힑', '힒', '힓', '힔', '힕', '힖', '힗', '힚', '힜', '힞', '힟', '힠', '힡', '힢', '힣', '\ud7a4']
+['가', '각', '간', '갇', '갈', '갉', '갊', '감', '갑', '값', '갓', '갔', '강', '갖', '갗', '같', '갚', '갛', '개', '객', '갠', '갤', '갬', '갭', '갯', '갰', '갱', '갸', '갹', '갼', '걀', '걋', '걍', '걔', '걘', '걜', '거', '걱', '건', '걷', '걸', '걺', '검', '겁', '것', '겄', '겅', '겆', '겉', '겊', '겋', '게', '겐', '겔', '겜', '겝', '겟', '겠', '겡', '겨', '격', '겪', '견', '겯', '결', '겸', '겹', '겻', '겼', '경', '곁', '계', '곈', '곌', '곕', '곗', '고', '곡', '곤', '곧', '골', '곪', '곬', '곯', '곰', '곱', '곳', '공', '곶', '과', '곽', '관', '괄', '괆', '괌', '괍', '괏', '광', '괘', '괜', '괠', '괩', '괬', '괭', '괴', '괵', '괸', '괼', '굄', '굅', '굇', '굉', '교', '굔', '굘', '굡', '굣', '구', '국', '군', '굳', '굴', '굵', '굶', '굻', '굼', '굽', '굿', '궁', '궂', '궈', '궉', '권', '궐', '궜', '궝', '궤', '궷', '귀', '귁', '귄', '귈', '귐', '귑', '귓', '규', '균', '귤', '그', '극', '근', '귿', '글', '긁', '금', '급', '긋', '긍', '긔', '기', '긱', '긴', '긷', '길', '긺', '김', '깁', '깃', '깅', '깆', '깊', '까', '깍', '깎', '깐', '깔', '깖', '깜', '깝', '깟', '깠', '깡', '깥', '깨', '깩', '깬', '깰', '깸', '깹', '깻', '깼', '깽', '꺄', '꺅', '꺌', '꺼', '꺽', '꺾', '껀', '껄', '껌', '껍', '껏', '껐', '껑', '께', '껙', '껜', '껨', '껫', '껭', '껴', '껸', '껼', '꼇', '꼈', '꼍', '꼐', '꼬', '꼭', '꼰', '꼲', '꼴', '꼼', '꼽', '꼿', '꽁', '꽂', '꽃', '꽈', '꽉', '꽐', '꽜', '꽝', '꽤', '꽥', '꽹', '꾀', '꾄', '꾈', '꾐', '꾑', '꾕', '꾜', '꾸', '꾹', '꾼', '꿀', '꿇', '꿈', '꿉', '꿋', '꿍', '꿎', '꿔', '꿜', '꿨', '꿩', '꿰', '꿱', '꿴', '꿸', '뀀', '뀁', '뀄', '뀌', '뀐', '뀔', '뀜', '뀝', '뀨', '끄', '끅', '끈', '끊', '끌', '끎', '끓', '끔', '끕', '끗', '끙', '끝', '끼', '끽', '낀', '낄', '낌', '낍', '낏', '낑', '나', '낙', '낚', '난', '낟', '날', '낡', '낢', '남', '납', '낫', '났', '낭', '낮', '낯', '낱', '낳', '내', '낵', '낸', '낼', '냄', '냅', '냇', '냈', '냉', '냐', '냑', '냔', '냘', '냠', '냥', '너', '넉', '넋', '넌', '널', '넒', '넓', '넘', '넙', '넛', '넜', '넝', '넣', '네', '넥', '넨', '넬', '넴', '넵', '넷', '넸', '넹', '녀', '녁', '년', '녈', '념', '녑', '녔', '녕', '녘', '녜', '녠', '노', '녹', '논', '놀', '놂', '놈', '놉', '놋', '농', '높', '놓', '놔', '놘', '놜', '놨', '뇌', '뇐', '뇔', '뇜', '뇝', '뇟', '뇨', '뇩', '뇬', '뇰', '뇹', '뇻', '뇽', '누', '눅', '눈', '눋', '눌', '눔', '눕', '눗', '눙', '눠', '눴', '눼', '뉘', '뉜', '뉠', '뉨', '뉩', '뉴', '뉵', '뉼', '늄', '늅', '늉', '느', '늑', '는', '늘', '늙', '늚', '늠', '늡', '늣', '능', '늦', '늪', '늬', '늰', '늴', '니', '닉', '닌', '닐', '닒', '님', '닙', '닛', '닝', '닢', '다', '닥', '닦', '단', '닫', '달', '닭', '닮', '닯', '닳', '담', '답', '닷', '닸', '당', '닺', '닻', '닿', '대', '댁', '댄', '댈', '댐', '댑', '댓', '댔', '댕', '댜', '더', '덕', '덖', '던', '덛', '덜', '덞', '덟', '덤', '덥', '덧', '덩', '덫', '덮', '데', '덱', '덴', '델', '뎀', '뎁', '뎃', '뎄', '뎅', '뎌', '뎐', '뎔', '뎠', '뎡', '뎨', '뎬', '도', '독', '돈', '돋', '돌', '돎', '돐', '돔', '돕', '돗', '동', '돛', '돝', '돠', '돤', '돨', '돼', '됐', '되', '된', '될', '됨', '됩', '됫', '됴', '두', '둑', '둔', '둘', '둠', '둡', '둣', '둥', '둬', '뒀', '뒈', '뒝', '뒤', '뒨', '뒬', '뒵', '뒷', '뒹', '듀', '듄', '듈', '듐', '듕', '드', '득', '든', '듣', '들', '듦', '듬', '듭', '듯', '등', '듸', '디', '딕', '딘', '딛', '딜', '딤', '딥', '딧', '딨', '딩', '딪', '따', '딱', '딴', '딸', '땀', '땁', '땃', '땄', '땅', '땋', '때', '땍', '땐', '땔', '땜', '땝', '땟', '땠', '땡', '떠', '떡', '떤', '떨', '떪', '떫', '떰', '떱', '떳', '떴', '떵', '떻', '떼', '떽', '뗀', '뗄', '뗌', '뗍', '뗏', '뗐', '뗑', '뗘', '뗬', '또', '똑', '똔', '똘', '똥', '똬', '똴', '뙈', '뙤', '뙨', '뚜', '뚝', '뚠', '뚤', '뚫', '뚬', '뚱', '뛔', '뛰', '뛴', '뛸', '뜀', '뜁', '뜅', '뜨', '뜩', '뜬', '뜯', '뜰', '뜸', '뜹', '뜻', '띄', '띈', '띌', '띔', '띕', '띠', '띤', '띨', '띰', '띱', '띳', '띵', '라', '락', '란', '랄', '람', '랍', '랏', '랐', '랑', '랒', '랖', '랗', '래', '랙', '랜', '랠', '램', '랩', '랫', '랬', '랭', '랴', '략', '랸', '럇', '량', '러', '럭', '런', '럴', '럼', '럽', '럿', '렀', '렁', '렇', '레', '렉', '렌', '렐', '렘', '렙', '렛', '렝', '려', '력', '련', '렬', '렴', '렵', '렷', '렸', '령', '례', '롄', '롑', '롓', '로', '록', '론', '롤', '롬', '롭', '롯', '롱', '롸', '롼', '뢍', '뢨', '뢰', '뢴', '뢸', '룀', '룁', '룃', '룅', '료', '룐', '룔', '룝', '룟', '룡', '루', '룩', '룬', '룰', '룸', '룹', '룻', '룽', '뤄', '뤘', '뤠', '뤼', '뤽', '륀', '륄', '륌', '륏', '륑', '류', '륙', '륜', '률', '륨', '륩', '륫', '륭', '르', '륵', '른', '를', '름', '릅', '릇', '릉', '릊', '릍', '릎', '리', '릭', '린', '릴', '림', '립', '릿', '링', '마', '막', '만', '많', '맏', '말', '맑', '맒', '맘', '맙', '맛', '망', '맞', '맡', '맣', '매', '맥', '맨', '맬', '맴', '맵', '맷', '맸', '맹', '맺', '먀', '먁', '먈', '먕', '머', '먹', '먼', '멀', '멂', '멈', '멉', '멋', '멍', '멎', '멓', '메', '멕', '멘', '멜', '멤', '멥', '멧', '멨', '멩', '며', '멱', '면', '멸', '몃', '몄', '명', '몇', '몌', '모', '목', '몫', '몬', '몰', '몲', '몸', '몹', '못', '몽', '뫄', '뫈', '뫘', '뫙', '뫼', '묀', '묄', '묍', '묏', '묑', '묘', '묜', '묠', '묩', '묫', '무', '묵', '묶', '문', '묻', '물', '묽', '묾', '뭄', '뭅', '뭇', '뭉', '뭍', '뭏', '뭐', '뭔', '뭘', '뭡', '뭣', '뭬', '뮈', '뮌', '뮐', '뮤', '뮨', '뮬', '뮴', '뮷', '므', '믄', '믈', '믐', '믓', '미', '믹', '민', '믿', '밀', '밂', '밈', '밉', '밋', '밌', '밍', '및', '밑', '바', '박', '밖', '밗', '반', '받', '발', '밝', '밞', '밟', '밤', '밥', '밧', '방', '밭', '배', '백', '밴', '밸', '뱀', '뱁', '뱃', '뱄', '뱅', '뱉', '뱌', '뱍', '뱐', '뱝', '버', '벅', '번', '벋', '벌', '벎', '범', '법', '벗', '벙', '벚', '베', '벡', '벤', '벧', '벨', '벰', '벱', '벳', '벴', '벵', '벼', '벽', '변', '별', '볍', '볏', '볐', '병', '볕', '볘', '볜', '보', '복', '볶', '본', '볼', '봄', '봅', '봇', '봉', '봐', '봔', '봤', '봬', '뵀', '뵈', '뵉', '뵌', '뵐', '뵘', '뵙', '뵤', '뵨', '부', '북', '분', '붇', '불', '붉', '붊', '붐', '붑', '붓', '붕', '붙', '붚', '붜', '붤', '붰', '붸', '뷔', '뷕', '뷘', '뷜', '뷩', '뷰', '뷴', '뷸', '븀', '븃', '븅', '브', '븍', '븐', '블', '븜', '븝', '븟', '비', '빅', '빈', '빌', '빎', '빔', '빕', '빗', '빙', '빚', '빛', '빠', '빡', '빤', '빨', '빪', '빰', '빱', '빳', '빴', '빵', '빻', '빼', '빽', '뺀', '뺄', '뺌', '뺍', '뺏', '뺐', '뺑', '뺘', '뺙', '뺨', '뻐', '뻑', '뻔', '뻗', '뻘', '뻠', '뻣', '뻤', '뻥', '뻬', '뼁', '뼈', '뼉', '뼘', '뼙', '뼛', '뼜', '뼝', '뽀', '뽁', '뽄', '뽈', '뽐', '뽑', '뽕', '뾔', '뾰', '뿅', '뿌', '뿍', '뿐', '뿔', '뿜', '뿟', '뿡', '쀼', '쁑', '쁘', '쁜', '쁠', '쁨', '쁩', '삐', '삑', '삔', '삘', '삠', '삡', '삣', '삥', '사', '삭', '삯', '산', '삳', '살', '삵', '삶', '삼', '삽', '삿', '샀', '상', '샅', '새', '색', '샌', '샐', '샘', '샙', '샛', '샜', '생', '샤', '샥', '샨', '샬', '샴', '샵', '샷', '샹', '섀', '섄', '섈', '섐', '섕', '서', '석', '섞', '섟', '선', '섣', '설', '섦', '섧', '섬', '섭', '섯', '섰', '성', '섶', '세', '섹', '센', '셀', '셈', '셉', '셋', '셌', '셍', '셔', '셕', '션', '셜', '셤', '셥', '셧', '셨', '셩', '셰', '셴', '셸', '솅', '소', '속', '솎', '손', '솔', '솖', '솜', '솝', '솟', '송', '솥', '솨', '솩', '솬', '솰', '솽', '쇄', '쇈', '쇌', '쇔', '쇗', '쇘', '쇠', '쇤', '쇨', '쇰', '쇱', '쇳', '쇼', '쇽', '숀', '숄', '숌', '숍', '숏', '숑', '수', '숙', '순', '숟', '술', '숨', '숩', '숫', '숭', '숯', '숱', '숲', '숴', '쉈', '쉐', '쉑', '쉔', '쉘', '쉠', '쉥', '쉬', '쉭', '쉰', '쉴', '쉼', '쉽', '쉿', '슁', '슈', '슉', '슐', '슘', '슛', '슝', '스', '슥', '슨', '슬', '슭', '슴', '습', '슷', '승', '시', '식', '신', '싣', '실', '싫', '심', '십', '싯', '싱', '싶', '싸', '싹', '싻', '싼', '쌀', '쌈', '쌉', '쌌', '쌍', '쌓', '쌔', '쌕', '쌘', '쌜', '쌤', '쌥', '쌨', '쌩', '썅', '써', '썩', '썬', '썰', '썲', '썸', '썹', '썼', '썽', '쎄', '쎈', '쎌', '쏀', '쏘', '쏙', '쏜', '쏟', '쏠', '쏢', '쏨', '쏩', '쏭', '쏴', '쏵', '쏸', '쐈', '쐐', '쐤', '쐬', '쐰', '쐴', '쐼', '쐽', '쑈', '쑤', '쑥', '쑨', '쑬', '쑴', '쑵', '쑹', '쒀', '쒔', '쒜', '쒸', '쒼', '쓩', '쓰', '쓱', '쓴', '쓸', '쓺', '쓿', '씀', '씁', '씌', '씐', '씔', '씜', '씨', '씩', '씬', '씰', '씸', '씹', '씻', '씽', '아', '악', '안', '앉', '않', '알', '앍', '앎', '앓', '암', '압', '앗', '았', '앙', '앝', '앞', '애', '액', '앤', '앨', '앰', '앱', '앳', '앴', '앵', '야', '약', '얀', '얄', '얇', '얌', '얍', '얏', '양', '얕', '얗', '얘', '얜', '얠', '얩', '어', '억', '언', '얹', '얻', '얼', '얽', '얾', '엄', '업', '없', '엇', '었', '엉', '엊', '엌', '엎', '에', '엑', '엔', '엘', '엠', '엡', '엣', '엥', '여', '역', '엮', '연', '열', '엶', '엷', '염', '엽', '엾', '엿', '였', '영', '옅', '옆', '옇', '예', '옌', '옐', '옘', '옙', '옛', '옜', '오', '옥', '온', '올', '옭', '옮', '옰', '옳', '옴', '옵', '옷', '옹', '옻', '와', '왁', '완', '왈', '왐', '왑', '왓', '왔', '왕', '왜', '왝', '왠', '왬', '왯', '왱', '외', '왹', '왼', '욀', '욈', '욉', '욋', '욍', '요', '욕', '욘', '욜', '욤', '욥', '욧', '용', '우', '욱', '운', '울', '욹', '욺', '움', '웁', '웃', '웅', '워', '웍', '원', '월', '웜', '웝', '웠', '웡', '웨', '웩', '웬', '웰', '웸', '웹', '웽', '위', '윅', '윈', '윌', '윔', '윕', '윗', '윙', '유', '육', '윤', '율', '윰', '윱', '윳', '융', '윷', '으', '윽', '은', '을', '읊', '음', '읍', '읏', '응', '읒', '읓', '읔', '읕', '읖', '읗', '의', '읜', '읠', '읨', '읫', '이', '익', '인', '일', '읽', '읾', '잃', '임', '입', '잇', '있', '잉', '잊', '잎', '자', '작', '잔', '잖', '잗', '잘', '잚', '잠', '잡', '잣', '잤', '장', '잦', '재', '잭', '잰', '잴', '잼', '잽', '잿', '쟀', '쟁', '쟈', '쟉', '쟌', '쟎', '쟐', '쟘', '쟝', '쟤', '쟨', '쟬', '저', '적', '전', '절', '젊', '점', '접', '젓', '정', '젖', '제', '젝', '젠', '젤', '젬', '젭', '젯', '젱', '져', '젼', '졀', '졈', '졉', '졌', '졍', '졔', '조', '족', '존', '졸', '졺', '좀', '좁', '좃', '종', '좆', '좇', '좋', '좌', '좍', '좔', '좝', '좟', '좡', '좨', '좼', '좽', '죄', '죈', '죌', '죔', '죕', '죗', '죙', '죠', '죡', '죤', '죵', '주', '죽', '준', '줄', '줅', '줆', '줌', '줍', '줏', '중', '줘', '줬', '줴', '쥐', '쥑', '쥔', '쥘', '쥠', '쥡', '쥣', '쥬', '쥰', '쥴', '쥼', '즈', '즉', '즌', '즐', '즘', '즙', '즛', '증', '지', '직', '진', '짇', '질', '짊', '짐', '집', '짓', '징', '짖', '짙', '짚', '짜', '짝', '짠', '짢', '짤', '짧', '짬', '짭', '짯', '짰', '짱', '째', '짹', '짼', '쨀', '쨈', '쨉', '쨋', '쨌', '쨍', '쨔', '쨘', '쨩', '쩌', '쩍', '쩐', '쩔', '쩜', '쩝', '쩟', '쩠', '쩡', '쩨', '쩽', '쪄', '쪘', '쪼', '쪽', '쫀', '쫄', '쫌', '쫍', '쫏', '쫑', '쫓', '쫘', '쫙', '쫠', '쫬', '쫴', '쬈', '쬐', '쬔', '쬘', '쬠', '쬡', '쭁', '쭈', '쭉', '쭌', '쭐', '쭘', '쭙', '쭝', '쭤', '쭸', '쭹', '쮜', '쮸', '쯔', '쯤', '쯧', '쯩', '찌', '찍', '찐', '찔', '찜', '찝', '찡', '찢', '찧', '차', '착', '찬', '찮', '찰', '참', '찹', '찻', '찼', '창', '찾', '채', '책', '챈', '챌', '챔', '챕', '챗', '챘', '챙', '챠', '챤', '챦', '챨', '챰', '챵', '처', '척', '천', '철', '첨', '첩', '첫', '첬', '청', '체', '첵', '첸', '첼', '쳄', '쳅', '쳇', '쳉', '쳐', '쳔', '쳤', '쳬', '쳰', '촁', '초', '촉', '촌', '촐', '촘', '촙', '촛', '총', '촤', '촨', '촬', '촹', '최', '쵠', '쵤', '쵬', '쵭', '쵯', '쵱', '쵸', '춈', '추', '축', '춘', '출', '춤', '춥', '춧', '충', '춰', '췄', '췌', '췐', '취', '췬', '췰', '췸', '췹', '췻', '췽', '츄', '츈', '츌', '츔', '츙', '츠', '측', '츤', '츨', '츰', '츱', '츳', '층', '치', '칙', '친', '칟', '칠', '칡', '침', '칩', '칫', '칭', '카', '칵', '칸', '칼', '캄', '캅', '캇', '캉', '캐', '캑', '캔', '캘', '캠', '캡', '캣', '캤', '캥', '캬', '캭', '컁', '커', '컥', '컨', '컫', '컬', '컴', '컵', '컷', '컸', '컹', '케', '켁', '켄', '켈', '켐', '켑', '켓', '켕', '켜', '켠', '켤', '켬', '켭', '켯', '켰', '켱', '켸', '코', '콕', '콘', '콜', '콤', '콥', '콧', '콩', '콰', '콱', '콴', '콸', '쾀', '쾅', '쾌', '쾡', '쾨', '쾰', '쿄', '쿠', '쿡', '쿤', '쿨', '쿰', '쿱', '쿳', '쿵', '쿼', '퀀', '퀄', '퀑', '퀘', '퀭', '퀴', '퀵', '퀸', '퀼', '큄', '큅', '큇', '큉', '큐', '큔', '큘', '큠', '크', '큭', '큰', '클', '큼', '큽', '킁', '키', '킥', '킨', '킬', '킴', '킵', '킷', '킹', '타', '탁', '탄', '탈', '탉', '탐', '탑', '탓', '탔', '탕', '태', '택', '탠', '탤', '탬', '탭', '탯', '탰', '탱', '탸', '턍', '터', '턱', '턴', '털', '턺', '텀', '텁', '텃', '텄', '텅', '테', '텍', '텐', '텔', '템', '텝', '텟', '텡', '텨', '텬', '텼', '톄', '톈', '토', '톡', '톤', '톨', '톰', '톱', '톳', '통', '톺', '톼', '퇀', '퇘', '퇴', '퇸', '툇', '툉', '툐', '투', '툭', '툰', '툴', '툼', '툽', '툿', '퉁', '퉈', '퉜', '퉤', '튀', '튁', '튄', '튈', '튐', '튑', '튕', '튜', '튠', '튤', '튬', '튱', '트', '특', '튼', '튿', '틀', '틂', '틈', '틉', '틋', '틔', '틘', '틜', '틤', '틥', '티', '틱', '틴', '틸', '팀', '팁', '팃', '팅', '파', '팍', '팎', '판', '팔', '팖', '팜', '팝', '팟', '팠', '팡', '팥', '패', '팩', '팬', '팰', '팸', '팹', '팻', '팼', '팽', '퍄', '퍅', '퍼', '퍽', '펀', '펄', '펌', '펍', '펏', '펐', '펑', '페', '펙', '펜', '펠', '펨', '펩', '펫', '펭', '펴', '편', '펼', '폄', '폅', '폈', '평', '폐', '폘', '폡', '폣', '포', '폭', '폰', '폴', '폼', '폽', '폿', '퐁', '퐈', '퐝', '푀', '푄', '표', '푠', '푤', '푭', '푯', '푸', '푹', '푼', '푿', '풀', '풂', '품', '풉', '풋', '풍', '풔', '풩', '퓌', '퓐', '퓔', '퓜', '퓟', '퓨', '퓬', '퓰', '퓸', '퓻', '퓽', '프', '픈', '플', '픔', '픕', '픗', '피', '픽', '핀', '필', '핌', '핍', '핏', '핑', '하', '학', '한', '할', '핥', '함', '합', '핫', '항', '해', '핵', '핸', '핼', '햄', '햅', '햇', '했', '행', '햐', '향', '허', '헉', '헌', '헐', '헒', '험', '헙', '헛', '헝', '헤', '헥', '헨', '헬', '헴', '헵', '헷', '헹', '혀', '혁', '현', '혈', '혐', '협', '혓', '혔', '형', '혜', '혠', '혤', '혭', '호', '혹', '혼', '홀', '홅', '홈', '홉', '홋', '홍', '홑', '화', '확', '환', '활', '홧', '황', '홰', '홱', '홴', '횃', '횅', '회', '획', '횐', '횔', '횝', '횟', '횡', '효', '횬', '횰', '횹', '횻', '후', '훅', '훈', '훌', '훑', '훔', '훗', '훙', '훠', '훤', '훨', '훰', '훵', '훼', '훽', '휀', '휄', '휑', '휘', '휙', '휜', '휠', '휨', '휩', '휫', '휭', '휴', '휵', '휸', '휼', '흄', '흇', '흉', '흐', '흑', '흔', '흖', '흗', '흘', '흙', '흠', '흡', '흣', '흥', '흩', '희', '흰', '흴', '흼', '흽', '힁', '히', '힉', '힌', '힐', '힘', '힙', '힛', '힝']
 ```
 </details>
 
 <details>
 <summary>28. get_all_incompleted_form_hangul_chars</summary>
 
-This returns all non-completed form Hangul characters.
+This returns all incompleted form Hangul characters.
 
 Returns:
-- `List[str]`: all non-completed form Hangul characters
+- `List[str]`: all incompleted form Hangul characters
 
 Examples:
 ```python
 >>> from kss import Kss
 >>> get_all_incompleted_form_hangul_chars = Kss("get_all_incompleted_form_hangul_chars")
 >>> output = get_all_incompleted_form_hangul_chars()
 >>> print(output)
@@ -1022,17 +1031,17 @@
 Returns:
 - `Union[str, List[str]]`: normalized text or list of normalized texts
 
 Examples:
 ```python
 >>> from kss import Kss
 >>> normalize = Kss("normalize")
->>> text = "안녕\u200b하세요 ﾻﾻﾻﾻﾻﾻ   <br>오늘\u200b은 날이 참 좋네요.\\n\\n\\n200 &lt; 300 &amp; 400"
+>>> text = "안녕\u200b하세요 ﾻﾻﾻﾻﾻﾻ   <br>오늘\u200b은 날이 참 좋네요.\n\n\n200 &lt; 300 &amp; 400"
 >>> normalize(text, allow_doubled_spaces=False, allow_html_tags=False, allow_html_escape=False, allow_halfwidth_hangul=False, allow_hangul_jamo=False, allow_invisible_chars=False, reduce_char_repeats_over=2, reduce_emoticon_repeats_over=2)
-'안녕하세요 ㅋㅋ 오늘은 날이 참 좋네요.\\n200 < 300 & 400'
+'안녕하세요 ㅋㅋ 오늘은 날이 참 좋네요.\n200 < 300 & 400'
 ```
 </details>
 
 <details>
 <summary>32. preprocess</summary>
 
 This preprocesses text with various options.
@@ -1249,15 +1258,16 @@
 ```
 References:
 - This was copied from [korean-romanizer](https://github.com/osori/korean-romanizer) and modified by Kss
 </details>
 
 <details>
 <summary>38. is_unsafe</summary>
-Check if the text is unsafe or not.
+
+This checks if the text is unsafe or not.
 
 Args:
 - text (`Union[str, List[str], Tuple[str]]`): single text or list of texts
 - return_matches (`bool`): whether to return matches or not
 - num_workers (`Union[int, str]`): the number of multiprocessing workers
 
 Returns:
@@ -1389,8 +1399,8 @@
   year         = {2021},
 }
 ```
 
 ## License
 Kss project is licensed under the terms of the BSD 3-Clause "New" or "Revised" License.
 
-Copyright 2021 [Hyunwoong Ko](https://github.com/hyunwoongko) and [Sang-kil Park](https://github.com/likejazz). All Rights Reserved.
+Copyright 2021 [Hyunwoong Ko](https://github.com/hyunwoongko) and [Sang-kil Park](https://github.com/likejazz). All Rights Reserved.
```

#### html2text {}

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1 Name: kss Version: 6.0.0.dev0 Summary: A Toolkit for
+Korean sentence segmentation Home-page: https://github.com/hyunwoongko/kss
+Author: Hyunwoong Ko Author-email: kevin.brain@kakaobrain.com License: BSD 3-
+Clause "New" or "Revised" License Platform: any Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.2
+Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
+Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
+LICENSE
                ************ KKSSSS:: KKoorreeaann SSttrriinngg pprroocceessssiinngg SSuuiittee ************
   _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_I_s_s_u_e_s_]_[_T_e_s_t_s_ _o_n_ _U_b_u_n_t_u_]_[_T_e_s_t_s_ _o_n_ _M_a_c_O_S_]_[_T_e_s_t_s_ _o_n_ _W_i_n_d_o_w_s_]
 KSS is a Korean string processing suite that provides various functions for
 processing Korean strings. It is designed to be simple and easy to use, and it
 is designed to be used in various fields such as natural language processing,
 data preprocessing, and data analysis. ### What's New: - April 27, 2024
 [Released Kss 6.0 Python](https://github.com/hyunwoongko/kss/releases/tag/
@@ -52,15 +63,15 @@
 (text) ['íì¬ ëë£ ë¶ë¤ê³¼ ë¤ëìëë° ë¶ìê¸°ë ì¢ê³  ììë
 ë§ììì´ì', 'ë¤ë§, ê°ë¨ í ë¼ì ì´ ê°ë¨ ììë²ê±° ê³¨ëª©ê¸¸ë¡
 ì­ ì¬ë¼ê°ì¼ íëë° ë¤ë¤ ììë²ê±°ì ì í¹ì ëì´ê° ë»
 íëµëë¤', 'ê°ë¨ì­ ë§ì§ í ë¼ì ì ì¸ë¶ ëª¨ìµ.'] ``` ### 4.
 Multiprocessing If you input a list of strings, Kss will automatically use
 multiprocessing to process the strings in parallel. And you can set the number
 of processes to use by setting the `num_workers` parameter. If you input
-`num_workers<2`, Kss will not use multiprocessing. ```python from kss import
+`num_workers < 2`, Kss will not use multiprocessing. ```python from kss import
 Kss module = Kss("MODULE_NAME") # using all cores output = module(
 ["YOUR_INPUT_STRING1", "YOUR_INPUT_STRING2", ...], **kwargs) # using 4 cores
 output = module(["YOUR_INPUT_STRING1", "YOUR_INPUT_STRING2", ...],
 num_workers=4, **kwargs) # using 1 core (no multiprocessing) output = module(
 ["YOUR_INPUT_STRING1", "YOUR_INPUT_STRING2", ...], num_workers=1, **kwargs) ```
 ### 5. Backward Compatibility The old version of Kss used functional usage. KSS
 also supports this for backward compatibility. ```python from kss import
@@ -645,27 +656,27 @@
 'ê³±ëì'), ('ë', 'ê³±ë'), ('ì°', 'ê³±ì°'), ('ì¼ë', 'ê³ ì°ë'),
 ('ì¼ëê³ ', 'ê³ ì°ëê³ '), ('ì¼ë¨', 'ê³ ì°ë¨'), ('ì¼ë',
 'ê³ ì°ë'), ('ì¼ëë¼', 'ê³ ì°ëë¼'), ('ì¼ì´', 'ê³ ì°ì´'),
 ('ìê°', 'ê³ ì´ê°'), ('ìê°', 'ê³ ì´ê°'), ('ìê³ ', 'ê³ ì´ê³ '),
 ('ìë°', 'ê³ ì´ë°'), ('ìëì¼', 'ê³ ì´ëì¼'), ('ìì§',
 'ê³ ì´ì§'), ('ìë°ë¼ë', 'ê³ ì¸ë°ë¼ë'), ('ììê³ ',
 'ê³ ì¸ìê³ ')]} ``` References: - This was copied from [KoParadigm](https://
-github.com/Kyubyong/KoParadigm) and modified by Kss 24. anonymize Anonymize
-sensitive information in the given text. Args: - text (`Union[str, List[str],
-Tuple[str]`): single text or list of texts - phone_number_anonymization
-(`bool`): whether to anonymize phone numbers or not - rrn_anonymization
-(`bool`): whether to anonymize resident registration numbers or not -
-card_anonymization (`bool`): whether to anonymize card numbers or not -
-email_anonymization (`bool`): whether to anonymize email addresses or not -
-back_account_anonymization (`bool`): whether to anonymize bank account numbers
-or not - credit_card_anonymization (`bool`): whether to anonymize credit card
-numbers or not - zip_anonymization (`bool`): whether to anonymize zip codes or
-not - bitcoin_anonymization (`bool`): whether to anonymize bitcoin addresses or
-not - url_anonymization (`bool`): whether to anonymize URLs or not -
-ip_v6_anonymization (`bool`): whether to anonymize IPv6 addresses or not -
+github.com/Kyubyong/KoParadigm) and modified by Kss 24. anonymize This
+anonymizes sensitive information in the given text. Args: - text (`Union[str,
+List[str], Tuple[str]`): single text or list of texts -
+phone_number_anonymization (`bool`): whether to anonymize phone numbers or not
+- rrn_anonymization (`bool`): whether to anonymize resident registration
+numbers or not - card_anonymization (`bool`): whether to anonymize card numbers
+or not - email_anonymization (`bool`): whether to anonymize email addresses or
+not - back_account_anonymization (`bool`): whether to anonymize bank account
+numbers or not - credit_card_anonymization (`bool`): whether to anonymize
+credit card numbers or not - zip_anonymization (`bool`): whether to anonymize
+zip codes or not - bitcoin_anonymization (`bool`): whether to anonymize bitcoin
+addresses or not - url_anonymization (`bool`): whether to anonymize URLs or not
+- ip_v6_anonymization (`bool`): whether to anonymize IPv6 addresses or not -
 ip_v4_anonymization (`bool`): whether to anonymize IPv4 addresses or not -
 phone_number_replacement (`str`): the replacement string for phone numbers,
 default is "" - rrn_replacement (`str`): the replacement string for resident
 registration numbers, default is "" - card_replacement (`str`): the replacement
 string for card numbers, default is "" - email_replacement (`str`): the
 replacement string for email addresses, default is "" -
 back_account_replacement (`str`): the replacement string for bank account
@@ -678,24 +689,24 @@
 ip_v4_replacement (`str`): the replacement string for IPv4 addresses, default
 is "" - num_workers (`Union[int, str]`): the number of multiprocessing workers
 Returns: - `Union[str, List[str], Tuple[str]]`: anonymized text or list of
 anonymized texts Examples: ```python >>> from kss import Kss >>> anonymize =
 Kss("anonymize") >>> text = "ì  ì íë²í¸ë 010-1234-5678, ì´ë©ì¼
 ì£¼ìë kevin.brain@kakaobrain.comìëë¤." >>> output = anonymize(text)
 >>> print(output) "ì  ì íë²í¸ë , ì´ë©ì¼ ì£¼ìë ìëë¤." ```
-25. clean_news Clean news articles by removing useless headers and footers.
-Args: - text (`Union[str, List[str], Tuple[str]]`): Input text or list of
-texts. - min_sentences (`int`): Minimum number of sentences to keep. Defaults
-to 3. - header_ratio (`float`): Ratio of the number of sentences to check in
-the header. Defaults to 0.4. - footer_ratio (`float`): Ratio of the number of
-sentences to check in the footer. Defaults to 0.4. - num_workers (`Union[int,
-str]`): the number of multiprocessing workers - verbose (`bool`): whether to
-print verbose outputs or not Returns: - `Union[str, List[str]]`: Cleaned text
-or list of cleaned texts. Examples: ```python >>> from kss import Kss >>>
-clean_news = Kss("clean_news") >>> text = "[ì¬ì§]ìë²ëë, ë´ê½
+25. clean_news This cleans news articles by removing useless headers and
+footers. Args: - text (`Union[str, List[str], Tuple[str]]`): Input text or list
+of texts. - min_sentences (`int`): Minimum number of sentences to keep.
+Defaults to 3. - header_ratio (`float`): Ratio of the number of sentences to
+check in the header. Defaults to 0.4. - footer_ratio (`float`): Ratio of the
+number of sentences to check in the footer. Defaults to 0.4. - num_workers
+(`Union[int, str]`): the number of multiprocessing workers - verbose (`bool`):
+whether to print verbose outputs or not Returns: - `Union[str, List[str]]`:
+Cleaned text or list of cleaned texts. Examples: ```python >>> from kss import
+Kss >>> clean_news = Kss("clean_news") >>> text = "[ì¬ì§]ìë²ëë, ë´ê½
 í¼ì³ì§ 'í¤ë¦½ì¶ì ' ì¤í\n\n[ ë´ì¤1 ì ê³µ](ìì¸=ë´ì¤1) ì´ëì
 ê¸°ì = ìë²ëëê° ì¤ë 22ì¼ë¶í° ë´ì ìì§íë í¤ë¦½ 120ë§
 ì¡ì´ì í¨ê» 'í¤ë¦½ì¶ì 'ë¥¼ ì¤íí´ ë³¸ê²©ì ì¸ ë´ì ììì
 ìë¦°ë¤. ì§ë 1992ë êµ­ë´ ì²« í¤ë¦½ ì¶ì ë¥¼ ì° ì´í ì¬í´ë¡
 22íì§¸ë¥¼ ë§ì´í ìë²ëë 'í¤ë¦½ì¶ì 'ë ì§ëí´ ì²« ì ì
 ë³´ì´ë©° ì¢ì ë°ìì ì»ìë ì¤ê°(äºæ)ì²´í 'ìí¬ë¦¿ê°ë 'ì
 ë¦¬ë´ì¼íê³ , ì ê· íë§ ê½ê¸¸ì ì¡°ì±íë ë± ë´ê½ì íì©í
@@ -731,826 +742,237 @@
 completed form. Args: - text (`Union[str, List[str], Tuple[str]`): single text
 or list of texts - num_workers (`Union[int, str]`): the number of
 multiprocessing workers Returns: - `Union[bool, List[bool]]`: whether the given
 text is in completed form or not Examples: ```python >>> from kss import Kss
 >>> is_completed_form = Kss("is_completed_form") >>> text = "ë°±" >>> output =
 is_completed_form(text) >>> print(output) True >>> text = "ë´¯" >>> output =
 is_completed_form(text) >>> print(output) False ``` 27.
-get_all_completed_form_hangul_chars This returns all non-completed form Hangul
-characters. Returns: - `List[str]`: all non-completed form Hangul characters
+get_all_completed_form_hangul_chars This returns all completed form Hangul
+characters. Returns: - `List[str]`: all completed form Hangul characters
 Examples: ```python >>> from kss import Kss >>>
-get_all_incompleted_form_hangul_chars = Kss
-("get_all_incompleted_form_hangul_chars") >>> output =
-get_all_incompleted_form_hangul_chars() >>> print(output) ['ê°', 'ê°', 'ê°',
-'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°¡', 'ê°¢',
-'ê°£', 'ê°¥', 'ê°¦', 'ê°§', 'ê°¨', 'ê°©', 'ê°ª', 'ê°«', 'ê°®', 'ê°²', 'ê°³',
-'ê°´', 'ê°µ', 'ê°¶', 'ê°·', 'ê°º', 'ê°»', 'ê°½', 'ê°¾', 'ê°¿', 'ê±', 'ê±',
-'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
-'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
-'ê±', 'ê±', 'ê± ', 'ê±¡', 'ê±¢', 'ê±£', 'ê±¤', 'ê±¥', 'ê±¦', 'ê±§', 'ê±¨',
-'ê±©', 'ê±ª', 'ê±«', 'ê±¬', 'ê±­', 'ê±®', 'ê±¯', 'ê±²', 'ê±³', 'ê±µ', 'ê±¶',
-'ê±¹', 'ê±»', 'ê±¼', 'ê±½', 'ê±¾', 'ê±¿', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²',
-'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²',
-'ê²', 'ê²¢', 'ê²£', 'ê²¤', 'ê²¥', 'ê²¦', 'ê²§', 'ê²«', 'ê²­', 'ê²®', 'ê²±',
-'ê²²', 'ê²³', 'ê²´', 'ê²µ', 'ê²¶', 'ê²·', 'ê²º', 'ê²¾', 'ê²¿', 'ê³', 'ê³',
-'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³',
-'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³',
-'ê³', 'ê³', 'ê³¢', 'ê³£', 'ê³¥', 'ê³¦', 'ê³©', 'ê³«', 'ê³­', 'ê³®', 'ê³²',
-'ê³´', 'ê³·', 'ê³¸', 'ê³¹', 'ê³º', 'ê³»', 'ê³¾', 'ê³¿', 'ê´', 'ê´', 'ê´',
-'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´',
-'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´¡', 'ê´¢',
-'ê´£', 'ê´¤', 'ê´¥', 'ê´¦', 'ê´§', 'ê´¨', 'ê´ª', 'ê´«', 'ê´®', 'ê´¯', 'ê´°',
-'ê´±', 'ê´²', 'ê´³', 'ê´¶', 'ê´·', 'ê´¹', 'ê´º', 'ê´»', 'ê´½', 'ê´¾', 'ê´¿',
-'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ',
-'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ',
-'êµ', 'êµ', 'êµ', 'êµ ', 'êµ¢', 'êµ¤', 'êµ¥', 'êµ¦', 'êµ§', 'êµ¨', 'êµ©',
-'êµª', 'êµ«', 'êµ®', 'êµ¯', 'êµ±', 'êµ²', 'êµ·', 'êµ¸', 'êµ¹', 'êµº', 'êµ¾',
-'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶',
-'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶',
-'ê¶', 'ê¶', 'ê¶ ', 'ê¶¡', 'ê¶¢', 'ê¶£', 'ê¶¥', 'ê¶¦', 'ê¶§', 'ê¶¨', 'ê¶©',
-'ê¶ª', 'ê¶«', 'ê¶¬', 'ê¶­', 'ê¶®', 'ê¶¯', 'ê¶°', 'ê¶±', 'ê¶²', 'ê¶³', 'ê¶´',
-'ê¶µ', 'ê¶¶', 'ê¶¸', 'ê¶¹', 'ê¶º', 'ê¶»', 'ê¶¼', 'ê¶½', 'ê¶¾', 'ê¶¿', 'ê·',
-'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·',
-'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·',
-'ê·', 'ê·¡', 'ê·¢', 'ê·£', 'ê·¥', 'ê·¦', 'ê·§', 'ê·¨', 'ê·©', 'ê·ª', 'ê·«',
-'ê·¬', 'ê·­', 'ê·®', 'ê·¯', 'ê·°', 'ê·±', 'ê·²', 'ê·³', 'ê·´', 'ê·µ', 'ê·¶',
-'ê··', 'ê·º', 'ê·»', 'ê·½', 'ê·¾', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸',
-'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸',
-'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸ ', 'ê¸¡', 'ê¸¢',
-'ê¸£', 'ê¸¤', 'ê¸¥', 'ê¸¦', 'ê¸§', 'ê¸¨', 'ê¸©', 'ê¸ª', 'ê¸«', 'ê¸¬', 'ê¸­',
-'ê¸®', 'ê¸¯', 'ê¸²', 'ê¸³', 'ê¸µ', 'ê¸¶', 'ê¸¹', 'ê¸»', 'ê¸¼', 'ê¸½', 'ê¸¾',
-'ê¸¿', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹',
-'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹¢', 'ê¹£', 'ê¹¤', 'ê¹¦',
-'ê¹§', 'ê¹ª', 'ê¹«', 'ê¹­', 'ê¹®', 'ê¹¯', 'ê¹±', 'ê¹²', 'ê¹³', 'ê¹´', 'ê¹µ',
-'ê¹¶', 'ê¹·', 'ê¹º', 'ê¹¾', 'ê¹¿', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº',
-'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº',
-'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº',
-'êº', 'êº ', 'êº¡', 'êº¢', 'êº£', 'êº¤', 'êº¥', 'êº¦', 'êº§', 'êº¨', 'êº©',
-'êºª', 'êº«', 'êº¬', 'êº­', 'êº®', 'êº¯', 'êº°', 'êº±', 'êº²', 'êº³', 'êº´',
-'êºµ', 'êº¶', 'êº·', 'êº¸', 'êº¹', 'êºº', 'êº»', 'êº¿', 'ê»', 'ê»', 'ê»',
-'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»',
-'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê» ', 'ê»¡', 'ê»¢',
-'ê»£', 'ê»¤', 'ê»¥', 'ê»¦', 'ê»§', 'ê»©', 'ê»ª', 'ê»¬', 'ê»®', 'ê»¯', 'ê»°',
-'ê»±', 'ê»²', 'ê»³', 'ê»µ', 'ê»¶', 'ê»·', 'ê»¹', 'ê»º', 'ê»»', 'ê»½', 'ê»¾',
-'ê»¿', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼',
-'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼',
-'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼ ', 'ê¼¡', 'ê¼¢', 'ê¼£',
-'ê¼¤', 'ê¼¥', 'ê¼¦', 'ê¼§', 'ê¼¨', 'ê¼©', 'ê¼ª', 'ê¼«', 'ê¼®', 'ê¼¯', 'ê¼±',
-'ê¼³', 'ê¼µ', 'ê¼¶', 'ê¼·', 'ê¼¸', 'ê¼¹', 'ê¼º', 'ê¼»', 'ê¼¾', 'ê½', 'ê½',
-'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½',
-'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½',
-'ê½ ', 'ê½¡', 'ê½¢', 'ê½£', 'ê½¦', 'ê½§', 'ê½¨', 'ê½©', 'ê½ª', 'ê½«', 'ê½¬',
-'ê½­', 'ê½®', 'ê½¯', 'ê½°', 'ê½±', 'ê½²', 'ê½³', 'ê½´', 'ê½µ', 'ê½¶', 'ê½·',
-'ê½¸', 'ê½º', 'ê½»', 'ê½¼', 'ê½½', 'ê½¾', 'ê½¿', 'ê¾', 'ê¾', 'ê¾', 'ê¾',
-'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾',
-'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾ ',
-'ê¾¡', 'ê¾¢', 'ê¾£', 'ê¾¤', 'ê¾¥', 'ê¾¦', 'ê¾§', 'ê¾¨', 'ê¾©', 'ê¾ª', 'ê¾«',
-'ê¾¬', 'ê¾­', 'ê¾®', 'ê¾¯', 'ê¾°', 'ê¾±', 'ê¾²', 'ê¾³', 'ê¾´', 'ê¾µ', 'ê¾¶',
-'ê¾·', 'ê¾º', 'ê¾»', 'ê¾½', 'ê¾¾', 'ê¾¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿',
-'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿',
-'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿ ', 'ê¿¡', 'ê¿¢', 'ê¿£',
-'ê¿¤', 'ê¿¥', 'ê¿¦', 'ê¿§', 'ê¿ª', 'ê¿«', 'ê¿¬', 'ê¿­', 'ê¿®', 'ê¿¯', 'ê¿²',
-'ê¿³', 'ê¿µ', 'ê¿¶', 'ê¿·', 'ê¿¹', 'ê¿º', 'ê¿»', 'ê¿¼', 'ê¿½', 'ê¿¾', 'ê¿¿',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë©',
-'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´',
-'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡',
-'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬',
-'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·',
-'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª',
-'ë°', 'ë²', 'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬',
-'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·',
-'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë¦', 'ë§',
-'ë©', 'ëª', 'ë«', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë¶',
-'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥',
-'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°',
-'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ëº', 'ë»', 'ë½', 'ë¾',
-'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ëª', 'ë«',
-'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶',
-'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª',
-'ë«', 'ë­', 'ë®', 'ë¯', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·',
-'ë¸', 'ëº', 'ë¼', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥',
-'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°',
-'ë±', 'ë²', 'ë³', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë½',
-'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë¡',
-'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®',
-'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»',
-'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë¢', 'ë¤', 'ë§', 'ë¨', 'ë©', 'ë«', 'ë­',
-'ë®', 'ë¯', 'ë±', 'ë²', 'ë³', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº',
-'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë£', 'ë§', 'ë©',
-'ëª', 'ë°', 'ë±', 'ë²', 'ë¶', 'ë¼', 'ë½', 'ë¾', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢',
-'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­',
-'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸',
-'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡',
-'ë¢', 'ë£', 'ë¦', 'ë¨', 'ëª', 'ë¬', 'ë­', 'ë¯', 'ë²', 'ë³', 'ëµ',
-'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ëª', 'ë«', 'ë­', 'ë®',
-'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹',
-'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ëª',
-'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ',
-'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦',
-'ë§', 'ëª', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ëµ',
-'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë¢', 'ë¤', 'ë¦', 'ë§', 'ë¨', 'ë©',
-'ëª', 'ë«', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ',
-'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¥',
-'ë¦', 'ë§', 'ë©', 'ëª', 'ë«', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²',
-'ë³', 'ë´', 'ë¶', 'ë¸', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë¡', 'ë¢', 'ë¥', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë®',
-'ë°', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼',
-'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢',
-'ë£', 'ë¦', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë²', 'ë³', 'ëµ', 'ë¶',
-'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§',
-'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²',
-'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½',
-'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë¢', 'ë£', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ë¬', 'ë­', 'ë®', 'ë¯',
-'ë²', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë¾', 'ë¿', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ',
-'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«',
-'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·',
-'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¦', 'ë§', 'ë¨',
-'ë©', 'ëª', 'ë«', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ëµ',
-'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢',
-'ë£', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯',
-'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº',
-'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª',
-'ë­', 'ë®', 'ë¯', 'ë°', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸',
-'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥',
-'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë±',
-'ë²', 'ë³', 'ëµ', 'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾',
-'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢',
-'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª', 'ë«', 'ë­', 'ë®', 'ë±', 'ë²',
-'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ëº', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¥', 'ë¦', 'ë§', 'ë©',
-'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë²', 'ë´', 'ë¶', 'ë·', 'ë¸',
-'ë¹', 'ëº', 'ë»', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª', 'ë®',
-'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼',
-'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª',
-'ë«', 'ë®', 'ë¯', 'ë±', 'ë²', 'ë³', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹',
-'ëº', 'ë»', 'ë¾', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ',
-'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ',
-'ë ', 'ë ', 'ë  ', 'ë ¡', 'ë ¢', 'ë £', 'ë ¦', 'ë §', 'ë ©', 'ë ª', 'ë «',
-'ë ­', 'ë ®', 'ë ¯', 'ë °', 'ë ±', 'ë ²', 'ë ³', 'ë ¶', 'ë º', 'ë »', 'ë ¼',
-'ë ½', 'ë ¾', 'ë ¿', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡',
-'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡',
-'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡¡', 'ë¡¢', 'ë¡£', 'ë¡¥',
-'ë¡¦', 'ë¡§', 'ë¡¨', 'ë¡©', 'ë¡ª', 'ë¡«', 'ë¡®', 'ë¡°', 'ë¡²', 'ë¡³', 'ë¡´',
-'ë¡µ', 'ë¡¶', 'ë¡·', 'ë¡¹', 'ë¡º', 'ë¡»', 'ë¡½', 'ë¡¾', 'ë¡¿', 'ë¢', 'ë¢',
-'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢',
-'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢',
-'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢ ', 'ë¢¡', 'ë¢¢', 'ë¢£',
-'ë¢¤', 'ë¢¥', 'ë¢¦', 'ë¢§', 'ë¢©', 'ë¢ª', 'ë¢«', 'ë¢¬', 'ë¢­', 'ë¢®', 'ë¢¯',
-'ë¢±', 'ë¢²', 'ë¢³', 'ë¢µ', 'ë¢¶', 'ë¢·', 'ë¢¹', 'ë¢º', 'ë¢»', 'ë¢¼', 'ë¢½',
-'ë¢¾', 'ë¢¿', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£',
-'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£',
-'ë£', 'ë£', 'ë£', 'ë£ ', 'ë£¢', 'ë££', 'ë£¤', 'ë£¥', 'ë£¦', 'ë£§', 'ë£ª',
-'ë£«', 'ë£­', 'ë£®', 'ë£¯', 'ë£±', 'ë£²', 'ë£³', 'ë£´', 'ë£µ', 'ë£¶', 'ë£·',
-'ë£º', 'ë£¼', 'ë£¾', 'ë£¿', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤',
-'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤',
-'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤',
-'ë¤', 'ë¤¡', 'ë¤¢', 'ë¤£', 'ë¤¤', 'ë¤¥', 'ë¤¦', 'ë¤§', 'ë¤¨', 'ë¤©', 'ë¤ª',
-'ë¤«', 'ë¤¬', 'ë¤­', 'ë¤®', 'ë¤¯', 'ë¤°', 'ë¤±', 'ë¤²', 'ë¤³', 'ë¤´', 'ë¤µ',
-'ë¤¶', 'ë¤·', 'ë¤¸', 'ë¤¹', 'ë¤º', 'ë¤»', 'ë¤¾', 'ë¤¿', 'ë¥', 'ë¥', 'ë¥',
-'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥',
-'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥¡',
-'ë¥¢', 'ë¥£', 'ë¥¤', 'ë¥¥', 'ë¥¦', 'ë¥§', 'ë¥ª', 'ë¥¬', 'ë¥®', 'ë¥¯', 'ë¥°',
-'ë¥±', 'ë¥²', 'ë¥³', 'ë¥¶', 'ë¥·', 'ë¥¹', 'ë¥º', 'ë¥»', 'ë¥½', 'ë¥¾', 'ë¥¿',
-'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦',
-'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦',
-'ë¦', 'ë¦', 'ë¦', 'ë¦ ', 'ë¦¡', 'ë¦¢', 'ë¦£', 'ë¦¤', 'ë¦¥', 'ë¦¦', 'ë¦§',
-'ë¦¨', 'ë¦©', 'ë¦ª', 'ë¦«', 'ë¦®', 'ë¦¯', 'ë¦±', 'ë¦²', 'ë¦³', 'ë¦µ', 'ë¦¶',
-'ë¦·', 'ë¦¸', 'ë¦¹', 'ë¦º', 'ë¦»', 'ë¦¾', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§',
-'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§',
-'ë§', 'ë§', 'ë§ ', 'ë§¢', 'ë§¦', 'ë§§', 'ë§©', 'ë§ª', 'ë§«', 'ë§­', 'ë§®',
-'ë§¯', 'ë§°', 'ë§±', 'ë§²', 'ë§³', 'ë§¶', 'ë§»', 'ë§¼', 'ë§½', 'ë§¾', 'ë§¿',
-'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨',
-'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨',
-'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨ ', 'ë¨¡', 'ë¨¢', 'ë¨£', 'ë¨¤',
-'ë¨¥', 'ë¨¦', 'ë¨§', 'ë¨¨', 'ë¨©', 'ë¨ª', 'ë¨«', 'ë¨¬', 'ë¨­', 'ë¨®', 'ë¨¯',
-'ë¨°', 'ë¨±', 'ë¨²', 'ë¨³', 'ë¨´', 'ë¨µ', 'ë¨¶', 'ë¨·', 'ë¨º', 'ë¨»', 'ë¨½',
-'ë¨¾', 'ë¨¿', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©',
-'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©',
-'ë© ', 'ë©¡', 'ë©¢', 'ë©£', 'ë©¦', 'ë©ª', 'ë©«', 'ë©¬', 'ë©­', 'ë©®', 'ë©¯',
-'ë©²', 'ë©³', 'ë©µ', 'ë©¶', 'ë©·', 'ë©¹', 'ë©º', 'ë©»', 'ë©¼', 'ë©½', 'ë©¾',
-'ë©¿', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª',
-'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª',
-'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª ', 'ëª¡', 'ëª¢', 'ëª£', 'ëª¤',
-'ëª¥', 'ëª¦', 'ëª§', 'ëªª', 'ëª­', 'ëª®', 'ëª¯', 'ëª±', 'ëª³', 'ëª´', 'ëªµ',
-'ëª¶', 'ëª·', 'ëªº', 'ëª¼', 'ëª¾', 'ëª¿', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«',
-'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«',
-'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«',
-'ë«', 'ë« ', 'ë«¡', 'ë«¢', 'ë«£', 'ë«¤', 'ë«¥', 'ë«¦', 'ë«§', 'ë«¨', 'ë«©',
-'ë«ª', 'ë««', 'ë«¬', 'ë«­', 'ë«®', 'ë«¯', 'ë«°', 'ë«±', 'ë«²', 'ë«³', 'ë«´',
-'ë«µ', 'ë«¶', 'ë«·', 'ë«¸', 'ë«¹', 'ë«º', 'ë«»', 'ë«½', 'ë«¾', 'ë«¿', 'ë¬',
-'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬',
-'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬',
-'ë¬', 'ë¬', 'ë¬¡', 'ë¬¢', 'ë¬£', 'ë¬¤', 'ë¬¥', 'ë¬¦', 'ë¬§', 'ë¬¨', 'ë¬ª',
-'ë¬¬', 'ë¬­', 'ë¬®', 'ë¬¯', 'ë¬°', 'ë¬±', 'ë¬²', 'ë¬³', 'ë¬·', 'ë¬¹', 'ë¬º',
-'ë¬¿', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­',
-'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­',
-'ë­', 'ë­', 'ë­ ', 'ë­¢', 'ë­¤', 'ë­¥', 'ë­¦', 'ë­§', 'ë­¨', 'ë­©', 'ë­ª',
-'ë­«', 'ë­­', 'ë­®', 'ë­¯', 'ë­°', 'ë­±', 'ë­²', 'ë­³', 'ë­´', 'ë­µ', 'ë­¶',
-'ë­·', 'ë­¸', 'ë­¹', 'ë­º', 'ë­»', 'ë­¼', 'ë­½', 'ë­¾', 'ë­¿', 'ë®', 'ë®',
-'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®',
-'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®',
-'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë® ', 'ë®¡', 'ë®¢', 'ë®£', 'ë®¥', 'ë®¦',
-'ë®§', 'ë®©', 'ë®ª', 'ë®«', 'ë®­', 'ë®®', 'ë®¯', 'ë®°', 'ë®±', 'ë®²', 'ë®³',
-'ë®µ', 'ë®¶', 'ë®¸', 'ë®¹', 'ë®º', 'ë®»', 'ë®¼', 'ë®½', 'ë®¾', 'ë®¿', 'ë¯',
-'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯',
-'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯',
-'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯ ', 'ë¯¡', 'ë¯¢', 'ë¯£', 'ë¯¤', 'ë¯¥', 'ë¯¦',
-'ë¯§', 'ë¯¨', 'ë¯©', 'ë¯ª', 'ë¯«', 'ë¯¬', 'ë¯­', 'ë¯®', 'ë¯¯', 'ë¯°', 'ë¯±',
-'ë¯²', 'ë¯³', 'ë¯´', 'ë¯µ', 'ë¯¶', 'ë¯·', 'ë¯º', 'ë¯»', 'ë¯½', 'ë¯¾', 'ë°',
-'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°',
-'ë°', 'ë° ', 'ë°¡', 'ë°¢', 'ë°£', 'ë°¦', 'ë°¨', 'ë°ª', 'ë°«', 'ë°¬', 'ë°®',
-'ë°¯', 'ë°²', 'ë°³', 'ë°µ', 'ë°¶', 'ë°·', 'ë°¹', 'ë°º', 'ë°»', 'ë°¼', 'ë°½',
-'ë°¾', 'ë°¿', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±',
-'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±',
-'ë±', 'ë±', 'ë± ', 'ë±¡', 'ë±¢', 'ë±£', 'ë±¤', 'ë±¥', 'ë±¦', 'ë±§', 'ë±¨',
-'ë±©', 'ë±ª', 'ë±«', 'ë±¬', 'ë±­', 'ë±®', 'ë±¯', 'ë±°', 'ë±±', 'ë±²', 'ë±³',
-'ë±´', 'ë±µ', 'ë±¶', 'ë±·', 'ë±¸', 'ë±¹', 'ë±º', 'ë±»', 'ë±¼', 'ë±½', 'ë±¾',
-'ë±¿', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²',
-'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²',
-'ë²¢', 'ë²£', 'ë²¥', 'ë²¦', 'ë²©', 'ë²ª', 'ë²«', 'ë²¬', 'ë²­', 'ë²®', 'ë²¯',
-'ë²²', 'ë²¶', 'ë²·', 'ë²¸', 'ë²¹', 'ë²º', 'ë²»', 'ë²¾', 'ë²¿', 'ë³', 'ë³',
-'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³',
-'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³ ',
-'ë³¡', 'ë³¢', 'ë³£', 'ë³¤', 'ë³¥', 'ë³¦', 'ë³§', 'ë³¨', 'ë³©', 'ë³ª', 'ë³«',
-'ë³¬', 'ë³­', 'ë³®', 'ë³¯', 'ë³°', 'ë³±', 'ë³²', 'ë³³', 'ë³·', 'ë³¹', 'ë³º',
-'ë³»', 'ë³½', 'ë³¾', 'ë³¿', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´',
-'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´',
-'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´ ', 'ë´¡', 'ë´¢',
-'ë´£', 'ë´¥', 'ë´¦', 'ë´§', 'ë´¨', 'ë´©', 'ë´ª', 'ë´«', 'ë´­', 'ë´®', 'ë´¯',
-'ë´°', 'ë´±', 'ë´²', 'ë´³', 'ë´´', 'ë´µ', 'ë´¶', 'ë´·', 'ë´¸', 'ë´¹', 'ë´º',
-'ë´»', 'ë´¼', 'ë´½', 'ë´¾', 'ë´¿', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ',
-'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ',
-'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ ', 'ëµ¡', 'ëµ¢',
-'ëµ£', 'ëµ¥', 'ëµ¦', 'ëµ§', 'ëµ©', 'ëµª', 'ëµ«', 'ëµ¬', 'ëµ­', 'ëµ®', 'ëµ¯',
-'ëµ°', 'ëµ±', 'ëµ²', 'ëµ³', 'ëµ´', 'ëµµ', 'ëµ¶', 'ëµ·', 'ëµ¸', 'ëµ¹', 'ëµº',
-'ëµ»', 'ëµ¼', 'ëµ½', 'ëµ¾', 'ëµ¿', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶',
-'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶',
-'ë¶', 'ë¶ ', 'ë¶¡', 'ë¶¢', 'ë¶£', 'ë¶¥', 'ë¶¦', 'ë¶§', 'ë¶¨', 'ë¶©', 'ë¶ª',
-'ë¶«', 'ë¶¬', 'ë¶­', 'ë¶®', 'ë¶¯', 'ë¶±', 'ë¶²', 'ë¶³', 'ë¶´', 'ë¶µ', 'ë¶¶',
-'ë¶·', 'ë¶¹', 'ë¶º', 'ë¶»', 'ë¶¼', 'ë¶½', 'ë¶¾', 'ë¶¿', 'ë·', 'ë·', 'ë·',
-'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·',
-'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·',
-'ë·', 'ë·', 'ë·', 'ë· ', 'ë·¡', 'ë·¢', 'ë·£', 'ë·¤', 'ë·¥', 'ë·¦', 'ë·§',
-'ë·¨', 'ë·ª', 'ë·«', 'ë·¬', 'ë·­', 'ë·®', 'ë·¯', 'ë·±', 'ë·²', 'ë·³', 'ë·µ',
-'ë·¶', 'ë··', 'ë·¹', 'ë·º', 'ë·»', 'ë·¼', 'ë·½', 'ë·¾', 'ë·¿', 'ë¸', 'ë¸',
-'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸',
-'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸ ', 'ë¸¡',
-'ë¸¢', 'ë¸£', 'ë¸¤', 'ë¸¥', 'ë¸¦', 'ë¸§', 'ë¸¨', 'ë¸©', 'ë¸ª', 'ë¸«', 'ë¸¬',
-'ë¸­', 'ë¸®', 'ë¸¯', 'ë¸°', 'ë¸±', 'ë¸²', 'ë¸³', 'ë¸´', 'ë¸µ', 'ë¸¶', 'ë¸·',
-'ë¸¸', 'ë¸¹', 'ë¸º', 'ë¸»', 'ë¸¼', 'ë¸½', 'ë¸¾', 'ë¸¿', 'ë¹', 'ë¹', 'ë¹',
-'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹',
-'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹¢', 'ë¹£', 'ë¹¥', 'ë¹¦',
-'ë¹§', 'ë¹©', 'ë¹«', 'ë¹¬', 'ë¹­', 'ë¹®', 'ë¹¯', 'ë¹²', 'ë¹¶', 'ë¹·', 'ë¹¸',
-'ë¹¹', 'ë¹º', 'ë¹¾', 'ë¹¿', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº',
-'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº',
-'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº ', 'ëº¡', 'ëº¢', 'ëº£', 'ëº¤', 'ëº¥',
-'ëº¦', 'ëº§', 'ëº©', 'ëºª', 'ëº«', 'ëº¬', 'ëº­', 'ëº®', 'ëº¯', 'ëº°', 'ëº±',
-'ëº²', 'ëº³', 'ëº´', 'ëºµ', 'ëº¶', 'ëº·', 'ëº¸', 'ëº¹', 'ëºº', 'ëº»', 'ëº¼',
-'ëº½', 'ëº¾', 'ëº¿', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»',
-'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»',
-'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»¡', 'ë»¢', 'ë»¦',
-'ë»§', 'ë»¨', 'ë»©', 'ë»ª', 'ë»«', 'ë»­', 'ë»®', 'ë»¯', 'ë»°', 'ë»±', 'ë»²',
-'ë»³', 'ë»´', 'ë»µ', 'ë»¶', 'ë»·', 'ë»¸', 'ë»¹', 'ë»º', 'ë»»', 'ë»¼', 'ë»½',
-'ë»¾', 'ë»¿', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼',
-'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼',
-'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼ ', 'ë¼¡', 'ë¼¢', 'ë¼£', 'ë¼¤', 'ë¼¥', 'ë¼¦',
-'ë¼§', 'ë¼¨', 'ë¼©', 'ë¼ª', 'ë¼«', 'ë¼¬', 'ë¼­', 'ë¼®', 'ë¼¯', 'ë¼°', 'ë¼±',
-'ë¼²', 'ë¼³', 'ë¼´', 'ë¼µ', 'ë¼¶', 'ë¼·', 'ë¼¸', 'ë¼¹', 'ë¼º', 'ë¼»', 'ë¼¼',
-'ë¼½', 'ë¼¾', 'ë¼¿', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½',
-'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½',
-'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½ ', 'ë½¡', 'ë½¢', 'ë½£', 'ë½¤',
-'ë½¥', 'ë½¦', 'ë½§', 'ë½¨', 'ë½©', 'ë½ª', 'ë½«', 'ë½¬', 'ë½­', 'ë½®', 'ë½¯',
-'ë½°', 'ë½±', 'ë½²', 'ë½³', 'ë½´', 'ë½µ', 'ë½¶', 'ë½·', 'ë½¸', 'ë½¹', 'ë½º',
-'ë½»', 'ë½¼', 'ë½½', 'ë½¾', 'ë½¿', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾',
-'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾',
-'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾',
-'ë¾', 'ë¾', 'ë¾', 'ë¾ ', 'ë¾¡', 'ë¾¢', 'ë¾£', 'ë¾¤', 'ë¾¥', 'ë¾¦', 'ë¾§',
-'ë¾¨', 'ë¾©', 'ë¾ª', 'ë¾«', 'ë¾¬', 'ë¾­', 'ë¾®', 'ë¾¯', 'ë¾±', 'ë¾²', 'ë¾³',
-'ë¾´', 'ë¾µ', 'ë¾¶', 'ë¾·', 'ë¾¸', 'ë¾¹', 'ë¾º', 'ë¾»', 'ë¾¼', 'ë¾½', 'ë¾¾',
-'ë¾¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿',
-'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿',
-'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿ ', 'ë¿¢', 'ë¿£', 'ë¿¤', 'ë¿¥', 'ë¿¦', 'ë¿§',
-'ë¿¨', 'ë¿©', 'ë¿ª', 'ë¿«', 'ë¿¬', 'ë¿­', 'ë¿®', 'ë¿¯', 'ë¿°', 'ë¿±', 'ë¿²',
-'ë¿³', 'ë¿´', 'ë¿µ', 'ë¿¶', 'ë¿·', 'ë¿¸', 'ë¿¹', 'ë¿º', 'ë¿»', 'ë¿¼', 'ë¿½',
-'ë¿¾', 'ë¿¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ì¨', 'ì©',
-'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì´',
-'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì½', 'ì¾', 'ì¿', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥',
-'ì¦', 'ì§', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²',
-'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½',
-'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¢', 'ì¤', 'ì¦',
-'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì®', 'ì±', 'ì²', 'ì·', 'ì¸', 'ì¹',
-'ìº', 'ì»', 'ì¾', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì­',
-'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì¶', 'ì¸', 'ìº', 'ì»', 'ì¼',
-'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì¥', 'ì¨', 'ì©', 'ìª', 'ì«',
-'ì®', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì·', 'ìº', 'ì»', 'ì½', 'ì¾', 'ì¿',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¦', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯',
-'ì±', 'ì²', 'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½',
-'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì ', 'ì¢', 'ì£', 'ì¤', 'ì¦', 'ì§', 'ìª', 'ì«', 'ì­',
-'ì®', 'ì¯', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹',
-'ìº', 'ì»', 'ì¼', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢',
-'ì£', 'ì¥', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯',
-'ì²', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì¿',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ìª', 'ì¬', 'ì®', 'ì°',
-'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾',
-'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¦',
-'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì®', 'ì¯', 'ì±', 'ì²', 'ì³', 'ìµ',
-'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ',
-'ì¡', 'ì¢', 'ì£', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì®', 'ì¯', 'ì°',
-'ì±', 'ì²', 'ì³', 'ì¶', 'ì¸', 'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì¥',
-'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì®', 'ì°', 'ì²', 'ì³', 'ì´', 'ìµ',
-'ì·', 'ìº', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¦', 'ì§',
-'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì´',
-'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡',
-'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ìª', 'ì«', 'ì­', 'ì®', 'ì¯',
-'ì±', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ìº', 'ì»', 'ì¾', 'ì¿', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¤',
-'ì¥', 'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯',
-'ì°', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº',
-'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡',
-'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ìª', 'ì«', 'ì¬', 'ì®', 'ì¯', 'ì°',
-'ì±', 'ì²', 'ì³', 'ì¶', 'ì·', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾',
-'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡',
-'ì¢', 'ì£', 'ì¥', 'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì­', 'ì®',
-'ì¯', 'ì±', 'ì²', 'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»',
-'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì­', 'ì®',
-'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì¶', 'ì·', 'ì¸', 'ìº', 'ì»', 'ì¼',
-'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ',
-'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì«',
-'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶',
-'ì·', 'ì¹', 'ìº', 'ì»', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¤',
-'ì¥', 'ì¦', 'ì§', 'ì¨', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì²',
-'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¹', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ìª',
-'ì«', 'ì­', 'ì®', 'ì¯', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·',
-'ìº', 'ì¼', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¢', 'ì£',
-'ì¥', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì²',
-'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì¿', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤',
-'ì¥', 'ì¦', 'ì§', 'ì¨', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°',
-'ì±', 'ì²', 'ì³', 'ì¶', 'ì·', 'ìº', 'ì¿', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì¢', 'ì¤', 'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª',
-'ì«', 'ì¯', 'ì±', 'ì²', 'ì³', 'ìµ', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢',
-'ì£', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì¯', 'ì±', 'ì²', 'ì¶', 'ì¸',
-'ìº', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§',
-'ì¨', 'ì©', 'ìª', 'ì«', 'ì­', 'ì®', 'ì°', 'ì²', 'ì³', 'ì´', 'ìµ',
-'ì¶', 'ì·', 'ìº', 'ì»', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢',
-'ì£', 'ì¦', 'ì¨', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì²', 'ì³',
-'ìµ', 'ì¶', 'ì·', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¢', 'ì£', 'ì¤',
-'ì¥', 'ì¦', 'ì§', 'ìª', 'ì«', 'ì­', 'ì®', 'ì¯', 'ì±', 'ì²', 'ì³',
-'ì´', 'ìµ', 'ì¶', 'ì·', 'ìº', 'ì»', 'ì¼', 'ì¾', 'ì¿', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì¢', 'ì£', 'ì¥', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®',
-'ì¯', 'ì²', 'ì´', 'ì¶', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì¿', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦',
-'ì§', 'ì©', 'ìª', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³',
-'ì¶', 'ì·', 'ì¹', 'ìº', 'ì»', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì¢', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì®', 'ì¯', 'ì±', 'ì²',
-'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ',
-'ì¡', 'ì¢', 'ì£', 'ì¥', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì­', 'ì®',
-'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹',
-'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ',
-'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ',
-'ì ', 'ì ', 'ì ', 'ì ', 'ì ¡', 'ì ¢', 'ì £', 'ì ¥', 'ì ¦', 'ì §', 'ì ¨',
-'ì ©', 'ì ª', 'ì «', 'ì ®', 'ì °', 'ì ²', 'ì ³', 'ì ´', 'ì µ', 'ì ¶', 'ì ·',
-'ì ¹', 'ì º', 'ì »', 'ì ½', 'ì ¾', 'ì ¿', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡',
-'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡',
-'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡ ',
-'ì¡¡', 'ì¡¢', 'ì¡£', 'ì¡¤', 'ì¡¥', 'ì¡¦', 'ì¡§', 'ì¡¨', 'ì¡©', 'ì¡ª', 'ì¡«',
-'ì¡¬', 'ì¡­', 'ì¡®', 'ì¡¯', 'ì¡²', 'ì¡³', 'ì¡µ', 'ì¡¶', 'ì¡·', 'ì¡¹', 'ì¡»',
-'ì¡¼', 'ì¡½', 'ì¡¾', 'ì¡¿', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢',
-'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢',
-'ì¢', 'ì¢', 'ì¢ ', 'ì¢¢', 'ì¢£', 'ì¢¤', 'ì¢¥', 'ì¢¦', 'ì¢§', 'ì¢©', 'ì¢ª',
-'ì¢«', 'ì¢¬', 'ì¢­', 'ì¢®', 'ì¢¯', 'ì¢°', 'ì¢±', 'ì¢²', 'ì¢³', 'ì¢´', 'ì¢µ',
-'ì¢¶', 'ì¢·', 'ì¢¸', 'ì¢¹', 'ì¢º', 'ì¢»', 'ì¢¾', 'ì¢¿', 'ì£', 'ì£', 'ì£',
-'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£',
-'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£',
-'ì£¢', 'ì££', 'ì£¥', 'ì£¦', 'ì£§', 'ì£¨', 'ì£©', 'ì£ª', 'ì£«', 'ì£¬', 'ì£­',
-'ì£®', 'ì£¯', 'ì£°', 'ì£±', 'ì£²', 'ì£³', 'ì£´', 'ì£¶', 'ì£·', 'ì£¸', 'ì£¹',
-'ì£º', 'ì£»', 'ì£¾', 'ì£¿', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤',
-'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤',
-'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤ ', 'ì¤¡', 'ì¤¢', 'ì¤£', 'ì¤¤', 'ì¤¥',
-'ì¤¦', 'ì¤§', 'ì¤¨', 'ì¤©', 'ì¤ª', 'ì¤«', 'ì¤­', 'ì¤®', 'ì¤¯', 'ì¤°', 'ì¤±',
-'ì¤²', 'ì¤³', 'ì¤µ', 'ì¤¶', 'ì¤·', 'ì¤¸', 'ì¤¹', 'ì¤º', 'ì¤»', 'ì¤¼', 'ì¤½',
-'ì¤¾', 'ì¤¿', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥',
-'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥',
-'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥¢', 'ì¥¤', 'ì¥¥',
-'ì¥¦', 'ì¥§', 'ì¥¨', 'ì¥©', 'ì¥ª', 'ì¥«', 'ì¥­', 'ì¥®', 'ì¥¯', 'ì¥±', 'ì¥²',
-'ì¥³', 'ì¥µ', 'ì¥¶', 'ì¥·', 'ì¥¸', 'ì¥¹', 'ì¥º', 'ì¥»', 'ì¥½', 'ì¥¾', 'ì¥¿',
-'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦',
-'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦',
-'ì¦', 'ì¦', 'ì¦ ', 'ì¦¡', 'ì¦¢', 'ì¦£', 'ì¦¤', 'ì¦¥', 'ì¦¦', 'ì¦§', 'ì¦¨',
-'ì¦©', 'ì¦ª', 'ì¦«', 'ì¦¬', 'ì¦­', 'ì¦®', 'ì¦¯', 'ì¦°', 'ì¦±', 'ì¦²', 'ì¦³',
-'ì¦´', 'ì¦µ', 'ì¦¶', 'ì¦·', 'ì¦¸', 'ì¦¹', 'ì¦º', 'ì¦»', 'ì¦¼', 'ì¦½', 'ì¦¾',
-'ì¦¿', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§',
-'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§¡', 'ì§£', 'ì§¥', 'ì§¦',
-'ì§¨', 'ì§©', 'ì§ª', 'ì§«', 'ì§®', 'ì§²', 'ì§³', 'ì§´', 'ì§µ', 'ì§¶', 'ì§·',
-'ì§º', 'ì§»', 'ì§½', 'ì§¾', 'ì§¿', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨',
-'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨',
-'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨ ', 'ì¨¡', 'ì¨¢', 'ì¨£',
-'ì¨¤', 'ì¨¥', 'ì¨¦', 'ì¨§', 'ì¨¨', 'ì¨ª', 'ì¨«', 'ì¨¬', 'ì¨­', 'ì¨®', 'ì¨¯',
-'ì¨°', 'ì¨±', 'ì¨²', 'ì¨³', 'ì¨´', 'ì¨µ', 'ì¨¶', 'ì¨·', 'ì¨¸', 'ì¨¹', 'ì¨º',
-'ì¨»', 'ì¨¼', 'ì¨½', 'ì¨¾', 'ì¨¿', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©',
-'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©',
-'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©¢', 'ì©£', 'ì©¤',
-'ì©¥', 'ì©¦', 'ì©§', 'ì©©', 'ì©ª', 'ì©«', 'ì©¬', 'ì©­', 'ì©®', 'ì©¯', 'ì©°',
-'ì©±', 'ì©²', 'ì©³', 'ì©´', 'ì©µ', 'ì©¶', 'ì©·', 'ì©¸', 'ì©¹', 'ì©º', 'ì©»',
-'ì©¼', 'ì©¾', 'ì©¿', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª',
-'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª',
-'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª',
-'ìª ', 'ìª¡', 'ìª¢', 'ìª£', 'ìª¤', 'ìª¥', 'ìª¦', 'ìª§', 'ìª¨', 'ìª©', 'ìªª',
-'ìª«', 'ìª¬', 'ìª­', 'ìª®', 'ìª¯', 'ìª°', 'ìª±', 'ìª²', 'ìª³', 'ìª´', 'ìªµ',
-'ìª¶', 'ìª·', 'ìª¸', 'ìª¹', 'ìªº', 'ìª»', 'ìª¾', 'ìª¿', 'ì«', 'ì«', 'ì«',
-'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«',
-'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«¡', 'ì«¢',
-'ì«£', 'ì«¤', 'ì«¥', 'ì«¦', 'ì«§', 'ì«¨', 'ì«©', 'ì«ª', 'ì««', 'ì«­', 'ì«®',
-'ì«¯', 'ì«°', 'ì«±', 'ì«²', 'ì«³', 'ì«µ', 'ì«¶', 'ì«·', 'ì«¸', 'ì«¹', 'ì«º',
-'ì«»', 'ì«¼', 'ì«½', 'ì«¾', 'ì«¿', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬',
-'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬',
-'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬',
-'ì¬¢', 'ì¬£', 'ì¬¤', 'ì¬¥', 'ì¬¦', 'ì¬§', 'ì¬¨', 'ì¬©', 'ì¬ª', 'ì¬«', 'ì¬¬',
-'ì¬­', 'ì¬®', 'ì¬¯', 'ì¬°', 'ì¬±', 'ì¬²', 'ì¬³', 'ì¬´', 'ì¬µ', 'ì¬¶', 'ì¬·',
-'ì¬¸', 'ì¬¹', 'ì¬º', 'ì¬»', 'ì¬¼', 'ì¬½', 'ì¬¾', 'ì¬¿', 'ì­', 'ì­', 'ì­',
-'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­',
-'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­ ',
-'ì­¡', 'ì­¢', 'ì­£', 'ì­¥', 'ì­¦', 'ì­§', 'ì­¨', 'ì­©', 'ì­ª', 'ì­«', 'ì­¬',
-'ì­­', 'ì­®', 'ì­¯', 'ì­°', 'ì­±', 'ì­²', 'ì­³', 'ì­´', 'ì­µ', 'ì­¶', 'ì­·',
-'ì­º', 'ì­»', 'ì­¼', 'ì­½', 'ì­¾', 'ì­¿', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®',
-'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®',
-'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®',
-'ì®', 'ì®', 'ì®', 'ì®', 'ì® ', 'ì®¡', 'ì®¢', 'ì®£', 'ì®¤', 'ì®¥', 'ì®¦',
-'ì®§', 'ì®¨', 'ì®©', 'ì®ª', 'ì®«', 'ì®¬', 'ì®­', 'ì®®', 'ì®¯', 'ì®°', 'ì®±',
-'ì®²', 'ì®³', 'ì®´', 'ì®µ', 'ì®¶', 'ì®·', 'ì®¹', 'ì®º', 'ì®»', 'ì®¼', 'ì®½',
-'ì®¾', 'ì®¿', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯',
-'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯',
-'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯',
-'ì¯ ', 'ì¯¡', 'ì¯¢', 'ì¯£', 'ì¯¥', 'ì¯¦', 'ì¯¨', 'ì¯ª', 'ì¯«', 'ì¯¬', 'ì¯­',
-'ì¯®', 'ì¯¯', 'ì¯°', 'ì¯±', 'ì¯²', 'ì¯³', 'ì¯´', 'ì¯µ', 'ì¯¶', 'ì¯·', 'ì¯¸',
-'ì¯¹', 'ì¯º', 'ì¯»', 'ì¯¼', 'ì¯½', 'ì¯¾', 'ì¯¿', 'ì°', 'ì°', 'ì°', 'ì°',
-'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°',
-'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°',
-'ì° ', 'ì°£', 'ì°¤', 'ì°¥', 'ì°¦', 'ì°ª', 'ì°«', 'ì°­', 'ì°¯', 'ì°±', 'ì°²',
-'ì°³', 'ì°´', 'ì°µ', 'ì°¶', 'ì°·', 'ì°º', 'ì°¿', 'ì±', 'ì±', 'ì±', 'ì±',
-'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±',
-'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±¡', 'ì±¢', 'ì±£',
-'ì±¥', 'ì±§', 'ì±©', 'ì±ª', 'ì±«', 'ì±¬', 'ì±­', 'ì±®', 'ì±¯', 'ì±±', 'ì±²',
-'ì±³', 'ì±´', 'ì±¶', 'ì±·', 'ì±¸', 'ì±¹', 'ì±º', 'ì±»', 'ì±¼', 'ì±½', 'ì±¾',
-'ì±¿', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²',
-'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²',
-'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²¡', 'ì²¢', 'ì²£',
-'ì²¤', 'ì²¥', 'ì²¦', 'ì²§', 'ì²ª', 'ì²®', 'ì²¯', 'ì²°', 'ì²±', 'ì²²', 'ì²³',
-'ì²¶', 'ì²·', 'ì²¹', 'ì²º', 'ì²»', 'ì²½', 'ì²¾', 'ì²¿', 'ì³', 'ì³', 'ì³',
-'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³',
-'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³',
-'ì³', 'ì³ ', 'ì³¡', 'ì³¢', 'ì³£', 'ì³¥', 'ì³¦', 'ì³§', 'ì³¨', 'ì³©', 'ì³ª',
-'ì³«', 'ì³­', 'ì³®', 'ì³¯', 'ì³±', 'ì³²', 'ì³³', 'ì³´', 'ì³µ', 'ì³¶', 'ì³·',
-'ì³¸', 'ì³¹', 'ì³º', 'ì³»', 'ì³¼', 'ì³½', 'ì³¾', 'ì³¿', 'ì´', 'ì´', 'ì´',
-'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´',
-'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´ ', 'ì´¡',
-'ì´¢', 'ì´£', 'ì´¥', 'ì´¦', 'ì´§', 'ì´©', 'ì´ª', 'ì´«', 'ì´­', 'ì´®', 'ì´¯',
-'ì´°', 'ì´±', 'ì´²', 'ì´³', 'ì´´', 'ì´µ', 'ì´¶', 'ì´·', 'ì´¸', 'ì´º', 'ì´»',
-'ì´¼', 'ì´½', 'ì´¾', 'ì´¿', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ',
-'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ',
-'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ',
-'ìµ', 'ìµ', 'ìµ¡', 'ìµ¢', 'ìµ£', 'ìµ¥', 'ìµ¦', 'ìµ§', 'ìµ¨', 'ìµ©', 'ìµª',
-'ìµ«', 'ìµ®', 'ìµ°', 'ìµ²', 'ìµ³', 'ìµ´', 'ìµµ', 'ìµ¶', 'ìµ·', 'ìµ¹', 'ìµº',
-'ìµ»', 'ìµ¼', 'ìµ½', 'ìµ¾', 'ìµ¿', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶',
-'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶',
-'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶ ',
-'ì¶¡', 'ì¶¢', 'ì¶£', 'ì¶¦', 'ì¶¨', 'ì¶ª', 'ì¶«', 'ì¶¬', 'ì¶­', 'ì¶®', 'ì¶¯',
-'ì¶±', 'ì¶²', 'ì¶³', 'ì¶´', 'ì¶µ', 'ì¶¶', 'ì¶·', 'ì¶¸', 'ì¶¹', 'ì¶º', 'ì¶»',
-'ì¶¼', 'ì¶½', 'ì¶¾', 'ì¶¿', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·',
-'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·',
-'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·',
-'ì· ', 'ì·¡', 'ì·¢', 'ì·£', 'ì·¤', 'ì·¥', 'ì·¦', 'ì·§', 'ì·©', 'ì·ª', 'ì·«',
-'ì·­', 'ì·®', 'ì·¯', 'ì·±', 'ì·²', 'ì·³', 'ì·´', 'ì·µ', 'ì·¶', 'ì··', 'ì·º',
-'ì·¼', 'ì·¾', 'ì·¿', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸',
-'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸',
-'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸¢', 'ì¸£', 'ì¸¥',
-'ì¸¦', 'ì¸§', 'ì¸©', 'ì¸ª', 'ì¸«', 'ì¸¬', 'ì¸­', 'ì¸®', 'ì¸¯', 'ì¸²', 'ì¸´',
-'ì¸¶', 'ì¸·', 'ì¸¸', 'ì¸¹', 'ì¸º', 'ì¸»', 'ì¸¼', 'ì¸½', 'ì¸¾', 'ì¸¿', 'ì¹',
-'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹',
-'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹',
-'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹¢', 'ì¹£', 'ì¹¤', 'ì¹¥', 'ì¹¦', 'ì¹§',
-'ì¹ª', 'ì¹¬', 'ì¹®', 'ì¹¯', 'ì¹°', 'ì¹±', 'ì¹²', 'ì¹³', 'ì¹¶', 'ì¹·', 'ì¹¹',
-'ì¹º', 'ì¹»', 'ì¹½', 'ì¹¾', 'ì¹¿', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº',
-'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº',
-'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº¢', 'ìº¦', 'ìº§', 'ìº¨',
-'ìº©', 'ìºª', 'ìº«', 'ìº®', 'ìº¯', 'ìº°', 'ìº±', 'ìº²', 'ìº³', 'ìº´', 'ìºµ',
-'ìº¶', 'ìº·', 'ìº¸', 'ìº¹', 'ìºº', 'ìº»', 'ìº¼', 'ìº½', 'ìº¾', 'ìº¿', 'ì»',
-'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»',
-'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»',
-'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì» ', 'ì»¡', 'ì»¢',
-'ì»£', 'ì»¦', 'ì»§', 'ì»©', 'ì»ª', 'ì»­', 'ì»®', 'ì»¯', 'ì»°', 'ì»±', 'ì»²',
-'ì»³', 'ì»¶', 'ì»º', 'ì»»', 'ì»¼', 'ì»½', 'ì»¾', 'ì»¿', 'ì¼', 'ì¼', 'ì¼',
-'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼',
-'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼¡', 'ì¼¢',
-'ì¼£', 'ì¼¥', 'ì¼¦', 'ì¼§', 'ì¼¨', 'ì¼©', 'ì¼ª', 'ì¼«', 'ì¼®', 'ì¼²', 'ì¼³',
-'ì¼´', 'ì¼µ', 'ì¼¶', 'ì¼·', 'ì¼¹', 'ì¼º', 'ì¼»', 'ì¼¼', 'ì¼½', 'ì¼¾', 'ì¼¿',
-'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½',
-'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½',
-'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½ ', 'ì½¡', 'ì½¢', 'ì½£', 'ì½¦',
-'ì½¨', 'ì½ª', 'ì½«', 'ì½¬', 'ì½­', 'ì½®', 'ì½¯', 'ì½²', 'ì½³', 'ì½µ', 'ì½¶',
-'ì½·', 'ì½¹', 'ì½º', 'ì½»', 'ì½¼', 'ì½½', 'ì½¾', 'ì½¿', 'ì¾', 'ì¾', 'ì¾',
-'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾',
-'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾',
-'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾ ', 'ì¾¢', 'ì¾£', 'ì¾¤', 'ì¾¥', 'ì¾¦', 'ì¾§',
-'ì¾©', 'ì¾ª', 'ì¾«', 'ì¾¬', 'ì¾­', 'ì¾®', 'ì¾¯', 'ì¾±', 'ì¾²', 'ì¾³', 'ì¾´',
-'ì¾µ', 'ì¾¶', 'ì¾·', 'ì¾¸', 'ì¾¹', 'ì¾º', 'ì¾»', 'ì¾¼', 'ì¾½', 'ì¾¾', 'ì¾¿',
-'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿',
-'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿',
-'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿¢', 'ì¿£',
-'ì¿¥', 'ì¿¦', 'ì¿§', 'ì¿©', 'ì¿ª', 'ì¿«', 'ì¿¬', 'ì¿­', 'ì¿®', 'ì¿¯', 'ì¿²',
-'ì¿´', 'ì¿¶', 'ì¿·', 'ì¿¸', 'ì¿¹', 'ì¿º', 'ì¿»', 'ì¿½', 'ì¿¾', 'ì¿¿', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¥',
-'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬', 'í®', 'í¯', 'í°', 'í±',
-'í²', 'í³', 'í¶', 'í·', 'í¹', 'íº', 'í»', 'í½', 'í¾', 'í¿', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©',
-'íª', 'í«', 'í®', 'í¯', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¸',
-'í¹', 'íº', 'í»', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¦', 'í§', 'í©', 'íª',
-'í«', 'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í¶', 'í¸', 'íº',
-'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¥', 'í¦', 'í§', 'í¨', 'í©',
-'íª', 'í«', 'í®', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¹', 'íº',
-'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§',
-'í¨', 'í©', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯', 'í²', 'í³', 'íµ',
-'í¶', 'í·', 'í¹', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¢', 'í£', 'í¤', 'í¥',
-'í¦', 'í§', 'í©', 'íª', 'í«', 'í­', 'í®', 'í¯', 'í°', 'í±', 'í²',
-'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¸', 'í¹', 'íº', 'í»', 'í½', 'í¾',
-'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í¢', 'í£',
-'í¥', 'í¦', 'í§', 'í©', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯', 'í²',
-'í´', 'í¶', 'í·', 'í¸', 'í¹', 'í»', 'í½', 'í¾', 'í¿', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤',
-'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯',
-'í°', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¹', 'íº', 'í»', 'í¼',
-'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ',
-'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¸', 'í¹', 'íº',
-'í»', 'í¾', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬', 'í­',
-'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¸',
-'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¢',
-'í£', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í­', 'í®', 'í¯',
-'í°', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'íº', 'í»', 'í½', 'í¾',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¦', 'í§', 'í¨', 'í©', 'íª',
-'í«', 'í¬', 'í­', 'í®', 'í¯', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¹',
-'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í¢', 'í£', 'í¤', 'í¦', 'í§', 'íª', 'í«', 'í­',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'íº', 'í¾',
-'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬',
-'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'í¸', 'í¹', 'íº', 'í»', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¤', 'í¥',
-'í¦', 'í§', 'íª', 'í¬', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'íµ',
-'í¶', 'í·', 'í¹', 'íº', 'í»', 'í½', 'í¾', 'í¿', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í ', 'í¢', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¸', 'í¹', 'íº',
-'í»', 'í¾', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬',
-'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'í¸', 'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¥', 'í¦', 'í§', 'í¨',
-'í©', 'íª', 'í«', 'í¬', 'í®', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ',
-'í¶', 'í·', 'íº', 'í»', 'í½', 'í¾', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'íª', 'í«', 'í¬', 'í­',
-'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¸',
-'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í©', 'íª',
-'í«', 'í­', 'í®', 'í¯', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'í¹', 'íº', 'í¼', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬',
-'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'í¸', 'í¹', 'íº', 'í»', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¤',
-'í¦', 'í§', 'íª', 'í¬', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í¶',
-'í·', 'í¹', 'íº', 'í»', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«',
-'í¬', 'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶',
-'í·', 'í¸', 'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ',
-'í¡', 'í¢', 'í£', 'í¦', 'í§', 'í©', 'íª', 'í«', 'í­', 'í®', 'í¯',
-'í°', 'í±', 'í²', 'í³', 'í¶', 'í¸', 'íº', 'í»', 'í¼', 'í½', 'í¾',
-'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í¡', 'í¢', 'í£', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«',
-'í¬', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'íº', 'í»', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦',
-'í¨', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯', 'í²', 'í³', 'íµ', 'í¶',
-'í·', 'í¸', 'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í ', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í©', 'íª', 'í«', 'í­',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¸', 'íº',
-'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¥', 'í¦',
-'í§', 'í©', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯', 'í±', 'í²', 'í³',
-'í´', 'í¶', 'í·', 'í¸', 'í¹', 'íº', 'í»', 'í¾', 'í¿', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'íª', 'í¬',
-'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í¶', 'í·', 'í¹', 'íº', 'í»',
-'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í¢', 'í¤', 'í¦', 'í§', 'í¨', 'íª', 'í«', 'í­',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¸', 'í¹', 'íº',
-'í»', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', '\ud7a4'] ``` 28.
-get_all_incompleted_form_hangul_chars This returns all non-completed form
-Hangul characters. Returns: - `List[str]`: all non-completed form Hangul
-characters Examples: ```python >>> from kss import Kss >>>
-get_all_incompleted_form_hangul_chars = Kss
+get_all_completed_form_hangul_chars = Kss
+("get_all_completed_form_hangul_chars") >>> output =
+get_all_completed_form_hangul_chars() >>> print(output) ['ê°', 'ê°', 'ê°',
+'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°',
+'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê° ', 'ê°¤', 'ê°¬', 'ê°­', 'ê°¯',
+'ê°°', 'ê°±', 'ê°¸', 'ê°¹', 'ê°¼', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
+'ê±°', 'ê±±', 'ê±´', 'ê±·', 'ê±¸', 'ê±º', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²',
+'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê² ',
+'ê²¡', 'ê²¨', 'ê²©', 'ê²ª', 'ê²¬', 'ê²¯', 'ê²°', 'ê²¸', 'ê²¹', 'ê²»', 'ê²¼',
+'ê²½', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³ ', 'ê³¡', 'ê³¤', 'ê³§',
+'ê³¨', 'ê³ª', 'ê³¬', 'ê³¯', 'ê³°', 'ê³±', 'ê³³', 'ê³µ', 'ê³¶', 'ê³¼', 'ê³½',
+'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´ ', 'ê´©',
+'ê´¬', 'ê´­', 'ê´´', 'ê´µ', 'ê´¸', 'ê´¼', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ',
+'êµ', 'êµ', 'êµ¡', 'êµ£', 'êµ¬', 'êµ­', 'êµ°', 'êµ³', 'êµ´', 'êµµ', 'êµ¶',
+'êµ»', 'êµ¼', 'êµ½', 'êµ¿', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶',
+'ê¶', 'ê¶¤', 'ê¶·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·',
+'ê· ', 'ê·¤', 'ê·¸', 'ê·¹', 'ê·¼', 'ê·¿', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸',
+'ê¸', 'ê¸', 'ê¸°', 'ê¸±', 'ê¸´', 'ê¸·', 'ê¸¸', 'ê¸º', 'ê¹', 'ê¹', 'ê¹',
+'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹',
+'ê¹', 'ê¹ ', 'ê¹¡', 'ê¹¥', 'ê¹¨', 'ê¹©', 'ê¹¬', 'ê¹°', 'ê¹¸', 'ê¹¹', 'ê¹»',
+'ê¹¼', 'ê¹½', 'êº', 'êº', 'êº', 'êº¼', 'êº½', 'êº¾', 'ê»', 'ê»', 'ê»',
+'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»¨', 'ê»«', 'ê»­', 'ê»´',
+'ê»¸', 'ê»¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼¬', 'ê¼­', 'ê¼°', 'ê¼²', 'ê¼´',
+'ê¼¼', 'ê¼½', 'ê¼¿', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½',
+'ê½¤', 'ê½¥', 'ê½¹', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾¸',
+'ê¾¹', 'ê¾¼', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿',
+'ê¿¨', 'ê¿©', 'ê¿°', 'ê¿±', 'ê¿´', 'ê¿¸', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë¨', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë¼', 'ë½', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë¨',
+'ë©', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë±', 'ë³', 'ë´', 'ëµ', 'ë¸',
+'ë¼', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ',
+'ë¥', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë£', 'ë¤', 'ë¥', 'ë¨', 'ë¬', 'ë´', 'ëµ', 'ë·', 'ë¸',
+'ë¹', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë ', 'ë¸', 'ë¹', 'ë¼', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë¨', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë¨', 'ë©', 'ë¬', 'ë°', 'ë¹', 'ë»', 'ë½', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë´', 'ë¼', 'ë', 'ë', 'ë ',
+'ë¨', 'ë©', 'ë´', 'ëµ', 'ë¼', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë£', 'ë¥', 'ë¦', 'ëª', 'ë¬', 'ë°',
+'ë´', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë¢',
+'ë¤', 'ë¥', 'ë¦', 'ë¨', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë³', 'ë´',
+'ëµ', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¿', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë¤', 'ë¥', 'ë§', 'ë©', 'ë«', 'ë®', 'ë°', 'ë±',
+'ë´', 'ë¸', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ',
+'ë¡', 'ë¨', 'ë¬', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¤', 'ë¨', 'ë¼', 'ë', 'ë',
+'ë', 'ë ', 'ë¨', 'ë©', 'ë«', 'ë´', 'ë', 'ë', 'ë', 'ë', 'ë ',
+'ë¡', 'ë£', 'ë¥', 'ë¬', 'ë', 'ë', 'ë', 'ë¤', 'ë¨', 'ë¬', 'ëµ',
+'ë·', 'ë¹', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë£',
+'ë¤', 'ë¦', 'ë¬', 'ë­', 'ë¯', 'ë±', 'ë¸', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë¤', 'ë¥', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë°', 'ë±', 'ë´', 'ë¸',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë ', 'ë¡', 'ë ', 'ë¡', 'ë¤', 'ë¨', 'ëª', 'ë«', 'ë°',
+'ë±', 'ë³', 'ë´', 'ëµ', 'ë»', 'ë¼', 'ë½', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë¬', 'ë', 'ë', 'ë', 'ë', 'ë¥', 'ë¬',
+'ë´', 'ë', 'ë¤', 'ë¨', 'ë', 'ë', 'ë ', 'ë¤', 'ë«', 'ë¬', 'ë±',
+'ë', 'ë°', 'ë´', 'ë¸', 'ë', 'ë', 'ë', 'ë¨', 'ë©', 'ë¬', 'ë¯',
+'ë°', 'ë¸', 'ë¹', 'ë»', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¤',
+'ë¨', 'ë°', 'ë±', 'ë³', 'ëµ', 'ë¼', 'ë½', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¨',
+'ë©', 'ë«', 'ë¬', 'ë­', 'ë´', 'ëµ', 'ë¸', 'ë', 'ë', 'ë¬', 'ë­',
+'ë°', 'ë´', 'ë¼', 'ë½', 'ë¿', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ',
+'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ¤', 'ë ¥', 'ë ¨', 'ë ¬', 'ë ´', 'ë µ',
+'ë ·', 'ë ¸', 'ë ¹', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡ ', 'ë¡¤',
+'ë¡¬', 'ë¡­', 'ë¡¯', 'ë¡±', 'ë¡¸', 'ë¡¼', 'ë¢', 'ë¢¨', 'ë¢°', 'ë¢´', 'ë¢¸',
+'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£¡', 'ë£¨',
+'ë£©', 'ë£¬', 'ë£°', 'ë£¸', 'ë£¹', 'ë£»', 'ë£½', 'ë¤', 'ë¤', 'ë¤ ', 'ë¤¼',
+'ë¤½', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥ ', 'ë¥¨',
+'ë¥©', 'ë¥«', 'ë¥­', 'ë¥´', 'ë¥µ', 'ë¥¸', 'ë¥¼', 'ë¦', 'ë¦', 'ë¦', 'ë¦',
+'ë¦', 'ë¦', 'ë¦', 'ë¦¬', 'ë¦­', 'ë¦°', 'ë¦´', 'ë¦¼', 'ë¦½', 'ë¦¿', 'ë§',
+'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§',
+'ë§', 'ë§', 'ë§¡', 'ë§£', 'ë§¤', 'ë§¥', 'ë§¨', 'ë§¬', 'ë§´', 'ë§µ', 'ë§·',
+'ë§¸', 'ë§¹', 'ë§º', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨¸', 'ë¨¹', 'ë¨¼', 'ë©',
+'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©',
+'ë©¤', 'ë©¥', 'ë©§', 'ë©¨', 'ë©©', 'ë©°', 'ë©±', 'ë©´', 'ë©¸', 'ëª', 'ëª',
+'ëª', 'ëª', 'ëª', 'ëª¨', 'ëª©', 'ëª«', 'ëª¬', 'ëª°', 'ëª²', 'ëª¸', 'ëª¹',
+'ëª»', 'ëª½', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«¼', 'ë¬', 'ë¬', 'ë¬', 'ë¬',
+'ë¬', 'ë¬', 'ë¬', 'ë¬ ', 'ë¬©', 'ë¬«', 'ë¬´', 'ë¬µ', 'ë¬¶', 'ë¬¸', 'ë¬»',
+'ë¬¼', 'ë¬½', 'ë¬¾', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­',
+'ë­', 'ë­¡', 'ë­£', 'ë­¬', 'ë®', 'ë®', 'ë®', 'ë®¤', 'ë®¨', 'ë®¬', 'ë®´',
+'ë®·', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯¸', 'ë¯¹', 'ë¯¼', 'ë¯¿', 'ë°',
+'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°',
+'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°¤', 'ë°¥', 'ë°§', 'ë°©',
+'ë°­', 'ë°°', 'ë°±', 'ë°´', 'ë°¸', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±',
+'ë±', 'ë±', 'ë±', 'ë±', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²',
+'ë²', 'ë²', 'ë²', 'ë²', 'ë² ', 'ë²¡', 'ë²¤', 'ë²§', 'ë²¨', 'ë²°', 'ë²±',
+'ë²³', 'ë²´', 'ë²µ', 'ë²¼', 'ë²½', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³',
+'ë³', 'ë³', 'ë³', 'ë³´', 'ë³µ', 'ë³¶', 'ë³¸', 'ë³¼', 'ë´', 'ë´', 'ë´',
+'ë´', 'ë´', 'ë´', 'ë´¤', 'ë´¬', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ',
+'ëµ', 'ëµ¤', 'ëµ¨', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶',
+'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶¤', 'ë¶°', 'ë¶¸', 'ë·', 'ë·',
+'ë·', 'ë·', 'ë·©', 'ë·°', 'ë·´', 'ë·¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸',
+'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹',
+'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹ ', 'ë¹¡', 'ë¹¤', 'ë¹¨', 'ë¹ª', 'ë¹°',
+'ë¹±', 'ë¹³', 'ë¹´', 'ë¹µ', 'ë¹»', 'ë¹¼', 'ë¹½', 'ëº', 'ëº', 'ëº', 'ëº',
+'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº¨', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»',
+'ë» ', 'ë»£', 'ë»¤', 'ë»¥', 'ë»¬', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼',
+'ë¼', 'ë¼', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë¾', 'ë¾°',
+'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿¡', 'ì¼', 'ì', 'ì',
+'ì', 'ì ', 'ì¨', 'ì©', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì£',
+'ì¥', 'ì¬', 'ì­', 'ì¯', 'ì°', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì¼', 'ì½',
+'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì¤', 'ì¥', 'ì¨', 'ì¬', 'ì´', 'ìµ', 'ì·', 'ì¹', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì£', 'ì¤',
+'ì¦', 'ì§', 'ì¬', 'ì­', 'ì¯', 'ì°', 'ì±', 'ì¶', 'ì¸', 'ì¹', 'ì¼',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¤',
+'ì¥', 'ì§', 'ì¨', 'ì©', 'ì°', 'ì´', 'ì¸', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¥', 'ì¨', 'ì©', 'ì¬',
+'ì°', 'ì½', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¤', 'ì¨',
+'ì°', 'ì±', 'ì³', 'ì¼', 'ì½', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¨', 'ì©', 'ì«', 'ì­', 'ì¯', 'ì±',
+'ì²', 'ì´', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¥', 'ì¬', 'ì­',
+'ì°', 'ì´', 'ì¼', 'ì½', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì¤', 'ì¥', 'ì¨', 'ì¬', 'ì­', 'ì´', 'ìµ', 'ì·', 'ì¹', 'ì',
+'ì', 'ì ', 'ì£', 'ì¤', 'ì«', 'ì¬', 'ì­', 'ì¯', 'ì±', 'ì¶', 'ì¸',
+'ì¹', 'ì»', 'ì¼', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì¤', 'ì¥', 'ì¨', 'ì©', 'ì', 'ì¨', 'ì©', 'ì¬', 'ì°',
+'ì²', 'ì¸', 'ì¹', 'ì¼', 'ì½', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì ', 'ì¢', 'ì¨', 'ì©', 'ì­', 'ì´', 'ìµ', 'ì¸', 'ì',
+'ì', 'ì¤', 'ì¬', 'ì°', 'ì´', 'ì¼', 'ì½', 'ì', 'ì¤', 'ì¥', 'ì¨',
+'ì¬', 'ì´', 'ìµ', 'ì¹', 'ì', 'ì', 'ì', 'ì¸', 'ì¼', 'ì©', 'ì°',
+'ì±', 'ì´', 'ì¸', 'ìº', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì¨', 'ì©', 'ì¬', 'ì°', 'ì¸', 'ì¹', 'ì»', 'ì½', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì ', 'ì¡', 'ì¤', 'ì¨', 'ì°', 'ì±', 'ì³', 'ì´', 'ìµ',
+'ì¼', 'ì½', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì ', 'ì©', 'ì´', 'ìµ', 'ì¸', 'ì¹', 'ì»', 'ì¼', 'ì½',
+'ì¾', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì£', 'ì¥', 'ì¬', 'ì­', 'ì®', 'ì°',
+'ì´', 'ì¶', 'ì·', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¤', 'ì¥', 'ì¨',
+'ì¬', 'ì­', 'ì®', 'ì°', 'ì³', 'ì´', 'ìµ', 'ì·', 'ì¹', 'ì»', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ',
+'ì¬', 'ì¯', 'ì±', 'ì¸', 'ì¹', 'ì¼', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì¤', 'ì¥', 'ì§', 'ì©', 'ì°', 'ì±', 'ì´',
+'ì¸', 'ì¹', 'ìº', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì ', 'ì¡', 'ì¨', 'ì©', 'ì¬', 'ì°', 'ì¸', 'ì¹', 'ì½',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¤',
+'ì¨', 'ì°', 'ì±', 'ì³', 'ìµ', 'ì·', 'ì¼', 'ì½', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì ', 'ì¨', 'ì«', 'ì´', 'ìµ', 'ì¸', 'ì¼', 'ì½', 'ì¾', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì¬', 'ì­',
+'ì°', 'ì´', 'ì¼', 'ì½', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì¤', 'ì¨', 'ì¬', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ',
+'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì  ', 'ì ¤', 'ì ¬', 'ì ­',
+'ì ¯', 'ì ±', 'ì ¸', 'ì ¼', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡°',
+'ì¡±', 'ì¡´', 'ì¡¸', 'ì¡º', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢',
+'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢¡', 'ì¢¨', 'ì¢¼', 'ì¢½', 'ì£', 'ì£',
+'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£ ', 'ì£¡', 'ì£¤', 'ì£µ', 'ì£¼', 'ì£½',
+'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤¬', 'ì¤´',
+'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥ ', 'ì¥¡', 'ì¥£', 'ì¥¬', 'ì¥°', 'ì¥´', 'ì¥¼',
+'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì§', 'ì§', 'ì§',
+'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§',
+'ì§', 'ì§ ', 'ì§¢', 'ì§¤', 'ì§§', 'ì§¬', 'ì§­', 'ì§¯', 'ì§°', 'ì§±', 'ì§¸',
+'ì§¹', 'ì§¼', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨©',
+'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì© ', 'ì©¡', 'ì©¨', 'ì©½',
+'ìª', 'ìª', 'ìª¼', 'ìª½', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«',
+'ì«', 'ì«', 'ì« ', 'ì«¬', 'ì«´', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬ ', 'ì¬¡',
+'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­¤', 'ì­¸', 'ì­¹',
+'ì®', 'ì®¸', 'ì¯', 'ì¯¤', 'ì¯§', 'ì¯©', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°',
+'ì°', 'ì°¡', 'ì°¢', 'ì°§', 'ì°¨', 'ì°©', 'ì°¬', 'ì°®', 'ì°°', 'ì°¸', 'ì°¹',
+'ì°»', 'ì°¼', 'ì°½', 'ì°¾', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±',
+'ì±', 'ì±', 'ì± ', 'ì±¤', 'ì±¦', 'ì±¨', 'ì±°', 'ì±µ', 'ì²', 'ì²', 'ì²',
+'ì² ', 'ì²¨', 'ì²©', 'ì²«', 'ì²¬', 'ì²­', 'ì²´', 'ì²µ', 'ì²¸', 'ì²¼', 'ì³',
+'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³¤', 'ì³¬', 'ì³°', 'ì´', 'ì´', 'ì´',
+'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´¤', 'ì´¨', 'ì´¬', 'ì´¹', 'ìµ',
+'ìµ ', 'ìµ¤', 'ìµ¬', 'ìµ­', 'ìµ¯', 'ìµ±', 'ìµ¸', 'ì¶', 'ì¶', 'ì¶', 'ì¶',
+'ì¶', 'ì¶¤', 'ì¶¥', 'ì¶§', 'ì¶©', 'ì¶°', 'ì·', 'ì·', 'ì·', 'ì·¨', 'ì·¬',
+'ì·°', 'ì·¸', 'ì·¹', 'ì·»', 'ì·½', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸ ',
+'ì¸¡', 'ì¸¤', 'ì¸¨', 'ì¸°', 'ì¸±', 'ì¸³', 'ì¸µ', 'ì¹', 'ì¹', 'ì¹', 'ì¹',
+'ì¹ ', 'ì¹¡', 'ì¹¨', 'ì¹©', 'ì¹«', 'ì¹­', 'ì¹´', 'ì¹µ', 'ì¹¸', 'ì¹¼', 'ìº',
+'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº ', 'ìº¡', 'ìº£', 'ìº¤',
+'ìº¥', 'ìº¬', 'ìº­', 'ì»', 'ì»¤', 'ì»¥', 'ì»¨', 'ì»«', 'ì»¬', 'ì»´', 'ì»µ',
+'ì»·', 'ì»¸', 'ì»¹', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼',
+'ì¼', 'ì¼ ', 'ì¼¤', 'ì¼¬', 'ì¼­', 'ì¼¯', 'ì¼°', 'ì¼±', 'ì¼¸', 'ì½', 'ì½',
+'ì½', 'ì½', 'ì½¤', 'ì½¥', 'ì½§', 'ì½©', 'ì½°', 'ì½±', 'ì½´', 'ì½¸', 'ì¾',
+'ì¾', 'ì¾', 'ì¾¡', 'ì¾¨', 'ì¾°', 'ì¿', 'ì¿ ', 'ì¿¡', 'ì¿¤', 'ì¿¨', 'ì¿°',
+'ì¿±', 'ì¿³', 'ì¿µ', 'ì¿¼', 'í', 'í', 'í', 'í', 'í­', 'í´', 'íµ',
+'í¸', 'í¼', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¬',
+'í­', 'í°', 'í´', 'í¼', 'í½', 'í', 'í¤', 'í¥', 'í¨', 'í¬', 'í´',
+'íµ', 'í·', 'í¹', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í ', 'í¤', 'í¬', 'í­', 'í¯', 'í°', 'í±',
+'í¸', 'í', 'í°', 'í±', 'í´', 'í¸', 'íº', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¨', 'í¬',
+'í¼', 'í', 'í', 'í ', 'í¡', 'í¤', 'í¨', 'í°', 'í±', 'í³', 'íµ',
+'íº', 'í¼', 'í', 'í', 'í´', 'í¸', 'í', 'í', 'í', 'í¬', 'í­',
+'í°', 'í´', 'í¼', 'í½', 'í¿', 'í', 'í', 'í', 'í¤', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¤', 'í¬', 'í±', 'í¸',
+'í¹', 'í¼', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í¤', 'í¥', 'í°', 'í±', 'í´', 'í¸', 'í', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¥',
+'í¨', 'í©', 'í¬', 'í°', 'í¸', 'í¹', 'í»', 'í¼', 'í½', 'í', 'í',
+'í¼', 'í½', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í ', 'í¨', 'í©', 'í«', 'í­', 'í´', 'í¸', 'í¼', 'í', 'í',
+'í', 'í', 'í', 'í', 'í¡', 'í£', 'í¬', 'í­', 'í°', 'í´', 'í¼',
+'í½', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¤', 'í­',
+'í¯', 'í¸', 'í¹', 'í¼', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í©', 'í', 'í', 'í', 'í', 'í', 'í¨', 'í¬', 'í°', 'í¸',
+'í»', 'í½', 'í', 'í', 'í', 'í', 'í', 'í', 'í¼', 'í½', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¥', 'í¨',
+'í©', 'í«', 'í­', 'í´', 'íµ', 'í¸', 'í¼', 'í', 'í', 'í', 'í',
+'í', 'í', 'í¥', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í¤', 'í¥', 'í¨', 'í¬', 'í´', 'íµ', 'í·', 'í¹', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¤', 'í­',
+'í¸', 'í¹', 'í¼', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í§', 'í©', 'í°', 'í±', 'í´', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í¡', 'í¨', 'í¬', 'í°', 'í¹', 'í»',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¤', 'í¨',
+'í°', 'íµ', 'í¼', 'í½', 'í', 'í', 'í', 'í', 'í', 'í', 'í ',
+'í¨', 'í©', 'í«', 'í­', 'í´', 'íµ', 'í¸', 'í¼', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡', 'í£', 'í¥',
+'í©', 'í¬', 'í°', 'í´', 'í¼', 'í½', 'í', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í'] ``` 28. get_all_incompleted_form_hangul_chars This
+returns all incompleted form Hangul characters. Returns: - `List[str]`: all
+incompleted form Hangul characters Examples: ```python >>> from kss import Kss
+>>> get_all_incompleted_form_hangul_chars = Kss
 ("get_all_incompleted_form_hangul_chars") >>> output =
 get_all_incompleted_form_hangul_chars() >>> print(output) ['ê°', 'ê°', 'ê°',
 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°¡', 'ê°¢',
 'ê°£', 'ê°¥', 'ê°¦', 'ê°§', 'ê°¨', 'ê°©', 'ê°ª', 'ê°«', 'ê°®', 'ê°²', 'ê°³',
 'ê°´', 'ê°µ', 'ê°¶', 'ê°·', 'ê°º', 'ê°»', 'ê°½', 'ê°¾', 'ê°¿', 'ê±', 'ê±',
 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
@@ -2433,20 +1855,20 @@
 reduce_char_repeats_over (`int`): the maximum number of character that can be
 repeated - reduce_emoticon_repeats_over (`int`): the maximum number of emoticon
 that can be repeated - num_workers (`Union[int, str]`): the number of
 multiprocessing workers Returns: - `Union[str, List[str]]`: normalized text or
 list of normalized texts Examples: ```python >>> from kss import Kss >>>
 normalize = Kss("normalize") >>> text = "ìë\u200bíì¸ì
 ï¾»ï¾»ï¾»ï¾»ï¾»ï¾»
-ì¤ë\u200bì ë ì´ ì°¸ ì¢ë¤ì.\\n\\n\\n200 < 300 & 400" >>> normalize
-(text, allow_doubled_spaces=False, allow_html_tags=False,
-allow_html_escape=False, allow_halfwidth_hangul=False, allow_hangul_jamo=False,
+ì¤ë\u200bì ë ì´ ì°¸ ì¢ë¤ì.\n\n\n200 < 300 & 400" >>> normalize(text,
+allow_doubled_spaces=False, allow_html_tags=False, allow_html_escape=False,
+allow_halfwidth_hangul=False, allow_hangul_jamo=False,
 allow_invisible_chars=False, reduce_char_repeats_over=2,
 reduce_emoticon_repeats_over=2) 'ìëíì¸ì ãã ì¤ëì ë ì´ ì°¸
-ì¢ë¤ì.\\n200 < 300 & 400' ``` 32. preprocess This preprocesses text with
+ì¢ë¤ì.\n200 < 300 & 400' ``` 32. preprocess This preprocesses text with
 various options. This does 1) normalization, 2) filtering out, and 3)
 anonymization in order. Args: - text (`Union[str, List[str], Tuple[str]]`):
 single text or list of texts - normalization_type (`Optional[str]`):
 normalization type - allow_doubled_spaces (`bool`): whether to allow doubled
 spaces or not - allow_html_tags (`bool`): whether to allow HTML tags or not -
 allow_html_escape (`bool`): whether to allow HTML escape or not -
 allow_halfwidth_hangul (`bool`): whether to allow halfwidth Hangul or not -
@@ -2554,17 +1976,17 @@
 convert_numbers_to_hangul_phonemes (`bool`): whether to convert numbers to
 Hangul phonemes or not - num_workers (`Union[int, str]`): the number of
 multiprocessing workers Returns: - `Union[str, List[str]]`: romanized text or
 list of romanized texts Examples: ```python >>> from kss import Kss >>>
 romanize = Kss("romanize") >>> text = "ìëíì¸ì" >>> romanize(text)
 'annyeonghaseyo' >>> text = "ëê´ë ¹" >>> romanize(text) 'daegwallyeong' ```
 References: - This was copied from [korean-romanizer](https://github.com/osori/
-korean-romanizer) and modified by Kss 38. is_unsafe Check if the text is unsafe
-or not. Args: - text (`Union[str, List[str], Tuple[str]]`): single text or list
-of texts - return_matches (`bool`): whether to return matches or not -
+korean-romanizer) and modified by Kss 38. is_unsafe This checks if the text is
+unsafe or not. Args: - text (`Union[str, List[str], Tuple[str]]`): single text
+or list of texts - return_matches (`bool`): whether to return matches or not -
 num_workers (`Union[int, str]`): the number of multiprocessing workers Returns:
 - `Union[bool, List[bool], List[bool], List[List[str]]]`: whether the text is
 unsafe or not or list of whether the texts are unsafe or not or list of matched
 bad words in the texts Examples: ```python >>> from kss import Kss >>>
 is_unsafe = Kss("is_unsafe") >>> text = "ìëíì¸ì" >>> is_unsafe(text)
 False >>> text = "ìëíì¸ì. ì¨ë°" >>> is_unsafe(text) True >>> text =
 ["ìëíì¸ì", "ìëíì¸ì. ì¨ë°"] >>> is_unsafe(text) [False,
```

### Comparing `kss-6.0.0/bench/sentence_split/sentence_split.py` & `kss-6.0.0.dev0/bench/sentence_split/sentence_split.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/bench/sentence_split/test_baseline.py` & `kss-6.0.0.dev0/bench/sentence_split/test_baseline.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/bench/sentence_split/test_kiwi.py` & `kss-6.0.0.dev0/bench/sentence_split/test_kiwi.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/bench/sentence_split/test_koalanlp.py` & `kss-6.0.0.dev0/bench/sentence_split/test_koalanlp.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/bench/sentence_split/test_kss.py` & `kss-6.0.0.dev0/bench/sentence_split/test_kss.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/bench/sentence_split/test_word_split.py` & `kss-6.0.0.dev0/bench/sentence_split/test_word_split.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/csrc/kss_cython.pyx` & `kss-6.0.0.dev0/csrc/kss_cython.pyx`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/csrc/sentence_splitter.cpp` & `kss-6.0.0.dev0/csrc/sentence_splitter.cpp`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/csrc/sentence_splitter.h` & `kss-6.0.0.dev0/csrc/sentence_splitter.h`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/__init__.py` & `kss-6.0.0.dev0/kss/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,8 +177,8 @@
         if closest_module is None:
             return None
         else:
             return closest_module
 
 
 __ALL__ = list(supported_modules.keys()) + ["Kss"]
-__version__ = "6.0.0"
+__version__ = "6.0.0.dev0"
```

### Comparing `kss-6.0.0/kss/_elements/element.py` & `kss-6.0.0.dev0/kss/_elements/element.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_elements/empty.py` & `kss-6.0.0.dev0/kss/_elements/empty.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_elements/subclasses.py` & `kss-6.0.0.dev0/kss/_elements/subclasses.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/augmentation/assets/wordnet.json` & `kss-6.0.0.dev0/kss/_modules/augmentation/assets/wordnet.json`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/augmentation/augment.py` & `kss-6.0.0.dev0/kss/_modules/augmentation/augment.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/augmentation/distance.py` & `kss-6.0.0.dev0/kss/_modules/augmentation/distance.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/augmentation/replacement.py` & `kss-6.0.0.dev0/kss/_modules/augmentation/replacement.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/augmentation/utils.py` & `kss-6.0.0.dev0/kss/_modules/augmentation/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/collocation/collocate.py` & `kss-6.0.0.dev0/kss/_modules/collocation/collocate.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/g2p/assets/rules.txt` & `kss-6.0.0.dev0/kss/_modules/g2p/assets/rules.txt`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/g2p/assets/table.csv` & `kss-6.0.0.dev0/kss/_modules/g2p/assets/table.csv`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/g2p/english.py` & `kss-6.0.0.dev0/kss/_modules/g2p/english.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/g2p/g2p.py` & `kss-6.0.0.dev0/kss/_modules/g2p/g2p.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/g2p/numerals.py` & `kss-6.0.0.dev0/kss/_modules/g2p/numerals.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/g2p/regular.py` & `kss-6.0.0.dev0/kss/_modules/g2p/regular.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/g2p/special.py` & `kss-6.0.0.dev0/kss/_modules/g2p/special.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/g2p/utils.py` & `kss-6.0.0.dev0/kss/_modules/g2p/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulization.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulization.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/hangul.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/hangul.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/aze/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/aze/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/bel/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/bel/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/bul/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/bul/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/cat/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/cat/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ces/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ces/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/cym/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/cym/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/deu/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/deu/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ell/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ell/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/epo/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/epo/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/est/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/est/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/fin/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/fin/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/grc/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/grc/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/hun/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/hun/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/isl/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/isl/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ita/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ita/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/kat/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/kat/narrow.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/narrow.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lat/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lat/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lav/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lav/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lit/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lit/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/nld/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/nld/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/pol/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/pol/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/por/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/por/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/por/br.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/por/br.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ron/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ron/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/rus/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/rus/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/slk/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/slk/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/slv/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/slv/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/spa/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/spa/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/swe/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/swe/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/tur/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/tur/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/vie/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/vie/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/models.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/models.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/normalization.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/normalization.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hangulization/hangulize/processing.py` & `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/processing.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hanja/_hanja.py` & `kss-6.0.0.dev0/kss/_modules/hanja/_hanja.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/hanja/utils.py` & `kss-6.0.0.dev0/kss/_modules/hanja/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/jamo/_jamo.py` & `kss-6.0.0.dev0/kss/_modules/jamo/_jamo.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/jamo/utils.py` & `kss-6.0.0.dev0/kss/_modules/jamo/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/josa/josa.py` & `kss-6.0.0.dev0/kss/_modules/josa/josa.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/josa/utils.py` & `kss-6.0.0.dev0/kss/_modules/josa/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/keywords/extract_keywords.py` & `kss-6.0.0.dev0/kss/_modules/keywords/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/keywords/utils.py` & `kss-6.0.0.dev0/kss/_modules/keywords/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/morphemes/analyzers.py` & `kss-6.0.0.dev0/kss/_modules/morphemes/analyzers.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/morphemes/split_morphemes.py` & `kss-6.0.0.dev0/kss/_modules/morphemes/split_morphemes.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/morphemes/utils.py` & `kss-6.0.0.dev0/kss/_modules/morphemes/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/paradigm/paradigm.py` & `kss-6.0.0.dev0/kss/_modules/paradigm/paradigm.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/preprocessing/anonymize.py` & `kss-6.0.0.dev0/kss/_modules/preprocessing/anonymize.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     bitcoin_replacement: str = "<BITCOIN>",
     url_replacement: str = "<URL>",
     ip_v6_replacement: str = "<IPV6>",
     ip_v4_replacement: str = "<IPV4>",
     num_workers: Union[int, str] = "auto",
 ):
     """
-    Anonymize sensitive information in the given text.
+    This anonymizes sensitive information in the given text.
 
     Args:
         text (Union[str, List[str], Tuple[str]): single text or list of texts
         phone_number_anonymization (bool): whether to anonymize phone numbers or not
         rrn_anonymization (bool): whether to anonymize resident registration numbers or not
         card_anonymization (bool): whether to anonymize card numbers or not
         email_anonymization (bool): whether to anonymize email addresses or not
```

### Comparing `kss-6.0.0/kss/_modules/preprocessing/clean_news.py` & `kss-6.0.0.dev0/kss/_modules/preprocessing/clean_news.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
     min_sentences: int = 3,
     header_ratio: float = 0.4,
     footer_ratio: float = 0.4,
     num_workers: Union[int, str] = "auto",
     verbose: bool = False,
 ) -> Union[str, List[str]]:
     """
-    Clean news articles by removing useless headers and footers.
+    This cleans news articles by removing useless headers and footers.
 
     Args:
         text (Union[str, List[str], Tuple[str]]): Input text or list of texts.
         min_sentences (int): Minimum number of sentences to keep. Defaults to 3.
         header_ratio (float): Ratio of the number of sentences to check in the header. Defaults to 0.4.
         footer_ratio (float): Ratio of the number of sentences to check in the footer. Defaults to 0.4.
         num_workers (Union[int, str]): the number of multiprocessing workers
```

### Comparing `kss-6.0.0/kss/_modules/preprocessing/completed_form.py` & `kss-6.0.0.dev0/kss/_modules/preprocessing/completed_form.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,18 +64,18 @@
         if _is_completed_form(chr(i)):
             completed_form.append(chr(i))
     return completed_form
 
 
 def get_all_incompleted_form_hangul_chars():
     """
-    This returns all non-completed form Hangul characters.
+    This returns all incompleted form Hangul characters.
 
     Returns:
-        List[str]: all non-completed form Hangul characters
+        List[str]: all incompleted form Hangul characters
 
     Examples:
         >>> from kss import Kss
         >>> get_all_incompleted_form_hangul_chars = Kss("get_all_incompleted_form_hangul_chars")
         >>> output = get_all_incompleted_form_hangul_chars()
         >>> print(output)
         ['갂', '갃', '갅', '갆', '갋', '갌', '갍', '갎', '갏', '갘', '갞', '갟', '갡', '갢', '갣', '갥', '갦', '갧', '갨', '갩', '갪', '갫', '갮', '갲', '갳', '갴', '갵', '갶', '갷', '갺', '갻', '갽', '갾', '갿', '걁', '걂', '걃', '걄', '걅', '걆', '걇', '걈', '걉', '걊', '걌', '걎', '걏', '걐', '걑', '걒', '걓', '걕', '걖', '걗', '걙', '걚', '걛', '걝', '걞', '걟', '걠', '걡', '걢', '걣', '걤', '걥', '걦', '걧', '걨', '걩', '걪', '걫', '걬', '걭', '걮', '걯', '걲', '걳', '걵', '걶', '걹', '걻', '걼', '걽', '걾', '걿', '겂', '겇', '겈', '겍', '겎', '겏', '겑', '겒', '겓', '겕', '겖', '겗', '겘', '겙', '겚', '겛', '겞', '겢', '겣', '겤', '겥', '겦', '겧', '겫', '겭', '겮', '겱', '겲', '겳', '겴', '겵', '겶', '겷', '겺', '겾', '겿', '곀', '곂', '곃', '곅', '곆', '곇', '곉', '곊', '곋', '곍', '곎', '곏', '곐', '곑', '곒', '곓', '곔', '곖', '곘', '곙', '곚', '곛', '곜', '곝', '곞', '곟', '곢', '곣', '곥', '곦', '곩', '곫', '곭', '곮', '곲', '곴', '곷', '곸', '곹', '곺', '곻', '곾', '곿', '괁', '괂', '괃', '괅', '괇', '괈', '괉', '괊', '괋', '괎', '괐', '괒', '괓', '괔', '괕', '괖', '괗', '괙', '괚', '괛', '괝', '괞', '괟', '괡', '괢', '괣', '괤', '괥', '괦', '괧', '괨', '괪', '괫', '괮', '괯', '괰', '괱', '괲', '괳', '괶', '괷', '괹', '괺', '괻', '괽', '괾', '괿', '굀', '굁', '굂', '굃', '굆', '굈', '굊', '굋', '굌', '굍', '굎', '굏', '굑', '굒', '굓', '굕', '굖', '굗', '굙', '굚', '굛', '굜', '굝', '굞', '굟', '굠', '굢', '굤', '굥', '굦', '굧', '굨', '굩', '굪', '굫', '굮', '굯', '굱', '굲', '굷', '굸', '굹', '굺', '굾', '궀', '궃', '궄', '궅', '궆', '궇', '궊', '궋', '궍', '궎', '궏', '궑', '궒', '궓', '궔', '궕', '궖', '궗', '궘', '궙', '궚', '궛', '궞', '궟', '궠', '궡', '궢', '궣', '궥', '궦', '궧', '궨', '궩', '궪', '궫', '궬', '궭', '궮', '궯', '궰', '궱', '궲', '궳', '궴', '궵', '궶', '궸', '궹', '궺', '궻', '궼', '궽', '궾', '궿', '귂', '귃', '귅', '귆', '귇', '귉', '귊', '귋', '귌', '귍', '귎', '귏', '귒', '귔', '귕', '귖', '귗', '귘', '귙', '귚', '귛', '귝', '귞', '귟', '귡', '귢', '귣', '귥', '귦', '귧', '귨', '귩', '귪', '귫', '귬', '귭', '귮', '귯', '귰', '귱', '귲', '귳', '귴', '귵', '귶', '귷', '귺', '귻', '귽', '귾', '긂', '긃', '긄', '긅', '긆', '긇', '긊', '긌', '긎', '긏', '긐', '긑', '긒', '긓', '긕', '긖', '긗', '긘', '긙', '긚', '긛', '긜', '긝', '긞', '긟', '긠', '긡', '긢', '긣', '긤', '긥', '긦', '긧', '긨', '긩', '긪', '긫', '긬', '긭', '긮', '긯', '긲', '긳', '긵', '긶', '긹', '긻', '긼', '긽', '긾', '긿', '깂', '깄', '깇', '깈', '깉', '깋', '깏', '깑', '깒', '깓', '깕', '깗', '깘', '깙', '깚', '깛', '깞', '깢', '깣', '깤', '깦', '깧', '깪', '깫', '깭', '깮', '깯', '깱', '깲', '깳', '깴', '깵', '깶', '깷', '깺', '깾', '깿', '꺀', '꺁', '꺂', '꺃', '꺆', '꺇', '꺈', '꺉', '꺊', '꺋', '꺍', '꺎', '꺏', '꺐', '꺑', '꺒', '꺓', '꺔', '꺕', '꺖', '꺗', '꺘', '꺙', '꺚', '꺛', '꺜', '꺝', '꺞', '꺟', '꺠', '꺡', '꺢', '꺣', '꺤', '꺥', '꺦', '꺧', '꺨', '꺩', '꺪', '꺫', '꺬', '꺭', '꺮', '꺯', '꺰', '꺱', '꺲', '꺳', '꺴', '꺵', '꺶', '꺷', '꺸', '꺹', '꺺', '꺻', '꺿', '껁', '껂', '껃', '껅', '껆', '껇', '껈', '껉', '껊', '껋', '껎', '껒', '껓', '껔', '껕', '껖', '껗', '껚', '껛', '껝', '껞', '껟', '껠', '껡', '껢', '껣', '껤', '껥', '껦', '껧', '껩', '껪', '껬', '껮', '껯', '껰', '껱', '껲', '껳', '껵', '껶', '껷', '껹', '껺', '껻', '껽', '껾', '껿', '꼀', '꼁', '꼂', '꼃', '꼄', '꼅', '꼆', '꼉', '꼊', '꼋', '꼌', '꼎', '꼏', '꼑', '꼒', '꼓', '꼔', '꼕', '꼖', '꼗', '꼘', '꼙', '꼚', '꼛', '꼜', '꼝', '꼞', '꼟', '꼠', '꼡', '꼢', '꼣', '꼤', '꼥', '꼦', '꼧', '꼨', '꼩', '꼪', '꼫', '꼮', '꼯', '꼱', '꼳', '꼵', '꼶', '꼷', '꼸', '꼹', '꼺', '꼻', '꼾', '꽀', '꽄', '꽅', '꽆', '꽇', '꽊', '꽋', '꽌', '꽍', '꽎', '꽏', '꽑', '꽒', '꽓', '꽔', '꽕', '꽖', '꽗', '꽘', '꽙', '꽚', '꽛', '꽞', '꽟', '꽠', '꽡', '꽢', '꽣', '꽦', '꽧', '꽨', '꽩', '꽪', '꽫', '꽬', '꽭', '꽮', '꽯', '꽰', '꽱', '꽲', '꽳', '꽴', '꽵', '꽶', '꽷', '꽸', '꽺', '꽻', '꽼', '꽽', '꽾', '꽿', '꾁', '꾂', '꾃', '꾅', '꾆', '꾇', '꾉', '꾊', '꾋', '꾌', '꾍', '꾎', '꾏', '꾒', '꾓', '꾔', '꾖', '꾗', '꾘', '꾙', '꾚', '꾛', '꾝', '꾞', '꾟', '꾠', '꾡', '꾢', '꾣', '꾤', '꾥', '꾦', '꾧', '꾨', '꾩', '꾪', '꾫', '꾬', '꾭', '꾮', '꾯', '꾰', '꾱', '꾲', '꾳', '꾴', '꾵', '꾶', '꾷', '꾺', '꾻', '꾽', '꾾', '꾿', '꿁', '꿂', '꿃', '꿄', '꿅', '꿆', '꿊', '꿌', '꿏', '꿐', '꿑', '꿒', '꿓', '꿕', '꿖', '꿗', '꿘', '꿙', '꿚', '꿛', '꿝', '꿞', '꿟', '꿠', '꿡', '꿢', '꿣', '꿤', '꿥', '꿦', '꿧', '꿪', '꿫', '꿬', '꿭', '꿮', '꿯', '꿲', '꿳', '꿵', '꿶', '꿷', '꿹', '꿺', '꿻', '꿼', '꿽', '꿾', '꿿', '뀂', '뀃', '뀅', '뀆', '뀇', '뀈', '뀉', '뀊', '뀋', '뀍', '뀎', '뀏', '뀑', '뀒', '뀓', '뀕', '뀖', '뀗', '뀘', '뀙', '뀚', '뀛', '뀞', '뀟', '뀠', '뀡', '뀢', '뀣', '뀤', '뀥', '뀦', '뀧', '뀩', '뀪', '뀫', '뀬', '뀭', '뀮', '뀯', '뀰', '뀱', '뀲', '뀳', '뀴', '뀵', '뀶', '뀷', '뀸', '뀹', '뀺', '뀻', '뀼', '뀽', '뀾', '뀿', '끀', '끁', '끂', '끃', '끆', '끇', '끉', '끋', '끍', '끏', '끐', '끑', '끒', '끖', '끘', '끚', '끛', '끜', '끞', '끟', '끠', '끡', '끢', '끣', '끤', '끥', '끦', '끧', '끨', '끩', '끪', '끫', '끬', '끭', '끮', '끯', '끰', '끱', '끲', '끳', '끴', '끵', '끶', '끷', '끸', '끹', '끺', '끻', '끾', '끿', '낁', '낂', '낃', '낅', '낆', '낇', '낈', '낉', '낊', '낋', '낎', '낐', '낒', '낓', '낔', '낕', '낖', '낗', '낛', '낝', '낞', '낣', '낤', '낥', '낦', '낧', '낪', '낰', '낲', '낶', '낷', '낹', '낺', '낻', '낽', '낾', '낿', '냀', '냁', '냂', '냃', '냆', '냊', '냋', '냌', '냍', '냎', '냏', '냒', '냓', '냕', '냖', '냗', '냙', '냚', '냛', '냜', '냝', '냞', '냟', '냡', '냢', '냣', '냤', '냦', '냧', '냨', '냩', '냪', '냫', '냬', '냭', '냮', '냯', '냰', '냱', '냲', '냳', '냴', '냵', '냶', '냷', '냸', '냹', '냺', '냻', '냼', '냽', '냾', '냿', '넀', '넁', '넂', '넃', '넄', '넅', '넆', '넇', '넊', '넍', '넎', '넏', '넑', '넔', '넕', '넖', '넗', '넚', '넞', '넟', '넠', '넡', '넢', '넦', '넧', '넩', '넪', '넫', '넭', '넮', '넯', '넰', '넱', '넲', '넳', '넶', '넺', '넻', '넼', '넽', '넾', '넿', '녂', '녃', '녅', '녆', '녇', '녉', '녊', '녋', '녌', '녍', '녎', '녏', '녒', '녓', '녖', '녗', '녙', '녚', '녛', '녝', '녞', '녟', '녡', '녢', '녣', '녤', '녥', '녦', '녧', '녨', '녩', '녪', '녫', '녬', '녭', '녮', '녯', '녰', '녱', '녲', '녳', '녴', '녵', '녶', '녷', '녺', '녻', '녽', '녾', '녿', '놁', '놃', '놄', '놅', '놆', '놇', '놊', '놌', '놎', '놏', '놐', '놑', '놕', '놖', '놗', '놙', '놚', '놛', '놝', '놞', '놟', '놠', '놡', '놢', '놣', '놤', '놥', '놦', '놧', '놩', '놪', '놫', '놬', '놭', '놮', '놯', '놰', '놱', '놲', '놳', '놴', '놵', '놶', '놷', '놸', '놹', '놺', '놻', '놼', '놽', '놾', '놿', '뇀', '뇁', '뇂', '뇃', '뇄', '뇅', '뇆', '뇇', '뇈', '뇉', '뇊', '뇋', '뇍', '뇎', '뇏', '뇑', '뇒', '뇓', '뇕', '뇖', '뇗', '뇘', '뇙', '뇚', '뇛', '뇞', '뇠', '뇡', '뇢', '뇣', '뇤', '뇥', '뇦', '뇧', '뇪', '뇫', '뇭', '뇮', '뇯', '뇱', '뇲', '뇳', '뇴', '뇵', '뇶', '뇷', '뇸', '뇺', '뇼', '뇾', '뇿', '눀', '눁', '눂', '눃', '눆', '눇', '눉', '눊', '눍', '눎', '눏', '눐', '눑', '눒', '눓', '눖', '눘', '눚', '눛', '눜', '눝', '눞', '눟', '눡', '눢', '눣', '눤', '눥', '눦', '눧', '눨', '눩', '눪', '눫', '눬', '눭', '눮', '눯', '눰', '눱', '눲', '눳', '눵', '눶', '눷', '눸', '눹', '눺', '눻', '눽', '눾', '눿', '뉀', '뉁', '뉂', '뉃', '뉄', '뉅', '뉆', '뉇', '뉈', '뉉', '뉊', '뉋', '뉌', '뉍', '뉎', '뉏', '뉐', '뉑', '뉒', '뉓', '뉔', '뉕', '뉖', '뉗', '뉙', '뉚', '뉛', '뉝', '뉞', '뉟', '뉡', '뉢', '뉣', '뉤', '뉥', '뉦', '뉧', '뉪', '뉫', '뉬', '뉭', '뉮', '뉯', '뉰', '뉱', '뉲', '뉳', '뉶', '뉷', '뉸', '뉹', '뉺', '뉻', '뉽', '뉾', '뉿', '늀', '늁', '늂', '늃', '늆', '늇', '늈', '늊', '늋', '늌', '늍', '늎', '늏', '늒', '늓', '늕', '늖', '늗', '늛', '늜', '늝', '늞', '늟', '늢', '늤', '늧', '늨', '늩', '늫', '늭', '늮', '늯', '늱', '늲', '늳', '늵', '늶', '늷', '늸', '늹', '늺', '늻', '늼', '늽', '늾', '늿', '닀', '닁', '닂', '닃', '닄', '닅', '닆', '닇', '닊', '닋', '닍', '닎', '닏', '닑', '닓', '닔', '닕', '닖', '닗', '닚', '닜', '닞', '닟', '닠', '닡', '닣', '닧', '닩', '닪', '닰', '닱', '닲', '닶', '닼', '닽', '닾', '댂', '댃', '댅', '댆', '댇', '댉', '댊', '댋', '댌', '댍', '댎', '댏', '댒', '댖', '댗', '댘', '댙', '댚', '댛', '댝', '댞', '댟', '댠', '댡', '댢', '댣', '댤', '댥', '댦', '댧', '댨', '댩', '댪', '댫', '댬', '댭', '댮', '댯', '댰', '댱', '댲', '댳', '댴', '댵', '댶', '댷', '댸', '댹', '댺', '댻', '댼', '댽', '댾', '댿', '덀', '덁', '덂', '덃', '덄', '덅', '덆', '덇', '덈', '덉', '덊', '덋', '덌', '덍', '덎', '덏', '덐', '덑', '덒', '덓', '덗', '덙', '덚', '덝', '덠', '덡', '덢', '덣', '덦', '덨', '덪', '덬', '덭', '덯', '덲', '덳', '덵', '덶', '덷', '덹', '덺', '덻', '덼', '덽', '덾', '덿', '뎂', '뎆', '뎇', '뎈', '뎉', '뎊', '뎋', '뎍', '뎎', '뎏', '뎑', '뎒', '뎓', '뎕', '뎖', '뎗', '뎘', '뎙', '뎚', '뎛', '뎜', '뎝', '뎞', '뎟', '뎢', '뎣', '뎤', '뎥', '뎦', '뎧', '뎩', '뎪', '뎫', '뎭', '뎮', '뎯', '뎰', '뎱', '뎲', '뎳', '뎴', '뎵', '뎶', '뎷', '뎸', '뎹', '뎺', '뎻', '뎼', '뎽', '뎾', '뎿', '돀', '돁', '돂', '돃', '돆', '돇', '돉', '돊', '돍', '돏', '돑', '돒', '돓', '돖', '돘', '돚', '돜', '돞', '돟', '돡', '돢', '돣', '돥', '돦', '돧', '돩', '돪', '돫', '돬', '돭', '돮', '돯', '돰', '돱', '돲', '돳', '돴', '돵', '돶', '돷', '돸', '돹', '돺', '돻', '돽', '돾', '돿', '됀', '됁', '됂', '됃', '됄', '됅', '됆', '됇', '됈', '됉', '됊', '됋', '됌', '됍', '됎', '됏', '됑', '됒', '됓', '됔', '됕', '됖', '됗', '됙', '됚', '됛', '됝', '됞', '됟', '됡', '됢', '됣', '됤', '됥', '됦', '됧', '됪', '됬', '됭', '됮', '됯', '됰', '됱', '됲', '됳', '됵', '됶', '됷', '됸', '됹', '됺', '됻', '됼', '됽', '됾', '됿', '둀', '둁', '둂', '둃', '둄', '둅', '둆', '둇', '둈', '둉', '둊', '둋', '둌', '둍', '둎', '둏', '둒', '둓', '둕', '둖', '둗', '둙', '둚', '둛', '둜', '둝', '둞', '둟', '둢', '둤', '둦', '둧', '둨', '둩', '둪', '둫', '둭', '둮', '둯', '둰', '둱', '둲', '둳', '둴', '둵', '둶', '둷', '둸', '둹', '둺', '둻', '둼', '둽', '둾', '둿', '뒁', '뒂', '뒃', '뒄', '뒅', '뒆', '뒇', '뒉', '뒊', '뒋', '뒌', '뒍', '뒎', '뒏', '뒐', '뒑', '뒒', '뒓', '뒔', '뒕', '뒖', '뒗', '뒘', '뒙', '뒚', '뒛', '뒜', '뒞', '뒟', '뒠', '뒡', '뒢', '뒣', '뒥', '뒦', '뒧', '뒩', '뒪', '뒫', '뒭', '뒮', '뒯', '뒰', '뒱', '뒲', '뒳', '뒴', '뒶', '뒸', '뒺', '뒻', '뒼', '뒽', '뒾', '뒿', '듁', '듂', '듃', '듅', '듆', '듇', '듉', '듊', '듋', '듌', '듍', '듎', '듏', '듑', '듒', '듓', '듔', '듖', '듗', '듘', '듙', '듚', '듛', '듞', '듟', '듡', '듢', '듥', '듧', '듨', '듩', '듪', '듫', '듮', '듰', '듲', '듳', '듴', '듵', '듶', '듷', '듹', '듺', '듻', '듼', '듽', '듾', '듿', '딀', '딁', '딂', '딃', '딄', '딅', '딆', '딇', '딈', '딉', '딊', '딋', '딌', '딍', '딎', '딏', '딐', '딑', '딒', '딓', '딖', '딗', '딙', '딚', '딝', '딞', '딟', '딠', '딡', '딢', '딣', '딦', '딫', '딬', '딭', '딮', '딯', '딲', '딳', '딵', '딶', '딷', '딹', '딺', '딻', '딼', '딽', '딾', '딿', '땂', '땆', '땇', '땈', '땉', '땊', '땎', '땏', '땑', '땒', '땓', '땕', '땖', '땗', '땘', '땙', '땚', '땛', '땞', '땢', '땣', '땤', '땥', '땦', '땧', '땨', '땩', '땪', '땫', '땬', '땭', '땮', '땯', '땰', '땱', '땲', '땳', '땴', '땵', '땶', '땷', '땸', '땹', '땺', '땻', '땼', '땽', '땾', '땿', '떀', '떁', '떂', '떃', '떄', '떅', '떆', '떇', '떈', '떉', '떊', '떋', '떌', '떍', '떎', '떏', '떐', '떑', '떒', '떓', '떔', '떕', '떖', '떗', '떘', '떙', '떚', '떛', '떜', '떝', '떞', '떟', '떢', '떣', '떥', '떦', '떧', '떩', '떬', '떭', '떮', '떯', '떲', '떶', '떷', '떸', '떹', '떺', '떾', '떿', '뗁', '뗂', '뗃', '뗅', '뗆', '뗇', '뗈', '뗉', '뗊', '뗋', '뗎', '뗒', '뗓', '뗔', '뗕', '뗖', '뗗', '뗙', '뗚', '뗛', '뗜', '뗝', '뗞', '뗟', '뗠', '뗡', '뗢', '뗣', '뗤', '뗥', '뗦', '뗧', '뗨', '뗩', '뗪', '뗫', '뗭', '뗮', '뗯', '뗰', '뗱', '뗲', '뗳', '뗴', '뗵', '뗶', '뗷', '뗸', '뗹', '뗺', '뗻', '뗼', '뗽', '뗾', '뗿', '똀', '똁', '똂', '똃', '똄', '똅', '똆', '똇', '똈', '똉', '똊', '똋', '똌', '똍', '똎', '똏', '똒', '똓', '똕', '똖', '똗', '똙', '똚', '똛', '똜', '똝', '똞', '똟', '똠', '똡', '똢', '똣', '똤', '똦', '똧', '똨', '똩', '똪', '똫', '똭', '똮', '똯', '똰', '똱', '똲', '똳', '똵', '똶', '똷', '똸', '똹', '똺', '똻', '똼', '똽', '똾', '똿', '뙀', '뙁', '뙂', '뙃', '뙄', '뙅', '뙆', '뙇', '뙉', '뙊', '뙋', '뙌', '뙍', '뙎', '뙏', '뙐', '뙑', '뙒', '뙓', '뙔', '뙕', '뙖', '뙗', '뙘', '뙙', '뙚', '뙛', '뙜', '뙝', '뙞', '뙟', '뙠', '뙡', '뙢', '뙣', '뙥', '뙦', '뙧', '뙩', '뙪', '뙫', '뙬', '뙭', '뙮', '뙯', '뙰', '뙱', '뙲', '뙳', '뙴', '뙵', '뙶', '뙷', '뙸', '뙹', '뙺', '뙻', '뙼', '뙽', '뙾', '뙿', '뚀', '뚁', '뚂', '뚃', '뚄', '뚅', '뚆', '뚇', '뚈', '뚉', '뚊', '뚋', '뚌', '뚍', '뚎', '뚏', '뚐', '뚑', '뚒', '뚓', '뚔', '뚕', '뚖', '뚗', '뚘', '뚙', '뚚', '뚛', '뚞', '뚟', '뚡', '뚢', '뚣', '뚥', '뚦', '뚧', '뚨', '뚩', '뚪', '뚭', '뚮', '뚯', '뚰', '뚲', '뚳', '뚴', '뚵', '뚶', '뚷', '뚸', '뚹', '뚺', '뚻', '뚼', '뚽', '뚾', '뚿', '뛀', '뛁', '뛂', '뛃', '뛄', '뛅', '뛆', '뛇', '뛈', '뛉', '뛊', '뛋', '뛌', '뛍', '뛎', '뛏', '뛐', '뛑', '뛒', '뛓', '뛕', '뛖', '뛗', '뛘', '뛙', '뛚', '뛛', '뛜', '뛝', '뛞', '뛟', '뛠', '뛡', '뛢', '뛣', '뛤', '뛥', '뛦', '뛧', '뛨', '뛩', '뛪', '뛫', '뛬', '뛭', '뛮', '뛯', '뛱', '뛲', '뛳', '뛵', '뛶', '뛷', '뛹', '뛺', '뛻', '뛼', '뛽', '뛾', '뛿', '뜂', '뜃', '뜄', '뜆', '뜇', '뜈', '뜉', '뜊', '뜋', '뜌', '뜍', '뜎', '뜏', '뜐', '뜑', '뜒', '뜓', '뜔', '뜕', '뜖', '뜗', '뜘', '뜙', '뜚', '뜛', '뜜', '뜝', '뜞', '뜟', '뜠', '뜡', '뜢', '뜣', '뜤', '뜥', '뜦', '뜧', '뜪', '뜫', '뜭', '뜮', '뜱', '뜲', '뜳', '뜴', '뜵', '뜶', '뜷', '뜺', '뜼', '뜽', '뜾', '뜿', '띀', '띁', '띂', '띃', '띅', '띆', '띇', '띉', '띊', '띋', '띍', '띎', '띏', '띐', '띑', '띒', '띓', '띖', '띗', '띘', '띙', '띚', '띛', '띜', '띝', '띞', '띟', '띡', '띢', '띣', '띥', '띦', '띧', '띩', '띪', '띫', '띬', '띭', '띮', '띯', '띲', '띴', '띶', '띷', '띸', '띹', '띺', '띻', '띾', '띿', '랁', '랂', '랃', '랅', '랆', '랇', '랈', '랉', '랊', '랋', '랎', '랓', '랔', '랕', '랚', '랛', '랝', '랞', '랟', '랡', '랢', '랣', '랤', '랥', '랦', '랧', '랪', '랮', '랯', '랰', '랱', '랲', '랳', '랶', '랷', '랹', '랺', '랻', '랼', '랽', '랾', '랿', '럀', '럁', '럂', '럃', '럄', '럅', '럆', '럈', '럊', '럋', '럌', '럍', '럎', '럏', '럐', '럑', '럒', '럓', '럔', '럕', '럖', '럗', '럘', '럙', '럚', '럛', '럜', '럝', '럞', '럟', '럠', '럡', '럢', '럣', '럤', '럥', '럦', '럧', '럨', '럩', '럪', '럫', '럮', '럯', '럱', '럲', '럳', '럵', '럶', '럷', '럸', '럹', '럺', '럻', '럾', '렂', '렃', '렄', '렅', '렆', '렊', '렋', '렍', '렎', '렏', '렑', '렒', '렓', '렔', '렕', '렖', '렗', '렚', '렜', '렞', '렟', '렠', '렡', '렢', '렣', '렦', '렧', '렩', '렪', '렫', '렭', '렮', '렯', '렰', '렱', '렲', '렳', '렶', '렺', '렻', '렼', '렽', '렾', '렿', '롁', '롂', '롃', '롅', '롆', '롇', '롈', '롉', '롊', '롋', '롌', '롍', '롎', '롏', '롐', '롒', '롔', '롕', '롖', '롗', '롘', '롙', '롚', '롛', '롞', '롟', '롡', '롢', '롣', '롥', '롦', '롧', '롨', '롩', '롪', '롫', '롮', '롰', '롲', '롳', '롴', '롵', '롶', '롷', '롹', '롺', '롻', '롽', '롾', '롿', '뢀', '뢁', '뢂', '뢃', '뢄', '뢅', '뢆', '뢇', '뢈', '뢉', '뢊', '뢋', '뢌', '뢎', '뢏', '뢐', '뢑', '뢒', '뢓', '뢔', '뢕', '뢖', '뢗', '뢘', '뢙', '뢚', '뢛', '뢜', '뢝', '뢞', '뢟', '뢠', '뢡', '뢢', '뢣', '뢤', '뢥', '뢦', '뢧', '뢩', '뢪', '뢫', '뢬', '뢭', '뢮', '뢯', '뢱', '뢲', '뢳', '뢵', '뢶', '뢷', '뢹', '뢺', '뢻', '뢼', '뢽', '뢾', '뢿', '룂', '룄', '룆', '룇', '룈', '룉', '룊', '룋', '룍', '룎', '룏', '룑', '룒', '룓', '룕', '룖', '룗', '룘', '룙', '룚', '룛', '룜', '룞', '룠', '룢', '룣', '룤', '룥', '룦', '룧', '룪', '룫', '룭', '룮', '룯', '룱', '룲', '룳', '룴', '룵', '룶', '룷', '룺', '룼', '룾', '룿', '뤀', '뤁', '뤂', '뤃', '뤅', '뤆', '뤇', '뤈', '뤉', '뤊', '뤋', '뤌', '뤍', '뤎', '뤏', '뤐', '뤑', '뤒', '뤓', '뤔', '뤕', '뤖', '뤗', '뤙', '뤚', '뤛', '뤜', '뤝', '뤞', '뤟', '뤡', '뤢', '뤣', '뤤', '뤥', '뤦', '뤧', '뤨', '뤩', '뤪', '뤫', '뤬', '뤭', '뤮', '뤯', '뤰', '뤱', '뤲', '뤳', '뤴', '뤵', '뤶', '뤷', '뤸', '뤹', '뤺', '뤻', '뤾', '뤿', '륁', '륂', '륃', '륅', '륆', '륇', '륈', '륉', '륊', '륋', '륍', '륎', '륐', '륒', '륓', '륔', '륕', '륖', '륗', '륚', '륛', '륝', '륞', '륟', '륡', '륢', '륣', '륤', '륥', '륦', '륧', '륪', '륬', '륮', '륯', '륰', '륱', '륲', '륳', '륶', '륷', '륹', '륺', '륻', '륽', '륾', '륿', '릀', '릁', '릂', '릃', '릆', '릈', '릋', '릌', '릏', '릐', '릑', '릒', '릓', '릔', '릕', '릖', '릗', '릘', '릙', '릚', '릛', '릜', '릝', '릞', '릟', '릠', '릡', '릢', '릣', '릤', '릥', '릦', '릧', '릨', '릩', '릪', '릫', '릮', '릯', '릱', '릲', '릳', '릵', '릶', '릷', '릸', '릹', '릺', '릻', '릾', '맀', '맂', '맃', '맄', '맅', '맆', '맇', '맊', '맋', '맍', '맓', '맔', '맕', '맖', '맗', '맚', '맜', '맟', '맠', '맢', '맦', '맧', '맩', '맪', '맫', '맭', '맮', '맯', '맰', '맱', '맲', '맳', '맶', '맻', '맼', '맽', '맾', '맿', '먂', '먃', '먄', '먅', '먆', '먇', '먉', '먊', '먋', '먌', '먍', '먎', '먏', '먐', '먑', '먒', '먓', '먔', '먖', '먗', '먘', '먙', '먚', '먛', '먜', '먝', '먞', '먟', '먠', '먡', '먢', '먣', '먤', '먥', '먦', '먧', '먨', '먩', '먪', '먫', '먬', '먭', '먮', '먯', '먰', '먱', '먲', '먳', '먴', '먵', '먶', '먷', '먺', '먻', '먽', '먾', '먿', '멁', '멃', '멄', '멅', '멆', '멇', '멊', '멌', '멏', '멐', '멑', '멒', '멖', '멗', '멙', '멚', '멛', '멝', '멞', '멟', '멠', '멡', '멢', '멣', '멦', '멪', '멫', '멬', '멭', '멮', '멯', '멲', '멳', '멵', '멶', '멷', '멹', '멺', '멻', '멼', '멽', '멾', '멿', '몀', '몁', '몂', '몆', '몈', '몉', '몊', '몋', '몍', '몎', '몏', '몐', '몑', '몒', '몓', '몔', '몕', '몖', '몗', '몘', '몙', '몚', '몛', '몜', '몝', '몞', '몟', '몠', '몡', '몢', '몣', '몤', '몥', '몦', '몧', '몪', '몭', '몮', '몯', '몱', '몳', '몴', '몵', '몶', '몷', '몺', '몼', '몾', '몿', '뫀', '뫁', '뫂', '뫃', '뫅', '뫆', '뫇', '뫉', '뫊', '뫋', '뫌', '뫍', '뫎', '뫏', '뫐', '뫑', '뫒', '뫓', '뫔', '뫕', '뫖', '뫗', '뫚', '뫛', '뫜', '뫝', '뫞', '뫟', '뫠', '뫡', '뫢', '뫣', '뫤', '뫥', '뫦', '뫧', '뫨', '뫩', '뫪', '뫫', '뫬', '뫭', '뫮', '뫯', '뫰', '뫱', '뫲', '뫳', '뫴', '뫵', '뫶', '뫷', '뫸', '뫹', '뫺', '뫻', '뫽', '뫾', '뫿', '묁', '묂', '묃', '묅', '묆', '묇', '묈', '묉', '묊', '묋', '묌', '묎', '묐', '묒', '묓', '묔', '묕', '묖', '묗', '묙', '묚', '묛', '묝', '묞', '묟', '묡', '묢', '묣', '묤', '묥', '묦', '묧', '묨', '묪', '묬', '묭', '묮', '묯', '묰', '묱', '묲', '묳', '묷', '묹', '묺', '묿', '뭀', '뭁', '뭂', '뭃', '뭆', '뭈', '뭊', '뭋', '뭌', '뭎', '뭑', '뭒', '뭓', '뭕', '뭖', '뭗', '뭙', '뭚', '뭛', '뭜', '뭝', '뭞', '뭟', '뭠', '뭢', '뭤', '뭥', '뭦', '뭧', '뭨', '뭩', '뭪', '뭫', '뭭', '뭮', '뭯', '뭰', '뭱', '뭲', '뭳', '뭴', '뭵', '뭶', '뭷', '뭸', '뭹', '뭺', '뭻', '뭼', '뭽', '뭾', '뭿', '뮀', '뮁', '뮂', '뮃', '뮄', '뮅', '뮆', '뮇', '뮉', '뮊', '뮋', '뮍', '뮎', '뮏', '뮑', '뮒', '뮓', '뮔', '뮕', '뮖', '뮗', '뮘', '뮙', '뮚', '뮛', '뮜', '뮝', '뮞', '뮟', '뮠', '뮡', '뮢', '뮣', '뮥', '뮦', '뮧', '뮩', '뮪', '뮫', '뮭', '뮮', '뮯', '뮰', '뮱', '뮲', '뮳', '뮵', '뮶', '뮸', '뮹', '뮺', '뮻', '뮼', '뮽', '뮾', '뮿', '믁', '믂', '믃', '믅', '믆', '믇', '믉', '믊', '믋', '믌', '믍', '믎', '믏', '믑', '믒', '믔', '믕', '믖', '믗', '믘', '믙', '믚', '믛', '믜', '믝', '믞', '믟', '믠', '믡', '믢', '믣', '믤', '믥', '믦', '믧', '믨', '믩', '믪', '믫', '믬', '믭', '믮', '믯', '믰', '믱', '믲', '믳', '믴', '믵', '믶', '믷', '믺', '믻', '믽', '믾', '밁', '밃', '밄', '밅', '밆', '밇', '밊', '밎', '밐', '밒', '밓', '밙', '밚', '밠', '밡', '밢', '밣', '밦', '밨', '밪', '밫', '밬', '밮', '밯', '밲', '밳', '밵', '밶', '밷', '밹', '밺', '밻', '밼', '밽', '밾', '밿', '뱂', '뱆', '뱇', '뱈', '뱊', '뱋', '뱎', '뱏', '뱑', '뱒', '뱓', '뱔', '뱕', '뱖', '뱗', '뱘', '뱙', '뱚', '뱛', '뱜', '뱞', '뱟', '뱠', '뱡', '뱢', '뱣', '뱤', '뱥', '뱦', '뱧', '뱨', '뱩', '뱪', '뱫', '뱬', '뱭', '뱮', '뱯', '뱰', '뱱', '뱲', '뱳', '뱴', '뱵', '뱶', '뱷', '뱸', '뱹', '뱺', '뱻', '뱼', '뱽', '뱾', '뱿', '벀', '벁', '벂', '벃', '벆', '벇', '벉', '벊', '벍', '벏', '벐', '벑', '벒', '벓', '벖', '벘', '벛', '벜', '벝', '벞', '벟', '벢', '벣', '벥', '벦', '벩', '벪', '벫', '벬', '벭', '벮', '벯', '벲', '벶', '벷', '벸', '벹', '벺', '벻', '벾', '벿', '볁', '볂', '볃', '볅', '볆', '볇', '볈', '볉', '볊', '볋', '볌', '볎', '볒', '볓', '볔', '볖', '볗', '볙', '볚', '볛', '볝', '볞', '볟', '볠', '볡', '볢', '볣', '볤', '볥', '볦', '볧', '볨', '볩', '볪', '볫', '볬', '볭', '볮', '볯', '볰', '볱', '볲', '볳', '볷', '볹', '볺', '볻', '볽', '볾', '볿', '봀', '봁', '봂', '봃', '봆', '봈', '봊', '봋', '봌', '봍', '봎', '봏', '봑', '봒', '봓', '봕', '봖', '봗', '봘', '봙', '봚', '봛', '봜', '봝', '봞', '봟', '봠', '봡', '봢', '봣', '봥', '봦', '봧', '봨', '봩', '봪', '봫', '봭', '봮', '봯', '봰', '봱', '봲', '봳', '봴', '봵', '봶', '봷', '봸', '봹', '봺', '봻', '봼', '봽', '봾', '봿', '뵁', '뵂', '뵃', '뵄', '뵅', '뵆', '뵇', '뵊', '뵋', '뵍', '뵎', '뵏', '뵑', '뵒', '뵓', '뵔', '뵕', '뵖', '뵗', '뵚', '뵛', '뵜', '뵝', '뵞', '뵟', '뵠', '뵡', '뵢', '뵣', '뵥', '뵦', '뵧', '뵩', '뵪', '뵫', '뵬', '뵭', '뵮', '뵯', '뵰', '뵱', '뵲', '뵳', '뵴', '뵵', '뵶', '뵷', '뵸', '뵹', '뵺', '뵻', '뵼', '뵽', '뵾', '뵿', '붂', '붃', '붅', '붆', '붋', '붌', '붍', '붎', '붏', '붒', '붔', '붖', '붗', '붘', '붛', '붝', '붞', '붟', '붠', '붡', '붢', '붣', '붥', '붦', '붧', '붨', '붩', '붪', '붫', '붬', '붭', '붮', '붯', '붱', '붲', '붳', '붴', '붵', '붶', '붷', '붹', '붺', '붻', '붼', '붽', '붾', '붿', '뷀', '뷁', '뷂', '뷃', '뷄', '뷅', '뷆', '뷇', '뷈', '뷉', '뷊', '뷋', '뷌', '뷍', '뷎', '뷏', '뷐', '뷑', '뷒', '뷓', '뷖', '뷗', '뷙', '뷚', '뷛', '뷝', '뷞', '뷟', '뷠', '뷡', '뷢', '뷣', '뷤', '뷥', '뷦', '뷧', '뷨', '뷪', '뷫', '뷬', '뷭', '뷮', '뷯', '뷱', '뷲', '뷳', '뷵', '뷶', '뷷', '뷹', '뷺', '뷻', '뷼', '뷽', '뷾', '뷿', '븁', '븂', '븄', '븆', '븇', '븈', '븉', '븊', '븋', '븎', '븏', '븑', '븒', '븓', '븕', '븖', '븗', '븘', '븙', '븚', '븛', '븞', '븠', '븡', '븢', '븣', '븤', '븥', '븦', '븧', '븨', '븩', '븪', '븫', '븬', '븭', '븮', '븯', '븰', '븱', '븲', '븳', '븴', '븵', '븶', '븷', '븸', '븹', '븺', '븻', '븼', '븽', '븾', '븿', '빀', '빁', '빂', '빃', '빆', '빇', '빉', '빊', '빋', '빍', '빏', '빐', '빑', '빒', '빓', '빖', '빘', '빜', '빝', '빞', '빟', '빢', '빣', '빥', '빦', '빧', '빩', '빫', '빬', '빭', '빮', '빯', '빲', '빶', '빷', '빸', '빹', '빺', '빾', '빿', '뺁', '뺂', '뺃', '뺅', '뺆', '뺇', '뺈', '뺉', '뺊', '뺋', '뺎', '뺒', '뺓', '뺔', '뺕', '뺖', '뺗', '뺚', '뺛', '뺜', '뺝', '뺞', '뺟', '뺠', '뺡', '뺢', '뺣', '뺤', '뺥', '뺦', '뺧', '뺩', '뺪', '뺫', '뺬', '뺭', '뺮', '뺯', '뺰', '뺱', '뺲', '뺳', '뺴', '뺵', '뺶', '뺷', '뺸', '뺹', '뺺', '뺻', '뺼', '뺽', '뺾', '뺿', '뻀', '뻁', '뻂', '뻃', '뻄', '뻅', '뻆', '뻇', '뻈', '뻉', '뻊', '뻋', '뻌', '뻍', '뻎', '뻏', '뻒', '뻓', '뻕', '뻖', '뻙', '뻚', '뻛', '뻜', '뻝', '뻞', '뻟', '뻡', '뻢', '뻦', '뻧', '뻨', '뻩', '뻪', '뻫', '뻭', '뻮', '뻯', '뻰', '뻱', '뻲', '뻳', '뻴', '뻵', '뻶', '뻷', '뻸', '뻹', '뻺', '뻻', '뻼', '뻽', '뻾', '뻿', '뼀', '뼂', '뼃', '뼄', '뼅', '뼆', '뼇', '뼊', '뼋', '뼌', '뼍', '뼎', '뼏', '뼐', '뼑', '뼒', '뼓', '뼔', '뼕', '뼖', '뼗', '뼚', '뼞', '뼟', '뼠', '뼡', '뼢', '뼣', '뼤', '뼥', '뼦', '뼧', '뼨', '뼩', '뼪', '뼫', '뼬', '뼭', '뼮', '뼯', '뼰', '뼱', '뼲', '뼳', '뼴', '뼵', '뼶', '뼷', '뼸', '뼹', '뼺', '뼻', '뼼', '뼽', '뼾', '뼿', '뽂', '뽃', '뽅', '뽆', '뽇', '뽉', '뽊', '뽋', '뽌', '뽍', '뽎', '뽏', '뽒', '뽓', '뽔', '뽖', '뽗', '뽘', '뽙', '뽚', '뽛', '뽜', '뽝', '뽞', '뽟', '뽠', '뽡', '뽢', '뽣', '뽤', '뽥', '뽦', '뽧', '뽨', '뽩', '뽪', '뽫', '뽬', '뽭', '뽮', '뽯', '뽰', '뽱', '뽲', '뽳', '뽴', '뽵', '뽶', '뽷', '뽸', '뽹', '뽺', '뽻', '뽼', '뽽', '뽾', '뽿', '뾀', '뾁', '뾂', '뾃', '뾄', '뾅', '뾆', '뾇', '뾈', '뾉', '뾊', '뾋', '뾌', '뾍', '뾎', '뾏', '뾐', '뾑', '뾒', '뾓', '뾕', '뾖', '뾗', '뾘', '뾙', '뾚', '뾛', '뾜', '뾝', '뾞', '뾟', '뾠', '뾡', '뾢', '뾣', '뾤', '뾥', '뾦', '뾧', '뾨', '뾩', '뾪', '뾫', '뾬', '뾭', '뾮', '뾯', '뾱', '뾲', '뾳', '뾴', '뾵', '뾶', '뾷', '뾸', '뾹', '뾺', '뾻', '뾼', '뾽', '뾾', '뾿', '뿀', '뿁', '뿂', '뿃', '뿄', '뿆', '뿇', '뿈', '뿉', '뿊', '뿋', '뿎', '뿏', '뿑', '뿒', '뿓', '뿕', '뿖', '뿗', '뿘', '뿙', '뿚', '뿛', '뿝', '뿞', '뿠', '뿢', '뿣', '뿤', '뿥', '뿦', '뿧', '뿨', '뿩', '뿪', '뿫', '뿬', '뿭', '뿮', '뿯', '뿰', '뿱', '뿲', '뿳', '뿴', '뿵', '뿶', '뿷', '뿸', '뿹', '뿺', '뿻', '뿼', '뿽', '뿾', '뿿', '쀀', '쀁', '쀂', '쀃', '쀄', '쀅', '쀆', '쀇', '쀈', '쀉', '쀊', '쀋', '쀌', '쀍', '쀎', '쀏', '쀐', '쀑', '쀒', '쀓', '쀔', '쀕', '쀖', '쀗', '쀘', '쀙', '쀚', '쀛', '쀜', '쀝', '쀞', '쀟', '쀠', '쀡', '쀢', '쀣', '쀤', '쀥', '쀦', '쀧', '쀨', '쀩', '쀪', '쀫', '쀬', '쀭', '쀮', '쀯', '쀰', '쀱', '쀲', '쀳', '쀴', '쀵', '쀶', '쀷', '쀸', '쀹', '쀺', '쀻', '쀽', '쀾', '쀿', '쁀', '쁁', '쁂', '쁃', '쁄', '쁅', '쁆', '쁇', '쁈', '쁉', '쁊', '쁋', '쁌', '쁍', '쁎', '쁏', '쁐', '쁒', '쁓', '쁔', '쁕', '쁖', '쁗', '쁙', '쁚', '쁛', '쁝', '쁞', '쁟', '쁡', '쁢', '쁣', '쁤', '쁥', '쁦', '쁧', '쁪', '쁫', '쁬', '쁭', '쁮', '쁯', '쁰', '쁱', '쁲', '쁳', '쁴', '쁵', '쁶', '쁷', '쁸', '쁹', '쁺', '쁻', '쁼', '쁽', '쁾', '쁿', '삀', '삁', '삂', '삃', '삄', '삅', '삆', '삇', '삈', '삉', '삊', '삋', '삌', '삍', '삎', '삏', '삒', '삓', '삕', '삖', '삗', '삙', '삚', '삛', '삜', '삝', '삞', '삟', '삢', '삤', '삦', '삧', '삨', '삩', '삪', '삫', '삮', '삱', '삲', '삷', '삸', '삹', '삺', '삻', '삾', '샂', '샃', '샄', '샆', '샇', '샊', '샋', '샍', '샎', '샏', '샑', '샒', '샓', '샔', '샕', '샖', '샗', '샚', '샞', '샟', '샠', '샡', '샢', '샣', '샦', '샧', '샩', '샪', '샫', '샭', '샮', '샯', '샰', '샱', '샲', '샳', '샶', '샸', '샺', '샻', '샼', '샽', '샾', '샿', '섁', '섂', '섃', '섅', '섆', '섇', '섉', '섊', '섋', '섌', '섍', '섎', '섏', '섑', '섒', '섓', '섔', '섖', '섗', '섘', '섙', '섚', '섛', '섡', '섢', '섥', '섨', '섩', '섪', '섫', '섮', '섲', '섳', '섴', '섵', '섷', '섺', '섻', '섽', '섾', '섿', '셁', '셂', '셃', '셄', '셅', '셆', '셇', '셊', '셎', '셏', '셐', '셑', '셒', '셓', '셖', '셗', '셙', '셚', '셛', '셝', '셞', '셟', '셠', '셡', '셢', '셣', '셦', '셪', '셫', '셬', '셭', '셮', '셯', '셱', '셲', '셳', '셵', '셶', '셷', '셹', '셺', '셻', '셼', '셽', '셾', '셿', '솀', '솁', '솂', '솃', '솄', '솆', '솇', '솈', '솉', '솊', '솋', '솏', '솑', '솒', '솓', '솕', '솗', '솘', '솙', '솚', '솛', '솞', '솠', '솢', '솣', '솤', '솦', '솧', '솪', '솫', '솭', '솮', '솯', '솱', '솲', '솳', '솴', '솵', '솶', '솷', '솸', '솹', '솺', '솻', '솼', '솾', '솿', '쇀', '쇁', '쇂', '쇃', '쇅', '쇆', '쇇', '쇉', '쇊', '쇋', '쇍', '쇎', '쇏', '쇐', '쇑', '쇒', '쇓', '쇕', '쇖', '쇙', '쇚', '쇛', '쇜', '쇝', '쇞', '쇟', '쇡', '쇢', '쇣', '쇥', '쇦', '쇧', '쇩', '쇪', '쇫', '쇬', '쇭', '쇮', '쇯', '쇲', '쇴', '쇵', '쇶', '쇷', '쇸', '쇹', '쇺', '쇻', '쇾', '쇿', '숁', '숂', '숃', '숅', '숆', '숇', '숈', '숉', '숊', '숋', '숎', '숐', '숒', '숓', '숔', '숕', '숖', '숗', '숚', '숛', '숝', '숞', '숡', '숢', '숣', '숤', '숥', '숦', '숧', '숪', '숬', '숮', '숰', '숳', '숵', '숶', '숷', '숸', '숹', '숺', '숻', '숼', '숽', '숾', '숿', '쉀', '쉁', '쉂', '쉃', '쉄', '쉅', '쉆', '쉇', '쉉', '쉊', '쉋', '쉌', '쉍', '쉎', '쉏', '쉒', '쉓', '쉕', '쉖', '쉗', '쉙', '쉚', '쉛', '쉜', '쉝', '쉞', '쉟', '쉡', '쉢', '쉣', '쉤', '쉦', '쉧', '쉨', '쉩', '쉪', '쉫', '쉮', '쉯', '쉱', '쉲', '쉳', '쉵', '쉶', '쉷', '쉸', '쉹', '쉺', '쉻', '쉾', '슀', '슂', '슃', '슄', '슅', '슆', '슇', '슊', '슋', '슌', '슍', '슎', '슏', '슑', '슒', '슓', '슔', '슕', '슖', '슗', '슙', '슚', '슜', '슞', '슟', '슠', '슡', '슢', '슣', '슦', '슧', '슩', '슪', '슫', '슮', '슯', '슰', '슱', '슲', '슳', '슶', '슸', '슺', '슻', '슼', '슽', '슾', '슿', '싀', '싁', '싂', '싃', '싄', '싅', '싆', '싇', '싈', '싉', '싊', '싋', '싌', '싍', '싎', '싏', '싐', '싑', '싒', '싓', '싔', '싕', '싖', '싗', '싘', '싙', '싚', '싛', '싞', '싟', '싡', '싢', '싥', '싦', '싧', '싨', '싩', '싪', '싮', '싰', '싲', '싳', '싴', '싵', '싷', '싺', '싽', '싾', '싿', '쌁', '쌂', '쌃', '쌄', '쌅', '쌆', '쌇', '쌊', '쌋', '쌎', '쌏', '쌐', '쌑', '쌒', '쌖', '쌗', '쌙', '쌚', '쌛', '쌝', '쌞', '쌟', '쌠', '쌡', '쌢', '쌣', '쌦', '쌧', '쌪', '쌫', '쌬', '쌭', '쌮', '쌯', '쌰', '쌱', '쌲', '쌳', '쌴', '쌵', '쌶', '쌷', '쌸', '쌹', '쌺', '쌻', '쌼', '쌽', '쌾', '쌿', '썀', '썁', '썂', '썃', '썄', '썆', '썇', '썈', '썉', '썊', '썋', '썌', '썍', '썎', '썏', '썐', '썑', '썒', '썓', '썔', '썕', '썖', '썗', '썘', '썙', '썚', '썛', '썜', '썝', '썞', '썟', '썠', '썡', '썢', '썣', '썤', '썥', '썦', '썧', '썪', '썫', '썭', '썮', '썯', '썱', '썳', '썴', '썵', '썶', '썷', '썺', '썻', '썾', '썿', '쎀', '쎁', '쎂', '쎃', '쎅', '쎆', '쎇', '쎉', '쎊', '쎋', '쎍', '쎎', '쎏', '쎐', '쎑', '쎒', '쎓', '쎔', '쎕', '쎖', '쎗', '쎘', '쎙', '쎚', '쎛', '쎜', '쎝', '쎞', '쎟', '쎠', '쎡', '쎢', '쎣', '쎤', '쎥', '쎦', '쎧', '쎨', '쎩', '쎪', '쎫', '쎬', '쎭', '쎮', '쎯', '쎰', '쎱', '쎲', '쎳', '쎴', '쎵', '쎶', '쎷', '쎸', '쎹', '쎺', '쎻', '쎼', '쎽', '쎾', '쎿', '쏁', '쏂', '쏃', '쏄', '쏅', '쏆', '쏇', '쏈', '쏉', '쏊', '쏋', '쏌', '쏍', '쏎', '쏏', '쏐', '쏑', '쏒', '쏓', '쏔', '쏕', '쏖', '쏗', '쏚', '쏛', '쏝', '쏞', '쏡', '쏣', '쏤', '쏥', '쏦', '쏧', '쏪', '쏫', '쏬', '쏮', '쏯', '쏰', '쏱', '쏲', '쏳', '쏶', '쏷', '쏹', '쏺', '쏻', '쏼', '쏽', '쏾', '쏿', '쐀', '쐁', '쐂', '쐃', '쐄', '쐅', '쐆', '쐇', '쐉', '쐊', '쐋', '쐌', '쐍', '쐎', '쐏', '쐑', '쐒', '쐓', '쐔', '쐕', '쐖', '쐗', '쐘', '쐙', '쐚', '쐛', '쐜', '쐝', '쐞', '쐟', '쐠', '쐡', '쐢', '쐣', '쐥', '쐦', '쐧', '쐨', '쐩', '쐪', '쐫', '쐭', '쐮', '쐯', '쐱', '쐲', '쐳', '쐵', '쐶', '쐷', '쐸', '쐹', '쐺', '쐻', '쐾', '쐿', '쑀', '쑁', '쑂', '쑃', '쑄', '쑅', '쑆', '쑇', '쑉', '쑊', '쑋', '쑌', '쑍', '쑎', '쑏', '쑐', '쑑', '쑒', '쑓', '쑔', '쑕', '쑖', '쑗', '쑘', '쑙', '쑚', '쑛', '쑜', '쑝', '쑞', '쑟', '쑠', '쑡', '쑢', '쑣', '쑦', '쑧', '쑩', '쑪', '쑫', '쑭', '쑮', '쑯', '쑰', '쑱', '쑲', '쑳', '쑶', '쑷', '쑸', '쑺', '쑻', '쑼', '쑽', '쑾', '쑿', '쒁', '쒂', '쒃', '쒄', '쒅', '쒆', '쒇', '쒈', '쒉', '쒊', '쒋', '쒌', '쒍', '쒎', '쒏', '쒐', '쒑', '쒒', '쒓', '쒕', '쒖', '쒗', '쒘', '쒙', '쒚', '쒛', '쒝', '쒞', '쒟', '쒠', '쒡', '쒢', '쒣', '쒤', '쒥', '쒦', '쒧', '쒨', '쒩', '쒪', '쒫', '쒬', '쒭', '쒮', '쒯', '쒰', '쒱', '쒲', '쒳', '쒴', '쒵', '쒶', '쒷', '쒹', '쒺', '쒻', '쒽', '쒾', '쒿', '쓀', '쓁', '쓂', '쓃', '쓄', '쓅', '쓆', '쓇', '쓈', '쓉', '쓊', '쓋', '쓌', '쓍', '쓎', '쓏', '쓐', '쓑', '쓒', '쓓', '쓔', '쓕', '쓖', '쓗', '쓘', '쓙', '쓚', '쓛', '쓜', '쓝', '쓞', '쓟', '쓠', '쓡', '쓢', '쓣', '쓤', '쓥', '쓦', '쓧', '쓨', '쓪', '쓫', '쓬', '쓭', '쓮', '쓯', '쓲', '쓳', '쓵', '쓶', '쓷', '쓹', '쓻', '쓼', '쓽', '쓾', '씂', '씃', '씄', '씅', '씆', '씇', '씈', '씉', '씊', '씋', '씍', '씎', '씏', '씑', '씒', '씓', '씕', '씖', '씗', '씘', '씙', '씚', '씛', '씝', '씞', '씟', '씠', '씡', '씢', '씣', '씤', '씥', '씦', '씧', '씪', '씫', '씭', '씮', '씯', '씱', '씲', '씳', '씴', '씵', '씶', '씷', '씺', '씼', '씾', '씿', '앀', '앁', '앂', '앃', '앆', '앇', '앋', '앏', '앐', '앑', '앒', '앖', '앚', '앛', '앜', '앟', '앢', '앣', '앥', '앦', '앧', '앩', '앪', '앫', '앬', '앭', '앮', '앯', '앲', '앶', '앷', '앸', '앹', '앺', '앻', '앾', '앿', '얁', '얂', '얃', '얅', '얆', '얈', '얉', '얊', '얋', '얎', '얐', '얒', '얓', '얔', '얖', '얙', '얚', '얛', '얝', '얞', '얟', '얡', '얢', '얣', '얤', '얥', '얦', '얧', '얨', '얪', '얫', '얬', '얭', '얮', '얯', '얰', '얱', '얲', '얳', '얶', '얷', '얺', '얿', '엀', '엁', '엂', '엃', '엋', '엍', '엏', '엒', '엓', '엕', '엖', '엗', '엙', '엚', '엛', '엜', '엝', '엞', '엟', '엢', '엤', '엦', '엧', '엨', '엩', '엪', '엫', '엯', '엱', '엲', '엳', '엵', '엸', '엹', '엺', '엻', '옂', '옃', '옄', '옉', '옊', '옋', '옍', '옎', '옏', '옑', '옒', '옓', '옔', '옕', '옖', '옗', '옚', '옝', '옞', '옟', '옠', '옡', '옢', '옣', '옦', '옧', '옩', '옪', '옫', '옯', '옱', '옲', '옶', '옸', '옺', '옼', '옽', '옾', '옿', '왂', '왃', '왅', '왆', '왇', '왉', '왊', '왋', '왌', '왍', '왎', '왏', '왒', '왖', '왗', '왘', '왙', '왚', '왛', '왞', '왟', '왡', '왢', '왣', '왤', '왥', '왦', '왧', '왨', '왩', '왪', '왫', '왭', '왮', '왰', '왲', '왳', '왴', '왵', '왶', '왷', '왺', '왻', '왽', '왾', '왿', '욁', '욂', '욃', '욄', '욅', '욆', '욇', '욊', '욌', '욎', '욏', '욐', '욑', '욒', '욓', '욖', '욗', '욙', '욚', '욛', '욝', '욞', '욟', '욠', '욡', '욢', '욣', '욦', '욨', '욪', '욫', '욬', '욭', '욮', '욯', '욲', '욳', '욵', '욶', '욷', '욻', '욼', '욽', '욾', '욿', '웂', '웄', '웆', '웇', '웈', '웉', '웊', '웋', '웎', '웏', '웑', '웒', '웓', '웕', '웖', '웗', '웘', '웙', '웚', '웛', '웞', '웟', '웢', '웣', '웤', '웥', '웦', '웧', '웪', '웫', '웭', '웮', '웯', '웱', '웲', '웳', '웴', '웵', '웶', '웷', '웺', '웻', '웼', '웾', '웿', '윀', '윁', '윂', '윃', '윆', '윇', '윉', '윊', '윋', '윍', '윎', '윏', '윐', '윑', '윒', '윓', '윖', '윘', '윚', '윛', '윜', '윝', '윞', '윟', '윢', '윣', '윥', '윦', '윧', '윩', '윪', '윫', '윬', '윭', '윮', '윯', '윲', '윴', '윶', '윸', '윹', '윺', '윻', '윾', '윿', '읁', '읂', '읃', '읅', '읆', '읇', '읈', '읉', '읋', '읎', '읐', '읙', '읚', '읛', '읝', '읞', '읟', '읡', '읢', '읣', '읤', '읥', '읦', '읧', '읩', '읪', '읬', '읭', '읮', '읯', '읰', '읱', '읲', '읳', '읶', '읷', '읹', '읺', '읻', '읿', '잀', '잁', '잂', '잆', '잋', '잌', '잍', '잏', '잒', '잓', '잕', '잙', '잛', '잜', '잝', '잞', '잟', '잢', '잧', '잨', '잩', '잪', '잫', '잮', '잯', '잱', '잲', '잳', '잵', '잶', '잷', '잸', '잹', '잺', '잻', '잾', '쟂', '쟃', '쟄', '쟅', '쟆', '쟇', '쟊', '쟋', '쟍', '쟏', '쟑', '쟒', '쟓', '쟔', '쟕', '쟖', '쟗', '쟙', '쟚', '쟛', '쟜', '쟞', '쟟', '쟠', '쟡', '쟢', '쟣', '쟥', '쟦', '쟧', '쟩', '쟪', '쟫', '쟭', '쟮', '쟯', '쟰', '쟱', '쟲', '쟳', '쟴', '쟵', '쟶', '쟷', '쟸', '쟹', '쟺', '쟻', '쟼', '쟽', '쟾', '쟿', '젂', '젃', '젅', '젆', '젇', '젉', '젋', '젌', '젍', '젎', '젏', '젒', '젔', '젗', '젘', '젙', '젚', '젛', '젞', '젟', '젡', '젢', '젣', '젥', '젦', '젧', '젨', '젩', '젪', '젫', '젮', '젰', '젲', '젳', '젴', '젵', '젶', '젷', '젹', '젺', '젻', '젽', '젾', '젿', '졁', '졂', '졃', '졄', '졅', '졆', '졇', '졊', '졋', '졎', '졏', '졐', '졑', '졒', '졓', '졕', '졖', '졗', '졘', '졙', '졚', '졛', '졜', '졝', '졞', '졟', '졠', '졡', '졢', '졣', '졤', '졥', '졦', '졧', '졨', '졩', '졪', '졫', '졬', '졭', '졮', '졯', '졲', '졳', '졵', '졶', '졷', '졹', '졻', '졼', '졽', '졾', '졿', '좂', '좄', '좈', '좉', '좊', '좎', '좏', '좐', '좑', '좒', '좓', '좕', '좖', '좗', '좘', '좙', '좚', '좛', '좜', '좞', '좠', '좢', '좣', '좤', '좥', '좦', '좧', '좩', '좪', '좫', '좬', '좭', '좮', '좯', '좰', '좱', '좲', '좳', '좴', '좵', '좶', '좷', '좸', '좹', '좺', '좻', '좾', '좿', '죀', '죁', '죂', '죃', '죅', '죆', '죇', '죉', '죊', '죋', '죍', '죎', '죏', '죐', '죑', '죒', '죓', '죖', '죘', '죚', '죛', '죜', '죝', '죞', '죟', '죢', '죣', '죥', '죦', '죧', '죨', '죩', '죪', '죫', '죬', '죭', '죮', '죯', '죰', '죱', '죲', '죳', '죴', '죶', '죷', '죸', '죹', '죺', '죻', '죾', '죿', '줁', '줂', '줃', '줇', '줈', '줉', '줊', '줋', '줎', '줐', '줒', '줓', '줔', '줕', '줖', '줗', '줙', '줚', '줛', '줜', '줝', '줞', '줟', '줠', '줡', '줢', '줣', '줤', '줥', '줦', '줧', '줨', '줩', '줪', '줫', '줭', '줮', '줯', '줰', '줱', '줲', '줳', '줵', '줶', '줷', '줸', '줹', '줺', '줻', '줼', '줽', '줾', '줿', '쥀', '쥁', '쥂', '쥃', '쥄', '쥅', '쥆', '쥇', '쥈', '쥉', '쥊', '쥋', '쥌', '쥍', '쥎', '쥏', '쥒', '쥓', '쥕', '쥖', '쥗', '쥙', '쥚', '쥛', '쥜', '쥝', '쥞', '쥟', '쥢', '쥤', '쥥', '쥦', '쥧', '쥨', '쥩', '쥪', '쥫', '쥭', '쥮', '쥯', '쥱', '쥲', '쥳', '쥵', '쥶', '쥷', '쥸', '쥹', '쥺', '쥻', '쥽', '쥾', '쥿', '즀', '즁', '즂', '즃', '즄', '즅', '즆', '즇', '즊', '즋', '즍', '즎', '즏', '즑', '즒', '즓', '즔', '즕', '즖', '즗', '즚', '즜', '즞', '즟', '즠', '즡', '즢', '즣', '즤', '즥', '즦', '즧', '즨', '즩', '즪', '즫', '즬', '즭', '즮', '즯', '즰', '즱', '즲', '즳', '즴', '즵', '즶', '즷', '즸', '즹', '즺', '즻', '즼', '즽', '즾', '즿', '짂', '짃', '짅', '짆', '짉', '짋', '짌', '짍', '짎', '짏', '짒', '짔', '짗', '짘', '짛', '짞', '짟', '짡', '짣', '짥', '짦', '짨', '짩', '짪', '짫', '짮', '짲', '짳', '짴', '짵', '짶', '짷', '짺', '짻', '짽', '짾', '짿', '쨁', '쨂', '쨃', '쨄', '쨅', '쨆', '쨇', '쨊', '쨎', '쨏', '쨐', '쨑', '쨒', '쨓', '쨕', '쨖', '쨗', '쨙', '쨚', '쨛', '쨜', '쨝', '쨞', '쨟', '쨠', '쨡', '쨢', '쨣', '쨤', '쨥', '쨦', '쨧', '쨨', '쨪', '쨫', '쨬', '쨭', '쨮', '쨯', '쨰', '쨱', '쨲', '쨳', '쨴', '쨵', '쨶', '쨷', '쨸', '쨹', '쨺', '쨻', '쨼', '쨽', '쨾', '쨿', '쩀', '쩁', '쩂', '쩃', '쩄', '쩅', '쩆', '쩇', '쩈', '쩉', '쩊', '쩋', '쩎', '쩏', '쩑', '쩒', '쩓', '쩕', '쩖', '쩗', '쩘', '쩙', '쩚', '쩛', '쩞', '쩢', '쩣', '쩤', '쩥', '쩦', '쩧', '쩩', '쩪', '쩫', '쩬', '쩭', '쩮', '쩯', '쩰', '쩱', '쩲', '쩳', '쩴', '쩵', '쩶', '쩷', '쩸', '쩹', '쩺', '쩻', '쩼', '쩾', '쩿', '쪀', '쪁', '쪂', '쪃', '쪅', '쪆', '쪇', '쪈', '쪉', '쪊', '쪋', '쪌', '쪍', '쪎', '쪏', '쪐', '쪑', '쪒', '쪓', '쪔', '쪕', '쪖', '쪗', '쪙', '쪚', '쪛', '쪜', '쪝', '쪞', '쪟', '쪠', '쪡', '쪢', '쪣', '쪤', '쪥', '쪦', '쪧', '쪨', '쪩', '쪪', '쪫', '쪬', '쪭', '쪮', '쪯', '쪰', '쪱', '쪲', '쪳', '쪴', '쪵', '쪶', '쪷', '쪸', '쪹', '쪺', '쪻', '쪾', '쪿', '쫁', '쫂', '쫃', '쫅', '쫆', '쫇', '쫈', '쫉', '쫊', '쫋', '쫎', '쫐', '쫒', '쫔', '쫕', '쫖', '쫗', '쫚', '쫛', '쫜', '쫝', '쫞', '쫟', '쫡', '쫢', '쫣', '쫤', '쫥', '쫦', '쫧', '쫨', '쫩', '쫪', '쫫', '쫭', '쫮', '쫯', '쫰', '쫱', '쫲', '쫳', '쫵', '쫶', '쫷', '쫸', '쫹', '쫺', '쫻', '쫼', '쫽', '쫾', '쫿', '쬀', '쬁', '쬂', '쬃', '쬄', '쬅', '쬆', '쬇', '쬉', '쬊', '쬋', '쬌', '쬍', '쬎', '쬏', '쬑', '쬒', '쬓', '쬕', '쬖', '쬗', '쬙', '쬚', '쬛', '쬜', '쬝', '쬞', '쬟', '쬢', '쬣', '쬤', '쬥', '쬦', '쬧', '쬨', '쬩', '쬪', '쬫', '쬬', '쬭', '쬮', '쬯', '쬰', '쬱', '쬲', '쬳', '쬴', '쬵', '쬶', '쬷', '쬸', '쬹', '쬺', '쬻', '쬼', '쬽', '쬾', '쬿', '쭀', '쭂', '쭃', '쭄', '쭅', '쭆', '쭇', '쭊', '쭋', '쭍', '쭎', '쭏', '쭑', '쭒', '쭓', '쭔', '쭕', '쭖', '쭗', '쭚', '쭛', '쭜', '쭞', '쭟', '쭠', '쭡', '쭢', '쭣', '쭥', '쭦', '쭧', '쭨', '쭩', '쭪', '쭫', '쭬', '쭭', '쭮', '쭯', '쭰', '쭱', '쭲', '쭳', '쭴', '쭵', '쭶', '쭷', '쭺', '쭻', '쭼', '쭽', '쭾', '쭿', '쮀', '쮁', '쮂', '쮃', '쮄', '쮅', '쮆', '쮇', '쮈', '쮉', '쮊', '쮋', '쮌', '쮍', '쮎', '쮏', '쮐', '쮑', '쮒', '쮓', '쮔', '쮕', '쮖', '쮗', '쮘', '쮙', '쮚', '쮛', '쮝', '쮞', '쮟', '쮠', '쮡', '쮢', '쮣', '쮤', '쮥', '쮦', '쮧', '쮨', '쮩', '쮪', '쮫', '쮬', '쮭', '쮮', '쮯', '쮰', '쮱', '쮲', '쮳', '쮴', '쮵', '쮶', '쮷', '쮹', '쮺', '쮻', '쮼', '쮽', '쮾', '쮿', '쯀', '쯁', '쯂', '쯃', '쯄', '쯅', '쯆', '쯇', '쯈', '쯉', '쯊', '쯋', '쯌', '쯍', '쯎', '쯏', '쯐', '쯑', '쯒', '쯓', '쯕', '쯖', '쯗', '쯘', '쯙', '쯚', '쯛', '쯜', '쯝', '쯞', '쯟', '쯠', '쯡', '쯢', '쯣', '쯥', '쯦', '쯨', '쯪', '쯫', '쯬', '쯭', '쯮', '쯯', '쯰', '쯱', '쯲', '쯳', '쯴', '쯵', '쯶', '쯷', '쯸', '쯹', '쯺', '쯻', '쯼', '쯽', '쯾', '쯿', '찀', '찁', '찂', '찃', '찄', '찅', '찆', '찇', '찈', '찉', '찊', '찋', '찎', '찏', '찑', '찒', '찓', '찕', '찖', '찗', '찘', '찙', '찚', '찛', '찞', '찟', '찠', '찣', '찤', '찥', '찦', '찪', '찫', '찭', '찯', '찱', '찲', '찳', '찴', '찵', '찶', '찷', '찺', '찿', '챀', '챁', '챂', '챃', '챆', '챇', '챉', '챊', '챋', '챍', '챎', '챏', '챐', '챑', '챒', '챓', '챖', '챚', '챛', '챜', '챝', '챞', '챟', '챡', '챢', '챣', '챥', '챧', '챩', '챪', '챫', '챬', '챭', '챮', '챯', '챱', '챲', '챳', '챴', '챶', '챷', '챸', '챹', '챺', '챻', '챼', '챽', '챾', '챿', '첀', '첁', '첂', '첃', '첄', '첅', '첆', '첇', '첈', '첉', '첊', '첋', '첌', '첍', '첎', '첏', '첐', '첑', '첒', '첓', '첔', '첕', '첖', '첗', '첚', '첛', '첝', '첞', '첟', '첡', '첢', '첣', '첤', '첥', '첦', '첧', '첪', '첮', '첯', '첰', '첱', '첲', '첳', '첶', '첷', '첹', '첺', '첻', '첽', '첾', '첿', '쳀', '쳁', '쳂', '쳃', '쳆', '쳈', '쳊', '쳋', '쳌', '쳍', '쳎', '쳏', '쳑', '쳒', '쳓', '쳕', '쳖', '쳗', '쳘', '쳙', '쳚', '쳛', '쳜', '쳝', '쳞', '쳟', '쳠', '쳡', '쳢', '쳣', '쳥', '쳦', '쳧', '쳨', '쳩', '쳪', '쳫', '쳭', '쳮', '쳯', '쳱', '쳲', '쳳', '쳴', '쳵', '쳶', '쳷', '쳸', '쳹', '쳺', '쳻', '쳼', '쳽', '쳾', '쳿', '촀', '촂', '촃', '촄', '촅', '촆', '촇', '촊', '촋', '촍', '촎', '촏', '촑', '촒', '촓', '촔', '촕', '촖', '촗', '촚', '촜', '촞', '촟', '촠', '촡', '촢', '촣', '촥', '촦', '촧', '촩', '촪', '촫', '촭', '촮', '촯', '촰', '촱', '촲', '촳', '촴', '촵', '촶', '촷', '촸', '촺', '촻', '촼', '촽', '촾', '촿', '쵀', '쵁', '쵂', '쵃', '쵄', '쵅', '쵆', '쵇', '쵈', '쵉', '쵊', '쵋', '쵌', '쵍', '쵎', '쵏', '쵐', '쵑', '쵒', '쵓', '쵔', '쵕', '쵖', '쵗', '쵘', '쵙', '쵚', '쵛', '쵝', '쵞', '쵟', '쵡', '쵢', '쵣', '쵥', '쵦', '쵧', '쵨', '쵩', '쵪', '쵫', '쵮', '쵰', '쵲', '쵳', '쵴', '쵵', '쵶', '쵷', '쵹', '쵺', '쵻', '쵼', '쵽', '쵾', '쵿', '춀', '춁', '춂', '춃', '춄', '춅', '춆', '춇', '춉', '춊', '춋', '춌', '춍', '춎', '춏', '춐', '춑', '춒', '춓', '춖', '춗', '춙', '춚', '춛', '춝', '춞', '춟', '춠', '춡', '춢', '춣', '춦', '춨', '춪', '춫', '춬', '춭', '춮', '춯', '춱', '춲', '춳', '춴', '춵', '춶', '춷', '춸', '춹', '춺', '춻', '춼', '춽', '춾', '춿', '췀', '췁', '췂', '췃', '췅', '췆', '췇', '췈', '췉', '췊', '췋', '췍', '췎', '췏', '췑', '췒', '췓', '췔', '췕', '췖', '췗', '췘', '췙', '췚', '췛', '췜', '췝', '췞', '췟', '췠', '췡', '췢', '췣', '췤', '췥', '췦', '췧', '췩', '췪', '췫', '췭', '췮', '췯', '췱', '췲', '췳', '췴', '췵', '췶', '췷', '췺', '췼', '췾', '췿', '츀', '츁', '츂', '츃', '츅', '츆', '츇', '츉', '츊', '츋', '츍', '츎', '츏', '츐', '츑', '츒', '츓', '츕', '츖', '츗', '츘', '츚', '츛', '츜', '츝', '츞', '츟', '츢', '츣', '츥', '츦', '츧', '츩', '츪', '츫', '츬', '츭', '츮', '츯', '츲', '츴', '츶', '츷', '츸', '츹', '츺', '츻', '츼', '츽', '츾', '츿', '칀', '칁', '칂', '칃', '칄', '칅', '칆', '칇', '칈', '칉', '칊', '칋', '칌', '칍', '칎', '칏', '칐', '칑', '칒', '칓', '칔', '칕', '칖', '칗', '칚', '칛', '칝', '칞', '칢', '칣', '칤', '칥', '칦', '칧', '칪', '칬', '칮', '칯', '칰', '칱', '칲', '칳', '칶', '칷', '칹', '칺', '칻', '칽', '칾', '칿', '캀', '캁', '캂', '캃', '캆', '캈', '캊', '캋', '캌', '캍', '캎', '캏', '캒', '캓', '캕', '캖', '캗', '캙', '캚', '캛', '캜', '캝', '캞', '캟', '캢', '캦', '캧', '캨', '캩', '캪', '캫', '캮', '캯', '캰', '캱', '캲', '캳', '캴', '캵', '캶', '캷', '캸', '캹', '캺', '캻', '캼', '캽', '캾', '캿', '컀', '컂', '컃', '컄', '컅', '컆', '컇', '컈', '컉', '컊', '컋', '컌', '컍', '컎', '컏', '컐', '컑', '컒', '컓', '컔', '컕', '컖', '컗', '컘', '컙', '컚', '컛', '컜', '컝', '컞', '컟', '컠', '컡', '컢', '컣', '컦', '컧', '컩', '컪', '컭', '컮', '컯', '컰', '컱', '컲', '컳', '컶', '컺', '컻', '컼', '컽', '컾', '컿', '켂', '켃', '켅', '켆', '켇', '켉', '켊', '켋', '켌', '켍', '켎', '켏', '켒', '켔', '켖', '켗', '켘', '켙', '켚', '켛', '켝', '켞', '켟', '켡', '켢', '켣', '켥', '켦', '켧', '켨', '켩', '켪', '켫', '켮', '켲', '켳', '켴', '켵', '켶', '켷', '켹', '켺', '켻', '켼', '켽', '켾', '켿', '콀', '콁', '콂', '콃', '콄', '콅', '콆', '콇', '콈', '콉', '콊', '콋', '콌', '콍', '콎', '콏', '콐', '콑', '콒', '콓', '콖', '콗', '콙', '콚', '콛', '콝', '콞', '콟', '콠', '콡', '콢', '콣', '콦', '콨', '콪', '콫', '콬', '콭', '콮', '콯', '콲', '콳', '콵', '콶', '콷', '콹', '콺', '콻', '콼', '콽', '콾', '콿', '쾁', '쾂', '쾃', '쾄', '쾆', '쾇', '쾈', '쾉', '쾊', '쾋', '쾍', '쾎', '쾏', '쾐', '쾑', '쾒', '쾓', '쾔', '쾕', '쾖', '쾗', '쾘', '쾙', '쾚', '쾛', '쾜', '쾝', '쾞', '쾟', '쾠', '쾢', '쾣', '쾤', '쾥', '쾦', '쾧', '쾩', '쾪', '쾫', '쾬', '쾭', '쾮', '쾯', '쾱', '쾲', '쾳', '쾴', '쾵', '쾶', '쾷', '쾸', '쾹', '쾺', '쾻', '쾼', '쾽', '쾾', '쾿', '쿀', '쿁', '쿂', '쿃', '쿅', '쿆', '쿇', '쿈', '쿉', '쿊', '쿋', '쿌', '쿍', '쿎', '쿏', '쿐', '쿑', '쿒', '쿓', '쿔', '쿕', '쿖', '쿗', '쿘', '쿙', '쿚', '쿛', '쿜', '쿝', '쿞', '쿟', '쿢', '쿣', '쿥', '쿦', '쿧', '쿩', '쿪', '쿫', '쿬', '쿭', '쿮', '쿯', '쿲', '쿴', '쿶', '쿷', '쿸', '쿹', '쿺', '쿻', '쿽', '쿾', '쿿', '퀁', '퀂', '퀃', '퀅', '퀆', '퀇', '퀈', '퀉', '퀊', '퀋', '퀌', '퀍', '퀎', '퀏', '퀐', '퀒', '퀓', '퀔', '퀕', '퀖', '퀗', '퀙', '퀚', '퀛', '퀜', '퀝', '퀞', '퀟', '퀠', '퀡', '퀢', '퀣', '퀤', '퀥', '퀦', '퀧', '퀨', '퀩', '퀪', '퀫', '퀬', '퀮', '퀯', '퀰', '퀱', '퀲', '퀳', '퀶', '퀷', '퀹', '퀺', '퀻', '퀽', '퀾', '퀿', '큀', '큁', '큂', '큃', '큆', '큈', '큊', '큋', '큌', '큍', '큎', '큏', '큑', '큒', '큓', '큕', '큖', '큗', '큙', '큚', '큛', '큜', '큝', '큞', '큟', '큡', '큢', '큣', '큤', '큥', '큦', '큧', '큨', '큩', '큪', '큫', '큮', '큯', '큱', '큲', '큳', '큵', '큶', '큷', '큸', '큹', '큺', '큻', '큾', '큿', '킀', '킂', '킃', '킄', '킅', '킆', '킇', '킈', '킉', '킊', '킋', '킌', '킍', '킎', '킏', '킐', '킑', '킒', '킓', '킔', '킕', '킖', '킗', '킘', '킙', '킚', '킛', '킜', '킝', '킞', '킟', '킠', '킡', '킢', '킣', '킦', '킧', '킩', '킪', '킫', '킭', '킮', '킯', '킰', '킱', '킲', '킳', '킶', '킸', '킺', '킻', '킼', '킽', '킾', '킿', '탂', '탃', '탅', '탆', '탇', '탊', '탋', '탌', '탍', '탎', '탏', '탒', '탖', '탗', '탘', '탙', '탚', '탛', '탞', '탟', '탡', '탢', '탣', '탥', '탦', '탧', '탨', '탩', '탪', '탫', '탮', '탲', '탳', '탴', '탵', '탶', '탷', '탹', '탺', '탻', '탼', '탽', '탾', '탿', '턀', '턁', '턂', '턃', '턄', '턅', '턆', '턇', '턈', '턉', '턊', '턋', '턌', '턎', '턏', '턐', '턑', '턒', '턓', '턔', '턕', '턖', '턗', '턘', '턙', '턚', '턛', '턜', '턝', '턞', '턟', '턠', '턡', '턢', '턣', '턤', '턥', '턦', '턧', '턨', '턩', '턪', '턫', '턬', '턭', '턮', '턯', '턲', '턳', '턵', '턶', '턷', '턹', '턻', '턼', '턽', '턾', '턿', '텂', '텆', '텇', '텈', '텉', '텊', '텋', '텎', '텏', '텑', '텒', '텓', '텕', '텖', '텗', '텘', '텙', '텚', '텛', '텞', '텠', '텢', '텣', '텤', '텥', '텦', '텧', '텩', '텪', '텫', '텭', '텮', '텯', '텰', '텱', '텲', '텳', '텴', '텵', '텶', '텷', '텸', '텹', '텺', '텻', '텽', '텾', '텿', '톀', '톁', '톂', '톃', '톅', '톆', '톇', '톉', '톊', '톋', '톌', '톍', '톎', '톏', '톐', '톑', '톒', '톓', '톔', '톕', '톖', '톗', '톘', '톙', '톚', '톛', '톜', '톝', '톞', '톟', '톢', '톣', '톥', '톦', '톧', '톩', '톪', '톫', '톬', '톭', '톮', '톯', '톲', '톴', '톶', '톷', '톸', '톹', '톻', '톽', '톾', '톿', '퇁', '퇂', '퇃', '퇄', '퇅', '퇆', '퇇', '퇈', '퇉', '퇊', '퇋', '퇌', '퇍', '퇎', '퇏', '퇐', '퇑', '퇒', '퇓', '퇔', '퇕', '퇖', '퇗', '퇙', '퇚', '퇛', '퇜', '퇝', '퇞', '퇟', '퇠', '퇡', '퇢', '퇣', '퇤', '퇥', '퇦', '퇧', '퇨', '퇩', '퇪', '퇫', '퇬', '퇭', '퇮', '퇯', '퇰', '퇱', '퇲', '퇳', '퇵', '퇶', '퇷', '퇹', '퇺', '퇻', '퇼', '퇽', '퇾', '퇿', '툀', '툁', '툂', '툃', '툄', '툅', '툆', '툈', '툊', '툋', '툌', '툍', '툎', '툏', '툑', '툒', '툓', '툔', '툕', '툖', '툗', '툘', '툙', '툚', '툛', '툜', '툝', '툞', '툟', '툠', '툡', '툢', '툣', '툤', '툥', '툦', '툧', '툨', '툩', '툪', '툫', '툮', '툯', '툱', '툲', '툳', '툵', '툶', '툷', '툸', '툹', '툺', '툻', '툾', '퉀', '퉂', '퉃', '퉄', '퉅', '퉆', '퉇', '퉉', '퉊', '퉋', '퉌', '퉍', '퉎', '퉏', '퉐', '퉑', '퉒', '퉓', '퉔', '퉕', '퉖', '퉗', '퉘', '퉙', '퉚', '퉛', '퉝', '퉞', '퉟', '퉠', '퉡', '퉢', '퉣', '퉥', '퉦', '퉧', '퉨', '퉩', '퉪', '퉫', '퉬', '퉭', '퉮', '퉯', '퉰', '퉱', '퉲', '퉳', '퉴', '퉵', '퉶', '퉷', '퉸', '퉹', '퉺', '퉻', '퉼', '퉽', '퉾', '퉿', '튂', '튃', '튅', '튆', '튇', '튉', '튊', '튋', '튌', '튍', '튎', '튏', '튒', '튓', '튔', '튖', '튗', '튘', '튙', '튚', '튛', '튝', '튞', '튟', '튡', '튢', '튣', '튥', '튦', '튧', '튨', '튩', '튪', '튫', '튭', '튮', '튯', '튰', '튲', '튳', '튴', '튵', '튶', '튷', '튺', '튻', '튽', '튾', '틁', '틃', '틄', '틅', '틆', '틇', '틊', '틌', '틍', '틎', '틏', '틐', '틑', '틒', '틓', '틕', '틖', '틗', '틙', '틚', '틛', '틝', '틞', '틟', '틠', '틡', '틢', '틣', '틦', '틧', '틨', '틩', '틪', '틫', '틬', '틭', '틮', '틯', '틲', '틳', '틵', '틶', '틷', '틹', '틺', '틻', '틼', '틽', '틾', '틿', '팂', '팄', '팆', '팇', '팈', '팉', '팊', '팋', '팏', '팑', '팒', '팓', '팕', '팗', '팘', '팙', '팚', '팛', '팞', '팢', '팣', '팤', '팦', '팧', '팪', '팫', '팭', '팮', '팯', '팱', '팲', '팳', '팴', '팵', '팶', '팷', '팺', '팾', '팿', '퍀', '퍁', '퍂', '퍃', '퍆', '퍇', '퍈', '퍉', '퍊', '퍋', '퍌', '퍍', '퍎', '퍏', '퍐', '퍑', '퍒', '퍓', '퍔', '퍕', '퍖', '퍗', '퍘', '퍙', '퍚', '퍛', '퍜', '퍝', '퍞', '퍟', '퍠', '퍡', '퍢', '퍣', '퍤', '퍥', '퍦', '퍧', '퍨', '퍩', '퍪', '퍫', '퍬', '퍭', '퍮', '퍯', '퍰', '퍱', '퍲', '퍳', '퍴', '퍵', '퍶', '퍷', '퍸', '퍹', '퍺', '퍻', '퍾', '퍿', '펁', '펂', '펃', '펅', '펆', '펇', '펈', '펉', '펊', '펋', '펎', '펒', '펓', '펔', '펕', '펖', '펗', '펚', '펛', '펝', '펞', '펟', '펡', '펢', '펣', '펤', '펥', '펦', '펧', '펪', '펬', '펮', '펯', '펰', '펱', '펲', '펳', '펵', '펶', '펷', '펹', '펺', '펻', '펽', '펾', '펿', '폀', '폁', '폂', '폃', '폆', '폇', '폊', '폋', '폌', '폍', '폎', '폏', '폑', '폒', '폓', '폔', '폕', '폖', '폗', '폙', '폚', '폛', '폜', '폝', '폞', '폟', '폠', '폢', '폤', '폥', '폦', '폧', '폨', '폩', '폪', '폫', '폮', '폯', '폱', '폲', '폳', '폵', '폶', '폷', '폸', '폹', '폺', '폻', '폾', '퐀', '퐂', '퐃', '퐄', '퐅', '퐆', '퐇', '퐉', '퐊', '퐋', '퐌', '퐍', '퐎', '퐏', '퐐', '퐑', '퐒', '퐓', '퐔', '퐕', '퐖', '퐗', '퐘', '퐙', '퐚', '퐛', '퐜', '퐞', '퐟', '퐠', '퐡', '퐢', '퐣', '퐤', '퐥', '퐦', '퐧', '퐨', '퐩', '퐪', '퐫', '퐬', '퐭', '퐮', '퐯', '퐰', '퐱', '퐲', '퐳', '퐴', '퐵', '퐶', '퐷', '퐸', '퐹', '퐺', '퐻', '퐼', '퐽', '퐾', '퐿', '푁', '푂', '푃', '푅', '푆', '푇', '푈', '푉', '푊', '푋', '푌', '푍', '푎', '푏', '푐', '푑', '푒', '푓', '푔', '푕', '푖', '푗', '푘', '푙', '푚', '푛', '푝', '푞', '푟', '푡', '푢', '푣', '푥', '푦', '푧', '푨', '푩', '푪', '푫', '푬', '푮', '푰', '푱', '푲', '푳', '푴', '푵', '푶', '푷', '푺', '푻', '푽', '푾', '풁', '풃', '풄', '풅', '풆', '풇', '풊', '풌', '풎', '풏', '풐', '풑', '풒', '풓', '풕', '풖', '풗', '풘', '풙', '풚', '풛', '풜', '풝', '풞', '풟', '풠', '풡', '풢', '풣', '풤', '풥', '풦', '풧', '풨', '풪', '풫', '풬', '풭', '풮', '풯', '풰', '풱', '풲', '풳', '풴', '풵', '풶', '풷', '풸', '풹', '풺', '풻', '풼', '풽', '풾', '풿', '퓀', '퓁', '퓂', '퓃', '퓄', '퓅', '퓆', '퓇', '퓈', '퓉', '퓊', '퓋', '퓍', '퓎', '퓏', '퓑', '퓒', '퓓', '퓕', '퓖', '퓗', '퓘', '퓙', '퓚', '퓛', '퓝', '퓞', '퓠', '퓡', '퓢', '퓣', '퓤', '퓥', '퓦', '퓧', '퓩', '퓪', '퓫', '퓭', '퓮', '퓯', '퓱', '퓲', '퓳', '퓴', '퓵', '퓶', '퓷', '퓹', '퓺', '퓼', '퓾', '퓿', '픀', '픁', '픂', '픃', '픅', '픆', '픇', '픉', '픊', '픋', '픍', '픎', '픏', '픐', '픑', '픒', '픓', '픖', '픘', '픙', '픚', '픛', '픜', '픝', '픞', '픟', '픠', '픡', '픢', '픣', '픤', '픥', '픦', '픧', '픨', '픩', '픪', '픫', '픬', '픭', '픮', '픯', '픰', '픱', '픲', '픳', '픴', '픵', '픶', '픷', '픸', '픹', '픺', '픻', '픾', '픿', '핁', '핂', '핃', '핅', '핆', '핇', '핈', '핉', '핊', '핋', '핎', '핐', '핒', '핓', '핔', '핕', '핖', '핗', '핚', '핛', '핝', '핞', '핟', '핡', '핢', '핣', '핤', '핦', '핧', '핪', '핬', '핮', '핯', '핰', '핱', '핲', '핳', '핶', '핷', '핹', '핺', '핻', '핽', '핾', '핿', '햀', '햁', '햂', '햃', '햆', '햊', '햋', '햌', '햍', '햎', '햏', '햑', '햒', '햓', '햔', '햕', '햖', '햗', '햘', '햙', '햚', '햛', '햜', '햝', '햞', '햟', '햠', '햡', '햢', '햣', '햤', '햦', '햧', '햨', '햩', '햪', '햫', '햬', '햭', '햮', '햯', '햰', '햱', '햲', '햳', '햴', '햵', '햶', '햷', '햸', '햹', '햺', '햻', '햼', '햽', '햾', '햿', '헀', '헁', '헂', '헃', '헄', '헅', '헆', '헇', '헊', '헋', '헍', '헎', '헏', '헑', '헓', '헔', '헕', '헖', '헗', '헚', '헜', '헞', '헟', '헠', '헡', '헢', '헣', '헦', '헧', '헩', '헪', '헫', '헭', '헮', '헯', '헰', '헱', '헲', '헳', '헶', '헸', '헺', '헻', '헼', '헽', '헾', '헿', '혂', '혃', '혅', '혆', '혇', '혉', '혊', '혋', '혌', '혍', '혎', '혏', '혒', '혖', '혗', '혘', '혙', '혚', '혛', '혝', '혞', '혟', '혡', '혢', '혣', '혥', '혦', '혧', '혨', '혩', '혪', '혫', '혬', '혮', '혯', '혰', '혱', '혲', '혳', '혴', '혵', '혶', '혷', '혺', '혻', '혽', '혾', '혿', '홁', '홂', '홃', '홄', '홆', '홇', '홊', '홌', '홎', '홏', '홐', '홒', '홓', '홖', '홗', '홙', '홚', '홛', '홝', '홞', '홟', '홠', '홡', '홢', '홣', '홤', '홥', '홦', '홨', '홪', '홫', '홬', '홭', '홮', '홯', '홲', '홳', '홵', '홶', '홷', '홸', '홹', '홺', '홻', '홼', '홽', '홾', '홿', '횀', '횁', '횂', '횄', '횆', '횇', '횈', '횉', '횊', '횋', '횎', '횏', '횑', '횒', '횓', '횕', '횖', '횗', '횘', '횙', '횚', '횛', '횜', '횞', '횠', '횢', '횣', '횤', '횥', '횦', '횧', '횩', '횪', '횫', '횭', '횮', '횯', '횱', '횲', '횳', '횴', '횵', '횶', '횷', '횸', '횺', '횼', '횽', '횾', '횿', '훀', '훁', '훂', '훃', '훆', '훇', '훉', '훊', '훋', '훍', '훎', '훏', '훐', '훒', '훓', '훕', '훖', '훘', '훚', '훛', '훜', '훝', '훞', '훟', '훡', '훢', '훣', '훥', '훦', '훧', '훩', '훪', '훫', '훬', '훭', '훮', '훯', '훱', '훲', '훳', '훴', '훶', '훷', '훸', '훹', '훺', '훻', '훾', '훿', '휁', '휂', '휃', '휅', '휆', '휇', '휈', '휉', '휊', '휋', '휌', '휍', '휎', '휏', '휐', '휒', '휓', '휔', '휕', '휖', '휗', '휚', '휛', '휝', '휞', '휟', '휡', '휢', '휣', '휤', '휥', '휦', '휧', '휪', '휬', '휮', '휯', '휰', '휱', '휲', '휳', '휶', '휷', '휹', '휺', '휻', '휽', '휾', '휿', '흀', '흁', '흂', '흃', '흅', '흆', '흈', '흊', '흋', '흌', '흍', '흎', '흏', '흒', '흓', '흕', '흚', '흛', '흜', '흝', '흞', '흟', '흢', '흤', '흦', '흧', '흨', '흪', '흫', '흭', '흮', '흯', '흱', '흲', '흳', '흵', '흶', '흷', '흸', '흹', '흺', '흻', '흾', '흿', '힀', '힂', '힃', '힄', '힅', '힆', '힇', '힊', '힋', '힍', '힎', '힏', '힑', '힒', '힓', '힔', '힕', '힖', '힗', '힚', '힜', '힞', '힟', '힠', '힡', '힢', '힣', '\ud7a4']
```

### Comparing `kss-6.0.0/kss/_modules/preprocessing/filter_out.py` & `kss-6.0.0.dev0/kss/_modules/preprocessing/filter_out.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/preprocessing/half2full.py` & `kss-6.0.0.dev0/kss/_modules/preprocessing/half2full.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/preprocessing/normalize.py` & `kss-6.0.0.dev0/kss/_modules/preprocessing/normalize.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/preprocessing/preprocess.py` & `kss-6.0.0.dev0/kss/_modules/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/preprocessing/reduce_repeats.py` & `kss-6.0.0.dev0/kss/_modules/preprocessing/reduce_repeats.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/preprocessing/remove_invisible_chars.py` & `kss-6.0.0.dev0/kss/_modules/preprocessing/remove_invisible_chars.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/qwerty/qwerty.py` & `kss-6.0.0.dev0/kss/_modules/qwerty/qwerty.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/qwerty/utils.py` & `kss-6.0.0.dev0/kss/_modules/qwerty/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/romanization/romanize.py` & `kss-6.0.0.dev0/kss/_modules/romanization/romanize.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/romanization/utils.py` & `kss-6.0.0.dev0/kss/_modules/romanization/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/safety/check_safety.py` & `kss-6.0.0.dev0/kss/_modules/safety/check_safety.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def is_unsafe(
     text: Union[str, List[str], Tuple[str]],
     return_matches: bool = False,
     num_workers: Union[int, str] = "auto",
 ) -> Union[bool, List[bool], List[bool], List[List[str]]]:
     """
-    Check if the text is unsafe or not.
+    This checks if the text is unsafe or not.
 
     Args:
         text (Union[str, List[str], Tuple[str]]): single text or list of texts
         return_matches (bool): whether to return matches or not
         num_workers (Union[int, str]): the number of multiprocessing workers
 
     Returns:
```

### Comparing `kss-6.0.0/kss/_modules/safety/utils.py` & `kss-6.0.0.dev0/kss/_modules/safety/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/sentences/embracing_processor.py` & `kss-6.0.0.dev0/kss/_modules/sentences/embracing_processor.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/sentences/sentence_postprocessor.py` & `kss-6.0.0.dev0/kss/_modules/sentences/sentence_postprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/sentences/sentence_preprocessor.py` & `kss-6.0.0.dev0/kss/_modules/sentences/sentence_preprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/sentences/sentence_processor.py` & `kss-6.0.0.dev0/kss/_modules/sentences/sentence_processor.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/sentences/sentence_splitter.py` & `kss-6.0.0.dev0/kss/_modules/sentences/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/sentences/sentence_splitter_fast.py` & `kss-6.0.0.dev0/kss/_modules/sentences/sentence_splitter_fast.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/sentences/split_sentences.py` & `kss-6.0.0.dev0/kss/_modules/sentences/split_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/spacing/correct_spacing.py` & `kss-6.0.0.dev0/kss/_modules/spacing/correct_spacing.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/spacing/utils.py` & `kss-6.0.0.dev0/kss/_modules/spacing/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/summarization/summarize_sentences.py` & `kss-6.0.0.dev0/kss/_modules/summarization/summarize_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_modules/summarization/utils.py` & `kss-6.0.0.dev0/kss/_modules/summarization/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_utils/const.py` & `kss-6.0.0.dev0/kss/_utils/const.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_utils/emojis.py` & `kss-6.0.0.dev0/kss/_utils/emojis.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_utils/logger.py` & `kss-6.0.0.dev0/kss/_utils/logger.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_utils/multiprocessing.py` & `kss-6.0.0.dev0/kss/_utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss/_utils/sanity_checks.py` & `kss-6.0.0.dev0/kss/_utils/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/kss.egg-info/PKG-INFO` & `kss-6.0.0.dev0/kss.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kss
-Version: 6.0.0
+Version: 6.0.0.dev0
 Summary: A Toolkit for Korean sentence segmentation
 Home-page: https://github.com/hyunwoongko/kss
 Author: Hyunwoong Ko
 Author-email: kevin.brain@kakaobrain.com
 License: BSD 3-Clause "New" or "Revised" License
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -20,29 +20,15 @@
 License-File: LICENSE
 
 <h1 align="center">
 KSS: Korean String processing Suite
 </h1>
 
 <p align="center">
-    <a href="https://github.com/hyunwoongko/kss/releases">
-        <img alt="GitHub release" src="https://img.shields.io/github/release/hyunwoongko/kss.svg">
-    </a> 
-    <a href="https://github.com/hyunwoongko/kss/issues">
-        <img alt="Issues" src="https://img.shields.io/github/issues/hyunwoongko/kss">
-    </a>
-    <a href="https://github.com/hyunwoongko/kss/actions">
-        <img alt="Tests on Ubuntu" src="https://github.com/hyunwoongko/kss/actions/workflows/test_ubuntu.yaml/badge.svg">
-    </a>
-    <a href="https://github.com/hyunwoongko/kss/actions">
-        <img alt="Tests on MacOS" src="https://github.com/hyunwoongko/kss/actions/workflows/test_macos.yaml/badge.svg">
-    </a>
-    <a href="https://github.com/hyunwoongko/kss/actions">
-        <img alt="Tests on Windows" src="https://github.com/hyunwoongko/kss/actions/workflows/test_windows.yaml/badge.svg">
-    </a>
+    <a href="https://github.com/hyunwoongko/kss/releases"><img alt="GitHub release" src="https://img.shields.io/github/release/hyunwoongko/kss.svg"></a> <a href="https://github.com/hyunwoongko/kss/issues"><img alt="Issues" src="https://img.shields.io/github/issues/hyunwoongko/kss"></a> <a href="https://github.com/hyunwoongko/kss/actions"><img alt="Tests on Ubuntu" src="https://github.com/hyunwoongko/kss/actions/workflows/test_ubuntu.yaml/badge.svg"></a> <a href="https://github.com/hyunwoongko/kss/actions"><img alt="Tests on MacOS" src="https://github.com/hyunwoongko/kss/actions/workflows/test_macos.yaml/badge.svg"></a> <a href="https://github.com/hyunwoongko/kss/actions"><img alt="Tests on Windows" src="https://github.com/hyunwoongko/kss/actions/workflows/test_windows.yaml/badge.svg"></a>
 </p>
 
 
 KSS is a Korean string processing suite that provides various functions for processing Korean strings. It is designed to be simple and easy to use, and it is designed to be used in various fields such as natural language processing, data preprocessing, and data analysis.
 
 ### What's New:
 - April 27, 2024 [Released Kss 6.0 Python](https://github.com/hyunwoongko/kss/releases/tag/6.0.0).
@@ -119,15 +105,15 @@
     >>> text = "회사 동료 분들과 다녀왔는데 분위기도 좋고 음식도 맛있었어요 다만, 강남 토끼정이 강남 쉑쉑버거 골목길로 쭉 올라가야 하는데 다들 쉑쉑버거의 유혹에 넘어갈 뻔 했답니다 강남역 맛집 토끼정의 외부 모습."
     >>> split_sentences(text)
     ['회사 동료 분들과 다녀왔는데 분위기도 좋고 음식도 맛있었어요', '다만, 강남 토끼정이 강남 쉑쉑버거 골목길로 쭉 올라가야 하는데 다들 쉑쉑버거의 유혹에 넘어갈 뻔 했답니다', '강남역 맛집 토끼정의 외부 모습.']
 ```
 ### 4. Multiprocessing
 If you input a list of strings, Kss will automatically use multiprocessing to process the strings in parallel.
 And you can set the number of processes to use by setting the `num_workers` parameter.
-If you input `num_workers<2`, Kss will not use multiprocessing.
+If you input `num_workers < 2`, Kss will not use multiprocessing.
 
 ```python
 from kss import Kss
 
 module = Kss("MODULE_NAME")
 
 # using all cores
@@ -802,15 +788,16 @@
 
 References:
 - This was copied from [KoParadigm](https://github.com/Kyubyong/KoParadigm) and modified by Kss
 </details>
 
 <details>
 <summary>24. anonymize</summary>
-Anonymize sensitive information in the given text.
+
+This anonymizes sensitive information in the given text.
 
 Args:
 - text (`Union[str, List[str], Tuple[str]`): single text or list of texts
 - phone_number_anonymization (`bool`): whether to anonymize phone numbers or not
 - rrn_anonymization (`bool`): whether to anonymize resident registration numbers or not
 - card_anonymization (`bool`): whether to anonymize card numbers or not
 - email_anonymization (`bool`): whether to anonymize email addresses or not
@@ -846,15 +833,16 @@
 >>> print(output)
 "제 전화번호는 <PHONE_NUMBER>, 이메일 주소는 <EMAIL>입니다."
 ```
 </details>
 
 <details>
 <summary>25. clean_news</summary>
-Clean news articles by removing useless headers and footers.
+
+This cleans news articles by removing useless headers and footers.
 
 Args:
 - text (`Union[str, List[str], Tuple[str]]`): Input text or list of texts.
 - min_sentences (`int`): Minimum number of sentences to keep. Defaults to 3.
 - header_ratio (`float`): Ratio of the number of sentences to check in the header. Defaults to 0.4.
 - footer_ratio (`float`): Ratio of the number of sentences to check in the footer. Defaults to 0.4.
 - num_workers (`Union[int, str]`): the number of multiprocessing workers
@@ -900,36 +888,36 @@
 False
 ```
 </details>
 
 <details>
 <summary>27. get_all_completed_form_hangul_chars</summary>
 
-This returns all non-completed form Hangul characters.
+This returns all completed form Hangul characters.
 
 Returns:
-- `List[str]`: all non-completed form Hangul characters
+- `List[str]`: all completed form Hangul characters
 
 Examples:
 ```python
 >>> from kss import Kss
->>> get_all_incompleted_form_hangul_chars = Kss("get_all_incompleted_form_hangul_chars")
->>> output = get_all_incompleted_form_hangul_chars()
+>>> get_all_completed_form_hangul_chars = Kss("get_all_completed_form_hangul_chars")
+>>> output = get_all_completed_form_hangul_chars()
 >>> print(output)
-['갂', '갃', '갅', '갆', '갋', '갌', '갍', '갎', '갏', '갘', '갞', '갟', '갡', '갢', '갣', '갥', '갦', '갧', '갨', '갩', '갪', '갫', '갮', '갲', '갳', '갴', '갵', '갶', '갷', '갺', '갻', '갽', '갾', '갿', '걁', '걂', '걃', '걄', '걅', '걆', '걇', '걈', '걉', '걊', '걌', '걎', '걏', '걐', '걑', '걒', '걓', '걕', '걖', '걗', '걙', '걚', '걛', '걝', '걞', '걟', '걠', '걡', '걢', '걣', '걤', '걥', '걦', '걧', '걨', '걩', '걪', '걫', '걬', '걭', '걮', '걯', '걲', '걳', '걵', '걶', '걹', '걻', '걼', '걽', '걾', '걿', '겂', '겇', '겈', '겍', '겎', '겏', '겑', '겒', '겓', '겕', '겖', '겗', '겘', '겙', '겚', '겛', '겞', '겢', '겣', '겤', '겥', '겦', '겧', '겫', '겭', '겮', '겱', '겲', '겳', '겴', '겵', '겶', '겷', '겺', '겾', '겿', '곀', '곂', '곃', '곅', '곆', '곇', '곉', '곊', '곋', '곍', '곎', '곏', '곐', '곑', '곒', '곓', '곔', '곖', '곘', '곙', '곚', '곛', '곜', '곝', '곞', '곟', '곢', '곣', '곥', '곦', '곩', '곫', '곭', '곮', '곲', '곴', '곷', '곸', '곹', '곺', '곻', '곾', '곿', '괁', '괂', '괃', '괅', '괇', '괈', '괉', '괊', '괋', '괎', '괐', '괒', '괓', '괔', '괕', '괖', '괗', '괙', '괚', '괛', '괝', '괞', '괟', '괡', '괢', '괣', '괤', '괥', '괦', '괧', '괨', '괪', '괫', '괮', '괯', '괰', '괱', '괲', '괳', '괶', '괷', '괹', '괺', '괻', '괽', '괾', '괿', '굀', '굁', '굂', '굃', '굆', '굈', '굊', '굋', '굌', '굍', '굎', '굏', '굑', '굒', '굓', '굕', '굖', '굗', '굙', '굚', '굛', '굜', '굝', '굞', '굟', '굠', '굢', '굤', '굥', '굦', '굧', '굨', '굩', '굪', '굫', '굮', '굯', '굱', '굲', '굷', '굸', '굹', '굺', '굾', '궀', '궃', '궄', '궅', '궆', '궇', '궊', '궋', '궍', '궎', '궏', '궑', '궒', '궓', '궔', '궕', '궖', '궗', '궘', '궙', '궚', '궛', '궞', '궟', '궠', '궡', '궢', '궣', '궥', '궦', '궧', '궨', '궩', '궪', '궫', '궬', '궭', '궮', '궯', '궰', '궱', '궲', '궳', '궴', '궵', '궶', '궸', '궹', '궺', '궻', '궼', '궽', '궾', '궿', '귂', '귃', '귅', '귆', '귇', '귉', '귊', '귋', '귌', '귍', '귎', '귏', '귒', '귔', '귕', '귖', '귗', '귘', '귙', '귚', '귛', '귝', '귞', '귟', '귡', '귢', '귣', '귥', '귦', '귧', '귨', '귩', '귪', '귫', '귬', '귭', '귮', '귯', '귰', '귱', '귲', '귳', '귴', '귵', '귶', '귷', '귺', '귻', '귽', '귾', '긂', '긃', '긄', '긅', '긆', '긇', '긊', '긌', '긎', '긏', '긐', '긑', '긒', '긓', '긕', '긖', '긗', '긘', '긙', '긚', '긛', '긜', '긝', '긞', '긟', '긠', '긡', '긢', '긣', '긤', '긥', '긦', '긧', '긨', '긩', '긪', '긫', '긬', '긭', '긮', '긯', '긲', '긳', '긵', '긶', '긹', '긻', '긼', '긽', '긾', '긿', '깂', '깄', '깇', '깈', '깉', '깋', '깏', '깑', '깒', '깓', '깕', '깗', '깘', '깙', '깚', '깛', '깞', '깢', '깣', '깤', '깦', '깧', '깪', '깫', '깭', '깮', '깯', '깱', '깲', '깳', '깴', '깵', '깶', '깷', '깺', '깾', '깿', '꺀', '꺁', '꺂', '꺃', '꺆', '꺇', '꺈', '꺉', '꺊', '꺋', '꺍', '꺎', '꺏', '꺐', '꺑', '꺒', '꺓', '꺔', '꺕', '꺖', '꺗', '꺘', '꺙', '꺚', '꺛', '꺜', '꺝', '꺞', '꺟', '꺠', '꺡', '꺢', '꺣', '꺤', '꺥', '꺦', '꺧', '꺨', '꺩', '꺪', '꺫', '꺬', '꺭', '꺮', '꺯', '꺰', '꺱', '꺲', '꺳', '꺴', '꺵', '꺶', '꺷', '꺸', '꺹', '꺺', '꺻', '꺿', '껁', '껂', '껃', '껅', '껆', '껇', '껈', '껉', '껊', '껋', '껎', '껒', '껓', '껔', '껕', '껖', '껗', '껚', '껛', '껝', '껞', '껟', '껠', '껡', '껢', '껣', '껤', '껥', '껦', '껧', '껩', '껪', '껬', '껮', '껯', '껰', '껱', '껲', '껳', '껵', '껶', '껷', '껹', '껺', '껻', '껽', '껾', '껿', '꼀', '꼁', '꼂', '꼃', '꼄', '꼅', '꼆', '꼉', '꼊', '꼋', '꼌', '꼎', '꼏', '꼑', '꼒', '꼓', '꼔', '꼕', '꼖', '꼗', '꼘', '꼙', '꼚', '꼛', '꼜', '꼝', '꼞', '꼟', '꼠', '꼡', '꼢', '꼣', '꼤', '꼥', '꼦', '꼧', '꼨', '꼩', '꼪', '꼫', '꼮', '꼯', '꼱', '꼳', '꼵', '꼶', '꼷', '꼸', '꼹', '꼺', '꼻', '꼾', '꽀', '꽄', '꽅', '꽆', '꽇', '꽊', '꽋', '꽌', '꽍', '꽎', '꽏', '꽑', '꽒', '꽓', '꽔', '꽕', '꽖', '꽗', '꽘', '꽙', '꽚', '꽛', '꽞', '꽟', '꽠', '꽡', '꽢', '꽣', '꽦', '꽧', '꽨', '꽩', '꽪', '꽫', '꽬', '꽭', '꽮', '꽯', '꽰', '꽱', '꽲', '꽳', '꽴', '꽵', '꽶', '꽷', '꽸', '꽺', '꽻', '꽼', '꽽', '꽾', '꽿', '꾁', '꾂', '꾃', '꾅', '꾆', '꾇', '꾉', '꾊', '꾋', '꾌', '꾍', '꾎', '꾏', '꾒', '꾓', '꾔', '꾖', '꾗', '꾘', '꾙', '꾚', '꾛', '꾝', '꾞', '꾟', '꾠', '꾡', '꾢', '꾣', '꾤', '꾥', '꾦', '꾧', '꾨', '꾩', '꾪', '꾫', '꾬', '꾭', '꾮', '꾯', '꾰', '꾱', '꾲', '꾳', '꾴', '꾵', '꾶', '꾷', '꾺', '꾻', '꾽', '꾾', '꾿', '꿁', '꿂', '꿃', '꿄', '꿅', '꿆', '꿊', '꿌', '꿏', '꿐', '꿑', '꿒', '꿓', '꿕', '꿖', '꿗', '꿘', '꿙', '꿚', '꿛', '꿝', '꿞', '꿟', '꿠', '꿡', '꿢', '꿣', '꿤', '꿥', '꿦', '꿧', '꿪', '꿫', '꿬', '꿭', '꿮', '꿯', '꿲', '꿳', '꿵', '꿶', '꿷', '꿹', '꿺', '꿻', '꿼', '꿽', '꿾', '꿿', '뀂', '뀃', '뀅', '뀆', '뀇', '뀈', '뀉', '뀊', '뀋', '뀍', '뀎', '뀏', '뀑', '뀒', '뀓', '뀕', '뀖', '뀗', '뀘', '뀙', '뀚', '뀛', '뀞', '뀟', '뀠', '뀡', '뀢', '뀣', '뀤', '뀥', '뀦', '뀧', '뀩', '뀪', '뀫', '뀬', '뀭', '뀮', '뀯', '뀰', '뀱', '뀲', '뀳', '뀴', '뀵', '뀶', '뀷', '뀸', '뀹', '뀺', '뀻', '뀼', '뀽', '뀾', '뀿', '끀', '끁', '끂', '끃', '끆', '끇', '끉', '끋', '끍', '끏', '끐', '끑', '끒', '끖', '끘', '끚', '끛', '끜', '끞', '끟', '끠', '끡', '끢', '끣', '끤', '끥', '끦', '끧', '끨', '끩', '끪', '끫', '끬', '끭', '끮', '끯', '끰', '끱', '끲', '끳', '끴', '끵', '끶', '끷', '끸', '끹', '끺', '끻', '끾', '끿', '낁', '낂', '낃', '낅', '낆', '낇', '낈', '낉', '낊', '낋', '낎', '낐', '낒', '낓', '낔', '낕', '낖', '낗', '낛', '낝', '낞', '낣', '낤', '낥', '낦', '낧', '낪', '낰', '낲', '낶', '낷', '낹', '낺', '낻', '낽', '낾', '낿', '냀', '냁', '냂', '냃', '냆', '냊', '냋', '냌', '냍', '냎', '냏', '냒', '냓', '냕', '냖', '냗', '냙', '냚', '냛', '냜', '냝', '냞', '냟', '냡', '냢', '냣', '냤', '냦', '냧', '냨', '냩', '냪', '냫', '냬', '냭', '냮', '냯', '냰', '냱', '냲', '냳', '냴', '냵', '냶', '냷', '냸', '냹', '냺', '냻', '냼', '냽', '냾', '냿', '넀', '넁', '넂', '넃', '넄', '넅', '넆', '넇', '넊', '넍', '넎', '넏', '넑', '넔', '넕', '넖', '넗', '넚', '넞', '넟', '넠', '넡', '넢', '넦', '넧', '넩', '넪', '넫', '넭', '넮', '넯', '넰', '넱', '넲', '넳', '넶', '넺', '넻', '넼', '넽', '넾', '넿', '녂', '녃', '녅', '녆', '녇', '녉', '녊', '녋', '녌', '녍', '녎', '녏', '녒', '녓', '녖', '녗', '녙', '녚', '녛', '녝', '녞', '녟', '녡', '녢', '녣', '녤', '녥', '녦', '녧', '녨', '녩', '녪', '녫', '녬', '녭', '녮', '녯', '녰', '녱', '녲', '녳', '녴', '녵', '녶', '녷', '녺', '녻', '녽', '녾', '녿', '놁', '놃', '놄', '놅', '놆', '놇', '놊', '놌', '놎', '놏', '놐', '놑', '놕', '놖', '놗', '놙', '놚', '놛', '놝', '놞', '놟', '놠', '놡', '놢', '놣', '놤', '놥', '놦', '놧', '놩', '놪', '놫', '놬', '놭', '놮', '놯', '놰', '놱', '놲', '놳', '놴', '놵', '놶', '놷', '놸', '놹', '놺', '놻', '놼', '놽', '놾', '놿', '뇀', '뇁', '뇂', '뇃', '뇄', '뇅', '뇆', '뇇', '뇈', '뇉', '뇊', '뇋', '뇍', '뇎', '뇏', '뇑', '뇒', '뇓', '뇕', '뇖', '뇗', '뇘', '뇙', '뇚', '뇛', '뇞', '뇠', '뇡', '뇢', '뇣', '뇤', '뇥', '뇦', '뇧', '뇪', '뇫', '뇭', '뇮', '뇯', '뇱', '뇲', '뇳', '뇴', '뇵', '뇶', '뇷', '뇸', '뇺', '뇼', '뇾', '뇿', '눀', '눁', '눂', '눃', '눆', '눇', '눉', '눊', '눍', '눎', '눏', '눐', '눑', '눒', '눓', '눖', '눘', '눚', '눛', '눜', '눝', '눞', '눟', '눡', '눢', '눣', '눤', '눥', '눦', '눧', '눨', '눩', '눪', '눫', '눬', '눭', '눮', '눯', '눰', '눱', '눲', '눳', '눵', '눶', '눷', '눸', '눹', '눺', '눻', '눽', '눾', '눿', '뉀', '뉁', '뉂', '뉃', '뉄', '뉅', '뉆', '뉇', '뉈', '뉉', '뉊', '뉋', '뉌', '뉍', '뉎', '뉏', '뉐', '뉑', '뉒', '뉓', '뉔', '뉕', '뉖', '뉗', '뉙', '뉚', '뉛', '뉝', '뉞', '뉟', '뉡', '뉢', '뉣', '뉤', '뉥', '뉦', '뉧', '뉪', '뉫', '뉬', '뉭', '뉮', '뉯', '뉰', '뉱', '뉲', '뉳', '뉶', '뉷', '뉸', '뉹', '뉺', '뉻', '뉽', '뉾', '뉿', '늀', '늁', '늂', '늃', '늆', '늇', '늈', '늊', '늋', '늌', '늍', '늎', '늏', '늒', '늓', '늕', '늖', '늗', '늛', '늜', '늝', '늞', '늟', '늢', '늤', '늧', '늨', '늩', '늫', '늭', '늮', '늯', '늱', '늲', '늳', '늵', '늶', '늷', '늸', '늹', '늺', '늻', '늼', '늽', '늾', '늿', '닀', '닁', '닂', '닃', '닄', '닅', '닆', '닇', '닊', '닋', '닍', '닎', '닏', '닑', '닓', '닔', '닕', '닖', '닗', '닚', '닜', '닞', '닟', '닠', '닡', '닣', '닧', '닩', '닪', '닰', '닱', '닲', '닶', '닼', '닽', '닾', '댂', '댃', '댅', '댆', '댇', '댉', '댊', '댋', '댌', '댍', '댎', '댏', '댒', '댖', '댗', '댘', '댙', '댚', '댛', '댝', '댞', '댟', '댠', '댡', '댢', '댣', '댤', '댥', '댦', '댧', '댨', '댩', '댪', '댫', '댬', '댭', '댮', '댯', '댰', '댱', '댲', '댳', '댴', '댵', '댶', '댷', '댸', '댹', '댺', '댻', '댼', '댽', '댾', '댿', '덀', '덁', '덂', '덃', '덄', '덅', '덆', '덇', '덈', '덉', '덊', '덋', '덌', '덍', '덎', '덏', '덐', '덑', '덒', '덓', '덗', '덙', '덚', '덝', '덠', '덡', '덢', '덣', '덦', '덨', '덪', '덬', '덭', '덯', '덲', '덳', '덵', '덶', '덷', '덹', '덺', '덻', '덼', '덽', '덾', '덿', '뎂', '뎆', '뎇', '뎈', '뎉', '뎊', '뎋', '뎍', '뎎', '뎏', '뎑', '뎒', '뎓', '뎕', '뎖', '뎗', '뎘', '뎙', '뎚', '뎛', '뎜', '뎝', '뎞', '뎟', '뎢', '뎣', '뎤', '뎥', '뎦', '뎧', '뎩', '뎪', '뎫', '뎭', '뎮', '뎯', '뎰', '뎱', '뎲', '뎳', '뎴', '뎵', '뎶', '뎷', '뎸', '뎹', '뎺', '뎻', '뎼', '뎽', '뎾', '뎿', '돀', '돁', '돂', '돃', '돆', '돇', '돉', '돊', '돍', '돏', '돑', '돒', '돓', '돖', '돘', '돚', '돜', '돞', '돟', '돡', '돢', '돣', '돥', '돦', '돧', '돩', '돪', '돫', '돬', '돭', '돮', '돯', '돰', '돱', '돲', '돳', '돴', '돵', '돶', '돷', '돸', '돹', '돺', '돻', '돽', '돾', '돿', '됀', '됁', '됂', '됃', '됄', '됅', '됆', '됇', '됈', '됉', '됊', '됋', '됌', '됍', '됎', '됏', '됑', '됒', '됓', '됔', '됕', '됖', '됗', '됙', '됚', '됛', '됝', '됞', '됟', '됡', '됢', '됣', '됤', '됥', '됦', '됧', '됪', '됬', '됭', '됮', '됯', '됰', '됱', '됲', '됳', '됵', '됶', '됷', '됸', '됹', '됺', '됻', '됼', '됽', '됾', '됿', '둀', '둁', '둂', '둃', '둄', '둅', '둆', '둇', '둈', '둉', '둊', '둋', '둌', '둍', '둎', '둏', '둒', '둓', '둕', '둖', '둗', '둙', '둚', '둛', '둜', '둝', '둞', '둟', '둢', '둤', '둦', '둧', '둨', '둩', '둪', '둫', '둭', '둮', '둯', '둰', '둱', '둲', '둳', '둴', '둵', '둶', '둷', '둸', '둹', '둺', '둻', '둼', '둽', '둾', '둿', '뒁', '뒂', '뒃', '뒄', '뒅', '뒆', '뒇', '뒉', '뒊', '뒋', '뒌', '뒍', '뒎', '뒏', '뒐', '뒑', '뒒', '뒓', '뒔', '뒕', '뒖', '뒗', '뒘', '뒙', '뒚', '뒛', '뒜', '뒞', '뒟', '뒠', '뒡', '뒢', '뒣', '뒥', '뒦', '뒧', '뒩', '뒪', '뒫', '뒭', '뒮', '뒯', '뒰', '뒱', '뒲', '뒳', '뒴', '뒶', '뒸', '뒺', '뒻', '뒼', '뒽', '뒾', '뒿', '듁', '듂', '듃', '듅', '듆', '듇', '듉', '듊', '듋', '듌', '듍', '듎', '듏', '듑', '듒', '듓', '듔', '듖', '듗', '듘', '듙', '듚', '듛', '듞', '듟', '듡', '듢', '듥', '듧', '듨', '듩', '듪', '듫', '듮', '듰', '듲', '듳', '듴', '듵', '듶', '듷', '듹', '듺', '듻', '듼', '듽', '듾', '듿', '딀', '딁', '딂', '딃', '딄', '딅', '딆', '딇', '딈', '딉', '딊', '딋', '딌', '딍', '딎', '딏', '딐', '딑', '딒', '딓', '딖', '딗', '딙', '딚', '딝', '딞', '딟', '딠', '딡', '딢', '딣', '딦', '딫', '딬', '딭', '딮', '딯', '딲', '딳', '딵', '딶', '딷', '딹', '딺', '딻', '딼', '딽', '딾', '딿', '땂', '땆', '땇', '땈', '땉', '땊', '땎', '땏', '땑', '땒', '땓', '땕', '땖', '땗', '땘', '땙', '땚', '땛', '땞', '땢', '땣', '땤', '땥', '땦', '땧', '땨', '땩', '땪', '땫', '땬', '땭', '땮', '땯', '땰', '땱', '땲', '땳', '땴', '땵', '땶', '땷', '땸', '땹', '땺', '땻', '땼', '땽', '땾', '땿', '떀', '떁', '떂', '떃', '떄', '떅', '떆', '떇', '떈', '떉', '떊', '떋', '떌', '떍', '떎', '떏', '떐', '떑', '떒', '떓', '떔', '떕', '떖', '떗', '떘', '떙', '떚', '떛', '떜', '떝', '떞', '떟', '떢', '떣', '떥', '떦', '떧', '떩', '떬', '떭', '떮', '떯', '떲', '떶', '떷', '떸', '떹', '떺', '떾', '떿', '뗁', '뗂', '뗃', '뗅', '뗆', '뗇', '뗈', '뗉', '뗊', '뗋', '뗎', '뗒', '뗓', '뗔', '뗕', '뗖', '뗗', '뗙', '뗚', '뗛', '뗜', '뗝', '뗞', '뗟', '뗠', '뗡', '뗢', '뗣', '뗤', '뗥', '뗦', '뗧', '뗨', '뗩', '뗪', '뗫', '뗭', '뗮', '뗯', '뗰', '뗱', '뗲', '뗳', '뗴', '뗵', '뗶', '뗷', '뗸', '뗹', '뗺', '뗻', '뗼', '뗽', '뗾', '뗿', '똀', '똁', '똂', '똃', '똄', '똅', '똆', '똇', '똈', '똉', '똊', '똋', '똌', '똍', '똎', '똏', '똒', '똓', '똕', '똖', '똗', '똙', '똚', '똛', '똜', '똝', '똞', '똟', '똠', '똡', '똢', '똣', '똤', '똦', '똧', '똨', '똩', '똪', '똫', '똭', '똮', '똯', '똰', '똱', '똲', '똳', '똵', '똶', '똷', '똸', '똹', '똺', '똻', '똼', '똽', '똾', '똿', '뙀', '뙁', '뙂', '뙃', '뙄', '뙅', '뙆', '뙇', '뙉', '뙊', '뙋', '뙌', '뙍', '뙎', '뙏', '뙐', '뙑', '뙒', '뙓', '뙔', '뙕', '뙖', '뙗', '뙘', '뙙', '뙚', '뙛', '뙜', '뙝', '뙞', '뙟', '뙠', '뙡', '뙢', '뙣', '뙥', '뙦', '뙧', '뙩', '뙪', '뙫', '뙬', '뙭', '뙮', '뙯', '뙰', '뙱', '뙲', '뙳', '뙴', '뙵', '뙶', '뙷', '뙸', '뙹', '뙺', '뙻', '뙼', '뙽', '뙾', '뙿', '뚀', '뚁', '뚂', '뚃', '뚄', '뚅', '뚆', '뚇', '뚈', '뚉', '뚊', '뚋', '뚌', '뚍', '뚎', '뚏', '뚐', '뚑', '뚒', '뚓', '뚔', '뚕', '뚖', '뚗', '뚘', '뚙', '뚚', '뚛', '뚞', '뚟', '뚡', '뚢', '뚣', '뚥', '뚦', '뚧', '뚨', '뚩', '뚪', '뚭', '뚮', '뚯', '뚰', '뚲', '뚳', '뚴', '뚵', '뚶', '뚷', '뚸', '뚹', '뚺', '뚻', '뚼', '뚽', '뚾', '뚿', '뛀', '뛁', '뛂', '뛃', '뛄', '뛅', '뛆', '뛇', '뛈', '뛉', '뛊', '뛋', '뛌', '뛍', '뛎', '뛏', '뛐', '뛑', '뛒', '뛓', '뛕', '뛖', '뛗', '뛘', '뛙', '뛚', '뛛', '뛜', '뛝', '뛞', '뛟', '뛠', '뛡', '뛢', '뛣', '뛤', '뛥', '뛦', '뛧', '뛨', '뛩', '뛪', '뛫', '뛬', '뛭', '뛮', '뛯', '뛱', '뛲', '뛳', '뛵', '뛶', '뛷', '뛹', '뛺', '뛻', '뛼', '뛽', '뛾', '뛿', '뜂', '뜃', '뜄', '뜆', '뜇', '뜈', '뜉', '뜊', '뜋', '뜌', '뜍', '뜎', '뜏', '뜐', '뜑', '뜒', '뜓', '뜔', '뜕', '뜖', '뜗', '뜘', '뜙', '뜚', '뜛', '뜜', '뜝', '뜞', '뜟', '뜠', '뜡', '뜢', '뜣', '뜤', '뜥', '뜦', '뜧', '뜪', '뜫', '뜭', '뜮', '뜱', '뜲', '뜳', '뜴', '뜵', '뜶', '뜷', '뜺', '뜼', '뜽', '뜾', '뜿', '띀', '띁', '띂', '띃', '띅', '띆', '띇', '띉', '띊', '띋', '띍', '띎', '띏', '띐', '띑', '띒', '띓', '띖', '띗', '띘', '띙', '띚', '띛', '띜', '띝', '띞', '띟', '띡', '띢', '띣', '띥', '띦', '띧', '띩', '띪', '띫', '띬', '띭', '띮', '띯', '띲', '띴', '띶', '띷', '띸', '띹', '띺', '띻', '띾', '띿', '랁', '랂', '랃', '랅', '랆', '랇', '랈', '랉', '랊', '랋', '랎', '랓', '랔', '랕', '랚', '랛', '랝', '랞', '랟', '랡', '랢', '랣', '랤', '랥', '랦', '랧', '랪', '랮', '랯', '랰', '랱', '랲', '랳', '랶', '랷', '랹', '랺', '랻', '랼', '랽', '랾', '랿', '럀', '럁', '럂', '럃', '럄', '럅', '럆', '럈', '럊', '럋', '럌', '럍', '럎', '럏', '럐', '럑', '럒', '럓', '럔', '럕', '럖', '럗', '럘', '럙', '럚', '럛', '럜', '럝', '럞', '럟', '럠', '럡', '럢', '럣', '럤', '럥', '럦', '럧', '럨', '럩', '럪', '럫', '럮', '럯', '럱', '럲', '럳', '럵', '럶', '럷', '럸', '럹', '럺', '럻', '럾', '렂', '렃', '렄', '렅', '렆', '렊', '렋', '렍', '렎', '렏', '렑', '렒', '렓', '렔', '렕', '렖', '렗', '렚', '렜', '렞', '렟', '렠', '렡', '렢', '렣', '렦', '렧', '렩', '렪', '렫', '렭', '렮', '렯', '렰', '렱', '렲', '렳', '렶', '렺', '렻', '렼', '렽', '렾', '렿', '롁', '롂', '롃', '롅', '롆', '롇', '롈', '롉', '롊', '롋', '롌', '롍', '롎', '롏', '롐', '롒', '롔', '롕', '롖', '롗', '롘', '롙', '롚', '롛', '롞', '롟', '롡', '롢', '롣', '롥', '롦', '롧', '롨', '롩', '롪', '롫', '롮', '롰', '롲', '롳', '롴', '롵', '롶', '롷', '롹', '롺', '롻', '롽', '롾', '롿', '뢀', '뢁', '뢂', '뢃', '뢄', '뢅', '뢆', '뢇', '뢈', '뢉', '뢊', '뢋', '뢌', '뢎', '뢏', '뢐', '뢑', '뢒', '뢓', '뢔', '뢕', '뢖', '뢗', '뢘', '뢙', '뢚', '뢛', '뢜', '뢝', '뢞', '뢟', '뢠', '뢡', '뢢', '뢣', '뢤', '뢥', '뢦', '뢧', '뢩', '뢪', '뢫', '뢬', '뢭', '뢮', '뢯', '뢱', '뢲', '뢳', '뢵', '뢶', '뢷', '뢹', '뢺', '뢻', '뢼', '뢽', '뢾', '뢿', '룂', '룄', '룆', '룇', '룈', '룉', '룊', '룋', '룍', '룎', '룏', '룑', '룒', '룓', '룕', '룖', '룗', '룘', '룙', '룚', '룛', '룜', '룞', '룠', '룢', '룣', '룤', '룥', '룦', '룧', '룪', '룫', '룭', '룮', '룯', '룱', '룲', '룳', '룴', '룵', '룶', '룷', '룺', '룼', '룾', '룿', '뤀', '뤁', '뤂', '뤃', '뤅', '뤆', '뤇', '뤈', '뤉', '뤊', '뤋', '뤌', '뤍', '뤎', '뤏', '뤐', '뤑', '뤒', '뤓', '뤔', '뤕', '뤖', '뤗', '뤙', '뤚', '뤛', '뤜', '뤝', '뤞', '뤟', '뤡', '뤢', '뤣', '뤤', '뤥', '뤦', '뤧', '뤨', '뤩', '뤪', '뤫', '뤬', '뤭', '뤮', '뤯', '뤰', '뤱', '뤲', '뤳', '뤴', '뤵', '뤶', '뤷', '뤸', '뤹', '뤺', '뤻', '뤾', '뤿', '륁', '륂', '륃', '륅', '륆', '륇', '륈', '륉', '륊', '륋', '륍', '륎', '륐', '륒', '륓', '륔', '륕', '륖', '륗', '륚', '륛', '륝', '륞', '륟', '륡', '륢', '륣', '륤', '륥', '륦', '륧', '륪', '륬', '륮', '륯', '륰', '륱', '륲', '륳', '륶', '륷', '륹', '륺', '륻', '륽', '륾', '륿', '릀', '릁', '릂', '릃', '릆', '릈', '릋', '릌', '릏', '릐', '릑', '릒', '릓', '릔', '릕', '릖', '릗', '릘', '릙', '릚', '릛', '릜', '릝', '릞', '릟', '릠', '릡', '릢', '릣', '릤', '릥', '릦', '릧', '릨', '릩', '릪', '릫', '릮', '릯', '릱', '릲', '릳', '릵', '릶', '릷', '릸', '릹', '릺', '릻', '릾', '맀', '맂', '맃', '맄', '맅', '맆', '맇', '맊', '맋', '맍', '맓', '맔', '맕', '맖', '맗', '맚', '맜', '맟', '맠', '맢', '맦', '맧', '맩', '맪', '맫', '맭', '맮', '맯', '맰', '맱', '맲', '맳', '맶', '맻', '맼', '맽', '맾', '맿', '먂', '먃', '먄', '먅', '먆', '먇', '먉', '먊', '먋', '먌', '먍', '먎', '먏', '먐', '먑', '먒', '먓', '먔', '먖', '먗', '먘', '먙', '먚', '먛', '먜', '먝', '먞', '먟', '먠', '먡', '먢', '먣', '먤', '먥', '먦', '먧', '먨', '먩', '먪', '먫', '먬', '먭', '먮', '먯', '먰', '먱', '먲', '먳', '먴', '먵', '먶', '먷', '먺', '먻', '먽', '먾', '먿', '멁', '멃', '멄', '멅', '멆', '멇', '멊', '멌', '멏', '멐', '멑', '멒', '멖', '멗', '멙', '멚', '멛', '멝', '멞', '멟', '멠', '멡', '멢', '멣', '멦', '멪', '멫', '멬', '멭', '멮', '멯', '멲', '멳', '멵', '멶', '멷', '멹', '멺', '멻', '멼', '멽', '멾', '멿', '몀', '몁', '몂', '몆', '몈', '몉', '몊', '몋', '몍', '몎', '몏', '몐', '몑', '몒', '몓', '몔', '몕', '몖', '몗', '몘', '몙', '몚', '몛', '몜', '몝', '몞', '몟', '몠', '몡', '몢', '몣', '몤', '몥', '몦', '몧', '몪', '몭', '몮', '몯', '몱', '몳', '몴', '몵', '몶', '몷', '몺', '몼', '몾', '몿', '뫀', '뫁', '뫂', '뫃', '뫅', '뫆', '뫇', '뫉', '뫊', '뫋', '뫌', '뫍', '뫎', '뫏', '뫐', '뫑', '뫒', '뫓', '뫔', '뫕', '뫖', '뫗', '뫚', '뫛', '뫜', '뫝', '뫞', '뫟', '뫠', '뫡', '뫢', '뫣', '뫤', '뫥', '뫦', '뫧', '뫨', '뫩', '뫪', '뫫', '뫬', '뫭', '뫮', '뫯', '뫰', '뫱', '뫲', '뫳', '뫴', '뫵', '뫶', '뫷', '뫸', '뫹', '뫺', '뫻', '뫽', '뫾', '뫿', '묁', '묂', '묃', '묅', '묆', '묇', '묈', '묉', '묊', '묋', '묌', '묎', '묐', '묒', '묓', '묔', '묕', '묖', '묗', '묙', '묚', '묛', '묝', '묞', '묟', '묡', '묢', '묣', '묤', '묥', '묦', '묧', '묨', '묪', '묬', '묭', '묮', '묯', '묰', '묱', '묲', '묳', '묷', '묹', '묺', '묿', '뭀', '뭁', '뭂', '뭃', '뭆', '뭈', '뭊', '뭋', '뭌', '뭎', '뭑', '뭒', '뭓', '뭕', '뭖', '뭗', '뭙', '뭚', '뭛', '뭜', '뭝', '뭞', '뭟', '뭠', '뭢', '뭤', '뭥', '뭦', '뭧', '뭨', '뭩', '뭪', '뭫', '뭭', '뭮', '뭯', '뭰', '뭱', '뭲', '뭳', '뭴', '뭵', '뭶', '뭷', '뭸', '뭹', '뭺', '뭻', '뭼', '뭽', '뭾', '뭿', '뮀', '뮁', '뮂', '뮃', '뮄', '뮅', '뮆', '뮇', '뮉', '뮊', '뮋', '뮍', '뮎', '뮏', '뮑', '뮒', '뮓', '뮔', '뮕', '뮖', '뮗', '뮘', '뮙', '뮚', '뮛', '뮜', '뮝', '뮞', '뮟', '뮠', '뮡', '뮢', '뮣', '뮥', '뮦', '뮧', '뮩', '뮪', '뮫', '뮭', '뮮', '뮯', '뮰', '뮱', '뮲', '뮳', '뮵', '뮶', '뮸', '뮹', '뮺', '뮻', '뮼', '뮽', '뮾', '뮿', '믁', '믂', '믃', '믅', '믆', '믇', '믉', '믊', '믋', '믌', '믍', '믎', '믏', '믑', '믒', '믔', '믕', '믖', '믗', '믘', '믙', '믚', '믛', '믜', '믝', '믞', '믟', '믠', '믡', '믢', '믣', '믤', '믥', '믦', '믧', '믨', '믩', '믪', '믫', '믬', '믭', '믮', '믯', '믰', '믱', '믲', '믳', '믴', '믵', '믶', '믷', '믺', '믻', '믽', '믾', '밁', '밃', '밄', '밅', '밆', '밇', '밊', '밎', '밐', '밒', '밓', '밙', '밚', '밠', '밡', '밢', '밣', '밦', '밨', '밪', '밫', '밬', '밮', '밯', '밲', '밳', '밵', '밶', '밷', '밹', '밺', '밻', '밼', '밽', '밾', '밿', '뱂', '뱆', '뱇', '뱈', '뱊', '뱋', '뱎', '뱏', '뱑', '뱒', '뱓', '뱔', '뱕', '뱖', '뱗', '뱘', '뱙', '뱚', '뱛', '뱜', '뱞', '뱟', '뱠', '뱡', '뱢', '뱣', '뱤', '뱥', '뱦', '뱧', '뱨', '뱩', '뱪', '뱫', '뱬', '뱭', '뱮', '뱯', '뱰', '뱱', '뱲', '뱳', '뱴', '뱵', '뱶', '뱷', '뱸', '뱹', '뱺', '뱻', '뱼', '뱽', '뱾', '뱿', '벀', '벁', '벂', '벃', '벆', '벇', '벉', '벊', '벍', '벏', '벐', '벑', '벒', '벓', '벖', '벘', '벛', '벜', '벝', '벞', '벟', '벢', '벣', '벥', '벦', '벩', '벪', '벫', '벬', '벭', '벮', '벯', '벲', '벶', '벷', '벸', '벹', '벺', '벻', '벾', '벿', '볁', '볂', '볃', '볅', '볆', '볇', '볈', '볉', '볊', '볋', '볌', '볎', '볒', '볓', '볔', '볖', '볗', '볙', '볚', '볛', '볝', '볞', '볟', '볠', '볡', '볢', '볣', '볤', '볥', '볦', '볧', '볨', '볩', '볪', '볫', '볬', '볭', '볮', '볯', '볰', '볱', '볲', '볳', '볷', '볹', '볺', '볻', '볽', '볾', '볿', '봀', '봁', '봂', '봃', '봆', '봈', '봊', '봋', '봌', '봍', '봎', '봏', '봑', '봒', '봓', '봕', '봖', '봗', '봘', '봙', '봚', '봛', '봜', '봝', '봞', '봟', '봠', '봡', '봢', '봣', '봥', '봦', '봧', '봨', '봩', '봪', '봫', '봭', '봮', '봯', '봰', '봱', '봲', '봳', '봴', '봵', '봶', '봷', '봸', '봹', '봺', '봻', '봼', '봽', '봾', '봿', '뵁', '뵂', '뵃', '뵄', '뵅', '뵆', '뵇', '뵊', '뵋', '뵍', '뵎', '뵏', '뵑', '뵒', '뵓', '뵔', '뵕', '뵖', '뵗', '뵚', '뵛', '뵜', '뵝', '뵞', '뵟', '뵠', '뵡', '뵢', '뵣', '뵥', '뵦', '뵧', '뵩', '뵪', '뵫', '뵬', '뵭', '뵮', '뵯', '뵰', '뵱', '뵲', '뵳', '뵴', '뵵', '뵶', '뵷', '뵸', '뵹', '뵺', '뵻', '뵼', '뵽', '뵾', '뵿', '붂', '붃', '붅', '붆', '붋', '붌', '붍', '붎', '붏', '붒', '붔', '붖', '붗', '붘', '붛', '붝', '붞', '붟', '붠', '붡', '붢', '붣', '붥', '붦', '붧', '붨', '붩', '붪', '붫', '붬', '붭', '붮', '붯', '붱', '붲', '붳', '붴', '붵', '붶', '붷', '붹', '붺', '붻', '붼', '붽', '붾', '붿', '뷀', '뷁', '뷂', '뷃', '뷄', '뷅', '뷆', '뷇', '뷈', '뷉', '뷊', '뷋', '뷌', '뷍', '뷎', '뷏', '뷐', '뷑', '뷒', '뷓', '뷖', '뷗', '뷙', '뷚', '뷛', '뷝', '뷞', '뷟', '뷠', '뷡', '뷢', '뷣', '뷤', '뷥', '뷦', '뷧', '뷨', '뷪', '뷫', '뷬', '뷭', '뷮', '뷯', '뷱', '뷲', '뷳', '뷵', '뷶', '뷷', '뷹', '뷺', '뷻', '뷼', '뷽', '뷾', '뷿', '븁', '븂', '븄', '븆', '븇', '븈', '븉', '븊', '븋', '븎', '븏', '븑', '븒', '븓', '븕', '븖', '븗', '븘', '븙', '븚', '븛', '븞', '븠', '븡', '븢', '븣', '븤', '븥', '븦', '븧', '븨', '븩', '븪', '븫', '븬', '븭', '븮', '븯', '븰', '븱', '븲', '븳', '븴', '븵', '븶', '븷', '븸', '븹', '븺', '븻', '븼', '븽', '븾', '븿', '빀', '빁', '빂', '빃', '빆', '빇', '빉', '빊', '빋', '빍', '빏', '빐', '빑', '빒', '빓', '빖', '빘', '빜', '빝', '빞', '빟', '빢', '빣', '빥', '빦', '빧', '빩', '빫', '빬', '빭', '빮', '빯', '빲', '빶', '빷', '빸', '빹', '빺', '빾', '빿', '뺁', '뺂', '뺃', '뺅', '뺆', '뺇', '뺈', '뺉', '뺊', '뺋', '뺎', '뺒', '뺓', '뺔', '뺕', '뺖', '뺗', '뺚', '뺛', '뺜', '뺝', '뺞', '뺟', '뺠', '뺡', '뺢', '뺣', '뺤', '뺥', '뺦', '뺧', '뺩', '뺪', '뺫', '뺬', '뺭', '뺮', '뺯', '뺰', '뺱', '뺲', '뺳', '뺴', '뺵', '뺶', '뺷', '뺸', '뺹', '뺺', '뺻', '뺼', '뺽', '뺾', '뺿', '뻀', '뻁', '뻂', '뻃', '뻄', '뻅', '뻆', '뻇', '뻈', '뻉', '뻊', '뻋', '뻌', '뻍', '뻎', '뻏', '뻒', '뻓', '뻕', '뻖', '뻙', '뻚', '뻛', '뻜', '뻝', '뻞', '뻟', '뻡', '뻢', '뻦', '뻧', '뻨', '뻩', '뻪', '뻫', '뻭', '뻮', '뻯', '뻰', '뻱', '뻲', '뻳', '뻴', '뻵', '뻶', '뻷', '뻸', '뻹', '뻺', '뻻', '뻼', '뻽', '뻾', '뻿', '뼀', '뼂', '뼃', '뼄', '뼅', '뼆', '뼇', '뼊', '뼋', '뼌', '뼍', '뼎', '뼏', '뼐', '뼑', '뼒', '뼓', '뼔', '뼕', '뼖', '뼗', '뼚', '뼞', '뼟', '뼠', '뼡', '뼢', '뼣', '뼤', '뼥', '뼦', '뼧', '뼨', '뼩', '뼪', '뼫', '뼬', '뼭', '뼮', '뼯', '뼰', '뼱', '뼲', '뼳', '뼴', '뼵', '뼶', '뼷', '뼸', '뼹', '뼺', '뼻', '뼼', '뼽', '뼾', '뼿', '뽂', '뽃', '뽅', '뽆', '뽇', '뽉', '뽊', '뽋', '뽌', '뽍', '뽎', '뽏', '뽒', '뽓', '뽔', '뽖', '뽗', '뽘', '뽙', '뽚', '뽛', '뽜', '뽝', '뽞', '뽟', '뽠', '뽡', '뽢', '뽣', '뽤', '뽥', '뽦', '뽧', '뽨', '뽩', '뽪', '뽫', '뽬', '뽭', '뽮', '뽯', '뽰', '뽱', '뽲', '뽳', '뽴', '뽵', '뽶', '뽷', '뽸', '뽹', '뽺', '뽻', '뽼', '뽽', '뽾', '뽿', '뾀', '뾁', '뾂', '뾃', '뾄', '뾅', '뾆', '뾇', '뾈', '뾉', '뾊', '뾋', '뾌', '뾍', '뾎', '뾏', '뾐', '뾑', '뾒', '뾓', '뾕', '뾖', '뾗', '뾘', '뾙', '뾚', '뾛', '뾜', '뾝', '뾞', '뾟', '뾠', '뾡', '뾢', '뾣', '뾤', '뾥', '뾦', '뾧', '뾨', '뾩', '뾪', '뾫', '뾬', '뾭', '뾮', '뾯', '뾱', '뾲', '뾳', '뾴', '뾵', '뾶', '뾷', '뾸', '뾹', '뾺', '뾻', '뾼', '뾽', '뾾', '뾿', '뿀', '뿁', '뿂', '뿃', '뿄', '뿆', '뿇', '뿈', '뿉', '뿊', '뿋', '뿎', '뿏', '뿑', '뿒', '뿓', '뿕', '뿖', '뿗', '뿘', '뿙', '뿚', '뿛', '뿝', '뿞', '뿠', '뿢', '뿣', '뿤', '뿥', '뿦', '뿧', '뿨', '뿩', '뿪', '뿫', '뿬', '뿭', '뿮', '뿯', '뿰', '뿱', '뿲', '뿳', '뿴', '뿵', '뿶', '뿷', '뿸', '뿹', '뿺', '뿻', '뿼', '뿽', '뿾', '뿿', '쀀', '쀁', '쀂', '쀃', '쀄', '쀅', '쀆', '쀇', '쀈', '쀉', '쀊', '쀋', '쀌', '쀍', '쀎', '쀏', '쀐', '쀑', '쀒', '쀓', '쀔', '쀕', '쀖', '쀗', '쀘', '쀙', '쀚', '쀛', '쀜', '쀝', '쀞', '쀟', '쀠', '쀡', '쀢', '쀣', '쀤', '쀥', '쀦', '쀧', '쀨', '쀩', '쀪', '쀫', '쀬', '쀭', '쀮', '쀯', '쀰', '쀱', '쀲', '쀳', '쀴', '쀵', '쀶', '쀷', '쀸', '쀹', '쀺', '쀻', '쀽', '쀾', '쀿', '쁀', '쁁', '쁂', '쁃', '쁄', '쁅', '쁆', '쁇', '쁈', '쁉', '쁊', '쁋', '쁌', '쁍', '쁎', '쁏', '쁐', '쁒', '쁓', '쁔', '쁕', '쁖', '쁗', '쁙', '쁚', '쁛', '쁝', '쁞', '쁟', '쁡', '쁢', '쁣', '쁤', '쁥', '쁦', '쁧', '쁪', '쁫', '쁬', '쁭', '쁮', '쁯', '쁰', '쁱', '쁲', '쁳', '쁴', '쁵', '쁶', '쁷', '쁸', '쁹', '쁺', '쁻', '쁼', '쁽', '쁾', '쁿', '삀', '삁', '삂', '삃', '삄', '삅', '삆', '삇', '삈', '삉', '삊', '삋', '삌', '삍', '삎', '삏', '삒', '삓', '삕', '삖', '삗', '삙', '삚', '삛', '삜', '삝', '삞', '삟', '삢', '삤', '삦', '삧', '삨', '삩', '삪', '삫', '삮', '삱', '삲', '삷', '삸', '삹', '삺', '삻', '삾', '샂', '샃', '샄', '샆', '샇', '샊', '샋', '샍', '샎', '샏', '샑', '샒', '샓', '샔', '샕', '샖', '샗', '샚', '샞', '샟', '샠', '샡', '샢', '샣', '샦', '샧', '샩', '샪', '샫', '샭', '샮', '샯', '샰', '샱', '샲', '샳', '샶', '샸', '샺', '샻', '샼', '샽', '샾', '샿', '섁', '섂', '섃', '섅', '섆', '섇', '섉', '섊', '섋', '섌', '섍', '섎', '섏', '섑', '섒', '섓', '섔', '섖', '섗', '섘', '섙', '섚', '섛', '섡', '섢', '섥', '섨', '섩', '섪', '섫', '섮', '섲', '섳', '섴', '섵', '섷', '섺', '섻', '섽', '섾', '섿', '셁', '셂', '셃', '셄', '셅', '셆', '셇', '셊', '셎', '셏', '셐', '셑', '셒', '셓', '셖', '셗', '셙', '셚', '셛', '셝', '셞', '셟', '셠', '셡', '셢', '셣', '셦', '셪', '셫', '셬', '셭', '셮', '셯', '셱', '셲', '셳', '셵', '셶', '셷', '셹', '셺', '셻', '셼', '셽', '셾', '셿', '솀', '솁', '솂', '솃', '솄', '솆', '솇', '솈', '솉', '솊', '솋', '솏', '솑', '솒', '솓', '솕', '솗', '솘', '솙', '솚', '솛', '솞', '솠', '솢', '솣', '솤', '솦', '솧', '솪', '솫', '솭', '솮', '솯', '솱', '솲', '솳', '솴', '솵', '솶', '솷', '솸', '솹', '솺', '솻', '솼', '솾', '솿', '쇀', '쇁', '쇂', '쇃', '쇅', '쇆', '쇇', '쇉', '쇊', '쇋', '쇍', '쇎', '쇏', '쇐', '쇑', '쇒', '쇓', '쇕', '쇖', '쇙', '쇚', '쇛', '쇜', '쇝', '쇞', '쇟', '쇡', '쇢', '쇣', '쇥', '쇦', '쇧', '쇩', '쇪', '쇫', '쇬', '쇭', '쇮', '쇯', '쇲', '쇴', '쇵', '쇶', '쇷', '쇸', '쇹', '쇺', '쇻', '쇾', '쇿', '숁', '숂', '숃', '숅', '숆', '숇', '숈', '숉', '숊', '숋', '숎', '숐', '숒', '숓', '숔', '숕', '숖', '숗', '숚', '숛', '숝', '숞', '숡', '숢', '숣', '숤', '숥', '숦', '숧', '숪', '숬', '숮', '숰', '숳', '숵', '숶', '숷', '숸', '숹', '숺', '숻', '숼', '숽', '숾', '숿', '쉀', '쉁', '쉂', '쉃', '쉄', '쉅', '쉆', '쉇', '쉉', '쉊', '쉋', '쉌', '쉍', '쉎', '쉏', '쉒', '쉓', '쉕', '쉖', '쉗', '쉙', '쉚', '쉛', '쉜', '쉝', '쉞', '쉟', '쉡', '쉢', '쉣', '쉤', '쉦', '쉧', '쉨', '쉩', '쉪', '쉫', '쉮', '쉯', '쉱', '쉲', '쉳', '쉵', '쉶', '쉷', '쉸', '쉹', '쉺', '쉻', '쉾', '슀', '슂', '슃', '슄', '슅', '슆', '슇', '슊', '슋', '슌', '슍', '슎', '슏', '슑', '슒', '슓', '슔', '슕', '슖', '슗', '슙', '슚', '슜', '슞', '슟', '슠', '슡', '슢', '슣', '슦', '슧', '슩', '슪', '슫', '슮', '슯', '슰', '슱', '슲', '슳', '슶', '슸', '슺', '슻', '슼', '슽', '슾', '슿', '싀', '싁', '싂', '싃', '싄', '싅', '싆', '싇', '싈', '싉', '싊', '싋', '싌', '싍', '싎', '싏', '싐', '싑', '싒', '싓', '싔', '싕', '싖', '싗', '싘', '싙', '싚', '싛', '싞', '싟', '싡', '싢', '싥', '싦', '싧', '싨', '싩', '싪', '싮', '싰', '싲', '싳', '싴', '싵', '싷', '싺', '싽', '싾', '싿', '쌁', '쌂', '쌃', '쌄', '쌅', '쌆', '쌇', '쌊', '쌋', '쌎', '쌏', '쌐', '쌑', '쌒', '쌖', '쌗', '쌙', '쌚', '쌛', '쌝', '쌞', '쌟', '쌠', '쌡', '쌢', '쌣', '쌦', '쌧', '쌪', '쌫', '쌬', '쌭', '쌮', '쌯', '쌰', '쌱', '쌲', '쌳', '쌴', '쌵', '쌶', '쌷', '쌸', '쌹', '쌺', '쌻', '쌼', '쌽', '쌾', '쌿', '썀', '썁', '썂', '썃', '썄', '썆', '썇', '썈', '썉', '썊', '썋', '썌', '썍', '썎', '썏', '썐', '썑', '썒', '썓', '썔', '썕', '썖', '썗', '썘', '썙', '썚', '썛', '썜', '썝', '썞', '썟', '썠', '썡', '썢', '썣', '썤', '썥', '썦', '썧', '썪', '썫', '썭', '썮', '썯', '썱', '썳', '썴', '썵', '썶', '썷', '썺', '썻', '썾', '썿', '쎀', '쎁', '쎂', '쎃', '쎅', '쎆', '쎇', '쎉', '쎊', '쎋', '쎍', '쎎', '쎏', '쎐', '쎑', '쎒', '쎓', '쎔', '쎕', '쎖', '쎗', '쎘', '쎙', '쎚', '쎛', '쎜', '쎝', '쎞', '쎟', '쎠', '쎡', '쎢', '쎣', '쎤', '쎥', '쎦', '쎧', '쎨', '쎩', '쎪', '쎫', '쎬', '쎭', '쎮', '쎯', '쎰', '쎱', '쎲', '쎳', '쎴', '쎵', '쎶', '쎷', '쎸', '쎹', '쎺', '쎻', '쎼', '쎽', '쎾', '쎿', '쏁', '쏂', '쏃', '쏄', '쏅', '쏆', '쏇', '쏈', '쏉', '쏊', '쏋', '쏌', '쏍', '쏎', '쏏', '쏐', '쏑', '쏒', '쏓', '쏔', '쏕', '쏖', '쏗', '쏚', '쏛', '쏝', '쏞', '쏡', '쏣', '쏤', '쏥', '쏦', '쏧', '쏪', '쏫', '쏬', '쏮', '쏯', '쏰', '쏱', '쏲', '쏳', '쏶', '쏷', '쏹', '쏺', '쏻', '쏼', '쏽', '쏾', '쏿', '쐀', '쐁', '쐂', '쐃', '쐄', '쐅', '쐆', '쐇', '쐉', '쐊', '쐋', '쐌', '쐍', '쐎', '쐏', '쐑', '쐒', '쐓', '쐔', '쐕', '쐖', '쐗', '쐘', '쐙', '쐚', '쐛', '쐜', '쐝', '쐞', '쐟', '쐠', '쐡', '쐢', '쐣', '쐥', '쐦', '쐧', '쐨', '쐩', '쐪', '쐫', '쐭', '쐮', '쐯', '쐱', '쐲', '쐳', '쐵', '쐶', '쐷', '쐸', '쐹', '쐺', '쐻', '쐾', '쐿', '쑀', '쑁', '쑂', '쑃', '쑄', '쑅', '쑆', '쑇', '쑉', '쑊', '쑋', '쑌', '쑍', '쑎', '쑏', '쑐', '쑑', '쑒', '쑓', '쑔', '쑕', '쑖', '쑗', '쑘', '쑙', '쑚', '쑛', '쑜', '쑝', '쑞', '쑟', '쑠', '쑡', '쑢', '쑣', '쑦', '쑧', '쑩', '쑪', '쑫', '쑭', '쑮', '쑯', '쑰', '쑱', '쑲', '쑳', '쑶', '쑷', '쑸', '쑺', '쑻', '쑼', '쑽', '쑾', '쑿', '쒁', '쒂', '쒃', '쒄', '쒅', '쒆', '쒇', '쒈', '쒉', '쒊', '쒋', '쒌', '쒍', '쒎', '쒏', '쒐', '쒑', '쒒', '쒓', '쒕', '쒖', '쒗', '쒘', '쒙', '쒚', '쒛', '쒝', '쒞', '쒟', '쒠', '쒡', '쒢', '쒣', '쒤', '쒥', '쒦', '쒧', '쒨', '쒩', '쒪', '쒫', '쒬', '쒭', '쒮', '쒯', '쒰', '쒱', '쒲', '쒳', '쒴', '쒵', '쒶', '쒷', '쒹', '쒺', '쒻', '쒽', '쒾', '쒿', '쓀', '쓁', '쓂', '쓃', '쓄', '쓅', '쓆', '쓇', '쓈', '쓉', '쓊', '쓋', '쓌', '쓍', '쓎', '쓏', '쓐', '쓑', '쓒', '쓓', '쓔', '쓕', '쓖', '쓗', '쓘', '쓙', '쓚', '쓛', '쓜', '쓝', '쓞', '쓟', '쓠', '쓡', '쓢', '쓣', '쓤', '쓥', '쓦', '쓧', '쓨', '쓪', '쓫', '쓬', '쓭', '쓮', '쓯', '쓲', '쓳', '쓵', '쓶', '쓷', '쓹', '쓻', '쓼', '쓽', '쓾', '씂', '씃', '씄', '씅', '씆', '씇', '씈', '씉', '씊', '씋', '씍', '씎', '씏', '씑', '씒', '씓', '씕', '씖', '씗', '씘', '씙', '씚', '씛', '씝', '씞', '씟', '씠', '씡', '씢', '씣', '씤', '씥', '씦', '씧', '씪', '씫', '씭', '씮', '씯', '씱', '씲', '씳', '씴', '씵', '씶', '씷', '씺', '씼', '씾', '씿', '앀', '앁', '앂', '앃', '앆', '앇', '앋', '앏', '앐', '앑', '앒', '앖', '앚', '앛', '앜', '앟', '앢', '앣', '앥', '앦', '앧', '앩', '앪', '앫', '앬', '앭', '앮', '앯', '앲', '앶', '앷', '앸', '앹', '앺', '앻', '앾', '앿', '얁', '얂', '얃', '얅', '얆', '얈', '얉', '얊', '얋', '얎', '얐', '얒', '얓', '얔', '얖', '얙', '얚', '얛', '얝', '얞', '얟', '얡', '얢', '얣', '얤', '얥', '얦', '얧', '얨', '얪', '얫', '얬', '얭', '얮', '얯', '얰', '얱', '얲', '얳', '얶', '얷', '얺', '얿', '엀', '엁', '엂', '엃', '엋', '엍', '엏', '엒', '엓', '엕', '엖', '엗', '엙', '엚', '엛', '엜', '엝', '엞', '엟', '엢', '엤', '엦', '엧', '엨', '엩', '엪', '엫', '엯', '엱', '엲', '엳', '엵', '엸', '엹', '엺', '엻', '옂', '옃', '옄', '옉', '옊', '옋', '옍', '옎', '옏', '옑', '옒', '옓', '옔', '옕', '옖', '옗', '옚', '옝', '옞', '옟', '옠', '옡', '옢', '옣', '옦', '옧', '옩', '옪', '옫', '옯', '옱', '옲', '옶', '옸', '옺', '옼', '옽', '옾', '옿', '왂', '왃', '왅', '왆', '왇', '왉', '왊', '왋', '왌', '왍', '왎', '왏', '왒', '왖', '왗', '왘', '왙', '왚', '왛', '왞', '왟', '왡', '왢', '왣', '왤', '왥', '왦', '왧', '왨', '왩', '왪', '왫', '왭', '왮', '왰', '왲', '왳', '왴', '왵', '왶', '왷', '왺', '왻', '왽', '왾', '왿', '욁', '욂', '욃', '욄', '욅', '욆', '욇', '욊', '욌', '욎', '욏', '욐', '욑', '욒', '욓', '욖', '욗', '욙', '욚', '욛', '욝', '욞', '욟', '욠', '욡', '욢', '욣', '욦', '욨', '욪', '욫', '욬', '욭', '욮', '욯', '욲', '욳', '욵', '욶', '욷', '욻', '욼', '욽', '욾', '욿', '웂', '웄', '웆', '웇', '웈', '웉', '웊', '웋', '웎', '웏', '웑', '웒', '웓', '웕', '웖', '웗', '웘', '웙', '웚', '웛', '웞', '웟', '웢', '웣', '웤', '웥', '웦', '웧', '웪', '웫', '웭', '웮', '웯', '웱', '웲', '웳', '웴', '웵', '웶', '웷', '웺', '웻', '웼', '웾', '웿', '윀', '윁', '윂', '윃', '윆', '윇', '윉', '윊', '윋', '윍', '윎', '윏', '윐', '윑', '윒', '윓', '윖', '윘', '윚', '윛', '윜', '윝', '윞', '윟', '윢', '윣', '윥', '윦', '윧', '윩', '윪', '윫', '윬', '윭', '윮', '윯', '윲', '윴', '윶', '윸', '윹', '윺', '윻', '윾', '윿', '읁', '읂', '읃', '읅', '읆', '읇', '읈', '읉', '읋', '읎', '읐', '읙', '읚', '읛', '읝', '읞', '읟', '읡', '읢', '읣', '읤', '읥', '읦', '읧', '읩', '읪', '읬', '읭', '읮', '읯', '읰', '읱', '읲', '읳', '읶', '읷', '읹', '읺', '읻', '읿', '잀', '잁', '잂', '잆', '잋', '잌', '잍', '잏', '잒', '잓', '잕', '잙', '잛', '잜', '잝', '잞', '잟', '잢', '잧', '잨', '잩', '잪', '잫', '잮', '잯', '잱', '잲', '잳', '잵', '잶', '잷', '잸', '잹', '잺', '잻', '잾', '쟂', '쟃', '쟄', '쟅', '쟆', '쟇', '쟊', '쟋', '쟍', '쟏', '쟑', '쟒', '쟓', '쟔', '쟕', '쟖', '쟗', '쟙', '쟚', '쟛', '쟜', '쟞', '쟟', '쟠', '쟡', '쟢', '쟣', '쟥', '쟦', '쟧', '쟩', '쟪', '쟫', '쟭', '쟮', '쟯', '쟰', '쟱', '쟲', '쟳', '쟴', '쟵', '쟶', '쟷', '쟸', '쟹', '쟺', '쟻', '쟼', '쟽', '쟾', '쟿', '젂', '젃', '젅', '젆', '젇', '젉', '젋', '젌', '젍', '젎', '젏', '젒', '젔', '젗', '젘', '젙', '젚', '젛', '젞', '젟', '젡', '젢', '젣', '젥', '젦', '젧', '젨', '젩', '젪', '젫', '젮', '젰', '젲', '젳', '젴', '젵', '젶', '젷', '젹', '젺', '젻', '젽', '젾', '젿', '졁', '졂', '졃', '졄', '졅', '졆', '졇', '졊', '졋', '졎', '졏', '졐', '졑', '졒', '졓', '졕', '졖', '졗', '졘', '졙', '졚', '졛', '졜', '졝', '졞', '졟', '졠', '졡', '졢', '졣', '졤', '졥', '졦', '졧', '졨', '졩', '졪', '졫', '졬', '졭', '졮', '졯', '졲', '졳', '졵', '졶', '졷', '졹', '졻', '졼', '졽', '졾', '졿', '좂', '좄', '좈', '좉', '좊', '좎', '좏', '좐', '좑', '좒', '좓', '좕', '좖', '좗', '좘', '좙', '좚', '좛', '좜', '좞', '좠', '좢', '좣', '좤', '좥', '좦', '좧', '좩', '좪', '좫', '좬', '좭', '좮', '좯', '좰', '좱', '좲', '좳', '좴', '좵', '좶', '좷', '좸', '좹', '좺', '좻', '좾', '좿', '죀', '죁', '죂', '죃', '죅', '죆', '죇', '죉', '죊', '죋', '죍', '죎', '죏', '죐', '죑', '죒', '죓', '죖', '죘', '죚', '죛', '죜', '죝', '죞', '죟', '죢', '죣', '죥', '죦', '죧', '죨', '죩', '죪', '죫', '죬', '죭', '죮', '죯', '죰', '죱', '죲', '죳', '죴', '죶', '죷', '죸', '죹', '죺', '죻', '죾', '죿', '줁', '줂', '줃', '줇', '줈', '줉', '줊', '줋', '줎', '줐', '줒', '줓', '줔', '줕', '줖', '줗', '줙', '줚', '줛', '줜', '줝', '줞', '줟', '줠', '줡', '줢', '줣', '줤', '줥', '줦', '줧', '줨', '줩', '줪', '줫', '줭', '줮', '줯', '줰', '줱', '줲', '줳', '줵', '줶', '줷', '줸', '줹', '줺', '줻', '줼', '줽', '줾', '줿', '쥀', '쥁', '쥂', '쥃', '쥄', '쥅', '쥆', '쥇', '쥈', '쥉', '쥊', '쥋', '쥌', '쥍', '쥎', '쥏', '쥒', '쥓', '쥕', '쥖', '쥗', '쥙', '쥚', '쥛', '쥜', '쥝', '쥞', '쥟', '쥢', '쥤', '쥥', '쥦', '쥧', '쥨', '쥩', '쥪', '쥫', '쥭', '쥮', '쥯', '쥱', '쥲', '쥳', '쥵', '쥶', '쥷', '쥸', '쥹', '쥺', '쥻', '쥽', '쥾', '쥿', '즀', '즁', '즂', '즃', '즄', '즅', '즆', '즇', '즊', '즋', '즍', '즎', '즏', '즑', '즒', '즓', '즔', '즕', '즖', '즗', '즚', '즜', '즞', '즟', '즠', '즡', '즢', '즣', '즤', '즥', '즦', '즧', '즨', '즩', '즪', '즫', '즬', '즭', '즮', '즯', '즰', '즱', '즲', '즳', '즴', '즵', '즶', '즷', '즸', '즹', '즺', '즻', '즼', '즽', '즾', '즿', '짂', '짃', '짅', '짆', '짉', '짋', '짌', '짍', '짎', '짏', '짒', '짔', '짗', '짘', '짛', '짞', '짟', '짡', '짣', '짥', '짦', '짨', '짩', '짪', '짫', '짮', '짲', '짳', '짴', '짵', '짶', '짷', '짺', '짻', '짽', '짾', '짿', '쨁', '쨂', '쨃', '쨄', '쨅', '쨆', '쨇', '쨊', '쨎', '쨏', '쨐', '쨑', '쨒', '쨓', '쨕', '쨖', '쨗', '쨙', '쨚', '쨛', '쨜', '쨝', '쨞', '쨟', '쨠', '쨡', '쨢', '쨣', '쨤', '쨥', '쨦', '쨧', '쨨', '쨪', '쨫', '쨬', '쨭', '쨮', '쨯', '쨰', '쨱', '쨲', '쨳', '쨴', '쨵', '쨶', '쨷', '쨸', '쨹', '쨺', '쨻', '쨼', '쨽', '쨾', '쨿', '쩀', '쩁', '쩂', '쩃', '쩄', '쩅', '쩆', '쩇', '쩈', '쩉', '쩊', '쩋', '쩎', '쩏', '쩑', '쩒', '쩓', '쩕', '쩖', '쩗', '쩘', '쩙', '쩚', '쩛', '쩞', '쩢', '쩣', '쩤', '쩥', '쩦', '쩧', '쩩', '쩪', '쩫', '쩬', '쩭', '쩮', '쩯', '쩰', '쩱', '쩲', '쩳', '쩴', '쩵', '쩶', '쩷', '쩸', '쩹', '쩺', '쩻', '쩼', '쩾', '쩿', '쪀', '쪁', '쪂', '쪃', '쪅', '쪆', '쪇', '쪈', '쪉', '쪊', '쪋', '쪌', '쪍', '쪎', '쪏', '쪐', '쪑', '쪒', '쪓', '쪔', '쪕', '쪖', '쪗', '쪙', '쪚', '쪛', '쪜', '쪝', '쪞', '쪟', '쪠', '쪡', '쪢', '쪣', '쪤', '쪥', '쪦', '쪧', '쪨', '쪩', '쪪', '쪫', '쪬', '쪭', '쪮', '쪯', '쪰', '쪱', '쪲', '쪳', '쪴', '쪵', '쪶', '쪷', '쪸', '쪹', '쪺', '쪻', '쪾', '쪿', '쫁', '쫂', '쫃', '쫅', '쫆', '쫇', '쫈', '쫉', '쫊', '쫋', '쫎', '쫐', '쫒', '쫔', '쫕', '쫖', '쫗', '쫚', '쫛', '쫜', '쫝', '쫞', '쫟', '쫡', '쫢', '쫣', '쫤', '쫥', '쫦', '쫧', '쫨', '쫩', '쫪', '쫫', '쫭', '쫮', '쫯', '쫰', '쫱', '쫲', '쫳', '쫵', '쫶', '쫷', '쫸', '쫹', '쫺', '쫻', '쫼', '쫽', '쫾', '쫿', '쬀', '쬁', '쬂', '쬃', '쬄', '쬅', '쬆', '쬇', '쬉', '쬊', '쬋', '쬌', '쬍', '쬎', '쬏', '쬑', '쬒', '쬓', '쬕', '쬖', '쬗', '쬙', '쬚', '쬛', '쬜', '쬝', '쬞', '쬟', '쬢', '쬣', '쬤', '쬥', '쬦', '쬧', '쬨', '쬩', '쬪', '쬫', '쬬', '쬭', '쬮', '쬯', '쬰', '쬱', '쬲', '쬳', '쬴', '쬵', '쬶', '쬷', '쬸', '쬹', '쬺', '쬻', '쬼', '쬽', '쬾', '쬿', '쭀', '쭂', '쭃', '쭄', '쭅', '쭆', '쭇', '쭊', '쭋', '쭍', '쭎', '쭏', '쭑', '쭒', '쭓', '쭔', '쭕', '쭖', '쭗', '쭚', '쭛', '쭜', '쭞', '쭟', '쭠', '쭡', '쭢', '쭣', '쭥', '쭦', '쭧', '쭨', '쭩', '쭪', '쭫', '쭬', '쭭', '쭮', '쭯', '쭰', '쭱', '쭲', '쭳', '쭴', '쭵', '쭶', '쭷', '쭺', '쭻', '쭼', '쭽', '쭾', '쭿', '쮀', '쮁', '쮂', '쮃', '쮄', '쮅', '쮆', '쮇', '쮈', '쮉', '쮊', '쮋', '쮌', '쮍', '쮎', '쮏', '쮐', '쮑', '쮒', '쮓', '쮔', '쮕', '쮖', '쮗', '쮘', '쮙', '쮚', '쮛', '쮝', '쮞', '쮟', '쮠', '쮡', '쮢', '쮣', '쮤', '쮥', '쮦', '쮧', '쮨', '쮩', '쮪', '쮫', '쮬', '쮭', '쮮', '쮯', '쮰', '쮱', '쮲', '쮳', '쮴', '쮵', '쮶', '쮷', '쮹', '쮺', '쮻', '쮼', '쮽', '쮾', '쮿', '쯀', '쯁', '쯂', '쯃', '쯄', '쯅', '쯆', '쯇', '쯈', '쯉', '쯊', '쯋', '쯌', '쯍', '쯎', '쯏', '쯐', '쯑', '쯒', '쯓', '쯕', '쯖', '쯗', '쯘', '쯙', '쯚', '쯛', '쯜', '쯝', '쯞', '쯟', '쯠', '쯡', '쯢', '쯣', '쯥', '쯦', '쯨', '쯪', '쯫', '쯬', '쯭', '쯮', '쯯', '쯰', '쯱', '쯲', '쯳', '쯴', '쯵', '쯶', '쯷', '쯸', '쯹', '쯺', '쯻', '쯼', '쯽', '쯾', '쯿', '찀', '찁', '찂', '찃', '찄', '찅', '찆', '찇', '찈', '찉', '찊', '찋', '찎', '찏', '찑', '찒', '찓', '찕', '찖', '찗', '찘', '찙', '찚', '찛', '찞', '찟', '찠', '찣', '찤', '찥', '찦', '찪', '찫', '찭', '찯', '찱', '찲', '찳', '찴', '찵', '찶', '찷', '찺', '찿', '챀', '챁', '챂', '챃', '챆', '챇', '챉', '챊', '챋', '챍', '챎', '챏', '챐', '챑', '챒', '챓', '챖', '챚', '챛', '챜', '챝', '챞', '챟', '챡', '챢', '챣', '챥', '챧', '챩', '챪', '챫', '챬', '챭', '챮', '챯', '챱', '챲', '챳', '챴', '챶', '챷', '챸', '챹', '챺', '챻', '챼', '챽', '챾', '챿', '첀', '첁', '첂', '첃', '첄', '첅', '첆', '첇', '첈', '첉', '첊', '첋', '첌', '첍', '첎', '첏', '첐', '첑', '첒', '첓', '첔', '첕', '첖', '첗', '첚', '첛', '첝', '첞', '첟', '첡', '첢', '첣', '첤', '첥', '첦', '첧', '첪', '첮', '첯', '첰', '첱', '첲', '첳', '첶', '첷', '첹', '첺', '첻', '첽', '첾', '첿', '쳀', '쳁', '쳂', '쳃', '쳆', '쳈', '쳊', '쳋', '쳌', '쳍', '쳎', '쳏', '쳑', '쳒', '쳓', '쳕', '쳖', '쳗', '쳘', '쳙', '쳚', '쳛', '쳜', '쳝', '쳞', '쳟', '쳠', '쳡', '쳢', '쳣', '쳥', '쳦', '쳧', '쳨', '쳩', '쳪', '쳫', '쳭', '쳮', '쳯', '쳱', '쳲', '쳳', '쳴', '쳵', '쳶', '쳷', '쳸', '쳹', '쳺', '쳻', '쳼', '쳽', '쳾', '쳿', '촀', '촂', '촃', '촄', '촅', '촆', '촇', '촊', '촋', '촍', '촎', '촏', '촑', '촒', '촓', '촔', '촕', '촖', '촗', '촚', '촜', '촞', '촟', '촠', '촡', '촢', '촣', '촥', '촦', '촧', '촩', '촪', '촫', '촭', '촮', '촯', '촰', '촱', '촲', '촳', '촴', '촵', '촶', '촷', '촸', '촺', '촻', '촼', '촽', '촾', '촿', '쵀', '쵁', '쵂', '쵃', '쵄', '쵅', '쵆', '쵇', '쵈', '쵉', '쵊', '쵋', '쵌', '쵍', '쵎', '쵏', '쵐', '쵑', '쵒', '쵓', '쵔', '쵕', '쵖', '쵗', '쵘', '쵙', '쵚', '쵛', '쵝', '쵞', '쵟', '쵡', '쵢', '쵣', '쵥', '쵦', '쵧', '쵨', '쵩', '쵪', '쵫', '쵮', '쵰', '쵲', '쵳', '쵴', '쵵', '쵶', '쵷', '쵹', '쵺', '쵻', '쵼', '쵽', '쵾', '쵿', '춀', '춁', '춂', '춃', '춄', '춅', '춆', '춇', '춉', '춊', '춋', '춌', '춍', '춎', '춏', '춐', '춑', '춒', '춓', '춖', '춗', '춙', '춚', '춛', '춝', '춞', '춟', '춠', '춡', '춢', '춣', '춦', '춨', '춪', '춫', '춬', '춭', '춮', '춯', '춱', '춲', '춳', '춴', '춵', '춶', '춷', '춸', '춹', '춺', '춻', '춼', '춽', '춾', '춿', '췀', '췁', '췂', '췃', '췅', '췆', '췇', '췈', '췉', '췊', '췋', '췍', '췎', '췏', '췑', '췒', '췓', '췔', '췕', '췖', '췗', '췘', '췙', '췚', '췛', '췜', '췝', '췞', '췟', '췠', '췡', '췢', '췣', '췤', '췥', '췦', '췧', '췩', '췪', '췫', '췭', '췮', '췯', '췱', '췲', '췳', '췴', '췵', '췶', '췷', '췺', '췼', '췾', '췿', '츀', '츁', '츂', '츃', '츅', '츆', '츇', '츉', '츊', '츋', '츍', '츎', '츏', '츐', '츑', '츒', '츓', '츕', '츖', '츗', '츘', '츚', '츛', '츜', '츝', '츞', '츟', '츢', '츣', '츥', '츦', '츧', '츩', '츪', '츫', '츬', '츭', '츮', '츯', '츲', '츴', '츶', '츷', '츸', '츹', '츺', '츻', '츼', '츽', '츾', '츿', '칀', '칁', '칂', '칃', '칄', '칅', '칆', '칇', '칈', '칉', '칊', '칋', '칌', '칍', '칎', '칏', '칐', '칑', '칒', '칓', '칔', '칕', '칖', '칗', '칚', '칛', '칝', '칞', '칢', '칣', '칤', '칥', '칦', '칧', '칪', '칬', '칮', '칯', '칰', '칱', '칲', '칳', '칶', '칷', '칹', '칺', '칻', '칽', '칾', '칿', '캀', '캁', '캂', '캃', '캆', '캈', '캊', '캋', '캌', '캍', '캎', '캏', '캒', '캓', '캕', '캖', '캗', '캙', '캚', '캛', '캜', '캝', '캞', '캟', '캢', '캦', '캧', '캨', '캩', '캪', '캫', '캮', '캯', '캰', '캱', '캲', '캳', '캴', '캵', '캶', '캷', '캸', '캹', '캺', '캻', '캼', '캽', '캾', '캿', '컀', '컂', '컃', '컄', '컅', '컆', '컇', '컈', '컉', '컊', '컋', '컌', '컍', '컎', '컏', '컐', '컑', '컒', '컓', '컔', '컕', '컖', '컗', '컘', '컙', '컚', '컛', '컜', '컝', '컞', '컟', '컠', '컡', '컢', '컣', '컦', '컧', '컩', '컪', '컭', '컮', '컯', '컰', '컱', '컲', '컳', '컶', '컺', '컻', '컼', '컽', '컾', '컿', '켂', '켃', '켅', '켆', '켇', '켉', '켊', '켋', '켌', '켍', '켎', '켏', '켒', '켔', '켖', '켗', '켘', '켙', '켚', '켛', '켝', '켞', '켟', '켡', '켢', '켣', '켥', '켦', '켧', '켨', '켩', '켪', '켫', '켮', '켲', '켳', '켴', '켵', '켶', '켷', '켹', '켺', '켻', '켼', '켽', '켾', '켿', '콀', '콁', '콂', '콃', '콄', '콅', '콆', '콇', '콈', '콉', '콊', '콋', '콌', '콍', '콎', '콏', '콐', '콑', '콒', '콓', '콖', '콗', '콙', '콚', '콛', '콝', '콞', '콟', '콠', '콡', '콢', '콣', '콦', '콨', '콪', '콫', '콬', '콭', '콮', '콯', '콲', '콳', '콵', '콶', '콷', '콹', '콺', '콻', '콼', '콽', '콾', '콿', '쾁', '쾂', '쾃', '쾄', '쾆', '쾇', '쾈', '쾉', '쾊', '쾋', '쾍', '쾎', '쾏', '쾐', '쾑', '쾒', '쾓', '쾔', '쾕', '쾖', '쾗', '쾘', '쾙', '쾚', '쾛', '쾜', '쾝', '쾞', '쾟', '쾠', '쾢', '쾣', '쾤', '쾥', '쾦', '쾧', '쾩', '쾪', '쾫', '쾬', '쾭', '쾮', '쾯', '쾱', '쾲', '쾳', '쾴', '쾵', '쾶', '쾷', '쾸', '쾹', '쾺', '쾻', '쾼', '쾽', '쾾', '쾿', '쿀', '쿁', '쿂', '쿃', '쿅', '쿆', '쿇', '쿈', '쿉', '쿊', '쿋', '쿌', '쿍', '쿎', '쿏', '쿐', '쿑', '쿒', '쿓', '쿔', '쿕', '쿖', '쿗', '쿘', '쿙', '쿚', '쿛', '쿜', '쿝', '쿞', '쿟', '쿢', '쿣', '쿥', '쿦', '쿧', '쿩', '쿪', '쿫', '쿬', '쿭', '쿮', '쿯', '쿲', '쿴', '쿶', '쿷', '쿸', '쿹', '쿺', '쿻', '쿽', '쿾', '쿿', '퀁', '퀂', '퀃', '퀅', '퀆', '퀇', '퀈', '퀉', '퀊', '퀋', '퀌', '퀍', '퀎', '퀏', '퀐', '퀒', '퀓', '퀔', '퀕', '퀖', '퀗', '퀙', '퀚', '퀛', '퀜', '퀝', '퀞', '퀟', '퀠', '퀡', '퀢', '퀣', '퀤', '퀥', '퀦', '퀧', '퀨', '퀩', '퀪', '퀫', '퀬', '퀮', '퀯', '퀰', '퀱', '퀲', '퀳', '퀶', '퀷', '퀹', '퀺', '퀻', '퀽', '퀾', '퀿', '큀', '큁', '큂', '큃', '큆', '큈', '큊', '큋', '큌', '큍', '큎', '큏', '큑', '큒', '큓', '큕', '큖', '큗', '큙', '큚', '큛', '큜', '큝', '큞', '큟', '큡', '큢', '큣', '큤', '큥', '큦', '큧', '큨', '큩', '큪', '큫', '큮', '큯', '큱', '큲', '큳', '큵', '큶', '큷', '큸', '큹', '큺', '큻', '큾', '큿', '킀', '킂', '킃', '킄', '킅', '킆', '킇', '킈', '킉', '킊', '킋', '킌', '킍', '킎', '킏', '킐', '킑', '킒', '킓', '킔', '킕', '킖', '킗', '킘', '킙', '킚', '킛', '킜', '킝', '킞', '킟', '킠', '킡', '킢', '킣', '킦', '킧', '킩', '킪', '킫', '킭', '킮', '킯', '킰', '킱', '킲', '킳', '킶', '킸', '킺', '킻', '킼', '킽', '킾', '킿', '탂', '탃', '탅', '탆', '탇', '탊', '탋', '탌', '탍', '탎', '탏', '탒', '탖', '탗', '탘', '탙', '탚', '탛', '탞', '탟', '탡', '탢', '탣', '탥', '탦', '탧', '탨', '탩', '탪', '탫', '탮', '탲', '탳', '탴', '탵', '탶', '탷', '탹', '탺', '탻', '탼', '탽', '탾', '탿', '턀', '턁', '턂', '턃', '턄', '턅', '턆', '턇', '턈', '턉', '턊', '턋', '턌', '턎', '턏', '턐', '턑', '턒', '턓', '턔', '턕', '턖', '턗', '턘', '턙', '턚', '턛', '턜', '턝', '턞', '턟', '턠', '턡', '턢', '턣', '턤', '턥', '턦', '턧', '턨', '턩', '턪', '턫', '턬', '턭', '턮', '턯', '턲', '턳', '턵', '턶', '턷', '턹', '턻', '턼', '턽', '턾', '턿', '텂', '텆', '텇', '텈', '텉', '텊', '텋', '텎', '텏', '텑', '텒', '텓', '텕', '텖', '텗', '텘', '텙', '텚', '텛', '텞', '텠', '텢', '텣', '텤', '텥', '텦', '텧', '텩', '텪', '텫', '텭', '텮', '텯', '텰', '텱', '텲', '텳', '텴', '텵', '텶', '텷', '텸', '텹', '텺', '텻', '텽', '텾', '텿', '톀', '톁', '톂', '톃', '톅', '톆', '톇', '톉', '톊', '톋', '톌', '톍', '톎', '톏', '톐', '톑', '톒', '톓', '톔', '톕', '톖', '톗', '톘', '톙', '톚', '톛', '톜', '톝', '톞', '톟', '톢', '톣', '톥', '톦', '톧', '톩', '톪', '톫', '톬', '톭', '톮', '톯', '톲', '톴', '톶', '톷', '톸', '톹', '톻', '톽', '톾', '톿', '퇁', '퇂', '퇃', '퇄', '퇅', '퇆', '퇇', '퇈', '퇉', '퇊', '퇋', '퇌', '퇍', '퇎', '퇏', '퇐', '퇑', '퇒', '퇓', '퇔', '퇕', '퇖', '퇗', '퇙', '퇚', '퇛', '퇜', '퇝', '퇞', '퇟', '퇠', '퇡', '퇢', '퇣', '퇤', '퇥', '퇦', '퇧', '퇨', '퇩', '퇪', '퇫', '퇬', '퇭', '퇮', '퇯', '퇰', '퇱', '퇲', '퇳', '퇵', '퇶', '퇷', '퇹', '퇺', '퇻', '퇼', '퇽', '퇾', '퇿', '툀', '툁', '툂', '툃', '툄', '툅', '툆', '툈', '툊', '툋', '툌', '툍', '툎', '툏', '툑', '툒', '툓', '툔', '툕', '툖', '툗', '툘', '툙', '툚', '툛', '툜', '툝', '툞', '툟', '툠', '툡', '툢', '툣', '툤', '툥', '툦', '툧', '툨', '툩', '툪', '툫', '툮', '툯', '툱', '툲', '툳', '툵', '툶', '툷', '툸', '툹', '툺', '툻', '툾', '퉀', '퉂', '퉃', '퉄', '퉅', '퉆', '퉇', '퉉', '퉊', '퉋', '퉌', '퉍', '퉎', '퉏', '퉐', '퉑', '퉒', '퉓', '퉔', '퉕', '퉖', '퉗', '퉘', '퉙', '퉚', '퉛', '퉝', '퉞', '퉟', '퉠', '퉡', '퉢', '퉣', '퉥', '퉦', '퉧', '퉨', '퉩', '퉪', '퉫', '퉬', '퉭', '퉮', '퉯', '퉰', '퉱', '퉲', '퉳', '퉴', '퉵', '퉶', '퉷', '퉸', '퉹', '퉺', '퉻', '퉼', '퉽', '퉾', '퉿', '튂', '튃', '튅', '튆', '튇', '튉', '튊', '튋', '튌', '튍', '튎', '튏', '튒', '튓', '튔', '튖', '튗', '튘', '튙', '튚', '튛', '튝', '튞', '튟', '튡', '튢', '튣', '튥', '튦', '튧', '튨', '튩', '튪', '튫', '튭', '튮', '튯', '튰', '튲', '튳', '튴', '튵', '튶', '튷', '튺', '튻', '튽', '튾', '틁', '틃', '틄', '틅', '틆', '틇', '틊', '틌', '틍', '틎', '틏', '틐', '틑', '틒', '틓', '틕', '틖', '틗', '틙', '틚', '틛', '틝', '틞', '틟', '틠', '틡', '틢', '틣', '틦', '틧', '틨', '틩', '틪', '틫', '틬', '틭', '틮', '틯', '틲', '틳', '틵', '틶', '틷', '틹', '틺', '틻', '틼', '틽', '틾', '틿', '팂', '팄', '팆', '팇', '팈', '팉', '팊', '팋', '팏', '팑', '팒', '팓', '팕', '팗', '팘', '팙', '팚', '팛', '팞', '팢', '팣', '팤', '팦', '팧', '팪', '팫', '팭', '팮', '팯', '팱', '팲', '팳', '팴', '팵', '팶', '팷', '팺', '팾', '팿', '퍀', '퍁', '퍂', '퍃', '퍆', '퍇', '퍈', '퍉', '퍊', '퍋', '퍌', '퍍', '퍎', '퍏', '퍐', '퍑', '퍒', '퍓', '퍔', '퍕', '퍖', '퍗', '퍘', '퍙', '퍚', '퍛', '퍜', '퍝', '퍞', '퍟', '퍠', '퍡', '퍢', '퍣', '퍤', '퍥', '퍦', '퍧', '퍨', '퍩', '퍪', '퍫', '퍬', '퍭', '퍮', '퍯', '퍰', '퍱', '퍲', '퍳', '퍴', '퍵', '퍶', '퍷', '퍸', '퍹', '퍺', '퍻', '퍾', '퍿', '펁', '펂', '펃', '펅', '펆', '펇', '펈', '펉', '펊', '펋', '펎', '펒', '펓', '펔', '펕', '펖', '펗', '펚', '펛', '펝', '펞', '펟', '펡', '펢', '펣', '펤', '펥', '펦', '펧', '펪', '펬', '펮', '펯', '펰', '펱', '펲', '펳', '펵', '펶', '펷', '펹', '펺', '펻', '펽', '펾', '펿', '폀', '폁', '폂', '폃', '폆', '폇', '폊', '폋', '폌', '폍', '폎', '폏', '폑', '폒', '폓', '폔', '폕', '폖', '폗', '폙', '폚', '폛', '폜', '폝', '폞', '폟', '폠', '폢', '폤', '폥', '폦', '폧', '폨', '폩', '폪', '폫', '폮', '폯', '폱', '폲', '폳', '폵', '폶', '폷', '폸', '폹', '폺', '폻', '폾', '퐀', '퐂', '퐃', '퐄', '퐅', '퐆', '퐇', '퐉', '퐊', '퐋', '퐌', '퐍', '퐎', '퐏', '퐐', '퐑', '퐒', '퐓', '퐔', '퐕', '퐖', '퐗', '퐘', '퐙', '퐚', '퐛', '퐜', '퐞', '퐟', '퐠', '퐡', '퐢', '퐣', '퐤', '퐥', '퐦', '퐧', '퐨', '퐩', '퐪', '퐫', '퐬', '퐭', '퐮', '퐯', '퐰', '퐱', '퐲', '퐳', '퐴', '퐵', '퐶', '퐷', '퐸', '퐹', '퐺', '퐻', '퐼', '퐽', '퐾', '퐿', '푁', '푂', '푃', '푅', '푆', '푇', '푈', '푉', '푊', '푋', '푌', '푍', '푎', '푏', '푐', '푑', '푒', '푓', '푔', '푕', '푖', '푗', '푘', '푙', '푚', '푛', '푝', '푞', '푟', '푡', '푢', '푣', '푥', '푦', '푧', '푨', '푩', '푪', '푫', '푬', '푮', '푰', '푱', '푲', '푳', '푴', '푵', '푶', '푷', '푺', '푻', '푽', '푾', '풁', '풃', '풄', '풅', '풆', '풇', '풊', '풌', '풎', '풏', '풐', '풑', '풒', '풓', '풕', '풖', '풗', '풘', '풙', '풚', '풛', '풜', '풝', '풞', '풟', '풠', '풡', '풢', '풣', '풤', '풥', '풦', '풧', '풨', '풪', '풫', '풬', '풭', '풮', '풯', '풰', '풱', '풲', '풳', '풴', '풵', '풶', '풷', '풸', '풹', '풺', '풻', '풼', '풽', '풾', '풿', '퓀', '퓁', '퓂', '퓃', '퓄', '퓅', '퓆', '퓇', '퓈', '퓉', '퓊', '퓋', '퓍', '퓎', '퓏', '퓑', '퓒', '퓓', '퓕', '퓖', '퓗', '퓘', '퓙', '퓚', '퓛', '퓝', '퓞', '퓠', '퓡', '퓢', '퓣', '퓤', '퓥', '퓦', '퓧', '퓩', '퓪', '퓫', '퓭', '퓮', '퓯', '퓱', '퓲', '퓳', '퓴', '퓵', '퓶', '퓷', '퓹', '퓺', '퓼', '퓾', '퓿', '픀', '픁', '픂', '픃', '픅', '픆', '픇', '픉', '픊', '픋', '픍', '픎', '픏', '픐', '픑', '픒', '픓', '픖', '픘', '픙', '픚', '픛', '픜', '픝', '픞', '픟', '픠', '픡', '픢', '픣', '픤', '픥', '픦', '픧', '픨', '픩', '픪', '픫', '픬', '픭', '픮', '픯', '픰', '픱', '픲', '픳', '픴', '픵', '픶', '픷', '픸', '픹', '픺', '픻', '픾', '픿', '핁', '핂', '핃', '핅', '핆', '핇', '핈', '핉', '핊', '핋', '핎', '핐', '핒', '핓', '핔', '핕', '핖', '핗', '핚', '핛', '핝', '핞', '핟', '핡', '핢', '핣', '핤', '핦', '핧', '핪', '핬', '핮', '핯', '핰', '핱', '핲', '핳', '핶', '핷', '핹', '핺', '핻', '핽', '핾', '핿', '햀', '햁', '햂', '햃', '햆', '햊', '햋', '햌', '햍', '햎', '햏', '햑', '햒', '햓', '햔', '햕', '햖', '햗', '햘', '햙', '햚', '햛', '햜', '햝', '햞', '햟', '햠', '햡', '햢', '햣', '햤', '햦', '햧', '햨', '햩', '햪', '햫', '햬', '햭', '햮', '햯', '햰', '햱', '햲', '햳', '햴', '햵', '햶', '햷', '햸', '햹', '햺', '햻', '햼', '햽', '햾', '햿', '헀', '헁', '헂', '헃', '헄', '헅', '헆', '헇', '헊', '헋', '헍', '헎', '헏', '헑', '헓', '헔', '헕', '헖', '헗', '헚', '헜', '헞', '헟', '헠', '헡', '헢', '헣', '헦', '헧', '헩', '헪', '헫', '헭', '헮', '헯', '헰', '헱', '헲', '헳', '헶', '헸', '헺', '헻', '헼', '헽', '헾', '헿', '혂', '혃', '혅', '혆', '혇', '혉', '혊', '혋', '혌', '혍', '혎', '혏', '혒', '혖', '혗', '혘', '혙', '혚', '혛', '혝', '혞', '혟', '혡', '혢', '혣', '혥', '혦', '혧', '혨', '혩', '혪', '혫', '혬', '혮', '혯', '혰', '혱', '혲', '혳', '혴', '혵', '혶', '혷', '혺', '혻', '혽', '혾', '혿', '홁', '홂', '홃', '홄', '홆', '홇', '홊', '홌', '홎', '홏', '홐', '홒', '홓', '홖', '홗', '홙', '홚', '홛', '홝', '홞', '홟', '홠', '홡', '홢', '홣', '홤', '홥', '홦', '홨', '홪', '홫', '홬', '홭', '홮', '홯', '홲', '홳', '홵', '홶', '홷', '홸', '홹', '홺', '홻', '홼', '홽', '홾', '홿', '횀', '횁', '횂', '횄', '횆', '횇', '횈', '횉', '횊', '횋', '횎', '횏', '횑', '횒', '횓', '횕', '횖', '횗', '횘', '횙', '횚', '횛', '횜', '횞', '횠', '횢', '횣', '횤', '횥', '횦', '횧', '횩', '횪', '횫', '횭', '횮', '횯', '횱', '횲', '횳', '횴', '횵', '횶', '횷', '횸', '횺', '횼', '횽', '횾', '횿', '훀', '훁', '훂', '훃', '훆', '훇', '훉', '훊', '훋', '훍', '훎', '훏', '훐', '훒', '훓', '훕', '훖', '훘', '훚', '훛', '훜', '훝', '훞', '훟', '훡', '훢', '훣', '훥', '훦', '훧', '훩', '훪', '훫', '훬', '훭', '훮', '훯', '훱', '훲', '훳', '훴', '훶', '훷', '훸', '훹', '훺', '훻', '훾', '훿', '휁', '휂', '휃', '휅', '휆', '휇', '휈', '휉', '휊', '휋', '휌', '휍', '휎', '휏', '휐', '휒', '휓', '휔', '휕', '휖', '휗', '휚', '휛', '휝', '휞', '휟', '휡', '휢', '휣', '휤', '휥', '휦', '휧', '휪', '휬', '휮', '휯', '휰', '휱', '휲', '휳', '휶', '휷', '휹', '휺', '휻', '휽', '휾', '휿', '흀', '흁', '흂', '흃', '흅', '흆', '흈', '흊', '흋', '흌', '흍', '흎', '흏', '흒', '흓', '흕', '흚', '흛', '흜', '흝', '흞', '흟', '흢', '흤', '흦', '흧', '흨', '흪', '흫', '흭', '흮', '흯', '흱', '흲', '흳', '흵', '흶', '흷', '흸', '흹', '흺', '흻', '흾', '흿', '힀', '힂', '힃', '힄', '힅', '힆', '힇', '힊', '힋', '힍', '힎', '힏', '힑', '힒', '힓', '힔', '힕', '힖', '힗', '힚', '힜', '힞', '힟', '힠', '힡', '힢', '힣', '\ud7a4']
+['가', '각', '간', '갇', '갈', '갉', '갊', '감', '갑', '값', '갓', '갔', '강', '갖', '갗', '같', '갚', '갛', '개', '객', '갠', '갤', '갬', '갭', '갯', '갰', '갱', '갸', '갹', '갼', '걀', '걋', '걍', '걔', '걘', '걜', '거', '걱', '건', '걷', '걸', '걺', '검', '겁', '것', '겄', '겅', '겆', '겉', '겊', '겋', '게', '겐', '겔', '겜', '겝', '겟', '겠', '겡', '겨', '격', '겪', '견', '겯', '결', '겸', '겹', '겻', '겼', '경', '곁', '계', '곈', '곌', '곕', '곗', '고', '곡', '곤', '곧', '골', '곪', '곬', '곯', '곰', '곱', '곳', '공', '곶', '과', '곽', '관', '괄', '괆', '괌', '괍', '괏', '광', '괘', '괜', '괠', '괩', '괬', '괭', '괴', '괵', '괸', '괼', '굄', '굅', '굇', '굉', '교', '굔', '굘', '굡', '굣', '구', '국', '군', '굳', '굴', '굵', '굶', '굻', '굼', '굽', '굿', '궁', '궂', '궈', '궉', '권', '궐', '궜', '궝', '궤', '궷', '귀', '귁', '귄', '귈', '귐', '귑', '귓', '규', '균', '귤', '그', '극', '근', '귿', '글', '긁', '금', '급', '긋', '긍', '긔', '기', '긱', '긴', '긷', '길', '긺', '김', '깁', '깃', '깅', '깆', '깊', '까', '깍', '깎', '깐', '깔', '깖', '깜', '깝', '깟', '깠', '깡', '깥', '깨', '깩', '깬', '깰', '깸', '깹', '깻', '깼', '깽', '꺄', '꺅', '꺌', '꺼', '꺽', '꺾', '껀', '껄', '껌', '껍', '껏', '껐', '껑', '께', '껙', '껜', '껨', '껫', '껭', '껴', '껸', '껼', '꼇', '꼈', '꼍', '꼐', '꼬', '꼭', '꼰', '꼲', '꼴', '꼼', '꼽', '꼿', '꽁', '꽂', '꽃', '꽈', '꽉', '꽐', '꽜', '꽝', '꽤', '꽥', '꽹', '꾀', '꾄', '꾈', '꾐', '꾑', '꾕', '꾜', '꾸', '꾹', '꾼', '꿀', '꿇', '꿈', '꿉', '꿋', '꿍', '꿎', '꿔', '꿜', '꿨', '꿩', '꿰', '꿱', '꿴', '꿸', '뀀', '뀁', '뀄', '뀌', '뀐', '뀔', '뀜', '뀝', '뀨', '끄', '끅', '끈', '끊', '끌', '끎', '끓', '끔', '끕', '끗', '끙', '끝', '끼', '끽', '낀', '낄', '낌', '낍', '낏', '낑', '나', '낙', '낚', '난', '낟', '날', '낡', '낢', '남', '납', '낫', '났', '낭', '낮', '낯', '낱', '낳', '내', '낵', '낸', '낼', '냄', '냅', '냇', '냈', '냉', '냐', '냑', '냔', '냘', '냠', '냥', '너', '넉', '넋', '넌', '널', '넒', '넓', '넘', '넙', '넛', '넜', '넝', '넣', '네', '넥', '넨', '넬', '넴', '넵', '넷', '넸', '넹', '녀', '녁', '년', '녈', '념', '녑', '녔', '녕', '녘', '녜', '녠', '노', '녹', '논', '놀', '놂', '놈', '놉', '놋', '농', '높', '놓', '놔', '놘', '놜', '놨', '뇌', '뇐', '뇔', '뇜', '뇝', '뇟', '뇨', '뇩', '뇬', '뇰', '뇹', '뇻', '뇽', '누', '눅', '눈', '눋', '눌', '눔', '눕', '눗', '눙', '눠', '눴', '눼', '뉘', '뉜', '뉠', '뉨', '뉩', '뉴', '뉵', '뉼', '늄', '늅', '늉', '느', '늑', '는', '늘', '늙', '늚', '늠', '늡', '늣', '능', '늦', '늪', '늬', '늰', '늴', '니', '닉', '닌', '닐', '닒', '님', '닙', '닛', '닝', '닢', '다', '닥', '닦', '단', '닫', '달', '닭', '닮', '닯', '닳', '담', '답', '닷', '닸', '당', '닺', '닻', '닿', '대', '댁', '댄', '댈', '댐', '댑', '댓', '댔', '댕', '댜', '더', '덕', '덖', '던', '덛', '덜', '덞', '덟', '덤', '덥', '덧', '덩', '덫', '덮', '데', '덱', '덴', '델', '뎀', '뎁', '뎃', '뎄', '뎅', '뎌', '뎐', '뎔', '뎠', '뎡', '뎨', '뎬', '도', '독', '돈', '돋', '돌', '돎', '돐', '돔', '돕', '돗', '동', '돛', '돝', '돠', '돤', '돨', '돼', '됐', '되', '된', '될', '됨', '됩', '됫', '됴', '두', '둑', '둔', '둘', '둠', '둡', '둣', '둥', '둬', '뒀', '뒈', '뒝', '뒤', '뒨', '뒬', '뒵', '뒷', '뒹', '듀', '듄', '듈', '듐', '듕', '드', '득', '든', '듣', '들', '듦', '듬', '듭', '듯', '등', '듸', '디', '딕', '딘', '딛', '딜', '딤', '딥', '딧', '딨', '딩', '딪', '따', '딱', '딴', '딸', '땀', '땁', '땃', '땄', '땅', '땋', '때', '땍', '땐', '땔', '땜', '땝', '땟', '땠', '땡', '떠', '떡', '떤', '떨', '떪', '떫', '떰', '떱', '떳', '떴', '떵', '떻', '떼', '떽', '뗀', '뗄', '뗌', '뗍', '뗏', '뗐', '뗑', '뗘', '뗬', '또', '똑', '똔', '똘', '똥', '똬', '똴', '뙈', '뙤', '뙨', '뚜', '뚝', '뚠', '뚤', '뚫', '뚬', '뚱', '뛔', '뛰', '뛴', '뛸', '뜀', '뜁', '뜅', '뜨', '뜩', '뜬', '뜯', '뜰', '뜸', '뜹', '뜻', '띄', '띈', '띌', '띔', '띕', '띠', '띤', '띨', '띰', '띱', '띳', '띵', '라', '락', '란', '랄', '람', '랍', '랏', '랐', '랑', '랒', '랖', '랗', '래', '랙', '랜', '랠', '램', '랩', '랫', '랬', '랭', '랴', '략', '랸', '럇', '량', '러', '럭', '런', '럴', '럼', '럽', '럿', '렀', '렁', '렇', '레', '렉', '렌', '렐', '렘', '렙', '렛', '렝', '려', '력', '련', '렬', '렴', '렵', '렷', '렸', '령', '례', '롄', '롑', '롓', '로', '록', '론', '롤', '롬', '롭', '롯', '롱', '롸', '롼', '뢍', '뢨', '뢰', '뢴', '뢸', '룀', '룁', '룃', '룅', '료', '룐', '룔', '룝', '룟', '룡', '루', '룩', '룬', '룰', '룸', '룹', '룻', '룽', '뤄', '뤘', '뤠', '뤼', '뤽', '륀', '륄', '륌', '륏', '륑', '류', '륙', '륜', '률', '륨', '륩', '륫', '륭', '르', '륵', '른', '를', '름', '릅', '릇', '릉', '릊', '릍', '릎', '리', '릭', '린', '릴', '림', '립', '릿', '링', '마', '막', '만', '많', '맏', '말', '맑', '맒', '맘', '맙', '맛', '망', '맞', '맡', '맣', '매', '맥', '맨', '맬', '맴', '맵', '맷', '맸', '맹', '맺', '먀', '먁', '먈', '먕', '머', '먹', '먼', '멀', '멂', '멈', '멉', '멋', '멍', '멎', '멓', '메', '멕', '멘', '멜', '멤', '멥', '멧', '멨', '멩', '며', '멱', '면', '멸', '몃', '몄', '명', '몇', '몌', '모', '목', '몫', '몬', '몰', '몲', '몸', '몹', '못', '몽', '뫄', '뫈', '뫘', '뫙', '뫼', '묀', '묄', '묍', '묏', '묑', '묘', '묜', '묠', '묩', '묫', '무', '묵', '묶', '문', '묻', '물', '묽', '묾', '뭄', '뭅', '뭇', '뭉', '뭍', '뭏', '뭐', '뭔', '뭘', '뭡', '뭣', '뭬', '뮈', '뮌', '뮐', '뮤', '뮨', '뮬', '뮴', '뮷', '므', '믄', '믈', '믐', '믓', '미', '믹', '민', '믿', '밀', '밂', '밈', '밉', '밋', '밌', '밍', '및', '밑', '바', '박', '밖', '밗', '반', '받', '발', '밝', '밞', '밟', '밤', '밥', '밧', '방', '밭', '배', '백', '밴', '밸', '뱀', '뱁', '뱃', '뱄', '뱅', '뱉', '뱌', '뱍', '뱐', '뱝', '버', '벅', '번', '벋', '벌', '벎', '범', '법', '벗', '벙', '벚', '베', '벡', '벤', '벧', '벨', '벰', '벱', '벳', '벴', '벵', '벼', '벽', '변', '별', '볍', '볏', '볐', '병', '볕', '볘', '볜', '보', '복', '볶', '본', '볼', '봄', '봅', '봇', '봉', '봐', '봔', '봤', '봬', '뵀', '뵈', '뵉', '뵌', '뵐', '뵘', '뵙', '뵤', '뵨', '부', '북', '분', '붇', '불', '붉', '붊', '붐', '붑', '붓', '붕', '붙', '붚', '붜', '붤', '붰', '붸', '뷔', '뷕', '뷘', '뷜', '뷩', '뷰', '뷴', '뷸', '븀', '븃', '븅', '브', '븍', '븐', '블', '븜', '븝', '븟', '비', '빅', '빈', '빌', '빎', '빔', '빕', '빗', '빙', '빚', '빛', '빠', '빡', '빤', '빨', '빪', '빰', '빱', '빳', '빴', '빵', '빻', '빼', '빽', '뺀', '뺄', '뺌', '뺍', '뺏', '뺐', '뺑', '뺘', '뺙', '뺨', '뻐', '뻑', '뻔', '뻗', '뻘', '뻠', '뻣', '뻤', '뻥', '뻬', '뼁', '뼈', '뼉', '뼘', '뼙', '뼛', '뼜', '뼝', '뽀', '뽁', '뽄', '뽈', '뽐', '뽑', '뽕', '뾔', '뾰', '뿅', '뿌', '뿍', '뿐', '뿔', '뿜', '뿟', '뿡', '쀼', '쁑', '쁘', '쁜', '쁠', '쁨', '쁩', '삐', '삑', '삔', '삘', '삠', '삡', '삣', '삥', '사', '삭', '삯', '산', '삳', '살', '삵', '삶', '삼', '삽', '삿', '샀', '상', '샅', '새', '색', '샌', '샐', '샘', '샙', '샛', '샜', '생', '샤', '샥', '샨', '샬', '샴', '샵', '샷', '샹', '섀', '섄', '섈', '섐', '섕', '서', '석', '섞', '섟', '선', '섣', '설', '섦', '섧', '섬', '섭', '섯', '섰', '성', '섶', '세', '섹', '센', '셀', '셈', '셉', '셋', '셌', '셍', '셔', '셕', '션', '셜', '셤', '셥', '셧', '셨', '셩', '셰', '셴', '셸', '솅', '소', '속', '솎', '손', '솔', '솖', '솜', '솝', '솟', '송', '솥', '솨', '솩', '솬', '솰', '솽', '쇄', '쇈', '쇌', '쇔', '쇗', '쇘', '쇠', '쇤', '쇨', '쇰', '쇱', '쇳', '쇼', '쇽', '숀', '숄', '숌', '숍', '숏', '숑', '수', '숙', '순', '숟', '술', '숨', '숩', '숫', '숭', '숯', '숱', '숲', '숴', '쉈', '쉐', '쉑', '쉔', '쉘', '쉠', '쉥', '쉬', '쉭', '쉰', '쉴', '쉼', '쉽', '쉿', '슁', '슈', '슉', '슐', '슘', '슛', '슝', '스', '슥', '슨', '슬', '슭', '슴', '습', '슷', '승', '시', '식', '신', '싣', '실', '싫', '심', '십', '싯', '싱', '싶', '싸', '싹', '싻', '싼', '쌀', '쌈', '쌉', '쌌', '쌍', '쌓', '쌔', '쌕', '쌘', '쌜', '쌤', '쌥', '쌨', '쌩', '썅', '써', '썩', '썬', '썰', '썲', '썸', '썹', '썼', '썽', '쎄', '쎈', '쎌', '쏀', '쏘', '쏙', '쏜', '쏟', '쏠', '쏢', '쏨', '쏩', '쏭', '쏴', '쏵', '쏸', '쐈', '쐐', '쐤', '쐬', '쐰', '쐴', '쐼', '쐽', '쑈', '쑤', '쑥', '쑨', '쑬', '쑴', '쑵', '쑹', '쒀', '쒔', '쒜', '쒸', '쒼', '쓩', '쓰', '쓱', '쓴', '쓸', '쓺', '쓿', '씀', '씁', '씌', '씐', '씔', '씜', '씨', '씩', '씬', '씰', '씸', '씹', '씻', '씽', '아', '악', '안', '앉', '않', '알', '앍', '앎', '앓', '암', '압', '앗', '았', '앙', '앝', '앞', '애', '액', '앤', '앨', '앰', '앱', '앳', '앴', '앵', '야', '약', '얀', '얄', '얇', '얌', '얍', '얏', '양', '얕', '얗', '얘', '얜', '얠', '얩', '어', '억', '언', '얹', '얻', '얼', '얽', '얾', '엄', '업', '없', '엇', '었', '엉', '엊', '엌', '엎', '에', '엑', '엔', '엘', '엠', '엡', '엣', '엥', '여', '역', '엮', '연', '열', '엶', '엷', '염', '엽', '엾', '엿', '였', '영', '옅', '옆', '옇', '예', '옌', '옐', '옘', '옙', '옛', '옜', '오', '옥', '온', '올', '옭', '옮', '옰', '옳', '옴', '옵', '옷', '옹', '옻', '와', '왁', '완', '왈', '왐', '왑', '왓', '왔', '왕', '왜', '왝', '왠', '왬', '왯', '왱', '외', '왹', '왼', '욀', '욈', '욉', '욋', '욍', '요', '욕', '욘', '욜', '욤', '욥', '욧', '용', '우', '욱', '운', '울', '욹', '욺', '움', '웁', '웃', '웅', '워', '웍', '원', '월', '웜', '웝', '웠', '웡', '웨', '웩', '웬', '웰', '웸', '웹', '웽', '위', '윅', '윈', '윌', '윔', '윕', '윗', '윙', '유', '육', '윤', '율', '윰', '윱', '윳', '융', '윷', '으', '윽', '은', '을', '읊', '음', '읍', '읏', '응', '읒', '읓', '읔', '읕', '읖', '읗', '의', '읜', '읠', '읨', '읫', '이', '익', '인', '일', '읽', '읾', '잃', '임', '입', '잇', '있', '잉', '잊', '잎', '자', '작', '잔', '잖', '잗', '잘', '잚', '잠', '잡', '잣', '잤', '장', '잦', '재', '잭', '잰', '잴', '잼', '잽', '잿', '쟀', '쟁', '쟈', '쟉', '쟌', '쟎', '쟐', '쟘', '쟝', '쟤', '쟨', '쟬', '저', '적', '전', '절', '젊', '점', '접', '젓', '정', '젖', '제', '젝', '젠', '젤', '젬', '젭', '젯', '젱', '져', '젼', '졀', '졈', '졉', '졌', '졍', '졔', '조', '족', '존', '졸', '졺', '좀', '좁', '좃', '종', '좆', '좇', '좋', '좌', '좍', '좔', '좝', '좟', '좡', '좨', '좼', '좽', '죄', '죈', '죌', '죔', '죕', '죗', '죙', '죠', '죡', '죤', '죵', '주', '죽', '준', '줄', '줅', '줆', '줌', '줍', '줏', '중', '줘', '줬', '줴', '쥐', '쥑', '쥔', '쥘', '쥠', '쥡', '쥣', '쥬', '쥰', '쥴', '쥼', '즈', '즉', '즌', '즐', '즘', '즙', '즛', '증', '지', '직', '진', '짇', '질', '짊', '짐', '집', '짓', '징', '짖', '짙', '짚', '짜', '짝', '짠', '짢', '짤', '짧', '짬', '짭', '짯', '짰', '짱', '째', '짹', '짼', '쨀', '쨈', '쨉', '쨋', '쨌', '쨍', '쨔', '쨘', '쨩', '쩌', '쩍', '쩐', '쩔', '쩜', '쩝', '쩟', '쩠', '쩡', '쩨', '쩽', '쪄', '쪘', '쪼', '쪽', '쫀', '쫄', '쫌', '쫍', '쫏', '쫑', '쫓', '쫘', '쫙', '쫠', '쫬', '쫴', '쬈', '쬐', '쬔', '쬘', '쬠', '쬡', '쭁', '쭈', '쭉', '쭌', '쭐', '쭘', '쭙', '쭝', '쭤', '쭸', '쭹', '쮜', '쮸', '쯔', '쯤', '쯧', '쯩', '찌', '찍', '찐', '찔', '찜', '찝', '찡', '찢', '찧', '차', '착', '찬', '찮', '찰', '참', '찹', '찻', '찼', '창', '찾', '채', '책', '챈', '챌', '챔', '챕', '챗', '챘', '챙', '챠', '챤', '챦', '챨', '챰', '챵', '처', '척', '천', '철', '첨', '첩', '첫', '첬', '청', '체', '첵', '첸', '첼', '쳄', '쳅', '쳇', '쳉', '쳐', '쳔', '쳤', '쳬', '쳰', '촁', '초', '촉', '촌', '촐', '촘', '촙', '촛', '총', '촤', '촨', '촬', '촹', '최', '쵠', '쵤', '쵬', '쵭', '쵯', '쵱', '쵸', '춈', '추', '축', '춘', '출', '춤', '춥', '춧', '충', '춰', '췄', '췌', '췐', '취', '췬', '췰', '췸', '췹', '췻', '췽', '츄', '츈', '츌', '츔', '츙', '츠', '측', '츤', '츨', '츰', '츱', '츳', '층', '치', '칙', '친', '칟', '칠', '칡', '침', '칩', '칫', '칭', '카', '칵', '칸', '칼', '캄', '캅', '캇', '캉', '캐', '캑', '캔', '캘', '캠', '캡', '캣', '캤', '캥', '캬', '캭', '컁', '커', '컥', '컨', '컫', '컬', '컴', '컵', '컷', '컸', '컹', '케', '켁', '켄', '켈', '켐', '켑', '켓', '켕', '켜', '켠', '켤', '켬', '켭', '켯', '켰', '켱', '켸', '코', '콕', '콘', '콜', '콤', '콥', '콧', '콩', '콰', '콱', '콴', '콸', '쾀', '쾅', '쾌', '쾡', '쾨', '쾰', '쿄', '쿠', '쿡', '쿤', '쿨', '쿰', '쿱', '쿳', '쿵', '쿼', '퀀', '퀄', '퀑', '퀘', '퀭', '퀴', '퀵', '퀸', '퀼', '큄', '큅', '큇', '큉', '큐', '큔', '큘', '큠', '크', '큭', '큰', '클', '큼', '큽', '킁', '키', '킥', '킨', '킬', '킴', '킵', '킷', '킹', '타', '탁', '탄', '탈', '탉', '탐', '탑', '탓', '탔', '탕', '태', '택', '탠', '탤', '탬', '탭', '탯', '탰', '탱', '탸', '턍', '터', '턱', '턴', '털', '턺', '텀', '텁', '텃', '텄', '텅', '테', '텍', '텐', '텔', '템', '텝', '텟', '텡', '텨', '텬', '텼', '톄', '톈', '토', '톡', '톤', '톨', '톰', '톱', '톳', '통', '톺', '톼', '퇀', '퇘', '퇴', '퇸', '툇', '툉', '툐', '투', '툭', '툰', '툴', '툼', '툽', '툿', '퉁', '퉈', '퉜', '퉤', '튀', '튁', '튄', '튈', '튐', '튑', '튕', '튜', '튠', '튤', '튬', '튱', '트', '특', '튼', '튿', '틀', '틂', '틈', '틉', '틋', '틔', '틘', '틜', '틤', '틥', '티', '틱', '틴', '틸', '팀', '팁', '팃', '팅', '파', '팍', '팎', '판', '팔', '팖', '팜', '팝', '팟', '팠', '팡', '팥', '패', '팩', '팬', '팰', '팸', '팹', '팻', '팼', '팽', '퍄', '퍅', '퍼', '퍽', '펀', '펄', '펌', '펍', '펏', '펐', '펑', '페', '펙', '펜', '펠', '펨', '펩', '펫', '펭', '펴', '편', '펼', '폄', '폅', '폈', '평', '폐', '폘', '폡', '폣', '포', '폭', '폰', '폴', '폼', '폽', '폿', '퐁', '퐈', '퐝', '푀', '푄', '표', '푠', '푤', '푭', '푯', '푸', '푹', '푼', '푿', '풀', '풂', '품', '풉', '풋', '풍', '풔', '풩', '퓌', '퓐', '퓔', '퓜', '퓟', '퓨', '퓬', '퓰', '퓸', '퓻', '퓽', '프', '픈', '플', '픔', '픕', '픗', '피', '픽', '핀', '필', '핌', '핍', '핏', '핑', '하', '학', '한', '할', '핥', '함', '합', '핫', '항', '해', '핵', '핸', '핼', '햄', '햅', '햇', '했', '행', '햐', '향', '허', '헉', '헌', '헐', '헒', '험', '헙', '헛', '헝', '헤', '헥', '헨', '헬', '헴', '헵', '헷', '헹', '혀', '혁', '현', '혈', '혐', '협', '혓', '혔', '형', '혜', '혠', '혤', '혭', '호', '혹', '혼', '홀', '홅', '홈', '홉', '홋', '홍', '홑', '화', '확', '환', '활', '홧', '황', '홰', '홱', '홴', '횃', '횅', '회', '획', '횐', '횔', '횝', '횟', '횡', '효', '횬', '횰', '횹', '횻', '후', '훅', '훈', '훌', '훑', '훔', '훗', '훙', '훠', '훤', '훨', '훰', '훵', '훼', '훽', '휀', '휄', '휑', '휘', '휙', '휜', '휠', '휨', '휩', '휫', '휭', '휴', '휵', '휸', '휼', '흄', '흇', '흉', '흐', '흑', '흔', '흖', '흗', '흘', '흙', '흠', '흡', '흣', '흥', '흩', '희', '흰', '흴', '흼', '흽', '힁', '히', '힉', '힌', '힐', '힘', '힙', '힛', '힝']
 ```
 </details>
 
 <details>
 <summary>28. get_all_incompleted_form_hangul_chars</summary>
 
-This returns all non-completed form Hangul characters.
+This returns all incompleted form Hangul characters.
 
 Returns:
-- `List[str]`: all non-completed form Hangul characters
+- `List[str]`: all incompleted form Hangul characters
 
 Examples:
 ```python
 >>> from kss import Kss
 >>> get_all_incompleted_form_hangul_chars = Kss("get_all_incompleted_form_hangul_chars")
 >>> output = get_all_incompleted_form_hangul_chars()
 >>> print(output)
@@ -1043,17 +1031,17 @@
 Returns:
 - `Union[str, List[str]]`: normalized text or list of normalized texts
 
 Examples:
 ```python
 >>> from kss import Kss
 >>> normalize = Kss("normalize")
->>> text = "안녕\u200b하세요 ﾻﾻﾻﾻﾻﾻ   <br>오늘\u200b은 날이 참 좋네요.\\n\\n\\n200 &lt; 300 &amp; 400"
+>>> text = "안녕\u200b하세요 ﾻﾻﾻﾻﾻﾻ   <br>오늘\u200b은 날이 참 좋네요.\n\n\n200 &lt; 300 &amp; 400"
 >>> normalize(text, allow_doubled_spaces=False, allow_html_tags=False, allow_html_escape=False, allow_halfwidth_hangul=False, allow_hangul_jamo=False, allow_invisible_chars=False, reduce_char_repeats_over=2, reduce_emoticon_repeats_over=2)
-'안녕하세요 ㅋㅋ 오늘은 날이 참 좋네요.\\n200 < 300 & 400'
+'안녕하세요 ㅋㅋ 오늘은 날이 참 좋네요.\n200 < 300 & 400'
 ```
 </details>
 
 <details>
 <summary>32. preprocess</summary>
 
 This preprocesses text with various options.
@@ -1270,15 +1258,16 @@
 ```
 References:
 - This was copied from [korean-romanizer](https://github.com/osori/korean-romanizer) and modified by Kss
 </details>
 
 <details>
 <summary>38. is_unsafe</summary>
-Check if the text is unsafe or not.
+
+This checks if the text is unsafe or not.
 
 Args:
 - text (`Union[str, List[str], Tuple[str]]`): single text or list of texts
 - return_matches (`bool`): whether to return matches or not
 - num_workers (`Union[int, str]`): the number of multiprocessing workers
 
 Returns:
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: kss Version: 6.0.0 Summary: A Toolkit for Korean
-sentence segmentation Home-page: https://github.com/hyunwoongko/kss Author:
-Hyunwoong Ko Author-email: kevin.brain@kakaobrain.com License: BSD 3-Clause
-"New" or "Revised" License Platform: any Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.2 Classifier:
-Programming Language :: Python :: 3.3 Classifier: Programming Language ::
-Python :: 3.4 Classifier: Programming Language :: Python :: 3.5 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Requires-
-Python: >=3 Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: kss Version: 6.0.0.dev0 Summary: A Toolkit for
+Korean sentence segmentation Home-page: https://github.com/hyunwoongko/kss
+Author: Hyunwoong Ko Author-email: kevin.brain@kakaobrain.com License: BSD 3-
+Clause "New" or "Revised" License Platform: any Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.2
+Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
+Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
+LICENSE
                ************ KKSSSS:: KKoorreeaann SSttrriinngg pprroocceessssiinngg SSuuiittee ************
   _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_I_s_s_u_e_s_]_[_T_e_s_t_s_ _o_n_ _U_b_u_n_t_u_]_[_T_e_s_t_s_ _o_n_ _M_a_c_O_S_]_[_T_e_s_t_s_ _o_n_ _W_i_n_d_o_w_s_]
 KSS is a Korean string processing suite that provides various functions for
 processing Korean strings. It is designed to be simple and easy to use, and it
 is designed to be used in various fields such as natural language processing,
 data preprocessing, and data analysis. ### What's New: - April 27, 2024
 [Released Kss 6.0 Python](https://github.com/hyunwoongko/kss/releases/tag/
@@ -62,15 +63,15 @@
 (text) ['íì¬ ëë£ ë¶ë¤ê³¼ ë¤ëìëë° ë¶ìê¸°ë ì¢ê³  ììë
 ë§ììì´ì', 'ë¤ë§, ê°ë¨ í ë¼ì ì´ ê°ë¨ ììë²ê±° ê³¨ëª©ê¸¸ë¡
 ì­ ì¬ë¼ê°ì¼ íëë° ë¤ë¤ ììë²ê±°ì ì í¹ì ëì´ê° ë»
 íëµëë¤', 'ê°ë¨ì­ ë§ì§ í ë¼ì ì ì¸ë¶ ëª¨ìµ.'] ``` ### 4.
 Multiprocessing If you input a list of strings, Kss will automatically use
 multiprocessing to process the strings in parallel. And you can set the number
 of processes to use by setting the `num_workers` parameter. If you input
-`num_workers<2`, Kss will not use multiprocessing. ```python from kss import
+`num_workers < 2`, Kss will not use multiprocessing. ```python from kss import
 Kss module = Kss("MODULE_NAME") # using all cores output = module(
 ["YOUR_INPUT_STRING1", "YOUR_INPUT_STRING2", ...], **kwargs) # using 4 cores
 output = module(["YOUR_INPUT_STRING1", "YOUR_INPUT_STRING2", ...],
 num_workers=4, **kwargs) # using 1 core (no multiprocessing) output = module(
 ["YOUR_INPUT_STRING1", "YOUR_INPUT_STRING2", ...], num_workers=1, **kwargs) ```
 ### 5. Backward Compatibility The old version of Kss used functional usage. KSS
 also supports this for backward compatibility. ```python from kss import
@@ -655,27 +656,27 @@
 'ê³±ëì'), ('ë', 'ê³±ë'), ('ì°', 'ê³±ì°'), ('ì¼ë', 'ê³ ì°ë'),
 ('ì¼ëê³ ', 'ê³ ì°ëê³ '), ('ì¼ë¨', 'ê³ ì°ë¨'), ('ì¼ë',
 'ê³ ì°ë'), ('ì¼ëë¼', 'ê³ ì°ëë¼'), ('ì¼ì´', 'ê³ ì°ì´'),
 ('ìê°', 'ê³ ì´ê°'), ('ìê°', 'ê³ ì´ê°'), ('ìê³ ', 'ê³ ì´ê³ '),
 ('ìë°', 'ê³ ì´ë°'), ('ìëì¼', 'ê³ ì´ëì¼'), ('ìì§',
 'ê³ ì´ì§'), ('ìë°ë¼ë', 'ê³ ì¸ë°ë¼ë'), ('ììê³ ',
 'ê³ ì¸ìê³ ')]} ``` References: - This was copied from [KoParadigm](https://
-github.com/Kyubyong/KoParadigm) and modified by Kss 24. anonymize Anonymize
-sensitive information in the given text. Args: - text (`Union[str, List[str],
-Tuple[str]`): single text or list of texts - phone_number_anonymization
-(`bool`): whether to anonymize phone numbers or not - rrn_anonymization
-(`bool`): whether to anonymize resident registration numbers or not -
-card_anonymization (`bool`): whether to anonymize card numbers or not -
-email_anonymization (`bool`): whether to anonymize email addresses or not -
-back_account_anonymization (`bool`): whether to anonymize bank account numbers
-or not - credit_card_anonymization (`bool`): whether to anonymize credit card
-numbers or not - zip_anonymization (`bool`): whether to anonymize zip codes or
-not - bitcoin_anonymization (`bool`): whether to anonymize bitcoin addresses or
-not - url_anonymization (`bool`): whether to anonymize URLs or not -
-ip_v6_anonymization (`bool`): whether to anonymize IPv6 addresses or not -
+github.com/Kyubyong/KoParadigm) and modified by Kss 24. anonymize This
+anonymizes sensitive information in the given text. Args: - text (`Union[str,
+List[str], Tuple[str]`): single text or list of texts -
+phone_number_anonymization (`bool`): whether to anonymize phone numbers or not
+- rrn_anonymization (`bool`): whether to anonymize resident registration
+numbers or not - card_anonymization (`bool`): whether to anonymize card numbers
+or not - email_anonymization (`bool`): whether to anonymize email addresses or
+not - back_account_anonymization (`bool`): whether to anonymize bank account
+numbers or not - credit_card_anonymization (`bool`): whether to anonymize
+credit card numbers or not - zip_anonymization (`bool`): whether to anonymize
+zip codes or not - bitcoin_anonymization (`bool`): whether to anonymize bitcoin
+addresses or not - url_anonymization (`bool`): whether to anonymize URLs or not
+- ip_v6_anonymization (`bool`): whether to anonymize IPv6 addresses or not -
 ip_v4_anonymization (`bool`): whether to anonymize IPv4 addresses or not -
 phone_number_replacement (`str`): the replacement string for phone numbers,
 default is "" - rrn_replacement (`str`): the replacement string for resident
 registration numbers, default is "" - card_replacement (`str`): the replacement
 string for card numbers, default is "" - email_replacement (`str`): the
 replacement string for email addresses, default is "" -
 back_account_replacement (`str`): the replacement string for bank account
@@ -688,24 +689,24 @@
 ip_v4_replacement (`str`): the replacement string for IPv4 addresses, default
 is "" - num_workers (`Union[int, str]`): the number of multiprocessing workers
 Returns: - `Union[str, List[str], Tuple[str]]`: anonymized text or list of
 anonymized texts Examples: ```python >>> from kss import Kss >>> anonymize =
 Kss("anonymize") >>> text = "ì  ì íë²í¸ë 010-1234-5678, ì´ë©ì¼
 ì£¼ìë kevin.brain@kakaobrain.comìëë¤." >>> output = anonymize(text)
 >>> print(output) "ì  ì íë²í¸ë , ì´ë©ì¼ ì£¼ìë ìëë¤." ```
-25. clean_news Clean news articles by removing useless headers and footers.
-Args: - text (`Union[str, List[str], Tuple[str]]`): Input text or list of
-texts. - min_sentences (`int`): Minimum number of sentences to keep. Defaults
-to 3. - header_ratio (`float`): Ratio of the number of sentences to check in
-the header. Defaults to 0.4. - footer_ratio (`float`): Ratio of the number of
-sentences to check in the footer. Defaults to 0.4. - num_workers (`Union[int,
-str]`): the number of multiprocessing workers - verbose (`bool`): whether to
-print verbose outputs or not Returns: - `Union[str, List[str]]`: Cleaned text
-or list of cleaned texts. Examples: ```python >>> from kss import Kss >>>
-clean_news = Kss("clean_news") >>> text = "[ì¬ì§]ìë²ëë, ë´ê½
+25. clean_news This cleans news articles by removing useless headers and
+footers. Args: - text (`Union[str, List[str], Tuple[str]]`): Input text or list
+of texts. - min_sentences (`int`): Minimum number of sentences to keep.
+Defaults to 3. - header_ratio (`float`): Ratio of the number of sentences to
+check in the header. Defaults to 0.4. - footer_ratio (`float`): Ratio of the
+number of sentences to check in the footer. Defaults to 0.4. - num_workers
+(`Union[int, str]`): the number of multiprocessing workers - verbose (`bool`):
+whether to print verbose outputs or not Returns: - `Union[str, List[str]]`:
+Cleaned text or list of cleaned texts. Examples: ```python >>> from kss import
+Kss >>> clean_news = Kss("clean_news") >>> text = "[ì¬ì§]ìë²ëë, ë´ê½
 í¼ì³ì§ 'í¤ë¦½ì¶ì ' ì¤í\n\n[ ë´ì¤1 ì ê³µ](ìì¸=ë´ì¤1) ì´ëì
 ê¸°ì = ìë²ëëê° ì¤ë 22ì¼ë¶í° ë´ì ìì§íë í¤ë¦½ 120ë§
 ì¡ì´ì í¨ê» 'í¤ë¦½ì¶ì 'ë¥¼ ì¤íí´ ë³¸ê²©ì ì¸ ë´ì ììì
 ìë¦°ë¤. ì§ë 1992ë êµ­ë´ ì²« í¤ë¦½ ì¶ì ë¥¼ ì° ì´í ì¬í´ë¡
 22íì§¸ë¥¼ ë§ì´í ìë²ëë 'í¤ë¦½ì¶ì 'ë ì§ëí´ ì²« ì ì
 ë³´ì´ë©° ì¢ì ë°ìì ì»ìë ì¤ê°(äºæ)ì²´í 'ìí¬ë¦¿ê°ë 'ì
 ë¦¬ë´ì¼íê³ , ì ê· íë§ ê½ê¸¸ì ì¡°ì±íë ë± ë´ê½ì íì©í
@@ -741,826 +742,237 @@
 completed form. Args: - text (`Union[str, List[str], Tuple[str]`): single text
 or list of texts - num_workers (`Union[int, str]`): the number of
 multiprocessing workers Returns: - `Union[bool, List[bool]]`: whether the given
 text is in completed form or not Examples: ```python >>> from kss import Kss
 >>> is_completed_form = Kss("is_completed_form") >>> text = "ë°±" >>> output =
 is_completed_form(text) >>> print(output) True >>> text = "ë´¯" >>> output =
 is_completed_form(text) >>> print(output) False ``` 27.
-get_all_completed_form_hangul_chars This returns all non-completed form Hangul
-characters. Returns: - `List[str]`: all non-completed form Hangul characters
+get_all_completed_form_hangul_chars This returns all completed form Hangul
+characters. Returns: - `List[str]`: all completed form Hangul characters
 Examples: ```python >>> from kss import Kss >>>
-get_all_incompleted_form_hangul_chars = Kss
-("get_all_incompleted_form_hangul_chars") >>> output =
-get_all_incompleted_form_hangul_chars() >>> print(output) ['ê°', 'ê°', 'ê°',
-'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°¡', 'ê°¢',
-'ê°£', 'ê°¥', 'ê°¦', 'ê°§', 'ê°¨', 'ê°©', 'ê°ª', 'ê°«', 'ê°®', 'ê°²', 'ê°³',
-'ê°´', 'ê°µ', 'ê°¶', 'ê°·', 'ê°º', 'ê°»', 'ê°½', 'ê°¾', 'ê°¿', 'ê±', 'ê±',
-'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
-'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
-'ê±', 'ê±', 'ê± ', 'ê±¡', 'ê±¢', 'ê±£', 'ê±¤', 'ê±¥', 'ê±¦', 'ê±§', 'ê±¨',
-'ê±©', 'ê±ª', 'ê±«', 'ê±¬', 'ê±­', 'ê±®', 'ê±¯', 'ê±²', 'ê±³', 'ê±µ', 'ê±¶',
-'ê±¹', 'ê±»', 'ê±¼', 'ê±½', 'ê±¾', 'ê±¿', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²',
-'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²',
-'ê²', 'ê²¢', 'ê²£', 'ê²¤', 'ê²¥', 'ê²¦', 'ê²§', 'ê²«', 'ê²­', 'ê²®', 'ê²±',
-'ê²²', 'ê²³', 'ê²´', 'ê²µ', 'ê²¶', 'ê²·', 'ê²º', 'ê²¾', 'ê²¿', 'ê³', 'ê³',
-'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³',
-'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³',
-'ê³', 'ê³', 'ê³¢', 'ê³£', 'ê³¥', 'ê³¦', 'ê³©', 'ê³«', 'ê³­', 'ê³®', 'ê³²',
-'ê³´', 'ê³·', 'ê³¸', 'ê³¹', 'ê³º', 'ê³»', 'ê³¾', 'ê³¿', 'ê´', 'ê´', 'ê´',
-'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´',
-'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´¡', 'ê´¢',
-'ê´£', 'ê´¤', 'ê´¥', 'ê´¦', 'ê´§', 'ê´¨', 'ê´ª', 'ê´«', 'ê´®', 'ê´¯', 'ê´°',
-'ê´±', 'ê´²', 'ê´³', 'ê´¶', 'ê´·', 'ê´¹', 'ê´º', 'ê´»', 'ê´½', 'ê´¾', 'ê´¿',
-'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ',
-'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ',
-'êµ', 'êµ', 'êµ', 'êµ ', 'êµ¢', 'êµ¤', 'êµ¥', 'êµ¦', 'êµ§', 'êµ¨', 'êµ©',
-'êµª', 'êµ«', 'êµ®', 'êµ¯', 'êµ±', 'êµ²', 'êµ·', 'êµ¸', 'êµ¹', 'êµº', 'êµ¾',
-'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶',
-'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶',
-'ê¶', 'ê¶', 'ê¶ ', 'ê¶¡', 'ê¶¢', 'ê¶£', 'ê¶¥', 'ê¶¦', 'ê¶§', 'ê¶¨', 'ê¶©',
-'ê¶ª', 'ê¶«', 'ê¶¬', 'ê¶­', 'ê¶®', 'ê¶¯', 'ê¶°', 'ê¶±', 'ê¶²', 'ê¶³', 'ê¶´',
-'ê¶µ', 'ê¶¶', 'ê¶¸', 'ê¶¹', 'ê¶º', 'ê¶»', 'ê¶¼', 'ê¶½', 'ê¶¾', 'ê¶¿', 'ê·',
-'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·',
-'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·',
-'ê·', 'ê·¡', 'ê·¢', 'ê·£', 'ê·¥', 'ê·¦', 'ê·§', 'ê·¨', 'ê·©', 'ê·ª', 'ê·«',
-'ê·¬', 'ê·­', 'ê·®', 'ê·¯', 'ê·°', 'ê·±', 'ê·²', 'ê·³', 'ê·´', 'ê·µ', 'ê·¶',
-'ê··', 'ê·º', 'ê·»', 'ê·½', 'ê·¾', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸',
-'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸',
-'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸ ', 'ê¸¡', 'ê¸¢',
-'ê¸£', 'ê¸¤', 'ê¸¥', 'ê¸¦', 'ê¸§', 'ê¸¨', 'ê¸©', 'ê¸ª', 'ê¸«', 'ê¸¬', 'ê¸­',
-'ê¸®', 'ê¸¯', 'ê¸²', 'ê¸³', 'ê¸µ', 'ê¸¶', 'ê¸¹', 'ê¸»', 'ê¸¼', 'ê¸½', 'ê¸¾',
-'ê¸¿', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹',
-'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹¢', 'ê¹£', 'ê¹¤', 'ê¹¦',
-'ê¹§', 'ê¹ª', 'ê¹«', 'ê¹­', 'ê¹®', 'ê¹¯', 'ê¹±', 'ê¹²', 'ê¹³', 'ê¹´', 'ê¹µ',
-'ê¹¶', 'ê¹·', 'ê¹º', 'ê¹¾', 'ê¹¿', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº',
-'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº',
-'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº', 'êº',
-'êº', 'êº ', 'êº¡', 'êº¢', 'êº£', 'êº¤', 'êº¥', 'êº¦', 'êº§', 'êº¨', 'êº©',
-'êºª', 'êº«', 'êº¬', 'êº­', 'êº®', 'êº¯', 'êº°', 'êº±', 'êº²', 'êº³', 'êº´',
-'êºµ', 'êº¶', 'êº·', 'êº¸', 'êº¹', 'êºº', 'êº»', 'êº¿', 'ê»', 'ê»', 'ê»',
-'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»',
-'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê» ', 'ê»¡', 'ê»¢',
-'ê»£', 'ê»¤', 'ê»¥', 'ê»¦', 'ê»§', 'ê»©', 'ê»ª', 'ê»¬', 'ê»®', 'ê»¯', 'ê»°',
-'ê»±', 'ê»²', 'ê»³', 'ê»µ', 'ê»¶', 'ê»·', 'ê»¹', 'ê»º', 'ê»»', 'ê»½', 'ê»¾',
-'ê»¿', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼',
-'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼',
-'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼ ', 'ê¼¡', 'ê¼¢', 'ê¼£',
-'ê¼¤', 'ê¼¥', 'ê¼¦', 'ê¼§', 'ê¼¨', 'ê¼©', 'ê¼ª', 'ê¼«', 'ê¼®', 'ê¼¯', 'ê¼±',
-'ê¼³', 'ê¼µ', 'ê¼¶', 'ê¼·', 'ê¼¸', 'ê¼¹', 'ê¼º', 'ê¼»', 'ê¼¾', 'ê½', 'ê½',
-'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½',
-'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½',
-'ê½ ', 'ê½¡', 'ê½¢', 'ê½£', 'ê½¦', 'ê½§', 'ê½¨', 'ê½©', 'ê½ª', 'ê½«', 'ê½¬',
-'ê½­', 'ê½®', 'ê½¯', 'ê½°', 'ê½±', 'ê½²', 'ê½³', 'ê½´', 'ê½µ', 'ê½¶', 'ê½·',
-'ê½¸', 'ê½º', 'ê½»', 'ê½¼', 'ê½½', 'ê½¾', 'ê½¿', 'ê¾', 'ê¾', 'ê¾', 'ê¾',
-'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾',
-'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾ ',
-'ê¾¡', 'ê¾¢', 'ê¾£', 'ê¾¤', 'ê¾¥', 'ê¾¦', 'ê¾§', 'ê¾¨', 'ê¾©', 'ê¾ª', 'ê¾«',
-'ê¾¬', 'ê¾­', 'ê¾®', 'ê¾¯', 'ê¾°', 'ê¾±', 'ê¾²', 'ê¾³', 'ê¾´', 'ê¾µ', 'ê¾¶',
-'ê¾·', 'ê¾º', 'ê¾»', 'ê¾½', 'ê¾¾', 'ê¾¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿',
-'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿',
-'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿ ', 'ê¿¡', 'ê¿¢', 'ê¿£',
-'ê¿¤', 'ê¿¥', 'ê¿¦', 'ê¿§', 'ê¿ª', 'ê¿«', 'ê¿¬', 'ê¿­', 'ê¿®', 'ê¿¯', 'ê¿²',
-'ê¿³', 'ê¿µ', 'ê¿¶', 'ê¿·', 'ê¿¹', 'ê¿º', 'ê¿»', 'ê¿¼', 'ê¿½', 'ê¿¾', 'ê¿¿',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë©',
-'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´',
-'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡',
-'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬',
-'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·',
-'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª',
-'ë°', 'ë²', 'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬',
-'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·',
-'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë¦', 'ë§',
-'ë©', 'ëª', 'ë«', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë¶',
-'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥',
-'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°',
-'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ëº', 'ë»', 'ë½', 'ë¾',
-'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ëª', 'ë«',
-'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶',
-'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª',
-'ë«', 'ë­', 'ë®', 'ë¯', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·',
-'ë¸', 'ëº', 'ë¼', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥',
-'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°',
-'ë±', 'ë²', 'ë³', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë½',
-'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë¡',
-'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®',
-'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»',
-'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë¢', 'ë¤', 'ë§', 'ë¨', 'ë©', 'ë«', 'ë­',
-'ë®', 'ë¯', 'ë±', 'ë²', 'ë³', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº',
-'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë£', 'ë§', 'ë©',
-'ëª', 'ë°', 'ë±', 'ë²', 'ë¶', 'ë¼', 'ë½', 'ë¾', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢',
-'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­',
-'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸',
-'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡',
-'ë¢', 'ë£', 'ë¦', 'ë¨', 'ëª', 'ë¬', 'ë­', 'ë¯', 'ë²', 'ë³', 'ëµ',
-'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ëª', 'ë«', 'ë­', 'ë®',
-'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹',
-'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ëª',
-'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ',
-'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦',
-'ë§', 'ëª', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ëµ',
-'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë¢', 'ë¤', 'ë¦', 'ë§', 'ë¨', 'ë©',
-'ëª', 'ë«', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ',
-'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¥',
-'ë¦', 'ë§', 'ë©', 'ëª', 'ë«', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²',
-'ë³', 'ë´', 'ë¶', 'ë¸', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë¡', 'ë¢', 'ë¥', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë®',
-'ë°', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼',
-'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢',
-'ë£', 'ë¦', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë²', 'ë³', 'ëµ', 'ë¶',
-'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§',
-'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²',
-'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½',
-'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë¢', 'ë£', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ë¬', 'ë­', 'ë®', 'ë¯',
-'ë²', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë¾', 'ë¿', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ',
-'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«',
-'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·',
-'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¦', 'ë§', 'ë¨',
-'ë©', 'ëª', 'ë«', 'ë­', 'ë®', 'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ëµ',
-'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢',
-'ë£', 'ë¥', 'ë¦', 'ë§', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯',
-'ë°', 'ë±', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹', 'ëº',
-'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª',
-'ë­', 'ë®', 'ë¯', 'ë°', 'ë²', 'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ë¸',
-'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥',
-'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë±',
-'ë²', 'ë³', 'ëµ', 'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼', 'ë½', 'ë¾',
-'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢',
-'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª', 'ë«', 'ë­', 'ë®', 'ë±', 'ë²',
-'ë³', 'ë´', 'ëµ', 'ë¶', 'ë·', 'ëº', 'ë¼', 'ë½', 'ë¾', 'ë¿', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¥', 'ë¦', 'ë§', 'ë©',
-'ëª', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë²', 'ë´', 'ë¶', 'ë·', 'ë¸',
-'ë¹', 'ëº', 'ë»', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ëª', 'ë®',
-'ë¯', 'ë°', 'ë±', 'ë²', 'ë³', 'ë¶', 'ë·', 'ë¹', 'ëº', 'ë»', 'ë¼',
-'ë½', 'ë¾', 'ë¿', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
-'ë ', 'ë¡', 'ë¢', 'ë£', 'ë¤', 'ë¥', 'ë¦', 'ë§', 'ë¨', 'ë©', 'ëª',
-'ë«', 'ë®', 'ë¯', 'ë±', 'ë²', 'ë³', 'ëµ', 'ë¶', 'ë·', 'ë¸', 'ë¹',
-'ëº', 'ë»', 'ë¾', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ',
-'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ',
-'ë ', 'ë ', 'ë  ', 'ë ¡', 'ë ¢', 'ë £', 'ë ¦', 'ë §', 'ë ©', 'ë ª', 'ë «',
-'ë ­', 'ë ®', 'ë ¯', 'ë °', 'ë ±', 'ë ²', 'ë ³', 'ë ¶', 'ë º', 'ë »', 'ë ¼',
-'ë ½', 'ë ¾', 'ë ¿', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡',
-'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡',
-'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡¡', 'ë¡¢', 'ë¡£', 'ë¡¥',
-'ë¡¦', 'ë¡§', 'ë¡¨', 'ë¡©', 'ë¡ª', 'ë¡«', 'ë¡®', 'ë¡°', 'ë¡²', 'ë¡³', 'ë¡´',
-'ë¡µ', 'ë¡¶', 'ë¡·', 'ë¡¹', 'ë¡º', 'ë¡»', 'ë¡½', 'ë¡¾', 'ë¡¿', 'ë¢', 'ë¢',
-'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢',
-'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢',
-'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢', 'ë¢ ', 'ë¢¡', 'ë¢¢', 'ë¢£',
-'ë¢¤', 'ë¢¥', 'ë¢¦', 'ë¢§', 'ë¢©', 'ë¢ª', 'ë¢«', 'ë¢¬', 'ë¢­', 'ë¢®', 'ë¢¯',
-'ë¢±', 'ë¢²', 'ë¢³', 'ë¢µ', 'ë¢¶', 'ë¢·', 'ë¢¹', 'ë¢º', 'ë¢»', 'ë¢¼', 'ë¢½',
-'ë¢¾', 'ë¢¿', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£',
-'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£',
-'ë£', 'ë£', 'ë£', 'ë£ ', 'ë£¢', 'ë££', 'ë£¤', 'ë£¥', 'ë£¦', 'ë£§', 'ë£ª',
-'ë£«', 'ë£­', 'ë£®', 'ë£¯', 'ë£±', 'ë£²', 'ë£³', 'ë£´', 'ë£µ', 'ë£¶', 'ë£·',
-'ë£º', 'ë£¼', 'ë£¾', 'ë£¿', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤',
-'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤',
-'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤', 'ë¤',
-'ë¤', 'ë¤¡', 'ë¤¢', 'ë¤£', 'ë¤¤', 'ë¤¥', 'ë¤¦', 'ë¤§', 'ë¤¨', 'ë¤©', 'ë¤ª',
-'ë¤«', 'ë¤¬', 'ë¤­', 'ë¤®', 'ë¤¯', 'ë¤°', 'ë¤±', 'ë¤²', 'ë¤³', 'ë¤´', 'ë¤µ',
-'ë¤¶', 'ë¤·', 'ë¤¸', 'ë¤¹', 'ë¤º', 'ë¤»', 'ë¤¾', 'ë¤¿', 'ë¥', 'ë¥', 'ë¥',
-'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥',
-'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥¡',
-'ë¥¢', 'ë¥£', 'ë¥¤', 'ë¥¥', 'ë¥¦', 'ë¥§', 'ë¥ª', 'ë¥¬', 'ë¥®', 'ë¥¯', 'ë¥°',
-'ë¥±', 'ë¥²', 'ë¥³', 'ë¥¶', 'ë¥·', 'ë¥¹', 'ë¥º', 'ë¥»', 'ë¥½', 'ë¥¾', 'ë¥¿',
-'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦',
-'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦', 'ë¦',
-'ë¦', 'ë¦', 'ë¦', 'ë¦ ', 'ë¦¡', 'ë¦¢', 'ë¦£', 'ë¦¤', 'ë¦¥', 'ë¦¦', 'ë¦§',
-'ë¦¨', 'ë¦©', 'ë¦ª', 'ë¦«', 'ë¦®', 'ë¦¯', 'ë¦±', 'ë¦²', 'ë¦³', 'ë¦µ', 'ë¦¶',
-'ë¦·', 'ë¦¸', 'ë¦¹', 'ë¦º', 'ë¦»', 'ë¦¾', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§',
-'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§',
-'ë§', 'ë§', 'ë§ ', 'ë§¢', 'ë§¦', 'ë§§', 'ë§©', 'ë§ª', 'ë§«', 'ë§­', 'ë§®',
-'ë§¯', 'ë§°', 'ë§±', 'ë§²', 'ë§³', 'ë§¶', 'ë§»', 'ë§¼', 'ë§½', 'ë§¾', 'ë§¿',
-'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨',
-'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨',
-'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨ ', 'ë¨¡', 'ë¨¢', 'ë¨£', 'ë¨¤',
-'ë¨¥', 'ë¨¦', 'ë¨§', 'ë¨¨', 'ë¨©', 'ë¨ª', 'ë¨«', 'ë¨¬', 'ë¨­', 'ë¨®', 'ë¨¯',
-'ë¨°', 'ë¨±', 'ë¨²', 'ë¨³', 'ë¨´', 'ë¨µ', 'ë¨¶', 'ë¨·', 'ë¨º', 'ë¨»', 'ë¨½',
-'ë¨¾', 'ë¨¿', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©',
-'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©',
-'ë© ', 'ë©¡', 'ë©¢', 'ë©£', 'ë©¦', 'ë©ª', 'ë©«', 'ë©¬', 'ë©­', 'ë©®', 'ë©¯',
-'ë©²', 'ë©³', 'ë©µ', 'ë©¶', 'ë©·', 'ë©¹', 'ë©º', 'ë©»', 'ë©¼', 'ë©½', 'ë©¾',
-'ë©¿', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª',
-'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª',
-'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª', 'ëª ', 'ëª¡', 'ëª¢', 'ëª£', 'ëª¤',
-'ëª¥', 'ëª¦', 'ëª§', 'ëªª', 'ëª­', 'ëª®', 'ëª¯', 'ëª±', 'ëª³', 'ëª´', 'ëªµ',
-'ëª¶', 'ëª·', 'ëªº', 'ëª¼', 'ëª¾', 'ëª¿', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«',
-'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«',
-'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«',
-'ë«', 'ë« ', 'ë«¡', 'ë«¢', 'ë«£', 'ë«¤', 'ë«¥', 'ë«¦', 'ë«§', 'ë«¨', 'ë«©',
-'ë«ª', 'ë««', 'ë«¬', 'ë«­', 'ë«®', 'ë«¯', 'ë«°', 'ë«±', 'ë«²', 'ë«³', 'ë«´',
-'ë«µ', 'ë«¶', 'ë«·', 'ë«¸', 'ë«¹', 'ë«º', 'ë«»', 'ë«½', 'ë«¾', 'ë«¿', 'ë¬',
-'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬',
-'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬', 'ë¬',
-'ë¬', 'ë¬', 'ë¬¡', 'ë¬¢', 'ë¬£', 'ë¬¤', 'ë¬¥', 'ë¬¦', 'ë¬§', 'ë¬¨', 'ë¬ª',
-'ë¬¬', 'ë¬­', 'ë¬®', 'ë¬¯', 'ë¬°', 'ë¬±', 'ë¬²', 'ë¬³', 'ë¬·', 'ë¬¹', 'ë¬º',
-'ë¬¿', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­',
-'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­',
-'ë­', 'ë­', 'ë­ ', 'ë­¢', 'ë­¤', 'ë­¥', 'ë­¦', 'ë­§', 'ë­¨', 'ë­©', 'ë­ª',
-'ë­«', 'ë­­', 'ë­®', 'ë­¯', 'ë­°', 'ë­±', 'ë­²', 'ë­³', 'ë­´', 'ë­µ', 'ë­¶',
-'ë­·', 'ë­¸', 'ë­¹', 'ë­º', 'ë­»', 'ë­¼', 'ë­½', 'ë­¾', 'ë­¿', 'ë®', 'ë®',
-'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®',
-'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë®',
-'ë®', 'ë®', 'ë®', 'ë®', 'ë®', 'ë® ', 'ë®¡', 'ë®¢', 'ë®£', 'ë®¥', 'ë®¦',
-'ë®§', 'ë®©', 'ë®ª', 'ë®«', 'ë®­', 'ë®®', 'ë®¯', 'ë®°', 'ë®±', 'ë®²', 'ë®³',
-'ë®µ', 'ë®¶', 'ë®¸', 'ë®¹', 'ë®º', 'ë®»', 'ë®¼', 'ë®½', 'ë®¾', 'ë®¿', 'ë¯',
-'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯',
-'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯',
-'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯ ', 'ë¯¡', 'ë¯¢', 'ë¯£', 'ë¯¤', 'ë¯¥', 'ë¯¦',
-'ë¯§', 'ë¯¨', 'ë¯©', 'ë¯ª', 'ë¯«', 'ë¯¬', 'ë¯­', 'ë¯®', 'ë¯¯', 'ë¯°', 'ë¯±',
-'ë¯²', 'ë¯³', 'ë¯´', 'ë¯µ', 'ë¯¶', 'ë¯·', 'ë¯º', 'ë¯»', 'ë¯½', 'ë¯¾', 'ë°',
-'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°',
-'ë°', 'ë° ', 'ë°¡', 'ë°¢', 'ë°£', 'ë°¦', 'ë°¨', 'ë°ª', 'ë°«', 'ë°¬', 'ë°®',
-'ë°¯', 'ë°²', 'ë°³', 'ë°µ', 'ë°¶', 'ë°·', 'ë°¹', 'ë°º', 'ë°»', 'ë°¼', 'ë°½',
-'ë°¾', 'ë°¿', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±',
-'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±',
-'ë±', 'ë±', 'ë± ', 'ë±¡', 'ë±¢', 'ë±£', 'ë±¤', 'ë±¥', 'ë±¦', 'ë±§', 'ë±¨',
-'ë±©', 'ë±ª', 'ë±«', 'ë±¬', 'ë±­', 'ë±®', 'ë±¯', 'ë±°', 'ë±±', 'ë±²', 'ë±³',
-'ë±´', 'ë±µ', 'ë±¶', 'ë±·', 'ë±¸', 'ë±¹', 'ë±º', 'ë±»', 'ë±¼', 'ë±½', 'ë±¾',
-'ë±¿', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²',
-'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²',
-'ë²¢', 'ë²£', 'ë²¥', 'ë²¦', 'ë²©', 'ë²ª', 'ë²«', 'ë²¬', 'ë²­', 'ë²®', 'ë²¯',
-'ë²²', 'ë²¶', 'ë²·', 'ë²¸', 'ë²¹', 'ë²º', 'ë²»', 'ë²¾', 'ë²¿', 'ë³', 'ë³',
-'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³',
-'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³ ',
-'ë³¡', 'ë³¢', 'ë³£', 'ë³¤', 'ë³¥', 'ë³¦', 'ë³§', 'ë³¨', 'ë³©', 'ë³ª', 'ë³«',
-'ë³¬', 'ë³­', 'ë³®', 'ë³¯', 'ë³°', 'ë³±', 'ë³²', 'ë³³', 'ë³·', 'ë³¹', 'ë³º',
-'ë³»', 'ë³½', 'ë³¾', 'ë³¿', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´',
-'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´',
-'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´', 'ë´ ', 'ë´¡', 'ë´¢',
-'ë´£', 'ë´¥', 'ë´¦', 'ë´§', 'ë´¨', 'ë´©', 'ë´ª', 'ë´«', 'ë´­', 'ë´®', 'ë´¯',
-'ë´°', 'ë´±', 'ë´²', 'ë´³', 'ë´´', 'ë´µ', 'ë´¶', 'ë´·', 'ë´¸', 'ë´¹', 'ë´º',
-'ë´»', 'ë´¼', 'ë´½', 'ë´¾', 'ë´¿', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ',
-'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ',
-'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ ', 'ëµ¡', 'ëµ¢',
-'ëµ£', 'ëµ¥', 'ëµ¦', 'ëµ§', 'ëµ©', 'ëµª', 'ëµ«', 'ëµ¬', 'ëµ­', 'ëµ®', 'ëµ¯',
-'ëµ°', 'ëµ±', 'ëµ²', 'ëµ³', 'ëµ´', 'ëµµ', 'ëµ¶', 'ëµ·', 'ëµ¸', 'ëµ¹', 'ëµº',
-'ëµ»', 'ëµ¼', 'ëµ½', 'ëµ¾', 'ëµ¿', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶',
-'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶',
-'ë¶', 'ë¶ ', 'ë¶¡', 'ë¶¢', 'ë¶£', 'ë¶¥', 'ë¶¦', 'ë¶§', 'ë¶¨', 'ë¶©', 'ë¶ª',
-'ë¶«', 'ë¶¬', 'ë¶­', 'ë¶®', 'ë¶¯', 'ë¶±', 'ë¶²', 'ë¶³', 'ë¶´', 'ë¶µ', 'ë¶¶',
-'ë¶·', 'ë¶¹', 'ë¶º', 'ë¶»', 'ë¶¼', 'ë¶½', 'ë¶¾', 'ë¶¿', 'ë·', 'ë·', 'ë·',
-'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·',
-'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·', 'ë·',
-'ë·', 'ë·', 'ë·', 'ë· ', 'ë·¡', 'ë·¢', 'ë·£', 'ë·¤', 'ë·¥', 'ë·¦', 'ë·§',
-'ë·¨', 'ë·ª', 'ë·«', 'ë·¬', 'ë·­', 'ë·®', 'ë·¯', 'ë·±', 'ë·²', 'ë·³', 'ë·µ',
-'ë·¶', 'ë··', 'ë·¹', 'ë·º', 'ë·»', 'ë·¼', 'ë·½', 'ë·¾', 'ë·¿', 'ë¸', 'ë¸',
-'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸',
-'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸ ', 'ë¸¡',
-'ë¸¢', 'ë¸£', 'ë¸¤', 'ë¸¥', 'ë¸¦', 'ë¸§', 'ë¸¨', 'ë¸©', 'ë¸ª', 'ë¸«', 'ë¸¬',
-'ë¸­', 'ë¸®', 'ë¸¯', 'ë¸°', 'ë¸±', 'ë¸²', 'ë¸³', 'ë¸´', 'ë¸µ', 'ë¸¶', 'ë¸·',
-'ë¸¸', 'ë¸¹', 'ë¸º', 'ë¸»', 'ë¸¼', 'ë¸½', 'ë¸¾', 'ë¸¿', 'ë¹', 'ë¹', 'ë¹',
-'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹',
-'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹¢', 'ë¹£', 'ë¹¥', 'ë¹¦',
-'ë¹§', 'ë¹©', 'ë¹«', 'ë¹¬', 'ë¹­', 'ë¹®', 'ë¹¯', 'ë¹²', 'ë¹¶', 'ë¹·', 'ë¹¸',
-'ë¹¹', 'ë¹º', 'ë¹¾', 'ë¹¿', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº',
-'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº',
-'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº ', 'ëº¡', 'ëº¢', 'ëº£', 'ëº¤', 'ëº¥',
-'ëº¦', 'ëº§', 'ëº©', 'ëºª', 'ëº«', 'ëº¬', 'ëº­', 'ëº®', 'ëº¯', 'ëº°', 'ëº±',
-'ëº²', 'ëº³', 'ëº´', 'ëºµ', 'ëº¶', 'ëº·', 'ëº¸', 'ëº¹', 'ëºº', 'ëº»', 'ëº¼',
-'ëº½', 'ëº¾', 'ëº¿', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»',
-'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»',
-'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»¡', 'ë»¢', 'ë»¦',
-'ë»§', 'ë»¨', 'ë»©', 'ë»ª', 'ë»«', 'ë»­', 'ë»®', 'ë»¯', 'ë»°', 'ë»±', 'ë»²',
-'ë»³', 'ë»´', 'ë»µ', 'ë»¶', 'ë»·', 'ë»¸', 'ë»¹', 'ë»º', 'ë»»', 'ë»¼', 'ë»½',
-'ë»¾', 'ë»¿', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼',
-'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼',
-'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼ ', 'ë¼¡', 'ë¼¢', 'ë¼£', 'ë¼¤', 'ë¼¥', 'ë¼¦',
-'ë¼§', 'ë¼¨', 'ë¼©', 'ë¼ª', 'ë¼«', 'ë¼¬', 'ë¼­', 'ë¼®', 'ë¼¯', 'ë¼°', 'ë¼±',
-'ë¼²', 'ë¼³', 'ë¼´', 'ë¼µ', 'ë¼¶', 'ë¼·', 'ë¼¸', 'ë¼¹', 'ë¼º', 'ë¼»', 'ë¼¼',
-'ë¼½', 'ë¼¾', 'ë¼¿', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½',
-'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½',
-'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½ ', 'ë½¡', 'ë½¢', 'ë½£', 'ë½¤',
-'ë½¥', 'ë½¦', 'ë½§', 'ë½¨', 'ë½©', 'ë½ª', 'ë½«', 'ë½¬', 'ë½­', 'ë½®', 'ë½¯',
-'ë½°', 'ë½±', 'ë½²', 'ë½³', 'ë½´', 'ë½µ', 'ë½¶', 'ë½·', 'ë½¸', 'ë½¹', 'ë½º',
-'ë½»', 'ë½¼', 'ë½½', 'ë½¾', 'ë½¿', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾',
-'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾',
-'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾', 'ë¾',
-'ë¾', 'ë¾', 'ë¾', 'ë¾ ', 'ë¾¡', 'ë¾¢', 'ë¾£', 'ë¾¤', 'ë¾¥', 'ë¾¦', 'ë¾§',
-'ë¾¨', 'ë¾©', 'ë¾ª', 'ë¾«', 'ë¾¬', 'ë¾­', 'ë¾®', 'ë¾¯', 'ë¾±', 'ë¾²', 'ë¾³',
-'ë¾´', 'ë¾µ', 'ë¾¶', 'ë¾·', 'ë¾¸', 'ë¾¹', 'ë¾º', 'ë¾»', 'ë¾¼', 'ë¾½', 'ë¾¾',
-'ë¾¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿',
-'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿',
-'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿ ', 'ë¿¢', 'ë¿£', 'ë¿¤', 'ë¿¥', 'ë¿¦', 'ë¿§',
-'ë¿¨', 'ë¿©', 'ë¿ª', 'ë¿«', 'ë¿¬', 'ë¿­', 'ë¿®', 'ë¿¯', 'ë¿°', 'ë¿±', 'ë¿²',
-'ë¿³', 'ë¿´', 'ë¿µ', 'ë¿¶', 'ë¿·', 'ë¿¸', 'ë¿¹', 'ë¿º', 'ë¿»', 'ë¿¼', 'ë¿½',
-'ë¿¾', 'ë¿¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ì¨', 'ì©',
-'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì´',
-'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì½', 'ì¾', 'ì¿', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥',
-'ì¦', 'ì§', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²',
-'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½',
-'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¢', 'ì¤', 'ì¦',
-'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì®', 'ì±', 'ì²', 'ì·', 'ì¸', 'ì¹',
-'ìº', 'ì»', 'ì¾', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì­',
-'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì¶', 'ì¸', 'ìº', 'ì»', 'ì¼',
-'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì¥', 'ì¨', 'ì©', 'ìª', 'ì«',
-'ì®', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì·', 'ìº', 'ì»', 'ì½', 'ì¾', 'ì¿',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¦', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯',
-'ì±', 'ì²', 'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½',
-'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì ', 'ì¢', 'ì£', 'ì¤', 'ì¦', 'ì§', 'ìª', 'ì«', 'ì­',
-'ì®', 'ì¯', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹',
-'ìº', 'ì»', 'ì¼', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢',
-'ì£', 'ì¥', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯',
-'ì²', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì¿',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ìª', 'ì¬', 'ì®', 'ì°',
-'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾',
-'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¦',
-'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì®', 'ì¯', 'ì±', 'ì²', 'ì³', 'ìµ',
-'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ',
-'ì¡', 'ì¢', 'ì£', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì®', 'ì¯', 'ì°',
-'ì±', 'ì²', 'ì³', 'ì¶', 'ì¸', 'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì¥',
-'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì®', 'ì°', 'ì²', 'ì³', 'ì´', 'ìµ',
-'ì·', 'ìº', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¦', 'ì§',
-'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì´',
-'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡',
-'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ìª', 'ì«', 'ì­', 'ì®', 'ì¯',
-'ì±', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ìº', 'ì»', 'ì¾', 'ì¿', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¤',
-'ì¥', 'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯',
-'ì°', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº',
-'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡',
-'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ìª', 'ì«', 'ì¬', 'ì®', 'ì¯', 'ì°',
-'ì±', 'ì²', 'ì³', 'ì¶', 'ì·', 'ì¹', 'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾',
-'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡',
-'ì¢', 'ì£', 'ì¥', 'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì­', 'ì®',
-'ì¯', 'ì±', 'ì²', 'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»',
-'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì­', 'ì®',
-'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì¶', 'ì·', 'ì¸', 'ìº', 'ì»', 'ì¼',
-'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ',
-'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì«',
-'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶',
-'ì·', 'ì¹', 'ìº', 'ì»', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¤',
-'ì¥', 'ì¦', 'ì§', 'ì¨', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì²',
-'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¹', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì ', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§', 'ìª',
-'ì«', 'ì­', 'ì®', 'ì¯', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·',
-'ìº', 'ì¼', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¢', 'ì£',
-'ì¥', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì²',
-'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì¿', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤',
-'ì¥', 'ì¦', 'ì§', 'ì¨', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°',
-'ì±', 'ì²', 'ì³', 'ì¶', 'ì·', 'ìº', 'ì¿', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì¢', 'ì¤', 'ì¦', 'ì§', 'ì¨', 'ì©', 'ìª',
-'ì«', 'ì¯', 'ì±', 'ì²', 'ì³', 'ìµ', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢',
-'ì£', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì¯', 'ì±', 'ì²', 'ì¶', 'ì¸',
-'ìº', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì§',
-'ì¨', 'ì©', 'ìª', 'ì«', 'ì­', 'ì®', 'ì°', 'ì²', 'ì³', 'ì´', 'ìµ',
-'ì¶', 'ì·', 'ìº', 'ì»', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¢',
-'ì£', 'ì¦', 'ì¨', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì²', 'ì³',
-'ìµ', 'ì¶', 'ì·', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¢', 'ì£', 'ì¤',
-'ì¥', 'ì¦', 'ì§', 'ìª', 'ì«', 'ì­', 'ì®', 'ì¯', 'ì±', 'ì²', 'ì³',
-'ì´', 'ìµ', 'ì¶', 'ì·', 'ìº', 'ì»', 'ì¼', 'ì¾', 'ì¿', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì¢', 'ì£', 'ì¥', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì¬', 'ì­', 'ì®',
-'ì¯', 'ì²', 'ì´', 'ì¶', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì¿', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¢', 'ì£', 'ì¤', 'ì¥', 'ì¦',
-'ì§', 'ì©', 'ìª', 'ì¬', 'ì­', 'ì®', 'ì¯', 'ì°', 'ì±', 'ì²', 'ì³',
-'ì¶', 'ì·', 'ì¹', 'ìº', 'ì»', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì¢', 'ì§', 'ì¨', 'ì©', 'ìª', 'ì«', 'ì®', 'ì¯', 'ì±', 'ì²',
-'ì³', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹', 'ìº', 'ì»', 'ì¾', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
-'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ',
-'ì¡', 'ì¢', 'ì£', 'ì¥', 'ì¦', 'ì§', 'ì©', 'ìª', 'ì«', 'ì­', 'ì®',
-'ì¯', 'ì°', 'ì±', 'ì²', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì·', 'ì¸', 'ì¹',
-'ìº', 'ì»', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ',
-'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ',
-'ì ', 'ì ', 'ì ', 'ì ', 'ì ¡', 'ì ¢', 'ì £', 'ì ¥', 'ì ¦', 'ì §', 'ì ¨',
-'ì ©', 'ì ª', 'ì «', 'ì ®', 'ì °', 'ì ²', 'ì ³', 'ì ´', 'ì µ', 'ì ¶', 'ì ·',
-'ì ¹', 'ì º', 'ì »', 'ì ½', 'ì ¾', 'ì ¿', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡',
-'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡',
-'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡ ',
-'ì¡¡', 'ì¡¢', 'ì¡£', 'ì¡¤', 'ì¡¥', 'ì¡¦', 'ì¡§', 'ì¡¨', 'ì¡©', 'ì¡ª', 'ì¡«',
-'ì¡¬', 'ì¡­', 'ì¡®', 'ì¡¯', 'ì¡²', 'ì¡³', 'ì¡µ', 'ì¡¶', 'ì¡·', 'ì¡¹', 'ì¡»',
-'ì¡¼', 'ì¡½', 'ì¡¾', 'ì¡¿', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢',
-'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢',
-'ì¢', 'ì¢', 'ì¢ ', 'ì¢¢', 'ì¢£', 'ì¢¤', 'ì¢¥', 'ì¢¦', 'ì¢§', 'ì¢©', 'ì¢ª',
-'ì¢«', 'ì¢¬', 'ì¢­', 'ì¢®', 'ì¢¯', 'ì¢°', 'ì¢±', 'ì¢²', 'ì¢³', 'ì¢´', 'ì¢µ',
-'ì¢¶', 'ì¢·', 'ì¢¸', 'ì¢¹', 'ì¢º', 'ì¢»', 'ì¢¾', 'ì¢¿', 'ì£', 'ì£', 'ì£',
-'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£',
-'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£',
-'ì£¢', 'ì££', 'ì£¥', 'ì£¦', 'ì£§', 'ì£¨', 'ì£©', 'ì£ª', 'ì£«', 'ì£¬', 'ì£­',
-'ì£®', 'ì£¯', 'ì£°', 'ì£±', 'ì£²', 'ì£³', 'ì£´', 'ì£¶', 'ì£·', 'ì£¸', 'ì£¹',
-'ì£º', 'ì£»', 'ì£¾', 'ì£¿', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤',
-'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤',
-'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤ ', 'ì¤¡', 'ì¤¢', 'ì¤£', 'ì¤¤', 'ì¤¥',
-'ì¤¦', 'ì¤§', 'ì¤¨', 'ì¤©', 'ì¤ª', 'ì¤«', 'ì¤­', 'ì¤®', 'ì¤¯', 'ì¤°', 'ì¤±',
-'ì¤²', 'ì¤³', 'ì¤µ', 'ì¤¶', 'ì¤·', 'ì¤¸', 'ì¤¹', 'ì¤º', 'ì¤»', 'ì¤¼', 'ì¤½',
-'ì¤¾', 'ì¤¿', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥',
-'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥',
-'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥¢', 'ì¥¤', 'ì¥¥',
-'ì¥¦', 'ì¥§', 'ì¥¨', 'ì¥©', 'ì¥ª', 'ì¥«', 'ì¥­', 'ì¥®', 'ì¥¯', 'ì¥±', 'ì¥²',
-'ì¥³', 'ì¥µ', 'ì¥¶', 'ì¥·', 'ì¥¸', 'ì¥¹', 'ì¥º', 'ì¥»', 'ì¥½', 'ì¥¾', 'ì¥¿',
-'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦',
-'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦',
-'ì¦', 'ì¦', 'ì¦ ', 'ì¦¡', 'ì¦¢', 'ì¦£', 'ì¦¤', 'ì¦¥', 'ì¦¦', 'ì¦§', 'ì¦¨',
-'ì¦©', 'ì¦ª', 'ì¦«', 'ì¦¬', 'ì¦­', 'ì¦®', 'ì¦¯', 'ì¦°', 'ì¦±', 'ì¦²', 'ì¦³',
-'ì¦´', 'ì¦µ', 'ì¦¶', 'ì¦·', 'ì¦¸', 'ì¦¹', 'ì¦º', 'ì¦»', 'ì¦¼', 'ì¦½', 'ì¦¾',
-'ì¦¿', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§',
-'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§¡', 'ì§£', 'ì§¥', 'ì§¦',
-'ì§¨', 'ì§©', 'ì§ª', 'ì§«', 'ì§®', 'ì§²', 'ì§³', 'ì§´', 'ì§µ', 'ì§¶', 'ì§·',
-'ì§º', 'ì§»', 'ì§½', 'ì§¾', 'ì§¿', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨',
-'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨',
-'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨ ', 'ì¨¡', 'ì¨¢', 'ì¨£',
-'ì¨¤', 'ì¨¥', 'ì¨¦', 'ì¨§', 'ì¨¨', 'ì¨ª', 'ì¨«', 'ì¨¬', 'ì¨­', 'ì¨®', 'ì¨¯',
-'ì¨°', 'ì¨±', 'ì¨²', 'ì¨³', 'ì¨´', 'ì¨µ', 'ì¨¶', 'ì¨·', 'ì¨¸', 'ì¨¹', 'ì¨º',
-'ì¨»', 'ì¨¼', 'ì¨½', 'ì¨¾', 'ì¨¿', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©',
-'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©',
-'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©¢', 'ì©£', 'ì©¤',
-'ì©¥', 'ì©¦', 'ì©§', 'ì©©', 'ì©ª', 'ì©«', 'ì©¬', 'ì©­', 'ì©®', 'ì©¯', 'ì©°',
-'ì©±', 'ì©²', 'ì©³', 'ì©´', 'ì©µ', 'ì©¶', 'ì©·', 'ì©¸', 'ì©¹', 'ì©º', 'ì©»',
-'ì©¼', 'ì©¾', 'ì©¿', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª',
-'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª',
-'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª', 'ìª',
-'ìª ', 'ìª¡', 'ìª¢', 'ìª£', 'ìª¤', 'ìª¥', 'ìª¦', 'ìª§', 'ìª¨', 'ìª©', 'ìªª',
-'ìª«', 'ìª¬', 'ìª­', 'ìª®', 'ìª¯', 'ìª°', 'ìª±', 'ìª²', 'ìª³', 'ìª´', 'ìªµ',
-'ìª¶', 'ìª·', 'ìª¸', 'ìª¹', 'ìªº', 'ìª»', 'ìª¾', 'ìª¿', 'ì«', 'ì«', 'ì«',
-'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«',
-'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«¡', 'ì«¢',
-'ì«£', 'ì«¤', 'ì«¥', 'ì«¦', 'ì«§', 'ì«¨', 'ì«©', 'ì«ª', 'ì««', 'ì«­', 'ì«®',
-'ì«¯', 'ì«°', 'ì«±', 'ì«²', 'ì«³', 'ì«µ', 'ì«¶', 'ì«·', 'ì«¸', 'ì«¹', 'ì«º',
-'ì«»', 'ì«¼', 'ì«½', 'ì«¾', 'ì«¿', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬',
-'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬',
-'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬',
-'ì¬¢', 'ì¬£', 'ì¬¤', 'ì¬¥', 'ì¬¦', 'ì¬§', 'ì¬¨', 'ì¬©', 'ì¬ª', 'ì¬«', 'ì¬¬',
-'ì¬­', 'ì¬®', 'ì¬¯', 'ì¬°', 'ì¬±', 'ì¬²', 'ì¬³', 'ì¬´', 'ì¬µ', 'ì¬¶', 'ì¬·',
-'ì¬¸', 'ì¬¹', 'ì¬º', 'ì¬»', 'ì¬¼', 'ì¬½', 'ì¬¾', 'ì¬¿', 'ì­', 'ì­', 'ì­',
-'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­',
-'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­ ',
-'ì­¡', 'ì­¢', 'ì­£', 'ì­¥', 'ì­¦', 'ì­§', 'ì­¨', 'ì­©', 'ì­ª', 'ì­«', 'ì­¬',
-'ì­­', 'ì­®', 'ì­¯', 'ì­°', 'ì­±', 'ì­²', 'ì­³', 'ì­´', 'ì­µ', 'ì­¶', 'ì­·',
-'ì­º', 'ì­»', 'ì­¼', 'ì­½', 'ì­¾', 'ì­¿', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®',
-'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®',
-'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®', 'ì®',
-'ì®', 'ì®', 'ì®', 'ì®', 'ì® ', 'ì®¡', 'ì®¢', 'ì®£', 'ì®¤', 'ì®¥', 'ì®¦',
-'ì®§', 'ì®¨', 'ì®©', 'ì®ª', 'ì®«', 'ì®¬', 'ì®­', 'ì®®', 'ì®¯', 'ì®°', 'ì®±',
-'ì®²', 'ì®³', 'ì®´', 'ì®µ', 'ì®¶', 'ì®·', 'ì®¹', 'ì®º', 'ì®»', 'ì®¼', 'ì®½',
-'ì®¾', 'ì®¿', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯',
-'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯',
-'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯', 'ì¯',
-'ì¯ ', 'ì¯¡', 'ì¯¢', 'ì¯£', 'ì¯¥', 'ì¯¦', 'ì¯¨', 'ì¯ª', 'ì¯«', 'ì¯¬', 'ì¯­',
-'ì¯®', 'ì¯¯', 'ì¯°', 'ì¯±', 'ì¯²', 'ì¯³', 'ì¯´', 'ì¯µ', 'ì¯¶', 'ì¯·', 'ì¯¸',
-'ì¯¹', 'ì¯º', 'ì¯»', 'ì¯¼', 'ì¯½', 'ì¯¾', 'ì¯¿', 'ì°', 'ì°', 'ì°', 'ì°',
-'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°',
-'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°',
-'ì° ', 'ì°£', 'ì°¤', 'ì°¥', 'ì°¦', 'ì°ª', 'ì°«', 'ì°­', 'ì°¯', 'ì°±', 'ì°²',
-'ì°³', 'ì°´', 'ì°µ', 'ì°¶', 'ì°·', 'ì°º', 'ì°¿', 'ì±', 'ì±', 'ì±', 'ì±',
-'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±',
-'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±¡', 'ì±¢', 'ì±£',
-'ì±¥', 'ì±§', 'ì±©', 'ì±ª', 'ì±«', 'ì±¬', 'ì±­', 'ì±®', 'ì±¯', 'ì±±', 'ì±²',
-'ì±³', 'ì±´', 'ì±¶', 'ì±·', 'ì±¸', 'ì±¹', 'ì±º', 'ì±»', 'ì±¼', 'ì±½', 'ì±¾',
-'ì±¿', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²',
-'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²',
-'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²', 'ì²¡', 'ì²¢', 'ì²£',
-'ì²¤', 'ì²¥', 'ì²¦', 'ì²§', 'ì²ª', 'ì²®', 'ì²¯', 'ì²°', 'ì²±', 'ì²²', 'ì²³',
-'ì²¶', 'ì²·', 'ì²¹', 'ì²º', 'ì²»', 'ì²½', 'ì²¾', 'ì²¿', 'ì³', 'ì³', 'ì³',
-'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³',
-'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³',
-'ì³', 'ì³ ', 'ì³¡', 'ì³¢', 'ì³£', 'ì³¥', 'ì³¦', 'ì³§', 'ì³¨', 'ì³©', 'ì³ª',
-'ì³«', 'ì³­', 'ì³®', 'ì³¯', 'ì³±', 'ì³²', 'ì³³', 'ì³´', 'ì³µ', 'ì³¶', 'ì³·',
-'ì³¸', 'ì³¹', 'ì³º', 'ì³»', 'ì³¼', 'ì³½', 'ì³¾', 'ì³¿', 'ì´', 'ì´', 'ì´',
-'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´',
-'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´ ', 'ì´¡',
-'ì´¢', 'ì´£', 'ì´¥', 'ì´¦', 'ì´§', 'ì´©', 'ì´ª', 'ì´«', 'ì´­', 'ì´®', 'ì´¯',
-'ì´°', 'ì´±', 'ì´²', 'ì´³', 'ì´´', 'ì´µ', 'ì´¶', 'ì´·', 'ì´¸', 'ì´º', 'ì´»',
-'ì´¼', 'ì´½', 'ì´¾', 'ì´¿', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ',
-'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ',
-'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ', 'ìµ',
-'ìµ', 'ìµ', 'ìµ¡', 'ìµ¢', 'ìµ£', 'ìµ¥', 'ìµ¦', 'ìµ§', 'ìµ¨', 'ìµ©', 'ìµª',
-'ìµ«', 'ìµ®', 'ìµ°', 'ìµ²', 'ìµ³', 'ìµ´', 'ìµµ', 'ìµ¶', 'ìµ·', 'ìµ¹', 'ìµº',
-'ìµ»', 'ìµ¼', 'ìµ½', 'ìµ¾', 'ìµ¿', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶',
-'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶',
-'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶', 'ì¶ ',
-'ì¶¡', 'ì¶¢', 'ì¶£', 'ì¶¦', 'ì¶¨', 'ì¶ª', 'ì¶«', 'ì¶¬', 'ì¶­', 'ì¶®', 'ì¶¯',
-'ì¶±', 'ì¶²', 'ì¶³', 'ì¶´', 'ì¶µ', 'ì¶¶', 'ì¶·', 'ì¶¸', 'ì¶¹', 'ì¶º', 'ì¶»',
-'ì¶¼', 'ì¶½', 'ì¶¾', 'ì¶¿', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·',
-'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·',
-'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·', 'ì·',
-'ì· ', 'ì·¡', 'ì·¢', 'ì·£', 'ì·¤', 'ì·¥', 'ì·¦', 'ì·§', 'ì·©', 'ì·ª', 'ì·«',
-'ì·­', 'ì·®', 'ì·¯', 'ì·±', 'ì·²', 'ì·³', 'ì·´', 'ì·µ', 'ì·¶', 'ì··', 'ì·º',
-'ì·¼', 'ì·¾', 'ì·¿', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸',
-'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸',
-'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸¢', 'ì¸£', 'ì¸¥',
-'ì¸¦', 'ì¸§', 'ì¸©', 'ì¸ª', 'ì¸«', 'ì¸¬', 'ì¸­', 'ì¸®', 'ì¸¯', 'ì¸²', 'ì¸´',
-'ì¸¶', 'ì¸·', 'ì¸¸', 'ì¸¹', 'ì¸º', 'ì¸»', 'ì¸¼', 'ì¸½', 'ì¸¾', 'ì¸¿', 'ì¹',
-'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹',
-'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹',
-'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹', 'ì¹¢', 'ì¹£', 'ì¹¤', 'ì¹¥', 'ì¹¦', 'ì¹§',
-'ì¹ª', 'ì¹¬', 'ì¹®', 'ì¹¯', 'ì¹°', 'ì¹±', 'ì¹²', 'ì¹³', 'ì¹¶', 'ì¹·', 'ì¹¹',
-'ì¹º', 'ì¹»', 'ì¹½', 'ì¹¾', 'ì¹¿', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº',
-'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº',
-'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº¢', 'ìº¦', 'ìº§', 'ìº¨',
-'ìº©', 'ìºª', 'ìº«', 'ìº®', 'ìº¯', 'ìº°', 'ìº±', 'ìº²', 'ìº³', 'ìº´', 'ìºµ',
-'ìº¶', 'ìº·', 'ìº¸', 'ìº¹', 'ìºº', 'ìº»', 'ìº¼', 'ìº½', 'ìº¾', 'ìº¿', 'ì»',
-'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»',
-'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»',
-'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì»', 'ì» ', 'ì»¡', 'ì»¢',
-'ì»£', 'ì»¦', 'ì»§', 'ì»©', 'ì»ª', 'ì»­', 'ì»®', 'ì»¯', 'ì»°', 'ì»±', 'ì»²',
-'ì»³', 'ì»¶', 'ì»º', 'ì»»', 'ì»¼', 'ì»½', 'ì»¾', 'ì»¿', 'ì¼', 'ì¼', 'ì¼',
-'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼',
-'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼¡', 'ì¼¢',
-'ì¼£', 'ì¼¥', 'ì¼¦', 'ì¼§', 'ì¼¨', 'ì¼©', 'ì¼ª', 'ì¼«', 'ì¼®', 'ì¼²', 'ì¼³',
-'ì¼´', 'ì¼µ', 'ì¼¶', 'ì¼·', 'ì¼¹', 'ì¼º', 'ì¼»', 'ì¼¼', 'ì¼½', 'ì¼¾', 'ì¼¿',
-'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½',
-'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½',
-'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½', 'ì½ ', 'ì½¡', 'ì½¢', 'ì½£', 'ì½¦',
-'ì½¨', 'ì½ª', 'ì½«', 'ì½¬', 'ì½­', 'ì½®', 'ì½¯', 'ì½²', 'ì½³', 'ì½µ', 'ì½¶',
-'ì½·', 'ì½¹', 'ì½º', 'ì½»', 'ì½¼', 'ì½½', 'ì½¾', 'ì½¿', 'ì¾', 'ì¾', 'ì¾',
-'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾',
-'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾',
-'ì¾', 'ì¾', 'ì¾', 'ì¾', 'ì¾ ', 'ì¾¢', 'ì¾£', 'ì¾¤', 'ì¾¥', 'ì¾¦', 'ì¾§',
-'ì¾©', 'ì¾ª', 'ì¾«', 'ì¾¬', 'ì¾­', 'ì¾®', 'ì¾¯', 'ì¾±', 'ì¾²', 'ì¾³', 'ì¾´',
-'ì¾µ', 'ì¾¶', 'ì¾·', 'ì¾¸', 'ì¾¹', 'ì¾º', 'ì¾»', 'ì¾¼', 'ì¾½', 'ì¾¾', 'ì¾¿',
-'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿',
-'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿',
-'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿', 'ì¿¢', 'ì¿£',
-'ì¿¥', 'ì¿¦', 'ì¿§', 'ì¿©', 'ì¿ª', 'ì¿«', 'ì¿¬', 'ì¿­', 'ì¿®', 'ì¿¯', 'ì¿²',
-'ì¿´', 'ì¿¶', 'ì¿·', 'ì¿¸', 'ì¿¹', 'ì¿º', 'ì¿»', 'ì¿½', 'ì¿¾', 'ì¿¿', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¥',
-'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬', 'í®', 'í¯', 'í°', 'í±',
-'í²', 'í³', 'í¶', 'í·', 'í¹', 'íº', 'í»', 'í½', 'í¾', 'í¿', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©',
-'íª', 'í«', 'í®', 'í¯', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¸',
-'í¹', 'íº', 'í»', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¦', 'í§', 'í©', 'íª',
-'í«', 'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í¶', 'í¸', 'íº',
-'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¥', 'í¦', 'í§', 'í¨', 'í©',
-'íª', 'í«', 'í®', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¹', 'íº',
-'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§',
-'í¨', 'í©', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯', 'í²', 'í³', 'íµ',
-'í¶', 'í·', 'í¹', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¢', 'í£', 'í¤', 'í¥',
-'í¦', 'í§', 'í©', 'íª', 'í«', 'í­', 'í®', 'í¯', 'í°', 'í±', 'í²',
-'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¸', 'í¹', 'íº', 'í»', 'í½', 'í¾',
-'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í¢', 'í£',
-'í¥', 'í¦', 'í§', 'í©', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯', 'í²',
-'í´', 'í¶', 'í·', 'í¸', 'í¹', 'í»', 'í½', 'í¾', 'í¿', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤',
-'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯',
-'í°', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¹', 'íº', 'í»', 'í¼',
-'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ',
-'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¸', 'í¹', 'íº',
-'í»', 'í¾', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬', 'í­',
-'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¸',
-'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¢',
-'í£', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í­', 'í®', 'í¯',
-'í°', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'íº', 'í»', 'í½', 'í¾',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¦', 'í§', 'í¨', 'í©', 'íª',
-'í«', 'í¬', 'í­', 'í®', 'í¯', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¹',
-'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í¢', 'í£', 'í¤', 'í¦', 'í§', 'íª', 'í«', 'í­',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'íº', 'í¾',
-'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬',
-'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'í¸', 'í¹', 'íº', 'í»', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¤', 'í¥',
-'í¦', 'í§', 'íª', 'í¬', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'íµ',
-'í¶', 'í·', 'í¹', 'íº', 'í»', 'í½', 'í¾', 'í¿', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í ', 'í¢', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¸', 'í¹', 'íº',
-'í»', 'í¾', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬',
-'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'í¸', 'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¥', 'í¦', 'í§', 'í¨',
-'í©', 'íª', 'í«', 'í¬', 'í®', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ',
-'í¶', 'í·', 'íº', 'í»', 'í½', 'í¾', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'íª', 'í«', 'í¬', 'í­',
-'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¸',
-'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í©', 'íª',
-'í«', 'í­', 'í®', 'í¯', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'í¹', 'íº', 'í¼', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡',
-'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«', 'í¬',
-'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'í¸', 'í¹', 'íº', 'í»', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¤',
-'í¦', 'í§', 'íª', 'í¬', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í¶',
-'í·', 'í¹', 'íº', 'í»', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«',
-'í¬', 'í­', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶',
-'í·', 'í¸', 'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ',
-'í¡', 'í¢', 'í£', 'í¦', 'í§', 'í©', 'íª', 'í«', 'í­', 'í®', 'í¯',
-'í°', 'í±', 'í²', 'í³', 'í¶', 'í¸', 'íº', 'í»', 'í¼', 'í½', 'í¾',
-'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í¡', 'í¢', 'í£', 'í¥', 'í¦', 'í§', 'í¨', 'í©', 'íª', 'í«',
-'í¬', 'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·',
-'íº', 'í»', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦',
-'í¨', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯', 'í²', 'í³', 'íµ', 'í¶',
-'í·', 'í¸', 'í¹', 'íº', 'í»', 'í¼', 'í½', 'í¾', 'í¿', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í ', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'í©', 'íª', 'í«', 'í­',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'í´', 'íµ', 'í¶', 'í·', 'í¸', 'íº',
-'í¼', 'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¢', 'í£', 'í¥', 'í¦',
-'í§', 'í©', 'íª', 'í«', 'í¬', 'í­', 'í®', 'í¯', 'í±', 'í²', 'í³',
-'í´', 'í¶', 'í·', 'í¸', 'í¹', 'íº', 'í»', 'í¾', 'í¿', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í¡', 'í¢', 'í£', 'í¤', 'í¥', 'í¦', 'í§', 'íª', 'í¬',
-'í®', 'í¯', 'í°', 'í±', 'í²', 'í³', 'í¶', 'í·', 'í¹', 'íº', 'í»',
-'í½', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í¢', 'í¤', 'í¦', 'í§', 'í¨', 'íª', 'í«', 'í­',
-'í®', 'í¯', 'í±', 'í²', 'í³', 'íµ', 'í¶', 'í·', 'í¸', 'í¹', 'íº',
-'í»', 'í¾', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
-'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¢', 'í£', '\ud7a4'] ``` 28.
-get_all_incompleted_form_hangul_chars This returns all non-completed form
-Hangul characters. Returns: - `List[str]`: all non-completed form Hangul
-characters Examples: ```python >>> from kss import Kss >>>
-get_all_incompleted_form_hangul_chars = Kss
+get_all_completed_form_hangul_chars = Kss
+("get_all_completed_form_hangul_chars") >>> output =
+get_all_completed_form_hangul_chars() >>> print(output) ['ê°', 'ê°', 'ê°',
+'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°',
+'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê° ', 'ê°¤', 'ê°¬', 'ê°­', 'ê°¯',
+'ê°°', 'ê°±', 'ê°¸', 'ê°¹', 'ê°¼', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
+'ê±°', 'ê±±', 'ê±´', 'ê±·', 'ê±¸', 'ê±º', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²',
+'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê²', 'ê² ',
+'ê²¡', 'ê²¨', 'ê²©', 'ê²ª', 'ê²¬', 'ê²¯', 'ê²°', 'ê²¸', 'ê²¹', 'ê²»', 'ê²¼',
+'ê²½', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³', 'ê³ ', 'ê³¡', 'ê³¤', 'ê³§',
+'ê³¨', 'ê³ª', 'ê³¬', 'ê³¯', 'ê³°', 'ê³±', 'ê³³', 'ê³µ', 'ê³¶', 'ê³¼', 'ê³½',
+'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´', 'ê´ ', 'ê´©',
+'ê´¬', 'ê´­', 'ê´´', 'ê´µ', 'ê´¸', 'ê´¼', 'êµ', 'êµ', 'êµ', 'êµ', 'êµ',
+'êµ', 'êµ', 'êµ¡', 'êµ£', 'êµ¬', 'êµ­', 'êµ°', 'êµ³', 'êµ´', 'êµµ', 'êµ¶',
+'êµ»', 'êµ¼', 'êµ½', 'êµ¿', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶', 'ê¶',
+'ê¶', 'ê¶¤', 'ê¶·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·', 'ê·',
+'ê· ', 'ê·¤', 'ê·¸', 'ê·¹', 'ê·¼', 'ê·¿', 'ê¸', 'ê¸', 'ê¸', 'ê¸', 'ê¸',
+'ê¸', 'ê¸', 'ê¸°', 'ê¸±', 'ê¸´', 'ê¸·', 'ê¸¸', 'ê¸º', 'ê¹', 'ê¹', 'ê¹',
+'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹', 'ê¹',
+'ê¹', 'ê¹ ', 'ê¹¡', 'ê¹¥', 'ê¹¨', 'ê¹©', 'ê¹¬', 'ê¹°', 'ê¹¸', 'ê¹¹', 'ê¹»',
+'ê¹¼', 'ê¹½', 'êº', 'êº', 'êº', 'êº¼', 'êº½', 'êº¾', 'ê»', 'ê»', 'ê»',
+'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»', 'ê»¨', 'ê»«', 'ê»­', 'ê»´',
+'ê»¸', 'ê»¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼', 'ê¼¬', 'ê¼­', 'ê¼°', 'ê¼²', 'ê¼´',
+'ê¼¼', 'ê¼½', 'ê¼¿', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½', 'ê½',
+'ê½¤', 'ê½¥', 'ê½¹', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾', 'ê¾¸',
+'ê¾¹', 'ê¾¼', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿', 'ê¿',
+'ê¿¨', 'ê¿©', 'ê¿°', 'ê¿±', 'ê¿´', 'ê¿¸', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë¨', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë¼', 'ë½', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë¢', 'ë¨',
+'ë©', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë±', 'ë³', 'ë´', 'ëµ', 'ë¸',
+'ë¼', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ',
+'ë¥', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë£', 'ë¤', 'ë¥', 'ë¨', 'ë¬', 'ë´', 'ëµ', 'ë·', 'ë¸',
+'ë¹', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë ', 'ë¸', 'ë¹', 'ë¼', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë¨', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë¨', 'ë©', 'ë¬', 'ë°', 'ë¹', 'ë»', 'ë½', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë´', 'ë¼', 'ë', 'ë', 'ë ',
+'ë¨', 'ë©', 'ë´', 'ëµ', 'ë¼', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë ', 'ë¡', 'ë£', 'ë¥', 'ë¦', 'ëª', 'ë¬', 'ë°',
+'ë´', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë¢',
+'ë¤', 'ë¥', 'ë¦', 'ë¨', 'ë«', 'ë¬', 'ë­', 'ë®', 'ë¯', 'ë³', 'ë´',
+'ëµ', 'ë·', 'ë¸', 'ë¹', 'ëº', 'ë»', 'ë¿', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë¤', 'ë¥', 'ë§', 'ë©', 'ë«', 'ë®', 'ë°', 'ë±',
+'ë´', 'ë¸', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ',
+'ë¡', 'ë¨', 'ë¬', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¤', 'ë¨', 'ë¼', 'ë', 'ë',
+'ë', 'ë ', 'ë¨', 'ë©', 'ë«', 'ë´', 'ë', 'ë', 'ë', 'ë', 'ë ',
+'ë¡', 'ë£', 'ë¥', 'ë¬', 'ë', 'ë', 'ë', 'ë¤', 'ë¨', 'ë¬', 'ëµ',
+'ë·', 'ë¹', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë£',
+'ë¤', 'ë¦', 'ë¬', 'ë­', 'ë¯', 'ë±', 'ë¸', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë¤', 'ë¥', 'ë§', 'ë¨', 'ë©', 'ëª', 'ë°', 'ë±', 'ë´', 'ë¸',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë ', 'ë¡', 'ë ', 'ë¡', 'ë¤', 'ë¨', 'ëª', 'ë«', 'ë°',
+'ë±', 'ë³', 'ë´', 'ëµ', 'ë»', 'ë¼', 'ë½', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë¬', 'ë', 'ë', 'ë', 'ë', 'ë¥', 'ë¬',
+'ë´', 'ë', 'ë¤', 'ë¨', 'ë', 'ë', 'ë ', 'ë¤', 'ë«', 'ë¬', 'ë±',
+'ë', 'ë°', 'ë´', 'ë¸', 'ë', 'ë', 'ë', 'ë¨', 'ë©', 'ë¬', 'ë¯',
+'ë°', 'ë¸', 'ë¹', 'ë»', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¤',
+'ë¨', 'ë°', 'ë±', 'ë³', 'ëµ', 'ë¼', 'ë½', 'ë', 'ë', 'ë', 'ë',
+'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë', 'ë ', 'ë¨',
+'ë©', 'ë«', 'ë¬', 'ë­', 'ë´', 'ëµ', 'ë¸', 'ë', 'ë', 'ë¬', 'ë­',
+'ë°', 'ë´', 'ë¼', 'ë½', 'ë¿', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ',
+'ë ', 'ë ', 'ë ', 'ë ', 'ë ', 'ë ¤', 'ë ¥', 'ë ¨', 'ë ¬', 'ë ´', 'ë µ',
+'ë ·', 'ë ¸', 'ë ¹', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡', 'ë¡ ', 'ë¡¤',
+'ë¡¬', 'ë¡­', 'ë¡¯', 'ë¡±', 'ë¡¸', 'ë¡¼', 'ë¢', 'ë¢¨', 'ë¢°', 'ë¢´', 'ë¢¸',
+'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£', 'ë£¡', 'ë£¨',
+'ë£©', 'ë£¬', 'ë£°', 'ë£¸', 'ë£¹', 'ë£»', 'ë£½', 'ë¤', 'ë¤', 'ë¤ ', 'ë¤¼',
+'ë¤½', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥', 'ë¥ ', 'ë¥¨',
+'ë¥©', 'ë¥«', 'ë¥­', 'ë¥´', 'ë¥µ', 'ë¥¸', 'ë¥¼', 'ë¦', 'ë¦', 'ë¦', 'ë¦',
+'ë¦', 'ë¦', 'ë¦', 'ë¦¬', 'ë¦­', 'ë¦°', 'ë¦´', 'ë¦¼', 'ë¦½', 'ë¦¿', 'ë§',
+'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§', 'ë§',
+'ë§', 'ë§', 'ë§¡', 'ë§£', 'ë§¤', 'ë§¥', 'ë§¨', 'ë§¬', 'ë§´', 'ë§µ', 'ë§·',
+'ë§¸', 'ë§¹', 'ë§º', 'ë¨', 'ë¨', 'ë¨', 'ë¨', 'ë¨¸', 'ë¨¹', 'ë¨¼', 'ë©',
+'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©', 'ë©',
+'ë©¤', 'ë©¥', 'ë©§', 'ë©¨', 'ë©©', 'ë©°', 'ë©±', 'ë©´', 'ë©¸', 'ëª', 'ëª',
+'ëª', 'ëª', 'ëª', 'ëª¨', 'ëª©', 'ëª«', 'ëª¬', 'ëª°', 'ëª²', 'ëª¸', 'ëª¹',
+'ëª»', 'ëª½', 'ë«', 'ë«', 'ë«', 'ë«', 'ë«¼', 'ë¬', 'ë¬', 'ë¬', 'ë¬',
+'ë¬', 'ë¬', 'ë¬', 'ë¬ ', 'ë¬©', 'ë¬«', 'ë¬´', 'ë¬µ', 'ë¬¶', 'ë¬¸', 'ë¬»',
+'ë¬¼', 'ë¬½', 'ë¬¾', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­', 'ë­',
+'ë­', 'ë­¡', 'ë­£', 'ë­¬', 'ë®', 'ë®', 'ë®', 'ë®¤', 'ë®¨', 'ë®¬', 'ë®´',
+'ë®·', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯', 'ë¯¸', 'ë¯¹', 'ë¯¼', 'ë¯¿', 'ë°',
+'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°',
+'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°', 'ë°¤', 'ë°¥', 'ë°§', 'ë°©',
+'ë°­', 'ë°°', 'ë°±', 'ë°´', 'ë°¸', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±', 'ë±',
+'ë±', 'ë±', 'ë±', 'ë±', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²', 'ë²',
+'ë²', 'ë²', 'ë²', 'ë²', 'ë² ', 'ë²¡', 'ë²¤', 'ë²§', 'ë²¨', 'ë²°', 'ë²±',
+'ë²³', 'ë²´', 'ë²µ', 'ë²¼', 'ë²½', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³', 'ë³',
+'ë³', 'ë³', 'ë³', 'ë³´', 'ë³µ', 'ë³¶', 'ë³¸', 'ë³¼', 'ë´', 'ë´', 'ë´',
+'ë´', 'ë´', 'ë´', 'ë´¤', 'ë´¬', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ', 'ëµ',
+'ëµ', 'ëµ¤', 'ëµ¨', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶',
+'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶', 'ë¶¤', 'ë¶°', 'ë¶¸', 'ë·', 'ë·',
+'ë·', 'ë·', 'ë·©', 'ë·°', 'ë·´', 'ë·¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸',
+'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¸', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹',
+'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹', 'ë¹ ', 'ë¹¡', 'ë¹¤', 'ë¹¨', 'ë¹ª', 'ë¹°',
+'ë¹±', 'ë¹³', 'ë¹´', 'ë¹µ', 'ë¹»', 'ë¹¼', 'ë¹½', 'ëº', 'ëº', 'ëº', 'ëº',
+'ëº', 'ëº', 'ëº', 'ëº', 'ëº', 'ëº¨', 'ë»', 'ë»', 'ë»', 'ë»', 'ë»',
+'ë» ', 'ë»£', 'ë»¤', 'ë»¥', 'ë»¬', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼', 'ë¼',
+'ë¼', 'ë¼', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë½', 'ë¾', 'ë¾°',
+'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿', 'ë¿¡', 'ì¼', 'ì', 'ì',
+'ì', 'ì ', 'ì¨', 'ì©', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì£',
+'ì¥', 'ì¬', 'ì­', 'ì¯', 'ì°', 'ì³', 'ì´', 'ìµ', 'ì¶', 'ì¼', 'ì½',
+'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì¤', 'ì¥', 'ì¨', 'ì¬', 'ì´', 'ìµ', 'ì·', 'ì¹', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì£', 'ì¤',
+'ì¦', 'ì§', 'ì¬', 'ì­', 'ì¯', 'ì°', 'ì±', 'ì¶', 'ì¸', 'ì¹', 'ì¼',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¤',
+'ì¥', 'ì§', 'ì¨', 'ì©', 'ì°', 'ì´', 'ì¸', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¡', 'ì¥', 'ì¨', 'ì©', 'ì¬',
+'ì°', 'ì½', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¤', 'ì¨',
+'ì°', 'ì±', 'ì³', 'ì¼', 'ì½', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¨', 'ì©', 'ì«', 'ì­', 'ì¯', 'ì±',
+'ì²', 'ì´', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¥', 'ì¬', 'ì­',
+'ì°', 'ì´', 'ì¼', 'ì½', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì¤', 'ì¥', 'ì¨', 'ì¬', 'ì­', 'ì´', 'ìµ', 'ì·', 'ì¹', 'ì',
+'ì', 'ì ', 'ì£', 'ì¤', 'ì«', 'ì¬', 'ì­', 'ì¯', 'ì±', 'ì¶', 'ì¸',
+'ì¹', 'ì»', 'ì¼', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì¤', 'ì¥', 'ì¨', 'ì©', 'ì', 'ì¨', 'ì©', 'ì¬', 'ì°',
+'ì²', 'ì¸', 'ì¹', 'ì¼', 'ì½', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì ', 'ì¢', 'ì¨', 'ì©', 'ì­', 'ì´', 'ìµ', 'ì¸', 'ì',
+'ì', 'ì¤', 'ì¬', 'ì°', 'ì´', 'ì¼', 'ì½', 'ì', 'ì¤', 'ì¥', 'ì¨',
+'ì¬', 'ì´', 'ìµ', 'ì¹', 'ì', 'ì', 'ì', 'ì¸', 'ì¼', 'ì©', 'ì°',
+'ì±', 'ì´', 'ì¸', 'ìº', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì¨', 'ì©', 'ì¬', 'ì°', 'ì¸', 'ì¹', 'ì»', 'ì½', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì ', 'ì¡', 'ì¤', 'ì¨', 'ì°', 'ì±', 'ì³', 'ì´', 'ìµ',
+'ì¼', 'ì½', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì ', 'ì©', 'ì´', 'ìµ', 'ì¸', 'ì¹', 'ì»', 'ì¼', 'ì½',
+'ì¾', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì£', 'ì¥', 'ì¬', 'ì­', 'ì®', 'ì°',
+'ì´', 'ì¶', 'ì·', 'ì¼', 'ì½', 'ì¾', 'ì¿', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì¤', 'ì¥', 'ì¨',
+'ì¬', 'ì­', 'ì®', 'ì°', 'ì³', 'ì´', 'ìµ', 'ì·', 'ì¹', 'ì»', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ',
+'ì¬', 'ì¯', 'ì±', 'ì¸', 'ì¹', 'ì¼', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì¤', 'ì¥', 'ì§', 'ì©', 'ì°', 'ì±', 'ì´',
+'ì¸', 'ì¹', 'ìº', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì ', 'ì¡', 'ì¨', 'ì©', 'ì¬', 'ì°', 'ì¸', 'ì¹', 'ì½',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì¤',
+'ì¨', 'ì°', 'ì±', 'ì³', 'ìµ', 'ì·', 'ì¼', 'ì½', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì ', 'ì¨', 'ì«', 'ì´', 'ìµ', 'ì¸', 'ì¼', 'ì½', 'ì¾', 'ì',
+'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì ', 'ì¡', 'ì£', 'ì¤', 'ì¥', 'ì¦', 'ì¬', 'ì­',
+'ì°', 'ì´', 'ì¼', 'ì½', 'ì¿', 'ì', 'ì', 'ì', 'ì', 'ì', 'ì',
+'ì', 'ì', 'ì', 'ì¤', 'ì¨', 'ì¬', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ',
+'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì ', 'ì  ', 'ì ¤', 'ì ¬', 'ì ­',
+'ì ¯', 'ì ±', 'ì ¸', 'ì ¼', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡', 'ì¡°',
+'ì¡±', 'ì¡´', 'ì¡¸', 'ì¡º', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢',
+'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢', 'ì¢¡', 'ì¢¨', 'ì¢¼', 'ì¢½', 'ì£', 'ì£',
+'ì£', 'ì£', 'ì£', 'ì£', 'ì£', 'ì£ ', 'ì£¡', 'ì£¤', 'ì£µ', 'ì£¼', 'ì£½',
+'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤', 'ì¤¬', 'ì¤´',
+'ì¥', 'ì¥', 'ì¥', 'ì¥', 'ì¥ ', 'ì¥¡', 'ì¥£', 'ì¥¬', 'ì¥°', 'ì¥´', 'ì¥¼',
+'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì¦', 'ì§', 'ì§', 'ì§',
+'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§', 'ì§',
+'ì§', 'ì§ ', 'ì§¢', 'ì§¤', 'ì§§', 'ì§¬', 'ì§­', 'ì§¯', 'ì§°', 'ì§±', 'ì§¸',
+'ì§¹', 'ì§¼', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨', 'ì¨©',
+'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì©', 'ì© ', 'ì©¡', 'ì©¨', 'ì©½',
+'ìª', 'ìª', 'ìª¼', 'ìª½', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«', 'ì«',
+'ì«', 'ì«', 'ì« ', 'ì«¬', 'ì«´', 'ì¬', 'ì¬', 'ì¬', 'ì¬', 'ì¬ ', 'ì¬¡',
+'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­', 'ì­¤', 'ì­¸', 'ì­¹',
+'ì®', 'ì®¸', 'ì¯', 'ì¯¤', 'ì¯§', 'ì¯©', 'ì°', 'ì°', 'ì°', 'ì°', 'ì°',
+'ì°', 'ì°¡', 'ì°¢', 'ì°§', 'ì°¨', 'ì°©', 'ì°¬', 'ì°®', 'ì°°', 'ì°¸', 'ì°¹',
+'ì°»', 'ì°¼', 'ì°½', 'ì°¾', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±', 'ì±',
+'ì±', 'ì±', 'ì± ', 'ì±¤', 'ì±¦', 'ì±¨', 'ì±°', 'ì±µ', 'ì²', 'ì²', 'ì²',
+'ì² ', 'ì²¨', 'ì²©', 'ì²«', 'ì²¬', 'ì²­', 'ì²´', 'ì²µ', 'ì²¸', 'ì²¼', 'ì³',
+'ì³', 'ì³', 'ì³', 'ì³', 'ì³', 'ì³¤', 'ì³¬', 'ì³°', 'ì´', 'ì´', 'ì´',
+'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´', 'ì´¤', 'ì´¨', 'ì´¬', 'ì´¹', 'ìµ',
+'ìµ ', 'ìµ¤', 'ìµ¬', 'ìµ­', 'ìµ¯', 'ìµ±', 'ìµ¸', 'ì¶', 'ì¶', 'ì¶', 'ì¶',
+'ì¶', 'ì¶¤', 'ì¶¥', 'ì¶§', 'ì¶©', 'ì¶°', 'ì·', 'ì·', 'ì·', 'ì·¨', 'ì·¬',
+'ì·°', 'ì·¸', 'ì·¹', 'ì·»', 'ì·½', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸', 'ì¸ ',
+'ì¸¡', 'ì¸¤', 'ì¸¨', 'ì¸°', 'ì¸±', 'ì¸³', 'ì¸µ', 'ì¹', 'ì¹', 'ì¹', 'ì¹',
+'ì¹ ', 'ì¹¡', 'ì¹¨', 'ì¹©', 'ì¹«', 'ì¹­', 'ì¹´', 'ì¹µ', 'ì¹¸', 'ì¹¼', 'ìº',
+'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº', 'ìº ', 'ìº¡', 'ìº£', 'ìº¤',
+'ìº¥', 'ìº¬', 'ìº­', 'ì»', 'ì»¤', 'ì»¥', 'ì»¨', 'ì»«', 'ì»¬', 'ì»´', 'ì»µ',
+'ì»·', 'ì»¸', 'ì»¹', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼', 'ì¼',
+'ì¼', 'ì¼ ', 'ì¼¤', 'ì¼¬', 'ì¼­', 'ì¼¯', 'ì¼°', 'ì¼±', 'ì¼¸', 'ì½', 'ì½',
+'ì½', 'ì½', 'ì½¤', 'ì½¥', 'ì½§', 'ì½©', 'ì½°', 'ì½±', 'ì½´', 'ì½¸', 'ì¾',
+'ì¾', 'ì¾', 'ì¾¡', 'ì¾¨', 'ì¾°', 'ì¿', 'ì¿ ', 'ì¿¡', 'ì¿¤', 'ì¿¨', 'ì¿°',
+'ì¿±', 'ì¿³', 'ì¿µ', 'ì¿¼', 'í', 'í', 'í', 'í', 'í­', 'í´', 'íµ',
+'í¸', 'í¼', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¬',
+'í­', 'í°', 'í´', 'í¼', 'í½', 'í', 'í¤', 'í¥', 'í¨', 'í¬', 'í´',
+'íµ', 'í·', 'í¹', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í ', 'í¤', 'í¬', 'í­', 'í¯', 'í°', 'í±',
+'í¸', 'í', 'í°', 'í±', 'í´', 'í¸', 'íº', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í¡', 'í¨', 'í¬',
+'í¼', 'í', 'í', 'í ', 'í¡', 'í¤', 'í¨', 'í°', 'í±', 'í³', 'íµ',
+'íº', 'í¼', 'í', 'í', 'í´', 'í¸', 'í', 'í', 'í', 'í¬', 'í­',
+'í°', 'í´', 'í¼', 'í½', 'í¿', 'í', 'í', 'í', 'í¤', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¤', 'í¬', 'í±', 'í¸',
+'í¹', 'í¼', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í¤', 'í¥', 'í°', 'í±', 'í´', 'í¸', 'í', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡', 'í¥',
+'í¨', 'í©', 'í¬', 'í°', 'í¸', 'í¹', 'í»', 'í¼', 'í½', 'í', 'í',
+'í¼', 'í½', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í ', 'í¨', 'í©', 'í«', 'í­', 'í´', 'í¸', 'í¼', 'í', 'í',
+'í', 'í', 'í', 'í', 'í¡', 'í£', 'í¬', 'í­', 'í°', 'í´', 'í¼',
+'í½', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¤', 'í­',
+'í¯', 'í¸', 'í¹', 'í¼', 'í¿', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í©', 'í', 'í', 'í', 'í', 'í', 'í¨', 'í¬', 'í°', 'í¸',
+'í»', 'í½', 'í', 'í', 'í', 'í', 'í', 'í', 'í¼', 'í½', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¥', 'í¨',
+'í©', 'í«', 'í­', 'í´', 'íµ', 'í¸', 'í¼', 'í', 'í', 'í', 'í',
+'í', 'í', 'í¥', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í¤', 'í¥', 'í¨', 'í¬', 'í´', 'íµ', 'í·', 'í¹', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¤', 'í­',
+'í¸', 'í¹', 'í¼', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í§', 'í©', 'í°', 'í±', 'í´', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í¡', 'í¨', 'í¬', 'í°', 'í¹', 'í»',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¤', 'í¨',
+'í°', 'íµ', 'í¼', 'í½', 'í', 'í', 'í', 'í', 'í', 'í', 'í ',
+'í¨', 'í©', 'í«', 'í­', 'í´', 'íµ', 'í¸', 'í¼', 'í', 'í', 'í',
+'í', 'í', 'í', 'í', 'í', 'í', 'í', 'í ', 'í¡', 'í£', 'í¥',
+'í©', 'í¬', 'í°', 'í´', 'í¼', 'í½', 'í', 'í', 'í', 'í', 'í',
+'í', 'í', 'í', 'í'] ``` 28. get_all_incompleted_form_hangul_chars This
+returns all incompleted form Hangul characters. Returns: - `List[str]`: all
+incompleted form Hangul characters Examples: ```python >>> from kss import Kss
+>>> get_all_incompleted_form_hangul_chars = Kss
 ("get_all_incompleted_form_hangul_chars") >>> output =
 get_all_incompleted_form_hangul_chars() >>> print(output) ['ê°', 'ê°', 'ê°',
 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°', 'ê°¡', 'ê°¢',
 'ê°£', 'ê°¥', 'ê°¦', 'ê°§', 'ê°¨', 'ê°©', 'ê°ª', 'ê°«', 'ê°®', 'ê°²', 'ê°³',
 'ê°´', 'ê°µ', 'ê°¶', 'ê°·', 'ê°º', 'ê°»', 'ê°½', 'ê°¾', 'ê°¿', 'ê±', 'ê±',
 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±', 'ê±',
@@ -2443,20 +1855,20 @@
 reduce_char_repeats_over (`int`): the maximum number of character that can be
 repeated - reduce_emoticon_repeats_over (`int`): the maximum number of emoticon
 that can be repeated - num_workers (`Union[int, str]`): the number of
 multiprocessing workers Returns: - `Union[str, List[str]]`: normalized text or
 list of normalized texts Examples: ```python >>> from kss import Kss >>>
 normalize = Kss("normalize") >>> text = "ìë\u200bíì¸ì
 ï¾»ï¾»ï¾»ï¾»ï¾»ï¾»
-ì¤ë\u200bì ë ì´ ì°¸ ì¢ë¤ì.\\n\\n\\n200 < 300 & 400" >>> normalize
-(text, allow_doubled_spaces=False, allow_html_tags=False,
-allow_html_escape=False, allow_halfwidth_hangul=False, allow_hangul_jamo=False,
+ì¤ë\u200bì ë ì´ ì°¸ ì¢ë¤ì.\n\n\n200 < 300 & 400" >>> normalize(text,
+allow_doubled_spaces=False, allow_html_tags=False, allow_html_escape=False,
+allow_halfwidth_hangul=False, allow_hangul_jamo=False,
 allow_invisible_chars=False, reduce_char_repeats_over=2,
 reduce_emoticon_repeats_over=2) 'ìëíì¸ì ãã ì¤ëì ë ì´ ì°¸
-ì¢ë¤ì.\\n200 < 300 & 400' ``` 32. preprocess This preprocesses text with
+ì¢ë¤ì.\n200 < 300 & 400' ``` 32. preprocess This preprocesses text with
 various options. This does 1) normalization, 2) filtering out, and 3)
 anonymization in order. Args: - text (`Union[str, List[str], Tuple[str]]`):
 single text or list of texts - normalization_type (`Optional[str]`):
 normalization type - allow_doubled_spaces (`bool`): whether to allow doubled
 spaces or not - allow_html_tags (`bool`): whether to allow HTML tags or not -
 allow_html_escape (`bool`): whether to allow HTML escape or not -
 allow_halfwidth_hangul (`bool`): whether to allow halfwidth Hangul or not -
@@ -2564,17 +1976,17 @@
 convert_numbers_to_hangul_phonemes (`bool`): whether to convert numbers to
 Hangul phonemes or not - num_workers (`Union[int, str]`): the number of
 multiprocessing workers Returns: - `Union[str, List[str]]`: romanized text or
 list of romanized texts Examples: ```python >>> from kss import Kss >>>
 romanize = Kss("romanize") >>> text = "ìëíì¸ì" >>> romanize(text)
 'annyeonghaseyo' >>> text = "ëê´ë ¹" >>> romanize(text) 'daegwallyeong' ```
 References: - This was copied from [korean-romanizer](https://github.com/osori/
-korean-romanizer) and modified by Kss 38. is_unsafe Check if the text is unsafe
-or not. Args: - text (`Union[str, List[str], Tuple[str]]`): single text or list
-of texts - return_matches (`bool`): whether to return matches or not -
+korean-romanizer) and modified by Kss 38. is_unsafe This checks if the text is
+unsafe or not. Args: - text (`Union[str, List[str], Tuple[str]]`): single text
+or list of texts - return_matches (`bool`): whether to return matches or not -
 num_workers (`Union[int, str]`): the number of multiprocessing workers Returns:
 - `Union[bool, List[bool], List[bool], List[List[str]]]`: whether the text is
 unsafe or not or list of whether the texts are unsafe or not or list of matched
 bad words in the texts Examples: ```python >>> from kss import Kss >>>
 is_unsafe = Kss("is_unsafe") >>> text = "ìëíì¸ì" >>> is_unsafe(text)
 False >>> text = "ìëíì¸ì. ì¨ë°" >>> is_unsafe(text) True >>> text =
 ["ìëíì¸ì", "ìëíì¸ì. ì¨ë°"] >>> is_unsafe(text) [False,
```

### Comparing `kss-6.0.0/kss.egg-info/SOURCES.txt` & `kss-6.0.0.dev0/kss.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 kss/_modules/g2p/__init__.py
 kss/_modules/g2p/english.py
 kss/_modules/g2p/g2p.py
 kss/_modules/g2p/numerals.py
 kss/_modules/g2p/regular.py
 kss/_modules/g2p/special.py
 kss/_modules/g2p/utils.py
+kss/_modules/g2p/assets/idioms.txt
 kss/_modules/g2p/assets/rules.txt
 kss/_modules/g2p/assets/table.csv
 kss/_modules/hangulization/__init__.py
 kss/_modules/hangulization/hangulization.py
 kss/_modules/hangulization/hangulize/__init__.py
 kss/_modules/hangulization/hangulize/hangul.py
 kss/_modules/hangulization/hangulize/models.py
```

### Comparing `kss-6.0.0/setup.py` & `kss-6.0.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/tests/test_augmentation.py` & `kss-6.0.0.dev0/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/tests/test_collocation.py` & `kss-6.0.0.dev0/tests/test_collocation.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/tests/test_hanja.py` & `kss-6.0.0.dev0/tests/test_hanja.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/tests/test_jamo.py` & `kss-6.0.0.dev0/tests/test_jamo.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/tests/test_keywords.py` & `kss-6.0.0.dev0/tests/test_keywords.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/tests/test_paradigm.py` & `kss-6.0.0.dev0/tests/test_paradigm.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/tests/test_preprocessing.py` & `kss-6.0.0.dev0/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/tests/test_sentences.py` & `kss-6.0.0.dev0/tests/test_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0/tests/test_summarization.py` & `kss-6.0.0.dev0/tests/test_summarization.py`

 * *Files identical despite different names*

