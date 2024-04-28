# Comparing `tmp/kss-6.0.0.dev0.tar.gz` & `tmp/kss-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kss-6.0.0.dev0.tar", last modified: Sun Apr 28 13:41:19 2024, max compression
+gzip compressed data, was "kss-6.0.1.tar", last modified: Sun Apr 28 13:42:58 2024, max compression
```

## Comparing `kss-6.0.0.dev0.tar` & `kss-6.0.1.tar`

### file list

```diff
@@ -1,236 +1,236 @@
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.550542 kss-6.0.0.dev0/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1569 2024-04-01 04:29:21.000000 kss-6.0.0.dev0/LICENSE
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      379 2024-04-28 13:40:34.000000 kss-6.0.0.dev0/MANIFEST.in
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   159355 2024-04-28 13:41:19.550707 kss-6.0.0.dev0/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   158598 2024-04-27 15:21:43.000000 kss-6.0.0.dev0/README.md
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.526052 kss-6.0.0.dev0/bench/
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.530930 kss-6.0.0.dev0/bench/sentence_split/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4379 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/sentence_split.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      615 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/test_baseline.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      600 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/test_kiwi.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1015 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/test_koalanlp.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      700 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/test_kss.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      587 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/bench/sentence_split/test_word_split.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.531329 kss-6.0.0.dev0/csrc/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2024-03-31 20:12:01.000000 kss-6.0.0.dev0/csrc/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      563 2024-03-31 20:36:14.000000 kss-6.0.0.dev0/csrc/kss_cython.pyx
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5965 2024-03-31 20:12:01.000000 kss-6.0.0.dev0/csrc/sentence_splitter.cpp
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7830 2024-03-31 20:12:01.000000 kss-6.0.0.dev0/csrc/sentence_splitter.h
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.531426 kss-6.0.0.dev0/kss/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6884 2024-04-28 13:41:15.000000 kss-6.0.0.dev0/kss/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.532462 kss-6.0.0.dev0/kss/_elements/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_elements/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4888 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_elements/element.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2702 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_elements/empty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      536 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_elements/subclasses.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.532558 kss-6.0.0.dev0/kss/_modules/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.533024 kss-6.0.0.dev0/kss/_modules/augmentation/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/augmentation/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.533134 kss-6.0.0.dev0/kss/_modules/augmentation/assets/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)  4865459 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/augmentation/assets/wordnet.json
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3892 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/augmentation/augment.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3251 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/augmentation/distance.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3602 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/augmentation/replacement.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1411 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/augmentation/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.535905 kss-6.0.0.dev0/kss/_modules/collocation/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/collocation/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9351 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/collocation/collocate.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.537083 kss-6.0.0.dev0/kss/_modules/g2p/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.537396 kss-6.0.0.dev0/kss/_modules/g2p/assets/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2634 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/assets/idioms.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    14802 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/assets/rules.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5390 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/assets/table.csv
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6586 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/english.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7184 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/g2p.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4459 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/numerals.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2722 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/regular.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4949 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/special.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8131 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/g2p/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.537576 kss-6.0.0.dev0/kss/_modules/hangulization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3616 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulization.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538120 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2277 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    10423 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/hangul.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538231 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1426 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538335 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/aze/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5272 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/aze/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538437 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/bel/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5425 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/bel/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538563 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/bul/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4925 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/bul/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538674 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/cat/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4328 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/cat/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538784 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ces/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4820 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ces/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538886 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/cym/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5791 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/cym/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.538998 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/deu/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7415 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/deu/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539159 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ell/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9068 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ell/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539265 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/epo/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4103 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/epo/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539370 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/est/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3931 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/est/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539465 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/fin/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3410 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/fin/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539564 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/grc/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8626 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/grc/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539664 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/hbs/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5606 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539768 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/hun/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4990 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/hun/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539868 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/isl/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5626 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/isl/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.539965 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ita/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4371 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ita/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540064 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/jpn/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4446 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540264 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6118 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6408 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/narrow.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540369 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lat/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3314 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lat/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540485 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lav/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4116 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lav/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540581 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lit/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4080 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lit/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540680 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/mkd/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5354 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540780 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/nld/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    22064 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/nld/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.540925 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/pol/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5785 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/pol/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541148 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/por/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6048 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/por/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/por/br.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541251 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ron/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5120 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ron/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541350 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/rus/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4994 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/rus/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541472 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/slk/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6693 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/slk/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541610 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/slv/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3836 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/slv/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541745 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/spa/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4002 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/spa/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541844 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/sqi/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3177 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.541953 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/swe/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7896 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/swe/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.542078 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/tur/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3528 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/tur/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.542176 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ukr/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5072 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.542293 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/vie/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4742 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/vie/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.542412 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/wlm/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5599 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    16108 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/models.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1069 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/normalization.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2897 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/processing.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.542705 kss-6.0.0.dev0/kss/_modules/hanja/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hanja/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4462 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hanja/_hanja.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2021 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/hanja/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.542998 kss-6.0.0.dev0/kss/_modules/jamo/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/jamo/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    12624 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/jamo/_jamo.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      912 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/jamo/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.543280 kss-6.0.0.dev0/kss/_modules/josa/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/josa/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2580 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/josa/josa.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7030 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/josa/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.543584 kss-6.0.0.dev0/kss/_modules/keywords/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/keywords/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6362 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/keywords/extract_keywords.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    17289 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/keywords/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.544046 kss-6.0.0.dev0/kss/_modules/morphemes/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/morphemes/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2652 2024-03-31 13:42:10.000000 kss-6.0.0.dev0/kss/_modules/morphemes/analyzers.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1849 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/morphemes/split_morphemes.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3588 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/morphemes/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.544245 kss-6.0.0.dev0/kss/_modules/paradigm/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/paradigm/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    18316 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/paradigm/paradigm.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.545329 kss-6.0.0.dev0/kss/_modules/preprocessing/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    15538 2024-04-27 14:56:06.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/anonymize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    29795 2024-04-27 14:58:49.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/clean_news.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    81165 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/completed_form.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    24570 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/filter_out.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2088 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/half2full.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/normalize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    26257 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/preprocess.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7186 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/reduce_repeats.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7661 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/preprocessing/remove_invisible_chars.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.545623 kss-6.0.0.dev0/kss/_modules/qwerty/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/qwerty/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6262 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/qwerty/qwerty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5941 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/qwerty/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.545923 kss-6.0.0.dev0/kss/_modules/romanization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/romanization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5813 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/romanization/romanize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8901 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/romanization/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.546214 kss-6.0.0.dev0/kss/_modules/safety/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/safety/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3531 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/safety/check_safety.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    35374 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/safety/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.547078 kss-6.0.0.dev0/kss/_modules/sentences/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/sentences/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9334 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/sentences/embracing_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    22898 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/sentences/sentence_postprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6751 2024-03-31 07:55:02.000000 kss-6.0.0.dev0/kss/_modules/sentences/sentence_preprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2298 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/sentences/sentence_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    30242 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/sentences/sentence_splitter.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    13304 2024-03-31 20:36:14.000000 kss-6.0.0.dev0/kss/_modules/sentences/sentence_splitter_fast.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8322 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/sentences/split_sentences.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.547353 kss-6.0.0.dev0/kss/_modules/spacing/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/spacing/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5539 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/spacing/correct_spacing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   296979 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/spacing/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.547822 kss-6.0.0.dev0/kss/_modules/summarization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_modules/summarization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5603 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/summarization/summarize_sentences.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3396 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_modules/summarization/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.548513 kss-6.0.0.dev0/kss/_utils/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_utils/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       66 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_utils/api.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    10329 2024-03-31 07:46:03.000000 kss-6.0.0.dev0/kss/_utils/const.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1399 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_utils/emojis.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      910 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_utils/logger.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1001 2023-08-22 23:38:03.000000 kss-6.0.0.dev0/kss/_utils/multiprocessing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    17275 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/kss/_utils/sanity_checks.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.532072 kss-6.0.0.dev0/kss.egg-info/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   159355 2024-04-28 13:41:19.000000 kss-6.0.0.dev0/kss.egg-info/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6374 2024-04-28 13:41:19.000000 kss-6.0.0.dev0/kss.egg-info/SOURCES.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-28 13:41:19.000000 kss-6.0.0.dev0/kss.egg-info/dependency_links.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:04:55.000000 kss-6.0.0.dev0/kss.egg-info/not-zip-safe
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      136 2024-04-28 13:41:19.000000 kss-6.0.0.dev0/kss.egg-info/requires.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       32 2024-04-28 13:41:19.000000 kss-6.0.0.dev0/kss.egg-info/top_level.txt
--rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2024-04-28 13:41:19.550940 kss-6.0.0.dev0/setup.cfg
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6191 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/setup.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:41:19.550448 kss-6.0.0.dev0/tests/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1033 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_augmentation.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8258 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_collocation.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      250 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_g2p.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      238 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_hangulize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      747 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_hanja.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      978 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_jamo.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      442 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_josa.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3405 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_keywords.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_morphemes.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    19148 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_paradigm.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    97981 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_preprocessing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      290 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_qwerty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      257 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_romanize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      313 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_safety.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      776 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_sentences.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      236 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_spacing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1966 2024-04-27 14:55:22.000000 kss-6.0.0.dev0/tests/test_summarization.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.880717 kss-6.0.1/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1569 2024-04-01 04:29:21.000000 kss-6.0.1/LICENSE
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      379 2024-04-28 13:40:34.000000 kss-6.0.1/MANIFEST.in
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   159350 2024-04-28 13:42:58.880903 kss-6.0.1/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   158598 2024-04-27 15:21:43.000000 kss-6.0.1/README.md
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.854333 kss-6.0.1/bench/
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.859932 kss-6.0.1/bench/sentence_split/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/bench/sentence_split/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4379 2024-04-27 14:55:22.000000 kss-6.0.1/bench/sentence_split/sentence_split.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      615 2024-04-27 14:55:22.000000 kss-6.0.1/bench/sentence_split/test_baseline.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      600 2024-04-27 14:55:22.000000 kss-6.0.1/bench/sentence_split/test_kiwi.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1015 2024-04-27 14:55:22.000000 kss-6.0.1/bench/sentence_split/test_koalanlp.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      700 2024-04-27 14:55:22.000000 kss-6.0.1/bench/sentence_split/test_kss.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      587 2024-04-27 14:55:22.000000 kss-6.0.1/bench/sentence_split/test_word_split.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.860374 kss-6.0.1/csrc/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2024-03-31 20:12:01.000000 kss-6.0.1/csrc/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      563 2024-03-31 20:36:14.000000 kss-6.0.1/csrc/kss_cython.pyx
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5965 2024-03-31 20:12:01.000000 kss-6.0.1/csrc/sentence_splitter.cpp
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7830 2024-03-31 20:12:01.000000 kss-6.0.1/csrc/sentence_splitter.h
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.860484 kss-6.0.1/kss/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6879 2024-04-28 13:42:53.000000 kss-6.0.1/kss/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.861686 kss-6.0.1/kss/_elements/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_elements/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4888 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_elements/element.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2702 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_elements/empty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      536 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_elements/subclasses.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.861791 kss-6.0.1/kss/_modules/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_modules/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.862287 kss-6.0.1/kss/_modules/augmentation/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/augmentation/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.862387 kss-6.0.1/kss/_modules/augmentation/assets/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)  4865459 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/augmentation/assets/wordnet.json
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3892 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/augmentation/augment.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3251 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/augmentation/distance.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3602 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/augmentation/replacement.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1411 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/augmentation/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.865373 kss-6.0.1/kss/_modules/collocation/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/collocation/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9351 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/collocation/collocate.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.866106 kss-6.0.1/kss/_modules/g2p/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/g2p/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.866421 kss-6.0.1/kss/_modules/g2p/assets/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2634 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/g2p/assets/idioms.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    14802 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/g2p/assets/rules.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5390 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/g2p/assets/table.csv
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6586 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/g2p/english.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7184 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/g2p/g2p.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4459 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/g2p/numerals.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2722 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/g2p/regular.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4949 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/g2p/special.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8131 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/g2p/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.866611 kss-6.0.1/kss/_modules/hangulization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3616 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulization.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.867148 kss-6.0.1/kss/_modules/hangulization/hangulize/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2277 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    10423 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/hangul.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.867252 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1426 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.867365 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/aze/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5272 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/aze/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.867477 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/bel/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5425 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/bel/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.867598 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/bul/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4925 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/bul/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.867708 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/cat/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4328 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/cat/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.867829 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ces/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4820 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ces/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.867938 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/cym/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5791 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/cym/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.868042 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/deu/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7415 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/deu/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.868143 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ell/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9068 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ell/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.868248 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/epo/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4103 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/epo/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.868349 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/est/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3931 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/est/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.868451 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/fin/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3410 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/fin/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.868556 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/grc/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8626 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/grc/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.868656 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/hbs/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5606 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.868753 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/hun/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4990 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/hun/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.868859 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/isl/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5626 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/isl/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.868968 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ita/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4371 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ita/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.869072 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/jpn/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4446 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.869275 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/kat/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6118 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/kat/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6408 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/kat/narrow.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.869386 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/lat/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3314 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/lat/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.869502 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/lav/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4116 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/lav/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.869646 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/lit/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4080 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/lit/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.869763 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/mkd/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5354 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.869889 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/nld/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    22064 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/nld/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.870037 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/pol/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5785 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/pol/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.870294 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/por/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6048 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/por/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/por/br.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.870409 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ron/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5120 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ron/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.870549 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/rus/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4994 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/rus/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.870658 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/slk/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6693 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/slk/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.870783 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/slv/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3836 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/slv/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.870896 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/spa/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4002 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/spa/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.871000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/sqi/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3177 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.871106 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/swe/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7896 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/swe/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.871211 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/tur/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3528 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/tur/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.871327 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ukr/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5072 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.871457 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/vie/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4742 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/vie/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.871595 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/wlm/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5599 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    16108 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/models.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1069 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/normalization.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2897 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hangulization/hangulize/processing.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.871990 kss-6.0.1/kss/_modules/hanja/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hanja/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4462 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hanja/_hanja.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2021 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/hanja/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.872320 kss-6.0.1/kss/_modules/jamo/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/jamo/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    12624 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/jamo/_jamo.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      912 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/jamo/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.872640 kss-6.0.1/kss/_modules/josa/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/josa/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2580 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/josa/josa.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7030 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/josa/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.872992 kss-6.0.1/kss/_modules/keywords/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/keywords/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6362 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/keywords/extract_keywords.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    17289 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/keywords/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.873489 kss-6.0.1/kss/_modules/morphemes/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_modules/morphemes/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2652 2024-03-31 13:42:10.000000 kss-6.0.1/kss/_modules/morphemes/analyzers.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1849 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/morphemes/split_morphemes.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3588 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/morphemes/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.873693 kss-6.0.1/kss/_modules/paradigm/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/paradigm/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    18316 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/paradigm/paradigm.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.875154 kss-6.0.1/kss/_modules/preprocessing/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/preprocessing/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    15538 2024-04-27 14:56:06.000000 kss-6.0.1/kss/_modules/preprocessing/anonymize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    29795 2024-04-27 14:58:49.000000 kss-6.0.1/kss/_modules/preprocessing/clean_news.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    81165 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/preprocessing/completed_form.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    24570 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/preprocessing/filter_out.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2088 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/preprocessing/half2full.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/preprocessing/normalize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    26257 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/preprocessing/preprocess.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7186 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/preprocessing/reduce_repeats.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7661 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/preprocessing/remove_invisible_chars.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.875527 kss-6.0.1/kss/_modules/qwerty/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/qwerty/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6262 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/qwerty/qwerty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5941 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/qwerty/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.875840 kss-6.0.1/kss/_modules/romanization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/romanization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5813 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/romanization/romanize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8901 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/romanization/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.876166 kss-6.0.1/kss/_modules/safety/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/safety/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3531 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/safety/check_safety.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    35374 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/safety/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.877077 kss-6.0.1/kss/_modules/sentences/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_modules/sentences/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9334 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_modules/sentences/embracing_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    22898 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_modules/sentences/sentence_postprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6751 2024-03-31 07:55:02.000000 kss-6.0.1/kss/_modules/sentences/sentence_preprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2298 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_modules/sentences/sentence_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    30242 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_modules/sentences/sentence_splitter.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    13304 2024-03-31 20:36:14.000000 kss-6.0.1/kss/_modules/sentences/sentence_splitter_fast.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8322 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/sentences/split_sentences.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.877365 kss-6.0.1/kss/_modules/spacing/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/spacing/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5539 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/spacing/correct_spacing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   296979 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/spacing/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.877866 kss-6.0.1/kss/_modules/summarization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_modules/summarization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5603 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/summarization/summarize_sentences.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3396 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_modules/summarization/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.878587 kss-6.0.1/kss/_utils/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_utils/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       66 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_utils/api.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    10329 2024-03-31 07:46:03.000000 kss-6.0.1/kss/_utils/const.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1399 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_utils/emojis.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      910 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_utils/logger.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1001 2023-08-22 23:38:03.000000 kss-6.0.1/kss/_utils/multiprocessing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    17275 2024-04-27 14:55:22.000000 kss-6.0.1/kss/_utils/sanity_checks.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.861227 kss-6.0.1/kss.egg-info/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   159350 2024-04-28 13:42:58.000000 kss-6.0.1/kss.egg-info/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6374 2024-04-28 13:42:58.000000 kss-6.0.1/kss.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-28 13:42:58.000000 kss-6.0.1/kss.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:04:55.000000 kss-6.0.1/kss.egg-info/not-zip-safe
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      136 2024-04-28 13:42:58.000000 kss-6.0.1/kss.egg-info/requires.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       32 2024-04-28 13:42:58.000000 kss-6.0.1/kss.egg-info/top_level.txt
+-rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2024-04-28 13:42:58.881168 kss-6.0.1/setup.cfg
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6191 2024-04-27 14:55:22.000000 kss-6.0.1/setup.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 13:42:58.880603 kss-6.0.1/tests/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.1/tests/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1033 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_augmentation.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8258 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_collocation.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      250 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_g2p.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      238 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_hangulize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      747 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_hanja.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      978 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_jamo.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      442 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_josa.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3405 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_keywords.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_morphemes.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    19148 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_paradigm.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    97981 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_preprocessing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      290 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_qwerty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      257 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_romanize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      313 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_safety.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      776 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_sentences.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      236 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_spacing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1966 2024-04-27 14:55:22.000000 kss-6.0.1/tests/test_summarization.py
```

### Comparing `kss-6.0.0.dev0/LICENSE` & `kss-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/PKG-INFO` & `kss-6.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kss
-Version: 6.0.0.dev0
+Version: 6.0.1
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
-Metadata-Version: 2.1 Name: kss Version: 6.0.0.dev0 Summary: A Toolkit for
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
+Metadata-Version: 2.1 Name: kss Version: 6.0.1 Summary: A Toolkit for Korean
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

