# Comparing `tmp/pyDecision-4.5.1.tar.gz` & `tmp/pyDecision-4.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-4.5.1.tar", last modified: Sat Apr 27 02:01:25 2024, max compression
+gzip compressed data, was "dist\pyDecision-4.5.2.tar", last modified: Sat Apr 27 19:58:17 2024, max compression
```

## Comparing `pyDecision-4.5.1.tar` & `pyDecision-4.5.2.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 02:01:25.000000 pyDecision-4.5.1/
--rw-rw-rw-   0        0        0      656 2023-10-24 20:28:27.000000 pyDecision-4.5.1/LICENSE
--rw-rw-rw-   0        0        0    20106 2024-04-27 02:01:25.000000 pyDecision-4.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    19604 2024-04-27 01:58:37.000000 pyDecision-4.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 02:01:24.000000 pyDecision-4.5.1/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.5.1/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 02:01:25.000000 pyDecision-4.5.1/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     3187 2024-04-26 23:34:28.000000 pyDecision-4.5.1/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1638 2023-08-15 11:11:40.000000 pyDecision-4.5.1/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.5.1/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.5.1/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     2553 2023-11-10 15:52:16.000000 pyDecision-4.5.1/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0     1006 2023-11-12 15:54:44.000000 pyDecision-4.5.1/pyDecision/algorithm/bwm_s.py
--rw-rw-rw-   0        0        0     1221 2024-04-24 14:49:40.000000 pyDecision-4.5.1/pyDecision/algorithm/cilos.py
--rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.5.1/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.5.1/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.5.1/pyDecision/algorithm/copeland.py
--rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.5.1/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.5.1/pyDecision/algorithm/cradis.py
--rw-rw-rw-   0        0        0     1125 2023-10-24 20:07:49.000000 pyDecision-4.5.1/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.5.1/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.5.1/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.5.1/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.5.1/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.5.1/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.5.1/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.5.1/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.5.1/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.5.1/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.5.1/pyDecision/algorithm/entropy.py
--rw-rw-rw-   0        0        0     2289 2024-04-24 15:29:47.000000 pyDecision-4.5.1/pyDecision/algorithm/fucom.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_aras.py
--rw-rw-rw-   0        0        0     4635 2023-11-12 11:24:00.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_bwm.py
--rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_copras.py
--rw-rw-rw-   0        0        0     2500 2024-04-26 21:40:48.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_critic.py
--rw-rw-rw-   0        0        0     4100 2023-08-01 01:06:41.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     5402 2024-04-27 00:21:30.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_fucom.py
--rw-rw-rw-   0        0        0     1786 2024-04-26 21:41:04.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_merec.py
--rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_moora.py
--rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_ocra.py
--rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     5399 2023-09-09 01:09:43.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_waspas.py
--rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.5.1/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     2300 2023-10-26 23:42:55.000000 pyDecision-4.5.1/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.5.1/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.5.1/pyDecision/algorithm/macbeth.py
--rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.5.1/pyDecision/algorithm/mairca.py
--rw-rw-rw-   0        0        0     2598 2024-04-25 15:20:07.000000 pyDecision-4.5.1/pyDecision/algorithm/mara.py
--rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.5.1/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.5.1/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0     1175 2023-10-26 23:47:00.000000 pyDecision-4.5.1/pyDecision/algorithm/merec.py
--rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.5.1/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.5.1/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.5.1/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.5.1/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     2563 2023-09-09 00:46:31.000000 pyDecision-4.5.1/pyDecision/algorithm/oreste.py
--rw-rw-rw-   0        0        0    13836 2023-10-30 12:17:12.000000 pyDecision-4.5.1/pyDecision/algorithm/p_ec.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.5.1/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.5.1/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.5.1/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.5.1/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6622 2023-08-02 21:49:15.000000 pyDecision-4.5.1/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.5.1/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.5.1/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.5.1/pyDecision/algorithm/piv.py
--rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.5.1/pyDecision/algorithm/psi.py
--rw-rw-rw-   0        0        0      688 2024-04-25 15:23:46.000000 pyDecision-4.5.1/pyDecision/algorithm/psi_m.py
--rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:15.000000 pyDecision-4.5.1/pyDecision/algorithm/regime.py
--rw-rw-rw-   0        0        0      969 2024-04-26 21:38:23.000000 pyDecision-4.5.1/pyDecision/algorithm/roc.py
--rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.5.1/pyDecision/algorithm/rov.py
--rw-rw-rw-   0        0        0      970 2024-04-26 21:39:12.000000 pyDecision-4.5.1/pyDecision/algorithm/rrw.py
--rw-rw-rw-   0        0        0      929 2024-04-26 21:38:49.000000 pyDecision-4.5.1/pyDecision/algorithm/rsw.py
--rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.5.1/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.5.1/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2185 2023-08-02 00:35:27.000000 pyDecision-4.5.1/pyDecision/algorithm/spotis.py
--rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.5.1/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.5.1/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.5.1/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0     4278 2023-09-08 23:55:42.000000 pyDecision-4.5.1/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.5.1/pyDecision/algorithm/wings.py
--rw-rw-rw-   0        0        0     3188 2024-04-24 01:11:01.000000 pyDecision-4.5.1/pyDecision/algorithm/wisp.py
-drwxrwxrwx   0        0        0        0 2024-04-27 02:01:25.000000 pyDecision-4.5.1/pyDecision/compare/
--rw-rw-rw-   0        0        0      127 2024-04-27 00:17:39.000000 pyDecision-4.5.1/pyDecision/compare/__init__.py
--rw-rw-rw-   0        0        0    26165 2024-04-27 01:59:48.000000 pyDecision-4.5.1/pyDecision/compare/compare.py
-drwxrwxrwx   0        0        0        0 2024-04-27 02:01:25.000000 pyDecision-4.5.1/pyDecision/util/
--rw-rw-rw-   0        0        0     8733 2023-12-03 18:26:24.000000 pyDecision-4.5.1/pyDecision/util/LLM.py
--rw-rw-rw-   0        0        0      109 2023-08-02 19:44:51.000000 pyDecision-4.5.1/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0     6266 2023-08-02 19:44:27.000000 pyDecision-4.5.1/pyDecision/util/ga.py
-drwxrwxrwx   0        0        0        0 2024-04-27 02:01:24.000000 pyDecision-4.5.1/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    20106 2024-04-27 02:01:23.000000 pyDecision-4.5.1/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2742 2024-04-27 02:01:23.000000 pyDecision-4.5.1/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 02:01:23.000000 pyDecision-4.5.1/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-27 02:01:23.000000 pyDecision-4.5.1/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-27 02:01:23.000000 pyDecision-4.5.1/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 02:01:25.000000 pyDecision-4.5.1/setup.cfg
--rw-rw-rw-   0        0        0      744 2024-04-26 21:35:52.000000 pyDecision-4.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:58:17.000000 pyDecision-4.5.2/
+-rw-rw-rw-   0        0        0      656 2023-10-24 20:28:27.000000 pyDecision-4.5.2/LICENSE
+-rw-rw-rw-   0        0        0    20343 2024-04-27 19:58:17.000000 pyDecision-4.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    19840 2024-04-27 19:55:54.000000 pyDecision-4.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 19:58:15.000000 pyDecision-4.5.2/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.5.2/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:58:16.000000 pyDecision-4.5.2/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     3226 2024-04-27 19:46:40.000000 pyDecision-4.5.2/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1638 2023-08-15 11:11:40.000000 pyDecision-4.5.2/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.5.2/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.5.2/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     2553 2023-11-10 15:52:16.000000 pyDecision-4.5.2/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0     1006 2023-11-12 15:54:44.000000 pyDecision-4.5.2/pyDecision/algorithm/bwm_s.py
+-rw-rw-rw-   0        0        0     1221 2024-04-24 14:49:40.000000 pyDecision-4.5.2/pyDecision/algorithm/cilos.py
+-rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.5.2/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.5.2/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.5.2/pyDecision/algorithm/copeland.py
+-rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.5.2/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.5.2/pyDecision/algorithm/cradis.py
+-rw-rw-rw-   0        0        0     1125 2023-10-24 20:07:49.000000 pyDecision-4.5.2/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.5.2/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.5.2/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.5.2/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.5.2/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.5.2/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.5.2/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.5.2/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.5.2/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.5.2/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.5.2/pyDecision/algorithm/entropy.py
+-rw-rw-rw-   0        0        0     2289 2024-04-24 15:29:47.000000 pyDecision-4.5.2/pyDecision/algorithm/fucom.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_aras.py
+-rw-rw-rw-   0        0        0     4635 2023-11-12 11:24:00.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_bwm.py
+-rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_copras.py
+-rw-rw-rw-   0        0        0     2500 2024-04-26 21:40:48.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_critic.py
+-rw-rw-rw-   0        0        0     4100 2023-08-01 01:06:41.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     5402 2024-04-27 00:21:30.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_fucom.py
+-rw-rw-rw-   0        0        0     1786 2024-04-26 21:41:04.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_merec.py
+-rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_moora.py
+-rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_ocra.py
+-rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     5399 2023-09-09 01:09:43.000000 pyDecision-4.5.2/pyDecision/algorithm/fuzzy_waspas.py
+-rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.5.2/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     2300 2023-10-26 23:42:55.000000 pyDecision-4.5.2/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.5.2/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.5.2/pyDecision/algorithm/macbeth.py
+-rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.5.2/pyDecision/algorithm/mairca.py
+-rw-rw-rw-   0        0        0     2598 2024-04-25 15:20:07.000000 pyDecision-4.5.2/pyDecision/algorithm/mara.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.5.2/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.5.2/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0     1175 2023-10-26 23:47:00.000000 pyDecision-4.5.2/pyDecision/algorithm/merec.py
+-rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.5.2/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.5.2/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.5.2/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.5.2/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     2563 2023-09-09 00:46:31.000000 pyDecision-4.5.2/pyDecision/algorithm/oreste.py
+-rw-rw-rw-   0        0        0    13836 2023-10-30 12:17:12.000000 pyDecision-4.5.2/pyDecision/algorithm/p_ec.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.5.2/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.5.2/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.5.2/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.5.2/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6622 2023-08-02 21:49:15.000000 pyDecision-4.5.2/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.5.2/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.5.2/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.5.2/pyDecision/algorithm/piv.py
+-rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.5.2/pyDecision/algorithm/psi.py
+-rw-rw-rw-   0        0        0      688 2024-04-25 15:23:46.000000 pyDecision-4.5.2/pyDecision/algorithm/psi_m.py
+-rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:15.000000 pyDecision-4.5.2/pyDecision/algorithm/regime.py
+-rw-rw-rw-   0        0        0      969 2024-04-26 21:38:23.000000 pyDecision-4.5.2/pyDecision/algorithm/roc.py
+-rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.5.2/pyDecision/algorithm/rov.py
+-rw-rw-rw-   0        0        0      970 2024-04-26 21:39:12.000000 pyDecision-4.5.2/pyDecision/algorithm/rrw.py
+-rw-rw-rw-   0        0        0      929 2024-04-26 21:38:49.000000 pyDecision-4.5.2/pyDecision/algorithm/rsw.py
+-rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.5.2/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     1991 2024-04-27 19:45:13.000000 pyDecision-4.5.2/pyDecision/algorithm/seca.py
+-rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.5.2/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2185 2023-08-02 00:35:27.000000 pyDecision-4.5.2/pyDecision/algorithm/spotis.py
+-rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.5.2/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.5.2/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.5.2/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0     4278 2023-09-08 23:55:42.000000 pyDecision-4.5.2/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.5.2/pyDecision/algorithm/wings.py
+-rw-rw-rw-   0        0        0     3188 2024-04-24 01:11:01.000000 pyDecision-4.5.2/pyDecision/algorithm/wisp.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:58:16.000000 pyDecision-4.5.2/pyDecision/compare/
+-rw-rw-rw-   0        0        0      127 2024-04-27 00:17:39.000000 pyDecision-4.5.2/pyDecision/compare/__init__.py
+-rw-rw-rw-   0        0        0    26444 2024-04-27 19:49:24.000000 pyDecision-4.5.2/pyDecision/compare/compare.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:58:17.000000 pyDecision-4.5.2/pyDecision/util/
+-rw-rw-rw-   0        0        0     8733 2023-12-03 18:26:24.000000 pyDecision-4.5.2/pyDecision/util/LLM.py
+-rw-rw-rw-   0        0        0      109 2023-08-02 19:44:51.000000 pyDecision-4.5.2/pyDecision/util/__init__.py
+-rw-rw-rw-   0        0        0     6266 2023-08-02 19:44:27.000000 pyDecision-4.5.2/pyDecision/util/ga.py
+drwxrwxrwx   0        0        0        0 2024-04-27 19:58:15.000000 pyDecision-4.5.2/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    20343 2024-04-27 19:58:14.000000 pyDecision-4.5.2/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2771 2024-04-27 19:58:15.000000 pyDecision-4.5.2/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 19:58:14.000000 pyDecision-4.5.2/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-27 19:58:14.000000 pyDecision-4.5.2/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-27 19:58:14.000000 pyDecision-4.5.2/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 19:58:17.000000 pyDecision-4.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      744 2024-04-27 19:49:47.000000 pyDecision-4.5.2/setup.py
```

### Comparing `pyDecision-4.5.1/LICENSE` & `pyDecision-4.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/PKG-INFO` & `pyDecision-4.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.5.1
+Version: 4.5.2
 Summary: A MCDA Library Incorporating a Large Language Model to Enhance Decision Analysis
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SECA** (Simultaneous Evaluation of Criteria and Alternatives); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
 
 pyDecision offers an array of features, including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Citation
 
 PEREIRA, V.; BASILIO, M.P.; SANTOS, C.H.T (2024). Enhancing Decision Analysis with a Large Language Model: pyDecision a Comprehensive Library of MCDA Methods in Python. arXiv. https://arxiv.org/abs/2404.06370
 
