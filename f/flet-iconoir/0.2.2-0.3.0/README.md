# Comparing `tmp/flet_iconoir-0.2.2.tar.gz` & `tmp/flet_iconoir-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_iconoir-0.2.2.tar", max compression
+gzip compressed data, was "flet_iconoir-0.3.0.tar", max compression
```

## Comparing `flet_iconoir-0.2.2.tar` & `flet_iconoir-0.3.0.tar`

### file list

```diff
@@ -1,1593 +1,1593 @@
--rw-r--r--   0        0        0      165 2024-04-26 01:39:53.802579 flet_iconoir-0.2.2/flet_iconoir/__init__.py
--rw-r--r--   0        0        0      459 2024-04-26 02:00:33.830972 flet_iconoir-0.2.2/flet_iconoir/iconoir_icon.py
--rw-r--r--   0        0        0     1639 2024-04-26 05:19:59.640434 flet_iconoir-0.2.2/flet_iconoir/iconoir_icon_button.py
--rw-r--r--   0        0        0      363 2024-04-26 01:02:31.244683 flet_iconoir-0.2.2/flet_iconoir/icons/__init__.py
--rw-r--r--   0        0        0     1068 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/LICENSE
--rw-r--r--   0        0        0        0 2024-04-25 23:20:21.429893 flet_iconoir-0.2.2/flet_iconoir/icons/regular/__init__.py
--rw-r--r--   0        0        0      902 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/accessibility-sign.svg
--rw-r--r--   0        0        0      964 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/accessibility-tech.svg
--rw-r--r--   0        0        0      681 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/accessibility.svg
--rw-r--r--   0        0        0      230 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/activity.svg
--rw-r--r--   0        0        0      677 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/adobe-after-effects.svg
--rw-r--r--   0        0        0      677 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/adobe-illustrator.svg
--rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/adobe-indesign.svg
--rw-r--r--   0        0        0      557 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/adobe-lightroom.svg
--rw-r--r--   0        0        0      807 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/adobe-photoshop.svg
--rw-r--r--   0        0        0      623 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/adobe-xd.svg
--rw-r--r--   0        0        0      550 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/african-tree.svg
--rw-r--r--   0        0        0      667 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/agile.svg
--rw-r--r--   0        0        0      996 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/air-conditioner.svg
--rw-r--r--   0        0        0     1843 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/airplane-helix-45deg.svg
--rw-r--r--   0        0        0     1495 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/airplane-helix.svg
--rw-r--r--   0        0        0     1100 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/airplane-off.svg
--rw-r--r--   0        0        0     1580 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/airplane-rotation.svg
--rw-r--r--   0        0        0     1016 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/airplane.svg
--rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/airplay.svg
--rw-r--r--   0        0        0      596 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/alarm.svg
--rw-r--r--   0        0        0      586 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/album-carousel.svg
--rw-r--r--   0        0        0      620 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/album-list.svg
--rw-r--r--   0        0        0      756 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/album-open.svg
--rw-r--r--   0        0        0      522 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/album.svg
--rw-r--r--   0        0        0      964 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-bottom-box.svg
--rw-r--r--   0        0        0      487 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-center.svg
--rw-r--r--   0        0        0      375 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-horizontal-centers.svg
--rw-r--r--   0        0        0      461 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-horizontal-spacing.svg
--rw-r--r--   0        0        0      481 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-justify.svg
--rw-r--r--   0        0        0     1041 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-left-box.svg
--rw-r--r--   0        0        0      487 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-left.svg
--rw-r--r--   0        0        0     1027 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-right-box.svg
--rw-r--r--   0        0        0      487 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-right.svg
--rw-r--r--   0        0        0      928 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-top-box.svg
--rw-r--r--   0        0        0      372 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-vertical-centers.svg
--rw-r--r--   0        0        0      463 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-vertical-spacing.svg
--rw-r--r--   0        0        0      626 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/angle-tool.svg
--rw-r--r--   0        0        0      671 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/antenna-off.svg
--rw-r--r--   0        0        0      911 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/antenna-signal-tag.svg
--rw-r--r--   0        0        0      861 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/antenna-signal.svg
--rw-r--r--   0        0        0      776 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/antenna.svg
--rw-r--r--   0        0        0      490 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/app-notification.svg
--rw-r--r--   0        0        0      705 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/app-store.svg
--rw-r--r--   0        0        0      676 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/app-window.svg
--rw-r--r--   0        0        0      910 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple-half.svg
--rw-r--r--   0        0        0      360 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple-imac-2021-side.svg
--rw-r--r--   0        0        0      430 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple-imac-2021.svg
--rw-r--r--   0        0        0      680 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple-mac.svg
--rw-r--r--   0        0        0      675 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple-shortcuts.svg
--rw-r--r--   0        0        0     1015 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple-swift.svg
--rw-r--r--   0        0        0      574 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple-wallet.svg
--rw-r--r--   0        0        0      754 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple.svg
--rw-r--r--   0        0        0      710 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ar-tag.svg
--rw-r--r--   0        0        0      834 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arc-3d-center-point.svg
--rw-r--r--   0        0        0      694 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arc-3d.svg
--rw-r--r--   0        0        0     1053 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arcade.svg
--rw-r--r--   0        0        0      604 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/archery-match.svg
--rw-r--r--   0        0        0      476 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/archery.svg
--rw-r--r--   0        0        0      670 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/archive.svg
--rw-r--r--   0        0        0     1036 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/area-search.svg
--rw-r--r--   0        0        0      363 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-archery.svg
--rw-r--r--   0        0        0      438 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-down-circle.svg
--rw-r--r--   0        0        0      479 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-down-left-circle.svg
--rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-down-left-square.svg
--rw-r--r--   0        0        0      237 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-down-left.svg
--rw-r--r--   0        0        0      479 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-down-right-circle.svg
--rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-down-right-square.svg
--rw-r--r--   0        0        0      254 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-down-right.svg
--rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-down-tag.svg
--rw-r--r--   0        0        0      246 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-down.svg
--rw-r--r--   0        0        0      253 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-email-forward.svg
--rw-r--r--   0        0        0      507 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-enlarge-tag.svg
--rw-r--r--   0        0        0      436 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-left-circle.svg
--rw-r--r--   0        0        0      427 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-left-tag.svg
--rw-r--r--   0        0        0      244 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-left.svg
--rw-r--r--   0        0        0      532 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-reduce-tag.svg
--rw-r--r--   0        0        0      438 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-right-circle.svg
--rw-r--r--   0        0        0      427 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-right-tag.svg
--rw-r--r--   0        0        0      246 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-right.svg
--rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-separate-vertical.svg
--rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-separate.svg
--rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-union-vertical.svg
--rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-union.svg
--rw-r--r--   0        0        0      436 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-up-circle.svg
--rw-r--r--   0        0        0      479 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-up-left-circle.svg
--rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-up-left-square.svg
--rw-r--r--   0        0        0      238 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-up-left.svg
--rw-r--r--   0        0        0      479 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-up-right-circle.svg
--rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-up-right-square.svg
--rw-r--r--   0        0        0      262 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-up-right.svg
--rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-up-tag.svg
--rw-r--r--   0        0        0      244 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-up.svg
--rw-r--r--   0        0        0      433 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrows-up-from-line.svg
--rw-r--r--   0        0        0      765 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/asana.svg
--rw-r--r--   0        0        0      443 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/asterisk.svg
--rw-r--r--   0        0        0      881 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/at-sign-circle.svg
--rw-r--r--   0        0        0      667 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/at-sign.svg
--rw-r--r--   0        0        0     1016 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/atom.svg
--rw-r--r--   0        0        0      822 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/attachment.svg
--rw-r--r--   0        0        0      738 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/augmented-reality.svg
--rw-r--r--   0        0        0      393 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/auto-flash.svg
--rw-r--r--   0        0        0      750 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/avi-format.svg
--rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/axes.svg
--rw-r--r--   0        0        0      741 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/backward-15-seconds.svg
--rw-r--r--   0        0        0     1312 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/badge-check.svg
--rw-r--r--   0        0        0      507 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bag.svg
--rw-r--r--   0        0        0      914 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/balcony.svg
--rw-r--r--   0        0        0      785 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bank.svg
--rw-r--r--   0        0        0      795 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/barcode.svg
--rw-r--r--   0        0        0      805 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/basketball-field.svg
--rw-r--r--   0        0        0      960 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/basketball.svg
--rw-r--r--   0        0        0      854 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bathroom.svg
--rw-r--r--   0        0        0      574 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-25.svg
--rw-r--r--   0        0        0      577 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-50.svg
--rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-75.svg
--rw-r--r--   0        0        0      502 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-charging.svg
--rw-r--r--   0        0        0      387 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-empty.svg
--rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-full.svg
--rw-r--r--   0        0        0      594 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-indicator.svg
--rw-r--r--   0        0        0      494 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-slash.svg
--rw-r--r--   0        0        0      591 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-warning.svg
--rw-r--r--   0        0        0     1186 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bbq.svg
--rw-r--r--   0        0        0      624 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/beach-bag.svg
--rw-r--r--   0        0        0      589 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bed-ready.svg
--rw-r--r--   0        0        0      517 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bed.svg
--rw-r--r--   0        0        0     1031 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/behance-tag.svg
--rw-r--r--   0        0        0      814 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/behance.svg
--rw-r--r--   0        0        0      838 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bell-notification.svg
--rw-r--r--   0        0        0      862 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bell-off.svg
--rw-r--r--   0        0        0      678 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bell.svg
--rw-r--r--   0        0        0      909 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bicycle.svg
--rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bin-full.svg
--rw-r--r--   0        0        0     1025 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bin-half.svg
--rw-r--r--   0        0        0      767 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bin-minus-in.svg
--rw-r--r--   0        0        0      806 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bin-plus-in.svg
--rw-r--r--   0        0        0      658 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bin.svg
--rw-r--r--   0        0        0      939 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/binocular.svg
--rw-r--r--   0        0        0     1134 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/birthday-cake.svg
--rw-r--r--   0        0        0      936 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bishop.svg
--rw-r--r--   0        0        0      716 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bitbucket.svg
--rw-r--r--   0        0        0      807 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bitcoin-circle.svg
--rw-r--r--   0        0        0     1207 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bitcoin-rotate-out.svg
--rw-r--r--   0        0        0      419 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bluetooth-tag.svg
--rw-r--r--   0        0        0      251 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bluetooth.svg
--rw-r--r--   0        0        0      588 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bold-square.svg
--rw-r--r--   0        0        0      442 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bold.svg
--rw-r--r--   0        0        0      807 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bonfire.svg
--rw-r--r--   0        0        0      826 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/book-lock.svg
--rw-r--r--   0        0        0      810 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/book-stack.svg
--rw-r--r--   0        0        0      601 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/book.svg
--rw-r--r--   0        0        0      640 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bookmark-book.svg
--rw-r--r--   0        0        0      535 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bookmark-circle.svg
--rw-r--r--   0        0        0      337 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bookmark.svg
--rw-r--r--   0        0        0      943 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-bl.svg
--rw-r--r--   0        0        0     1455 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-bottom.svg
--rw-r--r--   0        0        0      961 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-br.svg
--rw-r--r--   0        0        0     1480 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-inner.svg
--rw-r--r--   0        0        0     1461 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-left.svg
--rw-r--r--   0        0        0      892 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-out.svg
--rw-r--r--   0        0        0     1499 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-right.svg
--rw-r--r--   0        0        0      946 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-tl.svg
--rw-r--r--   0        0        0     1461 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-top.svg
--rw-r--r--   0        0        0      982 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-tr.svg
--rw-r--r--   0        0        0      440 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bounce-left.svg
--rw-r--r--   0        0        0      447 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bounce-right.svg
--rw-r--r--   0        0        0      992 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bowling-ball.svg
--rw-r--r--   0        0        0     1318 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/box-3d-center.svg
--rw-r--r--   0        0        0     1046 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/box-3d-point.svg
--rw-r--r--   0        0        0     1470 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/box-3d-three-points.svg
--rw-r--r--   0        0        0      927 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/box-iso.svg
--rw-r--r--   0        0        0      463 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/box.svg
--rw-r--r--   0        0        0      796 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/boxing-glove.svg
--rw-r--r--   0        0        0     1906 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/brain-electricity.svg
--rw-r--r--   0        0        0     2150 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/brain-research.svg
--rw-r--r--   0        0        0     2085 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/brain-warning.svg
--rw-r--r--   0        0        0     2005 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/brain.svg
--rw-r--r--   0        0        0      518 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bread-slice.svg
--rw-r--r--   0        0        0      861 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bridge-3d.svg
--rw-r--r--   0        0        0      888 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bridge-surface.svg
--rw-r--r--   0        0        0     1003 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bright-crown.svg
--rw-r--r--   0        0        0     1346 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bright-star.svg
--rw-r--r--   0        0        0     1090 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/brightness-window.svg
--rw-r--r--   0        0        0      756 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/brightness.svg
--rw-r--r--   0        0        0      534 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-download.svg
--rw-r--r--   0        0        0      535 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-income.svg
--rw-r--r--   0        0        0      535 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-outcome.svg
--rw-r--r--   0        0        0      771 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-search.svg
--rw-r--r--   0        0        0      917 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-star.svg
--rw-r--r--   0        0        0      534 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-upload.svg
--rw-r--r--   0        0        0      621 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-warning.svg
--rw-r--r--   0        0        0      635 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-xmark.svg
--rw-r--r--   0        0        0     1005 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/building.svg
--rw-r--r--   0        0        0     1173 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bus-green.svg
--rw-r--r--   0        0        0      978 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bus-stop.svg
--rw-r--r--   0        0        0     1013 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/bus.svg
--rw-r--r--   0        0        0      573 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/c-square.svg
--rw-r--r--   0        0        0      408 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cable-tag.svg
--rw-r--r--   0        0        0      880 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/calculator.svg
--rw-r--r--   0        0        0      691 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/calendar-minus.svg
--rw-r--r--   0        0        0      738 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/calendar-plus.svg
--rw-r--r--   0        0        0      623 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/calendar.svg
--rw-r--r--   0        0        0      683 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/camera.svg
--rw-r--r--   0        0        0     1332 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/candlestick-chart.svg
--rw-r--r--   0        0        0      843 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/car.svg
--rw-r--r--   0        0        0      680 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/card-lock.svg
--rw-r--r--   0        0        0      654 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/card-no-access.svg
--rw-r--r--   0        0        0      487 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/card-reader.svg
--rw-r--r--   0        0        0      650 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/card-shield.svg
--rw-r--r--   0        0        0      702 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/card-wallet.svg
--rw-r--r--   0        0        0     1035 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cart-alt.svg
--rw-r--r--   0        0        0      635 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cart-minus.svg
--rw-r--r--   0        0        0      681 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cart-plus.svg
--rw-r--r--   0        0        0      875 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cart.svg
--rw-r--r--   0        0        0      743 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cash.svg
--rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cell-2x2.svg
--rw-r--r--   0        0        0      644 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cellar.svg
--rw-r--r--   0        0        0     1879 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/center-align.svg
--rw-r--r--   0        0        0      477 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-bubble-check.svg
--rw-r--r--   0        0        0      378 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-bubble-empty.svg
--rw-r--r--   0        0        0      627 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-bubble-question.svg
--rw-r--r--   0        0        0      711 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-bubble-translate.svg
--rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-bubble-warning.svg
--rw-r--r--   0        0        0      540 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-bubble-xmark.svg
--rw-r--r--   0        0        0     1110 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-bubble.svg
--rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-lines.svg
--rw-r--r--   0        0        0      474 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-minus-in.svg
--rw-r--r--   0        0        0      494 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-plus-in.svg
--rw-r--r--   0        0        0      421 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/check-circle.svg
--rw-r--r--   0        0        0      418 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/check-square.svg
--rw-r--r--   0        0        0      219 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/check.svg
--rw-r--r--   0        0        0      532 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chocolate.svg
--rw-r--r--   0        0        0     1059 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chromecast-active.svg
--rw-r--r--   0        0        0      613 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/chromecast.svg
--rw-r--r--   0        0        0      984 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/church-side.svg
--rw-r--r--   0        0        0      951 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/church.svg
--rw-r--r--   0        0        0      811 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cigarette-slash.svg
--rw-r--r--   0        0        0     1110 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cinema-old.svg
--rw-r--r--   0        0        0      485 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/circle-spark.svg
--rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/circle.svg
--rw-r--r--   0        0        0     1081 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/city.svg
--rw-r--r--   0        0        0      789 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/clipboard-check.svg
--rw-r--r--   0        0        0      562 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/clock-rotate-right.svg
--rw-r--r--   0        0        0      416 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/clock.svg
--rw-r--r--   0        0        0      776 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/closed-captions-tag.svg
--rw-r--r--   0        0        0      517 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/closet.svg
--rw-r--r--   0        0        0      464 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-bookmark.svg
--rw-r--r--   0        0        0      449 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-check.svg
--rw-r--r--   0        0        0      999 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-desync.svg
--rw-r--r--   0        0        0      472 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-download.svg
--rw-r--r--   0        0        0      556 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-square.svg
--rw-r--r--   0        0        0      962 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-sunny.svg
--rw-r--r--   0        0        0      999 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-sync.svg
--rw-r--r--   0        0        0      472 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-upload.svg
--rw-r--r--   0        0        0      498 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-xmark.svg
--rw-r--r--   0        0        0      306 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud.svg
--rw-r--r--   0        0        0     1032 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/code-brackets-square.svg
--rw-r--r--   0        0        0      707 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/code-brackets.svg
--rw-r--r--   0        0        0      430 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/code.svg
--rw-r--r--   0        0        0      701 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/codepen.svg
--rw-r--r--   0        0        0      801 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/coffee-cup.svg
--rw-r--r--   0        0        0     1144 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/coin-slash.svg
--rw-r--r--   0        0        0      841 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/coins-swap.svg
--rw-r--r--   0        0        0     1376 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/coins.svg
--rw-r--r--   0        0        0      439 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/collage-frame.svg
--rw-r--r--   0        0        0      550 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/collapse.svg
--rw-r--r--   0        0        0      759 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/color-filter.svg
--rw-r--r--   0        0        0      920 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/color-picker.svg
--rw-r--r--   0        0        0     1324 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/color-wheel.svg
--rw-r--r--   0        0        0      562 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/combine.svg
--rw-r--r--   0        0        0      944 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/commodity.svg
--rw-r--r--   0        0        0     1100 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/community.svg
--rw-r--r--   0        0        0      372 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/comp-align-bottom.svg
--rw-r--r--   0        0        0      371 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/comp-align-left.svg
--rw-r--r--   0        0        0      372 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/comp-align-right.svg
--rw-r--r--   0        0        0      370 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/comp-align-top.svg
--rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/compact-disc.svg
--rw-r--r--   0        0        0      481 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/compass.svg
--rw-r--r--   0        0        0     1336 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/component.svg
--rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/compress-lines.svg
--rw-r--r--   0        0        0      437 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/compress.svg
--rw-r--r--   0        0        0      501 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/computer.svg
--rw-r--r--   0        0        0     1753 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/constrained-surface.svg
--rw-r--r--   0        0        0      948 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/consumable.svg
--rw-r--r--   0        0        0      569 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/contactless.svg
--rw-r--r--   0        0        0      500 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/control-slider.svg
--rw-r--r--   0        0        0     1249 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cookie.svg
--rw-r--r--   0        0        0      507 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cooling-square.svg
--rw-r--r--   0        0        0      527 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/copy.svg
--rw-r--r--   0        0        0      545 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/copyright.svg
--rw-r--r--   0        0        0     1481 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/corner-bottom-left.svg
--rw-r--r--   0        0        0     1447 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/corner-bottom-right.svg
--rw-r--r--   0        0        0     1366 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/corner-top-left.svg
--rw-r--r--   0        0        0     1432 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/corner-top-right.svg
--rw-r--r--   0        0        0     1501 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cpu-warning.svg
--rw-r--r--   0        0        0     1638 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cpu.svg
--rw-r--r--   0        0        0      427 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cracked-egg.svg
--rw-r--r--   0        0        0      781 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/creative-commons.svg
--rw-r--r--   0        0        0      608 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/credit-card-slash.svg
--rw-r--r--   0        0        0      333 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/credit-card.svg
--rw-r--r--   0        0        0      569 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/credit-cards.svg
--rw-r--r--   0        0        0     1158 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/crib.svg
--rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/crop-rotate-bl.svg
--rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/crop-rotate-br.svg
--rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/crop-rotate-tl.svg
--rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/crop-rotate-tr.svg
--rw-r--r--   0        0        0      306 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/crop.svg
--rw-r--r--   0        0        0      464 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/crown-circle.svg
--rw-r--r--   0        0        0      254 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/crown.svg
--rw-r--r--   0        0        0      470 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/css3.svg
--rw-r--r--   0        0        0     1398 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cube-bandage.svg
--rw-r--r--   0        0        0     1095 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cube-cut-with-curve.svg
--rw-r--r--   0        0        0      991 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cube-hole.svg
--rw-r--r--   0        0        0      883 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cube-replace-face.svg
--rw-r--r--   0        0        0      834 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cube.svg
--rw-r--r--   0        0        0      437 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cursor-pointer.svg
--rw-r--r--   0        0        0      918 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/curve-array.svg
--rw-r--r--   0        0        0      816 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cut.svg
--rw-r--r--   0        0        0      715 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cutlery.svg
--rw-r--r--   0        0        0      862 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cycling.svg
--rw-r--r--   0        0        0      506 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/cylinder.svg
--rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dash-flag.svg
--rw-r--r--   0        0        0     1363 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dashboard-dots.svg
--rw-r--r--   0        0        0     1101 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dashboard-speed.svg
--rw-r--r--   0        0        0      760 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dashboard.svg
--rw-r--r--   0        0        0      342 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/data-transfer-both.svg
--rw-r--r--   0        0        0      442 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/data-transfer-check.svg
--rw-r--r--   0        0        0      530 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/data-transfer-down.svg
--rw-r--r--   0        0        0      524 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/data-transfer-up.svg
--rw-r--r--   0        0        0      723 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/data-transfer-warning.svg
--rw-r--r--   0        0        0     1293 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-backup.svg
--rw-r--r--   0        0        0      596 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-check.svg
--rw-r--r--   0        0        0      611 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-export.svg
--rw-r--r--   0        0        0      638 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-monitor.svg
--rw-r--r--   0        0        0      611 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-restore.svg
--rw-r--r--   0        0        0      575 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-script-minus.svg
--rw-r--r--   0        0        0      627 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-script-plus.svg
--rw-r--r--   0        0        0      502 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-script.svg
--rw-r--r--   0        0        0      853 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-search.svg
--rw-r--r--   0        0        0     1009 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-settings.svg
--rw-r--r--   0        0        0      984 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-star.svg
--rw-r--r--   0        0        0      697 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-stats.svg
--rw-r--r--   0        0        0      742 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-tag.svg
--rw-r--r--   0        0        0      695 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-warning.svg
--rw-r--r--   0        0        0      702 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-xmark.svg
--rw-r--r--   0        0        0      433 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/database.svg
--rw-r--r--   0        0        0      437 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/de-compress.svg
--rw-r--r--   0        0        0     1151 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/delivery-truck.svg
--rw-r--r--   0        0        0      496 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/delivery.svg
--rw-r--r--   0        0        0     1090 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/depth.svg
--rw-r--r--   0        0        0     1180 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/design-nib.svg
--rw-r--r--   0        0        0      608 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/design-pencil.svg
--rw-r--r--   0        0        0      862 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/desk.svg
--rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/developer.svg
--rw-r--r--   0        0        0     1279 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dew-point.svg
--rw-r--r--   0        0        0     2397 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dialpad.svg
--rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/diameter.svg
--rw-r--r--   0        0        0     1436 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dice-five.svg
--rw-r--r--   0        0        0     1188 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dice-four.svg
--rw-r--r--   0        0        0      544 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dice-one.svg
--rw-r--r--   0        0        0     1663 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dice-six.svg
--rw-r--r--   0        0        0      990 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dice-three.svg
--rw-r--r--   0        0        0      742 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dice-two.svg
--rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dimmer-switch.svg
--rw-r--r--   0        0        0      718 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/director-chair.svg
--rw-r--r--   0        0        0     1079 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/discord.svg
--rw-r--r--   0        0        0      940 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dishwasher.svg
--rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/display-4k.svg
--rw-r--r--   0        0        0      932 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/divide-three.svg
--rw-r--r--   0        0        0      669 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/divide.svg
--rw-r--r--   0        0        0      744 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dna.svg
--rw-r--r--   0        0        0     1249 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dns.svg
--rw-r--r--   0        0        0      907 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/doc-magnifying-glass-in.svg
--rw-r--r--   0        0        0      844 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/doc-magnifying-glass.svg
--rw-r--r--   0        0        0     1022 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/doc-star-in.svg
--rw-r--r--   0        0        0      988 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/doc-star.svg
--rw-r--r--   0        0        0      630 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dogecoin-circle.svg
--rw-r--r--   0        0        0     1030 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dogecoin-rotate-out.svg
--rw-r--r--   0        0        0      633 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dollar-circle.svg
--rw-r--r--   0        0        0      499 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dollar.svg
--rw-r--r--   0        0        0      621 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/domotic-warning.svg
--rw-r--r--   0        0        0     1620 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/donate.svg
--rw-r--r--   0        0        0      430 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dot-arrow-down.svg
--rw-r--r--   0        0        0      432 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dot-arrow-left.svg
--rw-r--r--   0        0        0      427 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dot-arrow-right.svg
--rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dot-arrow-up.svg
--rw-r--r--   0        0        0      459 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/double-check.svg
--rw-r--r--   0        0        0      529 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/download-circle.svg
--rw-r--r--   0        0        0      796 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/download-data-window.svg
--rw-r--r--   0        0        0      528 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/download-square.svg
--rw-r--r--   0        0        0      336 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/download.svg
--rw-r--r--   0        0        0     1610 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/drag-hand-gesture.svg
--rw-r--r--   0        0        0      554 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/drag.svg
--rw-r--r--   0        0        0      978 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/drawer.svg
--rw-r--r--   0        0        0      723 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/dribbble.svg
--rw-r--r--   0        0        0     1871 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-charge-full.svg
--rw-r--r--   0        0        0     1780 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-charge-half.svg
--rw-r--r--   0        0        0     1689 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-charge-low.svg
--rw-r--r--   0        0        0     1562 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-check.svg
--rw-r--r--   0        0        0     1587 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-landing.svg
--rw-r--r--   0        0        0     1977 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-refresh.svg
--rw-r--r--   0        0        0     1587 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-take-off.svg
--rw-r--r--   0        0        0     1652 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-xmark.svg
--rw-r--r--   0        0        0     1696 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone.svg
--rw-r--r--   0        0        0      529 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/droplet-check.svg
--rw-r--r--   0        0        0      312 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/droplet-half.svg
--rw-r--r--   0        0        0      260 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/droplet.svg
--rw-r--r--   0        0        0      809 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ease-curve-control-points.svg
--rw-r--r--   0        0        0      526 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ease-in-control-point.svg
--rw-r--r--   0        0        0      225 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ease-in-out.svg
--rw-r--r--   0        0        0      225 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ease-in.svg
--rw-r--r--   0        0        0      507 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ease-out-control-point.svg
--rw-r--r--   0        0        0      224 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ease-out.svg
--rw-r--r--   0        0        0      975 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ecology-book.svg
--rw-r--r--   0        0        0      614 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/edit-pencil.svg
--rw-r--r--   0        0        0      565 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/edit.svg
--rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/egg.svg
--rw-r--r--   0        0        0      942 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/eject.svg
--rw-r--r--   0        0        0     1268 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/electronics-chip.svg
--rw-r--r--   0        0        0      350 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/electronics-transistor.svg
--rw-r--r--   0        0        0      636 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/elevator.svg
--rw-r--r--   0        0        0     1281 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ellipse-3d-three-points.svg
--rw-r--r--   0        0        0      750 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ellipse-3d.svg
--rw-r--r--   0        0        0      339 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-ball.svg
--rw-r--r--   0        0        0      688 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-blink-left.svg
--rw-r--r--   0        0        0      681 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-blink-right.svg
--rw-r--r--   0        0        0      779 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-look-down.svg
--rw-r--r--   0        0        0      587 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-look-left.svg
--rw-r--r--   0        0        0      600 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-look-right.svg
--rw-r--r--   0        0        0      761 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-look-up.svg
--rw-r--r--   0        0        0     1126 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-puzzled.svg
--rw-r--r--   0        0        0      760 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-quite.svg
--rw-r--r--   0        0        0      339 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-really.svg
--rw-r--r--   0        0        0      895 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-sad.svg
--rw-r--r--   0        0        0      474 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-satisfied.svg
--rw-r--r--   0        0        0     1349 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-sing-left-note.svg
--rw-r--r--   0        0        0      947 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-sing-left.svg
--rw-r--r--   0        0        0     1376 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-sing-right-note.svg
--rw-r--r--   0        0        0     1388 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-sing-right.svg
--rw-r--r--   0        0        0      953 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-surprise-alt.svg
--rw-r--r--   0        0        0      973 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-surprise.svg
--rw-r--r--   0        0        0      397 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-talking-angry.svg
--rw-r--r--   0        0        0      397 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-talking-happy.svg
--rw-r--r--   0        0        0      759 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-think-left.svg
--rw-r--r--   0        0        0      761 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-think-right.svg
--rw-r--r--   0        0        0      895 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji.svg
--rw-r--r--   0        0        0      534 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/empty-page.svg
--rw-r--r--   0        0        0      789 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/energy-usage-window.svg
--rw-r--r--   0        0        0      336 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/enlarge.svg
--rw-r--r--   0        0        0      707 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/erase.svg
--rw-r--r--   0        0        0      471 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ethereum-circle.svg
--rw-r--r--   0        0        0      871 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ethereum-rotate-out.svg
--rw-r--r--   0        0        0      718 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/euro-square.svg
--rw-r--r--   0        0        0      520 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/euro.svg
--rw-r--r--   0        0        0      838 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-charge-alt.svg
--rw-r--r--   0        0        0      667 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-charge.svg
--rw-r--r--   0        0        0      698 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-plug-charging.svg
--rw-r--r--   0        0        0      791 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-plug-xmark.svg
--rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-plug.svg
--rw-r--r--   0        0        0      618 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-station.svg
--rw-r--r--   0        0        0      589 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-tag.svg
--rw-r--r--   0        0        0      890 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/exclude.svg
--rw-r--r--   0        0        0      529 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/expand-lines.svg
--rw-r--r--   0        0        0      550 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/expand.svg
--rw-r--r--   0        0        0      947 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/extrude.svg
--rw-r--r--   0        0        0      532 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/eye-closed.svg
--rw-r--r--   0        0        0      426 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/eye.svg
--rw-r--r--   0        0        0      529 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/f-square.svg
--rw-r--r--   0        0        0     1030 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/face-3d-draft.svg
--rw-r--r--   0        0        0      999 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/face-id.svg
--rw-r--r--   0        0        0      545 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/facebook-tag.svg
--rw-r--r--   0        0        0      397 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/facebook.svg
--rw-r--r--   0        0        0      697 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/facetime.svg
--rw-r--r--   0        0        0      532 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/farm.svg
--rw-r--r--   0        0        0      526 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-arrow-down-square.svg
--rw-r--r--   0        0        0      318 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-arrow-down.svg
--rw-r--r--   0        0        0      527 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-arrow-left-square.svg
--rw-r--r--   0        0        0      319 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-arrow-left.svg
--rw-r--r--   0        0        0      522 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-arrow-right-square.svg
--rw-r--r--   0        0        0      318 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-arrow-right.svg
--rw-r--r--   0        0        0      527 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-arrow-up-square.svg
--rw-r--r--   0        0        0      319 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-arrow-up.svg
--rw-r--r--   0        0        0      529 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-down-circle.svg
--rw-r--r--   0        0        0      530 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-left-circle.svg
--rw-r--r--   0        0        0      525 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-right-circle.svg
--rw-r--r--   0        0        0      530 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-up-circle.svg
--rw-r--r--   0        0        0     1002 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/favourite-book.svg
--rw-r--r--   0        0        0     1140 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/favourite-window.svg
--rw-r--r--   0        0        0      351 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/female.svg
--rw-r--r--   0        0        0     2104 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/figma.svg
--rw-r--r--   0        0        0      869 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/file-not-found.svg
--rw-r--r--   0        0        0      844 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fill-color.svg
--rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fillet-3d.svg
--rw-r--r--   0        0        0      565 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/filter-alt.svg
--rw-r--r--   0        0        0      595 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/filter-list-circle.svg
--rw-r--r--   0        0        0      398 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/filter-list.svg
--rw-r--r--   0        0        0      674 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/filter.svg
--rw-r--r--   0        0        0      789 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/finder.svg
--rw-r--r--   0        0        0      854 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-check-circle.svg
--rw-r--r--   0        0        0      734 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-circle.svg
--rw-r--r--   0        0        0     1154 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-lock-circle.svg
--rw-r--r--   0        0        0      907 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-scan.svg
--rw-r--r--   0        0        0      759 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-square.svg
--rw-r--r--   0        0        0     1092 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-window.svg
--rw-r--r--   0        0        0      948 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-xmark-circle.svg
--rw-r--r--   0        0        0     1165 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint.svg
--rw-r--r--   0        0        0      502 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fire-flame.svg
--rw-r--r--   0        0        0      668 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fish.svg
--rw-r--r--   0        0        0      365 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fishing.svg
--rw-r--r--   0        0        0      709 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/flare.svg
--rw-r--r--   0        0        0      365 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/flash-off.svg
--rw-r--r--   0        0        0      233 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/flash.svg
--rw-r--r--   0        0        0      867 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/flask.svg
--rw-r--r--   0        0        0      717 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/flip-reverse.svg
--rw-r--r--   0        0        0      724 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/flip.svg
--rw-r--r--   0        0        0      942 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/floppy-disk-arrow-in.svg
--rw-r--r--   0        0        0      884 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/floppy-disk-arrow-out.svg
--rw-r--r--   0        0        0      691 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/floppy-disk.svg
--rw-r--r--   0        0        0     2393 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/flower.svg
--rw-r--r--   0        0        0      623 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fog.svg
--rw-r--r--   0        0        0      632 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/folder-minus.svg
--rw-r--r--   0        0        0      651 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/folder-plus.svg
--rw-r--r--   0        0        0     1172 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/folder-settings.svg
--rw-r--r--   0        0        0      703 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/folder-warning.svg
--rw-r--r--   0        0        0      460 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/folder.svg
--rw-r--r--   0        0        0      646 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/font-question.svg
--rw-r--r--   0        0        0     1012 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/football-ball.svg
--rw-r--r--   0        0        0      709 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/football.svg
--rw-r--r--   0        0        0      743 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/forward-15-seconds.svg
--rw-r--r--   0        0        0      546 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/forward-message.svg
--rw-r--r--   0        0        0      649 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/forward.svg
--rw-r--r--   0        0        0      490 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame-alt-empty.svg
--rw-r--r--   0        0        0      700 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame-alt.svg
--rw-r--r--   0        0        0     1300 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame-minus-in.svg
--rw-r--r--   0        0        0     1326 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame-plus-in.svg
--rw-r--r--   0        0        0     1620 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame-select.svg
--rw-r--r--   0        0        0     1209 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame-simple.svg
--rw-r--r--   0        0        0      402 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame-tool.svg
--rw-r--r--   0        0        0     2373 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame.svg
--rw-r--r--   0        0        0      515 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fridge.svg
--rw-r--r--   0        0        0      627 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fx-tag.svg
--rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/fx.svg
--rw-r--r--   0        0        0     1456 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/gamepad.svg
--rw-r--r--   0        0        0      305 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/garage.svg
--rw-r--r--   0        0        0     1069 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/gas-tank-droplet.svg
--rw-r--r--   0        0        0      916 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/gas-tank.svg
--rw-r--r--   0        0        0      454 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/gas.svg
--rw-r--r--   0        0        0      784 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/gif-format.svg
--rw-r--r--   0        0        0     1103 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/gift.svg
--rw-r--r--   0        0        0      709 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-branch.svg
--rw-r--r--   0        0        0      662 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-cherry-pick-commit.svg
--rw-r--r--   0        0        0      500 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-commit.svg
--rw-r--r--   0        0        0      957 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-compare.svg
--rw-r--r--   0        0        0      912 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-fork.svg
--rw-r--r--   0        0        0      708 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-merge.svg
--rw-r--r--   0        0        0      899 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-pull-request-closed.svg
--rw-r--r--   0        0        0     1025 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-pull-request.svg
--rw-r--r--   0        0        0     1152 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/github-circle.svg
--rw-r--r--   0        0        0      945 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/github.svg
--rw-r--r--   0        0        0      718 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/gitlab-full.svg
--rw-r--r--   0        0        0      754 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/glass-empty.svg
--rw-r--r--   0        0        0      594 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/glass-fragile.svg
--rw-r--r--   0        0        0      963 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/glass-half-alt.svg
--rw-r--r--   0        0        0      936 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/glass-half.svg
--rw-r--r--   0        0        0      624 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/glasses.svg
--rw-r--r--   0        0        0      807 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/globe.svg
--rw-r--r--   0        0        0      538 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/golf.svg
--rw-r--r--   0        0        0      522 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-circle.svg
--rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-docs.svg
--rw-r--r--   0        0        0      473 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-drive-check.svg
--rw-r--r--   0        0        0     1016 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-drive-sync.svg
--rw-r--r--   0        0        0      572 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-drive-warning.svg
--rw-r--r--   0        0        0      402 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-drive.svg
--rw-r--r--   0        0        0      738 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-home.svg
--rw-r--r--   0        0        0      647 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-one.svg
--rw-r--r--   0        0        0      529 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/google.svg
--rw-r--r--   0        0        0      799 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/gps.svg
--rw-r--r--   0        0        0      852 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/graduation-cap.svg
--rw-r--r--   0        0        0      322 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/graph-down.svg
--rw-r--r--   0        0        0      323 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/graph-up.svg
--rw-r--r--   0        0        0      808 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/grid-minus.svg
--rw-r--r--   0        0        0      847 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/grid-plus.svg
--rw-r--r--   0        0        0      887 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/grid-xmark.svg
--rw-r--r--   0        0        0      754 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/group.svg
--rw-r--r--   0        0        0     1092 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/gym.svg
--rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/h-square.svg
--rw-r--r--   0        0        0     1633 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/half-cookie.svg
--rw-r--r--   0        0        0      363 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/half-moon.svg
--rw-r--r--   0        0        0      617 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hammer.svg
--rw-r--r--   0        0        0      724 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hand-brake.svg
--rw-r--r--   0        0        0      723 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hand-card.svg
--rw-r--r--   0        0        0     1043 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hand-cash.svg
--rw-r--r--   0        0        0      869 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hand-contactless.svg
--rw-r--r--   0        0        0      418 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/handbag.svg
--rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hard-drive.svg
--rw-r--r--   0        0        0      394 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hashtag.svg
--rw-r--r--   0        0        0      377 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hat.svg
--rw-r--r--   0        0        0      567 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hd-display.svg
--rw-r--r--   0        0        0      380 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hd.svg
--rw-r--r--   0        0        0      669 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hdr.svg
--rw-r--r--   0        0        0      827 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/headset-bolt.svg
--rw-r--r--   0        0        0      916 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/headset-help.svg
--rw-r--r--   0        0        0      917 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/headset-warning.svg
--rw-r--r--   0        0        0      720 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/headset.svg
--rw-r--r--   0        0        0      637 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/health-shield.svg
--rw-r--r--   0        0        0     1326 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/healthcare.svg
--rw-r--r--   0        0        0      830 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/heart-arrow-down.svg
--rw-r--r--   0        0        0      590 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/heart.svg
--rw-r--r--   0        0        0      799 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/heating-square.svg
--rw-r--r--   0        0        0      622 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/heavy-rain.svg
--rw-r--r--   0        0        0      566 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/help-circle.svg
--rw-r--r--   0        0        0      563 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/help-square.svg
--rw-r--r--   0        0        0      653 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/heptagon.svg
--rw-r--r--   0        0        0     1207 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hexagon-dice.svg
--rw-r--r--   0        0        0      683 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hexagon-plus.svg
--rw-r--r--   0        0        0      567 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hexagon.svg
--rw-r--r--   0        0        0      626 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/historic-shield-alt.svg
--rw-r--r--   0        0        0      440 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/historic-shield.svg
--rw-r--r--   0        0        0      517 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-alt-slim-horiz.svg
--rw-r--r--   0        0        0      517 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-alt-slim.svg
--rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-alt.svg
--rw-r--r--   0        0        0      548 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-hospital.svg
--rw-r--r--   0        0        0      824 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-sale.svg
--rw-r--r--   0        0        0      720 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-secure.svg
--rw-r--r--   0        0        0      763 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-shield.svg
--rw-r--r--   0        0        0      516 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-simple-door.svg
--rw-r--r--   0        0        0      528 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-simple.svg
--rw-r--r--   0        0        0      490 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-table.svg
--rw-r--r--   0        0        0      900 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-temperature-in.svg
--rw-r--r--   0        0        0      980 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-temperature-out.svg
--rw-r--r--   0        0        0      544 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-user.svg
--rw-r--r--   0        0        0      426 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/home.svg
--rw-r--r--   0        0        0      476 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/horiz-distribution-left.svg
--rw-r--r--   0        0        0      481 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/horiz-distribution-right.svg
--rw-r--r--   0        0        0      549 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/horizontal-merge.svg
--rw-r--r--   0        0        0      547 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/horizontal-split.svg
--rw-r--r--   0        0        0      464 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hospital-circle.svg
--rw-r--r--   0        0        0     1207 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hospital.svg
--rw-r--r--   0        0        0      775 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hot-air-balloon.svg
--rw-r--r--   0        0        0      519 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/hourglass.svg
--rw-r--r--   0        0        0      899 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/house-rooms.svg
--rw-r--r--   0        0        0      386 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/html5.svg
--rw-r--r--   0        0        0      594 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ice-cream.svg
--rw-r--r--   0        0        0      523 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/iconoir.svg
--rw-r--r--   0        0        0      396 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/import.svg
--rw-r--r--   0        0        0      380 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/inclination.svg
--rw-r--r--   0        0        0      562 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/industry.svg
--rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/infinite.svg
--rw-r--r--   0        0        0      516 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/info-circle.svg
--rw-r--r--   0        0        0      460 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/input-field.svg
--rw-r--r--   0        0        0      426 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/input-output.svg
--rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/input-search.svg
--rw-r--r--   0        0        0      597 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/instagram.svg
--rw-r--r--   0        0        0     1079 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/internet.svg
--rw-r--r--   0        0        0     1890 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/intersect-alt.svg
--rw-r--r--   0        0        0     1344 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/intersect.svg
--rw-r--r--   0        0        0     1044 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ios-settings.svg
--rw-r--r--   0        0        0      630 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ip-address-tag.svg
--rw-r--r--   0        0        0      904 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/iris-scan.svg
--rw-r--r--   0        0        0      450 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/italic-square.svg
--rw-r--r--   0        0        0      258 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/italic.svg
--rw-r--r--   0        0        0     1152 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/jellyfish.svg
--rw-r--r--   0        0        0     1001 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/journal-page.svg
--rw-r--r--   0        0        0      809 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/journal.svg
--rw-r--r--   0        0        0      908 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/jpeg-format.svg
--rw-r--r--   0        0        0      721 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/jpg-format.svg
--rw-r--r--   0        0        0      711 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/kanban-board.svg
--rw-r--r--   0        0        0      421 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/key-back.svg
--rw-r--r--   0        0        0      792 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/key-command.svg
--rw-r--r--   0        0        0      677 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/key-minus.svg
--rw-r--r--   0        0        0      716 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/key-plus.svg
--rw-r--r--   0        0        0      758 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/key-xmark.svg
--rw-r--r--   0        0        0      418 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/key.svg
--rw-r--r--   0        0        0      837 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-align-center.svg
--rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-align-horizontal.svg
--rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-align-vertical.svg
--rw-r--r--   0        0        0      561 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-minus-in.svg
--rw-r--r--   0        0        0      566 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-minus.svg
--rw-r--r--   0        0        0      584 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-plus-in.svg
--rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-plus.svg
--rw-r--r--   0        0        0      584 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-position.svg
--rw-r--r--   0        0        0      468 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe.svg
--rw-r--r--   0        0        0      764 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframes-couple.svg
--rw-r--r--   0        0        0      812 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframes-minus.svg
--rw-r--r--   0        0        0      832 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframes-plus.svg
--rw-r--r--   0        0        0      782 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframes.svg
--rw-r--r--   0        0        0      414 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/label.svg
--rw-r--r--   0        0        0      272 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/lamp.svg
--rw-r--r--   0        0        0      836 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/language.svg
--rw-r--r--   0        0        0      613 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/laptop-charging.svg
--rw-r--r--   0        0        0      678 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/laptop-dev-mode.svg
--rw-r--r--   0        0        0     1135 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/laptop-fix.svg
--rw-r--r--   0        0        0      696 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/laptop-warning.svg
--rw-r--r--   0        0        0      502 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/laptop.svg
--rw-r--r--   0        0        0      444 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/layout-left.svg
--rw-r--r--   0        0        0      452 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/layout-right.svg
--rw-r--r--   0        0        0     1173 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/leaderboard-star.svg
--rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/leaderboard.svg
--rw-r--r--   0        0        0      550 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/leaf.svg
--rw-r--r--   0        0        0      978 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/learning.svg
--rw-r--r--   0        0        0      757 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/lens-plus.svg
--rw-r--r--   0        0        0      591 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/lens.svg
--rw-r--r--   0        0        0      931 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/lifebelt.svg
--rw-r--r--   0        0        0      802 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/light-bulb-off.svg
--rw-r--r--   0        0        0      993 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/light-bulb-on.svg
--rw-r--r--   0        0        0      618 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/light-bulb.svg
--rw-r--r--   0        0        0      523 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/line-space.svg
--rw-r--r--   0        0        0      214 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/linear.svg
--rw-r--r--   0        0        0      896 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/link-slash.svg
--rw-r--r--   0        0        0      961 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/link-xmark.svg
--rw-r--r--   0        0        0      710 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/link.svg
--rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/linkedin.svg
--rw-r--r--   0        0        0     1215 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/linux.svg
--rw-r--r--   0        0        0      725 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/list-select.svg
--rw-r--r--   0        0        0      707 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/list.svg
--rw-r--r--   0        0        0      519 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/litecoin-circle.svg
--rw-r--r--   0        0        0      919 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/litecoin-rotate-out.svg
--rw-r--r--   0        0        0      783 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/lock-slash.svg
--rw-r--r--   0        0        0      638 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/lock-square.svg
--rw-r--r--   0        0        0      409 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/lock.svg
--rw-r--r--   0        0        0      502 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/loft-3d.svg
--rw-r--r--   0        0        0      440 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/log-in.svg
--rw-r--r--   0        0        0      653 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/log-no-access.svg
--rw-r--r--   0        0        0      440 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/log-out.svg
--rw-r--r--   0        0        0      383 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/long-arrow-down-left.svg
--rw-r--r--   0        0        0      383 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/long-arrow-down-right.svg
--rw-r--r--   0        0        0      346 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/long-arrow-left-down.svg
--rw-r--r--   0        0        0      346 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/long-arrow-left-up.svg
--rw-r--r--   0        0        0      355 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/long-arrow-right-down.svg
--rw-r--r--   0        0        0      355 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/long-arrow-right-up.svg
--rw-r--r--   0        0        0      385 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/long-arrow-up-left.svg
--rw-r--r--   0        0        0      390 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/long-arrow-up-right.svg
--rw-r--r--   0        0        0      931 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/lot-of-cash.svg
--rw-r--r--   0        0        0      586 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/lullaby.svg
--rw-r--r--   0        0        0      395 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mac-control-key.svg
--rw-r--r--   0        0        0     1223 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mac-dock.svg
--rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mac-option-key.svg
--rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mac-os-window.svg
--rw-r--r--   0        0        0      538 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/magic-wand.svg
--rw-r--r--   0        0        0      895 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/magnet-energy.svg
--rw-r--r--   0        0        0      647 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/magnet.svg
--rw-r--r--   0        0        0      484 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mail-in.svg
--rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mail-open.svg
--rw-r--r--   0        0        0      484 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mail-out.svg
--rw-r--r--   0        0        0      395 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mail.svg
--rw-r--r--   0        0        0      411 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/male.svg
--rw-r--r--   0        0        0      581 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/map-pin-minus.svg
--rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/map-pin-plus.svg
--rw-r--r--   0        0        0      677 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/map-pin-xmark.svg
--rw-r--r--   0        0        0      497 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/map-pin.svg
--rw-r--r--   0        0        0      794 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/map-xmark.svg
--rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/map.svg
--rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/maps-arrow-diagonal.svg
--rw-r--r--   0        0        0      626 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/maps-arrow-xmark.svg
--rw-r--r--   0        0        0      477 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/maps-arrow.svg
--rw-r--r--   0        0        0      588 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/maps-go-straight.svg
--rw-r--r--   0        0        0      793 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/maps-turn-back.svg
--rw-r--r--   0        0        0      702 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/maps-turn-left.svg
--rw-r--r--   0        0        0      711 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/maps-turn-right.svg
--rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mask-square.svg
--rw-r--r--   0        0        0      793 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mastercard-card.svg
--rw-r--r--   0        0        0      727 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mastodon.svg
--rw-r--r--   0        0        0      812 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/math-book.svg
--rw-r--r--   0        0        0      490 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/maximize.svg
--rw-r--r--   0        0        0      506 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/medal-1st.svg
--rw-r--r--   0        0        0      401 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/medal.svg
--rw-r--r--   0        0        0      870 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-image-folder.svg
--rw-r--r--   0        0        0      783 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-image-list.svg
--rw-r--r--   0        0        0      729 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-image-plus.svg
--rw-r--r--   0        0        0      782 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-image-xmark.svg
--rw-r--r--   0        0        0      640 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-image.svg
--rw-r--r--   0        0        0      921 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-video-folder.svg
--rw-r--r--   0        0        0      733 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-video-list.svg
--rw-r--r--   0        0        0      693 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-video-plus.svg
--rw-r--r--   0        0        0      745 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-video-xmark.svg
--rw-r--r--   0        0        0      608 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-video.svg
--rw-r--r--   0        0        0      710 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/medium.svg
--rw-r--r--   0        0        0      537 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/megaphone.svg
--rw-r--r--   0        0        0      391 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/menu-scale.svg
--rw-r--r--   0        0        0      391 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/menu.svg
--rw-r--r--   0        0        0      570 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/message-alert.svg
--rw-r--r--   0        0        0      560 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/message-text.svg
--rw-r--r--   0        0        0      376 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/message.svg
--rw-r--r--   0        0        0      668 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/meter-arrow-down-right.svg
--rw-r--r--   0        0        0     1285 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/metro.svg
--rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone-check.svg
--rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone-minus.svg
--rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone-mute.svg
--rw-r--r--   0        0        0      615 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone-plus.svg
--rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone-speaking.svg
--rw-r--r--   0        0        0      670 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone-warning.svg
--rw-r--r--   0        0        0      471 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone.svg
--rw-r--r--   0        0        0      933 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/microscope.svg
--rw-r--r--   0        0        0      407 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/minus-circle.svg
--rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/minus-hexagon.svg
--rw-r--r--   0        0        0      945 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/minus-square-dashed.svg
--rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/minus-square.svg
--rw-r--r--   0        0        0      212 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/minus.svg
--rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mirror.svg
--rw-r--r--   0        0        0      699 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mobile-dev-mode.svg
--rw-r--r--   0        0        0      827 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mobile-fingerprint.svg
--rw-r--r--   0        0        0      875 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mobile-voice.svg
--rw-r--r--   0        0        0      698 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/modern-tv-4k.svg
--rw-r--r--   0        0        0      407 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/modern-tv.svg
--rw-r--r--   0        0        0      630 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/money-square.svg
--rw-r--r--   0        0        0      879 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/moon-sat.svg
--rw-r--r--   0        0        0     1049 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/more-horiz-circle.svg
--rw-r--r--   0        0        0      854 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/more-horiz.svg
--rw-r--r--   0        0        0     1049 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/more-vert-circle.svg
--rw-r--r--   0        0        0      854 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/more-vert.svg
--rw-r--r--   0        0        0      950 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/motorcycle.svg
--rw-r--r--   0        0        0      398 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mouse-button-left.svg
--rw-r--r--   0        0        0      397 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mouse-button-right.svg
--rw-r--r--   0        0        0     1592 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mouse-scroll-wheel.svg
--rw-r--r--   0        0        0     1016 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/movie.svg
--rw-r--r--   0        0        0      930 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/mpeg-format.svg
--rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/multi-bubble.svg
--rw-r--r--   0        0        0     1065 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/multi-mac-os-window.svg
--rw-r--r--   0        0        0      623 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/multi-window.svg
--rw-r--r--   0        0        0      637 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/multiple-pages-empty.svg
--rw-r--r--   0        0        0      714 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/multiple-pages-minus.svg
--rw-r--r--   0        0        0      753 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/multiple-pages-plus.svg
--rw-r--r--   0        0        0      795 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/multiple-pages-xmark.svg
--rw-r--r--   0        0        0      919 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/multiple-pages.svg
--rw-r--r--   0        0        0      803 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/music-double-note-plus.svg
--rw-r--r--   0        0        0      580 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/music-double-note.svg
--rw-r--r--   0        0        0      440 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/music-note-plus.svg
--rw-r--r--   0        0        0      330 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/music-note.svg
--rw-r--r--   0        0        0      445 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/n-square.svg
--rw-r--r--   0        0        0      219 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/nav-arrow-down.svg
--rw-r--r--   0        0        0      220 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/nav-arrow-left.svg
--rw-r--r--   0        0        0      219 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/nav-arrow-right.svg
--rw-r--r--   0        0        0      220 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/nav-arrow-up.svg
--rw-r--r--   0        0        0      511 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/navigator-alt.svg
--rw-r--r--   0        0        0      507 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/navigator.svg
--rw-r--r--   0        0        0     1231 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/neighbourhood.svg
--rw-r--r--   0        0        0      698 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/network-left.svg
--rw-r--r--   0        0        0      671 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/network-reverse.svg
--rw-r--r--   0        0        0      676 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/network-right.svg
--rw-r--r--   0        0        0      606 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/network.svg
--rw-r--r--   0        0        0      491 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/new-tab.svg
--rw-r--r--   0        0        0      924 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/nintendo-switch.svg
--rw-r--r--   0        0        0     1143 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/no-smoking-circle.svg
--rw-r--r--   0        0        0      505 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/non-binary.svg
--rw-r--r--   0        0        0      621 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/notes.svg
--rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/npm-square.svg
--rw-r--r--   0        0        0      699 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/npm.svg
--rw-r--r--   0        0        0      476 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-0-square.svg
--rw-r--r--   0        0        0      391 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-1-square.svg
--rw-r--r--   0        0        0      544 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-2-square.svg
--rw-r--r--   0        0        0      656 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-3-square.svg
--rw-r--r--   0        0        0      397 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-4-square.svg
--rw-r--r--   0        0        0      481 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-5-square.svg
--rw-r--r--   0        0        0      606 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-6-square.svg
--rw-r--r--   0        0        0      411 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-7-square.svg
--rw-r--r--   0        0        0      685 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-8-square.svg
--rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-9-square.svg
--rw-r--r--   0        0        0     1037 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/numbered-list-left.svg
--rw-r--r--   0        0        0     1027 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/numbered-list-right.svg
--rw-r--r--   0        0        0      569 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/o-square.svg
--rw-r--r--   0        0        0      733 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/octagon.svg
--rw-r--r--   0        0        0      851 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/off-tag.svg
--rw-r--r--   0        0        0      702 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/oil-industry.svg
--rw-r--r--   0        0        0      982 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/okrs.svg
--rw-r--r--   0        0        0      557 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/on-tag.svg
--rw-r--r--   0        0        0     1372 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/one-finger-select-hand-gesture.svg
--rw-r--r--   0        0        0      738 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/one-point-circle.svg
--rw-r--r--   0        0        0      768 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/open-book.svg
--rw-r--r--   0        0        0      603 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/open-in-browser.svg
--rw-r--r--   0        0        0      423 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/open-in-window.svg
--rw-r--r--   0        0        0      386 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/open-new-window.svg
--rw-r--r--   0        0        0     1326 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/open-select-hand-gesture.svg
--rw-r--r--   0        0        0     4298 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/open-vpn.svg
--rw-r--r--   0        0        0      344 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/orange-half.svg
--rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/orange-slice-alt.svg
--rw-r--r--   0        0        0      437 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/orange-slice.svg
--rw-r--r--   0        0        0      770 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/organic-food-square.svg
--rw-r--r--   0        0        0      745 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/organic-food.svg
--rw-r--r--   0        0        0      772 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/orthogonal-view.svg
--rw-r--r--   0        0        0      775 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/package-lock.svg
--rw-r--r--   0        0        0      437 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/package.svg
--rw-r--r--   0        0        0     1084 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/packages.svg
--rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pacman.svg
--rw-r--r--   0        0        0      422 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-down.svg
--rw-r--r--   0        0        0     1044 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-edit.svg
--rw-r--r--   0        0        0      727 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-flip.svg
--rw-r--r--   0        0        0      421 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-left.svg
--rw-r--r--   0        0        0      627 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-minus-in.svg
--rw-r--r--   0        0        0      603 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-minus.svg
--rw-r--r--   0        0        0      650 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-plus-in.svg
--rw-r--r--   0        0        0      650 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-plus.svg
--rw-r--r--   0        0        0      422 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-right.svg
--rw-r--r--   0        0        0      949 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-search.svg
--rw-r--r--   0        0        0     1093 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-star.svg
--rw-r--r--   0        0        0      421 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-up.svg
--rw-r--r--   0        0        0      813 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/page.svg
--rw-r--r--   0        0        0     1589 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/palette.svg
--rw-r--r--   0        0        0      707 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/panorama-enlarge.svg
--rw-r--r--   0        0        0      540 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/panorama-reduce.svg
--rw-r--r--   0        0        0      770 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pants-pockets.svg
--rw-r--r--   0        0        0      454 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pants.svg
--rw-r--r--   0        0        0      394 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/parking.svg
--rw-r--r--   0        0        0      721 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/password-check.svg
--rw-r--r--   0        0        0      925 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/password-cursor.svg
--rw-r--r--   0        0        0      815 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/password-xmark.svg
--rw-r--r--   0        0        0      639 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/paste-clipboard.svg
--rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/path-arrow.svg
--rw-r--r--   0        0        0      859 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pause-window.svg
--rw-r--r--   0        0        0      510 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pause.svg
--rw-r--r--   0        0        0      418 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/paypal.svg
--rw-r--r--   0        0        0      480 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pc-check.svg
--rw-r--r--   0        0        0      717 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pc-firewall.svg
--rw-r--r--   0        0        0      312 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pc-mouse.svg
--rw-r--r--   0        0        0      715 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pc-no-entry.svg
--rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pc-warning.svg
--rw-r--r--   0        0        0     1559 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/peace-hand.svg
--rw-r--r--   0        0        0      716 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/peerlist.svg
--rw-r--r--   0        0        0      620 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pen-connect-bluetooth.svg
--rw-r--r--   0        0        0      838 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pen-connect-wifi.svg
--rw-r--r--   0        0        0     1001 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pen-tablet-connect-usb.svg
--rw-r--r--   0        0        0      782 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pen-tablet-connect-wifi.svg
--rw-r--r--   0        0        0      623 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pen-tablet.svg
--rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pentagon.svg
--rw-r--r--   0        0        0      882 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/people-tag.svg
--rw-r--r--   0        0        0     1254 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/percent-rotate-out.svg
--rw-r--r--   0        0        0      853 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/percentage-circle.svg
--rw-r--r--   0        0        0      850 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/percentage-square.svg
--rw-r--r--   0        0        0      598 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/percentage.svg
--rw-r--r--   0        0        0      795 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/perspective-view.svg
--rw-r--r--   0        0        0      822 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pharmacy-cross-circle.svg
--rw-r--r--   0        0        0      829 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pharmacy-cross-tag.svg
--rw-r--r--   0        0        0      608 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-disabled.svg
--rw-r--r--   0        0        0      595 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-income.svg
--rw-r--r--   0        0        0      599 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-minus.svg
--rw-r--r--   0        0        0      595 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-outcome.svg
--rw-r--r--   0        0        0      669 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-paused.svg
--rw-r--r--   0        0        0      663 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-plus.svg
--rw-r--r--   0        0        0      689 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-xmark.svg
--rw-r--r--   0        0        0      485 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone.svg
--rw-r--r--   0        0        0     1279 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/piggy-bank.svg
--rw-r--r--   0        0        0      901 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pillow.svg
--rw-r--r--   0        0        0      538 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pin-slash.svg
--rw-r--r--   0        0        0      444 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pin.svg
--rw-r--r--   0        0        0      702 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pine-tree.svg
--rw-r--r--   0        0        0      602 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pinterest.svg
--rw-r--r--   0        0        0      913 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pipe-3d.svg
--rw-r--r--   0        0        0     1011 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pizza-slice.svg
--rw-r--r--   0        0        0      455 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/planet-alt.svg
--rw-r--r--   0        0        0      560 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/planet-sat.svg
--rw-r--r--   0        0        0      455 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/planet.svg
--rw-r--r--   0        0        0      995 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/planimetry.svg
--rw-r--r--   0        0        0      383 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/play.svg
--rw-r--r--   0        0        0      509 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/playlist-play.svg
--rw-r--r--   0        0        0      517 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/playlist-plus.svg
--rw-r--r--   0        0        0      632 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/playlist.svg
--rw-r--r--   0        0        0     1002 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/playstation-gamepad.svg
--rw-r--r--   0        0        0      498 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/plug-type-a.svg
--rw-r--r--   0        0        0      713 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/plug-type-c.svg
--rw-r--r--   0        0        0      588 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/plug-type-g.svg
--rw-r--r--   0        0        0      705 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/plug-type-l.svg
--rw-r--r--   0        0        0      433 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/plus-circle.svg
--rw-r--r--   0        0        0      968 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/plus-square-dashed.svg
--rw-r--r--   0        0        0      458 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/plus-square.svg
--rw-r--r--   0        0        0      238 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/plus.svg
--rw-r--r--   0        0        0      717 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/png-format.svg
--rw-r--r--   0        0        0      421 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pocket.svg
--rw-r--r--   0        0        0     1356 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/podcast.svg
--rw-r--r--   0        0        0      604 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pokeball.svg
--rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/polar-sh.svg
--rw-r--r--   0        0        0     1886 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/position-align.svg
--rw-r--r--   0        0        0      673 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/position.svg
--rw-r--r--   0        0        0      692 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/post.svg
--rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/potion.svg
--rw-r--r--   0        0        0      607 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/pound.svg
--rw-r--r--   0        0        0      683 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/precision-tool.svg
--rw-r--r--   0        0        0      809 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/presentation.svg
--rw-r--r--   0        0        0      524 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/printer.svg
--rw-r--r--   0        0        0      850 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/printing-page.svg
--rw-r--r--   0        0        0      586 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/priority-down.svg
--rw-r--r--   0        0        0      663 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/priority-high.svg
--rw-r--r--   0        0        0      646 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/priority-medium.svg
--rw-r--r--   0        0        0      584 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/priority-up.svg
--rw-r--r--   0        0        0      945 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/privacy-policy.svg
--rw-r--r--   0        0        0      941 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/private-wifi.svg
--rw-r--r--   0        0        0      682 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/profile-circle.svg
--rw-r--r--   0        0        0      437 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/prohibition.svg
--rw-r--r--   0        0        0      665 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/project-curve-3d.svg
--rw-r--r--   0        0        0     1216 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/puzzle.svg
--rw-r--r--   0        0        0     2455 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/qr-code.svg
--rw-r--r--   0        0        0      421 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/question-mark.svg
--rw-r--r--   0        0        0      765 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/quote-message.svg
--rw-r--r--   0        0        0      506 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/quote.svg
--rw-r--r--   0        0        0     1351 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/radiation.svg
--rw-r--r--   0        0        0      682 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/radius.svg
--rw-r--r--   0        0        0      713 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rain.svg
--rw-r--r--   0        0        0      998 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/raw-format.svg
--rw-r--r--   0        0        0      595 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/receive-dollars.svg
--rw-r--r--   0        0        0      644 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/receive-euros.svg
--rw-r--r--   0        0        0      666 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/receive-pounds.svg
--rw-r--r--   0        0        0      537 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/receive-yens.svg
--rw-r--r--   0        0        0      638 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/redo-action.svg
--rw-r--r--   0        0        0      606 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/redo-circle.svg
--rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/redo.svg
--rw-r--r--   0        0        0      336 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/reduce.svg
--rw-r--r--   0        0        0      826 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/refresh-circle.svg
--rw-r--r--   0        0        0      717 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/refresh-double.svg
--rw-r--r--   0        0        0      458 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/refresh.svg
--rw-r--r--   0        0        0     1334 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/reload-window.svg
--rw-r--r--   0        0        0     1554 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/reminder-hand-gesture.svg
--rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/repeat-once.svg
--rw-r--r--   0        0        0      423 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/repeat.svg
--rw-r--r--   0        0        0      546 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/reply-to-message.svg
--rw-r--r--   0        0        0      263 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/reply.svg
--rw-r--r--   0        0        0      902 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/report-columns.svg
--rw-r--r--   0        0        0      418 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/reports.svg
--rw-r--r--   0        0        0      575 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/repository.svg
--rw-r--r--   0        0        0      647 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/restart.svg
--rw-r--r--   0        0        0      650 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rewind.svg
--rw-r--r--   0        0        0      726 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rhombus-arrow-right.svg
--rw-r--r--   0        0        0      465 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rhombus.svg
--rw-r--r--   0        0        0      523 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rings.svg
--rw-r--r--   0        0        0      994 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rocket.svg
--rw-r--r--   0        0        0      901 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rook.svg
--rw-r--r--   0        0        0     1301 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rotate-camera-left.svg
--rw-r--r--   0        0        0     1298 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rotate-camera-right.svg
--rw-r--r--   0        0        0      922 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/round-flask.svg
--rw-r--r--   0        0        0      514 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rounded-mirror.svg
--rw-r--r--   0        0        0      635 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rss-feed-tag.svg
--rw-r--r--   0        0        0      440 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rss-feed.svg
--rw-r--r--   0        0        0      700 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/rubik-cube.svg
--rw-r--r--   0        0        0      748 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ruler-arrows.svg
--rw-r--r--   0        0        0      770 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ruler-combine.svg
--rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ruler-minus.svg
--rw-r--r--   0        0        0      494 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ruler-plus.svg
--rw-r--r--   0        0        0      385 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/ruler.svg
--rw-r--r--   0        0        0      733 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/running.svg
--rw-r--r--   0        0        0     1120 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/safari.svg
--rw-r--r--   0        0        0     1515 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/safe-arrow-left.svg
--rw-r--r--   0        0        0     1515 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/safe-arrow-right.svg
--rw-r--r--   0        0        0     1423 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/safe-open.svg
--rw-r--r--   0        0        0     1324 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/safe.svg
--rw-r--r--   0        0        0      787 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sandals.svg
--rw-r--r--   0        0        0     1108 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/scale-frame-enlarge.svg
--rw-r--r--   0        0        0      786 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/scale-frame-reduce.svg
--rw-r--r--   0        0        0     1567 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/scan-barcode.svg
--rw-r--r--   0        0        0     2139 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/scan-qr-code.svg
--rw-r--r--   0        0        0      965 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/scanning.svg
--rw-r--r--   0        0        0      570 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/scarf.svg
--rw-r--r--   0        0        0      630 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/scissor-alt.svg
--rw-r--r--   0        0        0      624 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/scissor.svg
--rw-r--r--   0        0        0     1358 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/screenshot.svg
--rw-r--r--   0        0        0      686 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sea-and-sun.svg
--rw-r--r--   0        0        0      542 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sea-waves.svg
--rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/search-engine.svg
--rw-r--r--   0        0        0      949 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/search-window.svg
--rw-r--r--   0        0        0      457 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/search.svg
--rw-r--r--   0        0        0     1011 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/secure-window.svg
--rw-r--r--   0        0        0      429 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/security-pass.svg
--rw-r--r--   0        0        0      912 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/select-edge-3d.svg
--rw-r--r--   0        0        0     1134 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/select-face-3d.svg
--rw-r--r--   0        0        0      786 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/select-point-3d.svg
--rw-r--r--   0        0        0      965 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/select-window.svg
--rw-r--r--   0        0        0      538 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/selective-tool.svg
--rw-r--r--   0        0        0      399 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/send-diagonal.svg
--rw-r--r--   0        0        0      595 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/send-dollars.svg
--rw-r--r--   0        0        0      644 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/send-euros.svg
--rw-r--r--   0        0        0      586 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/send-mail.svg
--rw-r--r--   0        0        0      666 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/send-pounds.svg
--rw-r--r--   0        0        0      537 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/send-yens.svg
--rw-r--r--   0        0        0      331 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/send.svg
--rw-r--r--   0        0        0      456 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/server-connection.svg
--rw-r--r--   0        0        0      713 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/server.svg
--rw-r--r--   0        0        0     1562 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/settings-profiles.svg
--rw-r--r--   0        0        0      786 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/settings.svg
--rw-r--r--   0        0        0      849 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/share-android.svg
--rw-r--r--   0        0        0      389 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/share-ios.svg
--rw-r--r--   0        0        0      667 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-alert.svg
--rw-r--r--   0        0        0      770 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-alt.svg
--rw-r--r--   0        0        0      577 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-broken.svg
--rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-check.svg
--rw-r--r--   0        0        0      582 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-download.svg
--rw-r--r--   0        0        0      804 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-eye.svg
--rw-r--r--   0        0        0      782 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-loading.svg
--rw-r--r--   0        0        0      562 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-minus.svg
--rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-plus-in.svg
--rw-r--r--   0        0        0      718 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-question.svg
--rw-r--r--   0        0        0      825 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-search.svg
--rw-r--r--   0        0        0      580 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-upload.svg
--rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-xmark.svg
--rw-r--r--   0        0        0      469 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield.svg
--rw-r--r--   0        0        0      635 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shirt-tank-top.svg
--rw-r--r--   0        0        0      744 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shirt.svg
--rw-r--r--   0        0        0     1037 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shop-four-tiles-window.svg
--rw-r--r--   0        0        0     1196 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shop-four-tiles.svg
--rw-r--r--   0        0        0     1195 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shop-window.svg
--rw-r--r--   0        0        0     1354 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shop.svg
--rw-r--r--   0        0        0      674 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-arrow-down.svg
--rw-r--r--   0        0        0      674 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-arrow-up.svg
--rw-r--r--   0        0        0      608 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-check.svg
--rw-r--r--   0        0        0      666 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-minus.svg
--rw-r--r--   0        0        0      713 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-plus.svg
--rw-r--r--   0        0        0      751 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-pocket.svg
--rw-r--r--   0        0        0      713 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-warning.svg
--rw-r--r--   0        0        0      565 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag.svg
--rw-r--r--   0        0        0     1126 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-code-check.svg
--rw-r--r--   0        0        0     1232 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-code-xmark.svg
--rw-r--r--   0        0        0     1212 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-code.svg
--rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/short-pants-pockets.svg
--rw-r--r--   0        0        0      455 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/short-pants.svg
--rw-r--r--   0        0        0      584 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shortcut-square.svg
--rw-r--r--   0        0        0      681 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/shuffle.svg
--rw-r--r--   0        0        0      534 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sidebar-collapse.svg
--rw-r--r--   0        0        0      533 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sidebar-expand.svg
--rw-r--r--   0        0        0      413 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sigma-function.svg
--rw-r--r--   0        0        0      534 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/simple-cart.svg
--rw-r--r--   0        0        0      678 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sine-wave.svg
--rw-r--r--   0        0        0      497 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/single-tap-gesture.svg
--rw-r--r--   0        0        0      648 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/skateboard.svg
--rw-r--r--   0        0        0     1061 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/skateboarding.svg
--rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/skip-next.svg
--rw-r--r--   0        0        0      477 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/skip-prev.svg
--rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/slash-square.svg
--rw-r--r--   0        0        0      214 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/slash.svg
--rw-r--r--   0        0        0      753 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sleeper-chair.svg
--rw-r--r--   0        0        0      593 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/slips.svg
--rw-r--r--   0        0        0      624 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/small-lamp-alt.svg
--rw-r--r--   0        0        0      770 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/small-lamp.svg
--rw-r--r--   0        0        0      419 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/smartphone-device.svg
--rw-r--r--   0        0        0      744 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/smoking.svg
--rw-r--r--   0        0        0      714 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/snapchat.svg
--rw-r--r--   0        0        0      501 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/snow-flake.svg
--rw-r--r--   0        0        0      518 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/snow.svg
--rw-r--r--   0        0        0      457 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/soap.svg
--rw-r--r--   0        0        0      748 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/soccer-ball.svg
--rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sofa.svg
--rw-r--r--   0        0        0     1457 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/soil-alt.svg
--rw-r--r--   0        0        0     1667 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/soil.svg
--rw-r--r--   0        0        0      600 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sort-down.svg
--rw-r--r--   0        0        0      593 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sort-up.svg
--rw-r--r--   0        0        0      613 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sort.svg
--rw-r--r--   0        0        0      744 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sound-high.svg
--rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sound-low.svg
--rw-r--r--   0        0        0      557 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sound-min.svg
--rw-r--r--   0        0        0      616 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sound-off.svg
--rw-r--r--   0        0        0      521 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/spades.svg
--rw-r--r--   0        0        0      297 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/spark.svg
--rw-r--r--   0        0        0      483 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sparks.svg
--rw-r--r--   0        0        0      456 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sphere.svg
--rw-r--r--   0        0        0     1281 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/spiral.svg
--rw-r--r--   0        0        0      584 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/split-area.svg
--rw-r--r--   0        0        0      761 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/split-square-dashed.svg
--rw-r--r--   0        0        0     1206 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/spock-hand-gesture.svg
--rw-r--r--   0        0        0      658 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/spotify.svg
--rw-r--r--   0        0        0      719 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/square-3d-corner-to-corner.svg
--rw-r--r--   0        0        0      516 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/square-3d-from-center.svg
--rw-r--r--   0        0        0     1308 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/square-3d-three-points.svg
--rw-r--r--   0        0        0      518 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/square-cursor.svg
--rw-r--r--   0        0        0      852 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/square-dashed.svg
--rw-r--r--   0        0        0      429 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/square-wave.svg
--rw-r--r--   0        0        0      342 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/square.svg
--rw-r--r--   0        0        0      753 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/stackoverflow.svg
--rw-r--r--   0        0        0     1622 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/star-dashed.svg
--rw-r--r--   0        0        0     1304 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/star-half-dashed.svg
--rw-r--r--   0        0        0      614 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/star.svg
--rw-r--r--   0        0        0      339 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/stat-down.svg
--rw-r--r--   0        0        0      339 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/stat-up.svg
--rw-r--r--   0        0        0      593 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/stats-down-square.svg
--rw-r--r--   0        0        0      804 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/stats-report.svg
--rw-r--r--   0        0        0      593 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/stats-up-square.svg
--rw-r--r--   0        0        0      731 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/strategy.svg
--rw-r--r--   0        0        0      584 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/stretching.svg
--rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/strikethrough.svg
--rw-r--r--   0        0        0      997 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/stroller.svg
--rw-r--r--   0        0        0      641 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/style-border.svg
--rw-r--r--   0        0        0      615 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/submit-document.svg
--rw-r--r--   0        0        0     1040 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/substract.svg
--rw-r--r--   0        0        0      650 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/suggestion.svg
--rw-r--r--   0        0        0      373 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/suitcase.svg
--rw-r--r--   0        0        0     1051 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sun-light.svg
--rw-r--r--   0        0        0      818 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/svg-format.svg
--rw-r--r--   0        0        0      717 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/sweep-3d.svg
--rw-r--r--   0        0        0      969 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/swimming.svg
--rw-r--r--   0        0        0      347 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/swipe-down-gesture.svg
--rw-r--r--   0        0        0      347 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/swipe-left-gesture.svg
--rw-r--r--   0        0        0      347 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/swipe-right-gesture.svg
--rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/swipe-two-fingers-down-gesture.svg
--rw-r--r--   0        0        0      589 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/swipe-two-fingers-left-gesture.svg
--rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/swipe-two-fingers-right-gesture.svg
--rw-r--r--   0        0        0      589 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/swipe-two-fingers-up-gesture.svg
--rw-r--r--   0        0        0      347 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/swipe-up-gesture.svg
--rw-r--r--   0        0        0      505 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/switch-off.svg
--rw-r--r--   0        0        0      514 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/switch-on.svg
--rw-r--r--   0        0        0      936 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/system-restart.svg
--rw-r--r--   0        0        0      407 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/system-shut.svg
--rw-r--r--   0        0        0      565 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/table-2-columns.svg
--rw-r--r--   0        0        0      456 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/table-rows.svg
--rw-r--r--   0        0        0      766 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/table.svg
--rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/task-list.svg
--rw-r--r--   0        0        0      450 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/telegram-circle.svg
--rw-r--r--   0        0        0      281 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/telegram.svg
--rw-r--r--   0        0        0     1055 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/temperature-down.svg
--rw-r--r--   0        0        0     1125 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/temperature-high.svg
--rw-r--r--   0        0        0     1126 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/temperature-low.svg
--rw-r--r--   0        0        0     1048 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/temperature-up.svg
--rw-r--r--   0        0        0      693 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tennis-ball-alt.svg
--rw-r--r--   0        0        0      608 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tennis-ball.svg
--rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/terminal-tag.svg
--rw-r--r--   0        0        0      310 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/terminal.svg
--rw-r--r--   0        0        0      521 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/test-tube.svg
--rw-r--r--   0        0        0      468 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/text-arrows-up-down.svg
--rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/text-box.svg
--rw-r--r--   0        0        0      669 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/text-magnifying-glass.svg
--rw-r--r--   0        0        0      542 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/text-size.svg
--rw-r--r--   0        0        0      545 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/text-square.svg
--rw-r--r--   0        0        0      328 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/text.svg
--rw-r--r--   0        0        0      485 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/threads.svg
--rw-r--r--   0        0        0     1321 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/three-points-circle.svg
--rw-r--r--   0        0        0     1587 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/three-stars.svg
--rw-r--r--   0        0        0      693 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/thumbs-down.svg
--rw-r--r--   0        0        0      667 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/thumbs-up.svg
--rw-r--r--   0        0        0      456 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/thunderstorm.svg
--rw-r--r--   0        0        0      772 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tif-format.svg
--rw-r--r--   0        0        0      960 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tiff-format.svg
--rw-r--r--   0        0        0      517 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tiktok.svg
--rw-r--r--   0        0        0     1075 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/time-zone.svg
--rw-r--r--   0        0        0      702 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/timer-off.svg
--rw-r--r--   0        0        0      502 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/timer.svg
--rw-r--r--   0        0        0     1145 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tools.svg
--rw-r--r--   0        0        0      538 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tournament.svg
--rw-r--r--   0        0        0      866 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tower-check.svg
--rw-r--r--   0        0        0     1048 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tower-no-access.svg
--rw-r--r--   0        0        0      965 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tower-warning.svg
--rw-r--r--   0        0        0      766 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tower.svg
--rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/trademark.svg
--rw-r--r--   0        0        0     1061 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/train.svg
--rw-r--r--   0        0        0     1092 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tram.svg
--rw-r--r--   0        0        0      562 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/transition-down.svg
--rw-r--r--   0        0        0      554 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/transition-left.svg
--rw-r--r--   0        0        0      558 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/transition-right.svg
--rw-r--r--   0        0        0      558 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/transition-up.svg
--rw-r--r--   0        0        0      553 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/translate.svg
--rw-r--r--   0        0        0      527 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/trash.svg
--rw-r--r--   0        0        0     1070 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/treadmill.svg
--rw-r--r--   0        0        0      686 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tree.svg
--rw-r--r--   0        0        0      760 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/trekking.svg
--rw-r--r--   0        0        0      775 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/trello.svg
--rw-r--r--   0        0        0      456 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/triangle-flag-circle.svg
--rw-r--r--   0        0        0      442 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/triangle-flag-two-stripes.svg
--rw-r--r--   0        0        0      337 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/triangle-flag.svg
--rw-r--r--   0        0        0      396 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/triangle.svg
--rw-r--r--   0        0        0     1079 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/trophy.svg
--rw-r--r--   0        0        0     1199 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/truck-green.svg
--rw-r--r--   0        0        0     1248 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/truck-length.svg
--rw-r--r--   0        0        0     1085 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/truck.svg
--rw-r--r--   0        0        0      655 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tunnel.svg
--rw-r--r--   0        0        0      896 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tv-fix.svg
--rw-r--r--   0        0        0      596 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tv-warning.svg
--rw-r--r--   0        0        0      400 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/tv.svg
--rw-r--r--   0        0        0      727 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/twitter.svg
--rw-r--r--   0        0        0     1235 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/two-points-circle.svg
--rw-r--r--   0        0        0      810 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/two-seater-sofa.svg
--rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/type.svg
--rw-r--r--   0        0        0      436 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/u-turn-arrow-left.svg
--rw-r--r--   0        0        0      441 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/u-turn-arrow-right.svg
--rw-r--r--   0        0        0      939 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/umbrella.svg
--rw-r--r--   0        0        0      556 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/underline-square.svg
--rw-r--r--   0        0        0      364 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/underline.svg
--rw-r--r--   0        0        0      636 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/undo-action.svg
--rw-r--r--   0        0        0      614 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/undo-circle.svg
--rw-r--r--   0        0        0      480 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/undo.svg
--rw-r--r--   0        0        0      495 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/union-alt.svg
--rw-r--r--   0        0        0      499 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/union-horiz-alt.svg
--rw-r--r--   0        0        0      496 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/union.svg
--rw-r--r--   0        0        0      811 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/unity-5.svg
--rw-r--r--   0        0        0      334 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/unity.svg
--rw-r--r--   0        0        0      540 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/unjoin-3d.svg
--rw-r--r--   0        0        0      796 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/upload-data-window.svg
--rw-r--r--   0        0        0      524 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/upload-square.svg
--rw-r--r--   0        0        0      332 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/upload.svg
--rw-r--r--   0        0        0     1027 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/usb.svg
--rw-r--r--   0        0        0     1510 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-badge-check.svg
--rw-r--r--   0        0        0      858 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-bag.svg
--rw-r--r--   0        0        0      819 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-cart.svg
--rw-r--r--   0        0        0      516 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-circle.svg
--rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-crown.svg
--rw-r--r--   0        0        0      938 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-love.svg
--rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-plus.svg
--rw-r--r--   0        0        0      834 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-scan.svg
--rw-r--r--   0        0        0      662 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-square.svg
--rw-r--r--   0        0        0      961 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-star.svg
--rw-r--r--   0        0        0      647 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-xmark.svg
--rw-r--r--   0        0        0      463 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/user.svg
--rw-r--r--   0        0        0      774 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/vegan-circle.svg
--rw-r--r--   0        0        0      800 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/vegan-square.svg
--rw-r--r--   0        0        0      603 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/vegan.svg
--rw-r--r--   0        0        0     1262 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/vehicle-green.svg
--rw-r--r--   0        0        0      549 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/vertical-merge.svg
--rw-r--r--   0        0        0      547 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/vertical-split.svg
--rw-r--r--   0        0        0      692 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/vials.svg
--rw-r--r--   0        0        0      552 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/video-camera-off.svg
--rw-r--r--   0        0        0      461 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/video-camera.svg
--rw-r--r--   0        0        0     1298 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/video-projector.svg
--rw-r--r--   0        0        0     1003 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/view-360.svg
--rw-r--r--   0        0        0      331 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/view-columns-2.svg
--rw-r--r--   0        0        0      351 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/view-columns-3.svg
--rw-r--r--   0        0        0      902 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/view-grid.svg
--rw-r--r--   0        0        0      701 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/view-structure-down.svg
--rw-r--r--   0        0        0      709 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/view-structure-up.svg
--rw-r--r--   0        0        0      695 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice-check.svg
--rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice-circle.svg
--rw-r--r--   0        0        0     1198 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice-lock-circle.svg
--rw-r--r--   0        0        0      953 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice-scan.svg
--rw-r--r--   0        0        0      805 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice-square.svg
--rw-r--r--   0        0        0      789 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice-xmark.svg
--rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice.svg
--rw-r--r--   0        0        0      646 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/vr-tag.svg
--rw-r--r--   0        0        0      360 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/vue-js.svg
--rw-r--r--   0        0        0      902 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/waist.svg
--rw-r--r--   0        0        0      767 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/walking.svg
--rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wallet.svg
--rw-r--r--   0        0        0      515 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/warning-circle.svg
--rw-r--r--   0        0        0      765 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/warning-hexagon.svg
--rw-r--r--   0        0        0      509 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/warning-square.svg
--rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/warning-triangle.svg
--rw-r--r--   0        0        0      870 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/warning-window.svg
--rw-r--r--   0        0        0      493 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wash.svg
--rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/washing-machine.svg
--rw-r--r--   0        0        0     1229 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/watering-soil.svg
--rw-r--r--   0        0        0      545 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/web-window-energy-consumption.svg
--rw-r--r--   0        0        0      563 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/web-window-xmark.svg
--rw-r--r--   0        0        0      433 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/web-window.svg
--rw-r--r--   0        0        0     1171 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/webp-format.svg
--rw-r--r--   0        0        0      956 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/weight-alt.svg
--rw-r--r--   0        0        0      863 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/weight.svg
--rw-r--r--   0        0        0      379 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/white-flag.svg
--rw-r--r--   0        0        0      810 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wifi-off.svg
--rw-r--r--   0        0        0      493 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wifi-signal-none.svg
--rw-r--r--   0        0        0      645 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wifi-tag.svg
--rw-r--r--   0        0        0      688 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wifi-warning.svg
--rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wifi-xmark.svg
--rw-r--r--   0        0        0      566 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wifi.svg
--rw-r--r--   0        0        0      588 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wind.svg
--rw-r--r--   0        0        0      771 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/window-check.svg
--rw-r--r--   0        0        0     1041 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/window-lock.svg
--rw-r--r--   0        0        0     1015 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/window-no-access.svg
--rw-r--r--   0        0        0      457 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/window-tabs.svg
--rw-r--r--   0        0        0      861 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/window-xmark.svg
--rw-r--r--   0        0        0      469 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/windows.svg
--rw-r--r--   0        0        0     1116 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wolf.svg
--rw-r--r--   0        0        0      574 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wrap-text.svg
--rw-r--r--   0        0        0      704 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wrench.svg
--rw-r--r--   0        0        0      728 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/wristwatch.svg
--rw-r--r--   0        0        0     1345 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/www.svg
--rw-r--r--   0        0        0      528 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/x-square.svg
--rw-r--r--   0        0        0      467 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/x.svg
--rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/xbox-a.svg
--rw-r--r--   0        0        0      626 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/xbox-b.svg
--rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/xbox-x.svg
--rw-r--r--   0        0        0      508 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/xbox-y.svg
--rw-r--r--   0        0        0      505 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/xmark-circle.svg
--rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/xmark-square.svg
--rw-r--r--   0        0        0      312 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/xmark.svg
--rw-r--r--   0        0        0     1004 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/xray-view.svg
--rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/y-square.svg
--rw-r--r--   0        0        0     1218 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/yelp.svg
--rw-r--r--   0        0        0      612 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/yen-square.svg
--rw-r--r--   0        0        0      414 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/yen.svg
--rw-r--r--   0        0        0     1013 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/yoga.svg
--rw-r--r--   0        0        0      825 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/youtube.svg
--rw-r--r--   0        0        0      441 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/z-square.svg
--rw-r--r--   0        0        0      573 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/zoom-in.svg
--rw-r--r--   0        0        0      550 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/regular/zoom-out.svg
--rw-r--r--   0        0        0        0 2024-04-25 23:08:11.213264 flet_iconoir-0.2.2/flet_iconoir/icons/solid/__init__.py
--rw-r--r--   0        0        0     1152 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/adobe-after-effects.svg
--rw-r--r--   0        0        0     1122 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/adobe-illustrator.svg
--rw-r--r--   0        0        0      824 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/adobe-indesign.svg
--rw-r--r--   0        0        0     1032 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/adobe-lightroom.svg
--rw-r--r--   0        0        0     1456 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/adobe-photoshop.svg
--rw-r--r--   0        0        0     1169 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/adobe-xd.svg
--rw-r--r--   0        0        0      495 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/airplay.svg
--rw-r--r--   0        0        0     1143 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/alarm.svg
--rw-r--r--   0        0        0     1117 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-bottom-box.svg
--rw-r--r--   0        0        0      414 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-horizontal-centers.svg
--rw-r--r--   0        0        0      519 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-horizontal-spacing.svg
--rw-r--r--   0        0        0     1221 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-left-box.svg
--rw-r--r--   0        0        0     1204 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-right-box.svg
--rw-r--r--   0        0        0     1116 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-top-box.svg
--rw-r--r--   0        0        0      411 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-vertical-centers.svg
--rw-r--r--   0        0        0      521 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-vertical-spacing.svg
--rw-r--r--   0        0        0      649 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/app-notification.svg
--rw-r--r--   0        0        0     1143 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/app-store.svg
--rw-r--r--   0        0        0     1196 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/apple-shortcuts.svg
--rw-r--r--   0        0        0      726 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-down-circle.svg
--rw-r--r--   0        0        0      743 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-down-left-circle.svg
--rw-r--r--   0        0        0      879 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-down-right-circle.svg
--rw-r--r--   0        0        0      904 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-down-right-square.svg
--rw-r--r--   0        0        0      731 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-left-circle.svg
--rw-r--r--   0        0        0      726 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-right-circle.svg
--rw-r--r--   0        0        0      731 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-up-circle.svg
--rw-r--r--   0        0        0      836 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-up-left-circle.svg
--rw-r--r--   0        0        0      861 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-up-left-square.svg
--rw-r--r--   0        0        0      836 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-up-right-circle.svg
--rw-r--r--   0        0        0      861 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-up-right-square.svg
--rw-r--r--   0        0        0      970 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/bathroom.svg
--rw-r--r--   0        0        0     1915 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/bitcoin-circle.svg
--rw-r--r--   0        0        0     1164 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/bluetooth-tag.svg
--rw-r--r--   0        0        0     2246 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/bold-square.svg
--rw-r--r--   0        0        0      733 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/book.svg
--rw-r--r--   0        0        0      669 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/bookmark-circle.svg
--rw-r--r--   0        0        0      357 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/bookmark.svg
--rw-r--r--   0        0        0     1632 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/bubble-search.svg
--rw-r--r--   0        0        0     1404 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/bubble-xmark.svg
--rw-r--r--   0        0        0      796 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/cable-tag.svg
--rw-r--r--   0        0        0      690 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/camera.svg
--rw-r--r--   0        0        0      975 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/cash.svg
--rw-r--r--   0        0        0     2203 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/center-align.svg
--rw-r--r--   0        0        0      816 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble-check.svg
--rw-r--r--   0        0        0      500 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble-empty.svg
--rw-r--r--   0        0        0     1695 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble-question.svg
--rw-r--r--   0        0        0     1480 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble-translate.svg
--rw-r--r--   0        0        0      890 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble-warning.svg
--rw-r--r--   0        0        0     1019 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble-xmark.svg
--rw-r--r--   0        0        0      965 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble.svg
--rw-r--r--   0        0        0      825 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-lines.svg
--rw-r--r--   0        0        0      664 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-minus-in.svg
--rw-r--r--   0        0        0      831 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-plus-in.svg
--rw-r--r--   0        0        0      648 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/check-circle.svg
--rw-r--r--   0        0        0      668 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/check-square.svg
--rw-r--r--   0        0        0      543 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/clock.svg
--rw-r--r--   0        0        0     1631 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/closed-captions-tag.svg
--rw-r--r--   0        0        0      895 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/cloud-square.svg
--rw-r--r--   0        0        0      411 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/comp-align-bottom.svg
--rw-r--r--   0        0        0      410 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/comp-align-left.svg
--rw-r--r--   0        0        0      411 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/comp-align-right.svg
--rw-r--r--   0        0        0      409 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/comp-align-top.svg
--rw-r--r--   0        0        0     1477 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/component.svg
--rw-r--r--   0        0        0      432 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/credit-card.svg
--rw-r--r--   0        0        0     3486 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/database-check.svg
--rw-r--r--   0        0        0     1807 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/database-tag.svg
--rw-r--r--   0        0        0     3173 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/database-xmark.svg
--rw-r--r--   0        0        0     3279 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/database.svg
--rw-r--r--   0        0        0     1477 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/design-nib.svg
--rw-r--r--   0        0        0     1252 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/dogecoin-circle.svg
--rw-r--r--   0        0        0     1843 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/dollar-circle.svg
--rw-r--r--   0        0        0      890 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/download-circle.svg
--rw-r--r--   0        0        0      921 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/download-square.svg
--rw-r--r--   0        0        0      280 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/droplet.svg
--rw-r--r--   0        0        0      743 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/erase.svg
--rw-r--r--   0        0        0      897 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/ethereum-circle.svg
--rw-r--r--   0        0        0     1413 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/euro-square.svg
--rw-r--r--   0        0        0      465 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/eye.svg
--rw-r--r--   0        0        0      637 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/facetime.svg
--rw-r--r--   0        0        0      903 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/fill-color.svg
--rw-r--r--   0        0        0      696 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/filter.svg
--rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/flash.svg
--rw-r--r--   0        0        0      708 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/forward.svg
--rw-r--r--   0        0        0      523 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/frame-tool.svg
--rw-r--r--   0        0        0     1161 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/fx-tag.svg
--rw-r--r--   0        0        0     1373 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/hd-display.svg
--rw-r--r--   0        0        0     1095 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/headset-bolt.svg
--rw-r--r--   0        0        0     1206 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/headset-warning.svg
--rw-r--r--   0        0        0      969 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/headset.svg
--rw-r--r--   0        0        0      635 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/heart.svg
--rw-r--r--   0        0        0     1575 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/help-circle.svg
--rw-r--r--   0        0        0     1585 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/help-square.svg
--rw-r--r--   0        0        0      712 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/horiz-distribution-left.svg
--rw-r--r--   0        0        0      722 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/horiz-distribution-right.svg
--rw-r--r--   0        0        0     7050 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/hospital-circle.svg
--rw-r--r--   0        0        0      843 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/ice-cream.svg
--rw-r--r--   0        0        0      739 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/info-circle.svg
--rw-r--r--   0        0        0      720 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/italic-square.svg
--rw-r--r--   0        0        0     1346 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-align-center.svg
--rw-r--r--   0        0        0      884 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-align-horizontal.svg
--rw-r--r--   0        0        0      884 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-align-vertical.svg
--rw-r--r--   0        0        0      658 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-minus-in.svg
--rw-r--r--   0        0        0      656 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-minus.svg
--rw-r--r--   0        0        0      819 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-plus-in.svg
--rw-r--r--   0        0        0      822 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-plus.svg
--rw-r--r--   0        0        0      742 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-position.svg
--rw-r--r--   0        0        0      425 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe.svg
--rw-r--r--   0        0        0      975 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframes-couple.svg
--rw-r--r--   0        0        0      778 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframes.svg
--rw-r--r--   0        0        0      415 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/label.svg
--rw-r--r--   0        0        0      804 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/litecoin-circle.svg
--rw-r--r--   0        0        0      769 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/mail-open.svg
--rw-r--r--   0        0        0      644 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/mail.svg
--rw-r--r--   0        0        0     1413 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/medal-1st.svg
--rw-r--r--   0        0        0     1098 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/medal.svg
--rw-r--r--   0        0        0      793 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/message-alert.svg
--rw-r--r--   0        0        0      715 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/message-text.svg
--rw-r--r--   0        0        0      408 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/message.svg
--rw-r--r--   0        0        0      637 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone-check.svg
--rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone-minus.svg
--rw-r--r--   0        0        0     1544 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone-mute.svg
--rw-r--r--   0        0        0      673 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone-plus.svg
--rw-r--r--   0        0        0      637 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone-speaking.svg
--rw-r--r--   0        0        0      747 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone-warning.svg
--rw-r--r--   0        0        0      510 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone.svg
--rw-r--r--   0        0        0      485 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/minus-circle.svg
--rw-r--r--   0        0        0      516 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/minus-square.svg
--rw-r--r--   0        0        0     1872 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/money-square.svg
--rw-r--r--   0        0        0     1502 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/multi-bubble.svg
--rw-r--r--   0        0        0      604 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/music-note-plus.svg
--rw-r--r--   0        0        0      480 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/music-note.svg
--rw-r--r--   0        0        0      739 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/network-left.svg
--rw-r--r--   0        0        0      712 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/network-reverse.svg
--rw-r--r--   0        0        0      717 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/network-right.svg
--rw-r--r--   0        0        0      647 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/network.svg
--rw-r--r--   0        0        0      700 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-0-square.svg
--rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-1-square.svg
--rw-r--r--   0        0        0     1236 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-2-square.svg
--rw-r--r--   0        0        0     1217 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-3-square.svg
--rw-r--r--   0        0        0      775 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-4-square.svg
--rw-r--r--   0        0        0     1002 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-5-square.svg
--rw-r--r--   0        0        0     1454 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-6-square.svg
--rw-r--r--   0        0        0      951 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-7-square.svg
--rw-r--r--   0        0        0     1539 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-8-square.svg
--rw-r--r--   0        0        0     1446 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-9-square.svg
--rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/pause.svg
--rw-r--r--   0        0        0      886 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/percentage-circle.svg
--rw-r--r--   0        0        0      911 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/percentage-square.svg
--rw-r--r--   0        0        0      762 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/pin-slash.svg
--rw-r--r--   0        0        0      483 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/pin.svg
--rw-r--r--   0        0        0      403 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/play.svg
--rw-r--r--   0        0        0      658 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/plus-circle.svg
--rw-r--r--   0        0        0      683 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/plus-square.svg
--rw-r--r--   0        0        0     1346 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/podcast.svg
--rw-r--r--   0        0        0     1156 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/post.svg
--rw-r--r--   0        0        0     1442 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/presentation.svg
--rw-r--r--   0        0        0     1045 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/priority-down.svg
--rw-r--r--   0        0        0     1003 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/priority-high.svg
--rw-r--r--   0        0        0      926 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/priority-medium.svg
--rw-r--r--   0        0        0     1051 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/priority-up.svg
--rw-r--r--   0        0        0     1261 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/quote-message.svg
--rw-r--r--   0        0        0     1082 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/quote.svg
--rw-r--r--   0        0        0    10294 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/redo-circle.svg
--rw-r--r--   0        0        0     1416 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/refresh-circle.svg
--rw-r--r--   0        0        0      313 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/reports.svg
--rw-r--r--   0        0        0      709 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/rewind.svg
--rw-r--r--   0        0        0     1177 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/rhombus-arrow-right.svg
--rw-r--r--   0        0        0      809 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/send-diagonal.svg
--rw-r--r--   0        0        0      610 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/send.svg
--rw-r--r--   0        0        0      986 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/server-connection.svg
--rw-r--r--   0        0        0     1084 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/server.svg
--rw-r--r--   0        0        0      947 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/share-android.svg
--rw-r--r--   0        0        0      514 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/skip-next.svg
--rw-r--r--   0        0        0      516 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/skip-prev.svg
--rw-r--r--   0        0        0     3738 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/sound-high.svg
--rw-r--r--   0        0        0     2014 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/sound-low.svg
--rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/sound-min.svg
--rw-r--r--   0        0        0     1262 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/sound-off.svg
--rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/spark.svg
--rw-r--r--   0        0        0      542 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/sparks.svg
--rw-r--r--   0        0        0      557 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/square-cursor.svg
--rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/star.svg
--rw-r--r--   0        0        0      829 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/stats-down-square.svg
--rw-r--r--   0        0        0      829 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/stats-up-square.svg
--rw-r--r--   0        0        0      642 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/style-border.svg
--rw-r--r--   0        0        0      810 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/text-square.svg
--rw-r--r--   0        0        0     1685 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/three-stars.svg
--rw-r--r--   0        0        0      732 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/timer.svg
--rw-r--r--   0        0        0     1204 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/transition-down.svg
--rw-r--r--   0        0        0     1202 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/transition-left.svg
--rw-r--r--   0        0        0     1212 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/transition-right.svg
--rw-r--r--   0        0        0     1202 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/transition-up.svg
--rw-r--r--   0        0        0      689 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/trash.svg
--rw-r--r--   0        0        0      821 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/underline-square.svg
--rw-r--r--   0        0        0     1951 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/undo-circle.svg
--rw-r--r--   0        0        0      926 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/upload-square.svg
--rw-r--r--   0        0        0     1201 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/usb.svg
--rw-r--r--   0        0        0      627 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/wallet.svg
--rw-r--r--   0        0        0      726 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/warning-circle.svg
--rw-r--r--   0        0        0      751 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/warning-square.svg
--rw-r--r--   0        0        0      772 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/warning-triangle.svg
--rw-r--r--   0        0        0     1012 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/web-window-energy-consumption.svg
--rw-r--r--   0        0        0     1055 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/web-window-xmark.svg
--rw-r--r--   0        0        0      546 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/web-window.svg
--rw-r--r--   0        0        0      586 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/white-flag.svg
--rw-r--r--   0        0        0      548 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/wifi-signal-none.svg
--rw-r--r--   0        0        0     1129 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/wifi-tag.svg
--rw-r--r--   0        0        0      947 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/wifi-warning.svg
--rw-r--r--   0        0        0      683 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/window-tabs.svg
--rw-r--r--   0        0        0      842 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/xmark-circle.svg
--rw-r--r--   0        0        0      852 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/xmark-square.svg
--rw-r--r--   0        0        0     1048 2024-04-25 12:40:38.000000 flet_iconoir-0.2.2/flet_iconoir/icons/solid/yen-square.svg
--rw-r--r--   0        0        0      363 2024-04-26 08:52:30.575838 flet_iconoir-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      656 2024-04-26 01:18:07.124963 flet_iconoir-0.2.2/README.md
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 flet_iconoir-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      165 2024-04-26 01:39:53.802579 flet_iconoir-0.3.0/flet_iconoir/__init__.py
+-rw-r--r--   0        0        0      459 2024-04-26 02:00:33.830972 flet_iconoir-0.3.0/flet_iconoir/iconoir_icon.py
+-rw-r--r--   0        0        0     1639 2024-04-26 05:19:59.640434 flet_iconoir-0.3.0/flet_iconoir/iconoir_icon_button.py
+-rw-r--r--   0        0        0      478 2024-04-28 00:20:58.934158 flet_iconoir-0.3.0/flet_iconoir/icons/__init__.py
+-rw-r--r--   0        0        0     1068 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-25 23:20:21.429893 flet_iconoir-0.3.0/flet_iconoir/icons/regular/__init__.py
+-rw-r--r--   0        0        0      902 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/accessibility-sign.svg
+-rw-r--r--   0        0        0      964 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/accessibility-tech.svg
+-rw-r--r--   0        0        0      681 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/accessibility.svg
+-rw-r--r--   0        0        0      230 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/activity.svg
+-rw-r--r--   0        0        0      677 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/adobe-after-effects.svg
+-rw-r--r--   0        0        0      677 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/adobe-illustrator.svg
+-rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/adobe-indesign.svg
+-rw-r--r--   0        0        0      557 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/adobe-lightroom.svg
+-rw-r--r--   0        0        0      807 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/adobe-photoshop.svg
+-rw-r--r--   0        0        0      623 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/adobe-xd.svg
+-rw-r--r--   0        0        0      550 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/african-tree.svg
+-rw-r--r--   0        0        0      667 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/agile.svg
+-rw-r--r--   0        0        0      996 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/air-conditioner.svg
+-rw-r--r--   0        0        0     1843 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/airplane-helix-45deg.svg
+-rw-r--r--   0        0        0     1495 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/airplane-helix.svg
+-rw-r--r--   0        0        0     1100 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/airplane-off.svg
+-rw-r--r--   0        0        0     1580 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/airplane-rotation.svg
+-rw-r--r--   0        0        0     1016 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/airplane.svg
+-rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/airplay.svg
+-rw-r--r--   0        0        0      596 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/alarm.svg
+-rw-r--r--   0        0        0      586 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/album-carousel.svg
+-rw-r--r--   0        0        0      620 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/album-list.svg
+-rw-r--r--   0        0        0      756 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/album-open.svg
+-rw-r--r--   0        0        0      522 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/album.svg
+-rw-r--r--   0        0        0      964 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-bottom-box.svg
+-rw-r--r--   0        0        0      487 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-center.svg
+-rw-r--r--   0        0        0      375 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-horizontal-centers.svg
+-rw-r--r--   0        0        0      461 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-horizontal-spacing.svg
+-rw-r--r--   0        0        0      481 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-justify.svg
+-rw-r--r--   0        0        0     1041 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-left-box.svg
+-rw-r--r--   0        0        0      487 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-left.svg
+-rw-r--r--   0        0        0     1027 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-right-box.svg
+-rw-r--r--   0        0        0      487 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-right.svg
+-rw-r--r--   0        0        0      928 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-top-box.svg
+-rw-r--r--   0        0        0      372 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-vertical-centers.svg
+-rw-r--r--   0        0        0      463 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-vertical-spacing.svg
+-rw-r--r--   0        0        0      626 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/angle-tool.svg
+-rw-r--r--   0        0        0      671 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/antenna-off.svg
+-rw-r--r--   0        0        0      911 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/antenna-signal-tag.svg
+-rw-r--r--   0        0        0      861 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/antenna-signal.svg
+-rw-r--r--   0        0        0      776 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/antenna.svg
+-rw-r--r--   0        0        0      490 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/app-notification.svg
+-rw-r--r--   0        0        0      705 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/app-store.svg
+-rw-r--r--   0        0        0      676 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/app-window.svg
+-rw-r--r--   0        0        0      910 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple-half.svg
+-rw-r--r--   0        0        0      360 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple-imac-2021-side.svg
+-rw-r--r--   0        0        0      430 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple-imac-2021.svg
+-rw-r--r--   0        0        0      680 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple-mac.svg
+-rw-r--r--   0        0        0      675 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple-shortcuts.svg
+-rw-r--r--   0        0        0     1015 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple-swift.svg
+-rw-r--r--   0        0        0      574 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple-wallet.svg
+-rw-r--r--   0        0        0      754 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple.svg
+-rw-r--r--   0        0        0      710 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ar-tag.svg
+-rw-r--r--   0        0        0      834 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arc-3d-center-point.svg
+-rw-r--r--   0        0        0      694 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arc-3d.svg
+-rw-r--r--   0        0        0     1053 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arcade.svg
+-rw-r--r--   0        0        0      604 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/archery-match.svg
+-rw-r--r--   0        0        0      476 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/archery.svg
+-rw-r--r--   0        0        0      670 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/archive.svg
+-rw-r--r--   0        0        0     1036 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/area-search.svg
+-rw-r--r--   0        0        0      363 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-archery.svg
+-rw-r--r--   0        0        0      438 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-down-circle.svg
+-rw-r--r--   0        0        0      479 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-down-left-circle.svg
+-rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-down-left-square.svg
+-rw-r--r--   0        0        0      237 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-down-left.svg
+-rw-r--r--   0        0        0      479 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-down-right-circle.svg
+-rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-down-right-square.svg
+-rw-r--r--   0        0        0      254 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-down-right.svg
+-rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-down-tag.svg
+-rw-r--r--   0        0        0      246 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-down.svg
+-rw-r--r--   0        0        0      253 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-email-forward.svg
+-rw-r--r--   0        0        0      507 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-enlarge-tag.svg
+-rw-r--r--   0        0        0      436 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-left-circle.svg
+-rw-r--r--   0        0        0      427 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-left-tag.svg
+-rw-r--r--   0        0        0      244 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-left.svg
+-rw-r--r--   0        0        0      532 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-reduce-tag.svg
+-rw-r--r--   0        0        0      438 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-right-circle.svg
+-rw-r--r--   0        0        0      427 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-right-tag.svg
+-rw-r--r--   0        0        0      246 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-right.svg
+-rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-separate-vertical.svg
+-rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-separate.svg
+-rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-union-vertical.svg
+-rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-union.svg
+-rw-r--r--   0        0        0      436 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-up-circle.svg
+-rw-r--r--   0        0        0      479 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-up-left-circle.svg
+-rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-up-left-square.svg
+-rw-r--r--   0        0        0      238 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-up-left.svg
+-rw-r--r--   0        0        0      479 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-up-right-circle.svg
+-rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-up-right-square.svg
+-rw-r--r--   0        0        0      262 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-up-right.svg
+-rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-up-tag.svg
+-rw-r--r--   0        0        0      244 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-up.svg
+-rw-r--r--   0        0        0      433 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrows-up-from-line.svg
+-rw-r--r--   0        0        0      765 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/asana.svg
+-rw-r--r--   0        0        0      443 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/asterisk.svg
+-rw-r--r--   0        0        0      881 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/at-sign-circle.svg
+-rw-r--r--   0        0        0      667 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/at-sign.svg
+-rw-r--r--   0        0        0     1016 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/atom.svg
+-rw-r--r--   0        0        0      822 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/attachment.svg
+-rw-r--r--   0        0        0      738 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/augmented-reality.svg
+-rw-r--r--   0        0        0      393 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/auto-flash.svg
+-rw-r--r--   0        0        0      750 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/avi-format.svg
+-rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/axes.svg
+-rw-r--r--   0        0        0      741 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/backward-15-seconds.svg
+-rw-r--r--   0        0        0     1312 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/badge-check.svg
+-rw-r--r--   0        0        0      507 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bag.svg
+-rw-r--r--   0        0        0      914 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/balcony.svg
+-rw-r--r--   0        0        0      785 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bank.svg
+-rw-r--r--   0        0        0      795 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/barcode.svg
+-rw-r--r--   0        0        0      805 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/basketball-field.svg
+-rw-r--r--   0        0        0      960 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/basketball.svg
+-rw-r--r--   0        0        0      854 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bathroom.svg
+-rw-r--r--   0        0        0      574 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-25.svg
+-rw-r--r--   0        0        0      577 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-50.svg
+-rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-75.svg
+-rw-r--r--   0        0        0      502 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-charging.svg
+-rw-r--r--   0        0        0      387 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-empty.svg
+-rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-full.svg
+-rw-r--r--   0        0        0      594 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-indicator.svg
+-rw-r--r--   0        0        0      494 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-slash.svg
+-rw-r--r--   0        0        0      591 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-warning.svg
+-rw-r--r--   0        0        0     1186 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bbq.svg
+-rw-r--r--   0        0        0      624 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/beach-bag.svg
+-rw-r--r--   0        0        0      589 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bed-ready.svg
+-rw-r--r--   0        0        0      517 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bed.svg
+-rw-r--r--   0        0        0     1031 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/behance-tag.svg
+-rw-r--r--   0        0        0      814 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/behance.svg
+-rw-r--r--   0        0        0      838 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bell-notification.svg
+-rw-r--r--   0        0        0      862 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bell-off.svg
+-rw-r--r--   0        0        0      678 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bell.svg
+-rw-r--r--   0        0        0      909 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bicycle.svg
+-rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bin-full.svg
+-rw-r--r--   0        0        0     1025 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bin-half.svg
+-rw-r--r--   0        0        0      767 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bin-minus-in.svg
+-rw-r--r--   0        0        0      806 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bin-plus-in.svg
+-rw-r--r--   0        0        0      658 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bin.svg
+-rw-r--r--   0        0        0      939 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/binocular.svg
+-rw-r--r--   0        0        0     1134 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/birthday-cake.svg
+-rw-r--r--   0        0        0      936 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bishop.svg
+-rw-r--r--   0        0        0      716 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bitbucket.svg
+-rw-r--r--   0        0        0      807 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bitcoin-circle.svg
+-rw-r--r--   0        0        0     1207 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bitcoin-rotate-out.svg
+-rw-r--r--   0        0        0      419 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bluetooth-tag.svg
+-rw-r--r--   0        0        0      251 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bluetooth.svg
+-rw-r--r--   0        0        0      588 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bold-square.svg
+-rw-r--r--   0        0        0      442 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bold.svg
+-rw-r--r--   0        0        0      807 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bonfire.svg
+-rw-r--r--   0        0        0      826 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/book-lock.svg
+-rw-r--r--   0        0        0      810 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/book-stack.svg
+-rw-r--r--   0        0        0      601 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/book.svg
+-rw-r--r--   0        0        0      640 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bookmark-book.svg
+-rw-r--r--   0        0        0      535 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bookmark-circle.svg
+-rw-r--r--   0        0        0      337 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bookmark.svg
+-rw-r--r--   0        0        0      943 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-bl.svg
+-rw-r--r--   0        0        0     1455 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-bottom.svg
+-rw-r--r--   0        0        0      961 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-br.svg
+-rw-r--r--   0        0        0     1480 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-inner.svg
+-rw-r--r--   0        0        0     1461 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-left.svg
+-rw-r--r--   0        0        0      892 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-out.svg
+-rw-r--r--   0        0        0     1499 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-right.svg
+-rw-r--r--   0        0        0      946 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-tl.svg
+-rw-r--r--   0        0        0     1461 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-top.svg
+-rw-r--r--   0        0        0      982 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-tr.svg
+-rw-r--r--   0        0        0      440 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bounce-left.svg
+-rw-r--r--   0        0        0      447 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bounce-right.svg
+-rw-r--r--   0        0        0      992 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bowling-ball.svg
+-rw-r--r--   0        0        0     1318 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/box-3d-center.svg
+-rw-r--r--   0        0        0     1046 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/box-3d-point.svg
+-rw-r--r--   0        0        0     1470 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/box-3d-three-points.svg
+-rw-r--r--   0        0        0      927 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/box-iso.svg
+-rw-r--r--   0        0        0      463 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/box.svg
+-rw-r--r--   0        0        0      796 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/boxing-glove.svg
+-rw-r--r--   0        0        0     1906 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/brain-electricity.svg
+-rw-r--r--   0        0        0     2150 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/brain-research.svg
+-rw-r--r--   0        0        0     2085 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/brain-warning.svg
+-rw-r--r--   0        0        0     2005 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/brain.svg
+-rw-r--r--   0        0        0      518 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bread-slice.svg
+-rw-r--r--   0        0        0      861 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bridge-3d.svg
+-rw-r--r--   0        0        0      888 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bridge-surface.svg
+-rw-r--r--   0        0        0     1003 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bright-crown.svg
+-rw-r--r--   0        0        0     1346 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bright-star.svg
+-rw-r--r--   0        0        0     1090 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/brightness-window.svg
+-rw-r--r--   0        0        0      756 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/brightness.svg
+-rw-r--r--   0        0        0      534 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-download.svg
+-rw-r--r--   0        0        0      535 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-income.svg
+-rw-r--r--   0        0        0      535 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-outcome.svg
+-rw-r--r--   0        0        0      771 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-search.svg
+-rw-r--r--   0        0        0      917 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-star.svg
+-rw-r--r--   0        0        0      534 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-upload.svg
+-rw-r--r--   0        0        0      621 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-warning.svg
+-rw-r--r--   0        0        0      635 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-xmark.svg
+-rw-r--r--   0        0        0     1005 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/building.svg
+-rw-r--r--   0        0        0     1173 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bus-green.svg
+-rw-r--r--   0        0        0      978 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bus-stop.svg
+-rw-r--r--   0        0        0     1013 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/bus.svg
+-rw-r--r--   0        0        0      573 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/c-square.svg
+-rw-r--r--   0        0        0      408 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cable-tag.svg
+-rw-r--r--   0        0        0      880 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/calculator.svg
+-rw-r--r--   0        0        0      691 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/calendar-minus.svg
+-rw-r--r--   0        0        0      738 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/calendar-plus.svg
+-rw-r--r--   0        0        0      623 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/calendar.svg
+-rw-r--r--   0        0        0      683 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/camera.svg
+-rw-r--r--   0        0        0     1332 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/candlestick-chart.svg
+-rw-r--r--   0        0        0      843 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/car.svg
+-rw-r--r--   0        0        0      680 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/card-lock.svg
+-rw-r--r--   0        0        0      654 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/card-no-access.svg
+-rw-r--r--   0        0        0      487 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/card-reader.svg
+-rw-r--r--   0        0        0      650 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/card-shield.svg
+-rw-r--r--   0        0        0      702 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/card-wallet.svg
+-rw-r--r--   0        0        0     1035 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cart-alt.svg
+-rw-r--r--   0        0        0      635 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cart-minus.svg
+-rw-r--r--   0        0        0      681 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cart-plus.svg
+-rw-r--r--   0        0        0      875 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cart.svg
+-rw-r--r--   0        0        0      743 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cash.svg
+-rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cell-2x2.svg
+-rw-r--r--   0        0        0      644 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cellar.svg
+-rw-r--r--   0        0        0     1879 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/center-align.svg
+-rw-r--r--   0        0        0      477 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-bubble-check.svg
+-rw-r--r--   0        0        0      378 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-bubble-empty.svg
+-rw-r--r--   0        0        0      627 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-bubble-question.svg
+-rw-r--r--   0        0        0      711 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-bubble-translate.svg
+-rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-bubble-warning.svg
+-rw-r--r--   0        0        0      540 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-bubble-xmark.svg
+-rw-r--r--   0        0        0     1110 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-bubble.svg
+-rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-lines.svg
+-rw-r--r--   0        0        0      474 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-minus-in.svg
+-rw-r--r--   0        0        0      494 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-plus-in.svg
+-rw-r--r--   0        0        0      421 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/check-circle.svg
+-rw-r--r--   0        0        0      418 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/check-square.svg
+-rw-r--r--   0        0        0      219 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/check.svg
+-rw-r--r--   0        0        0      532 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chocolate.svg
+-rw-r--r--   0        0        0     1059 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chromecast-active.svg
+-rw-r--r--   0        0        0      613 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/chromecast.svg
+-rw-r--r--   0        0        0      984 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/church-side.svg
+-rw-r--r--   0        0        0      951 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/church.svg
+-rw-r--r--   0        0        0      811 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cigarette-slash.svg
+-rw-r--r--   0        0        0     1110 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cinema-old.svg
+-rw-r--r--   0        0        0      485 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/circle-spark.svg
+-rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/circle.svg
+-rw-r--r--   0        0        0     1081 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/city.svg
+-rw-r--r--   0        0        0      789 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/clipboard-check.svg
+-rw-r--r--   0        0        0      562 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/clock-rotate-right.svg
+-rw-r--r--   0        0        0      416 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/clock.svg
+-rw-r--r--   0        0        0      776 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/closed-captions-tag.svg
+-rw-r--r--   0        0        0      517 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/closet.svg
+-rw-r--r--   0        0        0      464 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-bookmark.svg
+-rw-r--r--   0        0        0      449 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-check.svg
+-rw-r--r--   0        0        0      999 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-desync.svg
+-rw-r--r--   0        0        0      472 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-download.svg
+-rw-r--r--   0        0        0      556 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-square.svg
+-rw-r--r--   0        0        0      962 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-sunny.svg
+-rw-r--r--   0        0        0      999 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-sync.svg
+-rw-r--r--   0        0        0      472 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-upload.svg
+-rw-r--r--   0        0        0      498 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-xmark.svg
+-rw-r--r--   0        0        0      306 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud.svg
+-rw-r--r--   0        0        0     1032 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/code-brackets-square.svg
+-rw-r--r--   0        0        0      707 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/code-brackets.svg
+-rw-r--r--   0        0        0      430 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/code.svg
+-rw-r--r--   0        0        0      701 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/codepen.svg
+-rw-r--r--   0        0        0      801 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/coffee-cup.svg
+-rw-r--r--   0        0        0     1144 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/coin-slash.svg
+-rw-r--r--   0        0        0      841 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/coins-swap.svg
+-rw-r--r--   0        0        0     1376 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/coins.svg
+-rw-r--r--   0        0        0      439 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/collage-frame.svg
+-rw-r--r--   0        0        0      550 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/collapse.svg
+-rw-r--r--   0        0        0      759 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/color-filter.svg
+-rw-r--r--   0        0        0      920 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/color-picker.svg
+-rw-r--r--   0        0        0     1324 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/color-wheel.svg
+-rw-r--r--   0        0        0      562 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/combine.svg
+-rw-r--r--   0        0        0      944 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/commodity.svg
+-rw-r--r--   0        0        0     1100 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/community.svg
+-rw-r--r--   0        0        0      372 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/comp-align-bottom.svg
+-rw-r--r--   0        0        0      371 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/comp-align-left.svg
+-rw-r--r--   0        0        0      372 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/comp-align-right.svg
+-rw-r--r--   0        0        0      370 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/comp-align-top.svg
+-rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/compact-disc.svg
+-rw-r--r--   0        0        0      481 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/compass.svg
+-rw-r--r--   0        0        0     1336 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/component.svg
+-rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/compress-lines.svg
+-rw-r--r--   0        0        0      437 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/compress.svg
+-rw-r--r--   0        0        0      501 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/computer.svg
+-rw-r--r--   0        0        0     1753 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/constrained-surface.svg
+-rw-r--r--   0        0        0      948 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/consumable.svg
+-rw-r--r--   0        0        0      569 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/contactless.svg
+-rw-r--r--   0        0        0      500 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/control-slider.svg
+-rw-r--r--   0        0        0     1249 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cookie.svg
+-rw-r--r--   0        0        0      507 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cooling-square.svg
+-rw-r--r--   0        0        0      527 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/copy.svg
+-rw-r--r--   0        0        0      545 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/copyright.svg
+-rw-r--r--   0        0        0     1481 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/corner-bottom-left.svg
+-rw-r--r--   0        0        0     1447 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/corner-bottom-right.svg
+-rw-r--r--   0        0        0     1366 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/corner-top-left.svg
+-rw-r--r--   0        0        0     1432 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/corner-top-right.svg
+-rw-r--r--   0        0        0     1501 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cpu-warning.svg
+-rw-r--r--   0        0        0     1638 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cpu.svg
+-rw-r--r--   0        0        0      427 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cracked-egg.svg
+-rw-r--r--   0        0        0      781 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/creative-commons.svg
+-rw-r--r--   0        0        0      608 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/credit-card-slash.svg
+-rw-r--r--   0        0        0      333 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/credit-card.svg
+-rw-r--r--   0        0        0      569 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/credit-cards.svg
+-rw-r--r--   0        0        0     1158 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/crib.svg
+-rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/crop-rotate-bl.svg
+-rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/crop-rotate-br.svg
+-rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/crop-rotate-tl.svg
+-rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/crop-rotate-tr.svg
+-rw-r--r--   0        0        0      306 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/crop.svg
+-rw-r--r--   0        0        0      464 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/crown-circle.svg
+-rw-r--r--   0        0        0      254 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/crown.svg
+-rw-r--r--   0        0        0      470 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/css3.svg
+-rw-r--r--   0        0        0     1398 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cube-bandage.svg
+-rw-r--r--   0        0        0     1095 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cube-cut-with-curve.svg
+-rw-r--r--   0        0        0      991 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cube-hole.svg
+-rw-r--r--   0        0        0      883 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cube-replace-face.svg
+-rw-r--r--   0        0        0      834 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cube.svg
+-rw-r--r--   0        0        0      437 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cursor-pointer.svg
+-rw-r--r--   0        0        0      918 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/curve-array.svg
+-rw-r--r--   0        0        0      816 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cut.svg
+-rw-r--r--   0        0        0      715 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cutlery.svg
+-rw-r--r--   0        0        0      862 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cycling.svg
+-rw-r--r--   0        0        0      506 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/cylinder.svg
+-rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dash-flag.svg
+-rw-r--r--   0        0        0     1363 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dashboard-dots.svg
+-rw-r--r--   0        0        0     1101 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dashboard-speed.svg
+-rw-r--r--   0        0        0      760 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dashboard.svg
+-rw-r--r--   0        0        0      342 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/data-transfer-both.svg
+-rw-r--r--   0        0        0      442 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/data-transfer-check.svg
+-rw-r--r--   0        0        0      530 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/data-transfer-down.svg
+-rw-r--r--   0        0        0      524 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/data-transfer-up.svg
+-rw-r--r--   0        0        0      723 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/data-transfer-warning.svg
+-rw-r--r--   0        0        0     1293 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-backup.svg
+-rw-r--r--   0        0        0      596 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-check.svg
+-rw-r--r--   0        0        0      611 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-export.svg
+-rw-r--r--   0        0        0      638 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-monitor.svg
+-rw-r--r--   0        0        0      611 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-restore.svg
+-rw-r--r--   0        0        0      575 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-script-minus.svg
+-rw-r--r--   0        0        0      627 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-script-plus.svg
+-rw-r--r--   0        0        0      502 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-script.svg
+-rw-r--r--   0        0        0      853 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-search.svg
+-rw-r--r--   0        0        0     1009 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-settings.svg
+-rw-r--r--   0        0        0      984 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-star.svg
+-rw-r--r--   0        0        0      697 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-stats.svg
+-rw-r--r--   0        0        0      742 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-tag.svg
+-rw-r--r--   0        0        0      695 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-warning.svg
+-rw-r--r--   0        0        0      702 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-xmark.svg
+-rw-r--r--   0        0        0      433 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/database.svg
+-rw-r--r--   0        0        0      437 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/de-compress.svg
+-rw-r--r--   0        0        0     1151 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/delivery-truck.svg
+-rw-r--r--   0        0        0      496 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/delivery.svg
+-rw-r--r--   0        0        0     1090 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/depth.svg
+-rw-r--r--   0        0        0     1180 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/design-nib.svg
+-rw-r--r--   0        0        0      608 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/design-pencil.svg
+-rw-r--r--   0        0        0      862 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/desk.svg
+-rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/developer.svg
+-rw-r--r--   0        0        0     1279 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dew-point.svg
+-rw-r--r--   0        0        0     2397 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dialpad.svg
+-rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/diameter.svg
+-rw-r--r--   0        0        0     1436 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dice-five.svg
+-rw-r--r--   0        0        0     1188 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dice-four.svg
+-rw-r--r--   0        0        0      544 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dice-one.svg
+-rw-r--r--   0        0        0     1663 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dice-six.svg
+-rw-r--r--   0        0        0      990 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dice-three.svg
+-rw-r--r--   0        0        0      742 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dice-two.svg
+-rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dimmer-switch.svg
+-rw-r--r--   0        0        0      718 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/director-chair.svg
+-rw-r--r--   0        0        0     1079 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/discord.svg
+-rw-r--r--   0        0        0      940 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dishwasher.svg
+-rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/display-4k.svg
+-rw-r--r--   0        0        0      932 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/divide-three.svg
+-rw-r--r--   0        0        0      669 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/divide.svg
+-rw-r--r--   0        0        0      744 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dna.svg
+-rw-r--r--   0        0        0     1249 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dns.svg
+-rw-r--r--   0        0        0      907 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/doc-magnifying-glass-in.svg
+-rw-r--r--   0        0        0      844 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/doc-magnifying-glass.svg
+-rw-r--r--   0        0        0     1022 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/doc-star-in.svg
+-rw-r--r--   0        0        0      988 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/doc-star.svg
+-rw-r--r--   0        0        0      630 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dogecoin-circle.svg
+-rw-r--r--   0        0        0     1030 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dogecoin-rotate-out.svg
+-rw-r--r--   0        0        0      633 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dollar-circle.svg
+-rw-r--r--   0        0        0      499 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dollar.svg
+-rw-r--r--   0        0        0      621 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/domotic-warning.svg
+-rw-r--r--   0        0        0     1620 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/donate.svg
+-rw-r--r--   0        0        0      430 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dot-arrow-down.svg
+-rw-r--r--   0        0        0      432 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dot-arrow-left.svg
+-rw-r--r--   0        0        0      427 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dot-arrow-right.svg
+-rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dot-arrow-up.svg
+-rw-r--r--   0        0        0      459 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/double-check.svg
+-rw-r--r--   0        0        0      529 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/download-circle.svg
+-rw-r--r--   0        0        0      796 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/download-data-window.svg
+-rw-r--r--   0        0        0      528 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/download-square.svg
+-rw-r--r--   0        0        0      336 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/download.svg
+-rw-r--r--   0        0        0     1610 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/drag-hand-gesture.svg
+-rw-r--r--   0        0        0      554 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/drag.svg
+-rw-r--r--   0        0        0      978 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/drawer.svg
+-rw-r--r--   0        0        0      723 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/dribbble.svg
+-rw-r--r--   0        0        0     1871 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-charge-full.svg
+-rw-r--r--   0        0        0     1780 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-charge-half.svg
+-rw-r--r--   0        0        0     1689 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-charge-low.svg
+-rw-r--r--   0        0        0     1562 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-check.svg
+-rw-r--r--   0        0        0     1587 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-landing.svg
+-rw-r--r--   0        0        0     1977 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-refresh.svg
+-rw-r--r--   0        0        0     1587 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-take-off.svg
+-rw-r--r--   0        0        0     1652 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-xmark.svg
+-rw-r--r--   0        0        0     1696 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone.svg
+-rw-r--r--   0        0        0      529 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/droplet-check.svg
+-rw-r--r--   0        0        0      312 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/droplet-half.svg
+-rw-r--r--   0        0        0      260 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/droplet.svg
+-rw-r--r--   0        0        0      809 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ease-curve-control-points.svg
+-rw-r--r--   0        0        0      526 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ease-in-control-point.svg
+-rw-r--r--   0        0        0      225 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ease-in-out.svg
+-rw-r--r--   0        0        0      225 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ease-in.svg
+-rw-r--r--   0        0        0      507 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ease-out-control-point.svg
+-rw-r--r--   0        0        0      224 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ease-out.svg
+-rw-r--r--   0        0        0      975 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ecology-book.svg
+-rw-r--r--   0        0        0      614 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/edit-pencil.svg
+-rw-r--r--   0        0        0      565 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/edit.svg
+-rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/egg.svg
+-rw-r--r--   0        0        0      942 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/eject.svg
+-rw-r--r--   0        0        0     1268 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/electronics-chip.svg
+-rw-r--r--   0        0        0      350 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/electronics-transistor.svg
+-rw-r--r--   0        0        0      636 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/elevator.svg
+-rw-r--r--   0        0        0     1281 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ellipse-3d-three-points.svg
+-rw-r--r--   0        0        0      750 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ellipse-3d.svg
+-rw-r--r--   0        0        0      339 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-ball.svg
+-rw-r--r--   0        0        0      688 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-blink-left.svg
+-rw-r--r--   0        0        0      681 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-blink-right.svg
+-rw-r--r--   0        0        0      779 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-look-down.svg
+-rw-r--r--   0        0        0      587 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-look-left.svg
+-rw-r--r--   0        0        0      600 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-look-right.svg
+-rw-r--r--   0        0        0      761 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-look-up.svg
+-rw-r--r--   0        0        0     1126 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-puzzled.svg
+-rw-r--r--   0        0        0      760 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-quite.svg
+-rw-r--r--   0        0        0      339 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-really.svg
+-rw-r--r--   0        0        0      895 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-sad.svg
+-rw-r--r--   0        0        0      474 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-satisfied.svg
+-rw-r--r--   0        0        0     1349 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-sing-left-note.svg
+-rw-r--r--   0        0        0      947 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-sing-left.svg
+-rw-r--r--   0        0        0     1376 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-sing-right-note.svg
+-rw-r--r--   0        0        0     1388 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-sing-right.svg
+-rw-r--r--   0        0        0      953 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-surprise-alt.svg
+-rw-r--r--   0        0        0      973 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-surprise.svg
+-rw-r--r--   0        0        0      397 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-talking-angry.svg
+-rw-r--r--   0        0        0      397 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-talking-happy.svg
+-rw-r--r--   0        0        0      759 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-think-left.svg
+-rw-r--r--   0        0        0      761 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-think-right.svg
+-rw-r--r--   0        0        0      895 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji.svg
+-rw-r--r--   0        0        0      534 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/empty-page.svg
+-rw-r--r--   0        0        0      789 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/energy-usage-window.svg
+-rw-r--r--   0        0        0      336 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/enlarge.svg
+-rw-r--r--   0        0        0      707 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/erase.svg
+-rw-r--r--   0        0        0      471 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ethereum-circle.svg
+-rw-r--r--   0        0        0      871 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ethereum-rotate-out.svg
+-rw-r--r--   0        0        0      718 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/euro-square.svg
+-rw-r--r--   0        0        0      520 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/euro.svg
+-rw-r--r--   0        0        0      838 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-charge-alt.svg
+-rw-r--r--   0        0        0      667 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-charge.svg
+-rw-r--r--   0        0        0      698 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-plug-charging.svg
+-rw-r--r--   0        0        0      791 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-plug-xmark.svg
+-rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-plug.svg
+-rw-r--r--   0        0        0      618 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-station.svg
+-rw-r--r--   0        0        0      589 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-tag.svg
+-rw-r--r--   0        0        0      890 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/exclude.svg
+-rw-r--r--   0        0        0      529 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/expand-lines.svg
+-rw-r--r--   0        0        0      550 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/expand.svg
+-rw-r--r--   0        0        0      947 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/extrude.svg
+-rw-r--r--   0        0        0      532 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/eye-closed.svg
+-rw-r--r--   0        0        0      426 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/eye.svg
+-rw-r--r--   0        0        0      529 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/f-square.svg
+-rw-r--r--   0        0        0     1030 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/face-3d-draft.svg
+-rw-r--r--   0        0        0      999 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/face-id.svg
+-rw-r--r--   0        0        0      545 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/facebook-tag.svg
+-rw-r--r--   0        0        0      397 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/facebook.svg
+-rw-r--r--   0        0        0      697 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/facetime.svg
+-rw-r--r--   0        0        0      532 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/farm.svg
+-rw-r--r--   0        0        0      526 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-arrow-down-square.svg
+-rw-r--r--   0        0        0      318 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-arrow-down.svg
+-rw-r--r--   0        0        0      527 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-arrow-left-square.svg
+-rw-r--r--   0        0        0      319 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-arrow-left.svg
+-rw-r--r--   0        0        0      522 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-arrow-right-square.svg
+-rw-r--r--   0        0        0      318 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-arrow-right.svg
+-rw-r--r--   0        0        0      527 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-arrow-up-square.svg
+-rw-r--r--   0        0        0      319 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-arrow-up.svg
+-rw-r--r--   0        0        0      529 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-down-circle.svg
+-rw-r--r--   0        0        0      530 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-left-circle.svg
+-rw-r--r--   0        0        0      525 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-right-circle.svg
+-rw-r--r--   0        0        0      530 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-up-circle.svg
+-rw-r--r--   0        0        0     1002 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/favourite-book.svg
+-rw-r--r--   0        0        0     1140 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/favourite-window.svg
+-rw-r--r--   0        0        0      351 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/female.svg
+-rw-r--r--   0        0        0     2104 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/figma.svg
+-rw-r--r--   0        0        0      869 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/file-not-found.svg
+-rw-r--r--   0        0        0      844 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fill-color.svg
+-rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fillet-3d.svg
+-rw-r--r--   0        0        0      565 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/filter-alt.svg
+-rw-r--r--   0        0        0      595 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/filter-list-circle.svg
+-rw-r--r--   0        0        0      398 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/filter-list.svg
+-rw-r--r--   0        0        0      674 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/filter.svg
+-rw-r--r--   0        0        0      789 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/finder.svg
+-rw-r--r--   0        0        0      854 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-check-circle.svg
+-rw-r--r--   0        0        0      734 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-circle.svg
+-rw-r--r--   0        0        0     1154 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-lock-circle.svg
+-rw-r--r--   0        0        0      907 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-scan.svg
+-rw-r--r--   0        0        0      759 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-square.svg
+-rw-r--r--   0        0        0     1092 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-window.svg
+-rw-r--r--   0        0        0      948 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-xmark-circle.svg
+-rw-r--r--   0        0        0     1165 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint.svg
+-rw-r--r--   0        0        0      502 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fire-flame.svg
+-rw-r--r--   0        0        0      668 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fish.svg
+-rw-r--r--   0        0        0      365 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fishing.svg
+-rw-r--r--   0        0        0      709 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/flare.svg
+-rw-r--r--   0        0        0      365 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/flash-off.svg
+-rw-r--r--   0        0        0      233 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/flash.svg
+-rw-r--r--   0        0        0      867 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/flask.svg
+-rw-r--r--   0        0        0      717 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/flip-reverse.svg
+-rw-r--r--   0        0        0      724 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/flip.svg
+-rw-r--r--   0        0        0      942 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/floppy-disk-arrow-in.svg
+-rw-r--r--   0        0        0      884 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/floppy-disk-arrow-out.svg
+-rw-r--r--   0        0        0      691 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/floppy-disk.svg
+-rw-r--r--   0        0        0     2393 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/flower.svg
+-rw-r--r--   0        0        0      623 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fog.svg
+-rw-r--r--   0        0        0      632 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/folder-minus.svg
+-rw-r--r--   0        0        0      651 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/folder-plus.svg
+-rw-r--r--   0        0        0     1172 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/folder-settings.svg
+-rw-r--r--   0        0        0      703 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/folder-warning.svg
+-rw-r--r--   0        0        0      460 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/folder.svg
+-rw-r--r--   0        0        0      646 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/font-question.svg
+-rw-r--r--   0        0        0     1012 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/football-ball.svg
+-rw-r--r--   0        0        0      709 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/football.svg
+-rw-r--r--   0        0        0      743 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/forward-15-seconds.svg
+-rw-r--r--   0        0        0      546 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/forward-message.svg
+-rw-r--r--   0        0        0      649 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/forward.svg
+-rw-r--r--   0        0        0      490 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame-alt-empty.svg
+-rw-r--r--   0        0        0      700 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame-alt.svg
+-rw-r--r--   0        0        0     1300 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame-minus-in.svg
+-rw-r--r--   0        0        0     1326 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame-plus-in.svg
+-rw-r--r--   0        0        0     1620 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame-select.svg
+-rw-r--r--   0        0        0     1209 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame-simple.svg
+-rw-r--r--   0        0        0      402 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame-tool.svg
+-rw-r--r--   0        0        0     2373 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame.svg
+-rw-r--r--   0        0        0      515 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fridge.svg
+-rw-r--r--   0        0        0      627 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fx-tag.svg
+-rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/fx.svg
+-rw-r--r--   0        0        0     1456 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/gamepad.svg
+-rw-r--r--   0        0        0      305 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/garage.svg
+-rw-r--r--   0        0        0     1069 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/gas-tank-droplet.svg
+-rw-r--r--   0        0        0      916 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/gas-tank.svg
+-rw-r--r--   0        0        0      454 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/gas.svg
+-rw-r--r--   0        0        0      784 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/gif-format.svg
+-rw-r--r--   0        0        0     1103 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/gift.svg
+-rw-r--r--   0        0        0      709 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-branch.svg
+-rw-r--r--   0        0        0      662 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-cherry-pick-commit.svg
+-rw-r--r--   0        0        0      500 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-commit.svg
+-rw-r--r--   0        0        0      957 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-compare.svg
+-rw-r--r--   0        0        0      912 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-fork.svg
+-rw-r--r--   0        0        0      708 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-merge.svg
+-rw-r--r--   0        0        0      899 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-pull-request-closed.svg
+-rw-r--r--   0        0        0     1025 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-pull-request.svg
+-rw-r--r--   0        0        0     1152 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/github-circle.svg
+-rw-r--r--   0        0        0      945 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/github.svg
+-rw-r--r--   0        0        0      718 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/gitlab-full.svg
+-rw-r--r--   0        0        0      754 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/glass-empty.svg
+-rw-r--r--   0        0        0      594 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/glass-fragile.svg
+-rw-r--r--   0        0        0      963 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/glass-half-alt.svg
+-rw-r--r--   0        0        0      936 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/glass-half.svg
+-rw-r--r--   0        0        0      624 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/glasses.svg
+-rw-r--r--   0        0        0      807 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/globe.svg
+-rw-r--r--   0        0        0      538 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/golf.svg
+-rw-r--r--   0        0        0      522 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-circle.svg
+-rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-docs.svg
+-rw-r--r--   0        0        0      473 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-drive-check.svg
+-rw-r--r--   0        0        0     1016 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-drive-sync.svg
+-rw-r--r--   0        0        0      572 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-drive-warning.svg
+-rw-r--r--   0        0        0      402 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-drive.svg
+-rw-r--r--   0        0        0      738 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-home.svg
+-rw-r--r--   0        0        0      647 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-one.svg
+-rw-r--r--   0        0        0      529 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/google.svg
+-rw-r--r--   0        0        0      799 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/gps.svg
+-rw-r--r--   0        0        0      852 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/graduation-cap.svg
+-rw-r--r--   0        0        0      322 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/graph-down.svg
+-rw-r--r--   0        0        0      323 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/graph-up.svg
+-rw-r--r--   0        0        0      808 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/grid-minus.svg
+-rw-r--r--   0        0        0      847 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/grid-plus.svg
+-rw-r--r--   0        0        0      887 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/grid-xmark.svg
+-rw-r--r--   0        0        0      754 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/group.svg
+-rw-r--r--   0        0        0     1092 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/gym.svg
+-rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/h-square.svg
+-rw-r--r--   0        0        0     1633 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/half-cookie.svg
+-rw-r--r--   0        0        0      363 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/half-moon.svg
+-rw-r--r--   0        0        0      617 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hammer.svg
+-rw-r--r--   0        0        0      724 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hand-brake.svg
+-rw-r--r--   0        0        0      723 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hand-card.svg
+-rw-r--r--   0        0        0     1043 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hand-cash.svg
+-rw-r--r--   0        0        0      869 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hand-contactless.svg
+-rw-r--r--   0        0        0      418 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/handbag.svg
+-rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hard-drive.svg
+-rw-r--r--   0        0        0      394 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hashtag.svg
+-rw-r--r--   0        0        0      377 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hat.svg
+-rw-r--r--   0        0        0      567 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hd-display.svg
+-rw-r--r--   0        0        0      380 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hd.svg
+-rw-r--r--   0        0        0      669 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hdr.svg
+-rw-r--r--   0        0        0      827 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/headset-bolt.svg
+-rw-r--r--   0        0        0      916 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/headset-help.svg
+-rw-r--r--   0        0        0      917 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/headset-warning.svg
+-rw-r--r--   0        0        0      720 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/headset.svg
+-rw-r--r--   0        0        0      637 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/health-shield.svg
+-rw-r--r--   0        0        0     1326 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/healthcare.svg
+-rw-r--r--   0        0        0      830 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/heart-arrow-down.svg
+-rw-r--r--   0        0        0      590 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/heart.svg
+-rw-r--r--   0        0        0      799 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/heating-square.svg
+-rw-r--r--   0        0        0      622 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/heavy-rain.svg
+-rw-r--r--   0        0        0      566 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/help-circle.svg
+-rw-r--r--   0        0        0      563 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/help-square.svg
+-rw-r--r--   0        0        0      653 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/heptagon.svg
+-rw-r--r--   0        0        0     1207 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hexagon-dice.svg
+-rw-r--r--   0        0        0      683 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hexagon-plus.svg
+-rw-r--r--   0        0        0      567 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hexagon.svg
+-rw-r--r--   0        0        0      626 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/historic-shield-alt.svg
+-rw-r--r--   0        0        0      440 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/historic-shield.svg
+-rw-r--r--   0        0        0      517 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-alt-slim-horiz.svg
+-rw-r--r--   0        0        0      517 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-alt-slim.svg
+-rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-alt.svg
+-rw-r--r--   0        0        0      548 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-hospital.svg
+-rw-r--r--   0        0        0      824 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-sale.svg
+-rw-r--r--   0        0        0      720 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-secure.svg
+-rw-r--r--   0        0        0      763 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-shield.svg
+-rw-r--r--   0        0        0      516 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-simple-door.svg
+-rw-r--r--   0        0        0      528 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-simple.svg
+-rw-r--r--   0        0        0      490 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-table.svg
+-rw-r--r--   0        0        0      900 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-temperature-in.svg
+-rw-r--r--   0        0        0      980 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-temperature-out.svg
+-rw-r--r--   0        0        0      544 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-user.svg
+-rw-r--r--   0        0        0      426 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/home.svg
+-rw-r--r--   0        0        0      476 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/horiz-distribution-left.svg
+-rw-r--r--   0        0        0      481 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/horiz-distribution-right.svg
+-rw-r--r--   0        0        0      549 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/horizontal-merge.svg
+-rw-r--r--   0        0        0      547 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/horizontal-split.svg
+-rw-r--r--   0        0        0      464 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hospital-circle.svg
+-rw-r--r--   0        0        0     1207 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hospital.svg
+-rw-r--r--   0        0        0      775 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hot-air-balloon.svg
+-rw-r--r--   0        0        0      519 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/hourglass.svg
+-rw-r--r--   0        0        0      899 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/house-rooms.svg
+-rw-r--r--   0        0        0      386 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/html5.svg
+-rw-r--r--   0        0        0      594 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ice-cream.svg
+-rw-r--r--   0        0        0      523 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/iconoir.svg
+-rw-r--r--   0        0        0      396 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/import.svg
+-rw-r--r--   0        0        0      380 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/inclination.svg
+-rw-r--r--   0        0        0      562 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/industry.svg
+-rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/infinite.svg
+-rw-r--r--   0        0        0      516 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/info-circle.svg
+-rw-r--r--   0        0        0      460 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/input-field.svg
+-rw-r--r--   0        0        0      426 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/input-output.svg
+-rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/input-search.svg
+-rw-r--r--   0        0        0      597 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/instagram.svg
+-rw-r--r--   0        0        0     1079 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/internet.svg
+-rw-r--r--   0        0        0     1890 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/intersect-alt.svg
+-rw-r--r--   0        0        0     1344 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/intersect.svg
+-rw-r--r--   0        0        0     1044 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ios-settings.svg
+-rw-r--r--   0        0        0      630 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ip-address-tag.svg
+-rw-r--r--   0        0        0      904 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/iris-scan.svg
+-rw-r--r--   0        0        0      450 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/italic-square.svg
+-rw-r--r--   0        0        0      258 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/italic.svg
+-rw-r--r--   0        0        0     1152 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/jellyfish.svg
+-rw-r--r--   0        0        0     1001 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/journal-page.svg
+-rw-r--r--   0        0        0      809 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/journal.svg
+-rw-r--r--   0        0        0      908 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/jpeg-format.svg
+-rw-r--r--   0        0        0      721 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/jpg-format.svg
+-rw-r--r--   0        0        0      711 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/kanban-board.svg
+-rw-r--r--   0        0        0      421 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/key-back.svg
+-rw-r--r--   0        0        0      792 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/key-command.svg
+-rw-r--r--   0        0        0      677 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/key-minus.svg
+-rw-r--r--   0        0        0      716 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/key-plus.svg
+-rw-r--r--   0        0        0      758 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/key-xmark.svg
+-rw-r--r--   0        0        0      418 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/key.svg
+-rw-r--r--   0        0        0      837 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-align-center.svg
+-rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-align-horizontal.svg
+-rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-align-vertical.svg
+-rw-r--r--   0        0        0      561 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-minus-in.svg
+-rw-r--r--   0        0        0      566 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-minus.svg
+-rw-r--r--   0        0        0      584 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-plus-in.svg
+-rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-plus.svg
+-rw-r--r--   0        0        0      584 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-position.svg
+-rw-r--r--   0        0        0      468 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe.svg
+-rw-r--r--   0        0        0      764 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframes-couple.svg
+-rw-r--r--   0        0        0      812 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframes-minus.svg
+-rw-r--r--   0        0        0      832 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframes-plus.svg
+-rw-r--r--   0        0        0      782 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframes.svg
+-rw-r--r--   0        0        0      414 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/label.svg
+-rw-r--r--   0        0        0      272 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/lamp.svg
+-rw-r--r--   0        0        0      836 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/language.svg
+-rw-r--r--   0        0        0      613 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/laptop-charging.svg
+-rw-r--r--   0        0        0      678 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/laptop-dev-mode.svg
+-rw-r--r--   0        0        0     1135 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/laptop-fix.svg
+-rw-r--r--   0        0        0      696 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/laptop-warning.svg
+-rw-r--r--   0        0        0      502 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/laptop.svg
+-rw-r--r--   0        0        0      444 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/layout-left.svg
+-rw-r--r--   0        0        0      452 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/layout-right.svg
+-rw-r--r--   0        0        0     1173 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/leaderboard-star.svg
+-rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/leaderboard.svg
+-rw-r--r--   0        0        0      550 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/leaf.svg
+-rw-r--r--   0        0        0      978 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/learning.svg
+-rw-r--r--   0        0        0      757 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/lens-plus.svg
+-rw-r--r--   0        0        0      591 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/lens.svg
+-rw-r--r--   0        0        0      931 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/lifebelt.svg
+-rw-r--r--   0        0        0      802 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/light-bulb-off.svg
+-rw-r--r--   0        0        0      993 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/light-bulb-on.svg
+-rw-r--r--   0        0        0      618 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/light-bulb.svg
+-rw-r--r--   0        0        0      523 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/line-space.svg
+-rw-r--r--   0        0        0      214 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/linear.svg
+-rw-r--r--   0        0        0      896 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/link-slash.svg
+-rw-r--r--   0        0        0      961 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/link-xmark.svg
+-rw-r--r--   0        0        0      710 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/link.svg
+-rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/linkedin.svg
+-rw-r--r--   0        0        0     1215 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/linux.svg
+-rw-r--r--   0        0        0      725 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/list-select.svg
+-rw-r--r--   0        0        0      707 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/list.svg
+-rw-r--r--   0        0        0      519 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/litecoin-circle.svg
+-rw-r--r--   0        0        0      919 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/litecoin-rotate-out.svg
+-rw-r--r--   0        0        0      783 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/lock-slash.svg
+-rw-r--r--   0        0        0      638 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/lock-square.svg
+-rw-r--r--   0        0        0      409 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/lock.svg
+-rw-r--r--   0        0        0      502 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/loft-3d.svg
+-rw-r--r--   0        0        0      440 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/log-in.svg
+-rw-r--r--   0        0        0      653 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/log-no-access.svg
+-rw-r--r--   0        0        0      440 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/log-out.svg
+-rw-r--r--   0        0        0      383 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/long-arrow-down-left.svg
+-rw-r--r--   0        0        0      383 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/long-arrow-down-right.svg
+-rw-r--r--   0        0        0      346 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/long-arrow-left-down.svg
+-rw-r--r--   0        0        0      346 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/long-arrow-left-up.svg
+-rw-r--r--   0        0        0      355 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/long-arrow-right-down.svg
+-rw-r--r--   0        0        0      355 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/long-arrow-right-up.svg
+-rw-r--r--   0        0        0      385 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/long-arrow-up-left.svg
+-rw-r--r--   0        0        0      390 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/long-arrow-up-right.svg
+-rw-r--r--   0        0        0      931 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/lot-of-cash.svg
+-rw-r--r--   0        0        0      586 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/lullaby.svg
+-rw-r--r--   0        0        0      395 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mac-control-key.svg
+-rw-r--r--   0        0        0     1223 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mac-dock.svg
+-rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mac-option-key.svg
+-rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mac-os-window.svg
+-rw-r--r--   0        0        0      538 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/magic-wand.svg
+-rw-r--r--   0        0        0      895 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/magnet-energy.svg
+-rw-r--r--   0        0        0      647 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/magnet.svg
+-rw-r--r--   0        0        0      484 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mail-in.svg
+-rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mail-open.svg
+-rw-r--r--   0        0        0      484 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mail-out.svg
+-rw-r--r--   0        0        0      395 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mail.svg
+-rw-r--r--   0        0        0      411 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/male.svg
+-rw-r--r--   0        0        0      581 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/map-pin-minus.svg
+-rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/map-pin-plus.svg
+-rw-r--r--   0        0        0      677 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/map-pin-xmark.svg
+-rw-r--r--   0        0        0      497 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/map-pin.svg
+-rw-r--r--   0        0        0      794 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/map-xmark.svg
+-rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/map.svg
+-rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/maps-arrow-diagonal.svg
+-rw-r--r--   0        0        0      626 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/maps-arrow-xmark.svg
+-rw-r--r--   0        0        0      477 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/maps-arrow.svg
+-rw-r--r--   0        0        0      588 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/maps-go-straight.svg
+-rw-r--r--   0        0        0      793 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/maps-turn-back.svg
+-rw-r--r--   0        0        0      702 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/maps-turn-left.svg
+-rw-r--r--   0        0        0      711 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/maps-turn-right.svg
+-rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mask-square.svg
+-rw-r--r--   0        0        0      793 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mastercard-card.svg
+-rw-r--r--   0        0        0      727 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mastodon.svg
+-rw-r--r--   0        0        0      812 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/math-book.svg
+-rw-r--r--   0        0        0      490 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/maximize.svg
+-rw-r--r--   0        0        0      506 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/medal-1st.svg
+-rw-r--r--   0        0        0      401 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/medal.svg
+-rw-r--r--   0        0        0      870 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-image-folder.svg
+-rw-r--r--   0        0        0      783 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-image-list.svg
+-rw-r--r--   0        0        0      729 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-image-plus.svg
+-rw-r--r--   0        0        0      782 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-image-xmark.svg
+-rw-r--r--   0        0        0      640 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-image.svg
+-rw-r--r--   0        0        0      921 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-video-folder.svg
+-rw-r--r--   0        0        0      733 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-video-list.svg
+-rw-r--r--   0        0        0      693 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-video-plus.svg
+-rw-r--r--   0        0        0      745 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-video-xmark.svg
+-rw-r--r--   0        0        0      608 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-video.svg
+-rw-r--r--   0        0        0      710 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/medium.svg
+-rw-r--r--   0        0        0      537 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/megaphone.svg
+-rw-r--r--   0        0        0      391 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/menu-scale.svg
+-rw-r--r--   0        0        0      391 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/menu.svg
+-rw-r--r--   0        0        0      570 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/message-alert.svg
+-rw-r--r--   0        0        0      560 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/message-text.svg
+-rw-r--r--   0        0        0      376 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/message.svg
+-rw-r--r--   0        0        0      668 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/meter-arrow-down-right.svg
+-rw-r--r--   0        0        0     1285 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/metro.svg
+-rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone-check.svg
+-rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone-minus.svg
+-rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone-mute.svg
+-rw-r--r--   0        0        0      615 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone-plus.svg
+-rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone-speaking.svg
+-rw-r--r--   0        0        0      670 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone-warning.svg
+-rw-r--r--   0        0        0      471 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone.svg
+-rw-r--r--   0        0        0      933 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/microscope.svg
+-rw-r--r--   0        0        0      407 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/minus-circle.svg
+-rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/minus-hexagon.svg
+-rw-r--r--   0        0        0      945 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/minus-square-dashed.svg
+-rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/minus-square.svg
+-rw-r--r--   0        0        0      212 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/minus.svg
+-rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mirror.svg
+-rw-r--r--   0        0        0      699 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mobile-dev-mode.svg
+-rw-r--r--   0        0        0      827 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mobile-fingerprint.svg
+-rw-r--r--   0        0        0      875 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mobile-voice.svg
+-rw-r--r--   0        0        0      698 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/modern-tv-4k.svg
+-rw-r--r--   0        0        0      407 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/modern-tv.svg
+-rw-r--r--   0        0        0      630 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/money-square.svg
+-rw-r--r--   0        0        0      879 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/moon-sat.svg
+-rw-r--r--   0        0        0     1049 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/more-horiz-circle.svg
+-rw-r--r--   0        0        0      854 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/more-horiz.svg
+-rw-r--r--   0        0        0     1049 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/more-vert-circle.svg
+-rw-r--r--   0        0        0      854 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/more-vert.svg
+-rw-r--r--   0        0        0      950 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/motorcycle.svg
+-rw-r--r--   0        0        0      398 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mouse-button-left.svg
+-rw-r--r--   0        0        0      397 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mouse-button-right.svg
+-rw-r--r--   0        0        0     1592 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mouse-scroll-wheel.svg
+-rw-r--r--   0        0        0     1016 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/movie.svg
+-rw-r--r--   0        0        0      930 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/mpeg-format.svg
+-rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/multi-bubble.svg
+-rw-r--r--   0        0        0     1065 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/multi-mac-os-window.svg
+-rw-r--r--   0        0        0      623 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/multi-window.svg
+-rw-r--r--   0        0        0      637 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/multiple-pages-empty.svg
+-rw-r--r--   0        0        0      714 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/multiple-pages-minus.svg
+-rw-r--r--   0        0        0      753 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/multiple-pages-plus.svg
+-rw-r--r--   0        0        0      795 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/multiple-pages-xmark.svg
+-rw-r--r--   0        0        0      919 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/multiple-pages.svg
+-rw-r--r--   0        0        0      803 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/music-double-note-plus.svg
+-rw-r--r--   0        0        0      580 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/music-double-note.svg
+-rw-r--r--   0        0        0      440 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/music-note-plus.svg
+-rw-r--r--   0        0        0      330 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/music-note.svg
+-rw-r--r--   0        0        0      445 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/n-square.svg
+-rw-r--r--   0        0        0      219 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/nav-arrow-down.svg
+-rw-r--r--   0        0        0      220 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/nav-arrow-left.svg
+-rw-r--r--   0        0        0      219 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/nav-arrow-right.svg
+-rw-r--r--   0        0        0      220 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/nav-arrow-up.svg
+-rw-r--r--   0        0        0      511 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/navigator-alt.svg
+-rw-r--r--   0        0        0      507 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/navigator.svg
+-rw-r--r--   0        0        0     1231 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/neighbourhood.svg
+-rw-r--r--   0        0        0      698 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/network-left.svg
+-rw-r--r--   0        0        0      671 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/network-reverse.svg
+-rw-r--r--   0        0        0      676 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/network-right.svg
+-rw-r--r--   0        0        0      606 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/network.svg
+-rw-r--r--   0        0        0      491 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/new-tab.svg
+-rw-r--r--   0        0        0      924 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/nintendo-switch.svg
+-rw-r--r--   0        0        0     1143 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/no-smoking-circle.svg
+-rw-r--r--   0        0        0      505 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/non-binary.svg
+-rw-r--r--   0        0        0      621 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/notes.svg
+-rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/npm-square.svg
+-rw-r--r--   0        0        0      699 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/npm.svg
+-rw-r--r--   0        0        0      476 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-0-square.svg
+-rw-r--r--   0        0        0      391 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-1-square.svg
+-rw-r--r--   0        0        0      544 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-2-square.svg
+-rw-r--r--   0        0        0      656 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-3-square.svg
+-rw-r--r--   0        0        0      397 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-4-square.svg
+-rw-r--r--   0        0        0      481 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-5-square.svg
+-rw-r--r--   0        0        0      606 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-6-square.svg
+-rw-r--r--   0        0        0      411 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-7-square.svg
+-rw-r--r--   0        0        0      685 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-8-square.svg
+-rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-9-square.svg
+-rw-r--r--   0        0        0     1037 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/numbered-list-left.svg
+-rw-r--r--   0        0        0     1027 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/numbered-list-right.svg
+-rw-r--r--   0        0        0      569 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/o-square.svg
+-rw-r--r--   0        0        0      733 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/octagon.svg
+-rw-r--r--   0        0        0      851 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/off-tag.svg
+-rw-r--r--   0        0        0      702 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/oil-industry.svg
+-rw-r--r--   0        0        0      982 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/okrs.svg
+-rw-r--r--   0        0        0      557 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/on-tag.svg
+-rw-r--r--   0        0        0     1372 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/one-finger-select-hand-gesture.svg
+-rw-r--r--   0        0        0      738 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/one-point-circle.svg
+-rw-r--r--   0        0        0      768 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/open-book.svg
+-rw-r--r--   0        0        0      603 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/open-in-browser.svg
+-rw-r--r--   0        0        0      423 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/open-in-window.svg
+-rw-r--r--   0        0        0      386 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/open-new-window.svg
+-rw-r--r--   0        0        0     1326 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/open-select-hand-gesture.svg
+-rw-r--r--   0        0        0     4298 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/open-vpn.svg
+-rw-r--r--   0        0        0      344 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/orange-half.svg
+-rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/orange-slice-alt.svg
+-rw-r--r--   0        0        0      437 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/orange-slice.svg
+-rw-r--r--   0        0        0      770 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/organic-food-square.svg
+-rw-r--r--   0        0        0      745 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/organic-food.svg
+-rw-r--r--   0        0        0      772 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/orthogonal-view.svg
+-rw-r--r--   0        0        0      775 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/package-lock.svg
+-rw-r--r--   0        0        0      437 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/package.svg
+-rw-r--r--   0        0        0     1084 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/packages.svg
+-rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pacman.svg
+-rw-r--r--   0        0        0      422 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-down.svg
+-rw-r--r--   0        0        0     1044 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-edit.svg
+-rw-r--r--   0        0        0      727 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-flip.svg
+-rw-r--r--   0        0        0      421 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-left.svg
+-rw-r--r--   0        0        0      627 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-minus-in.svg
+-rw-r--r--   0        0        0      603 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-minus.svg
+-rw-r--r--   0        0        0      650 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-plus-in.svg
+-rw-r--r--   0        0        0      650 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-plus.svg
+-rw-r--r--   0        0        0      422 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-right.svg
+-rw-r--r--   0        0        0      949 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-search.svg
+-rw-r--r--   0        0        0     1093 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-star.svg
+-rw-r--r--   0        0        0      421 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-up.svg
+-rw-r--r--   0        0        0      813 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/page.svg
+-rw-r--r--   0        0        0     1589 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/palette.svg
+-rw-r--r--   0        0        0      707 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/panorama-enlarge.svg
+-rw-r--r--   0        0        0      540 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/panorama-reduce.svg
+-rw-r--r--   0        0        0      770 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pants-pockets.svg
+-rw-r--r--   0        0        0      454 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pants.svg
+-rw-r--r--   0        0        0      394 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/parking.svg
+-rw-r--r--   0        0        0      721 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/password-check.svg
+-rw-r--r--   0        0        0      925 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/password-cursor.svg
+-rw-r--r--   0        0        0      815 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/password-xmark.svg
+-rw-r--r--   0        0        0      639 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/paste-clipboard.svg
+-rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/path-arrow.svg
+-rw-r--r--   0        0        0      859 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pause-window.svg
+-rw-r--r--   0        0        0      510 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pause.svg
+-rw-r--r--   0        0        0      418 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/paypal.svg
+-rw-r--r--   0        0        0      480 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pc-check.svg
+-rw-r--r--   0        0        0      717 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pc-firewall.svg
+-rw-r--r--   0        0        0      312 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pc-mouse.svg
+-rw-r--r--   0        0        0      715 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pc-no-entry.svg
+-rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pc-warning.svg
+-rw-r--r--   0        0        0     1559 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/peace-hand.svg
+-rw-r--r--   0        0        0      716 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/peerlist.svg
+-rw-r--r--   0        0        0      620 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pen-connect-bluetooth.svg
+-rw-r--r--   0        0        0      838 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pen-connect-wifi.svg
+-rw-r--r--   0        0        0     1001 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pen-tablet-connect-usb.svg
+-rw-r--r--   0        0        0      782 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pen-tablet-connect-wifi.svg
+-rw-r--r--   0        0        0      623 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pen-tablet.svg
+-rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pentagon.svg
+-rw-r--r--   0        0        0      882 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/people-tag.svg
+-rw-r--r--   0        0        0     1254 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/percent-rotate-out.svg
+-rw-r--r--   0        0        0      853 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/percentage-circle.svg
+-rw-r--r--   0        0        0      850 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/percentage-square.svg
+-rw-r--r--   0        0        0      598 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/percentage.svg
+-rw-r--r--   0        0        0      795 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/perspective-view.svg
+-rw-r--r--   0        0        0      822 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pharmacy-cross-circle.svg
+-rw-r--r--   0        0        0      829 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pharmacy-cross-tag.svg
+-rw-r--r--   0        0        0      608 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-disabled.svg
+-rw-r--r--   0        0        0      595 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-income.svg
+-rw-r--r--   0        0        0      599 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-minus.svg
+-rw-r--r--   0        0        0      595 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-outcome.svg
+-rw-r--r--   0        0        0      669 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-paused.svg
+-rw-r--r--   0        0        0      663 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-plus.svg
+-rw-r--r--   0        0        0      689 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-xmark.svg
+-rw-r--r--   0        0        0      485 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone.svg
+-rw-r--r--   0        0        0     1279 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/piggy-bank.svg
+-rw-r--r--   0        0        0      901 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pillow.svg
+-rw-r--r--   0        0        0      538 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pin-slash.svg
+-rw-r--r--   0        0        0      444 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pin.svg
+-rw-r--r--   0        0        0      702 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pine-tree.svg
+-rw-r--r--   0        0        0      602 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pinterest.svg
+-rw-r--r--   0        0        0      913 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pipe-3d.svg
+-rw-r--r--   0        0        0     1011 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pizza-slice.svg
+-rw-r--r--   0        0        0      455 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/planet-alt.svg
+-rw-r--r--   0        0        0      560 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/planet-sat.svg
+-rw-r--r--   0        0        0      455 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/planet.svg
+-rw-r--r--   0        0        0      995 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/planimetry.svg
+-rw-r--r--   0        0        0      383 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/play.svg
+-rw-r--r--   0        0        0      509 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/playlist-play.svg
+-rw-r--r--   0        0        0      517 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/playlist-plus.svg
+-rw-r--r--   0        0        0      632 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/playlist.svg
+-rw-r--r--   0        0        0     1002 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/playstation-gamepad.svg
+-rw-r--r--   0        0        0      498 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/plug-type-a.svg
+-rw-r--r--   0        0        0      713 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/plug-type-c.svg
+-rw-r--r--   0        0        0      588 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/plug-type-g.svg
+-rw-r--r--   0        0        0      705 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/plug-type-l.svg
+-rw-r--r--   0        0        0      433 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/plus-circle.svg
+-rw-r--r--   0        0        0      968 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/plus-square-dashed.svg
+-rw-r--r--   0        0        0      458 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/plus-square.svg
+-rw-r--r--   0        0        0      238 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/plus.svg
+-rw-r--r--   0        0        0      717 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/png-format.svg
+-rw-r--r--   0        0        0      421 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pocket.svg
+-rw-r--r--   0        0        0     1356 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/podcast.svg
+-rw-r--r--   0        0        0      604 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pokeball.svg
+-rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/polar-sh.svg
+-rw-r--r--   0        0        0     1886 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/position-align.svg
+-rw-r--r--   0        0        0      673 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/position.svg
+-rw-r--r--   0        0        0      692 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/post.svg
+-rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/potion.svg
+-rw-r--r--   0        0        0      607 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/pound.svg
+-rw-r--r--   0        0        0      683 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/precision-tool.svg
+-rw-r--r--   0        0        0      809 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/presentation.svg
+-rw-r--r--   0        0        0      524 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/printer.svg
+-rw-r--r--   0        0        0      850 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/printing-page.svg
+-rw-r--r--   0        0        0      586 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/priority-down.svg
+-rw-r--r--   0        0        0      663 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/priority-high.svg
+-rw-r--r--   0        0        0      646 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/priority-medium.svg
+-rw-r--r--   0        0        0      584 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/priority-up.svg
+-rw-r--r--   0        0        0      945 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/privacy-policy.svg
+-rw-r--r--   0        0        0      941 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/private-wifi.svg
+-rw-r--r--   0        0        0      682 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/profile-circle.svg
+-rw-r--r--   0        0        0      437 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/prohibition.svg
+-rw-r--r--   0        0        0      665 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/project-curve-3d.svg
+-rw-r--r--   0        0        0     1216 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/puzzle.svg
+-rw-r--r--   0        0        0     2455 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/qr-code.svg
+-rw-r--r--   0        0        0      421 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/question-mark.svg
+-rw-r--r--   0        0        0      765 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/quote-message.svg
+-rw-r--r--   0        0        0      506 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/quote.svg
+-rw-r--r--   0        0        0     1351 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/radiation.svg
+-rw-r--r--   0        0        0      682 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/radius.svg
+-rw-r--r--   0        0        0      713 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rain.svg
+-rw-r--r--   0        0        0      998 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/raw-format.svg
+-rw-r--r--   0        0        0      595 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/receive-dollars.svg
+-rw-r--r--   0        0        0      644 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/receive-euros.svg
+-rw-r--r--   0        0        0      666 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/receive-pounds.svg
+-rw-r--r--   0        0        0      537 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/receive-yens.svg
+-rw-r--r--   0        0        0      638 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/redo-action.svg
+-rw-r--r--   0        0        0      606 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/redo-circle.svg
+-rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/redo.svg
+-rw-r--r--   0        0        0      336 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/reduce.svg
+-rw-r--r--   0        0        0      826 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/refresh-circle.svg
+-rw-r--r--   0        0        0      717 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/refresh-double.svg
+-rw-r--r--   0        0        0      458 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/refresh.svg
+-rw-r--r--   0        0        0     1334 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/reload-window.svg
+-rw-r--r--   0        0        0     1554 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/reminder-hand-gesture.svg
+-rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/repeat-once.svg
+-rw-r--r--   0        0        0      423 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/repeat.svg
+-rw-r--r--   0        0        0      546 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/reply-to-message.svg
+-rw-r--r--   0        0        0      263 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/reply.svg
+-rw-r--r--   0        0        0      902 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/report-columns.svg
+-rw-r--r--   0        0        0      418 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/reports.svg
+-rw-r--r--   0        0        0      575 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/repository.svg
+-rw-r--r--   0        0        0      647 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/restart.svg
+-rw-r--r--   0        0        0      650 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rewind.svg
+-rw-r--r--   0        0        0      726 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rhombus-arrow-right.svg
+-rw-r--r--   0        0        0      465 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rhombus.svg
+-rw-r--r--   0        0        0      523 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rings.svg
+-rw-r--r--   0        0        0      994 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rocket.svg
+-rw-r--r--   0        0        0      901 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rook.svg
+-rw-r--r--   0        0        0     1301 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rotate-camera-left.svg
+-rw-r--r--   0        0        0     1298 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rotate-camera-right.svg
+-rw-r--r--   0        0        0      922 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/round-flask.svg
+-rw-r--r--   0        0        0      514 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rounded-mirror.svg
+-rw-r--r--   0        0        0      635 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rss-feed-tag.svg
+-rw-r--r--   0        0        0      440 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rss-feed.svg
+-rw-r--r--   0        0        0      700 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/rubik-cube.svg
+-rw-r--r--   0        0        0      748 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ruler-arrows.svg
+-rw-r--r--   0        0        0      770 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ruler-combine.svg
+-rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ruler-minus.svg
+-rw-r--r--   0        0        0      494 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ruler-plus.svg
+-rw-r--r--   0        0        0      385 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/ruler.svg
+-rw-r--r--   0        0        0      733 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/running.svg
+-rw-r--r--   0        0        0     1120 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/safari.svg
+-rw-r--r--   0        0        0     1515 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/safe-arrow-left.svg
+-rw-r--r--   0        0        0     1515 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/safe-arrow-right.svg
+-rw-r--r--   0        0        0     1423 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/safe-open.svg
+-rw-r--r--   0        0        0     1324 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/safe.svg
+-rw-r--r--   0        0        0      787 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sandals.svg
+-rw-r--r--   0        0        0     1108 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/scale-frame-enlarge.svg
+-rw-r--r--   0        0        0      786 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/scale-frame-reduce.svg
+-rw-r--r--   0        0        0     1567 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/scan-barcode.svg
+-rw-r--r--   0        0        0     2139 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/scan-qr-code.svg
+-rw-r--r--   0        0        0      965 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/scanning.svg
+-rw-r--r--   0        0        0      570 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/scarf.svg
+-rw-r--r--   0        0        0      630 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/scissor-alt.svg
+-rw-r--r--   0        0        0      624 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/scissor.svg
+-rw-r--r--   0        0        0     1358 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/screenshot.svg
+-rw-r--r--   0        0        0      686 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sea-and-sun.svg
+-rw-r--r--   0        0        0      542 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sea-waves.svg
+-rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/search-engine.svg
+-rw-r--r--   0        0        0      949 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/search-window.svg
+-rw-r--r--   0        0        0      457 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/search.svg
+-rw-r--r--   0        0        0     1011 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/secure-window.svg
+-rw-r--r--   0        0        0      429 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/security-pass.svg
+-rw-r--r--   0        0        0      912 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/select-edge-3d.svg
+-rw-r--r--   0        0        0     1134 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/select-face-3d.svg
+-rw-r--r--   0        0        0      786 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/select-point-3d.svg
+-rw-r--r--   0        0        0      965 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/select-window.svg
+-rw-r--r--   0        0        0      538 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/selective-tool.svg
+-rw-r--r--   0        0        0      399 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/send-diagonal.svg
+-rw-r--r--   0        0        0      595 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/send-dollars.svg
+-rw-r--r--   0        0        0      644 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/send-euros.svg
+-rw-r--r--   0        0        0      586 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/send-mail.svg
+-rw-r--r--   0        0        0      666 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/send-pounds.svg
+-rw-r--r--   0        0        0      537 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/send-yens.svg
+-rw-r--r--   0        0        0      331 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/send.svg
+-rw-r--r--   0        0        0      456 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/server-connection.svg
+-rw-r--r--   0        0        0      713 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/server.svg
+-rw-r--r--   0        0        0     1562 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/settings-profiles.svg
+-rw-r--r--   0        0        0      786 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/settings.svg
+-rw-r--r--   0        0        0      849 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/share-android.svg
+-rw-r--r--   0        0        0      389 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/share-ios.svg
+-rw-r--r--   0        0        0      667 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-alert.svg
+-rw-r--r--   0        0        0      770 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-alt.svg
+-rw-r--r--   0        0        0      577 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-broken.svg
+-rw-r--r--   0        0        0      579 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-check.svg
+-rw-r--r--   0        0        0      582 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-download.svg
+-rw-r--r--   0        0        0      804 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-eye.svg
+-rw-r--r--   0        0        0      782 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-loading.svg
+-rw-r--r--   0        0        0      562 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-minus.svg
+-rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-plus-in.svg
+-rw-r--r--   0        0        0      718 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-question.svg
+-rw-r--r--   0        0        0      825 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-search.svg
+-rw-r--r--   0        0        0      580 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-upload.svg
+-rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-xmark.svg
+-rw-r--r--   0        0        0      469 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield.svg
+-rw-r--r--   0        0        0      635 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shirt-tank-top.svg
+-rw-r--r--   0        0        0      744 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shirt.svg
+-rw-r--r--   0        0        0     1037 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shop-four-tiles-window.svg
+-rw-r--r--   0        0        0     1196 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shop-four-tiles.svg
+-rw-r--r--   0        0        0     1195 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shop-window.svg
+-rw-r--r--   0        0        0     1354 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shop.svg
+-rw-r--r--   0        0        0      674 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-arrow-down.svg
+-rw-r--r--   0        0        0      674 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-arrow-up.svg
+-rw-r--r--   0        0        0      608 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-check.svg
+-rw-r--r--   0        0        0      666 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-minus.svg
+-rw-r--r--   0        0        0      713 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-plus.svg
+-rw-r--r--   0        0        0      751 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-pocket.svg
+-rw-r--r--   0        0        0      713 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-warning.svg
+-rw-r--r--   0        0        0      565 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag.svg
+-rw-r--r--   0        0        0     1126 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-code-check.svg
+-rw-r--r--   0        0        0     1232 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-code-xmark.svg
+-rw-r--r--   0        0        0     1212 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-code.svg
+-rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/short-pants-pockets.svg
+-rw-r--r--   0        0        0      455 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/short-pants.svg
+-rw-r--r--   0        0        0      584 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shortcut-square.svg
+-rw-r--r--   0        0        0      681 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/shuffle.svg
+-rw-r--r--   0        0        0      534 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sidebar-collapse.svg
+-rw-r--r--   0        0        0      533 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sidebar-expand.svg
+-rw-r--r--   0        0        0      413 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sigma-function.svg
+-rw-r--r--   0        0        0      534 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/simple-cart.svg
+-rw-r--r--   0        0        0      678 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sine-wave.svg
+-rw-r--r--   0        0        0      497 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/single-tap-gesture.svg
+-rw-r--r--   0        0        0      648 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/skateboard.svg
+-rw-r--r--   0        0        0     1061 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/skateboarding.svg
+-rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/skip-next.svg
+-rw-r--r--   0        0        0      477 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/skip-prev.svg
+-rw-r--r--   0        0        0      435 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/slash-square.svg
+-rw-r--r--   0        0        0      214 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/slash.svg
+-rw-r--r--   0        0        0      753 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sleeper-chair.svg
+-rw-r--r--   0        0        0      593 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/slips.svg
+-rw-r--r--   0        0        0      624 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/small-lamp-alt.svg
+-rw-r--r--   0        0        0      770 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/small-lamp.svg
+-rw-r--r--   0        0        0      419 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/smartphone-device.svg
+-rw-r--r--   0        0        0      744 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/smoking.svg
+-rw-r--r--   0        0        0      714 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/snapchat.svg
+-rw-r--r--   0        0        0      501 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/snow-flake.svg
+-rw-r--r--   0        0        0      518 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/snow.svg
+-rw-r--r--   0        0        0      457 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/soap.svg
+-rw-r--r--   0        0        0      748 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/soccer-ball.svg
+-rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sofa.svg
+-rw-r--r--   0        0        0     1457 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/soil-alt.svg
+-rw-r--r--   0        0        0     1667 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/soil.svg
+-rw-r--r--   0        0        0      600 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sort-down.svg
+-rw-r--r--   0        0        0      593 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sort-up.svg
+-rw-r--r--   0        0        0      613 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sort.svg
+-rw-r--r--   0        0        0      744 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sound-high.svg
+-rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sound-low.svg
+-rw-r--r--   0        0        0      557 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sound-min.svg
+-rw-r--r--   0        0        0      616 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sound-off.svg
+-rw-r--r--   0        0        0      521 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/spades.svg
+-rw-r--r--   0        0        0      297 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/spark.svg
+-rw-r--r--   0        0        0      483 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sparks.svg
+-rw-r--r--   0        0        0      456 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sphere.svg
+-rw-r--r--   0        0        0     1281 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/spiral.svg
+-rw-r--r--   0        0        0      584 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/split-area.svg
+-rw-r--r--   0        0        0      761 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/split-square-dashed.svg
+-rw-r--r--   0        0        0     1206 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/spock-hand-gesture.svg
+-rw-r--r--   0        0        0      658 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/spotify.svg
+-rw-r--r--   0        0        0      719 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/square-3d-corner-to-corner.svg
+-rw-r--r--   0        0        0      516 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/square-3d-from-center.svg
+-rw-r--r--   0        0        0     1308 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/square-3d-three-points.svg
+-rw-r--r--   0        0        0      518 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/square-cursor.svg
+-rw-r--r--   0        0        0      852 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/square-dashed.svg
+-rw-r--r--   0        0        0      429 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/square-wave.svg
+-rw-r--r--   0        0        0      342 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/square.svg
+-rw-r--r--   0        0        0      753 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/stackoverflow.svg
+-rw-r--r--   0        0        0     1622 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/star-dashed.svg
+-rw-r--r--   0        0        0     1304 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/star-half-dashed.svg
+-rw-r--r--   0        0        0      614 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/star.svg
+-rw-r--r--   0        0        0      339 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/stat-down.svg
+-rw-r--r--   0        0        0      339 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/stat-up.svg
+-rw-r--r--   0        0        0      593 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/stats-down-square.svg
+-rw-r--r--   0        0        0      804 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/stats-report.svg
+-rw-r--r--   0        0        0      593 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/stats-up-square.svg
+-rw-r--r--   0        0        0      731 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/strategy.svg
+-rw-r--r--   0        0        0      584 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/stretching.svg
+-rw-r--r--   0        0        0      475 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/strikethrough.svg
+-rw-r--r--   0        0        0      997 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/stroller.svg
+-rw-r--r--   0        0        0      641 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/style-border.svg
+-rw-r--r--   0        0        0      615 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/submit-document.svg
+-rw-r--r--   0        0        0     1040 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/substract.svg
+-rw-r--r--   0        0        0      650 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/suggestion.svg
+-rw-r--r--   0        0        0      373 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/suitcase.svg
+-rw-r--r--   0        0        0     1051 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sun-light.svg
+-rw-r--r--   0        0        0      818 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/svg-format.svg
+-rw-r--r--   0        0        0      717 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/sweep-3d.svg
+-rw-r--r--   0        0        0      969 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/swimming.svg
+-rw-r--r--   0        0        0      347 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/swipe-down-gesture.svg
+-rw-r--r--   0        0        0      347 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/swipe-left-gesture.svg
+-rw-r--r--   0        0        0      347 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/swipe-right-gesture.svg
+-rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/swipe-two-fingers-down-gesture.svg
+-rw-r--r--   0        0        0      589 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/swipe-two-fingers-left-gesture.svg
+-rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/swipe-two-fingers-right-gesture.svg
+-rw-r--r--   0        0        0      589 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/swipe-two-fingers-up-gesture.svg
+-rw-r--r--   0        0        0      347 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/swipe-up-gesture.svg
+-rw-r--r--   0        0        0      505 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/switch-off.svg
+-rw-r--r--   0        0        0      514 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/switch-on.svg
+-rw-r--r--   0        0        0      936 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/system-restart.svg
+-rw-r--r--   0        0        0      407 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/system-shut.svg
+-rw-r--r--   0        0        0      565 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/table-2-columns.svg
+-rw-r--r--   0        0        0      456 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/table-rows.svg
+-rw-r--r--   0        0        0      766 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/table.svg
+-rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/task-list.svg
+-rw-r--r--   0        0        0      450 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/telegram-circle.svg
+-rw-r--r--   0        0        0      281 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/telegram.svg
+-rw-r--r--   0        0        0     1055 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/temperature-down.svg
+-rw-r--r--   0        0        0     1125 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/temperature-high.svg
+-rw-r--r--   0        0        0     1126 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/temperature-low.svg
+-rw-r--r--   0        0        0     1048 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/temperature-up.svg
+-rw-r--r--   0        0        0      693 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tennis-ball-alt.svg
+-rw-r--r--   0        0        0      608 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tennis-ball.svg
+-rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/terminal-tag.svg
+-rw-r--r--   0        0        0      310 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/terminal.svg
+-rw-r--r--   0        0        0      521 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/test-tube.svg
+-rw-r--r--   0        0        0      468 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/text-arrows-up-down.svg
+-rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/text-box.svg
+-rw-r--r--   0        0        0      669 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/text-magnifying-glass.svg
+-rw-r--r--   0        0        0      542 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/text-size.svg
+-rw-r--r--   0        0        0      545 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/text-square.svg
+-rw-r--r--   0        0        0      328 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/text.svg
+-rw-r--r--   0        0        0      485 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/threads.svg
+-rw-r--r--   0        0        0     1321 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/three-points-circle.svg
+-rw-r--r--   0        0        0     1587 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/three-stars.svg
+-rw-r--r--   0        0        0      693 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/thumbs-down.svg
+-rw-r--r--   0        0        0      667 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/thumbs-up.svg
+-rw-r--r--   0        0        0      456 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/thunderstorm.svg
+-rw-r--r--   0        0        0      772 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tif-format.svg
+-rw-r--r--   0        0        0      960 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tiff-format.svg
+-rw-r--r--   0        0        0      517 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tiktok.svg
+-rw-r--r--   0        0        0     1075 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/time-zone.svg
+-rw-r--r--   0        0        0      702 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/timer-off.svg
+-rw-r--r--   0        0        0      502 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/timer.svg
+-rw-r--r--   0        0        0     1145 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tools.svg
+-rw-r--r--   0        0        0      538 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tournament.svg
+-rw-r--r--   0        0        0      866 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tower-check.svg
+-rw-r--r--   0        0        0     1048 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tower-no-access.svg
+-rw-r--r--   0        0        0      965 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tower-warning.svg
+-rw-r--r--   0        0        0      766 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tower.svg
+-rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/trademark.svg
+-rw-r--r--   0        0        0     1061 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/train.svg
+-rw-r--r--   0        0        0     1092 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tram.svg
+-rw-r--r--   0        0        0      562 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/transition-down.svg
+-rw-r--r--   0        0        0      554 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/transition-left.svg
+-rw-r--r--   0        0        0      558 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/transition-right.svg
+-rw-r--r--   0        0        0      558 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/transition-up.svg
+-rw-r--r--   0        0        0      553 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/translate.svg
+-rw-r--r--   0        0        0      527 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/trash.svg
+-rw-r--r--   0        0        0     1070 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/treadmill.svg
+-rw-r--r--   0        0        0      686 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tree.svg
+-rw-r--r--   0        0        0      760 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/trekking.svg
+-rw-r--r--   0        0        0      775 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/trello.svg
+-rw-r--r--   0        0        0      456 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/triangle-flag-circle.svg
+-rw-r--r--   0        0        0      442 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/triangle-flag-two-stripes.svg
+-rw-r--r--   0        0        0      337 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/triangle-flag.svg
+-rw-r--r--   0        0        0      396 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/triangle.svg
+-rw-r--r--   0        0        0     1079 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/trophy.svg
+-rw-r--r--   0        0        0     1199 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/truck-green.svg
+-rw-r--r--   0        0        0     1248 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/truck-length.svg
+-rw-r--r--   0        0        0     1085 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/truck.svg
+-rw-r--r--   0        0        0      655 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tunnel.svg
+-rw-r--r--   0        0        0      896 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tv-fix.svg
+-rw-r--r--   0        0        0      596 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tv-warning.svg
+-rw-r--r--   0        0        0      400 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/tv.svg
+-rw-r--r--   0        0        0      727 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/twitter.svg
+-rw-r--r--   0        0        0     1235 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/two-points-circle.svg
+-rw-r--r--   0        0        0      810 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/two-seater-sofa.svg
+-rw-r--r--   0        0        0      660 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/type.svg
+-rw-r--r--   0        0        0      436 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/u-turn-arrow-left.svg
+-rw-r--r--   0        0        0      441 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/u-turn-arrow-right.svg
+-rw-r--r--   0        0        0      939 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/umbrella.svg
+-rw-r--r--   0        0        0      556 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/underline-square.svg
+-rw-r--r--   0        0        0      364 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/underline.svg
+-rw-r--r--   0        0        0      636 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/undo-action.svg
+-rw-r--r--   0        0        0      614 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/undo-circle.svg
+-rw-r--r--   0        0        0      480 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/undo.svg
+-rw-r--r--   0        0        0      495 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/union-alt.svg
+-rw-r--r--   0        0        0      499 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/union-horiz-alt.svg
+-rw-r--r--   0        0        0      496 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/union.svg
+-rw-r--r--   0        0        0      811 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/unity-5.svg
+-rw-r--r--   0        0        0      334 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/unity.svg
+-rw-r--r--   0        0        0      540 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/unjoin-3d.svg
+-rw-r--r--   0        0        0      796 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/upload-data-window.svg
+-rw-r--r--   0        0        0      524 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/upload-square.svg
+-rw-r--r--   0        0        0      332 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/upload.svg
+-rw-r--r--   0        0        0     1027 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/usb.svg
+-rw-r--r--   0        0        0     1510 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-badge-check.svg
+-rw-r--r--   0        0        0      858 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-bag.svg
+-rw-r--r--   0        0        0      819 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-cart.svg
+-rw-r--r--   0        0        0      516 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-circle.svg
+-rw-r--r--   0        0        0      605 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-crown.svg
+-rw-r--r--   0        0        0      938 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-love.svg
+-rw-r--r--   0        0        0      576 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-plus.svg
+-rw-r--r--   0        0        0      834 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-scan.svg
+-rw-r--r--   0        0        0      662 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-square.svg
+-rw-r--r--   0        0        0      961 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-star.svg
+-rw-r--r--   0        0        0      647 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-xmark.svg
+-rw-r--r--   0        0        0      463 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/user.svg
+-rw-r--r--   0        0        0      774 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/vegan-circle.svg
+-rw-r--r--   0        0        0      800 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/vegan-square.svg
+-rw-r--r--   0        0        0      603 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/vegan.svg
+-rw-r--r--   0        0        0     1262 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/vehicle-green.svg
+-rw-r--r--   0        0        0      549 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/vertical-merge.svg
+-rw-r--r--   0        0        0      547 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/vertical-split.svg
+-rw-r--r--   0        0        0      692 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/vials.svg
+-rw-r--r--   0        0        0      552 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/video-camera-off.svg
+-rw-r--r--   0        0        0      461 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/video-camera.svg
+-rw-r--r--   0        0        0     1298 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/video-projector.svg
+-rw-r--r--   0        0        0     1003 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/view-360.svg
+-rw-r--r--   0        0        0      331 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/view-columns-2.svg
+-rw-r--r--   0        0        0      351 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/view-columns-3.svg
+-rw-r--r--   0        0        0      902 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/view-grid.svg
+-rw-r--r--   0        0        0      701 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/view-structure-down.svg
+-rw-r--r--   0        0        0      709 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/view-structure-up.svg
+-rw-r--r--   0        0        0      695 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice-check.svg
+-rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice-circle.svg
+-rw-r--r--   0        0        0     1198 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice-lock-circle.svg
+-rw-r--r--   0        0        0      953 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice-scan.svg
+-rw-r--r--   0        0        0      805 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice-square.svg
+-rw-r--r--   0        0        0      789 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice-xmark.svg
+-rw-r--r--   0        0        0      585 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice.svg
+-rw-r--r--   0        0        0      646 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/vr-tag.svg
+-rw-r--r--   0        0        0      360 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/vue-js.svg
+-rw-r--r--   0        0        0      902 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/waist.svg
+-rw-r--r--   0        0        0      767 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/walking.svg
+-rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wallet.svg
+-rw-r--r--   0        0        0      515 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/warning-circle.svg
+-rw-r--r--   0        0        0      765 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/warning-hexagon.svg
+-rw-r--r--   0        0        0      509 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/warning-square.svg
+-rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/warning-triangle.svg
+-rw-r--r--   0        0        0      870 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/warning-window.svg
+-rw-r--r--   0        0        0      493 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wash.svg
+-rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/washing-machine.svg
+-rw-r--r--   0        0        0     1229 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/watering-soil.svg
+-rw-r--r--   0        0        0      545 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/web-window-energy-consumption.svg
+-rw-r--r--   0        0        0      563 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/web-window-xmark.svg
+-rw-r--r--   0        0        0      433 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/web-window.svg
+-rw-r--r--   0        0        0     1171 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/webp-format.svg
+-rw-r--r--   0        0        0      956 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/weight-alt.svg
+-rw-r--r--   0        0        0      863 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/weight.svg
+-rw-r--r--   0        0        0      379 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/white-flag.svg
+-rw-r--r--   0        0        0      810 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wifi-off.svg
+-rw-r--r--   0        0        0      493 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wifi-signal-none.svg
+-rw-r--r--   0        0        0      645 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wifi-tag.svg
+-rw-r--r--   0        0        0      688 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wifi-warning.svg
+-rw-r--r--   0        0        0      777 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wifi-xmark.svg
+-rw-r--r--   0        0        0      566 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wifi.svg
+-rw-r--r--   0        0        0      588 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wind.svg
+-rw-r--r--   0        0        0      771 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/window-check.svg
+-rw-r--r--   0        0        0     1041 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/window-lock.svg
+-rw-r--r--   0        0        0     1015 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/window-no-access.svg
+-rw-r--r--   0        0        0      457 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/window-tabs.svg
+-rw-r--r--   0        0        0      861 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/window-xmark.svg
+-rw-r--r--   0        0        0      469 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/windows.svg
+-rw-r--r--   0        0        0     1116 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wolf.svg
+-rw-r--r--   0        0        0      574 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wrap-text.svg
+-rw-r--r--   0        0        0      704 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wrench.svg
+-rw-r--r--   0        0        0      728 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/wristwatch.svg
+-rw-r--r--   0        0        0     1345 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/www.svg
+-rw-r--r--   0        0        0      528 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/x-square.svg
+-rw-r--r--   0        0        0      467 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/x.svg
+-rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/xbox-a.svg
+-rw-r--r--   0        0        0      626 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/xbox-b.svg
+-rw-r--r--   0        0        0      504 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/xbox-x.svg
+-rw-r--r--   0        0        0      508 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/xbox-y.svg
+-rw-r--r--   0        0        0      505 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/xmark-circle.svg
+-rw-r--r--   0        0        0      512 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/xmark-square.svg
+-rw-r--r--   0        0        0      312 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/xmark.svg
+-rw-r--r--   0        0        0     1004 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/xray-view.svg
+-rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/y-square.svg
+-rw-r--r--   0        0        0     1218 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/yelp.svg
+-rw-r--r--   0        0        0      612 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/yen-square.svg
+-rw-r--r--   0        0        0      414 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/yen.svg
+-rw-r--r--   0        0        0     1013 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/yoga.svg
+-rw-r--r--   0        0        0      825 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/youtube.svg
+-rw-r--r--   0        0        0      441 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/z-square.svg
+-rw-r--r--   0        0        0      573 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/zoom-in.svg
+-rw-r--r--   0        0        0      550 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/regular/zoom-out.svg
+-rw-r--r--   0        0        0        0 2024-04-25 23:08:11.213264 flet_iconoir-0.3.0/flet_iconoir/icons/solid/__init__.py
+-rw-r--r--   0        0        0     1152 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/adobe-after-effects.svg
+-rw-r--r--   0        0        0     1122 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/adobe-illustrator.svg
+-rw-r--r--   0        0        0      824 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/adobe-indesign.svg
+-rw-r--r--   0        0        0     1032 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/adobe-lightroom.svg
+-rw-r--r--   0        0        0     1456 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/adobe-photoshop.svg
+-rw-r--r--   0        0        0     1169 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/adobe-xd.svg
+-rw-r--r--   0        0        0      495 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/airplay.svg
+-rw-r--r--   0        0        0     1143 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/alarm.svg
+-rw-r--r--   0        0        0     1117 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-bottom-box.svg
+-rw-r--r--   0        0        0      414 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-horizontal-centers.svg
+-rw-r--r--   0        0        0      519 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-horizontal-spacing.svg
+-rw-r--r--   0        0        0     1221 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-left-box.svg
+-rw-r--r--   0        0        0     1204 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-right-box.svg
+-rw-r--r--   0        0        0     1116 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-top-box.svg
+-rw-r--r--   0        0        0      411 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-vertical-centers.svg
+-rw-r--r--   0        0        0      521 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-vertical-spacing.svg
+-rw-r--r--   0        0        0      649 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/app-notification.svg
+-rw-r--r--   0        0        0     1143 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/app-store.svg
+-rw-r--r--   0        0        0     1196 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/apple-shortcuts.svg
+-rw-r--r--   0        0        0      726 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-down-circle.svg
+-rw-r--r--   0        0        0      743 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-down-left-circle.svg
+-rw-r--r--   0        0        0      879 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-down-right-circle.svg
+-rw-r--r--   0        0        0      904 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-down-right-square.svg
+-rw-r--r--   0        0        0      731 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-left-circle.svg
+-rw-r--r--   0        0        0      726 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-right-circle.svg
+-rw-r--r--   0        0        0      731 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-up-circle.svg
+-rw-r--r--   0        0        0      836 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-up-left-circle.svg
+-rw-r--r--   0        0        0      861 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-up-left-square.svg
+-rw-r--r--   0        0        0      836 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-up-right-circle.svg
+-rw-r--r--   0        0        0      861 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-up-right-square.svg
+-rw-r--r--   0        0        0      970 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/bathroom.svg
+-rw-r--r--   0        0        0     1915 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/bitcoin-circle.svg
+-rw-r--r--   0        0        0     1164 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/bluetooth-tag.svg
+-rw-r--r--   0        0        0     2246 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/bold-square.svg
+-rw-r--r--   0        0        0      733 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/book.svg
+-rw-r--r--   0        0        0      669 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/bookmark-circle.svg
+-rw-r--r--   0        0        0      357 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/bookmark.svg
+-rw-r--r--   0        0        0     1632 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/bubble-search.svg
+-rw-r--r--   0        0        0     1404 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/bubble-xmark.svg
+-rw-r--r--   0        0        0      796 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/cable-tag.svg
+-rw-r--r--   0        0        0      690 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/camera.svg
+-rw-r--r--   0        0        0      975 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/cash.svg
+-rw-r--r--   0        0        0     2203 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/center-align.svg
+-rw-r--r--   0        0        0      816 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble-check.svg
+-rw-r--r--   0        0        0      500 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble-empty.svg
+-rw-r--r--   0        0        0     1695 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble-question.svg
+-rw-r--r--   0        0        0     1480 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble-translate.svg
+-rw-r--r--   0        0        0      890 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble-warning.svg
+-rw-r--r--   0        0        0     1019 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble-xmark.svg
+-rw-r--r--   0        0        0      965 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble.svg
+-rw-r--r--   0        0        0      825 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-lines.svg
+-rw-r--r--   0        0        0      664 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-minus-in.svg
+-rw-r--r--   0        0        0      831 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-plus-in.svg
+-rw-r--r--   0        0        0      648 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/check-circle.svg
+-rw-r--r--   0        0        0      668 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/check-square.svg
+-rw-r--r--   0        0        0      543 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/clock.svg
+-rw-r--r--   0        0        0     1631 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/closed-captions-tag.svg
+-rw-r--r--   0        0        0      895 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/cloud-square.svg
+-rw-r--r--   0        0        0      411 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/comp-align-bottom.svg
+-rw-r--r--   0        0        0      410 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/comp-align-left.svg
+-rw-r--r--   0        0        0      411 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/comp-align-right.svg
+-rw-r--r--   0        0        0      409 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/comp-align-top.svg
+-rw-r--r--   0        0        0     1477 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/component.svg
+-rw-r--r--   0        0        0      432 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/credit-card.svg
+-rw-r--r--   0        0        0     3486 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/database-check.svg
+-rw-r--r--   0        0        0     1807 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/database-tag.svg
+-rw-r--r--   0        0        0     3173 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/database-xmark.svg
+-rw-r--r--   0        0        0     3279 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/database.svg
+-rw-r--r--   0        0        0     1477 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/design-nib.svg
+-rw-r--r--   0        0        0     1252 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/dogecoin-circle.svg
+-rw-r--r--   0        0        0     1843 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/dollar-circle.svg
+-rw-r--r--   0        0        0      890 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/download-circle.svg
+-rw-r--r--   0        0        0      921 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/download-square.svg
+-rw-r--r--   0        0        0      280 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/droplet.svg
+-rw-r--r--   0        0        0      743 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/erase.svg
+-rw-r--r--   0        0        0      897 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/ethereum-circle.svg
+-rw-r--r--   0        0        0     1413 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/euro-square.svg
+-rw-r--r--   0        0        0      465 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/eye.svg
+-rw-r--r--   0        0        0      637 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/facetime.svg
+-rw-r--r--   0        0        0      903 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/fill-color.svg
+-rw-r--r--   0        0        0      696 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/filter.svg
+-rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/flash.svg
+-rw-r--r--   0        0        0      708 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/forward.svg
+-rw-r--r--   0        0        0      523 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/frame-tool.svg
+-rw-r--r--   0        0        0     1161 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/fx-tag.svg
+-rw-r--r--   0        0        0     1373 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/hd-display.svg
+-rw-r--r--   0        0        0     1095 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/headset-bolt.svg
+-rw-r--r--   0        0        0     1206 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/headset-warning.svg
+-rw-r--r--   0        0        0      969 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/headset.svg
+-rw-r--r--   0        0        0      635 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/heart.svg
+-rw-r--r--   0        0        0     1575 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/help-circle.svg
+-rw-r--r--   0        0        0     1585 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/help-square.svg
+-rw-r--r--   0        0        0      712 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/horiz-distribution-left.svg
+-rw-r--r--   0        0        0      722 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/horiz-distribution-right.svg
+-rw-r--r--   0        0        0     7050 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/hospital-circle.svg
+-rw-r--r--   0        0        0      843 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/ice-cream.svg
+-rw-r--r--   0        0        0      739 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/info-circle.svg
+-rw-r--r--   0        0        0      720 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/italic-square.svg
+-rw-r--r--   0        0        0     1346 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-align-center.svg
+-rw-r--r--   0        0        0      884 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-align-horizontal.svg
+-rw-r--r--   0        0        0      884 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-align-vertical.svg
+-rw-r--r--   0        0        0      658 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-minus-in.svg
+-rw-r--r--   0        0        0      656 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-minus.svg
+-rw-r--r--   0        0        0      819 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-plus-in.svg
+-rw-r--r--   0        0        0      822 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-plus.svg
+-rw-r--r--   0        0        0      742 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-position.svg
+-rw-r--r--   0        0        0      425 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe.svg
+-rw-r--r--   0        0        0      975 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframes-couple.svg
+-rw-r--r--   0        0        0      778 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframes.svg
+-rw-r--r--   0        0        0      415 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/label.svg
+-rw-r--r--   0        0        0      804 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/litecoin-circle.svg
+-rw-r--r--   0        0        0      769 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/mail-open.svg
+-rw-r--r--   0        0        0      644 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/mail.svg
+-rw-r--r--   0        0        0     1413 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/medal-1st.svg
+-rw-r--r--   0        0        0     1098 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/medal.svg
+-rw-r--r--   0        0        0      793 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/message-alert.svg
+-rw-r--r--   0        0        0      715 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/message-text.svg
+-rw-r--r--   0        0        0      408 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/message.svg
+-rw-r--r--   0        0        0      637 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone-check.svg
+-rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone-minus.svg
+-rw-r--r--   0        0        0     1544 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone-mute.svg
+-rw-r--r--   0        0        0      673 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone-plus.svg
+-rw-r--r--   0        0        0      637 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone-speaking.svg
+-rw-r--r--   0        0        0      747 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone-warning.svg
+-rw-r--r--   0        0        0      510 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone.svg
+-rw-r--r--   0        0        0      485 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/minus-circle.svg
+-rw-r--r--   0        0        0      516 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/minus-square.svg
+-rw-r--r--   0        0        0     1872 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/money-square.svg
+-rw-r--r--   0        0        0     1502 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/multi-bubble.svg
+-rw-r--r--   0        0        0      604 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/music-note-plus.svg
+-rw-r--r--   0        0        0      480 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/music-note.svg
+-rw-r--r--   0        0        0      739 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/network-left.svg
+-rw-r--r--   0        0        0      712 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/network-reverse.svg
+-rw-r--r--   0        0        0      717 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/network-right.svg
+-rw-r--r--   0        0        0      647 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/network.svg
+-rw-r--r--   0        0        0      700 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-0-square.svg
+-rw-r--r--   0        0        0      657 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-1-square.svg
+-rw-r--r--   0        0        0     1236 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-2-square.svg
+-rw-r--r--   0        0        0     1217 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-3-square.svg
+-rw-r--r--   0        0        0      775 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-4-square.svg
+-rw-r--r--   0        0        0     1002 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-5-square.svg
+-rw-r--r--   0        0        0     1454 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-6-square.svg
+-rw-r--r--   0        0        0      951 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-7-square.svg
+-rw-r--r--   0        0        0     1539 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-8-square.svg
+-rw-r--r--   0        0        0     1446 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-9-square.svg
+-rw-r--r--   0        0        0      531 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/pause.svg
+-rw-r--r--   0        0        0      886 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/percentage-circle.svg
+-rw-r--r--   0        0        0      911 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/percentage-square.svg
+-rw-r--r--   0        0        0      762 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/pin-slash.svg
+-rw-r--r--   0        0        0      483 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/pin.svg
+-rw-r--r--   0        0        0      403 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/play.svg
+-rw-r--r--   0        0        0      658 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/plus-circle.svg
+-rw-r--r--   0        0        0      683 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/plus-square.svg
+-rw-r--r--   0        0        0     1346 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/podcast.svg
+-rw-r--r--   0        0        0     1156 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/post.svg
+-rw-r--r--   0        0        0     1442 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/presentation.svg
+-rw-r--r--   0        0        0     1045 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/priority-down.svg
+-rw-r--r--   0        0        0     1003 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/priority-high.svg
+-rw-r--r--   0        0        0      926 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/priority-medium.svg
+-rw-r--r--   0        0        0     1051 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/priority-up.svg
+-rw-r--r--   0        0        0     1261 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/quote-message.svg
+-rw-r--r--   0        0        0     1082 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/quote.svg
+-rw-r--r--   0        0        0    10294 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/redo-circle.svg
+-rw-r--r--   0        0        0     1416 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/refresh-circle.svg
+-rw-r--r--   0        0        0      313 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/reports.svg
+-rw-r--r--   0        0        0      709 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/rewind.svg
+-rw-r--r--   0        0        0     1177 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/rhombus-arrow-right.svg
+-rw-r--r--   0        0        0      809 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/send-diagonal.svg
+-rw-r--r--   0        0        0      610 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/send.svg
+-rw-r--r--   0        0        0      986 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/server-connection.svg
+-rw-r--r--   0        0        0     1084 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/server.svg
+-rw-r--r--   0        0        0      947 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/share-android.svg
+-rw-r--r--   0        0        0      514 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/skip-next.svg
+-rw-r--r--   0        0        0      516 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/skip-prev.svg
+-rw-r--r--   0        0        0     3738 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/sound-high.svg
+-rw-r--r--   0        0        0     2014 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/sound-low.svg
+-rw-r--r--   0        0        0      780 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/sound-min.svg
+-rw-r--r--   0        0        0     1262 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/sound-off.svg
+-rw-r--r--   0        0        0      317 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/spark.svg
+-rw-r--r--   0        0        0      542 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/sparks.svg
+-rw-r--r--   0        0        0      557 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/square-cursor.svg
+-rw-r--r--   0        0        0      634 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/star.svg
+-rw-r--r--   0        0        0      829 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/stats-down-square.svg
+-rw-r--r--   0        0        0      829 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/stats-up-square.svg
+-rw-r--r--   0        0        0      642 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/style-border.svg
+-rw-r--r--   0        0        0      810 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/text-square.svg
+-rw-r--r--   0        0        0     1685 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/three-stars.svg
+-rw-r--r--   0        0        0      732 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/timer.svg
+-rw-r--r--   0        0        0     1204 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/transition-down.svg
+-rw-r--r--   0        0        0     1202 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/transition-left.svg
+-rw-r--r--   0        0        0     1212 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/transition-right.svg
+-rw-r--r--   0        0        0     1202 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/transition-up.svg
+-rw-r--r--   0        0        0      689 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/trash.svg
+-rw-r--r--   0        0        0      821 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/underline-square.svg
+-rw-r--r--   0        0        0     1951 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/undo-circle.svg
+-rw-r--r--   0        0        0      926 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/upload-square.svg
+-rw-r--r--   0        0        0     1201 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/usb.svg
+-rw-r--r--   0        0        0      627 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/wallet.svg
+-rw-r--r--   0        0        0      726 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/warning-circle.svg
+-rw-r--r--   0        0        0      751 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/warning-square.svg
+-rw-r--r--   0        0        0      772 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/warning-triangle.svg
+-rw-r--r--   0        0        0     1012 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/web-window-energy-consumption.svg
+-rw-r--r--   0        0        0     1055 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/web-window-xmark.svg
+-rw-r--r--   0        0        0      546 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/web-window.svg
+-rw-r--r--   0        0        0      586 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/white-flag.svg
+-rw-r--r--   0        0        0      548 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/wifi-signal-none.svg
+-rw-r--r--   0        0        0     1129 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/wifi-tag.svg
+-rw-r--r--   0        0        0      947 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/wifi-warning.svg
+-rw-r--r--   0        0        0      683 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/window-tabs.svg
+-rw-r--r--   0        0        0      842 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/xmark-circle.svg
+-rw-r--r--   0        0        0      852 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/xmark-square.svg
+-rw-r--r--   0        0        0     1048 2024-04-25 12:40:38.000000 flet_iconoir-0.3.0/flet_iconoir/icons/solid/yen-square.svg
+-rw-r--r--   0        0        0      363 2024-04-28 00:20:44.943595 flet_iconoir-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1220 2024-04-28 00:24:46.873905 flet_iconoir-0.3.0/README.md
+-rw-r--r--   0        0        0     1661 1970-01-01 00:00:00.000000 flet_iconoir-0.3.0/PKG-INFO
```

### Comparing `flet_iconoir-0.2.2/flet_iconoir/iconoir_icon_button.py` & `flet_iconoir-0.3.0/flet_iconoir/iconoir_icon_button.py`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/LICENSE` & `flet_iconoir-0.3.0/flet_iconoir/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/accessibility-sign.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/accessibility-sign.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/accessibility-tech.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/accessibility-tech.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/accessibility.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/accessibility.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/adobe-after-effects.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/adobe-after-effects.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/adobe-illustrator.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/adobe-illustrator.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/adobe-indesign.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/adobe-indesign.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/adobe-lightroom.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/adobe-lightroom.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/adobe-photoshop.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/adobe-photoshop.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/adobe-xd.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/adobe-xd.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/african-tree.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/african-tree.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/agile.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/agile.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/air-conditioner.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/air-conditioner.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/airplane-helix-45deg.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/airplane-helix-45deg.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/airplane-helix.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/airplane-helix.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/airplane-off.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/airplane-off.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/airplane-rotation.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/airplane-rotation.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/airplane.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/airplane.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/alarm.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/alarm.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/album-carousel.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/album-carousel.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/album-list.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/album-list.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/album-open.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/album-open.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/album.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/album.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-bottom-box.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-bottom-box.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-left-box.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-left-box.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-right-box.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-right-box.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/align-top-box.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/align-top-box.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/angle-tool.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/angle-tool.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/antenna-off.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/antenna-off.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/antenna-signal-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/antenna-signal-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/antenna-signal.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/antenna-signal.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/antenna.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/antenna.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/app-store.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/app-store.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/app-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/app-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple-half.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple-half.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple-mac.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple-mac.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple-shortcuts.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple-shortcuts.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple-swift.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple-swift.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple-wallet.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple-wallet.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/apple.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/apple.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ar-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ar-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/arc-3d-center-point.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/arc-3d-center-point.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/arc-3d.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/arc-3d.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/arcade.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/arcade.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/archery-match.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/archery-match.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/archive.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/archive.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/area-search.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/area-search.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/arrow-reduce-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/arrow-reduce-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/asana.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/asana.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/at-sign-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/at-sign-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/at-sign.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/at-sign.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/atom.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/atom.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/attachment.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/attachment.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/augmented-reality.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/augmented-reality.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/avi-format.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/avi-format.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/axes.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/axes.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/backward-15-seconds.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/backward-15-seconds.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/badge-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/badge-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/balcony.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/balcony.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bank.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bank.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/barcode.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/barcode.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/basketball-field.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/basketball-field.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/basketball.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/basketball.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bathroom.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bathroom.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-25.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-25.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-50.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-50.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-75.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-75.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-full.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-full.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-indicator.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-indicator.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/battery-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/battery-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bbq.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bbq.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/beach-bag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/beach-bag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bed-ready.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bed-ready.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bed.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bed.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/behance-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/behance-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/behance.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/behance.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bell-notification.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bell-notification.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bell-off.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bell-off.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bell.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bell.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bicycle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bicycle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bin-full.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bin-full.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bin-half.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bin-half.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bin-minus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bin-minus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bin-plus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bin-plus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bin.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bin.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/binocular.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/binocular.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/birthday-cake.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/birthday-cake.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bishop.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bishop.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bitbucket.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bitbucket.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bitcoin-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bitcoin-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bitcoin-rotate-out.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bitcoin-rotate-out.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bold-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bold-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bonfire.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bonfire.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/book-lock.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/book-lock.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/book-stack.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/book-stack.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/book.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/book.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bookmark-book.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bookmark-book.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bookmark-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bookmark-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-bl.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-bl.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-bottom.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-bottom.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-br.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-br.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-inner.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-inner.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-out.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-out.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-tl.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-tl.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-top.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-top.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/border-tr.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/border-tr.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bowling-ball.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bowling-ball.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/box-3d-center.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/box-3d-center.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/box-3d-point.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/box-3d-point.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/box-3d-three-points.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/box-3d-three-points.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/box-iso.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/box-iso.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/boxing-glove.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/boxing-glove.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/brain-electricity.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/brain-electricity.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/brain-research.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/brain-research.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/brain-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/brain-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/brain.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/brain.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bread-slice.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bread-slice.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bridge-3d.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bridge-3d.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bridge-surface.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bridge-surface.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bright-crown.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bright-crown.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bright-star.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bright-star.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/brightness-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/brightness-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/brightness.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/brightness.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-download.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-download.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-income.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-income.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-outcome.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-outcome.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-search.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-search.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-star.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-star.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-upload.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-upload.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bubble-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bubble-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/building.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/building.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bus-green.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bus-green.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bus-stop.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bus-stop.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/bus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/bus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/c-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/c-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/calculator.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/calculator.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/calendar-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/calendar-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/calendar-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/calendar-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/calendar.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/calendar.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/camera.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/camera.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/candlestick-chart.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/candlestick-chart.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/car.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/car.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/card-lock.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/card-lock.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/card-no-access.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/card-no-access.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/card-shield.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/card-shield.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/card-wallet.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/card-wallet.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cart-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cart-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cart-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cart-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cart-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cart-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cart.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cart.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cell-2x2.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cell-2x2.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cellar.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cellar.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/center-align.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/center-align.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-bubble-question.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-bubble-question.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-bubble-translate.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-bubble-translate.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-bubble-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-bubble-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-bubble-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-bubble-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-bubble.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-bubble.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/chat-lines.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/chat-lines.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/chocolate.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/chocolate.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/chromecast-active.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/chromecast-active.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/chromecast.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/chromecast.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/church-side.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/church-side.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/church.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/church.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cigarette-slash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cigarette-slash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cinema-old.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cinema-old.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/city.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/city.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/clipboard-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/clipboard-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/clock-rotate-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/clock-rotate-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/closed-captions-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/closed-captions-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/closet.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/closet.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-desync.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-desync.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-sunny.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-sunny.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cloud-sync.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cloud-sync.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/code-brackets-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/code-brackets-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/code-brackets.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/code-brackets.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/codepen.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/codepen.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/coffee-cup.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/coffee-cup.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/coin-slash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/coin-slash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/coins-swap.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/coins-swap.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/coins.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/coins.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/collapse.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/collapse.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/color-filter.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/color-filter.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/color-picker.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/color-picker.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/color-wheel.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/color-wheel.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/combine.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/combine.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/commodity.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/commodity.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/community.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/community.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/compact-disc.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/compact-disc.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/component.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/component.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/compress-lines.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/compress-lines.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/constrained-surface.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/constrained-surface.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/consumable.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/consumable.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/contactless.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/contactless.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cookie.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cookie.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/copy.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/copy.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/copyright.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/copyright.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/corner-bottom-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/corner-bottom-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/corner-bottom-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/corner-bottom-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/corner-top-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/corner-top-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/corner-top-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/corner-top-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cpu-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cpu-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cpu.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cpu.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/creative-commons.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/creative-commons.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/credit-card-slash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/credit-card-slash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/credit-cards.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/credit-cards.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/crib.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/crib.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/crop-rotate-bl.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/crop-rotate-bl.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/crop-rotate-br.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/crop-rotate-br.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/crop-rotate-tl.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/crop-rotate-tl.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/crop-rotate-tr.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/crop-rotate-tr.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cube-bandage.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cube-bandage.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cube-cut-with-curve.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cube-cut-with-curve.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cube-hole.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cube-hole.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cube-replace-face.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cube-replace-face.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cube.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cube.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/curve-array.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/curve-array.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cut.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cut.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cutlery.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cutlery.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/cycling.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/cycling.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dashboard-dots.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dashboard-dots.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dashboard-speed.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dashboard-speed.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dashboard.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dashboard.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/data-transfer-down.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/data-transfer-down.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/data-transfer-up.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/data-transfer-up.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/data-transfer-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/data-transfer-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-backup.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-backup.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-export.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-export.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-monitor.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-monitor.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-restore.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-restore.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-script-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-script-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-script-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-script-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-search.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-search.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-settings.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-settings.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-star.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-star.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-stats.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-stats.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/database-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/database-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/delivery-truck.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/delivery-truck.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/depth.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/depth.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/design-nib.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/design-nib.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/design-pencil.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/design-pencil.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/desk.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/desk.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/developer.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/developer.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dew-point.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dew-point.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dialpad.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dialpad.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dice-five.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dice-five.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dice-four.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dice-four.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dice-one.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dice-one.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dice-six.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dice-six.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dice-three.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dice-three.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dice-two.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dice-two.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dimmer-switch.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dimmer-switch.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/director-chair.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/director-chair.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/discord.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/discord.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dishwasher.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dishwasher.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/display-4k.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/display-4k.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/divide-three.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/divide-three.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/divide.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/divide.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dna.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dna.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dns.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dns.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/doc-magnifying-glass-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/doc-magnifying-glass-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/doc-magnifying-glass.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/doc-magnifying-glass.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/doc-star-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/doc-star-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/doc-star.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/doc-star.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dogecoin-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dogecoin-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dogecoin-rotate-out.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dogecoin-rotate-out.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dollar-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dollar-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/domotic-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/domotic-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/donate.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/donate.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/download-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/download-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/download-data-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/download-data-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/download-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/download-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/drag-hand-gesture.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/drag-hand-gesture.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/drag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/drag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/drawer.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/drawer.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/dribbble.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/dribbble.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-charge-full.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-charge-full.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-charge-half.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-charge-half.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-charge-low.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-charge-low.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-landing.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-landing.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-refresh.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-refresh.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-take-off.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-take-off.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/drone.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/drone.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/droplet-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/droplet-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ease-curve-control-points.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ease-curve-control-points.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ease-in-control-point.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ease-in-control-point.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ecology-book.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ecology-book.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/edit-pencil.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/edit-pencil.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/edit.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/edit.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/eject.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/eject.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/electronics-chip.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/electronics-chip.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/elevator.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/elevator.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ellipse-3d-three-points.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ellipse-3d-three-points.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ellipse-3d.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ellipse-3d.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-blink-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-blink-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-blink-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-blink-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-look-down.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-look-down.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-look-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-look-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-look-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-look-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-look-up.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-look-up.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-puzzled.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-puzzled.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-quite.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-quite.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-sad.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-sad.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-sing-left-note.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-sing-left-note.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-sing-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-sing-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-sing-right-note.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-sing-right-note.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-sing-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-sing-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-surprise-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-surprise-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-surprise.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-surprise.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-think-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-think-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji-think-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji-think-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/emoji.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/emoji.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/empty-page.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/empty-page.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/energy-usage-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/energy-usage-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/erase.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/erase.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ethereum-rotate-out.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ethereum-rotate-out.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/euro-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/euro-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/euro.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/euro.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-charge-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-charge-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-charge.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-charge.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-plug-charging.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-plug-charging.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-plug-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-plug-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-plug.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-plug.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-station.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-station.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ev-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ev-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/exclude.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/exclude.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/expand-lines.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/expand-lines.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/expand.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/expand.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/extrude.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/extrude.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/eye-closed.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/eye-closed.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/f-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/f-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/face-3d-draft.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/face-3d-draft.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/face-id.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/face-id.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/facebook-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/facebook-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/facetime.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/facetime.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/farm.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/farm.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-arrow-down-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-arrow-down-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-arrow-left-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-arrow-left-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-arrow-right-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-arrow-right-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-arrow-up-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-arrow-up-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-down-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-down-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-left-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-left-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-right-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-right-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fast-up-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fast-up-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/favourite-book.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/favourite-book.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/favourite-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/favourite-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/figma.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/figma.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/file-not-found.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/file-not-found.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fill-color.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fill-color.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fillet-3d.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fillet-3d.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/filter-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/filter-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/filter-list-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/filter-list-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/filter.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/filter.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/finder.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/finder.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-check-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-check-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-lock-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-lock-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-scan.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-scan.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint-xmark-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint-xmark-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fingerprint.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fish.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fish.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/flare.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/flare.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/flask.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/flask.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/flip-reverse.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/flip-reverse.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/flip.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/flip.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/floppy-disk-arrow-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/floppy-disk-arrow-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/floppy-disk-arrow-out.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/floppy-disk-arrow-out.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/floppy-disk.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/floppy-disk.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/flower.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/flower.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fog.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fog.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/folder-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/folder-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/folder-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/folder-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/folder-settings.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/folder-settings.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/folder-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/folder-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/font-question.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/font-question.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/football-ball.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/football-ball.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/football.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/football.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/forward-15-seconds.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/forward-15-seconds.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/forward-message.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/forward-message.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/forward.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/forward.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame-minus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame-minus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame-plus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame-plus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame-select.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame-select.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame-simple.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame-simple.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/frame.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/frame.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fridge.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fridge.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/fx-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/fx-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/gamepad.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/gamepad.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/gas-tank-droplet.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/gas-tank-droplet.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/gas-tank.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/gas-tank.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/gif-format.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/gif-format.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/gift.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/gift.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-branch.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-branch.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-cherry-pick-commit.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-cherry-pick-commit.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-compare.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-compare.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-fork.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-fork.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-merge.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-merge.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-pull-request-closed.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-pull-request-closed.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/git-pull-request.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/git-pull-request.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/github-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/github-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/github.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/github.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/gitlab-full.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/gitlab-full.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/glass-empty.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/glass-empty.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/glass-fragile.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/glass-fragile.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/glass-half-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/glass-half-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/glass-half.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/glass-half.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/glasses.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/glasses.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/globe.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/globe.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/golf.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/golf.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-docs.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-docs.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-drive-sync.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-drive-sync.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-drive-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-drive-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-home.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-home.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/google-one.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/google-one.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/google.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/google.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/gps.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/gps.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/graduation-cap.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/graduation-cap.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/grid-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/grid-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/grid-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/grid-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/grid-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/grid-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/group.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/group.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/gym.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/gym.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/half-cookie.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/half-cookie.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hammer.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hammer.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hand-brake.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hand-brake.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hand-card.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hand-card.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hand-cash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hand-cash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hand-contactless.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hand-contactless.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hard-drive.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hard-drive.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hd-display.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hd-display.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hdr.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hdr.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/headset-bolt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/headset-bolt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/headset-help.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/headset-help.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/headset-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/headset-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/headset.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/headset.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/health-shield.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/health-shield.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/healthcare.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/healthcare.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/heart-arrow-down.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/heart-arrow-down.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/heart.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/heart.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/heating-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/heating-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/heavy-rain.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/heavy-rain.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/help-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/help-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/help-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/help-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/heptagon.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/heptagon.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hexagon-dice.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hexagon-dice.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hexagon-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hexagon-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hexagon.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hexagon.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/historic-shield-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/historic-shield-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-alt-slim-horiz.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-alt-slim-horiz.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-alt-slim.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-alt-slim.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-hospital.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-hospital.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-sale.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-sale.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-secure.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-secure.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-shield.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-shield.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-simple-door.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-simple-door.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-simple.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-simple.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-temperature-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-temperature-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-temperature-out.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-temperature-out.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/home-user.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/home-user.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/horizontal-merge.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/horizontal-merge.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/horizontal-split.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/horizontal-split.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hospital.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hospital.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hot-air-balloon.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hot-air-balloon.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/hourglass.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/hourglass.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/house-rooms.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/house-rooms.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ice-cream.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ice-cream.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/iconoir.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/iconoir.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/industry.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/industry.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/infinite.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/infinite.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/info-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/info-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/input-search.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/input-search.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/instagram.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/instagram.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/internet.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/internet.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/intersect-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/intersect-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/intersect.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/intersect.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ios-settings.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ios-settings.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ip-address-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ip-address-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/iris-scan.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/iris-scan.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/jellyfish.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/jellyfish.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/journal-page.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/journal-page.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/journal.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/journal.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/jpeg-format.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/jpeg-format.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/jpg-format.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/jpg-format.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/kanban-board.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/kanban-board.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/key-command.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/key-command.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/key-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/key-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/key-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/key-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/key-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/key-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-align-center.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-align-center.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-align-horizontal.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-align-horizontal.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-align-vertical.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-align-vertical.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-minus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-minus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-plus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-plus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframe-position.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframe-position.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframes-couple.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframes-couple.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframes-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframes-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframes-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframes-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/keyframes.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/keyframes.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/language.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/language.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/laptop-charging.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/laptop-charging.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/laptop-dev-mode.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/laptop-dev-mode.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/laptop-fix.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/laptop-fix.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/laptop-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/laptop-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/leaderboard-star.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/leaderboard-star.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/leaderboard.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/leaderboard.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/leaf.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/leaf.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/learning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/learning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/lens-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/lens-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/lens.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/lens.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/lifebelt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/lifebelt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/light-bulb-off.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/light-bulb-off.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/light-bulb-on.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/light-bulb-on.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/light-bulb.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/light-bulb.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/line-space.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/line-space.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/link-slash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/link-slash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/link-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/link-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/link.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/link.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/linkedin.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/linkedin.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/linux.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/linux.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/list-select.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/list-select.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/list.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/list.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/litecoin-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/litecoin-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/litecoin-rotate-out.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/litecoin-rotate-out.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/lock-slash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/lock-slash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/lock-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/lock-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/log-no-access.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/log-no-access.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/lot-of-cash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/lot-of-cash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/lullaby.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/lullaby.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/mac-dock.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/mac-dock.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/mac-option-key.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/mac-option-key.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/mac-os-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/mac-os-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/magic-wand.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/magic-wand.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/magnet-energy.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/magnet-energy.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/magnet.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/magnet.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/map-pin-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/map-pin-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/map-pin-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/map-pin-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/map-pin-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/map-pin-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/map-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/map-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/maps-arrow-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/maps-arrow-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/maps-go-straight.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/maps-go-straight.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/maps-turn-back.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/maps-turn-back.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/maps-turn-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/maps-turn-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/maps-turn-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/maps-turn-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/mask-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/mask-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/mastercard-card.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/mastercard-card.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/mastodon.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/mastodon.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/math-book.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/math-book.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-image-folder.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-image-folder.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-image-list.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-image-list.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-image-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-image-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-image-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-image-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-image.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-image.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-video-folder.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-video-folder.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-video-list.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-video-list.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-video-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-video-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-video-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-video-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/media-video.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/media-video.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/medium.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/medium.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/megaphone.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/megaphone.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/message-alert.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/message-alert.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/message-text.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/message-text.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/meter-arrow-down-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/meter-arrow-down-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/metro.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/metro.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone-mute.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone-mute.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone-speaking.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone-speaking.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/microphone-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/microphone-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/microscope.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/microscope.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/minus-hexagon.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/minus-hexagon.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/minus-square-dashed.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/minus-square-dashed.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/mirror.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/mirror.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/mobile-dev-mode.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/mobile-dev-mode.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/mobile-fingerprint.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/mobile-fingerprint.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/mobile-voice.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/mobile-voice.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/modern-tv-4k.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/modern-tv-4k.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/money-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/money-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/moon-sat.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/moon-sat.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/more-horiz-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/more-horiz-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/more-horiz.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/more-horiz.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/more-vert-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/more-vert-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/more-vert.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/more-vert.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/motorcycle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/motorcycle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/mouse-scroll-wheel.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/mouse-scroll-wheel.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/movie.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/movie.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/mpeg-format.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/mpeg-format.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/multi-bubble.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/multi-bubble.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/multi-mac-os-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/multi-mac-os-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/multi-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/multi-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/multiple-pages-empty.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/multiple-pages-empty.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/multiple-pages-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/multiple-pages-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/multiple-pages-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/multiple-pages-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/multiple-pages-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/multiple-pages-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/multiple-pages.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/multiple-pages.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/music-double-note-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/music-double-note-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/music-double-note.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/music-double-note.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/neighbourhood.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/neighbourhood.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/network-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/network-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/network-reverse.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/network-reverse.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/network-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/network-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/network.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/network.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/nintendo-switch.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/nintendo-switch.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/no-smoking-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/no-smoking-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/notes.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/notes.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/npm-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/npm-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/npm.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/npm.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-2-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-2-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-3-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-3-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-6-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-6-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-8-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-8-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/number-9-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/number-9-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/numbered-list-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/numbered-list-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/numbered-list-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/numbered-list-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/o-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/o-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/octagon.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/octagon.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/off-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/off-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/oil-industry.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/oil-industry.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/okrs.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/okrs.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/on-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/on-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/one-finger-select-hand-gesture.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/one-finger-select-hand-gesture.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/one-point-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/one-point-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/open-book.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/open-book.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/open-in-browser.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/open-in-browser.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/open-select-hand-gesture.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/open-select-hand-gesture.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/open-vpn.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/open-vpn.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/organic-food-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/organic-food-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/organic-food.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/organic-food.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/orthogonal-view.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/orthogonal-view.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/package-lock.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/package-lock.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/packages.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/packages.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pacman.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pacman.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-edit.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-edit.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-flip.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-flip.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-minus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-minus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-plus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-plus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-search.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-search.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/page-star.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/page-star.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/page.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/page.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/palette.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/palette.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/panorama-enlarge.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/panorama-enlarge.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/panorama-reduce.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/panorama-reduce.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pants-pockets.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pants-pockets.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/password-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/password-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/password-cursor.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/password-cursor.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/password-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/password-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/paste-clipboard.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/paste-clipboard.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/path-arrow.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/path-arrow.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pause-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pause-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pc-firewall.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pc-firewall.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pc-no-entry.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pc-no-entry.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pc-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pc-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/peace-hand.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/peace-hand.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/peerlist.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/peerlist.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pen-connect-bluetooth.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pen-connect-bluetooth.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pen-connect-wifi.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pen-connect-wifi.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pen-tablet-connect-usb.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pen-tablet-connect-usb.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pen-tablet-connect-wifi.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pen-tablet-connect-wifi.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pen-tablet.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pen-tablet.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pentagon.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pentagon.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/people-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/people-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/percent-rotate-out.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/percent-rotate-out.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/percentage-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/percentage-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/percentage-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/percentage-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/percentage.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/percentage.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/perspective-view.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/perspective-view.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pharmacy-cross-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pharmacy-cross-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pharmacy-cross-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pharmacy-cross-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-disabled.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-disabled.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-income.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-income.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-outcome.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-outcome.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-paused.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-paused.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/phone-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/phone-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/piggy-bank.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/piggy-bank.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pillow.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pillow.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pin-slash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pin-slash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pine-tree.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pine-tree.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pinterest.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pinterest.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pipe-3d.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pipe-3d.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pizza-slice.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pizza-slice.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/planet-sat.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/planet-sat.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/planimetry.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/planimetry.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/playlist-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/playlist-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/playlist.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/playlist.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/playstation-gamepad.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/playstation-gamepad.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/plug-type-c.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/plug-type-c.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/plug-type-g.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/plug-type-g.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/plug-type-l.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/plug-type-l.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/plus-square-dashed.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/plus-square-dashed.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/png-format.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/png-format.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/podcast.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/podcast.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pokeball.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pokeball.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/polar-sh.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/polar-sh.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/position-align.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/position-align.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/position.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/position.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/post.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/post.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/potion.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/potion.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/pound.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/pound.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/precision-tool.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/precision-tool.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/presentation.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/presentation.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/printer.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/printer.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/printing-page.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/printing-page.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/priority-down.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/priority-down.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/priority-high.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/priority-high.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/priority-medium.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/priority-medium.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/priority-up.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/priority-up.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/privacy-policy.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/privacy-policy.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/private-wifi.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/private-wifi.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/profile-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/profile-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/project-curve-3d.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/project-curve-3d.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/puzzle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/puzzle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/qr-code.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/qr-code.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/quote-message.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/quote-message.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/radiation.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/radiation.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/radius.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/radius.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/rain.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/rain.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/raw-format.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/raw-format.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/receive-dollars.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/receive-dollars.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/receive-euros.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/receive-euros.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/receive-pounds.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/receive-pounds.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/receive-yens.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/receive-yens.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/redo-action.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/redo-action.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/redo-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/redo-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/refresh-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/refresh-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/refresh-double.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/refresh-double.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/reload-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/reload-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/reminder-hand-gesture.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/reminder-hand-gesture.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/repeat-once.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/repeat-once.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/reply-to-message.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/reply-to-message.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/report-columns.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/report-columns.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/repository.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/repository.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/restart.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/restart.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/rewind.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/rewind.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/rhombus-arrow-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/rhombus-arrow-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/rings.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/rings.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/rocket.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/rocket.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/rook.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/rook.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/rotate-camera-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/rotate-camera-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/rotate-camera-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/rotate-camera-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/round-flask.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/round-flask.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/rounded-mirror.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/rounded-mirror.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/rss-feed-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/rss-feed-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/rubik-cube.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/rubik-cube.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ruler-arrows.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ruler-arrows.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/ruler-combine.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/ruler-combine.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/running.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/running.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/safari.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/safari.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/safe-arrow-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/safe-arrow-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/safe-arrow-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/safe-arrow-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/safe-open.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/safe-open.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/safe.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/safe.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sandals.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sandals.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/scale-frame-enlarge.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/scale-frame-enlarge.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/scale-frame-reduce.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/scale-frame-reduce.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/scan-barcode.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/scan-barcode.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/scan-qr-code.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/scan-qr-code.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/scanning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/scanning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/scarf.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/scarf.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/scissor-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/scissor-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/scissor.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/scissor.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/screenshot.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/screenshot.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sea-and-sun.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sea-and-sun.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sea-waves.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sea-waves.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/search-engine.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/search-engine.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/search-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/search-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/secure-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/secure-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/select-edge-3d.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/select-edge-3d.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/select-face-3d.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/select-face-3d.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/select-point-3d.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/select-point-3d.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/select-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/select-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/selective-tool.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/selective-tool.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/send-dollars.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/send-dollars.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/send-euros.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/send-euros.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/send-mail.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/send-mail.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/send-pounds.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/send-pounds.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/send-yens.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/send-yens.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/server.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/server.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/settings-profiles.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/settings-profiles.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/settings.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/settings.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/share-android.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/share-android.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-alert.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-alert.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-broken.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-broken.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-download.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-download.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-eye.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-eye.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-loading.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-loading.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-plus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-plus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-question.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-question.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-search.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-search.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-upload.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-upload.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shield-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shield-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shirt-tank-top.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shirt-tank-top.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shirt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shirt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shop-four-tiles-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shop-four-tiles-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shop-four-tiles.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shop-four-tiles.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shop-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shop-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shop.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shop.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-arrow-down.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-arrow-down.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-arrow-up.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-pocket.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-pocket.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-bag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-bag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-code-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-code-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-code-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-code-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shopping-code.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shopping-code.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/short-pants-pockets.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/short-pants-pockets.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shortcut-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shortcut-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/shuffle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/shuffle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sidebar-collapse.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sidebar-collapse.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sidebar-expand.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sidebar-expand.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/simple-cart.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/simple-cart.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sine-wave.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sine-wave.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/skateboard.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/skateboard.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/skateboarding.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/skateboarding.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sleeper-chair.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sleeper-chair.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/slips.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/slips.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/small-lamp-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/small-lamp-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/small-lamp.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/small-lamp.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/smoking.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/smoking.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/snapchat.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/snapchat.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/snow.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/snow.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/soccer-ball.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/soccer-ball.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sofa.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sofa.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/soil-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/soil-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/soil.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/soil.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sort-down.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sort-down.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sort-up.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sort-up.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sort.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sort.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sound-high.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sound-high.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sound-low.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sound-low.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sound-min.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sound-min.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sound-off.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sound-off.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/spades.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/spades.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/spiral.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/spiral.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/split-area.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/split-area.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/split-square-dashed.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/split-square-dashed.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/spock-hand-gesture.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/spock-hand-gesture.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/spotify.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/spotify.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/square-3d-corner-to-corner.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/square-3d-corner-to-corner.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/square-3d-from-center.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/square-3d-from-center.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/square-3d-three-points.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/square-3d-three-points.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/square-cursor.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/square-cursor.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/square-dashed.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/square-dashed.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/stackoverflow.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/stackoverflow.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/star-dashed.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/star-dashed.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/star-half-dashed.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/star-half-dashed.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/star.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/star.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/stats-down-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/stats-down-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/stats-report.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/stats-report.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/stats-up-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/stats-up-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/strategy.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/strategy.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/stretching.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/stretching.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/stroller.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/stroller.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/style-border.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/style-border.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/submit-document.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/submit-document.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/substract.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/substract.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/suggestion.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/suggestion.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sun-light.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sun-light.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/svg-format.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/svg-format.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/sweep-3d.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/sweep-3d.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/swimming.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/swimming.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/swipe-two-fingers-down-gesture.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/swipe-two-fingers-down-gesture.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/swipe-two-fingers-left-gesture.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/swipe-two-fingers-left-gesture.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/swipe-two-fingers-right-gesture.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/swipe-two-fingers-right-gesture.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/swipe-two-fingers-up-gesture.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/swipe-two-fingers-up-gesture.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/switch-on.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/switch-on.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/system-restart.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/system-restart.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/table-2-columns.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/table-2-columns.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/table.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/table.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/task-list.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/task-list.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/temperature-down.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/temperature-down.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/temperature-high.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/temperature-high.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/temperature-low.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/temperature-low.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/temperature-up.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/temperature-up.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tennis-ball-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tennis-ball-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tennis-ball.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tennis-ball.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/terminal-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/terminal-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/test-tube.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/test-tube.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/text-box.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/text-box.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/text-magnifying-glass.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/text-magnifying-glass.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/text-size.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/text-size.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/text-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/text-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/three-points-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/three-points-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/three-stars.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/three-stars.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/thumbs-down.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/thumbs-down.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/thumbs-up.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/thumbs-up.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tif-format.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tif-format.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tiff-format.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tiff-format.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tiktok.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tiktok.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/time-zone.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/time-zone.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/timer-off.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/timer-off.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tools.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tools.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tournament.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tournament.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tower-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tower-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tower-no-access.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tower-no-access.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tower-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tower-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tower.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tower.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/trademark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/trademark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/train.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/train.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tram.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tram.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/transition-down.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/transition-down.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/transition-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/transition-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/transition-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/transition-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/transition-up.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/transition-up.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/translate.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/translate.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/trash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/trash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/treadmill.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/treadmill.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tree.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tree.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/trekking.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/trekking.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/trello.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/trello.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/trophy.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/trophy.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/truck-green.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/truck-green.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/truck-length.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/truck-length.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/truck.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/truck.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tunnel.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tunnel.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tv-fix.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tv-fix.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/tv-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/tv-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/twitter.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/twitter.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/two-points-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/two-points-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/two-seater-sofa.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/two-seater-sofa.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/type.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/type.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/umbrella.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/umbrella.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/underline-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/underline-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/undo-action.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/undo-action.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/undo-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/undo-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/unity-5.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/unity-5.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/unjoin-3d.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/unjoin-3d.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/upload-data-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/upload-data-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/upload-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/upload-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/usb.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/usb.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-badge-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-badge-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-bag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-bag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-cart.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-cart.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-crown.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-crown.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-love.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-love.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-scan.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-scan.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-star.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-star.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/user-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/user-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/vegan-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/vegan-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/vegan-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/vegan-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/vegan.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/vegan.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/vehicle-green.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/vehicle-green.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/vertical-merge.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/vertical-merge.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/vertical-split.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/vertical-split.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/vials.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/vials.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/video-camera-off.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/video-camera-off.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/video-projector.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/video-projector.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/view-360.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/view-360.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/view-grid.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/view-grid.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/view-structure-down.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/view-structure-down.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/view-structure-up.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/view-structure-up.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice-lock-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice-lock-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice-scan.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice-scan.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/voice.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/voice.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/vr-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/vr-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/waist.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/waist.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/walking.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/walking.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/wallet.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/wallet.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/warning-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/warning-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/warning-hexagon.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/warning-hexagon.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/warning-triangle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/warning-triangle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/warning-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/warning-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/washing-machine.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/washing-machine.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/watering-soil.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/watering-soil.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/web-window-energy-consumption.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/web-window-energy-consumption.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/web-window-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/web-window-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/webp-format.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/webp-format.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/weight-alt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/weight-alt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/weight.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/weight.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/wifi-off.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/wifi-off.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/wifi-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/wifi-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/wifi-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/wifi-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/wifi-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/wifi-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/wifi.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/wifi.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/wind.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/wind.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/window-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/window-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/window-lock.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/window-lock.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/window-no-access.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/window-no-access.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/window-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/window-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/wolf.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/wolf.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/wrap-text.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/wrap-text.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/wrench.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/wrench.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/wristwatch.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/wristwatch.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/www.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/www.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/x-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/x-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/xbox-a.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/xbox-a.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/xbox-b.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/xbox-b.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/xmark-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/xmark-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/xray-view.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/xray-view.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/y-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/y-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/yelp.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/yelp.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/yen-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/yen-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/yoga.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/yoga.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/youtube.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/youtube.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/zoom-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/zoom-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/regular/zoom-out.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/regular/zoom-out.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/adobe-after-effects.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/adobe-after-effects.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/adobe-illustrator.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/adobe-illustrator.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/adobe-indesign.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/adobe-indesign.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/adobe-lightroom.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/adobe-lightroom.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/adobe-photoshop.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/adobe-photoshop.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/adobe-xd.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/adobe-xd.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/alarm.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/alarm.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-bottom-box.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-bottom-box.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-horizontal-spacing.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-horizontal-spacing.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-left-box.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-left-box.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-right-box.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-right-box.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-top-box.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-top-box.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/align-vertical-spacing.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/align-vertical-spacing.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/app-notification.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/app-notification.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/app-store.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/app-store.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/apple-shortcuts.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/apple-shortcuts.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-down-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-down-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-down-left-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-down-left-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-down-right-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-down-right-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-down-right-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-down-right-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-left-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-left-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-right-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-right-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-up-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-up-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-up-left-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-up-left-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-up-left-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-up-left-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-up-right-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-up-right-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/arrow-up-right-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/arrow-up-right-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/bathroom.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/bathroom.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/bitcoin-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/bitcoin-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/bluetooth-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/bluetooth-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/bold-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/bold-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/book.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/book.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/bookmark-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/bookmark-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/bubble-search.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/bubble-search.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/bubble-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/bubble-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/cable-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/cable-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/camera.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/camera.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/cash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/cash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/center-align.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/center-align.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble-question.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble-question.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble-translate.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble-translate.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-bubble.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-bubble.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-lines.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-lines.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-minus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-minus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/chat-plus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/chat-plus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/check-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/check-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/check-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/check-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/clock.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/clock.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/closed-captions-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/closed-captions-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/cloud-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/cloud-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/component.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/component.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/database-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/database-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/database-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/database-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/database-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/database-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/database.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/database.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/design-nib.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/design-nib.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/dogecoin-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/dogecoin-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/dollar-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/dollar-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/download-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/download-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/download-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/download-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/erase.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/erase.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/ethereum-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/ethereum-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/euro-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/euro-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/facetime.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/facetime.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/fill-color.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/fill-color.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/filter.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/filter.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/flash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/flash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/forward.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/forward.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/frame-tool.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/frame-tool.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/fx-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/fx-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/hd-display.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/hd-display.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/headset-bolt.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/headset-bolt.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/headset-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/headset-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/headset.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/headset.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/heart.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/heart.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/help-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/help-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/help-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/help-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/horiz-distribution-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/horiz-distribution-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/horiz-distribution-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/horiz-distribution-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/hospital-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/hospital-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/ice-cream.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/ice-cream.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/info-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/info-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/italic-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/italic-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-align-center.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-align-center.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-align-horizontal.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-align-horizontal.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-align-vertical.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-align-vertical.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-minus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-minus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-plus-in.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-plus-in.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframe-position.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframe-position.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframes-couple.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframes-couple.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/keyframes.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/keyframes.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/litecoin-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/litecoin-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/mail-open.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/mail-open.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/mail.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/mail.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/medal-1st.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/medal-1st.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/medal.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/medal.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/message-alert.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/message-alert.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/message-text.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/message-text.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone-check.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone-check.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone-minus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone-minus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone-mute.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone-mute.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone-speaking.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone-speaking.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/microphone-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/microphone-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/minus-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/minus-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/money-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/money-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/multi-bubble.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/multi-bubble.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/music-note-plus.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/music-note-plus.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/network-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/network-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/network-reverse.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/network-reverse.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/network-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/network-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/network.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/network.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-0-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-0-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-1-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-1-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-2-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-2-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-3-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-3-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-4-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-4-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-5-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-5-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-6-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-6-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-7-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-7-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-8-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-8-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/number-9-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/number-9-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/pause.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/pause.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/percentage-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/percentage-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/percentage-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/percentage-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/pin-slash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/pin-slash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/plus-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/plus-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/plus-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/plus-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/podcast.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/podcast.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/post.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/post.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/presentation.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/presentation.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/priority-down.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/priority-down.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/priority-high.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/priority-high.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/priority-medium.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/priority-medium.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/priority-up.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/priority-up.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/quote-message.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/quote-message.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/quote.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/quote.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/redo-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/redo-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/refresh-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/refresh-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/rewind.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/rewind.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/rhombus-arrow-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/rhombus-arrow-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/send-diagonal.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/send-diagonal.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/send.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/send.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/server-connection.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/server-connection.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/server.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/server.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/share-android.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/share-android.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/skip-next.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/skip-next.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/skip-prev.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/skip-prev.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/sound-high.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/sound-high.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/sound-low.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/sound-low.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/sound-min.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/sound-min.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/sound-off.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/sound-off.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/sparks.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/sparks.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/square-cursor.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/square-cursor.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/star.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/star.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/stats-down-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/stats-down-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/stats-up-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/stats-up-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/style-border.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/style-border.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/text-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/text-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/three-stars.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/three-stars.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/timer.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/timer.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/transition-down.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/transition-down.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/transition-left.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/transition-left.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/transition-right.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/transition-right.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/transition-up.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/transition-up.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/trash.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/trash.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/underline-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/underline-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/undo-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/undo-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/upload-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/upload-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/usb.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/usb.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/wallet.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/wallet.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/warning-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/warning-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/warning-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/warning-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/warning-triangle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/warning-triangle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/web-window-energy-consumption.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/web-window-energy-consumption.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/web-window-xmark.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/web-window-xmark.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/web-window.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/web-window.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/white-flag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/white-flag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/wifi-signal-none.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/wifi-signal-none.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/wifi-tag.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/wifi-tag.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/wifi-warning.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/wifi-warning.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/window-tabs.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/window-tabs.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/xmark-circle.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/xmark-circle.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/xmark-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/xmark-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/flet_iconoir/icons/solid/yen-square.svg` & `flet_iconoir-0.3.0/flet_iconoir/icons/solid/yen-square.svg`

 * *Files identical despite different names*

