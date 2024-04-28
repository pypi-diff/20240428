# Comparing `tmp/tart-1.2.0b1.tar.gz` & `tmp/tart-1.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tart-1.2.0b1.tar", last modified: Sat Dec  2 11:59:30 2023, max compression
+gzip compressed data, was "tart-1.2.0b3.tar", last modified: Sun Apr 28 09:02:33 2024, max compression
```

## Comparing `tart-1.2.0b1.tar` & `tart-1.2.0b3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:30.729797 tart-1.2.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-12-02 11:59:20.000000 tart-1.2.0b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-02 11:59:20.000000 tart-1.2.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2023-12-02 11:59:30.729797 tart-1.2.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-12-02 11:59:20.000000 tart-1.2.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-02 11:59:30.729797 tart-1.2.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-12-02 11:59:20.000000 tart-1.2.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:30.713797 tart-1.2.0b1/tart/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:30.717797 tart-1.2.0b1/tart/imaging/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/antenna_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7686 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/correlator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/elaz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/ephemerides_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9446 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/ephemeris.py
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/gps_satellite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/gps_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     9814 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/radio_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/simulate_transit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/sp3_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/sun.py
--rw-r--r--   0 runner    (1001) docker     (127)    12238 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/synthesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/tart_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:30.721797 tart-1.2.0b1/tart/imaging/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/test_antenna_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/test_correlator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/test_elaz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/test_ephemerides_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/test_ephemeris.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/test_gps_satellite.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/test_gps_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    15826 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/test_sun.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/test_tart_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/test/test_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12746 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/uvfitsgenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/imaging/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:30.721797 tart-1.2.0b1/tart/operation/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/operation/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/operation/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:30.721797 tart-1.2.0b1/tart/operation/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/operation/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/operation/test/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/operation/test/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/operation/test/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:30.725797 tart-1.2.0b1/tart/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/antennas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/butter_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/calculate_delay.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/sample_delay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/sample_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/simulation_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14932 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/skymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/telescope_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/telescope_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:30.725797 tart-1.2.0b1/tart/simulation/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/test/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/test/test_antennas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/test/test_radio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/test/test_simulated_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/test/test_simulation_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/test/test_skymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/simulation/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:30.725797 tart-1.2.0b1/tart/test/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/test/testbench.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:30.729797 tart-1.2.0b1/tart/util/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/compare_phases.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/hilbert.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/mp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/nelder_mead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/skyloc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:30.729797 tart-1.2.0b1/tart/util/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/test/all.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/test/test_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/test/test_compare_phases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/test/test_utc.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/utc.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-12-02 11:59:20.000000 tart-1.2.0b1/tart/util/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 11:59:30.729797 tart-1.2.0b1/tart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2023-12-02 11:59:30.000000 tart-1.2.0b1/tart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2023-12-02 11:59:30.000000 tart-1.2.0b1/tart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-02 11:59:30.000000 tart-1.2.0b1/tart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-02 11:59:30.000000 tart-1.2.0b1/tart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-02 11:59:30.000000 tart-1.2.0b1/tart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:33.443235 tart-1.2.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-28 09:02:29.000000 tart-1.2.0b3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 09:02:29.000000 tart-1.2.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-28 09:02:33.443235 tart-1.2.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-28 09:02:29.000000 tart-1.2.0b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-28 09:02:33.443235 tart-1.2.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-28 09:02:29.000000 tart-1.2.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:33.431235 tart-1.2.0b3/tart/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:33.435235 tart-1.2.0b3/tart/imaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/antenna_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/correlator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/elaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/ephemerides_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/ephemeris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/gps_satellite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/gps_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/radio_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/simulate_transit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/sp3_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/sun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/tart_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:33.435235 tart-1.2.0b3/tart/imaging/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/test_antenna_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/test_correlator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/test_elaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/test_ephemerides_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/test_ephemeris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/test_gps_satellite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/test_gps_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15826 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/test_sun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/test_tart_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/test/test_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/uvfitsgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/imaging/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:33.435235 tart-1.2.0b3/tart/operation/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/operation/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/operation/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:33.439235 tart-1.2.0b3/tart/operation/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/operation/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/operation/test/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/operation/test/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/operation/test/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:33.439235 tart-1.2.0b3/tart/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/antennas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/butter_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/calculate_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/sample_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/sample_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/simulation_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14932 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/telescope_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/telescope_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:33.439235 tart-1.2.0b3/tart/simulation/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/test/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/test/test_antennas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/test/test_radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/test/test_simulated_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/test/test_simulation_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/test/test_skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/simulation/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:33.439235 tart-1.2.0b3/tart/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/test/testbench.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:33.443235 tart-1.2.0b3/tart/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/compare_phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/hilbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/nelder_mead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/skyloc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:33.443235 tart-1.2.0b3/tart/util/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/test/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/test/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/test/test_compare_phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/test/test_utc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/utc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-28 09:02:29.000000 tart-1.2.0b3/tart/util/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:02:33.443235 tart-1.2.0b3/tart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-28 09:02:33.000000 tart-1.2.0b3/tart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-28 09:02:33.000000 tart-1.2.0b3/tart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 09:02:33.000000 tart-1.2.0b3/tart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-28 09:02:33.000000 tart-1.2.0b3/tart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-28 09:02:33.000000 tart-1.2.0b3/tart.egg-info/top_level.txt
```

### Comparing `tart-1.2.0b1/LICENSE.txt` & `tart-1.2.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/PKG-INFO` & `tart-1.2.0b3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tart
-Version: 1.2.0b1
+Version: 1.2.0b3
 Summary: Transient Array Radio Telescope Imaging and Operation Library