### Comparing `kss-6.0.0.dev0/README.md` & `kss-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/bench/sentence_split/sentence_split.py` & `kss-6.0.1/bench/sentence_split/sentence_split.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/bench/sentence_split/test_baseline.py` & `kss-6.0.1/bench/sentence_split/test_baseline.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/bench/sentence_split/test_kiwi.py` & `kss-6.0.1/bench/sentence_split/test_kiwi.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/bench/sentence_split/test_koalanlp.py` & `kss-6.0.1/bench/sentence_split/test_koalanlp.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/bench/sentence_split/test_kss.py` & `kss-6.0.1/bench/sentence_split/test_kss.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/bench/sentence_split/test_word_split.py` & `kss-6.0.1/bench/sentence_split/test_word_split.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/csrc/kss_cython.pyx` & `kss-6.0.1/csrc/kss_cython.pyx`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/csrc/sentence_splitter.cpp` & `kss-6.0.1/csrc/sentence_splitter.cpp`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/csrc/sentence_splitter.h` & `kss-6.0.1/csrc/sentence_splitter.h`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/__init__.py` & `kss-6.0.1/kss/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,8 +177,8 @@
         if closest_module is None:
             return None
         else:
             return closest_module
 
 
 __ALL__ = list(supported_modules.keys()) + ["Kss"]
