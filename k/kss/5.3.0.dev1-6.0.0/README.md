# Comparing `tmp/kss-5.3.0.dev1.tar.gz` & `tmp/kss-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kss-5.3.0.dev1.tar", last modified: Sat Apr 27 14:18:21 2024, max compression
+gzip compressed data, was "kss-6.0.0.tar", last modified: Sat Apr 27 14:20:50 2024, max compression
```

## Comparing `kss-5.3.0.dev1.tar` & `kss-6.0.0.tar`

### file list

```diff
@@ -1,235 +1,235 @@
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.105661 kss-5.3.0.dev1/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1569 2024-04-01 04:29:21.000000 kss-5.3.0.dev1/LICENSE
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-26 04:11:11.000000 kss-5.3.0.dev1/MANIFEST.in
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   204755 2024-04-27 14:18:21.105854 kss-5.3.0.dev1/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   203997 2024-04-27 14:03:15.000000 kss-5.3.0.dev1/README.md
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.081315 kss-5.3.0.dev1/bench/
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.086785 kss-5.3.0.dev1/bench/sentence_split/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 04:39:09.000000 kss-5.3.0.dev1/bench/sentence_split/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4379 2023-05-16 17:34:32.000000 kss-5.3.0.dev1/bench/sentence_split/sentence_split.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      615 2023-05-16 17:34:32.000000 kss-5.3.0.dev1/bench/sentence_split/test_baseline.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      600 2023-05-16 17:34:32.000000 kss-5.3.0.dev1/bench/sentence_split/test_kiwi.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1015 2023-05-16 17:34:32.000000 kss-5.3.0.dev1/bench/sentence_split/test_koalanlp.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      700 2024-03-31 14:00:52.000000 kss-5.3.0.dev1/bench/sentence_split/test_kss.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      587 2023-05-16 17:34:32.000000 kss-5.3.0.dev1/bench/sentence_split/test_word_split.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.087172 kss-5.3.0.dev1/csrc/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2024-03-31 20:12:01.000000 kss-5.3.0.dev1/csrc/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      563 2024-03-31 20:36:14.000000 kss-5.3.0.dev1/csrc/kss_cython.pyx
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5965 2024-03-31 20:12:01.000000 kss-5.3.0.dev1/csrc/sentence_splitter.cpp
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7830 2024-03-31 20:12:01.000000 kss-5.3.0.dev1/csrc/sentence_splitter.h
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.087269 kss-5.3.0.dev1/kss/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6883 2024-04-27 14:18:12.000000 kss-5.3.0.dev1/kss/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.088343 kss-5.3.0.dev1/kss/_elements/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_elements/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4888 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_elements/element.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2702 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_elements/empty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      536 2024-04-14 01:15:11.000000 kss-5.3.0.dev1/kss/_elements/subclasses.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.088446 kss-5.3.0.dev1/kss/_modules/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_modules/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.088929 kss-5.3.0.dev1/kss/_modules/augmentation/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:47:16.000000 kss-5.3.0.dev1/kss/_modules/augmentation/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.089037 kss-5.3.0.dev1/kss/_modules/augmentation/assets/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)  4865459 2021-09-26 12:11:43.000000 kss-5.3.0.dev1/kss/_modules/augmentation/assets/wordnet.json
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3892 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/augmentation/augment.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3251 2024-04-23 11:22:09.000000 kss-5.3.0.dev1/kss/_modules/augmentation/distance.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3602 2024-04-27 11:42:40.000000 kss-5.3.0.dev1/kss/_modules/augmentation/replacement.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1411 2024-04-27 11:42:40.000000 kss-5.3.0.dev1/kss/_modules/augmentation/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.091757 kss-5.3.0.dev1/kss/_modules/collocation/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 18:49:12.000000 kss-5.3.0.dev1/kss/_modules/collocation/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9351 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/collocation/collocate.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.092456 kss-5.3.0.dev1/kss/_modules/g2p/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 11:01:28.000000 kss-5.3.0.dev1/kss/_modules/g2p/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.092683 kss-5.3.0.dev1/kss/_modules/g2p/assets/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    14802 2024-04-21 10:45:23.000000 kss-5.3.0.dev1/kss/_modules/g2p/assets/rules.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5390 2024-04-21 10:46:10.000000 kss-5.3.0.dev1/kss/_modules/g2p/assets/table.csv
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6586 2024-04-27 11:42:40.000000 kss-5.3.0.dev1/kss/_modules/g2p/english.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7184 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/g2p/g2p.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4459 2024-04-27 11:42:40.000000 kss-5.3.0.dev1/kss/_modules/g2p/numerals.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2722 2024-04-27 11:42:40.000000 kss-5.3.0.dev1/kss/_modules/g2p/regular.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4949 2024-04-27 11:42:40.000000 kss-5.3.0.dev1/kss/_modules/g2p/special.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8131 2024-04-27 11:42:40.000000 kss-5.3.0.dev1/kss/_modules/g2p/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.092870 kss-5.3.0.dev1/kss/_modules/hangulization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-26 07:28:27.000000 kss-5.3.0.dev1/kss/_modules/hangulization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3616 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulization.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.093391 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     2277 2024-04-27 09:12:39.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/__init__.py
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)    10423 2024-04-27 09:00:03.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/hangul.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.093493 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     1426 2018-08-18 18:42:06.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.093595 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/aze/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5272 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/aze/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.093700 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/bel/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5425 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/bel/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.093798 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/bul/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4925 2018-08-18 18:42:06.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/bul/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.093897 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/cat/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4328 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/cat/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.094000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ces/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4820 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ces/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.094121 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/cym/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5791 2018-08-18 18:42:06.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/cym/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.094231 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/deu/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     7415 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/deu/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.094335 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ell/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     9068 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ell/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.094441 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/epo/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4103 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/epo/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.094547 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/est/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3931 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/est/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.094645 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/fin/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3410 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/fin/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.094752 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/grc/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     8626 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/grc/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.094851 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/hbs/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5606 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.094951 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/hun/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4990 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/hun/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.095054 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/isl/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5626 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/isl/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.095153 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ita/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4371 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ita/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.095265 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/jpn/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4446 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.095466 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/kat/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6118 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/kat/__init__.py
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6408 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/kat/narrow.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.095569 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/lat/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3314 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/lat/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.095667 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/lav/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4116 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/lav/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.095767 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/lit/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4080 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/lit/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.095865 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/mkd/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5354 2018-08-18 18:42:06.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.095982 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/nld/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)    22064 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/nld/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.096119 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/pol/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5785 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/pol/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.096342 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/por/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6048 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/por/__init__.py
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/por/br.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.096450 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ron/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5120 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ron/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.096553 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/rus/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4994 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/rus/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.096653 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/slk/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6693 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/slk/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.096755 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/slv/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3836 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/slv/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.096854 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/spa/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4002 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/spa/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.096957 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/sqi/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3177 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.097053 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/swe/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     7896 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/swe/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.097152 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/tur/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3528 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/tur/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.097247 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ukr/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5072 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.097342 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/vie/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4742 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/vie/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.097440 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/wlm/
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5599 2024-04-27 09:05:48.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)    16108 2024-04-27 09:00:03.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/models.py
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     1069 2018-08-18 18:42:06.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/normalization.py
--rw-rw-r--   0 hyunwoongko   (501) staff       (20)     2897 2024-04-27 08:57:42.000000 kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/processing.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.097708 kss-5.3.0.dev1/kss/_modules/hanja/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:46:48.000000 kss-5.3.0.dev1/kss/_modules/hanja/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4462 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/hanja/_hanja.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2021 2024-04-25 08:27:31.000000 kss-5.3.0.dev1/kss/_modules/hanja/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.097995 kss-5.3.0.dev1/kss/_modules/jamo/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:46:59.000000 kss-5.3.0.dev1/kss/_modules/jamo/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    12624 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/jamo/_jamo.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      912 2024-04-25 08:38:54.000000 kss-5.3.0.dev1/kss/_modules/jamo/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.098260 kss-5.3.0.dev1/kss/_modules/josa/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 07:12:50.000000 kss-5.3.0.dev1/kss/_modules/josa/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2580 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/josa/josa.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7030 2024-04-25 16:33:55.000000 kss-5.3.0.dev1/kss/_modules/josa/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.098530 kss-5.3.0.dev1/kss/_modules/keywords/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 11:01:42.000000 kss-5.3.0.dev1/kss/_modules/keywords/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6362 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/keywords/extract_keywords.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    17289 2024-04-27 12:31:02.000000 kss-5.3.0.dev1/kss/_modules/keywords/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.098937 kss-5.3.0.dev1/kss/_modules/morphemes/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_modules/morphemes/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2652 2024-03-31 13:42:10.000000 kss-5.3.0.dev1/kss/_modules/morphemes/analyzers.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1849 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/morphemes/split_morphemes.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3588 2024-04-23 09:05:15.000000 kss-5.3.0.dev1/kss/_modules/morphemes/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.099130 kss-5.3.0.dev1/kss/_modules/paradigm/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 08:40:05.000000 kss-5.3.0.dev1/kss/_modules/paradigm/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    18316 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/paradigm/paradigm.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.100250 kss-5.3.0.dev1/kss/_modules/preprocessing/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-26 07:58:23.000000 kss-5.3.0.dev1/kss/_modules/preprocessing/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    15532 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/preprocessing/anonymize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    29789 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/preprocessing/clean_news.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    81169 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/preprocessing/completed_form.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    24570 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/preprocessing/filter_out.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2088 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/preprocessing/half2full.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/preprocessing/normalize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    26257 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/preprocessing/preprocess.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7186 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/preprocessing/reduce_repeats.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7661 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/preprocessing/remove_invisible_chars.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.100544 kss-5.3.0.dev1/kss/_modules/qwerty/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 08:21:28.000000 kss-5.3.0.dev1/kss/_modules/qwerty/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6262 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/qwerty/qwerty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5941 2024-04-21 19:55:18.000000 kss-5.3.0.dev1/kss/_modules/qwerty/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.100934 kss-5.3.0.dev1/kss/_modules/romanization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:48:29.000000 kss-5.3.0.dev1/kss/_modules/romanization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5813 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/romanization/romanize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8901 2024-04-21 17:45:54.000000 kss-5.3.0.dev1/kss/_modules/romanization/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.101277 kss-5.3.0.dev1/kss/_modules/safety/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 04:59:07.000000 kss-5.3.0.dev1/kss/_modules/safety/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3525 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/safety/check_safety.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    35374 2024-04-21 06:06:58.000000 kss-5.3.0.dev1/kss/_modules/safety/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.102239 kss-5.3.0.dev1/kss/_modules/sentences/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_modules/sentences/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9334 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_modules/sentences/embracing_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    22898 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_modules/sentences/sentence_postprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6751 2024-03-31 07:55:02.000000 kss-5.3.0.dev1/kss/_modules/sentences/sentence_preprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2298 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_modules/sentences/sentence_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    30242 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_modules/sentences/sentence_splitter.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    13304 2024-03-31 20:36:14.000000 kss-5.3.0.dev1/kss/_modules/sentences/sentence_splitter_fast.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8322 2024-04-27 14:18:12.000000 kss-5.3.0.dev1/kss/_modules/sentences/split_sentences.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.102537 kss-5.3.0.dev1/kss/_modules/spacing/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 14:16:36.000000 kss-5.3.0.dev1/kss/_modules/spacing/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5539 2024-04-27 13:58:40.000000 kss-5.3.0.dev1/kss/_modules/spacing/correct_spacing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   296979 2024-04-27 02:42:16.000000 kss-5.3.0.dev1/kss/_modules/spacing/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.103033 kss-5.3.0.dev1/kss/_modules/summarization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_modules/summarization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5603 2024-04-27 13:55:54.000000 kss-5.3.0.dev1/kss/_modules/summarization/summarize_sentences.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3396 2024-04-26 07:26:56.000000 kss-5.3.0.dev1/kss/_modules/summarization/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.103745 kss-5.3.0.dev1/kss/_utils/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_utils/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       66 2024-04-27 04:09:55.000000 kss-5.3.0.dev1/kss/_utils/api.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    10329 2024-03-31 07:46:03.000000 kss-5.3.0.dev1/kss/_utils/const.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1399 2024-04-21 19:08:53.000000 kss-5.3.0.dev1/kss/_utils/emojis.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      910 2024-04-23 08:15:52.000000 kss-5.3.0.dev1/kss/_utils/logger.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1001 2023-08-22 23:38:03.000000 kss-5.3.0.dev1/kss/_utils/multiprocessing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    17275 2024-04-27 03:50:29.000000 kss-5.3.0.dev1/kss/_utils/sanity_checks.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.087957 kss-5.3.0.dev1/kss.egg-info/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   204755 2024-04-27 14:18:21.000000 kss-5.3.0.dev1/kss.egg-info/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6339 2024-04-27 14:18:21.000000 kss-5.3.0.dev1/kss.egg-info/SOURCES.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:18:21.000000 kss-5.3.0.dev1/kss.egg-info/dependency_links.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:04:55.000000 kss-5.3.0.dev1/kss.egg-info/not-zip-safe
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      136 2024-04-27 14:18:21.000000 kss-5.3.0.dev1/kss.egg-info/requires.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       32 2024-04-27 14:18:21.000000 kss-5.3.0.dev1/kss.egg-info/top_level.txt
--rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2024-04-27 14:18:21.106114 kss-5.3.0.dev1/setup.cfg
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6191 2024-04-27 09:17:01.000000 kss-5.3.0.dev1/setup.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:18:21.105574 kss-5.3.0.dev1/tests/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 02:40:08.000000 kss-5.3.0.dev1/tests/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1033 2024-04-27 09:25:57.000000 kss-5.3.0.dev1/tests/test_augmentation.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8258 2024-04-27 08:00:32.000000 kss-5.3.0.dev1/tests/test_collocation.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      250 2024-04-27 08:00:32.000000 kss-5.3.0.dev1/tests/test_g2p.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      238 2024-04-27 08:00:32.000000 kss-5.3.0.dev1/tests/test_hangulize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      747 2024-04-27 04:21:47.000000 kss-5.3.0.dev1/tests/test_hanja.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      978 2024-04-27 04:13:17.000000 kss-5.3.0.dev1/tests/test_jamo.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      442 2024-04-27 04:17:41.000000 kss-5.3.0.dev1/tests/test_josa.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3405 2024-04-27 04:17:41.000000 kss-5.3.0.dev1/tests/test_keywords.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-27 09:20:57.000000 kss-5.3.0.dev1/tests/test_morphemes.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    19148 2024-04-27 04:25:01.000000 kss-5.3.0.dev1/tests/test_paradigm.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    97981 2024-04-27 13:38:44.000000 kss-5.3.0.dev1/tests/test_preprocessing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      290 2024-04-27 07:33:52.000000 kss-5.3.0.dev1/tests/test_qwerty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      257 2024-04-27 07:39:43.000000 kss-5.3.0.dev1/tests/test_romanize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      313 2024-04-27 08:03:40.000000 kss-5.3.0.dev1/tests/test_safety.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      776 2024-04-27 07:56:55.000000 kss-5.3.0.dev1/tests/test_sentences.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      236 2024-04-27 08:00:32.000000 kss-5.3.0.dev1/tests/test_spacing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1966 2024-04-27 08:00:32.000000 kss-5.3.0.dev1/tests/test_summarization.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.456971 kss-6.0.0/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1569 2024-04-01 04:29:21.000000 kss-6.0.0/LICENSE
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-26 04:11:11.000000 kss-6.0.0/MANIFEST.in
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   204750 2024-04-27 14:20:50.457167 kss-6.0.0/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   203997 2024-04-27 14:03:15.000000 kss-6.0.0/README.md
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.432871 kss-6.0.0/bench/
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.438034 kss-6.0.0/bench/sentence_split/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 04:39:09.000000 kss-6.0.0/bench/sentence_split/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4379 2023-05-16 17:34:32.000000 kss-6.0.0/bench/sentence_split/sentence_split.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      615 2023-05-16 17:34:32.000000 kss-6.0.0/bench/sentence_split/test_baseline.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      600 2023-05-16 17:34:32.000000 kss-6.0.0/bench/sentence_split/test_kiwi.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1015 2023-05-16 17:34:32.000000 kss-6.0.0/bench/sentence_split/test_koalanlp.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      700 2024-03-31 14:00:52.000000 kss-6.0.0/bench/sentence_split/test_kss.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      587 2023-05-16 17:34:32.000000 kss-6.0.0/bench/sentence_split/test_word_split.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.438611 kss-6.0.0/csrc/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2024-03-31 20:12:01.000000 kss-6.0.0/csrc/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      563 2024-03-31 20:36:14.000000 kss-6.0.0/csrc/kss_cython.pyx
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5965 2024-03-31 20:12:01.000000 kss-6.0.0/csrc/sentence_splitter.cpp
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7830 2024-03-31 20:12:01.000000 kss-6.0.0/csrc/sentence_splitter.h
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.438706 kss-6.0.0/kss/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6879 2024-04-27 14:20:34.000000 kss-6.0.0/kss/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.439775 kss-6.0.0/kss/_elements/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_elements/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4888 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_elements/element.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2702 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_elements/empty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      536 2024-04-14 01:15:11.000000 kss-6.0.0/kss/_elements/subclasses.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.439874 kss-6.0.0/kss/_modules/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.440428 kss-6.0.0/kss/_modules/augmentation/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:47:16.000000 kss-6.0.0/kss/_modules/augmentation/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.440551 kss-6.0.0/kss/_modules/augmentation/assets/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)  4865459 2021-09-26 12:11:43.000000 kss-6.0.0/kss/_modules/augmentation/assets/wordnet.json
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3892 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/augmentation/augment.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3251 2024-04-23 11:22:09.000000 kss-6.0.0/kss/_modules/augmentation/distance.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3602 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/augmentation/replacement.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1411 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/augmentation/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.443519 kss-6.0.0/kss/_modules/collocation/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 18:49:12.000000 kss-6.0.0/kss/_modules/collocation/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9351 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/collocation/collocate.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.444218 kss-6.0.0/kss/_modules/g2p/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 11:01:28.000000 kss-6.0.0/kss/_modules/g2p/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.444424 kss-6.0.0/kss/_modules/g2p/assets/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    14802 2024-04-21 10:45:23.000000 kss-6.0.0/kss/_modules/g2p/assets/rules.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5390 2024-04-21 10:46:10.000000 kss-6.0.0/kss/_modules/g2p/assets/table.csv
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6586 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/g2p/english.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7184 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/g2p/g2p.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4459 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/g2p/numerals.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2722 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/g2p/regular.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4949 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/g2p/special.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8131 2024-04-27 11:42:40.000000 kss-6.0.0/kss/_modules/g2p/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.444601 kss-6.0.0/kss/_modules/hangulization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-26 07:28:27.000000 kss-6.0.0/kss/_modules/hangulization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3616 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/hangulization/hangulization.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445130 kss-6.0.0/kss/_modules/hangulization/hangulize/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     2277 2024-04-27 09:12:39.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/__init__.py
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)    10423 2024-04-27 09:00:03.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/hangul.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445232 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     1426 2018-08-18 18:42:06.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445328 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/aze/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5272 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/aze/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445429 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/bel/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5425 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/bel/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445526 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/bul/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4925 2018-08-18 18:42:06.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/bul/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445636 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/cat/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4328 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/cat/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445745 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ces/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4820 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ces/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445848 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/cym/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5791 2018-08-18 18:42:06.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/cym/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.445951 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/deu/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     7415 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/deu/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446068 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ell/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     9068 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ell/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446176 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/epo/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4103 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/epo/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446285 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/est/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3931 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/est/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446394 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/fin/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3410 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/fin/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446509 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/grc/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     8626 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/grc/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446628 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/hbs/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5606 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446736 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/hun/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4990 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/hun/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446840 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/isl/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5626 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/isl/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.446943 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ita/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4371 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ita/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447047 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/jpn/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4446 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447255 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/kat/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6118 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/kat/__init__.py
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6408 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/kat/narrow.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447352 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lat/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3314 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lat/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447464 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lav/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4116 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lav/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447560 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lit/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4080 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lit/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447665 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/mkd/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5354 2018-08-18 18:42:06.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447764 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/nld/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)    22064 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/nld/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.447880 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/pol/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5785 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/pol/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448080 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/por/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6048 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/por/__init__.py
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/por/br.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448184 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ron/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5120 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ron/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448280 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/rus/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4994 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/rus/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448379 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/slk/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     6693 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/slk/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448475 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/slv/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3836 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/slv/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448578 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/spa/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4002 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/spa/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448672 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/sqi/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3177 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448769 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/swe/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     7896 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/swe/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448864 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/tur/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     3528 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/tur/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.448961 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ukr/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5072 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.449066 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/vie/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     4742 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/vie/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.449161 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/wlm/
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     5599 2024-04-27 09:05:48.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)    16108 2024-04-27 09:00:03.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/models.py
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     1069 2018-08-18 18:42:06.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/normalization.py
+-rw-rw-r--   0 hyunwoongko   (501) staff       (20)     2897 2024-04-27 08:57:42.000000 kss-6.0.0/kss/_modules/hangulization/hangulize/processing.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.449429 kss-6.0.0/kss/_modules/hanja/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:46:48.000000 kss-6.0.0/kss/_modules/hanja/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4462 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/hanja/_hanja.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2021 2024-04-25 08:27:31.000000 kss-6.0.0/kss/_modules/hanja/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.449694 kss-6.0.0/kss/_modules/jamo/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:46:59.000000 kss-6.0.0/kss/_modules/jamo/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    12624 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/jamo/_jamo.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      912 2024-04-25 08:38:54.000000 kss-6.0.0/kss/_modules/jamo/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.449969 kss-6.0.0/kss/_modules/josa/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 07:12:50.000000 kss-6.0.0/kss/_modules/josa/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2580 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/josa/josa.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7030 2024-04-25 16:33:55.000000 kss-6.0.0/kss/_modules/josa/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.450239 kss-6.0.0/kss/_modules/keywords/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 11:01:42.000000 kss-6.0.0/kss/_modules/keywords/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6362 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/keywords/extract_keywords.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    17289 2024-04-27 12:31:02.000000 kss-6.0.0/kss/_modules/keywords/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.450647 kss-6.0.0/kss/_modules/morphemes/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/morphemes/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2652 2024-03-31 13:42:10.000000 kss-6.0.0/kss/_modules/morphemes/analyzers.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1849 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/morphemes/split_morphemes.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3588 2024-04-23 09:05:15.000000 kss-6.0.0/kss/_modules/morphemes/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.450821 kss-6.0.0/kss/_modules/paradigm/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 08:40:05.000000 kss-6.0.0/kss/_modules/paradigm/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    18316 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/paradigm/paradigm.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.451926 kss-6.0.0/kss/_modules/preprocessing/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-26 07:58:23.000000 kss-6.0.0/kss/_modules/preprocessing/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    15532 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/anonymize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    29789 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/clean_news.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    81169 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/completed_form.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    24570 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/filter_out.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2088 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/half2full.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/normalize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    26257 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/preprocess.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7186 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/reduce_repeats.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7661 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/preprocessing/remove_invisible_chars.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.452201 kss-6.0.0/kss/_modules/qwerty/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 08:21:28.000000 kss-6.0.0/kss/_modules/qwerty/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6262 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/qwerty/qwerty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5941 2024-04-21 19:55:18.000000 kss-6.0.0/kss/_modules/qwerty/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.452475 kss-6.0.0/kss/_modules/romanization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 10:48:29.000000 kss-6.0.0/kss/_modules/romanization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5813 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/romanization/romanize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8901 2024-04-21 17:45:54.000000 kss-6.0.0/kss/_modules/romanization/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.452757 kss-6.0.0/kss/_modules/safety/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-21 04:59:07.000000 kss-6.0.0/kss/_modules/safety/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3525 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/safety/check_safety.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    35374 2024-04-21 06:06:58.000000 kss-6.0.0/kss/_modules/safety/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.453649 kss-6.0.0/kss/_modules/sentences/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/sentences/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9334 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/sentences/embracing_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    22898 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/sentences/sentence_postprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6751 2024-03-31 07:55:02.000000 kss-6.0.0/kss/_modules/sentences/sentence_preprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2298 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/sentences/sentence_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    30242 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/sentences/sentence_splitter.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    13304 2024-03-31 20:36:14.000000 kss-6.0.0/kss/_modules/sentences/sentence_splitter_fast.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8322 2024-04-27 14:18:12.000000 kss-6.0.0/kss/_modules/sentences/split_sentences.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.453928 kss-6.0.0/kss/_modules/spacing/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-19 14:16:36.000000 kss-6.0.0/kss/_modules/spacing/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5539 2024-04-27 13:58:40.000000 kss-6.0.0/kss/_modules/spacing/correct_spacing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   296979 2024-04-27 02:42:16.000000 kss-6.0.0/kss/_modules/spacing/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.454394 kss-6.0.0/kss/_modules/summarization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_modules/summarization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5603 2024-04-27 13:55:54.000000 kss-6.0.0/kss/_modules/summarization/summarize_sentences.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3396 2024-04-26 07:26:56.000000 kss-6.0.0/kss/_modules/summarization/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.455070 kss-6.0.0/kss/_utils/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_utils/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       66 2024-04-27 04:09:55.000000 kss-6.0.0/kss/_utils/api.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    10329 2024-03-31 07:46:03.000000 kss-6.0.0/kss/_utils/const.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1399 2024-04-21 19:08:53.000000 kss-6.0.0/kss/_utils/emojis.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      910 2024-04-23 08:15:52.000000 kss-6.0.0/kss/_utils/logger.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1001 2023-08-22 23:38:03.000000 kss-6.0.0/kss/_utils/multiprocessing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    17275 2024-04-27 03:50:29.000000 kss-6.0.0/kss/_utils/sanity_checks.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.439392 kss-6.0.0/kss.egg-info/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   204750 2024-04-27 14:20:50.000000 kss-6.0.0/kss.egg-info/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6339 2024-04-27 14:20:50.000000 kss-6.0.0/kss.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:20:50.000000 kss-6.0.0/kss.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:04:55.000000 kss-6.0.0/kss.egg-info/not-zip-safe
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      136 2024-04-27 14:20:50.000000 kss-6.0.0/kss.egg-info/requires.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       32 2024-04-27 14:20:50.000000 kss-6.0.0/kss.egg-info/top_level.txt
+-rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2024-04-27 14:20:50.457410 kss-6.0.0/setup.cfg
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6191 2024-04-27 09:17:01.000000 kss-6.0.0/setup.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:20:50.456879 kss-6.0.0/tests/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 02:40:08.000000 kss-6.0.0/tests/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1033 2024-04-27 09:25:57.000000 kss-6.0.0/tests/test_augmentation.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8258 2024-04-27 08:00:32.000000 kss-6.0.0/tests/test_collocation.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      250 2024-04-27 08:00:32.000000 kss-6.0.0/tests/test_g2p.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      238 2024-04-27 08:00:32.000000 kss-6.0.0/tests/test_hangulize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      747 2024-04-27 04:21:47.000000 kss-6.0.0/tests/test_hanja.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      978 2024-04-27 04:13:17.000000 kss-6.0.0/tests/test_jamo.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      442 2024-04-27 04:17:41.000000 kss-6.0.0/tests/test_josa.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3405 2024-04-27 04:17:41.000000 kss-6.0.0/tests/test_keywords.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-27 09:20:57.000000 kss-6.0.0/tests/test_morphemes.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    19148 2024-04-27 04:25:01.000000 kss-6.0.0/tests/test_paradigm.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    97981 2024-04-27 13:38:44.000000 kss-6.0.0/tests/test_preprocessing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      290 2024-04-27 07:33:52.000000 kss-6.0.0/tests/test_qwerty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      257 2024-04-27 07:39:43.000000 kss-6.0.0/tests/test_romanize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      313 2024-04-27 08:03:40.000000 kss-6.0.0/tests/test_safety.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      776 2024-04-27 07:56:55.000000 kss-6.0.0/tests/test_sentences.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      236 2024-04-27 08:00:32.000000 kss-6.0.0/tests/test_spacing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1966 2024-04-27 08:00:32.000000 kss-6.0.0/tests/test_summarization.py
```

### Comparing `kss-5.3.0.dev1/LICENSE` & `kss-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/PKG-INFO` & `kss-6.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kss
-Version: 5.3.0.dev1
+Version: 6.0.0
 Summary: A Toolkit for Korean sentence segmentation
 Home-page: https://github.com/hyunwoongko/kss
 Author: Hyunwoong Ko
 Author-email: kevin.brain@kakaobrain.com
 License: BSD 3-Clause "New" or "Revised" License
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: kss Version: 5.3.0.dev1 Summary: A Toolkit for
-Korean sentence segmentation Home-page: https://github.com/hyunwoongko/kss
-Author: Hyunwoong Ko Author-email: kevin.brain@kakaobrain.com License: BSD 3-
-Clause "New" or "Revised" License Platform: any Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
-Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
-LICENSE
+Metadata-Version: 2.1 Name: kss Version: 6.0.0 Summary: A Toolkit for Korean
+sentence segmentation Home-page: https://github.com/hyunwoongko/kss Author:
+Hyunwoong Ko Author-email: kevin.brain@kakaobrain.com License: BSD 3-Clause
+"New" or "Revised" License Platform: any Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.2 Classifier:
+Programming Language :: Python :: 3.3 Classifier: Programming Language ::
+Python :: 3.4 Classifier: Programming Language :: Python :: 3.5 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Requires-
+Python: >=3 Description-Content-Type: text/markdown License-File: LICENSE
                ************ KKSSSS:: KKoorreeaann SSttrriinngg pprroocceessssiinngg SSuuiittee ************
   _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_I_s_s_u_e_s_]_[_T_e_s_t_s_ _o_n_ _U_b_u_n_t_u_]_[_T_e_s_t_s_ _o_n_ _M_a_c_O_S_]_[_T_e_s_t_s_ _o_n_ _W_i_n_d_o_w_s_]
 KSS is a Korean string processing suite that provides various functions for
 processing Korean strings. It is designed to be simple and easy to use, and it
 is designed to be used in various fields such as natural language processing,
 data preprocessing, and data analysis. ### What's New: - April 27, 2024
 [Released Kss 6.0 Python](https://github.com/hyunwoongko/kss/releases/tag/
```

### Comparing `kss-5.3.0.dev1/README.md` & `kss-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/bench/sentence_split/sentence_split.py` & `kss-6.0.0/bench/sentence_split/sentence_split.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/bench/sentence_split/test_baseline.py` & `kss-6.0.0/bench/sentence_split/test_baseline.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/bench/sentence_split/test_kiwi.py` & `kss-6.0.0/bench/sentence_split/test_kiwi.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/bench/sentence_split/test_koalanlp.py` & `kss-6.0.0/bench/sentence_split/test_koalanlp.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/bench/sentence_split/test_kss.py` & `kss-6.0.0/bench/sentence_split/test_kss.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/bench/sentence_split/test_word_split.py` & `kss-6.0.0/bench/sentence_split/test_word_split.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/csrc/kss_cython.pyx` & `kss-6.0.0/csrc/kss_cython.pyx`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/csrc/sentence_splitter.cpp` & `kss-6.0.0/csrc/sentence_splitter.cpp`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/csrc/sentence_splitter.h` & `kss-6.0.0/csrc/sentence_splitter.h`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/__init__.py` & `kss-6.0.0/kss/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,8 +177,8 @@
         if closest_module is None:
             return None
         else:
             return closest_module
 
 
 __ALL__ = list(supported_modules.keys()) + ["Kss"]
-__version__ = "5.3.0dev1"
+__version__ = "6.0.0"
```

### Comparing `kss-5.3.0.dev1/kss/_elements/element.py` & `kss-6.0.0/kss/_elements/element.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_elements/empty.py` & `kss-6.0.0/kss/_elements/empty.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_elements/subclasses.py` & `kss-6.0.0/kss/_elements/subclasses.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/augmentation/assets/wordnet.json` & `kss-6.0.0/kss/_modules/augmentation/assets/wordnet.json`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/augmentation/augment.py` & `kss-6.0.0/kss/_modules/augmentation/augment.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/augmentation/distance.py` & `kss-6.0.0/kss/_modules/augmentation/distance.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/augmentation/replacement.py` & `kss-6.0.0/kss/_modules/augmentation/replacement.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/augmentation/utils.py` & `kss-6.0.0/kss/_modules/augmentation/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/collocation/collocate.py` & `kss-6.0.0/kss/_modules/collocation/collocate.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/g2p/assets/rules.txt` & `kss-6.0.0/kss/_modules/g2p/assets/rules.txt`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/g2p/assets/table.csv` & `kss-6.0.0/kss/_modules/g2p/assets/table.csv`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/g2p/english.py` & `kss-6.0.0/kss/_modules/g2p/english.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/g2p/g2p.py` & `kss-6.0.0/kss/_modules/g2p/g2p.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/g2p/numerals.py` & `kss-6.0.0/kss/_modules/g2p/numerals.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/g2p/regular.py` & `kss-6.0.0/kss/_modules/g2p/regular.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/g2p/special.py` & `kss-6.0.0/kss/_modules/g2p/special.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/g2p/utils.py` & `kss-6.0.0/kss/_modules/g2p/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulization.py` & `kss-6.0.0/kss/_modules/hangulization/hangulization.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/hangul.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/hangul.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/aze/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/aze/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/bel/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/bel/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/bul/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/bul/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/cat/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/cat/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ces/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ces/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/cym/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/cym/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/deu/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/deu/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ell/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ell/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/epo/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/epo/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/est/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/est/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/fin/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/fin/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/grc/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/grc/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/hun/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/hun/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/isl/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/isl/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ita/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ita/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/kat/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/kat/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/kat/narrow.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/kat/narrow.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/lat/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lat/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/lav/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lav/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/lit/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/lit/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/nld/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/nld/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/pol/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/pol/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/por/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/por/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/por/br.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/por/br.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ron/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ron/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/rus/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/rus/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/slk/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/slk/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/slv/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/slv/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/spa/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/spa/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/swe/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/swe/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/tur/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/tur/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/vie/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/vie/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/models.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/models.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/normalization.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/normalization.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hangulization/hangulize/processing.py` & `kss-6.0.0/kss/_modules/hangulization/hangulize/processing.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hanja/_hanja.py` & `kss-6.0.0/kss/_modules/hanja/_hanja.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/hanja/utils.py` & `kss-6.0.0/kss/_modules/hanja/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/jamo/_jamo.py` & `kss-6.0.0/kss/_modules/jamo/_jamo.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/jamo/utils.py` & `kss-6.0.0/kss/_modules/jamo/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/josa/josa.py` & `kss-6.0.0/kss/_modules/josa/josa.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/josa/utils.py` & `kss-6.0.0/kss/_modules/josa/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/keywords/extract_keywords.py` & `kss-6.0.0/kss/_modules/keywords/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/keywords/utils.py` & `kss-6.0.0/kss/_modules/keywords/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/morphemes/analyzers.py` & `kss-6.0.0/kss/_modules/morphemes/analyzers.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/morphemes/split_morphemes.py` & `kss-6.0.0/kss/_modules/morphemes/split_morphemes.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/morphemes/utils.py` & `kss-6.0.0/kss/_modules/morphemes/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/paradigm/paradigm.py` & `kss-6.0.0/kss/_modules/paradigm/paradigm.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/preprocessing/anonymize.py` & `kss-6.0.0/kss/_modules/preprocessing/anonymize.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/preprocessing/clean_news.py` & `kss-6.0.0/kss/_modules/preprocessing/clean_news.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/preprocessing/completed_form.py` & `kss-6.0.0/kss/_modules/preprocessing/completed_form.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/preprocessing/filter_out.py` & `kss-6.0.0/kss/_modules/preprocessing/filter_out.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/preprocessing/half2full.py` & `kss-6.0.0/kss/_modules/preprocessing/half2full.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/preprocessing/normalize.py` & `kss-6.0.0/kss/_modules/preprocessing/normalize.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/preprocessing/preprocess.py` & `kss-6.0.0/kss/_modules/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/preprocessing/reduce_repeats.py` & `kss-6.0.0/kss/_modules/preprocessing/reduce_repeats.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/preprocessing/remove_invisible_chars.py` & `kss-6.0.0/kss/_modules/preprocessing/remove_invisible_chars.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/qwerty/qwerty.py` & `kss-6.0.0/kss/_modules/qwerty/qwerty.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/qwerty/utils.py` & `kss-6.0.0/kss/_modules/qwerty/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/romanization/romanize.py` & `kss-6.0.0/kss/_modules/romanization/romanize.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/romanization/utils.py` & `kss-6.0.0/kss/_modules/romanization/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/safety/check_safety.py` & `kss-6.0.0/kss/_modules/safety/check_safety.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/safety/utils.py` & `kss-6.0.0/kss/_modules/safety/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/sentences/embracing_processor.py` & `kss-6.0.0/kss/_modules/sentences/embracing_processor.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/sentences/sentence_postprocessor.py` & `kss-6.0.0/kss/_modules/sentences/sentence_postprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/sentences/sentence_preprocessor.py` & `kss-6.0.0/kss/_modules/sentences/sentence_preprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/sentences/sentence_processor.py` & `kss-6.0.0/kss/_modules/sentences/sentence_processor.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/sentences/sentence_splitter.py` & `kss-6.0.0/kss/_modules/sentences/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/sentences/sentence_splitter_fast.py` & `kss-6.0.0/kss/_modules/sentences/sentence_splitter_fast.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/sentences/split_sentences.py` & `kss-6.0.0/kss/_modules/sentences/split_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/spacing/correct_spacing.py` & `kss-6.0.0/kss/_modules/spacing/correct_spacing.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/spacing/utils.py` & `kss-6.0.0/kss/_modules/spacing/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/summarization/summarize_sentences.py` & `kss-6.0.0/kss/_modules/summarization/summarize_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_modules/summarization/utils.py` & `kss-6.0.0/kss/_modules/summarization/utils.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_utils/const.py` & `kss-6.0.0/kss/_utils/const.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_utils/emojis.py` & `kss-6.0.0/kss/_utils/emojis.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_utils/logger.py` & `kss-6.0.0/kss/_utils/logger.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_utils/multiprocessing.py` & `kss-6.0.0/kss/_utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss/_utils/sanity_checks.py` & `kss-6.0.0/kss/_utils/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/kss.egg-info/PKG-INFO` & `kss-6.0.0/kss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kss
-Version: 5.3.0.dev1
+Version: 6.0.0
 Summary: A Toolkit for Korean sentence segmentation
 Home-page: https://github.com/hyunwoongko/kss
 Author: Hyunwoong Ko
 Author-email: kevin.brain@kakaobrain.com
 License: BSD 3-Clause "New" or "Revised" License
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: kss Version: 5.3.0.dev1 Summary: A Toolkit for
-Korean sentence segmentation Home-page: https://github.com/hyunwoongko/kss
-Author: Hyunwoong Ko Author-email: kevin.brain@kakaobrain.com License: BSD 3-
-Clause "New" or "Revised" License Platform: any Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
-Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
-LICENSE
+Metadata-Version: 2.1 Name: kss Version: 6.0.0 Summary: A Toolkit for Korean
+sentence segmentation Home-page: https://github.com/hyunwoongko/kss Author:
+Hyunwoong Ko Author-email: kevin.brain@kakaobrain.com License: BSD 3-Clause
+"New" or "Revised" License Platform: any Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.2 Classifier:
+Programming Language :: Python :: 3.3 Classifier: Programming Language ::
+Python :: 3.4 Classifier: Programming Language :: Python :: 3.5 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Requires-
+Python: >=3 Description-Content-Type: text/markdown License-File: LICENSE
                ************ KKSSSS:: KKoorreeaann SSttrriinngg pprroocceessssiinngg SSuuiittee ************
   _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_I_s_s_u_e_s_]_[_T_e_s_t_s_ _o_n_ _U_b_u_n_t_u_]_[_T_e_s_t_s_ _o_n_ _M_a_c_O_S_]_[_T_e_s_t_s_ _o_n_ _W_i_n_d_o_w_s_]
 KSS is a Korean string processing suite that provides various functions for
 processing Korean strings. It is designed to be simple and easy to use, and it
 is designed to be used in various fields such as natural language processing,
 data preprocessing, and data analysis. ### What's New: - April 27, 2024
 [Released Kss 6.0 Python](https://github.com/hyunwoongko/kss/releases/tag/
```

### Comparing `kss-5.3.0.dev1/kss.egg-info/SOURCES.txt` & `kss-6.0.0/kss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/setup.py` & `kss-6.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/tests/test_augmentation.py` & `kss-6.0.0/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/tests/test_collocation.py` & `kss-6.0.0/tests/test_collocation.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/tests/test_hanja.py` & `kss-6.0.0/tests/test_hanja.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/tests/test_jamo.py` & `kss-6.0.0/tests/test_jamo.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/tests/test_keywords.py` & `kss-6.0.0/tests/test_keywords.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/tests/test_paradigm.py` & `kss-6.0.0/tests/test_paradigm.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/tests/test_preprocessing.py` & `kss-6.0.0/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/tests/test_sentences.py` & `kss-6.0.0/tests/test_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-5.3.0.dev1/tests/test_summarization.py` & `kss-6.0.0/tests/test_summarization.py`

 * *Files identical despite different names*