-Home-page: http://github.com/tmolteno/TART
+Home-page: http://github.com/tmolteno/tart_modules
 Author: Tim Molteno
 Author-email: tim@elec.ac.nz
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Communications :: Ham Radio
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tart-1.2.0b1/README.md` & `tart-1.2.0b3/README.md`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/setup.py` & `tart-1.2.0b3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(name='tart',
-    version='1.2.0b1',
+    version='1.2.0b3',
     description='Transient Array Radio Telescope Imaging and Operation Library',
     long_description=readme,
     long_description_content_type="text/markdown",
-    url='http://github.com/tmolteno/TART',
+    url='http://github.com/tmolteno/tart_modules',
     author='Tim Molteno',
     author_email='tim@elec.ac.nz',
     license='GPLv3',
     install_requires=['numpy', 'matplotlib', 'healpy', 'astropy', 'h5py', 'python-dateutil'],
     packages=['tart', 'tart.imaging', 'tart.simulation', 'tart.operation', 'tart.util',\
             'tart.test',  'tart.imaging.test', 'tart.simulation.test', 'tart.operation.test', 'tart.util.test'],
     classifiers=[
```

### Comparing `tart-1.2.0b1/tart/imaging/antenna_model.py` & `tart-1.2.0b3/tart/imaging/antenna_model.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/calibration.py` & `tart-1.2.0b3/tart/imaging/calibration.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/correlator.py` & `tart-1.2.0b3/tart/imaging/correlator.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/elaz.py` & `tart-1.2.0b3/tart/imaging/elaz.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/ephemerides_proxy.py` & `tart-1.2.0b3/tart/imaging/ephemerides_proxy.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/ephemeris.py` & `tart-1.2.0b3/tart/imaging/ephemeris.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/gps_satellite.py` & `tart-1.2.0b3/tart/imaging/gps_satellite.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/gps_time.py` & `tart-1.2.0b3/tart/imaging/gps_time.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/location.py` & `tart-1.2.0b3/tart/imaging/location.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/radio_source.py` & `tart-1.2.0b3/tart/imaging/radio_source.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/simulate_transit.py` & `tart-1.2.0b3/tart/imaging/simulate_transit.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/sp3_interpolator.py` & `tart-1.2.0b3/tart/imaging/sp3_interpolator.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/sun.py` & `tart-1.2.0b3/tart/imaging/sun.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/synthesis.py` & `tart-1.2.0b3/tart/imaging/synthesis.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/tart_util.py` & `tart-1.2.0b3/tart/imaging/tart_util.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/test/all.py` & `tart-1.2.0b3/tart/imaging/test/all.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/test/test_antenna_model.py` & `tart-1.2.0b3/tart/imaging/test/test_antenna_model.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/test/test_correlator.py` & `tart-1.2.0b3/tart/imaging/test/test_correlator.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/test/test_elaz.py` & `tart-1.2.0b3/tart/imaging/test/test_elaz.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/test/test_ephemerides_proxy.py` & `tart-1.2.0b3/tart/imaging/test/test_ephemerides_proxy.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/test/test_ephemeris.py` & `tart-1.2.0b3/tart/imaging/test/test_ephemeris.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/test/test_gps_satellite.py` & `tart-1.2.0b3/tart/imaging/test/test_gps_satellite.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/test/test_gps_time.py` & `tart-1.2.0b3/tart/imaging/test/test_gps_time.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/test/test_location.py` & `tart-1.2.0b3/tart/imaging/test/test_location.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/test/test_sun.py` & `tart-1.2.0b3/tart/imaging/test/test_sun.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/test/test_visibility.py` & `tart-1.2.0b3/tart/imaging/test/test_visibility.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/uvfitsgenerator.py` & `tart-1.2.0b3/tart/imaging/uvfitsgenerator.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/imaging/visibility.py` & `tart-1.2.0b3/tart/imaging/visibility.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/operation/observation.py` & `tart-1.2.0b3/tart/operation/observation.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/operation/settings.py` & `tart-1.2.0b3/tart/operation/settings.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/operation/test/test_observation.py` & `tart-1.2.0b3/tart/operation/test/test_observation.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/operation/test/test_settings.py` & `tart-1.2.0b3/tart/operation/test/test_settings.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/antennas.py` & `tart-1.2.0b3/tart/simulation/antennas.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/butter_filter.py` & `tart-1.2.0b3/tart/simulation/butter_filter.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/calculate_delay.py` & `tart-1.2.0b3/tart/simulation/calculate_delay.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/radio.py` & `tart-1.2.0b3/tart/simulation/radio.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/sample_delay.py` & `tart-1.2.0b3/tart/simulation/sample_delay.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/sample_size.py` & `tart-1.2.0b3/tart/simulation/sample_size.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/simulation_source.py` & `tart-1.2.0b3/tart/simulation/simulation_source.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/simulator.py` & `tart-1.2.0b3/tart/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/skymodel.py` & `tart-1.2.0b3/tart/simulation/skymodel.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/spectrum.py` & `tart-1.2.0b3/tart/simulation/spectrum.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/telescope_signals.py` & `tart-1.2.0b3/tart/simulation/telescope_signals.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/telescope_system.py` & `tart-1.2.0b3/tart/simulation/telescope_system.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/test/all.py` & `tart-1.2.0b3/tart/simulation/test/all.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/test/test_antennas.py` & `tart-1.2.0b3/tart/simulation/test/test_antennas.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/test/test_radio.py` & `tart-1.2.0b3/tart/simulation/test/test_radio.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/test/test_simulated_visibility.py` & `tart-1.2.0b3/tart/simulation/test/test_simulated_visibility.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/test/test_simulation_source.py` & `tart-1.2.0b3/tart/simulation/test/test_simulation_source.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/test/test_skymodel.py` & `tart-1.2.0b3/tart/simulation/test/test_skymodel.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/test/test_util.py` & `tart-1.2.0b3/tart/simulation/test/test_util.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/simulation/util.py` & `tart-1.2.0b3/tart/simulation/util.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/test/testbench.py` & `tart-1.2.0b3/tart/test/testbench.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/util/angle.py` & `tart-1.2.0b3/tart/util/angle.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/util/db.py` & `tart-1.2.0b3/tart/util/db.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/util/hilbert.py` & `tart-1.2.0b3/tart/util/hilbert.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/util/mp.py` & `tart-1.2.0b3/tart/util/mp.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/util/nelder_mead.py` & `tart-1.2.0b3/tart/util/nelder_mead.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/util/singleton.py` & `tart-1.2.0b3/tart/util/singleton.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/util/skyloc.py` & `tart-1.2.0b3/tart/util/skyloc.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/util/test/test_angle.py` & `tart-1.2.0b3/tart/util/test/test_angle.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/util/test/test_compare_phases.py` & `tart-1.2.0b3/tart/util/test/test_compare_phases.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/util/test/test_utc.py` & `tart-1.2.0b3/tart/util/test/test_utc.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/util/utc.py` & `tart-1.2.0b3/tart/util/utc.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart/util/vector.py` & `tart-1.2.0b3/tart/util/vector.py`

 * *Files identical despite different names*

### Comparing `tart-1.2.0b1/tart.egg-info/PKG-INFO` & `tart-1.2.0b3/tart.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tart
-Version: 1.2.0b1
+Version: 1.2.0b3
 Summary: Transient Array Radio Telescope Imaging and Operation Library
-Home-page: http://github.com/tmolteno/TART
+Home-page: http://github.com/tmolteno/tart_modules
 Author: Tim Molteno
 Author-email: tim@elec.ac.nz
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Communications :: Ham Radio
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tart-1.2.0b1/tart.egg-info/SOURCES.txt` & `tart-1.2.0b3/tart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