-__version__ = "6.0.0.dev0"
+__version__ = "6.0.1"
```

### Comparing `kss-6.0.0.dev0/kss/_elements/element.py` & `kss-6.0.1/kss/_elements/element.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_elements/empty.py` & `kss-6.0.1/kss/_elements/empty.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_elements/subclasses.py` & `kss-6.0.1/kss/_elements/subclasses.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/augmentation/assets/wordnet.json` & `kss-6.0.1/kss/_modules/augmentation/assets/wordnet.json`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/augmentation/augment.py` & `kss-6.0.1/kss/_modules/augmentation/augment.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/augmentation/distance.py` & `kss-6.0.1/kss/_modules/augmentation/distance.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/augmentation/replacement.py` & `kss-6.0.1/kss/_modules/augmentation/replacement.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/augmentation/utils.py` & `kss-6.0.1/kss/_modules/augmentation/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/collocation/collocate.py` & `kss-6.0.1/kss/_modules/collocation/collocate.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/g2p/assets/idioms.txt` & `kss-6.0.1/kss/_modules/g2p/assets/idioms.txt`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/g2p/assets/rules.txt` & `kss-6.0.1/kss/_modules/g2p/assets/rules.txt`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/g2p/assets/table.csv` & `kss-6.0.1/kss/_modules/g2p/assets/table.csv`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/g2p/english.py` & `kss-6.0.1/kss/_modules/g2p/english.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/g2p/g2p.py` & `kss-6.0.1/kss/_modules/g2p/g2p.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/g2p/numerals.py` & `kss-6.0.1/kss/_modules/g2p/numerals.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/g2p/regular.py` & `kss-6.0.1/kss/_modules/g2p/regular.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/g2p/special.py` & `kss-6.0.1/kss/_modules/g2p/special.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/g2p/utils.py` & `kss-6.0.1/kss/_modules/g2p/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulization.py` & `kss-6.0.1/kss/_modules/hangulization/hangulization.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/hangul.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/hangul.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/aze/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/aze/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/bel/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/bel/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/bul/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/bul/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/cat/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/cat/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ces/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ces/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/cym/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/cym/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/deu/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/deu/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ell/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ell/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/epo/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/epo/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/est/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/est/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/fin/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/fin/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/grc/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/grc/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/hun/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/hun/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/isl/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/isl/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ita/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ita/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/kat/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/kat/narrow.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/kat/narrow.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lat/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/lat/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lav/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/lav/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/lit/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/lit/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/nld/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/nld/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/pol/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/pol/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/por/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/por/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/por/br.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/por/br.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ron/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ron/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/rus/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/rus/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/slk/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/slk/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/slv/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/slv/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/spa/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/spa/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/swe/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/swe/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/tur/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/tur/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/vie/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/vie/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/models.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/models.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/normalization.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/normalization.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hangulization/hangulize/processing.py` & `kss-6.0.1/kss/_modules/hangulization/hangulize/processing.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hanja/_hanja.py` & `kss-6.0.1/kss/_modules/hanja/_hanja.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/hanja/utils.py` & `kss-6.0.1/kss/_modules/hanja/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/jamo/_jamo.py` & `kss-6.0.1/kss/_modules/jamo/_jamo.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/jamo/utils.py` & `kss-6.0.1/kss/_modules/jamo/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/josa/josa.py` & `kss-6.0.1/kss/_modules/josa/josa.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/josa/utils.py` & `kss-6.0.1/kss/_modules/josa/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/keywords/extract_keywords.py` & `kss-6.0.1/kss/_modules/keywords/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/keywords/utils.py` & `kss-6.0.1/kss/_modules/keywords/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/morphemes/analyzers.py` & `kss-6.0.1/kss/_modules/morphemes/analyzers.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/morphemes/split_morphemes.py` & `kss-6.0.1/kss/_modules/morphemes/split_morphemes.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/morphemes/utils.py` & `kss-6.0.1/kss/_modules/morphemes/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/paradigm/paradigm.py` & `kss-6.0.1/kss/_modules/paradigm/paradigm.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/preprocessing/anonymize.py` & `kss-6.0.1/kss/_modules/preprocessing/anonymize.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/preprocessing/clean_news.py` & `kss-6.0.1/kss/_modules/preprocessing/clean_news.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/preprocessing/completed_form.py` & `kss-6.0.1/kss/_modules/preprocessing/completed_form.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/preprocessing/filter_out.py` & `kss-6.0.1/kss/_modules/preprocessing/filter_out.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/preprocessing/half2full.py` & `kss-6.0.1/kss/_modules/preprocessing/half2full.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/preprocessing/normalize.py` & `kss-6.0.1/kss/_modules/preprocessing/normalize.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/preprocessing/preprocess.py` & `kss-6.0.1/kss/_modules/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/preprocessing/reduce_repeats.py` & `kss-6.0.1/kss/_modules/preprocessing/reduce_repeats.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/preprocessing/remove_invisible_chars.py` & `kss-6.0.1/kss/_modules/preprocessing/remove_invisible_chars.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/qwerty/qwerty.py` & `kss-6.0.1/kss/_modules/qwerty/qwerty.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/qwerty/utils.py` & `kss-6.0.1/kss/_modules/qwerty/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/romanization/romanize.py` & `kss-6.0.1/kss/_modules/romanization/romanize.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/romanization/utils.py` & `kss-6.0.1/kss/_modules/romanization/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/safety/check_safety.py` & `kss-6.0.1/kss/_modules/safety/check_safety.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/safety/utils.py` & `kss-6.0.1/kss/_modules/safety/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/sentences/embracing_processor.py` & `kss-6.0.1/kss/_modules/sentences/embracing_processor.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/sentences/sentence_postprocessor.py` & `kss-6.0.1/kss/_modules/sentences/sentence_postprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/sentences/sentence_preprocessor.py` & `kss-6.0.1/kss/_modules/sentences/sentence_preprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/sentences/sentence_processor.py` & `kss-6.0.1/kss/_modules/sentences/sentence_processor.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/sentences/sentence_splitter.py` & `kss-6.0.1/kss/_modules/sentences/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/sentences/sentence_splitter_fast.py` & `kss-6.0.1/kss/_modules/sentences/sentence_splitter_fast.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/sentences/split_sentences.py` & `kss-6.0.1/kss/_modules/sentences/split_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/spacing/correct_spacing.py` & `kss-6.0.1/kss/_modules/spacing/correct_spacing.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/spacing/utils.py` & `kss-6.0.1/kss/_modules/spacing/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/summarization/summarize_sentences.py` & `kss-6.0.1/kss/_modules/summarization/summarize_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_modules/summarization/utils.py` & `kss-6.0.1/kss/_modules/summarization/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_utils/const.py` & `kss-6.0.1/kss/_utils/const.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_utils/emojis.py` & `kss-6.0.1/kss/_utils/emojis.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_utils/logger.py` & `kss-6.0.1/kss/_utils/logger.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_utils/multiprocessing.py` & `kss-6.0.1/kss/_utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss/_utils/sanity_checks.py` & `kss-6.0.1/kss/_utils/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/kss.egg-info/PKG-INFO` & `kss-6.0.1/kss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kss
-Version: 6.0.0.dev0
+Version: 6.0.1
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
-Metadata-Version: 2.1 Name: kss Version: 6.0.0.dev0 Summary: A Toolkit for
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
+Metadata-Version: 2.1 Name: kss Version: 6.0.1 Summary: A Toolkit for Korean
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

### Comparing `kss-6.0.0.dev0/kss.egg-info/SOURCES.txt` & `kss-6.0.1/kss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/setup.py` & `kss-6.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/tests/test_augmentation.py` & `kss-6.0.1/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/tests/test_collocation.py` & `kss-6.0.1/tests/test_collocation.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/tests/test_hanja.py` & `kss-6.0.1/tests/test_hanja.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/tests/test_jamo.py` & `kss-6.0.1/tests/test_jamo.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/tests/test_keywords.py` & `kss-6.0.1/tests/test_keywords.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/tests/test_paradigm.py` & `kss-6.0.1/tests/test_paradigm.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/tests/test_preprocessing.py` & `kss-6.0.1/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/tests/test_sentences.py` & `kss-6.0.1/tests/test_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.0.dev0/tests/test_summarization.py` & `kss-6.0.1/tests/test_summarization.py`

 * *Files identical despite different names*