### Comparing `flet_iconoir-0.2.2/PKG-INFO` & `flet_iconoir-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-iconoir
-Version: 0.2.2
+Version: 0.3.0
 Summary: the Iconoir library, wrapped for Flet.
 License: MIT
 Author: hex benjamin
 Author-email: hex@hexbenjam.in
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,16 +22,35 @@
 adds a new `IconoirIcon` function. use it like this with a name from the [Iconoir](https://iconoir.com/) list!
 
 ```python
 page.add(
     IconoirIcon(
         icon_name="wifi",
         icon_set="regular",  # or "solid" !
-        icon_size=32,  # default
         icon_color=ft.colors.PRIMARY,  # default
         **kwargs,  # passed to the flet.Image this thing returns!
     )
 )
 ```
 
+also adds the `IconoirIconButton`, which is a class with more parameters.
+
+```python
+page.add(
+    IconoirIconButton(
+        page=page,  # reference to the page this button will be on
+        icon_name="settings",
+        icon_set="regular",
+        on_click=lambda: print("clicked!"),  # defaults to None
+        icon_size=16,
+        icon_color=ft.colors.ON_PRIMARY,
+        hover_color=ft.colors.PRIMARY_CONTAINER,
+        bg_color=ft.colors.ON_PRIMARY_CONTAINER,
+        padding=8,
+        circular=True,
+        border_radius=8,  # for when circular is False
+    )
+)
+```
+
 quick, dirty, simple, hopefully helpful. find me on [github](https://github.com/hexbenjamin) and reach out if you have questions. have a day!
```