@@ -130,14 +130,15 @@
 - MPSI ([ Colab Demo ](https://colab.research.google.com/drive/1zj2AS6W_VWmG5mYgY4b-dnCK0q3AG1-K?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/BF00221383))
 - ROC ([ Colab Demo ](https://colab.research.google.com/drive/1uUFXlCsZkFnh8HemNJ_hppvDC1eAwu4W?usp=sharing)) ( [ Paper ](https://doi.org/10.1002/(SICI)1099-0771(199806)11:2<85::AID-BDM282>3.0.CO;2-K))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - RRW ([ Colab Demo ](https://colab.research.google.com/drive/1Pd13mNOosg0bxKAhALA3U9ppQYMB6yp_?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0030-5073(81)90015-5))
 - RSW ([ Colab Demo ](https://colab.research.google.com/drive/1IvAmwypsA6J3JRKGQsi0fmwnlGmL3rKM?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0030-5073(81)90015-5))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
+- SECA ([ Colab Demo ](https://colab.research.google.com/drive/1Hs2zeOPJdkpdeXnfg6_GeWN6zo5JrIzn?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2018.167))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.23919/FUSION45008.2020.9190347))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2007.10.046))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0377-2217(03)00020-1))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
```

### Comparing `pyDecision-4.5.1/README.md` & `pyDecision-4.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SECA** (Simultaneous Evaluation of Criteria and Alternatives); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
 
 pyDecision offers an array of features, including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Citation
 
 PEREIRA, V.; BASILIO, M.P.; SANTOS, C.H.T (2024). Enhancing Decision Analysis with a Large Language Model: pyDecision a Comprehensive Library of MCDA Methods in Python. arXiv. https://arxiv.org/abs/2404.06370
 
@@ -119,14 +119,15 @@
 - MPSI ([ Colab Demo ](https://colab.research.google.com/drive/1zj2AS6W_VWmG5mYgY4b-dnCK0q3AG1-K?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/BF00221383))
 - ROC ([ Colab Demo ](https://colab.research.google.com/drive/1uUFXlCsZkFnh8HemNJ_hppvDC1eAwu4W?usp=sharing)) ( [ Paper ](https://doi.org/10.1002/(SICI)1099-0771(199806)11:2<85::AID-BDM282>3.0.CO;2-K))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - RRW ([ Colab Demo ](https://colab.research.google.com/drive/1Pd13mNOosg0bxKAhALA3U9ppQYMB6yp_?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0030-5073(81)90015-5))
 - RSW ([ Colab Demo ](https://colab.research.google.com/drive/1IvAmwypsA6J3JRKGQsi0fmwnlGmL3rKM?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0030-5073(81)90015-5))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
+- SECA ([ Colab Demo ](https://colab.research.google.com/drive/1Hs2zeOPJdkpdeXnfg6_GeWN6zo5JrIzn?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2018.167))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.23919/FUSION45008.2020.9190347))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2007.10.046))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0377-2217(03)00020-1))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
```

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/__init__.py` & `pyDecision-4.5.2/pyDecision/algorithm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 from .psi_m         import mpsi_method
 from .regime        import regime_method
 from .roc           import roc_method
 from .rov           import rov_method
 from .rrw           import rrw_method
 from .rsw           import rsw_method
 from .saw           import saw_method
+from .seca          import seca_method
 from .smart         import smart_method
 from .spotis        import spotis_method
 from .todim         import todim_method
 from .topsis        import topsis_method
 from .vikor         import vikor_method, ranking
 from .waspas        import waspas_method
 from .wisp          import wisp_method
```

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/ahp.py` & `pyDecision-4.5.2/pyDecision/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/aras.py` & `pyDecision-4.5.2/pyDecision/algorithm/aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/borda.py` & `pyDecision-4.5.2/pyDecision/algorithm/borda.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/bwm.py` & `pyDecision-4.5.2/pyDecision/algorithm/bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/bwm_s.py` & `pyDecision-4.5.2/pyDecision/algorithm/bwm_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/cilos.py` & `pyDecision-4.5.2/pyDecision/algorithm/cilos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/cocoso.py` & `pyDecision-4.5.2/pyDecision/algorithm/cocoso.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/codas.py` & `pyDecision-4.5.2/pyDecision/algorithm/codas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/copeland.py` & `pyDecision-4.5.2/pyDecision/algorithm/copeland.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/copras.py` & `pyDecision-4.5.2/pyDecision/algorithm/copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/cradis.py` & `pyDecision-4.5.2/pyDecision/algorithm/cradis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/critic.py` & `pyDecision-4.5.2/pyDecision/algorithm/critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/dematel.py` & `pyDecision-4.5.2/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/e_i.py` & `pyDecision-4.5.2/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/e_i_s.py` & `pyDecision-4.5.2/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/e_i_v.py` & `pyDecision-4.5.2/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/e_ii.py` & `pyDecision-4.5.2/pyDecision/algorithm/e_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/e_iii.py` & `pyDecision-4.5.2/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/e_iv.py` & `pyDecision-4.5.2/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/e_tri_b.py` & `pyDecision-4.5.2/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/edas.py` & `pyDecision-4.5.2/pyDecision/algorithm/edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/entropy.py` & `pyDecision-4.5.2/pyDecision/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fucom.py` & `pyDecision-4.5.2/pyDecision/algorithm/fucom.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_aras.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_bwm.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_copras.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_critic.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_fucom.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_fucom.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_merec.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_merec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_moora.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_ocra.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_waspas.py` & `pyDecision-4.5.2/pyDecision/algorithm/fuzzy_waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/gra.py` & `pyDecision-4.5.2/pyDecision/algorithm/gra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/idocriw.py` & `pyDecision-4.5.2/pyDecision/algorithm/idocriw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/mabac.py` & `pyDecision-4.5.2/pyDecision/algorithm/mabac.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/macbeth.py` & `pyDecision-4.5.2/pyDecision/algorithm/macbeth.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/mairca.py` & `pyDecision-4.5.2/pyDecision/algorithm/mairca.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/mara.py` & `pyDecision-4.5.2/pyDecision/algorithm/mara.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/marcos.py` & `pyDecision-4.5.2/pyDecision/algorithm/marcos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/maut.py` & `pyDecision-4.5.2/pyDecision/algorithm/maut.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/merec.py` & `pyDecision-4.5.2/pyDecision/algorithm/merec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/moora.py` & `pyDecision-4.5.2/pyDecision/algorithm/moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/moosra.py` & `pyDecision-4.5.2/pyDecision/algorithm/moosra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/multimoora.py` & `pyDecision-4.5.2/pyDecision/algorithm/multimoora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/ocra.py` & `pyDecision-4.5.2/pyDecision/algorithm/ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/oreste.py` & `pyDecision-4.5.2/pyDecision/algorithm/oreste.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/p_ec.py` & `pyDecision-4.5.2/pyDecision/algorithm/p_ec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/p_i.py` & `pyDecision-4.5.2/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/p_ii.py` & `pyDecision-4.5.2/pyDecision/algorithm/p_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/p_iii.py` & `pyDecision-4.5.2/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/p_iv.py` & `pyDecision-4.5.2/pyDecision/algorithm/p_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/p_v.py` & `pyDecision-4.5.2/pyDecision/algorithm/p_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/p_vi.py` & `pyDecision-4.5.2/pyDecision/algorithm/p_vi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/p_xgaia.py` & `pyDecision-4.5.2/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/piv.py` & `pyDecision-4.5.2/pyDecision/algorithm/piv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/psi.py` & `pyDecision-4.5.2/pyDecision/algorithm/psi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/psi_m.py` & `pyDecision-4.5.2/pyDecision/algorithm/psi_m.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/regime.py` & `pyDecision-4.5.2/pyDecision/algorithm/regime.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/roc.py` & `pyDecision-4.5.2/pyDecision/algorithm/roc.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/rov.py` & `pyDecision-4.5.2/pyDecision/algorithm/rov.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/rrw.py` & `pyDecision-4.5.2/pyDecision/algorithm/rrw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/rsw.py` & `pyDecision-4.5.2/pyDecision/algorithm/rsw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/saw.py` & `pyDecision-4.5.2/pyDecision/algorithm/saw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/smart.py` & `pyDecision-4.5.2/pyDecision/algorithm/smart.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/spotis.py` & `pyDecision-4.5.2/pyDecision/algorithm/spotis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/todim.py` & `pyDecision-4.5.2/pyDecision/algorithm/todim.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/topsis.py` & `pyDecision-4.5.2/pyDecision/algorithm/topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/vikor.py` & `pyDecision-4.5.2/pyDecision/algorithm/vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/waspas.py` & `pyDecision-4.5.2/pyDecision/algorithm/waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/wings.py` & `pyDecision-4.5.2/pyDecision/algorithm/wings.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/algorithm/wisp.py` & `pyDecision-4.5.2/pyDecision/algorithm/wisp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/compare/compare.py` & `pyDecision-4.5.2/pyDecision/compare/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pyDecision.algorithm.fucom        import fucom_method
 from pyDecision.algorithm.idocriw      import idocriw_method
 from pyDecision.algorithm.merec        import merec_method
 from pyDecision.algorithm.psi_m        import mpsi_method
 from pyDecision.algorithm.roc          import roc_method
 from pyDecision.algorithm.rrw          import rrw_method
 from pyDecision.algorithm.rsw          import rsw_method
+from pyDecision.algorithm.seca         import seca_method
 
 from pyDecision.algorithm.fuzzy_bwm    import fuzzy_bw_method
 from pyDecision.algorithm.fuzzy_critic import fuzzy_critic_method
 from pyDecision.algorithm.fuzzy_fucom  import fuzzy_fucom_method
 from pyDecision.algorithm.fuzzy_merec  import fuzzy_merec_method
 
 from pyDecision.algorithm.aras         import aras_method
@@ -124,17 +125,17 @@
         for (i, j), z in np.ndenumerate(corr_df):
             plt.text(j, i, '{:0.2f}'.format(z), ha = 'center', va = 'center', fontsize = font_size, bbox = dict(boxstyle = 'round', facecolor = 'white', edgecolor = '0.1'))
     return corr_df
 
 ###############################################################################
 
 # Function: Compare Weights Crisp
-def compare_weights(dataset, criterion_type, custom_methods = [], custom_weigths = [], methods_list = [], mic = [], lic = [], criteria_priority = [], criteria_rank = [], alpha = 0.5):
+def compare_weights(dataset, criterion_type, custom_methods = [], custom_weigths = [], methods_list = [], mic = [], lic = [], criteria_priority = [], criteria_rank = [], alpha = 0.5, beta = 3):
     if ('all' in methods_list):
-        methods_list = ['bwm', 'bwm_s', 'cilos', 'critic', 'entropy', 'fucom', 'idocriw', 'merec', 'mpsi', 'roc', 'rrw', 'rsw']
+        methods_list = ['bwm', 'bwm_s', 'cilos', 'critic', 'entropy', 'fucom', 'idocriw', 'merec', 'mpsi', 'roc', 'rrw', 'rsw', 'seca']
     if (len(custom_methods) > 0):
         methods_list = custom_methods + methods_list 
     X       = np.zeros((dataset.shape[1], len(methods_list)))
     j       = 0
     for i in range(0, len(custom_weigths)):
         X[:,j] = custom_weigths[i]
         j      = j + 1 
@@ -196,14 +197,19 @@
             j      = j + 1
             print('RRW: Done!')
         if (method == 'rsw' or method == 'all'):
             w      = rsw_method(criteria_rank)
             X[:,j] = w
             j      = j + 1
             print('RSW: Done!')
+        if (method == 'seca' or method == 'all'):
+            w      = seca_method(dataset, criterion_type, beta)
+            X[:,j] = w
+            j      = j + 1
+            print('SECA: Done!')
     X = pd.DataFrame(X, index = ['g'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)    
     return X
 
 # Function: Compare Weights Fuzzy
 def compare_weights_fuzzy(dataset = [], criterion_type = [], custom_methods = [], custom_weigths = [], methods_list = [], criteria_priority = [], criteria_rank = [], mic = [], lic = [], eps_penalty = 1, n_starts = 250):
     if ('all' in methods_list):
         methods_list = ['fuzzy_bwm', 'fuzzy_critic', 'fuzzy_fucom', 'fuzzy_merec']
```

### Comparing `pyDecision-4.5.1/pyDecision/util/LLM.py` & `pyDecision-4.5.2/pyDecision/util/LLM.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision/util/ga.py` & `pyDecision-4.5.2/pyDecision/util/ga.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.1/pyDecision.egg-info/PKG-INFO` & `pyDecision-4.5.2/pyDecision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.5.1
+Version: 4.5.2
 Summary: A MCDA Library Incorporating a Large Language Model to Enhance Decision Analysis
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SECA** (Simultaneous Evaluation of Criteria and Alternatives); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
 
 pyDecision offers an array of features, including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Citation
 
 PEREIRA, V.; BASILIO, M.P.; SANTOS, C.H.T (2024). Enhancing Decision Analysis with a Large Language Model: pyDecision a Comprehensive Library of MCDA Methods in Python. arXiv. https://arxiv.org/abs/2404.06370
 
@@ -130,14 +130,15 @@
 - MPSI ([ Colab Demo ](https://colab.research.google.com/drive/1zj2AS6W_VWmG5mYgY4b-dnCK0q3AG1-K?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/BF00221383))
 - ROC ([ Colab Demo ](https://colab.research.google.com/drive/1uUFXlCsZkFnh8HemNJ_hppvDC1eAwu4W?usp=sharing)) ( [ Paper ](https://doi.org/10.1002/(SICI)1099-0771(199806)11:2<85::AID-BDM282>3.0.CO;2-K))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - RRW ([ Colab Demo ](https://colab.research.google.com/drive/1Pd13mNOosg0bxKAhALA3U9ppQYMB6yp_?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0030-5073(81)90015-5))
 - RSW ([ Colab Demo ](https://colab.research.google.com/drive/1IvAmwypsA6J3JRKGQsi0fmwnlGmL3rKM?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0030-5073(81)90015-5))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
+- SECA ([ Colab Demo ](https://colab.research.google.com/drive/1Hs2zeOPJdkpdeXnfg6_GeWN6zo5JrIzn?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2018.167))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.23919/FUSION45008.2020.9190347))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2007.10.046))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0377-2217(03)00020-1))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
```

### Comparing `pyDecision-4.5.1/pyDecision.egg-info/SOURCES.txt` & `pyDecision-4.5.2/pyDecision.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 pyDecision/algorithm/psi_m.py
 pyDecision/algorithm/regime.py
 pyDecision/algorithm/roc.py
 pyDecision/algorithm/rov.py
 pyDecision/algorithm/rrw.py
 pyDecision/algorithm/rsw.py
 pyDecision/algorithm/saw.py
+pyDecision/algorithm/seca.py
 pyDecision/algorithm/smart.py
 pyDecision/algorithm/spotis.py
 pyDecision/algorithm/todim.py
 pyDecision/algorithm/topsis.py
 pyDecision/algorithm/vikor.py
 pyDecision/algorithm/waspas.py
 pyDecision/algorithm/wings.py
```

### Comparing `pyDecision-4.5.1/setup.py` & `pyDecision-4.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='4.5.1',
+    version='4.5.2',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```

